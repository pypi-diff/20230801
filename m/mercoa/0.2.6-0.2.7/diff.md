# Comparing `tmp/mercoa-0.2.6.tar.gz` & `tmp/mercoa-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercoa-0.2.6.tar", max compression
+gzip compressed data, was "mercoa-0.2.7.tar", max compression
```

## Comparing `mercoa-0.2.6.tar` & `mercoa-0.2.7.tar`

### file list

```diff
@@ -1,201 +1,215 @@
--rw-r--r--   0        0        0     1930 2023-07-29 18:16:28.144321 mercoa-0.2.6/README.md
--rw-r--r--   0        0        0      368 2023-07-29 18:16:28.144321 mercoa-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     7849 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/__init__.py
--rw-r--r--   0        0        0     2384 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/client.py
--rw-r--r--   0        0        0      348 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/core/__init__.py
--rw-r--r--   0        0        0      426 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      157 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/environment.py
--rw-r--r--   0        0        0        0 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/py.typed
--rw-r--r--   0        0        0     7958 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/__init__.py
--rw-r--r--   0        0        0      165 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/bank_lookup/__init__.py
--rw-r--r--   0        0        0     3801 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/bank_lookup/client.py
--rw-r--r--   0        0        0      205 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/bank_lookup/types/__init__.py
--rw-r--r--   0        0        0      960 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/bank_lookup/types/bank_address.py
--rw-r--r--   0        0        0      946 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py
--rw-r--r--   0        0        0      499 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/commons/__init__.py
--rw-r--r--   0        0        0      314 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/commons/errors/__init__.py
--rw-r--r--   0        0        0      237 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/commons/errors/auth_header_malformed_error.py
--rw-r--r--   0        0        0      221 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/commons/errors/auth_header_missing_error.py
--rw-r--r--   0        0        0      225 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/commons/errors/unauthorized.py
--rw-r--r--   0        0        0      469 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/commons/types/__init__.py
--rw-r--r--   0        0        0     1093 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/commons/types/address.py
--rw-r--r--   0        0        0      824 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/commons/types/birth_date.py
--rw-r--r--   0        0        0      994 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/commons/types/full_name.py
--rw-r--r--   0        0        0      850 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/commons/types/individual_government_id.py
--rw-r--r--   0        0        0      857 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/commons/types/itin.py
--rw-r--r--   0        0        0      441 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/commons/types/order_direction.py
--rw-r--r--   0        0        0      855 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/commons/types/phone_number.py
--rw-r--r--   0        0        0      856 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/commons/types/ssn.py
--rw-r--r--   0        0        0      523 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity/__init__.py
--rw-r--r--   0        0        0    37562 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity/client.py
--rw-r--r--   0        0        0      501 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity/resources/__init__.py
--rw-r--r--   0        0        0      228 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity/resources/approval_policy/__init__.py
--rw-r--r--   0        0        0    17689 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity/resources/approval_policy/client.py
--rw-r--r--   0        0        0      305 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity/resources/approval_policy/errors/__init__.py
--rw-r--r--   0        0        0      242 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity/resources/approval_policy/errors/num_approver_less_than_one_error.py
--rw-r--r--   0        0        0      248 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity/resources/approval_policy/errors/num_approvers_user_list_mismatch_error.py
--rw-r--r--   0        0        0       65 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity/resources/counterparty/__init__.py
--rw-r--r--   0        0        0     4109 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity/resources/counterparty/client.py
--rw-r--r--   0        0        0       65 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity/resources/invoice/__init__.py
--rw-r--r--   0        0        0    11215 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity/resources/invoice/client.py
--rw-r--r--   0        0        0       65 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity/resources/notification_policy/__init__.py
--rw-r--r--   0        0        0    10326 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity/resources/notification_policy/client.py
--rw-r--r--   0        0        0       65 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity/resources/payment_method/__init__.py
--rw-r--r--   0        0        0    22306 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity/resources/payment_method/client.py
--rw-r--r--   0        0        0       65 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity/resources/representative/__init__.py
--rw-r--r--   0        0        0    12767 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity/resources/representative/client.py
--rw-r--r--   0        0        0      175 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity/resources/user/__init__.py
--rw-r--r--   0        0        0    18708 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity/resources/user/client.py
--rw-r--r--   0        0        0      166 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity/resources/user/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity/resources/user/resources/notification_policy/__init__.py
--rw-r--r--   0        0        0    10769 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity/resources/user/resources/notification_policy/client.py
--rw-r--r--   0        0        0       65 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity/resources/user/resources/notifications/__init__.py
--rw-r--r--   0        0        0     8720 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity/resources/user/resources/notifications/client.py
--rw-r--r--   0        0        0     2369 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/__init__.py
--rw-r--r--   0        0        0     3483 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/__init__.py
--rw-r--r--   0        0        0      487 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/account_type.py
--rw-r--r--   0        0        0      849 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/amount_trigger.py
--rw-r--r--   0        0        0       88 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/approval_policy_id.py
--rw-r--r--   0        0        0     1100 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/approval_policy_request.py
--rw-r--r--   0        0        0     1036 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/approval_policy_response.py
--rw-r--r--   0        0        0     1067 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/approval_policy_update_request.py
--rw-r--r--   0        0        0      963 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/approver_rule.py
--rw-r--r--   0        0        0     1451 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/business_profile_request.py
--rw-r--r--   0        0        0     1509 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/business_profile_response.py
--rw-r--r--   0        0        0     1917 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/business_type.py
--rw-r--r--   0        0        0     1013 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/counterparty_response.py
--rw-r--r--   0        0        0      741 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/ein.py
--rw-r--r--   0        0        0      914 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/entity_add_payees_request.py
--rw-r--r--   0        0        0       80 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/entity_id.py
--rw-r--r--   0        0        0     2432 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/entity_request.py
--rw-r--r--   0        0        0     1814 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/entity_response.py
--rw-r--r--   0        0        0     1084 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/entity_status.py
--rw-r--r--   0        0        0     2084 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/entity_update_request.py
--rw-r--r--   0        0        0       84 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/entity_user_id.py
--rw-r--r--   0        0        0     1100 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/entity_user_request.py
--rw-r--r--   0        0        0     1224 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/entity_user_response.py
--rw-r--r--   0        0        0     1446 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/find_counterparties_response.py
--rw-r--r--   0        0        0     1343 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/find_entity_response.py
--rw-r--r--   0        0        0     1367 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/find_notification_response.py
--rw-r--r--   0        0        0      633 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/identifier_list.py
--rw-r--r--   0        0        0     1372 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/individual_profile_request.py
--rw-r--r--   0        0        0     1206 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/individual_profile_response.py
--rw-r--r--   0        0        0       86 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/notification_id.py
--rw-r--r--   0        0        0     1051 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/notification_policy_request.py
--rw-r--r--   0        0        0     1127 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/notification_policy_response.py
--rw-r--r--   0        0        0     1129 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/notification_response.py
--rw-r--r--   0        0        0     1945 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/notification_type.py
--rw-r--r--   0        0        0      974 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/profile_request.py
--rw-r--r--   0        0        0      981 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/profile_response.py
--rw-r--r--   0        0        0       88 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/representative_id.py
--rw-r--r--   0        0        0     1370 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/representative_request.py
--rw-r--r--   0        0        0     1539 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/representative_response.py
--rw-r--r--   0        0        0     1100 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/responsibilities.py
--rw-r--r--   0        0        0      391 2023-07-29 18:16:28.144321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/rule.py
--rw-r--r--   0        0        0      761 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/tax_id.py
--rw-r--r--   0        0        0      573 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/trigger.py
--rw-r--r--   0        0        0      947 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/entity_types/types/user_notification_policy_response.py
--rw-r--r--   0        0        0      163 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/invoice/__init__.py
--rw-r--r--   0        0        0    20874 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/invoice/client.py
--rw-r--r--   0        0        0      154 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/invoice/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/invoice/resources/approval/__init__.py
--rw-r--r--   0        0        0     6559 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/invoice/resources/approval/client.py
--rw-r--r--   0        0        0       65 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/invoice/resources/comment/__init__.py
--rw-r--r--   0        0        0    15332 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/invoice/resources/comment/client.py
--rw-r--r--   0        0        0       65 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/invoice/resources/document/__init__.py
--rw-r--r--   0        0        0     3870 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/invoice/resources/document/client.py
--rw-r--r--   0        0        0      991 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/invoice_types/__init__.py
--rw-r--r--   0        0        0     1480 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/invoice_types/types/__init__.py
--rw-r--r--   0        0        0     1017 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/invoice_types/types/approval_request.py
--rw-r--r--   0        0        0     1592 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/invoice_types/types/approval_slot.py
--rw-r--r--   0        0        0     1147 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/invoice_types/types/approval_slot_assignment.py
--rw-r--r--   0        0        0       86 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/invoice_types/types/approval_slot_id.py
--rw-r--r--   0        0        0      631 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/invoice_types/types/approver_action.py
--rw-r--r--   0        0        0      984 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/invoice_types/types/associated_approval_action.py
--rw-r--r--   0        0        0       81 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/invoice_types/types/comment_id.py
--rw-r--r--   0        0        0      934 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/invoice_types/types/comment_request.py
--rw-r--r--   0        0        0     1428 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/invoice_types/types/comment_response.py
--rw-r--r--   0        0        0      851 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/invoice_types/types/document_response.py
--rw-r--r--   0        0        0     1347 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/invoice_types/types/find_invoice_response.py
--rw-r--r--   0        0        0       81 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/invoice_types/types/invoice_id.py
--rw-r--r--   0        0        0     1331 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/invoice_types/types/invoice_line_item_request.py
--rw-r--r--   0        0        0     1258 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/invoice_types/types/invoice_line_item_response.py
--rw-r--r--   0        0        0     1072 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/invoice_types/types/invoice_metrics_response.py
--rw-r--r--   0        0        0      870 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/invoice_types/types/invoice_order_by_field.py
--rw-r--r--   0        0        0     3578 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/invoice_types/types/invoice_request.py
--rw-r--r--   0        0        0     4306 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/invoice_types/types/invoice_response.py
--rw-r--r--   0        0        0     1485 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/invoice_types/types/invoice_status.py
--rw-r--r--   0        0        0      155 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/ocr/__init__.py
--rw-r--r--   0        0        0     4424 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/ocr/client.py
--rw-r--r--   0        0        0      189 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/ocr/types/__init__.py
--rw-r--r--   0        0        0     1258 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/ocr/types/ocr_response.py
--rw-r--r--   0        0        0      642 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/ocr/types/vendor_network.py
--rw-r--r--   0        0        0      983 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/organization/__init__.py
--rw-r--r--   0        0        0    10870 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/organization/client.py
--rw-r--r--   0        0        0     1466 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/organization/types/__init__.py
--rw-r--r--   0        0        0      948 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/organization/types/color_scheme_request.py
--rw-r--r--   0        0        0      949 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/organization/types/color_scheme_response.py
--rw-r--r--   0        0        0      981 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/organization/types/email_log_response.py
--rw-r--r--   0        0        0      932 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/organization/types/email_provider_request.py
--rw-r--r--   0        0        0      936 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/organization/types/email_provider_response.py
--rw-r--r--   0        0        0      785 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/organization/types/email_sender_provider.py
--rw-r--r--   0        0        0     1052 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/organization/types/email_sender_request.py
--rw-r--r--   0        0        0     1044 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/organization/types/email_sender_response.py
--rw-r--r--   0        0        0       86 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/organization/types/organization_id.py
--rw-r--r--   0        0        0     1463 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/organization/types/organization_request.py
--rw-r--r--   0        0        0     1579 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/organization/types/organization_response.py
--rw-r--r--   0        0        0     1142 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/organization/types/payment_methods_request.py
--rw-r--r--   0        0        0     1148 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/organization/types/payment_methods_response.py
--rw-r--r--   0        0        0      849 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/organization/types/payment_rail_markup.py
--rw-r--r--   0        0        0      482 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/organization/types/payment_rail_markup_type.py
--rw-r--r--   0        0        0     1151 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/organization/types/payment_rail_request.py
--rw-r--r--   0        0        0      843 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/organization/types/payment_rail_response.py
--rw-r--r--   0        0        0       65 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_schema/__init__.py
--rw-r--r--   0        0        0    15390 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_schema/client.py
--rw-r--r--   0        0        0     2547 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/__init__.py
--rw-r--r--   0        0        0     3587 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/__init__.py
--rw-r--r--   0        0        0     1336 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/bank_account_base_request.py
--rw-r--r--   0        0        0     1466 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/bank_account_base_response.py
--rw-r--r--   0        0        0     1026 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/bank_account_request.py
--rw-r--r--   0        0        0     1014 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/bank_account_response.py
--rw-r--r--   0        0        0      960 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/bank_status.py
--rw-r--r--   0        0        0      632 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/bank_type.py
--rw-r--r--   0        0        0     1247 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/card_base_request.py
--rw-r--r--   0        0        0     1468 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/card_base_response.py
--rw-r--r--   0        0        0      819 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/card_brand.py
--rw-r--r--   0        0        0      961 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/card_request.py
--rw-r--r--   0        0        0      935 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/card_response.py
--rw-r--r--   0        0        0      750 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/card_type.py
--rw-r--r--   0        0        0     1258 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/check_base_request.py
--rw-r--r--   0        0        0     1494 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/check_base_response.py
--rw-r--r--   0        0        0      967 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/check_request.py
--rw-r--r--   0        0        0      941 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/check_response.py
--rw-r--r--   0        0        0    22179 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/currency_code.py
--rw-r--r--   0        0        0     1607 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_request.py
--rw-r--r--   0        0        0     2026 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_response.py
--rw-r--r--   0        0        0     1040 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/custom_payment_method_request.py
--rw-r--r--   0        0        0     1028 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/custom_payment_method_response.py
--rw-r--r--   0        0        0     1613 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_base_request.py
--rw-r--r--   0        0        0     1071 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_request.py
--rw-r--r--   0        0        0       87 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/payment_method_id.py
--rw-r--r--   0        0        0     1264 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/payment_method_request.py
--rw-r--r--   0        0        0     1298 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/payment_method_response.py
--rw-r--r--   0        0        0     1984 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/payment_method_schema_field.py
--rw-r--r--   0        0        0      682 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/payment_method_schema_field_type.py
--rw-r--r--   0        0        0       93 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/payment_method_schema_id.py
--rw-r--r--   0        0        0     1581 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/payment_method_schema_request.py
--rw-r--r--   0        0        0     1693 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/payment_method_schema_response.py
--rw-r--r--   0        0        0     1229 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/payment_method_type.py
--rw-r--r--   0        0        0      514 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/payment_method_update_request.py
--rw-r--r--   0        0        0     1042 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/plaid_link_request.py
--rw-r--r--   0        0        0      271 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/transaction/__init__.py
--rw-r--r--   0        0        0     6642 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/transaction/client.py
--rw-r--r--   0        0        0      386 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/transaction/types/__init__.py
--rw-r--r--   0        0        0       85 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/transaction/types/transaction_id.py
--rw-r--r--   0        0        0     1138 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/transaction/types/transaction_response.py
--rw-r--r--   0        0        0     1582 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/transaction/types/transaction_response_expanded.py
--rw-r--r--   0        0        0     1261 2023-07-29 18:16:28.148321 mercoa-0.2.6/src/mercoa/resources/transaction/types/transaction_status.py
--rw-r--r--   0        0        0     2433 1970-01-01 00:00:00.000000 mercoa-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1930 2023-08-01 00:16:04.691748 mercoa-0.2.7/README.md
+-rw-r--r--   0        0        0      368 2023-08-01 00:16:04.691748 mercoa-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     8859 2023-08-01 00:16:04.691748 mercoa-0.2.7/src/mercoa/__init__.py
+-rw-r--r--   0        0        0     2384 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/client.py
+-rw-r--r--   0        0        0      348 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      157 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/environment.py
+-rw-r--r--   0        0        0        0 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/py.typed
+-rw-r--r--   0        0        0     8978 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/__init__.py
+-rw-r--r--   0        0        0      165 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/bank_lookup/__init__.py
+-rw-r--r--   0        0        0     3801 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/bank_lookup/client.py
+-rw-r--r--   0        0        0      205 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/bank_lookup/types/__init__.py
+-rw-r--r--   0        0        0      960 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/bank_lookup/types/bank_address.py
+-rw-r--r--   0        0        0      946 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py
+-rw-r--r--   0        0        0      499 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/commons/__init__.py
+-rw-r--r--   0        0        0      314 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/commons/errors/__init__.py
+-rw-r--r--   0        0        0      237 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/commons/errors/auth_header_malformed_error.py
+-rw-r--r--   0        0        0      221 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/commons/errors/auth_header_missing_error.py
+-rw-r--r--   0        0        0      225 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/commons/errors/unauthorized.py
+-rw-r--r--   0        0        0      469 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/commons/types/__init__.py
+-rw-r--r--   0        0        0     1093 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/commons/types/address.py
+-rw-r--r--   0        0        0      824 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/commons/types/birth_date.py
+-rw-r--r--   0        0        0      994 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/commons/types/full_name.py
+-rw-r--r--   0        0        0      850 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/commons/types/individual_government_id.py
+-rw-r--r--   0        0        0      857 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/commons/types/itin.py
+-rw-r--r--   0        0        0      441 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/commons/types/order_direction.py
+-rw-r--r--   0        0        0      855 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/commons/types/phone_number.py
+-rw-r--r--   0        0        0      856 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/commons/types/ssn.py
+-rw-r--r--   0        0        0      523 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/__init__.py
+-rw-r--r--   0        0        0    40498 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/client.py
+-rw-r--r--   0        0        0      501 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/__init__.py
+-rw-r--r--   0        0        0      228 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/approval_policy/__init__.py
+-rw-r--r--   0        0        0    17689 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/approval_policy/client.py
+-rw-r--r--   0        0        0      305 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/approval_policy/errors/__init__.py
+-rw-r--r--   0        0        0      242 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/approval_policy/errors/num_approver_less_than_one_error.py
+-rw-r--r--   0        0        0      248 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/approval_policy/errors/num_approvers_user_list_mismatch_error.py
+-rw-r--r--   0        0        0       65 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/counterparty/__init__.py
+-rw-r--r--   0        0        0     4109 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/counterparty/client.py
+-rw-r--r--   0        0        0       65 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/invoice/__init__.py
+-rw-r--r--   0        0        0    11215 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/invoice/client.py
+-rw-r--r--   0        0        0       65 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/notification_policy/__init__.py
+-rw-r--r--   0        0        0    10326 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/notification_policy/client.py
+-rw-r--r--   0        0        0       65 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/payment_method/__init__.py
+-rw-r--r--   0        0        0    22306 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/payment_method/client.py
+-rw-r--r--   0        0        0       65 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/representative/__init__.py
+-rw-r--r--   0        0        0    12767 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/representative/client.py
+-rw-r--r--   0        0        0      175 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/user/__init__.py
+-rw-r--r--   0        0        0    21722 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/user/client.py
+-rw-r--r--   0        0        0      166 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/user/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/user/resources/notification_policy/__init__.py
+-rw-r--r--   0        0        0    10769 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/user/resources/notification_policy/client.py
+-rw-r--r--   0        0        0       65 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/user/resources/notifications/__init__.py
+-rw-r--r--   0        0        0     8720 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/user/resources/notifications/client.py
+-rw-r--r--   0        0        0     2745 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/__init__.py
+-rw-r--r--   0        0        0     4074 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/__init__.py
+-rw-r--r--   0        0        0      487 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/account_type.py
+-rw-r--r--   0        0        0      849 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/amount_trigger.py
+-rw-r--r--   0        0        0       88 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/approval_policy_id.py
+-rw-r--r--   0        0        0     1100 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/approval_policy_request.py
+-rw-r--r--   0        0        0     1036 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/approval_policy_response.py
+-rw-r--r--   0        0        0     1067 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/approval_policy_update_request.py
+-rw-r--r--   0        0        0      963 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/approver_rule.py
+-rw-r--r--   0        0        0     1451 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/business_profile_request.py
+-rw-r--r--   0        0        0     1509 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/business_profile_response.py
+-rw-r--r--   0        0        0     1917 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/business_type.py
+-rw-r--r--   0        0        0     1013 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/counterparty_response.py
+-rw-r--r--   0        0        0      741 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/ein.py
+-rw-r--r--   0        0        0      914 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/entity_add_payees_request.py
+-rw-r--r--   0        0        0       80 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/entity_id.py
+-rw-r--r--   0        0        0     2432 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/entity_request.py
+-rw-r--r--   0        0        0     1814 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/entity_response.py
+-rw-r--r--   0        0        0     1084 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/entity_status.py
+-rw-r--r--   0        0        0     2084 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/entity_update_request.py
+-rw-r--r--   0        0        0       84 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/entity_user_id.py
+-rw-r--r--   0        0        0     1100 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/entity_user_request.py
+-rw-r--r--   0        0        0     1224 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/entity_user_response.py
+-rw-r--r--   0        0        0     1446 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/find_counterparties_response.py
+-rw-r--r--   0        0        0     1343 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/find_entity_response.py
+-rw-r--r--   0        0        0     1367 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/find_notification_response.py
+-rw-r--r--   0        0        0      633 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/identifier_list.py
+-rw-r--r--   0        0        0     1372 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/individual_profile_request.py
+-rw-r--r--   0        0        0     1206 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/individual_profile_response.py
+-rw-r--r--   0        0        0       86 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/notification_id.py
+-rw-r--r--   0        0        0     1051 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/notification_policy_request.py
+-rw-r--r--   0        0        0     1127 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/notification_policy_response.py
+-rw-r--r--   0        0        0     1129 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/notification_response.py
+-rw-r--r--   0        0        0     1945 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/notification_type.py
+-rw-r--r--   0        0        0      974 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/profile_request.py
+-rw-r--r--   0        0        0      981 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/profile_response.py
+-rw-r--r--   0        0        0       88 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/representative_id.py
+-rw-r--r--   0        0        0     1370 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/representative_request.py
+-rw-r--r--   0        0        0     1539 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/representative_response.py
+-rw-r--r--   0        0        0     1100 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/responsibilities.py
+-rw-r--r--   0        0        0      391 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/rule.py
+-rw-r--r--   0        0        0      761 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/tax_id.py
+-rw-r--r--   0        0        0      854 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/token_generation_invoice_options.py
+-rw-r--r--   0        0        0     1269 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/token_generation_options.py
+-rw-r--r--   0        0        0      963 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/token_generation_pages_options.py
+-rw-r--r--   0        0        0      857 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/token_generation_style_options.py
+-rw-r--r--   0        0        0      951 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/token_generation_vendor_options.py
+-rw-r--r--   0        0        0      573 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/trigger.py
+-rw-r--r--   0        0        0      947 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/user_notification_policy_response.py
+-rw-r--r--   0        0        0      627 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/vendor_network.py
+-rw-r--r--   0        0        0      163 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice/__init__.py
+-rw-r--r--   0        0        0    20874 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice/client.py
+-rw-r--r--   0        0        0      154 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice/resources/approval/__init__.py
+-rw-r--r--   0        0        0     6559 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice/resources/approval/client.py
+-rw-r--r--   0        0        0       65 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice/resources/comment/__init__.py
+-rw-r--r--   0        0        0    15332 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice/resources/comment/client.py
+-rw-r--r--   0        0        0       65 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice/resources/document/__init__.py
+-rw-r--r--   0        0        0     3870 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice/resources/document/client.py
+-rw-r--r--   0        0        0      991 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/__init__.py
+-rw-r--r--   0        0        0     1480 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/__init__.py
+-rw-r--r--   0        0        0     1017 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/approval_request.py
+-rw-r--r--   0        0        0     1592 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/approval_slot.py
+-rw-r--r--   0        0        0     1147 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/approval_slot_assignment.py
+-rw-r--r--   0        0        0       86 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/approval_slot_id.py
+-rw-r--r--   0        0        0      631 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/approver_action.py
+-rw-r--r--   0        0        0      984 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/associated_approval_action.py
+-rw-r--r--   0        0        0       81 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/comment_id.py
+-rw-r--r--   0        0        0      934 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/comment_request.py
+-rw-r--r--   0        0        0     1428 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/comment_response.py
+-rw-r--r--   0        0        0      851 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/document_response.py
+-rw-r--r--   0        0        0     1347 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/find_invoice_response.py
+-rw-r--r--   0        0        0       81 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/invoice_id.py
+-rw-r--r--   0        0        0     1331 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/invoice_line_item_request.py
+-rw-r--r--   0        0        0     1258 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/invoice_line_item_response.py
+-rw-r--r--   0        0        0     1072 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/invoice_metrics_response.py
+-rw-r--r--   0        0        0      870 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/invoice_order_by_field.py
+-rw-r--r--   0        0        0     3578 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/invoice_request.py
+-rw-r--r--   0        0        0     4306 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/invoice_response.py
+-rw-r--r--   0        0        0     1485 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/invoice_status.py
+-rw-r--r--   0        0        0      123 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/ocr/__init__.py
+-rw-r--r--   0        0        0     4438 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/ocr/client.py
+-rw-r--r--   0        0        0      130 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/ocr/types/__init__.py
+-rw-r--r--   0        0        0     1258 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/ocr/types/ocr_response.py
+-rw-r--r--   0        0        0      157 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization/__init__.py
+-rw-r--r--   0        0        0    11712 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization/client.py
+-rw-r--r--   0        0        0      148 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization/resources/notification_configuration/__init__.py
+-rw-r--r--   0        0        0    10288 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization/resources/notification_configuration/client.py
+-rw-r--r--   0        0        0     1607 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/__init__.py
+-rw-r--r--   0        0        0     2348 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/__init__.py
+-rw-r--r--   0        0        0      948 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/color_scheme_request.py
+-rw-r--r--   0        0        0      949 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/color_scheme_response.py
+-rw-r--r--   0        0        0      981 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/email_log_response.py
+-rw-r--r--   0        0        0      932 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/email_provider_request.py
+-rw-r--r--   0        0        0      936 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/email_provider_response.py
+-rw-r--r--   0        0        0      785 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/email_sender_provider.py
+-rw-r--r--   0        0        0     1052 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/email_sender_request.py
+-rw-r--r--   0        0        0     1044 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/email_sender_response.py
+-rw-r--r--   0        0        0      926 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/global_notification_configuration_request.py
+-rw-r--r--   0        0        0      774 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/invoice_notification_configuration_request.py
+-rw-r--r--   0        0        0     1004 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/invoice_notification_configuration_response.py
+-rw-r--r--   0        0        0      627 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/notification_configuration_request.py
+-rw-r--r--   0        0        0      633 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/notification_configuration_response.py
+-rw-r--r--   0        0        0       86 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/organization_id.py
+-rw-r--r--   0        0        0     1711 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/organization_request.py
+-rw-r--r--   0        0        0     1808 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/organization_response.py
+-rw-r--r--   0        0        0     1142 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/payment_methods_request.py
+-rw-r--r--   0        0        0     1148 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/payment_methods_response.py
+-rw-r--r--   0        0        0      849 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/payment_rail_markup.py
+-rw-r--r--   0        0        0      482 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/payment_rail_markup_type.py
+-rw-r--r--   0        0        0     1151 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/payment_rail_request.py
+-rw-r--r--   0        0        0      843 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/payment_rail_response.py
+-rw-r--r--   0        0        0       65 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/payment_method_schema/__init__.py
+-rw-r--r--   0        0        0    15390 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/payment_method_schema/client.py
+-rw-r--r--   0        0        0     2547 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/__init__.py
+-rw-r--r--   0        0        0     3587 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/__init__.py
+-rw-r--r--   0        0        0     1336 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/bank_account_base_request.py
+-rw-r--r--   0        0        0     1466 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/bank_account_base_response.py
+-rw-r--r--   0        0        0     1026 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/bank_account_request.py
+-rw-r--r--   0        0        0     1014 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/bank_account_response.py
+-rw-r--r--   0        0        0      960 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/bank_status.py
+-rw-r--r--   0        0        0      632 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/bank_type.py
+-rw-r--r--   0        0        0     1247 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/card_base_request.py
+-rw-r--r--   0        0        0     1468 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/card_base_response.py
+-rw-r--r--   0        0        0      819 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/card_brand.py
+-rw-r--r--   0        0        0      961 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/card_request.py
+-rw-r--r--   0        0        0      935 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/card_response.py
+-rw-r--r--   0        0        0      750 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/card_type.py
+-rw-r--r--   0        0        0     1258 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/check_base_request.py
+-rw-r--r--   0        0        0     1494 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/check_base_response.py
+-rw-r--r--   0        0        0      967 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/check_request.py
+-rw-r--r--   0        0        0      941 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/check_response.py
+-rw-r--r--   0        0        0    22179 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/currency_code.py
+-rw-r--r--   0        0        0     1607 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_request.py
+-rw-r--r--   0        0        0     2026 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_response.py
+-rw-r--r--   0        0        0     1040 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/custom_payment_method_request.py
+-rw-r--r--   0        0        0     1028 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/custom_payment_method_response.py
+-rw-r--r--   0        0        0     1613 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_base_request.py
+-rw-r--r--   0        0        0     1071 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_request.py
+-rw-r--r--   0        0        0       87 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_id.py
+-rw-r--r--   0        0        0     1264 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_request.py
+-rw-r--r--   0        0        0     1298 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_response.py
+-rw-r--r--   0        0        0     1984 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_schema_field.py
+-rw-r--r--   0        0        0      682 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_schema_field_type.py
+-rw-r--r--   0        0        0       93 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_schema_id.py
+-rw-r--r--   0        0        0     1581 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_schema_request.py
+-rw-r--r--   0        0        0     1693 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_schema_response.py
+-rw-r--r--   0        0        0     1229 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_type.py
+-rw-r--r--   0        0        0      514 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_update_request.py
+-rw-r--r--   0        0        0     1042 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/plaid_link_request.py
+-rw-r--r--   0        0        0      271 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/transaction/__init__.py
+-rw-r--r--   0        0        0     6642 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/transaction/client.py
+-rw-r--r--   0        0        0      386 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/transaction/types/__init__.py
+-rw-r--r--   0        0        0       85 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/transaction/types/transaction_id.py
+-rw-r--r--   0        0        0     1138 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/transaction/types/transaction_response.py
+-rw-r--r--   0        0        0     1582 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/transaction/types/transaction_response_expanded.py
+-rw-r--r--   0        0        0     1261 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/transaction/types/transaction_status.py
+-rw-r--r--   0        0        0     2433 1970-01-01 00:00:00.000000 mercoa-0.2.7/PKG-INFO
```

### Comparing `mercoa-0.2.6/README.md` & `mercoa-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/__init__.py` & `mercoa-0.2.7/src/mercoa/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -71,29 +71,36 @@
     EntityUserRequest,
     EntityUserResponse,
     FindCounterpartiesResponse,
     FindEntityResponse,
     FindInvoiceResponse,
     FindNotificationResponse,
     FullName,
+    GlobalNotificationConfigurationRequest,
     IdentifierList,
     IdentifierList_RolesList,
     IdentifierList_UserList,
     IndividualGovernmentId,
     IndividualProfileRequest,
     IndividualProfileResponse,
     InvoiceId,
     InvoiceLineItemRequest,
     InvoiceLineItemResponse,
     InvoiceMetricsResponse,
+    InvoiceNotificationConfigurationRequest,
+    InvoiceNotificationConfigurationResponse,
     InvoiceOrderByField,
     InvoiceRequest,
     InvoiceResponse,
     InvoiceStatus,
     Itin,
+    NotificationConfigurationRequest,
+    NotificationConfigurationRequest_Invoice,
+    NotificationConfigurationResponse,
+    NotificationConfigurationResponse_Invoice,
     NotificationId,
     NotificationPolicyRequest,
     NotificationPolicyResponse,
     NotificationResponse,
     NotificationType,
     OcrResponse,
     OrderDirection,
@@ -133,14 +140,19 @@
     RepresentativeRequest,
     RepresentativeResponse,
     Responsibilities,
     Rule,
     Rule_Approver,
     Ssn,
     TaxId,
+    TokenGenerationInvoiceOptions,
+    TokenGenerationOptions,
+    TokenGenerationPagesOptions,
+    TokenGenerationStyleOptions,
+    TokenGenerationVendorOptions,
     TransactionId,
     TransactionResponse,
     TransactionResponseExpanded,
     TransactionStatus,
     Trigger,
     Trigger_All,
     Trigger_Amount,
@@ -151,14 +163,15 @@
     commons,
     entity,
     entity_types,
     invoice,
     invoice_types,
     ocr,
     organization,
+    organization_types,
     payment_method_schema,
     payment_method_types,
     transaction,
 )
 
 __all__ = [
     "AccountType",
@@ -230,30 +243,37 @@
     "EntityUserRequest",
     "EntityUserResponse",
     "FindCounterpartiesResponse",
     "FindEntityResponse",
     "FindInvoiceResponse",
     "FindNotificationResponse",
     "FullName",
+    "GlobalNotificationConfigurationRequest",
     "IdentifierList",
     "IdentifierList_RolesList",
     "IdentifierList_UserList",
     "IndividualGovernmentId",
     "IndividualProfileRequest",
     "IndividualProfileResponse",
     "InvoiceId",
     "InvoiceLineItemRequest",
     "InvoiceLineItemResponse",
     "InvoiceMetricsResponse",
+    "InvoiceNotificationConfigurationRequest",
+    "InvoiceNotificationConfigurationResponse",
     "InvoiceOrderByField",
     "InvoiceRequest",
     "InvoiceResponse",
     "InvoiceStatus",
     "Itin",
     "MercoaEnvironment",
+    "NotificationConfigurationRequest",
+    "NotificationConfigurationRequest_Invoice",
+    "NotificationConfigurationResponse",
+    "NotificationConfigurationResponse_Invoice",
     "NotificationId",
     "NotificationPolicyRequest",
     "NotificationPolicyResponse",
     "NotificationResponse",
     "NotificationType",
     "OcrResponse",
     "OrderDirection",
@@ -293,14 +313,19 @@
     "RepresentativeRequest",
     "RepresentativeResponse",
     "Responsibilities",
     "Rule",
     "Rule_Approver",
     "Ssn",
     "TaxId",
+    "TokenGenerationInvoiceOptions",
+    "TokenGenerationOptions",
+    "TokenGenerationPagesOptions",
+    "TokenGenerationStyleOptions",
+    "TokenGenerationVendorOptions",
     "TransactionId",
     "TransactionResponse",
     "TransactionResponseExpanded",
     "TransactionStatus",
     "Trigger",
     "Trigger_All",
     "Trigger_Amount",
@@ -311,11 +336,12 @@
     "commons",
     "entity",
     "entity_types",
     "invoice",
     "invoice_types",
     "ocr",
     "organization",
+    "organization_types",
     "payment_method_schema",
     "payment_method_types",
     "transaction",
 ]
```

### Comparing `mercoa-0.2.6/src/mercoa/client.py` & `mercoa-0.2.7/src/mercoa/client.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 
 class Mercoa:
     def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
         self.entity = EntityClient(environment=self._environment, token=self._token)
         self.invoice = InvoiceClient(environment=self._environment, token=self._token)
+        self.organization = OrganizationClient(environment=self._environment, token=self._token)
         self.bank_lookup = BankLookupClient(environment=self._environment, token=self._token)
         self.ocr = OcrClient(environment=self._environment, token=self._token)
-        self.organization = OrganizationClient(environment=self._environment, token=self._token)
         self.payment_method_schema = PaymentMethodSchemaClient(environment=self._environment, token=self._token)
         self.transaction = TransactionClient(environment=self._environment, token=self._token)
 
 
 class AsyncMercoa:
     def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
         self.entity = AsyncEntityClient(environment=self._environment, token=self._token)
         self.invoice = AsyncInvoiceClient(environment=self._environment, token=self._token)
+        self.organization = AsyncOrganizationClient(environment=self._environment, token=self._token)
         self.bank_lookup = AsyncBankLookupClient(environment=self._environment, token=self._token)
         self.ocr = AsyncOcrClient(environment=self._environment, token=self._token)
-        self.organization = AsyncOrganizationClient(environment=self._environment, token=self._token)
         self.payment_method_schema = AsyncPaymentMethodSchemaClient(environment=self._environment, token=self._token)
         self.transaction = AsyncTransactionClient(environment=self._environment, token=self._token)
```

### Comparing `mercoa-0.2.6/src/mercoa/core/datetime_utils.py` & `mercoa-0.2.7/src/mercoa/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/core/jsonable_encoder.py` & `mercoa-0.2.7/src/mercoa/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/__init__.py` & `mercoa-0.2.7/src/mercoa/resources/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     commons,
     entity,
     entity_types,
     invoice,
     invoice_types,
     ocr,
     organization,
+    organization_types,
     payment_method_schema,
     payment_method_types,
     transaction,
 )
 from .bank_lookup import BankAddress, BankLookupResponse
 from .commons import (
     Address,
@@ -67,18 +68,24 @@
     RepresentativeId,
     RepresentativeRequest,
     RepresentativeResponse,
     Responsibilities,
     Rule,
     Rule_Approver,
     TaxId,
+    TokenGenerationInvoiceOptions,
+    TokenGenerationOptions,
+    TokenGenerationPagesOptions,
+    TokenGenerationStyleOptions,
+    TokenGenerationVendorOptions,
     Trigger,
     Trigger_All,
     Trigger_Amount,
     UserNotificationPolicyResponse,
+    VendorNetwork,
 )
 from .invoice_types import (
     ApprovalRequest,
     ApprovalSlot,
     ApprovalSlotAssignment,
     ApprovalSlotId,
     ApproverAction,
@@ -93,24 +100,31 @@
     InvoiceLineItemResponse,
     InvoiceMetricsResponse,
     InvoiceOrderByField,
     InvoiceRequest,
     InvoiceResponse,
     InvoiceStatus,
 )
-from .ocr import OcrResponse, VendorNetwork
-from .organization import (
+from .ocr import OcrResponse
+from .organization_types import (
     ColorSchemeRequest,
     ColorSchemeResponse,
     EmailLogResponse,
     EmailProviderRequest,
     EmailProviderResponse,
     EmailSenderProvider,
     EmailSenderRequest,
     EmailSenderResponse,
+    GlobalNotificationConfigurationRequest,
+    InvoiceNotificationConfigurationRequest,
+    InvoiceNotificationConfigurationResponse,
+    NotificationConfigurationRequest,
+    NotificationConfigurationRequest_Invoice,
+    NotificationConfigurationResponse,
+    NotificationConfigurationResponse_Invoice,
     OrganizationId,
     OrganizationRequest,
     OrganizationResponse,
     PaymentMethodsRequest,
     PaymentMethodsResponse,
     PaymentRailMarkup,
     PaymentRailMarkupType,
@@ -234,29 +248,36 @@
     "EntityUserRequest",
     "EntityUserResponse",
     "FindCounterpartiesResponse",
     "FindEntityResponse",
     "FindInvoiceResponse",
     "FindNotificationResponse",
     "FullName",
+    "GlobalNotificationConfigurationRequest",
     "IdentifierList",
     "IdentifierList_RolesList",
     "IdentifierList_UserList",
     "IndividualGovernmentId",
     "IndividualProfileRequest",
     "IndividualProfileResponse",
     "InvoiceId",
     "InvoiceLineItemRequest",
     "InvoiceLineItemResponse",
     "InvoiceMetricsResponse",
+    "InvoiceNotificationConfigurationRequest",
+    "InvoiceNotificationConfigurationResponse",
     "InvoiceOrderByField",
     "InvoiceRequest",
     "InvoiceResponse",
     "InvoiceStatus",
     "Itin",
+    "NotificationConfigurationRequest",
+    "NotificationConfigurationRequest_Invoice",
+    "NotificationConfigurationResponse",
+    "NotificationConfigurationResponse_Invoice",
     "NotificationId",
     "NotificationPolicyRequest",
     "NotificationPolicyResponse",
     "NotificationResponse",
     "NotificationType",
     "OcrResponse",
     "OrderDirection",
@@ -296,14 +317,19 @@
     "RepresentativeRequest",
     "RepresentativeResponse",
     "Responsibilities",
     "Rule",
     "Rule_Approver",
     "Ssn",
     "TaxId",
+    "TokenGenerationInvoiceOptions",
+    "TokenGenerationOptions",
+    "TokenGenerationPagesOptions",
+    "TokenGenerationStyleOptions",
+    "TokenGenerationVendorOptions",
     "TransactionId",
     "TransactionResponse",
     "TransactionResponseExpanded",
     "TransactionStatus",
     "Trigger",
     "Trigger_All",
     "Trigger_Amount",
@@ -314,11 +340,12 @@
     "commons",
     "entity",
     "entity_types",
     "invoice",
     "invoice_types",
     "ocr",
     "organization",
+    "organization_types",
     "payment_method_schema",
     "payment_method_types",
     "transaction",
 ]
```

### Comparing `mercoa-0.2.6/src/mercoa/resources/bank_lookup/client.py` & `mercoa-0.2.7/src/mercoa/resources/bank_lookup/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/bank_lookup/types/bank_address.py` & `mercoa-0.2.7/src/mercoa/resources/bank_lookup/types/bank_address.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py` & `mercoa-0.2.7/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/commons/types/address.py` & `mercoa-0.2.7/src/mercoa/resources/commons/types/address.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/commons/types/birth_date.py` & `mercoa-0.2.7/src/mercoa/resources/commons/types/birth_date.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/commons/types/full_name.py` & `mercoa-0.2.7/src/mercoa/resources/commons/types/full_name.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/commons/types/individual_government_id.py` & `mercoa-0.2.7/src/mercoa/resources/commons/types/individual_government_id.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/commons/types/itin.py` & `mercoa-0.2.7/src/mercoa/resources/commons/types/itin.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/commons/types/phone_number.py` & `mercoa-0.2.7/src/mercoa/resources/commons/types/phone_number.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/commons/types/ssn.py` & `mercoa-0.2.7/src/mercoa/resources/commons/types/ssn.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity/__init__.py` & `mercoa-0.2.7/src/mercoa/resources/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity/client.py` & `mercoa-0.2.7/src/mercoa/resources/entity/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from ..entity_types.types.entity_add_payees_request import EntityAddPayeesRequest
 from ..entity_types.types.entity_id import EntityId
 from ..entity_types.types.entity_request import EntityRequest
 from ..entity_types.types.entity_response import EntityResponse
 from ..entity_types.types.entity_status import EntityStatus
 from ..entity_types.types.entity_update_request import EntityUpdateRequest
 from ..entity_types.types.find_entity_response import FindEntityResponse
+from ..entity_types.types.token_generation_options import TokenGenerationOptions
 from .resources.approval_policy.client import ApprovalPolicyClient, AsyncApprovalPolicyClient
 from .resources.counterparty.client import AsyncCounterpartyClient, CounterpartyClient
 from .resources.invoice.client import AsyncInvoiceClient, InvoiceClient
 from .resources.notification_policy.client import AsyncNotificationPolicyClient, NotificationPolicyClient
 from .resources.payment_method.client import AsyncPaymentMethodClient, PaymentMethodClient
 from .resources.representative.client import AsyncRepresentativeClient, RepresentativeClient
 from .resources.user.client import AsyncUserClient, UserClient
@@ -254,15 +255,15 @@
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_token(self, entity_id: EntityId) -> str:
+    def get_raw_token(self, entity_id: EntityId) -> str:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/token"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
@@ -278,14 +279,39 @@
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    def get_token(self, entity_id: EntityId, *, request: TokenGenerationOptions) -> str:
+        _response = httpx.request(
+            "POST",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/token"),
+            json=jsonable_encoder(request),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
+            timeout=60,
+        )
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(str, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
     def plaid_link_token(self, entity_id: EntityId) -> str:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/plaidLinkToken"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
@@ -588,26 +614,52 @@
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_token(self, entity_id: EntityId) -> str:
+    async def get_raw_token(self, entity_id: EntityId) -> str:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/token"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         try:
             _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(str, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def get_token(self, entity_id: EntityId, *, request: TokenGenerationOptions) -> str:
+        async with httpx.AsyncClient() as _client:
+            _response = await _client.request(
+                "POST",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/token"),
+                json=jsonable_encoder(request),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
+                timeout=60,
+            )
+        try:
+            _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(str, _response_json)  # type: ignore
         if "errorName" in _response_json:
             if _response_json["errorName"] == "AuthHeaderMissingError":
                 raise AuthHeaderMissingError()
```

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity/resources/approval_policy/client.py` & `mercoa-0.2.7/src/mercoa/resources/entity/resources/approval_policy/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity/resources/counterparty/client.py` & `mercoa-0.2.7/src/mercoa/resources/entity/resources/counterparty/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity/resources/invoice/client.py` & `mercoa-0.2.7/src/mercoa/resources/entity/resources/invoice/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity/resources/notification_policy/client.py` & `mercoa-0.2.7/src/mercoa/resources/entity/resources/notification_policy/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity/resources/payment_method/client.py` & `mercoa-0.2.7/src/mercoa/resources/entity/resources/payment_method/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity/resources/representative/client.py` & `mercoa-0.2.7/src/mercoa/resources/entity/resources/representative/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity/resources/user/client.py` & `mercoa-0.2.7/src/mercoa/resources/invoice/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,140 +1,171 @@
 # This file was auto-generated by Fern from our API Definition.
 
+import datetime as dt
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
-from .....core.api_error import ApiError
-from .....core.jsonable_encoder import jsonable_encoder
-from .....core.remove_none_from_headers import remove_none_from_headers
-from .....environment import MercoaEnvironment
-from ....commons.errors.auth_header_malformed_error import AuthHeaderMalformedError
-from ....commons.errors.auth_header_missing_error import AuthHeaderMissingError
-from ....commons.errors.unauthorized import Unauthorized
-from ....entity_types.types.entity_id import EntityId
-from ....entity_types.types.entity_user_id import EntityUserId
-from ....entity_types.types.entity_user_request import EntityUserRequest
-from ....entity_types.types.entity_user_response import EntityUserResponse
-from .resources.notification_policy.client import AsyncNotificationPolicyClient, NotificationPolicyClient
-from .resources.notifications.client import AsyncNotificationsClient, NotificationsClient
+from ...core.api_error import ApiError
+from ...core.datetime_utils import serialize_datetime
+from ...core.jsonable_encoder import jsonable_encoder
+from ...core.remove_none_from_headers import remove_none_from_headers
+from ...environment import MercoaEnvironment
+from ..commons.errors.auth_header_malformed_error import AuthHeaderMalformedError
+from ..commons.errors.auth_header_missing_error import AuthHeaderMissingError
+from ..commons.errors.unauthorized import Unauthorized
+from ..commons.types.order_direction import OrderDirection
+from ..entity_types.types.entity_id import EntityId
+from ..invoice_types.types.find_invoice_response import FindInvoiceResponse
+from ..invoice_types.types.invoice_id import InvoiceId
+from ..invoice_types.types.invoice_order_by_field import InvoiceOrderByField
+from ..invoice_types.types.invoice_request import InvoiceRequest
+from ..invoice_types.types.invoice_response import InvoiceResponse
+from ..invoice_types.types.invoice_status import InvoiceStatus
+from .resources.approval.client import ApprovalClient, AsyncApprovalClient
+from .resources.comment.client import AsyncCommentClient, CommentClient
+from .resources.document.client import AsyncDocumentClient, DocumentClient
 
 
-class UserClient:
+class InvoiceClient:
     def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
-        self.notification_policy = NotificationPolicyClient(environment=self._environment, token=self._token)
-        self.notifications = NotificationsClient(environment=self._environment, token=self._token)
-
-    def get_all(self, entity_id: EntityId) -> typing.List[EntityUserResponse]:
+        self.approval = ApprovalClient(environment=self._environment, token=self._token)
+        self.comment = CommentClient(environment=self._environment, token=self._token)
+        self.document = DocumentClient(environment=self._environment, token=self._token)
+
+    def find(
+        self,
+        *,
+        entity_ids: typing.Union[typing.Optional[EntityId], typing.List[EntityId]],
+        start_date: typing.Optional[dt.datetime] = None,
+        end_date: typing.Optional[dt.datetime] = None,
+        order_by: typing.Optional[InvoiceOrderByField] = None,
+        order_direction: typing.Optional[OrderDirection] = None,
+        limit: typing.Optional[int] = None,
+        starting_after: typing.Optional[InvoiceId] = None,
+        search: typing.Optional[str] = None,
+        status: typing.Union[typing.Optional[InvoiceStatus], typing.List[InvoiceStatus]],
+    ) -> FindInvoiceResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/users"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "invoices"),
+            params={
+                "entityIds": entity_ids,
+                "startDate": serialize_datetime(start_date) if start_date is not None else None,
+                "endDate": serialize_datetime(end_date) if end_date is not None else None,
+                "orderBy": order_by,
+                "orderDirection": order_direction,
+                "limit": limit,
+                "startingAfter": starting_after,
+                "search": search,
+                "status": status,
+            },
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[EntityUserResponse], _response_json)  # type: ignore
+            return pydantic.parse_obj_as(FindInvoiceResponse, _response_json)  # type: ignore
         if "errorName" in _response_json:
             if _response_json["errorName"] == "AuthHeaderMissingError":
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def create(self, entity_id: EntityId, *, request: EntityUserRequest) -> EntityUserResponse:
+    def create(self, *, request: InvoiceRequest) -> InvoiceResponse:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/user"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "invoice"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(EntityUserResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
         if "errorName" in _response_json:
             if _response_json["errorName"] == "AuthHeaderMissingError":
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get(self, entity_id: EntityId, user_id: EntityUserId) -> EntityUserResponse:
+    def get(self, invoice_id: InvoiceId) -> InvoiceResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/user/{user_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(EntityUserResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
         if "errorName" in _response_json:
             if _response_json["errorName"] == "AuthHeaderMissingError":
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def update(self, entity_id: EntityId, user_id: EntityUserId, *, request: EntityUserRequest) -> EntityUserResponse:
+    def update(self, invoice_id: InvoiceId, *, request: InvoiceRequest) -> InvoiceResponse:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/user/{user_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(EntityUserResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
         if "errorName" in _response_json:
             if _response_json["errorName"] == "AuthHeaderMissingError":
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def delete(self, entity_id: EntityId, user_id: EntityUserId) -> None:
+    def delete(self, invoice_id: InvoiceId) -> None:
         _response = httpx.request(
             "DELETE",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/user/{user_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
@@ -147,18 +178,18 @@
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_token(self, entity_id: EntityId, user_id: EntityUserId) -> str:
+    def get_vendor_link(self, invoice_id: InvoiceId) -> str:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/user/{user_id}/token"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/vendorlink"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         try:
             _response_json = _response.json()
@@ -172,130 +203,152 @@
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncUserClient:
+class AsyncInvoiceClient:
     def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
-        self.notification_policy = AsyncNotificationPolicyClient(environment=self._environment, token=self._token)
-        self.notifications = AsyncNotificationsClient(environment=self._environment, token=self._token)
-
-    async def get_all(self, entity_id: EntityId) -> typing.List[EntityUserResponse]:
+        self.approval = AsyncApprovalClient(environment=self._environment, token=self._token)
+        self.comment = AsyncCommentClient(environment=self._environment, token=self._token)
+        self.document = AsyncDocumentClient(environment=self._environment, token=self._token)
+
+    async def find(
+        self,
+        *,
+        entity_ids: typing.Union[typing.Optional[EntityId], typing.List[EntityId]],
+        start_date: typing.Optional[dt.datetime] = None,
+        end_date: typing.Optional[dt.datetime] = None,
+        order_by: typing.Optional[InvoiceOrderByField] = None,
+        order_direction: typing.Optional[OrderDirection] = None,
+        limit: typing.Optional[int] = None,
+        starting_after: typing.Optional[InvoiceId] = None,
+        search: typing.Optional[str] = None,
+        status: typing.Union[typing.Optional[InvoiceStatus], typing.List[InvoiceStatus]],
+    ) -> FindInvoiceResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/users"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "invoices"),
+                params={
+                    "entityIds": entity_ids,
+                    "startDate": serialize_datetime(start_date) if start_date is not None else None,
+                    "endDate": serialize_datetime(end_date) if end_date is not None else None,
+                    "orderBy": order_by,
+                    "orderDirection": order_direction,
+                    "limit": limit,
+                    "startingAfter": starting_after,
+                    "search": search,
+                    "status": status,
+                },
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[EntityUserResponse], _response_json)  # type: ignore
+            return pydantic.parse_obj_as(FindInvoiceResponse, _response_json)  # type: ignore
         if "errorName" in _response_json:
             if _response_json["errorName"] == "AuthHeaderMissingError":
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def create(self, entity_id: EntityId, *, request: EntityUserRequest) -> EntityUserResponse:
+    async def create(self, *, request: InvoiceRequest) -> InvoiceResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/user"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "invoice"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(EntityUserResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
         if "errorName" in _response_json:
             if _response_json["errorName"] == "AuthHeaderMissingError":
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get(self, entity_id: EntityId, user_id: EntityUserId) -> EntityUserResponse:
+    async def get(self, invoice_id: InvoiceId) -> InvoiceResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/user/{user_id}"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(EntityUserResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
         if "errorName" in _response_json:
             if _response_json["errorName"] == "AuthHeaderMissingError":
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def update(
-        self, entity_id: EntityId, user_id: EntityUserId, *, request: EntityUserRequest
-    ) -> EntityUserResponse:
+    async def update(self, invoice_id: InvoiceId, *, request: InvoiceRequest) -> InvoiceResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/user/{user_id}"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(EntityUserResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
         if "errorName" in _response_json:
             if _response_json["errorName"] == "AuthHeaderMissingError":
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def delete(self, entity_id: EntityId, user_id: EntityUserId) -> None:
+    async def delete(self, invoice_id: InvoiceId) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/user/{user_id}"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
@@ -308,19 +361,19 @@
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_token(self, entity_id: EntityId, user_id: EntityUserId) -> str:
+    async def get_vendor_link(self, invoice_id: InvoiceId) -> str:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/user/{user_id}/token"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/vendorlink"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         try:
             _response_json = _response.json()
```

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity/resources/user/resources/notification_policy/client.py` & `mercoa-0.2.7/src/mercoa/resources/entity/resources/user/resources/notification_policy/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity/resources/user/resources/notifications/client.py` & `mercoa-0.2.7/src/mercoa/resources/entity/resources/user/resources/notifications/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/__init__.py` & `mercoa-0.2.7/src/mercoa/resources/organization_types/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,101 +1,55 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .types import (
-    AccountType,
-    AmountTrigger,
-    ApprovalPolicyId,
-    ApprovalPolicyRequest,
-    ApprovalPolicyResponse,
-    ApprovalPolicyUpdateRequest,
-    ApproverRule,
-    BusinessProfileRequest,
-    BusinessProfileResponse,
-    BusinessType,
-    CounterpartyResponse,
-    Ein,
-    EntityAddPayeesRequest,
-    EntityId,
-    EntityRequest,
-    EntityResponse,
-    EntityStatus,
-    EntityUpdateRequest,
-    EntityUserId,
-    EntityUserRequest,
-    EntityUserResponse,
-    FindCounterpartiesResponse,
-    FindEntityResponse,
-    FindNotificationResponse,
-    IdentifierList,
-    IdentifierList_RolesList,
-    IdentifierList_UserList,
-    IndividualProfileRequest,
-    IndividualProfileResponse,
-    NotificationId,
-    NotificationPolicyRequest,
-    NotificationPolicyResponse,
-    NotificationResponse,
-    NotificationType,
-    ProfileRequest,
-    ProfileResponse,
-    RepresentativeId,
-    RepresentativeRequest,
-    RepresentativeResponse,
-    Responsibilities,
-    Rule,
-    Rule_Approver,
-    TaxId,
-    Trigger,
-    Trigger_All,
-    Trigger_Amount,
-    UserNotificationPolicyResponse,
+    ColorSchemeRequest,
+    ColorSchemeResponse,
+    EmailLogResponse,
+    EmailProviderRequest,
+    EmailProviderResponse,
+    EmailSenderProvider,
+    EmailSenderRequest,
+    EmailSenderResponse,
+    GlobalNotificationConfigurationRequest,
+    InvoiceNotificationConfigurationRequest,
+    InvoiceNotificationConfigurationResponse,
+    NotificationConfigurationRequest,
+    NotificationConfigurationRequest_Invoice,
+    NotificationConfigurationResponse,
+    NotificationConfigurationResponse_Invoice,
+    OrganizationId,
+    OrganizationRequest,
+    OrganizationResponse,
+    PaymentMethodsRequest,
+    PaymentMethodsResponse,
+    PaymentRailMarkup,
+    PaymentRailMarkupType,
+    PaymentRailRequest,
+    PaymentRailResponse,
 )
 
 __all__ = [
-    "AccountType",
-    "AmountTrigger",
-    "ApprovalPolicyId",
-    "ApprovalPolicyRequest",
-    "ApprovalPolicyResponse",
-    "ApprovalPolicyUpdateRequest",
-    "ApproverRule",
-    "BusinessProfileRequest",
-    "BusinessProfileResponse",
-    "BusinessType",
-    "CounterpartyResponse",
-    "Ein",
-    "EntityAddPayeesRequest",
-    "EntityId",
-    "EntityRequest",
-    "EntityResponse",
-    "EntityStatus",
-    "EntityUpdateRequest",
-    "EntityUserId",
-    "EntityUserRequest",
-    "EntityUserResponse",
-    "FindCounterpartiesResponse",
-    "FindEntityResponse",
-    "FindNotificationResponse",
-    "IdentifierList",
-    "IdentifierList_RolesList",
-    "IdentifierList_UserList",
-    "IndividualProfileRequest",
-    "IndividualProfileResponse",
-    "NotificationId",
-    "NotificationPolicyRequest",
-    "NotificationPolicyResponse",
-    "NotificationResponse",
-    "NotificationType",
-    "ProfileRequest",
-    "ProfileResponse",
-    "RepresentativeId",
-    "RepresentativeRequest",
-    "RepresentativeResponse",
-    "Responsibilities",
-    "Rule",
-    "Rule_Approver",
-    "TaxId",
-    "Trigger",
-    "Trigger_All",
-    "Trigger_Amount",
-    "UserNotificationPolicyResponse",
+    "ColorSchemeRequest",
+    "ColorSchemeResponse",
+    "EmailLogResponse",
+    "EmailProviderRequest",
+    "EmailProviderResponse",
+    "EmailSenderProvider",
+    "EmailSenderRequest",
+    "EmailSenderResponse",
+    "GlobalNotificationConfigurationRequest",
+    "InvoiceNotificationConfigurationRequest",
+    "InvoiceNotificationConfigurationResponse",
+    "NotificationConfigurationRequest",
+    "NotificationConfigurationRequest_Invoice",
+    "NotificationConfigurationResponse",
+    "NotificationConfigurationResponse_Invoice",
+    "OrganizationId",
+    "OrganizationRequest",
+    "OrganizationResponse",
+    "PaymentMethodsRequest",
+    "PaymentMethodsResponse",
+    "PaymentRailMarkup",
+    "PaymentRailMarkupType",
+    "PaymentRailRequest",
+    "PaymentRailResponse",
 ]
```

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/types/amount_trigger.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/amount_trigger.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/types/approval_policy_request.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/approval_policy_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/types/approval_policy_response.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/approval_policy_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/types/approval_policy_update_request.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/approval_policy_update_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/types/approver_rule.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/approver_rule.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/types/business_profile_request.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/business_profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/types/business_profile_response.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/business_profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/types/business_type.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/business_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/types/counterparty_response.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/counterparty_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/types/ein.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/ein.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/types/entity_add_payees_request.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/entity_add_payees_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/types/entity_request.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/entity_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/types/entity_response.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/entity_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/types/entity_status.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/entity_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/types/entity_update_request.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/entity_update_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/types/entity_user_request.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/entity_user_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/types/entity_user_response.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/entity_user_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/types/find_counterparties_response.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/find_counterparties_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/types/find_entity_response.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/find_entity_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/types/find_notification_response.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/find_notification_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/types/identifier_list.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/identifier_list.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/types/individual_profile_request.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/individual_profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/types/individual_profile_response.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/individual_profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/types/notification_policy_request.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/notification_policy_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/types/notification_policy_response.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/notification_policy_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/types/notification_response.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/notification_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/types/notification_type.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/notification_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/types/profile_request.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/types/profile_response.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/types/representative_request.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/representative_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/types/representative_response.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/representative_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/types/responsibilities.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/responsibilities.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/types/tax_id.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/tax_id.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/types/trigger.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/trigger.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/entity_types/types/user_notification_policy_response.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/user_notification_policy_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/invoice/client.py` & `mercoa-0.2.7/src/mercoa/resources/entity/resources/user/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,171 +1,141 @@
 # This file was auto-generated by Fern from our API Definition.
 
-import datetime as dt
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
-from ...core.api_error import ApiError
-from ...core.datetime_utils import serialize_datetime
-from ...core.jsonable_encoder import jsonable_encoder
-from ...core.remove_none_from_headers import remove_none_from_headers
-from ...environment import MercoaEnvironment
-from ..commons.errors.auth_header_malformed_error import AuthHeaderMalformedError
-from ..commons.errors.auth_header_missing_error import AuthHeaderMissingError
-from ..commons.errors.unauthorized import Unauthorized
-from ..commons.types.order_direction import OrderDirection
-from ..entity_types.types.entity_id import EntityId
-from ..invoice_types.types.find_invoice_response import FindInvoiceResponse
-from ..invoice_types.types.invoice_id import InvoiceId
-from ..invoice_types.types.invoice_order_by_field import InvoiceOrderByField
-from ..invoice_types.types.invoice_request import InvoiceRequest
-from ..invoice_types.types.invoice_response import InvoiceResponse
-from ..invoice_types.types.invoice_status import InvoiceStatus
-from .resources.approval.client import ApprovalClient, AsyncApprovalClient
-from .resources.comment.client import AsyncCommentClient, CommentClient
-from .resources.document.client import AsyncDocumentClient, DocumentClient
+from .....core.api_error import ApiError
+from .....core.jsonable_encoder import jsonable_encoder
+from .....core.remove_none_from_headers import remove_none_from_headers
+from .....environment import MercoaEnvironment
+from ....commons.errors.auth_header_malformed_error import AuthHeaderMalformedError
+from ....commons.errors.auth_header_missing_error import AuthHeaderMissingError
+from ....commons.errors.unauthorized import Unauthorized
+from ....entity_types.types.entity_id import EntityId
+from ....entity_types.types.entity_user_id import EntityUserId
+from ....entity_types.types.entity_user_request import EntityUserRequest
+from ....entity_types.types.entity_user_response import EntityUserResponse
+from ....entity_types.types.token_generation_options import TokenGenerationOptions
+from .resources.notification_policy.client import AsyncNotificationPolicyClient, NotificationPolicyClient
+from .resources.notifications.client import AsyncNotificationsClient, NotificationsClient
 
 
-class InvoiceClient:
+class UserClient:
     def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
-        self.approval = ApprovalClient(environment=self._environment, token=self._token)
-        self.comment = CommentClient(environment=self._environment, token=self._token)
-        self.document = DocumentClient(environment=self._environment, token=self._token)
-
-    def find(
-        self,
-        *,
-        entity_ids: typing.Union[typing.Optional[EntityId], typing.List[EntityId]],
-        start_date: typing.Optional[dt.datetime] = None,
-        end_date: typing.Optional[dt.datetime] = None,
-        order_by: typing.Optional[InvoiceOrderByField] = None,
-        order_direction: typing.Optional[OrderDirection] = None,
-        limit: typing.Optional[int] = None,
-        starting_after: typing.Optional[InvoiceId] = None,
-        search: typing.Optional[str] = None,
-        status: typing.Union[typing.Optional[InvoiceStatus], typing.List[InvoiceStatus]],
-    ) -> FindInvoiceResponse:
+        self.notification_policy = NotificationPolicyClient(environment=self._environment, token=self._token)
+        self.notifications = NotificationsClient(environment=self._environment, token=self._token)
+
+    def get_all(self, entity_id: EntityId) -> typing.List[EntityUserResponse]:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "invoices"),
-            params={
-                "entityIds": entity_ids,
-                "startDate": serialize_datetime(start_date) if start_date is not None else None,
-                "endDate": serialize_datetime(end_date) if end_date is not None else None,
-                "orderBy": order_by,
-                "orderDirection": order_direction,
-                "limit": limit,
-                "startingAfter": starting_after,
-                "search": search,
-                "status": status,
-            },
+            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/users"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(FindInvoiceResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(typing.List[EntityUserResponse], _response_json)  # type: ignore
         if "errorName" in _response_json:
             if _response_json["errorName"] == "AuthHeaderMissingError":
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def create(self, *, request: InvoiceRequest) -> InvoiceResponse:
+    def create(self, entity_id: EntityId, *, request: EntityUserRequest) -> EntityUserResponse:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "invoice"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/user"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(EntityUserResponse, _response_json)  # type: ignore
         if "errorName" in _response_json:
             if _response_json["errorName"] == "AuthHeaderMissingError":
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get(self, invoice_id: InvoiceId) -> InvoiceResponse:
+    def get(self, entity_id: EntityId, user_id: EntityUserId) -> EntityUserResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/user/{user_id}"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(EntityUserResponse, _response_json)  # type: ignore
         if "errorName" in _response_json:
             if _response_json["errorName"] == "AuthHeaderMissingError":
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def update(self, invoice_id: InvoiceId, *, request: InvoiceRequest) -> InvoiceResponse:
+    def update(self, entity_id: EntityId, user_id: EntityUserId, *, request: EntityUserRequest) -> EntityUserResponse:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/user/{user_id}"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(EntityUserResponse, _response_json)  # type: ignore
         if "errorName" in _response_json:
             if _response_json["errorName"] == "AuthHeaderMissingError":
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def delete(self, invoice_id: InvoiceId) -> None:
+    def delete(self, entity_id: EntityId, user_id: EntityUserId) -> None:
         _response = httpx.request(
             "DELETE",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/user/{user_id}"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
@@ -178,18 +148,43 @@
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_vendor_link(self, invoice_id: InvoiceId) -> str:
+    def get_raw_token(self, entity_id: EntityId, user_id: EntityUserId) -> str:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/vendorlink"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/user/{user_id}/token"),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
+            timeout=60,
+        )
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(str, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    def get_token(self, entity_id: EntityId, user_id: EntityUserId, *, request: TokenGenerationOptions) -> str:
+        _response = httpx.request(
+            "POST",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/user/{user_id}/token"),
+            json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         try:
             _response_json = _response.json()
@@ -203,152 +198,130 @@
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncInvoiceClient:
+class AsyncUserClient:
     def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
-        self.approval = AsyncApprovalClient(environment=self._environment, token=self._token)
-        self.comment = AsyncCommentClient(environment=self._environment, token=self._token)
-        self.document = AsyncDocumentClient(environment=self._environment, token=self._token)
-
-    async def find(
-        self,
-        *,
-        entity_ids: typing.Union[typing.Optional[EntityId], typing.List[EntityId]],
-        start_date: typing.Optional[dt.datetime] = None,
-        end_date: typing.Optional[dt.datetime] = None,
-        order_by: typing.Optional[InvoiceOrderByField] = None,
-        order_direction: typing.Optional[OrderDirection] = None,
-        limit: typing.Optional[int] = None,
-        starting_after: typing.Optional[InvoiceId] = None,
-        search: typing.Optional[str] = None,
-        status: typing.Union[typing.Optional[InvoiceStatus], typing.List[InvoiceStatus]],
-    ) -> FindInvoiceResponse:
+        self.notification_policy = AsyncNotificationPolicyClient(environment=self._environment, token=self._token)
+        self.notifications = AsyncNotificationsClient(environment=self._environment, token=self._token)
+
+    async def get_all(self, entity_id: EntityId) -> typing.List[EntityUserResponse]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "invoices"),
-                params={
-                    "entityIds": entity_ids,
-                    "startDate": serialize_datetime(start_date) if start_date is not None else None,
-                    "endDate": serialize_datetime(end_date) if end_date is not None else None,
-                    "orderBy": order_by,
-                    "orderDirection": order_direction,
-                    "limit": limit,
-                    "startingAfter": starting_after,
-                    "search": search,
-                    "status": status,
-                },
+                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/users"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(FindInvoiceResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(typing.List[EntityUserResponse], _response_json)  # type: ignore
         if "errorName" in _response_json:
             if _response_json["errorName"] == "AuthHeaderMissingError":
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def create(self, *, request: InvoiceRequest) -> InvoiceResponse:
+    async def create(self, entity_id: EntityId, *, request: EntityUserRequest) -> EntityUserResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "invoice"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/user"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(EntityUserResponse, _response_json)  # type: ignore
         if "errorName" in _response_json:
             if _response_json["errorName"] == "AuthHeaderMissingError":
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get(self, invoice_id: InvoiceId) -> InvoiceResponse:
+    async def get(self, entity_id: EntityId, user_id: EntityUserId) -> EntityUserResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/user/{user_id}"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(EntityUserResponse, _response_json)  # type: ignore
         if "errorName" in _response_json:
             if _response_json["errorName"] == "AuthHeaderMissingError":
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def update(self, invoice_id: InvoiceId, *, request: InvoiceRequest) -> InvoiceResponse:
+    async def update(
+        self, entity_id: EntityId, user_id: EntityUserId, *, request: EntityUserRequest
+    ) -> EntityUserResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/user/{user_id}"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(EntityUserResponse, _response_json)  # type: ignore
         if "errorName" in _response_json:
             if _response_json["errorName"] == "AuthHeaderMissingError":
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def delete(self, invoice_id: InvoiceId) -> None:
+    async def delete(self, entity_id: EntityId, user_id: EntityUserId) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/user/{user_id}"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
@@ -361,19 +334,45 @@
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_vendor_link(self, invoice_id: InvoiceId) -> str:
+    async def get_raw_token(self, entity_id: EntityId, user_id: EntityUserId) -> str:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/vendorlink"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/user/{user_id}/token"),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
+                timeout=60,
+            )
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(str, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def get_token(self, entity_id: EntityId, user_id: EntityUserId, *, request: TokenGenerationOptions) -> str:
+        async with httpx.AsyncClient() as _client:
+            _response = await _client.request(
+                "POST",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/user/{user_id}/token"),
+                json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         try:
             _response_json = _response.json()
```

### Comparing `mercoa-0.2.6/src/mercoa/resources/invoice/resources/approval/client.py` & `mercoa-0.2.7/src/mercoa/resources/invoice/resources/approval/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/invoice/resources/comment/client.py` & `mercoa-0.2.7/src/mercoa/resources/invoice/resources/comment/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/invoice/resources/document/client.py` & `mercoa-0.2.7/src/mercoa/resources/invoice/resources/document/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/invoice_types/__init__.py` & `mercoa-0.2.7/src/mercoa/resources/invoice_types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/invoice_types/types/__init__.py` & `mercoa-0.2.7/src/mercoa/resources/invoice_types/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/invoice_types/types/approval_request.py` & `mercoa-0.2.7/src/mercoa/resources/invoice_types/types/approval_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/invoice_types/types/approval_slot.py` & `mercoa-0.2.7/src/mercoa/resources/invoice_types/types/approval_slot.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/invoice_types/types/approval_slot_assignment.py` & `mercoa-0.2.7/src/mercoa/resources/invoice_types/types/approval_slot_assignment.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/invoice_types/types/approver_action.py` & `mercoa-0.2.7/src/mercoa/resources/invoice_types/types/approver_action.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/invoice_types/types/associated_approval_action.py` & `mercoa-0.2.7/src/mercoa/resources/invoice_types/types/associated_approval_action.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/invoice_types/types/comment_request.py` & `mercoa-0.2.7/src/mercoa/resources/invoice_types/types/comment_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/invoice_types/types/comment_response.py` & `mercoa-0.2.7/src/mercoa/resources/invoice_types/types/comment_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/invoice_types/types/document_response.py` & `mercoa-0.2.7/src/mercoa/resources/invoice_types/types/document_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/invoice_types/types/find_invoice_response.py` & `mercoa-0.2.7/src/mercoa/resources/invoice_types/types/find_invoice_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/invoice_types/types/invoice_line_item_request.py` & `mercoa-0.2.7/src/mercoa/resources/invoice_types/types/invoice_line_item_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/invoice_types/types/invoice_line_item_response.py` & `mercoa-0.2.7/src/mercoa/resources/invoice_types/types/invoice_line_item_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/invoice_types/types/invoice_metrics_response.py` & `mercoa-0.2.7/src/mercoa/resources/invoice_types/types/invoice_metrics_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/invoice_types/types/invoice_order_by_field.py` & `mercoa-0.2.7/src/mercoa/resources/invoice_types/types/invoice_order_by_field.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/invoice_types/types/invoice_request.py` & `mercoa-0.2.7/src/mercoa/resources/invoice_types/types/invoice_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/invoice_types/types/invoice_response.py` & `mercoa-0.2.7/src/mercoa/resources/invoice_types/types/invoice_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/invoice_types/types/invoice_status.py` & `mercoa-0.2.7/src/mercoa/resources/invoice_types/types/invoice_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/ocr/client.py` & `mercoa-0.2.7/src/mercoa/resources/ocr/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import MercoaEnvironment
 from ..commons.errors.auth_header_malformed_error import AuthHeaderMalformedError
 from ..commons.errors.auth_header_missing_error import AuthHeaderMissingError
 from ..commons.errors.unauthorized import Unauthorized
 from ..entity_types.types.entity_id import EntityId
+from ..entity_types.types.vendor_network import VendorNetwork
 from .types.ocr_response import OcrResponse
-from .types.vendor_network import VendorNetwork
 
 
 class OcrClient:
     def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
```

### Comparing `mercoa-0.2.6/src/mercoa/resources/ocr/types/ocr_response.py` & `mercoa-0.2.7/src/mercoa/resources/ocr/types/ocr_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/ocr/types/vendor_network.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/vendor_network.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
 class VendorNetwork(str, enum.Enum):
-    ENTITY = "ENTITY"
-    PLATFORM = "PLATFORM"
-    MERCOA = "MERCOA"
+    ALL = "all"
+    PLATFORM = "platform"
+    ENTITY = "entity"
 
     def visit(
         self,
-        entity: typing.Callable[[], T_Result],
+        all: typing.Callable[[], T_Result],
         platform: typing.Callable[[], T_Result],
-        mercoa: typing.Callable[[], T_Result],
+        entity: typing.Callable[[], T_Result],
     ) -> T_Result:
-        if self is VendorNetwork.ENTITY:
-            return entity()
+        if self is VendorNetwork.ALL:
+            return all()
         if self is VendorNetwork.PLATFORM:
             return platform()
-        if self is VendorNetwork.MERCOA:
-            return mercoa()
+        if self is VendorNetwork.ENTITY:
+            return entity()
```

### Comparing `mercoa-0.2.6/src/mercoa/resources/organization/client.py` & `mercoa-0.2.7/src/mercoa/resources/organization/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,35 +12,48 @@
 from ...core.datetime_utils import serialize_datetime
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import MercoaEnvironment
 from ..commons.errors.auth_header_malformed_error import AuthHeaderMalformedError
 from ..commons.errors.auth_header_missing_error import AuthHeaderMissingError
 from ..commons.errors.unauthorized import Unauthorized
-from .types.email_log_response import EmailLogResponse
-from .types.organization_request import OrganizationRequest
-from .types.organization_response import OrganizationResponse
+from ..organization_types.types.email_log_response import EmailLogResponse
+from ..organization_types.types.organization_request import OrganizationRequest
+from ..organization_types.types.organization_response import OrganizationResponse
+from .resources.notification_configuration.client import (
+    AsyncNotificationConfigurationClient,
+    NotificationConfigurationClient,
+)
 
 
 class OrganizationClient:
     def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
+        self.notification_configuration = NotificationConfigurationClient(
+            environment=self._environment, token=self._token
+        )
 
     def get(
         self,
         *,
         payment_methods: typing.Optional[bool] = None,
         email_provider: typing.Optional[bool] = None,
         color_scheme: typing.Optional[bool] = None,
+        notification_configuration: typing.Optional[bool] = None,
     ) -> OrganizationResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "organization"),
-            params={"paymentMethods": payment_methods, "emailProvider": email_provider, "colorScheme": color_scheme},
+            params={
+                "paymentMethods": payment_methods,
+                "emailProvider": email_provider,
+                "colorScheme": color_scheme,
+                "notificationConfiguration": notification_configuration,
+            },
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         try:
             _response_json = _response.json()
@@ -113,30 +126,35 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncOrganizationClient:
     def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
+        self.notification_configuration = AsyncNotificationConfigurationClient(
+            environment=self._environment, token=self._token
+        )
 
     async def get(
         self,
         *,
         payment_methods: typing.Optional[bool] = None,
         email_provider: typing.Optional[bool] = None,
         color_scheme: typing.Optional[bool] = None,
+        notification_configuration: typing.Optional[bool] = None,
     ) -> OrganizationResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", "organization"),
                 params={
                     "paymentMethods": payment_methods,
                     "emailProvider": email_provider,
                     "colorScheme": color_scheme,
+                    "notificationConfiguration": notification_configuration,
                 },
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         try:
```

### Comparing `mercoa-0.2.6/src/mercoa/resources/organization/types/color_scheme_request.py` & `mercoa-0.2.7/src/mercoa/resources/organization_types/types/color_scheme_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/organization/types/color_scheme_response.py` & `mercoa-0.2.7/src/mercoa/resources/organization_types/types/color_scheme_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/organization/types/email_log_response.py` & `mercoa-0.2.7/src/mercoa/resources/organization_types/types/email_log_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/organization/types/email_provider_request.py` & `mercoa-0.2.7/src/mercoa/resources/organization_types/types/email_provider_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/organization/types/email_provider_response.py` & `mercoa-0.2.7/src/mercoa/resources/organization_types/types/email_provider_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/organization/types/email_sender_provider.py` & `mercoa-0.2.7/src/mercoa/resources/organization_types/types/email_sender_provider.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/organization/types/email_sender_request.py` & `mercoa-0.2.7/src/mercoa/resources/organization_types/types/email_sender_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/organization/types/email_sender_response.py` & `mercoa-0.2.7/src/mercoa/resources/organization_types/types/email_sender_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/organization/types/organization_request.py` & `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_base_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,27 +2,32 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .color_scheme_request import ColorSchemeRequest
-from .email_provider_request import EmailProviderRequest
-from .payment_methods_request import PaymentMethodsRequest
+from .payment_method_schema_id import PaymentMethodSchemaId
 
 
-class OrganizationRequest(pydantic.BaseModel):
-    name: typing.Optional[str]
-    logo: typing.Optional[str]
-    website_url: typing.Optional[str] = pydantic.Field(alias="websiteUrl")
-    support_email: typing.Optional[str] = pydantic.Field(alias="supportEmail")
-    payment_methods: typing.Optional[PaymentMethodsRequest] = pydantic.Field(alias="paymentMethods")
-    email_provider: typing.Optional[EmailProviderRequest] = pydantic.Field(alias="emailProvider")
-    color_scheme: typing.Optional[ColorSchemeRequest] = pydantic.Field(alias="colorScheme")
+class CustomPaymentMethodUpdateBaseRequest(pydantic.BaseModel):
+    foreign_id: typing.Optional[str] = pydantic.Field(
+        alias="foreignId", description=("ID for this payment method in your system\n")
+    )
+    account_name: typing.Optional[str] = pydantic.Field(alias="accountName")
+    account_number: typing.Optional[str] = pydantic.Field(alias="accountNumber")
+    schema_id: typing.Optional[PaymentMethodSchemaId] = pydantic.Field(
+        alias="schemaId",
+        description=(
+            "Payment method schema used for this payment method. Defines the fields that this payment method contains.\n"
+        ),
+    )
+    data: typing.Optional[typing.Dict[str, str]] = pydantic.Field(
+        description=("Object of key/value pairs that matches the keys in the linked payment method schema.\n")
+    )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.2.6/src/mercoa/resources/organization/types/organization_response.py` & `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/card_base_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .color_scheme_response import ColorSchemeResponse
-from .email_provider_response import EmailProviderResponse
-from .organization_id import OrganizationId
-from .payment_methods_response import PaymentMethodsResponse
-
-
-class OrganizationResponse(pydantic.BaseModel):
-    id: OrganizationId
-    sandbox: bool
-    name: str
-    logo_url: typing.Optional[str] = pydantic.Field(alias="logoUrl")
-    website_url: typing.Optional[str] = pydantic.Field(alias="websiteUrl")
-    support_email: typing.Optional[str] = pydantic.Field(alias="supportEmail")
-    payment_methods: typing.Optional[PaymentMethodsResponse] = pydantic.Field(alias="paymentMethods")
-    email_provider: typing.Optional[EmailProviderResponse] = pydantic.Field(alias="emailProvider")
-    color_scheme: typing.Optional[ColorSchemeResponse] = pydantic.Field(alias="colorScheme")
+from .card_brand import CardBrand
+from .card_type import CardType
+from .currency_code import CurrencyCode
+from .payment_method_id import PaymentMethodId
+
+
+class CardBaseResponse(pydantic.BaseModel):
+    id: PaymentMethodId
+    card_type: CardType = pydantic.Field(alias="cardType")
+    card_brand: CardBrand = pydantic.Field(alias="cardBrand")
+    last_four: str = pydantic.Field(alias="lastFour")
+    exp_month: str = pydantic.Field(alias="expMonth")
+    exp_year: str = pydantic.Field(alias="expYear")
+    supported_currencies: typing.List[CurrencyCode] = pydantic.Field(alias="supportedCurrencies")
+    created_at: dt.datetime = pydantic.Field(alias="createdAt")
+    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.2.6/src/mercoa/resources/organization/types/payment_methods_request.py` & `mercoa-0.2.7/src/mercoa/resources/organization_types/types/payment_methods_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/organization/types/payment_methods_response.py` & `mercoa-0.2.7/src/mercoa/resources/organization_types/types/payment_methods_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/organization/types/payment_rail_markup.py` & `mercoa-0.2.7/src/mercoa/resources/organization_types/types/payment_rail_markup.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/organization/types/payment_rail_request.py` & `mercoa-0.2.7/src/mercoa/resources/organization_types/types/payment_rail_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/organization/types/payment_rail_response.py` & `mercoa-0.2.7/src/mercoa/resources/organization_types/types/payment_rail_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/payment_method_schema/client.py` & `mercoa-0.2.7/src/mercoa/resources/payment_method_schema/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/payment_method_types/__init__.py` & `mercoa-0.2.7/src/mercoa/resources/payment_method_types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/__init__.py` & `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/bank_account_base_request.py` & `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/bank_account_base_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/bank_account_base_response.py` & `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/bank_account_base_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/bank_account_request.py` & `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/bank_account_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/bank_account_response.py` & `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/bank_account_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/bank_status.py` & `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/bank_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/bank_type.py` & `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/bank_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/card_base_request.py` & `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/card_base_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/card_base_response.py` & `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_schema_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,28 +2,32 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .card_brand import CardBrand
-from .card_type import CardType
 from .currency_code import CurrencyCode
-from .payment_method_id import PaymentMethodId
+from .payment_method_schema_field import PaymentMethodSchemaField
+from .payment_method_schema_id import PaymentMethodSchemaId
 
 
-class CardBaseResponse(pydantic.BaseModel):
-    id: PaymentMethodId
-    card_type: CardType = pydantic.Field(alias="cardType")
-    card_brand: CardBrand = pydantic.Field(alias="cardBrand")
-    last_four: str = pydantic.Field(alias="lastFour")
-    exp_month: str = pydantic.Field(alias="expMonth")
-    exp_year: str = pydantic.Field(alias="expYear")
-    supported_currencies: typing.List[CurrencyCode] = pydantic.Field(alias="supportedCurrencies")
+class PaymentMethodSchemaResponse(pydantic.BaseModel):
+    id: PaymentMethodSchemaId
+    name: str
+    is_source: bool = pydantic.Field(
+        alias="isSource", description=("This payment method can be used as a payment source for an invoice\n")
+    )
+    is_destination: bool = pydantic.Field(
+        alias="isDestination", description=("This payment method can be used as a payment destination for an invoice\n")
+    )
+    supported_currencies: typing.List[CurrencyCode] = pydantic.Field(
+        alias="supportedCurrencies", description=("List of currencies that this payment method supports.\n")
+    )
+    fields: typing.List[PaymentMethodSchemaField]
     created_at: dt.datetime = pydantic.Field(alias="createdAt")
     updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/card_brand.py` & `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/card_brand.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/card_request.py` & `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/card_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/card_response.py` & `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/card_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/card_type.py` & `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/card_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/check_base_request.py` & `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/check_base_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/check_base_response.py` & `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/check_base_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/check_request.py` & `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/check_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/check_response.py` & `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/check_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/currency_code.py` & `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/currency_code.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_request.py` & `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_response.py` & `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/custom_payment_method_request.py` & `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/custom_payment_method_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/custom_payment_method_response.py` & `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/custom_payment_method_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_base_request.py` & `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_schema_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,32 +2,33 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .payment_method_schema_id import PaymentMethodSchemaId
+from .currency_code import CurrencyCode
+from .payment_method_schema_field import PaymentMethodSchemaField
 
 
-class CustomPaymentMethodUpdateBaseRequest(pydantic.BaseModel):
-    foreign_id: typing.Optional[str] = pydantic.Field(
-        alias="foreignId", description=("ID for this payment method in your system\n")
+class PaymentMethodSchemaRequest(pydantic.BaseModel):
+    name: str
+    is_source: bool = pydantic.Field(
+        alias="isSource", description=("This payment method can be used as a payment source for an invoice\n")
     )
-    account_name: typing.Optional[str] = pydantic.Field(alias="accountName")
-    account_number: typing.Optional[str] = pydantic.Field(alias="accountNumber")
-    schema_id: typing.Optional[PaymentMethodSchemaId] = pydantic.Field(
-        alias="schemaId",
+    is_destination: bool = pydantic.Field(
+        alias="isDestination", description=("This payment method can be used as a payment destination for an invoice\n")
+    )
+    supported_currencies: typing.Optional[typing.List[CurrencyCode]] = pydantic.Field(
+        alias="supportedCurrencies",
         description=(
-            "Payment method schema used for this payment method. Defines the fields that this payment method contains.\n"
+            "List of currencies that this payment method supports. If not provided, the payment method will support only USD.\n"
         ),
     )
-    data: typing.Optional[typing.Dict[str, str]] = pydantic.Field(
-        description=("Object of key/value pairs that matches the keys in the linked payment method schema.\n")
-    )
+    fields: typing.List[PaymentMethodSchemaField]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_request.py` & `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/payment_method_request.py` & `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/payment_method_response.py` & `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/payment_method_schema_field.py` & `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_schema_field.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/payment_method_schema_field_type.py` & `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_schema_field_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/payment_method_schema_request.py` & `mercoa-0.2.7/src/mercoa/resources/entity_types/types/token_generation_pages_options.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,33 +2,20 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .currency_code import CurrencyCode
-from .payment_method_schema_field import PaymentMethodSchemaField
 
 
-class PaymentMethodSchemaRequest(pydantic.BaseModel):
-    name: str
-    is_source: bool = pydantic.Field(
-        alias="isSource", description=("This payment method can be used as a payment source for an invoice\n")
-    )
-    is_destination: bool = pydantic.Field(
-        alias="isDestination", description=("This payment method can be used as a payment destination for an invoice\n")
-    )
-    supported_currencies: typing.Optional[typing.List[CurrencyCode]] = pydantic.Field(
-        alias="supportedCurrencies",
-        description=(
-            "List of currencies that this payment method supports. If not provided, the payment method will support only USD.\n"
-        ),
-    )
-    fields: typing.List[PaymentMethodSchemaField]
+class TokenGenerationPagesOptions(pydantic.BaseModel):
+    payment_methods: typing.Optional[bool] = pydantic.Field(alias="paymentMethods")
+    representatives: typing.Optional[bool]
+    notifications: typing.Optional[bool]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/payment_method_schema_response.py` & `mercoa-0.2.7/src/mercoa/resources/transaction/types/transaction_response_expanded.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,34 +2,28 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .currency_code import CurrencyCode
-from .payment_method_schema_field import PaymentMethodSchemaField
-from .payment_method_schema_id import PaymentMethodSchemaId
-
-
-class PaymentMethodSchemaResponse(pydantic.BaseModel):
-    id: PaymentMethodSchemaId
-    name: str
-    is_source: bool = pydantic.Field(
-        alias="isSource", description=("This payment method can be used as a payment source for an invoice\n")
-    )
-    is_destination: bool = pydantic.Field(
-        alias="isDestination", description=("This payment method can be used as a payment destination for an invoice\n")
-    )
-    supported_currencies: typing.List[CurrencyCode] = pydantic.Field(
-        alias="supportedCurrencies", description=("List of currencies that this payment method supports.\n")
-    )
-    fields: typing.List[PaymentMethodSchemaField]
-    created_at: dt.datetime = pydantic.Field(alias="createdAt")
-    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
+from ...entity_types.types.entity_response import EntityResponse
+from ...invoice_types.types.invoice_id import InvoiceId
+from ...payment_method_types.types.payment_method_response import PaymentMethodResponse
+from .transaction_response import TransactionResponse
+
+
+class TransactionResponseExpanded(TransactionResponse):
+    invoice_id: InvoiceId = pydantic.Field(alias="invoiceId")
+    deduction_date: typing.Optional[dt.datetime] = pydantic.Field(alias="deductionDate")
+    due_date: typing.Optional[dt.datetime] = pydantic.Field(alias="dueDate")
+    payer: typing.Optional[EntityResponse]
+    vendor: typing.Optional[EntityResponse]
+    payment_source: typing.Optional[PaymentMethodResponse] = pydantic.Field(alias="paymentSource")
+    payment_destination: typing.Optional[PaymentMethodResponse] = pydantic.Field(alias="paymentDestination")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/payment_method_type.py` & `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/payment_method_update_request.py` & `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_update_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/payment_method_types/types/plaid_link_request.py` & `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/plaid_link_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/transaction/client.py` & `mercoa-0.2.7/src/mercoa/resources/transaction/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/transaction/types/transaction_response.py` & `mercoa-0.2.7/src/mercoa/resources/transaction/types/transaction_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/src/mercoa/resources/transaction/types/transaction_status.py` & `mercoa-0.2.7/src/mercoa/resources/transaction/types/transaction_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.6/PKG-INFO` & `mercoa-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercoa
-Version: 0.2.6
+Version: 0.2.7
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

