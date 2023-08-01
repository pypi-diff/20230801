# Comparing `tmp/mercoa-0.2.7.tar.gz` & `tmp/mercoa-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercoa-0.2.7.tar", max compression
+gzip compressed data, was "mercoa-0.2.8.tar", max compression
```

## Comparing `mercoa-0.2.7.tar` & `mercoa-0.2.8.tar`

### file list

```diff
@@ -1,215 +1,215 @@
--rw-r--r--   0        0        0     1930 2023-08-01 00:16:04.691748 mercoa-0.2.7/README.md
--rw-r--r--   0        0        0      368 2023-08-01 00:16:04.691748 mercoa-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     8859 2023-08-01 00:16:04.691748 mercoa-0.2.7/src/mercoa/__init__.py
--rw-r--r--   0        0        0     2384 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/client.py
--rw-r--r--   0        0        0      348 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/core/__init__.py
--rw-r--r--   0        0        0      426 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      157 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/environment.py
--rw-r--r--   0        0        0        0 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/py.typed
--rw-r--r--   0        0        0     8978 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/__init__.py
--rw-r--r--   0        0        0      165 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/bank_lookup/__init__.py
--rw-r--r--   0        0        0     3801 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/bank_lookup/client.py
--rw-r--r--   0        0        0      205 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/bank_lookup/types/__init__.py
--rw-r--r--   0        0        0      960 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/bank_lookup/types/bank_address.py
--rw-r--r--   0        0        0      946 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py
--rw-r--r--   0        0        0      499 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/commons/__init__.py
--rw-r--r--   0        0        0      314 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/commons/errors/__init__.py
--rw-r--r--   0        0        0      237 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/commons/errors/auth_header_malformed_error.py
--rw-r--r--   0        0        0      221 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/commons/errors/auth_header_missing_error.py
--rw-r--r--   0        0        0      225 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/commons/errors/unauthorized.py
--rw-r--r--   0        0        0      469 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/commons/types/__init__.py
--rw-r--r--   0        0        0     1093 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/commons/types/address.py
--rw-r--r--   0        0        0      824 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/commons/types/birth_date.py
--rw-r--r--   0        0        0      994 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/commons/types/full_name.py
--rw-r--r--   0        0        0      850 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/commons/types/individual_government_id.py
--rw-r--r--   0        0        0      857 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/commons/types/itin.py
--rw-r--r--   0        0        0      441 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/commons/types/order_direction.py
--rw-r--r--   0        0        0      855 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/commons/types/phone_number.py
--rw-r--r--   0        0        0      856 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/commons/types/ssn.py
--rw-r--r--   0        0        0      523 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/__init__.py
--rw-r--r--   0        0        0    40498 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/client.py
--rw-r--r--   0        0        0      501 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/__init__.py
--rw-r--r--   0        0        0      228 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/approval_policy/__init__.py
--rw-r--r--   0        0        0    17689 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/approval_policy/client.py
--rw-r--r--   0        0        0      305 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/approval_policy/errors/__init__.py
--rw-r--r--   0        0        0      242 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/approval_policy/errors/num_approver_less_than_one_error.py
--rw-r--r--   0        0        0      248 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/approval_policy/errors/num_approvers_user_list_mismatch_error.py
--rw-r--r--   0        0        0       65 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/counterparty/__init__.py
--rw-r--r--   0        0        0     4109 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/counterparty/client.py
--rw-r--r--   0        0        0       65 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/invoice/__init__.py
--rw-r--r--   0        0        0    11215 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/invoice/client.py
--rw-r--r--   0        0        0       65 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/notification_policy/__init__.py
--rw-r--r--   0        0        0    10326 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/notification_policy/client.py
--rw-r--r--   0        0        0       65 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/payment_method/__init__.py
--rw-r--r--   0        0        0    22306 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/payment_method/client.py
--rw-r--r--   0        0        0       65 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/representative/__init__.py
--rw-r--r--   0        0        0    12767 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/representative/client.py
--rw-r--r--   0        0        0      175 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/user/__init__.py
--rw-r--r--   0        0        0    21722 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/user/client.py
--rw-r--r--   0        0        0      166 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/user/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/user/resources/notification_policy/__init__.py
--rw-r--r--   0        0        0    10769 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/user/resources/notification_policy/client.py
--rw-r--r--   0        0        0       65 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/user/resources/notifications/__init__.py
--rw-r--r--   0        0        0     8720 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity/resources/user/resources/notifications/client.py
--rw-r--r--   0        0        0     2745 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/__init__.py
--rw-r--r--   0        0        0     4074 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/__init__.py
--rw-r--r--   0        0        0      487 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/account_type.py
--rw-r--r--   0        0        0      849 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/amount_trigger.py
--rw-r--r--   0        0        0       88 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/approval_policy_id.py
--rw-r--r--   0        0        0     1100 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/approval_policy_request.py
--rw-r--r--   0        0        0     1036 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/approval_policy_response.py
--rw-r--r--   0        0        0     1067 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/approval_policy_update_request.py
--rw-r--r--   0        0        0      963 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/approver_rule.py
--rw-r--r--   0        0        0     1451 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/business_profile_request.py
--rw-r--r--   0        0        0     1509 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/business_profile_response.py
--rw-r--r--   0        0        0     1917 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/business_type.py
--rw-r--r--   0        0        0     1013 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/counterparty_response.py
--rw-r--r--   0        0        0      741 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/ein.py
--rw-r--r--   0        0        0      914 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/entity_add_payees_request.py
--rw-r--r--   0        0        0       80 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/entity_id.py
--rw-r--r--   0        0        0     2432 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/entity_request.py
--rw-r--r--   0        0        0     1814 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/entity_response.py
--rw-r--r--   0        0        0     1084 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/entity_status.py
--rw-r--r--   0        0        0     2084 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/entity_update_request.py
--rw-r--r--   0        0        0       84 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/entity_user_id.py
--rw-r--r--   0        0        0     1100 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/entity_user_request.py
--rw-r--r--   0        0        0     1224 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/entity_user_response.py
--rw-r--r--   0        0        0     1446 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/find_counterparties_response.py
--rw-r--r--   0        0        0     1343 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/find_entity_response.py
--rw-r--r--   0        0        0     1367 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/find_notification_response.py
--rw-r--r--   0        0        0      633 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/identifier_list.py
--rw-r--r--   0        0        0     1372 2023-08-01 00:16:04.695749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/individual_profile_request.py
--rw-r--r--   0        0        0     1206 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/individual_profile_response.py
--rw-r--r--   0        0        0       86 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/notification_id.py
--rw-r--r--   0        0        0     1051 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/notification_policy_request.py
--rw-r--r--   0        0        0     1127 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/notification_policy_response.py
--rw-r--r--   0        0        0     1129 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/notification_response.py
--rw-r--r--   0        0        0     1945 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/notification_type.py
--rw-r--r--   0        0        0      974 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/profile_request.py
--rw-r--r--   0        0        0      981 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/profile_response.py
--rw-r--r--   0        0        0       88 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/representative_id.py
--rw-r--r--   0        0        0     1370 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/representative_request.py
--rw-r--r--   0        0        0     1539 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/representative_response.py
--rw-r--r--   0        0        0     1100 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/responsibilities.py
--rw-r--r--   0        0        0      391 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/rule.py
--rw-r--r--   0        0        0      761 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/tax_id.py
--rw-r--r--   0        0        0      854 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/token_generation_invoice_options.py
--rw-r--r--   0        0        0     1269 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/token_generation_options.py
--rw-r--r--   0        0        0      963 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/token_generation_pages_options.py
--rw-r--r--   0        0        0      857 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/token_generation_style_options.py
--rw-r--r--   0        0        0      951 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/token_generation_vendor_options.py
--rw-r--r--   0        0        0      573 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/trigger.py
--rw-r--r--   0        0        0      947 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/user_notification_policy_response.py
--rw-r--r--   0        0        0      627 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/entity_types/types/vendor_network.py
--rw-r--r--   0        0        0      163 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice/__init__.py
--rw-r--r--   0        0        0    20874 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice/client.py
--rw-r--r--   0        0        0      154 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice/resources/approval/__init__.py
--rw-r--r--   0        0        0     6559 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice/resources/approval/client.py
--rw-r--r--   0        0        0       65 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice/resources/comment/__init__.py
--rw-r--r--   0        0        0    15332 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice/resources/comment/client.py
--rw-r--r--   0        0        0       65 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice/resources/document/__init__.py
--rw-r--r--   0        0        0     3870 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice/resources/document/client.py
--rw-r--r--   0        0        0      991 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/__init__.py
--rw-r--r--   0        0        0     1480 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/__init__.py
--rw-r--r--   0        0        0     1017 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/approval_request.py
--rw-r--r--   0        0        0     1592 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/approval_slot.py
--rw-r--r--   0        0        0     1147 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/approval_slot_assignment.py
--rw-r--r--   0        0        0       86 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/approval_slot_id.py
--rw-r--r--   0        0        0      631 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/approver_action.py
--rw-r--r--   0        0        0      984 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/associated_approval_action.py
--rw-r--r--   0        0        0       81 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/comment_id.py
--rw-r--r--   0        0        0      934 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/comment_request.py
--rw-r--r--   0        0        0     1428 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/comment_response.py
--rw-r--r--   0        0        0      851 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/document_response.py
--rw-r--r--   0        0        0     1347 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/find_invoice_response.py
--rw-r--r--   0        0        0       81 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/invoice_id.py
--rw-r--r--   0        0        0     1331 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/invoice_line_item_request.py
--rw-r--r--   0        0        0     1258 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/invoice_line_item_response.py
--rw-r--r--   0        0        0     1072 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/invoice_metrics_response.py
--rw-r--r--   0        0        0      870 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/invoice_order_by_field.py
--rw-r--r--   0        0        0     3578 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/invoice_request.py
--rw-r--r--   0        0        0     4306 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/invoice_response.py
--rw-r--r--   0        0        0     1485 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/invoice_types/types/invoice_status.py
--rw-r--r--   0        0        0      123 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/ocr/__init__.py
--rw-r--r--   0        0        0     4438 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/ocr/client.py
--rw-r--r--   0        0        0      130 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/ocr/types/__init__.py
--rw-r--r--   0        0        0     1258 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/ocr/types/ocr_response.py
--rw-r--r--   0        0        0      157 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization/__init__.py
--rw-r--r--   0        0        0    11712 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization/client.py
--rw-r--r--   0        0        0      148 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization/resources/notification_configuration/__init__.py
--rw-r--r--   0        0        0    10288 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization/resources/notification_configuration/client.py
--rw-r--r--   0        0        0     1607 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/__init__.py
--rw-r--r--   0        0        0     2348 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/__init__.py
--rw-r--r--   0        0        0      948 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/color_scheme_request.py
--rw-r--r--   0        0        0      949 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/color_scheme_response.py
--rw-r--r--   0        0        0      981 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/email_log_response.py
--rw-r--r--   0        0        0      932 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/email_provider_request.py
--rw-r--r--   0        0        0      936 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/email_provider_response.py
--rw-r--r--   0        0        0      785 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/email_sender_provider.py
--rw-r--r--   0        0        0     1052 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/email_sender_request.py
--rw-r--r--   0        0        0     1044 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/email_sender_response.py
--rw-r--r--   0        0        0      926 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/global_notification_configuration_request.py
--rw-r--r--   0        0        0      774 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/invoice_notification_configuration_request.py
--rw-r--r--   0        0        0     1004 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/invoice_notification_configuration_response.py
--rw-r--r--   0        0        0      627 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/notification_configuration_request.py
--rw-r--r--   0        0        0      633 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/notification_configuration_response.py
--rw-r--r--   0        0        0       86 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/organization_id.py
--rw-r--r--   0        0        0     1711 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/organization_request.py
--rw-r--r--   0        0        0     1808 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/organization_response.py
--rw-r--r--   0        0        0     1142 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/payment_methods_request.py
--rw-r--r--   0        0        0     1148 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/payment_methods_response.py
--rw-r--r--   0        0        0      849 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/payment_rail_markup.py
--rw-r--r--   0        0        0      482 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/payment_rail_markup_type.py
--rw-r--r--   0        0        0     1151 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/payment_rail_request.py
--rw-r--r--   0        0        0      843 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/organization_types/types/payment_rail_response.py
--rw-r--r--   0        0        0       65 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/payment_method_schema/__init__.py
--rw-r--r--   0        0        0    15390 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/payment_method_schema/client.py
--rw-r--r--   0        0        0     2547 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/__init__.py
--rw-r--r--   0        0        0     3587 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/__init__.py
--rw-r--r--   0        0        0     1336 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/bank_account_base_request.py
--rw-r--r--   0        0        0     1466 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/bank_account_base_response.py
--rw-r--r--   0        0        0     1026 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/bank_account_request.py
--rw-r--r--   0        0        0     1014 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/bank_account_response.py
--rw-r--r--   0        0        0      960 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/bank_status.py
--rw-r--r--   0        0        0      632 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/bank_type.py
--rw-r--r--   0        0        0     1247 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/card_base_request.py
--rw-r--r--   0        0        0     1468 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/card_base_response.py
--rw-r--r--   0        0        0      819 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/card_brand.py
--rw-r--r--   0        0        0      961 2023-08-01 00:16:04.699749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/card_request.py
--rw-r--r--   0        0        0      935 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/card_response.py
--rw-r--r--   0        0        0      750 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/card_type.py
--rw-r--r--   0        0        0     1258 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/check_base_request.py
--rw-r--r--   0        0        0     1494 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/check_base_response.py
--rw-r--r--   0        0        0      967 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/check_request.py
--rw-r--r--   0        0        0      941 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/check_response.py
--rw-r--r--   0        0        0    22179 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/currency_code.py
--rw-r--r--   0        0        0     1607 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_request.py
--rw-r--r--   0        0        0     2026 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_response.py
--rw-r--r--   0        0        0     1040 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/custom_payment_method_request.py
--rw-r--r--   0        0        0     1028 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/custom_payment_method_response.py
--rw-r--r--   0        0        0     1613 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_base_request.py
--rw-r--r--   0        0        0     1071 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_request.py
--rw-r--r--   0        0        0       87 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_id.py
--rw-r--r--   0        0        0     1264 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_request.py
--rw-r--r--   0        0        0     1298 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_response.py
--rw-r--r--   0        0        0     1984 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_schema_field.py
--rw-r--r--   0        0        0      682 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_schema_field_type.py
--rw-r--r--   0        0        0       93 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_schema_id.py
--rw-r--r--   0        0        0     1581 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_schema_request.py
--rw-r--r--   0        0        0     1693 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_schema_response.py
--rw-r--r--   0        0        0     1229 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_type.py
--rw-r--r--   0        0        0      514 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_update_request.py
--rw-r--r--   0        0        0     1042 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/plaid_link_request.py
--rw-r--r--   0        0        0      271 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/transaction/__init__.py
--rw-r--r--   0        0        0     6642 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/transaction/client.py
--rw-r--r--   0        0        0      386 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/transaction/types/__init__.py
--rw-r--r--   0        0        0       85 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/transaction/types/transaction_id.py
--rw-r--r--   0        0        0     1138 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/transaction/types/transaction_response.py
--rw-r--r--   0        0        0     1582 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/transaction/types/transaction_response_expanded.py
--rw-r--r--   0        0        0     1261 2023-08-01 00:16:04.703749 mercoa-0.2.7/src/mercoa/resources/transaction/types/transaction_status.py
--rw-r--r--   0        0        0     2433 1970-01-01 00:00:00.000000 mercoa-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1930 2023-08-01 01:57:14.703607 mercoa-0.2.8/README.md
+-rw-r--r--   0        0        0      368 2023-08-01 01:57:14.703607 mercoa-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     8859 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/__init__.py
+-rw-r--r--   0        0        0     2384 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/client.py
+-rw-r--r--   0        0        0      348 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      157 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/environment.py
+-rw-r--r--   0        0        0        0 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/py.typed
+-rw-r--r--   0        0        0     8978 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/__init__.py
+-rw-r--r--   0        0        0      165 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/bank_lookup/__init__.py
+-rw-r--r--   0        0        0     3801 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/bank_lookup/client.py
+-rw-r--r--   0        0        0      205 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/bank_lookup/types/__init__.py
+-rw-r--r--   0        0        0      960 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/bank_lookup/types/bank_address.py
+-rw-r--r--   0        0        0      946 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py
+-rw-r--r--   0        0        0      499 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/commons/__init__.py
+-rw-r--r--   0        0        0      314 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/commons/errors/__init__.py
+-rw-r--r--   0        0        0      237 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/commons/errors/auth_header_malformed_error.py
+-rw-r--r--   0        0        0      221 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/commons/errors/auth_header_missing_error.py
+-rw-r--r--   0        0        0      225 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/commons/errors/unauthorized.py
+-rw-r--r--   0        0        0      469 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/commons/types/__init__.py
+-rw-r--r--   0        0        0     1093 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/commons/types/address.py
+-rw-r--r--   0        0        0      824 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/commons/types/birth_date.py
+-rw-r--r--   0        0        0      994 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/commons/types/full_name.py
+-rw-r--r--   0        0        0      850 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/commons/types/individual_government_id.py
+-rw-r--r--   0        0        0      857 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/commons/types/itin.py
+-rw-r--r--   0        0        0      441 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/commons/types/order_direction.py
+-rw-r--r--   0        0        0      855 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/commons/types/phone_number.py
+-rw-r--r--   0        0        0      856 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/commons/types/ssn.py
+-rw-r--r--   0        0        0      523 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/__init__.py
+-rw-r--r--   0        0        0    40498 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/client.py
+-rw-r--r--   0        0        0      501 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/__init__.py
+-rw-r--r--   0        0        0      228 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/approval_policy/__init__.py
+-rw-r--r--   0        0        0    17689 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/approval_policy/client.py
+-rw-r--r--   0        0        0      305 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/approval_policy/errors/__init__.py
+-rw-r--r--   0        0        0      242 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/approval_policy/errors/num_approver_less_than_one_error.py
+-rw-r--r--   0        0        0      248 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/approval_policy/errors/num_approvers_user_list_mismatch_error.py
+-rw-r--r--   0        0        0       65 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/counterparty/__init__.py
+-rw-r--r--   0        0        0     4109 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/counterparty/client.py
+-rw-r--r--   0        0        0       65 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/invoice/__init__.py
+-rw-r--r--   0        0        0    11215 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/invoice/client.py
+-rw-r--r--   0        0        0       65 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/notification_policy/__init__.py
+-rw-r--r--   0        0        0    10326 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/notification_policy/client.py
+-rw-r--r--   0        0        0       65 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/payment_method/__init__.py
+-rw-r--r--   0        0        0    22306 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/payment_method/client.py
+-rw-r--r--   0        0        0       65 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/representative/__init__.py
+-rw-r--r--   0        0        0    12767 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/representative/client.py
+-rw-r--r--   0        0        0      175 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/user/__init__.py
+-rw-r--r--   0        0        0    21722 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/user/client.py
+-rw-r--r--   0        0        0      166 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/user/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/user/resources/notification_policy/__init__.py
+-rw-r--r--   0        0        0    10769 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/user/resources/notification_policy/client.py
+-rw-r--r--   0        0        0       65 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/user/resources/notifications/__init__.py
+-rw-r--r--   0        0        0     8720 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/user/resources/notifications/client.py
+-rw-r--r--   0        0        0     2745 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/__init__.py
+-rw-r--r--   0        0        0     4074 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/__init__.py
+-rw-r--r--   0        0        0      487 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/account_type.py
+-rw-r--r--   0        0        0      849 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/amount_trigger.py
+-rw-r--r--   0        0        0       88 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/approval_policy_id.py
+-rw-r--r--   0        0        0     1100 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/approval_policy_request.py
+-rw-r--r--   0        0        0     1036 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/approval_policy_response.py
+-rw-r--r--   0        0        0     1067 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/approval_policy_update_request.py
+-rw-r--r--   0        0        0      963 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/approver_rule.py
+-rw-r--r--   0        0        0     1451 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/business_profile_request.py
+-rw-r--r--   0        0        0     1509 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/business_profile_response.py
+-rw-r--r--   0        0        0     1917 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/business_type.py
+-rw-r--r--   0        0        0     1013 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/counterparty_response.py
+-rw-r--r--   0        0        0      741 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/ein.py
+-rw-r--r--   0        0        0      914 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/entity_add_payees_request.py
+-rw-r--r--   0        0        0       80 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/entity_id.py
+-rw-r--r--   0        0        0     2432 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/entity_request.py
+-rw-r--r--   0        0        0     1814 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/entity_response.py
+-rw-r--r--   0        0        0     1084 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/entity_status.py
+-rw-r--r--   0        0        0     2084 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/entity_update_request.py
+-rw-r--r--   0        0        0       84 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/entity_user_id.py
+-rw-r--r--   0        0        0     1100 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/entity_user_request.py
+-rw-r--r--   0        0        0     1224 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/entity_user_response.py
+-rw-r--r--   0        0        0     1446 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/find_counterparties_response.py
+-rw-r--r--   0        0        0     1343 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/find_entity_response.py
+-rw-r--r--   0        0        0     1367 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/find_notification_response.py
+-rw-r--r--   0        0        0      633 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/identifier_list.py
+-rw-r--r--   0        0        0     1372 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/individual_profile_request.py
+-rw-r--r--   0        0        0     1206 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/individual_profile_response.py
+-rw-r--r--   0        0        0       86 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/notification_id.py
+-rw-r--r--   0        0        0     1051 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/notification_policy_request.py
+-rw-r--r--   0        0        0     1127 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/notification_policy_response.py
+-rw-r--r--   0        0        0     1129 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/notification_response.py
+-rw-r--r--   0        0        0     1945 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/notification_type.py
+-rw-r--r--   0        0        0      974 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/profile_request.py
+-rw-r--r--   0        0        0      981 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/profile_response.py
+-rw-r--r--   0        0        0       88 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/representative_id.py
+-rw-r--r--   0        0        0     1370 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/representative_request.py
+-rw-r--r--   0        0        0     1539 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/representative_response.py
+-rw-r--r--   0        0        0     1100 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/responsibilities.py
+-rw-r--r--   0        0        0      391 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/rule.py
+-rw-r--r--   0        0        0      761 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/tax_id.py
+-rw-r--r--   0        0        0      854 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/token_generation_invoice_options.py
+-rw-r--r--   0        0        0     1269 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/token_generation_options.py
+-rw-r--r--   0        0        0      963 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/token_generation_pages_options.py
+-rw-r--r--   0        0        0      857 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/token_generation_style_options.py
+-rw-r--r--   0        0        0      951 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/token_generation_vendor_options.py
+-rw-r--r--   0        0        0      573 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/trigger.py
+-rw-r--r--   0        0        0      947 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/user_notification_policy_response.py
+-rw-r--r--   0        0        0      627 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/vendor_network.py
+-rw-r--r--   0        0        0      163 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/invoice/__init__.py
+-rw-r--r--   0        0        0    20874 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/invoice/client.py
+-rw-r--r--   0        0        0      154 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/invoice/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/invoice/resources/approval/__init__.py
+-rw-r--r--   0        0        0     6559 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/invoice/resources/approval/client.py
+-rw-r--r--   0        0        0       65 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice/resources/comment/__init__.py
+-rw-r--r--   0        0        0    15332 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice/resources/comment/client.py
+-rw-r--r--   0        0        0       65 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice/resources/document/__init__.py
+-rw-r--r--   0        0        0     3870 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice/resources/document/client.py
+-rw-r--r--   0        0        0      991 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/__init__.py
+-rw-r--r--   0        0        0     1480 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/__init__.py
+-rw-r--r--   0        0        0     1017 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/approval_request.py
+-rw-r--r--   0        0        0     1592 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/approval_slot.py
+-rw-r--r--   0        0        0     1147 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/approval_slot_assignment.py
+-rw-r--r--   0        0        0       86 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/approval_slot_id.py
+-rw-r--r--   0        0        0      631 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/approver_action.py
+-rw-r--r--   0        0        0      984 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/associated_approval_action.py
+-rw-r--r--   0        0        0       81 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/comment_id.py
+-rw-r--r--   0        0        0      934 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/comment_request.py
+-rw-r--r--   0        0        0     1428 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/comment_response.py
+-rw-r--r--   0        0        0      851 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/document_response.py
+-rw-r--r--   0        0        0     1347 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/find_invoice_response.py
+-rw-r--r--   0        0        0       81 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/invoice_id.py
+-rw-r--r--   0        0        0     1331 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/invoice_line_item_request.py
+-rw-r--r--   0        0        0     1258 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/invoice_line_item_response.py
+-rw-r--r--   0        0        0     1072 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/invoice_metrics_response.py
+-rw-r--r--   0        0        0      870 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/invoice_order_by_field.py
+-rw-r--r--   0        0        0     3578 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/invoice_request.py
+-rw-r--r--   0        0        0     4306 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/invoice_response.py
+-rw-r--r--   0        0        0     1485 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/invoice_status.py
+-rw-r--r--   0        0        0      123 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/ocr/__init__.py
+-rw-r--r--   0        0        0     4438 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/ocr/client.py
+-rw-r--r--   0        0        0      130 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/ocr/types/__init__.py
+-rw-r--r--   0        0        0     1258 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/ocr/types/ocr_response.py
+-rw-r--r--   0        0        0      157 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization/__init__.py
+-rw-r--r--   0        0        0    11712 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization/client.py
+-rw-r--r--   0        0        0      148 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization/resources/notification_configuration/__init__.py
+-rw-r--r--   0        0        0    10288 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization/resources/notification_configuration/client.py
+-rw-r--r--   0        0        0     1607 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/__init__.py
+-rw-r--r--   0        0        0     2348 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/__init__.py
+-rw-r--r--   0        0        0      948 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/color_scheme_request.py
+-rw-r--r--   0        0        0      949 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/color_scheme_response.py
+-rw-r--r--   0        0        0      981 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/email_log_response.py
+-rw-r--r--   0        0        0      932 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/email_provider_request.py
+-rw-r--r--   0        0        0      936 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/email_provider_response.py
+-rw-r--r--   0        0        0      785 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/email_sender_provider.py
+-rw-r--r--   0        0        0     1052 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/email_sender_request.py
+-rw-r--r--   0        0        0     1044 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/email_sender_response.py
+-rw-r--r--   0        0        0      926 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/global_notification_configuration_request.py
+-rw-r--r--   0        0        0      774 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/invoice_notification_configuration_request.py
+-rw-r--r--   0        0        0     1004 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/invoice_notification_configuration_response.py
+-rw-r--r--   0        0        0      627 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/notification_configuration_request.py
+-rw-r--r--   0        0        0      633 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/notification_configuration_response.py
+-rw-r--r--   0        0        0       86 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/organization_id.py
+-rw-r--r--   0        0        0     1711 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/organization_request.py
+-rw-r--r--   0        0        0     1808 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/organization_response.py
+-rw-r--r--   0        0        0     1142 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/payment_methods_request.py
+-rw-r--r--   0        0        0     1148 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/payment_methods_response.py
+-rw-r--r--   0        0        0      849 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/payment_rail_markup.py
+-rw-r--r--   0        0        0      482 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/payment_rail_markup_type.py
+-rw-r--r--   0        0        0     1151 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/payment_rail_request.py
+-rw-r--r--   0        0        0      843 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/payment_rail_response.py
+-rw-r--r--   0        0        0       65 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_schema/__init__.py
+-rw-r--r--   0        0        0    15390 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_schema/client.py
+-rw-r--r--   0        0        0     2547 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/__init__.py
+-rw-r--r--   0        0        0     3587 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/__init__.py
+-rw-r--r--   0        0        0     1336 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/bank_account_base_request.py
+-rw-r--r--   0        0        0     1466 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/bank_account_base_response.py
+-rw-r--r--   0        0        0     1026 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/bank_account_request.py
+-rw-r--r--   0        0        0     1014 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/bank_account_response.py
+-rw-r--r--   0        0        0      960 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/bank_status.py
+-rw-r--r--   0        0        0      632 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/bank_type.py
+-rw-r--r--   0        0        0     1247 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/card_base_request.py
+-rw-r--r--   0        0        0     1468 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/card_base_response.py
+-rw-r--r--   0        0        0      819 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/card_brand.py
+-rw-r--r--   0        0        0      961 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/card_request.py
+-rw-r--r--   0        0        0      935 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/card_response.py
+-rw-r--r--   0        0        0      750 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/card_type.py
+-rw-r--r--   0        0        0     1258 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/check_base_request.py
+-rw-r--r--   0        0        0     1494 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/check_base_response.py
+-rw-r--r--   0        0        0      967 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/check_request.py
+-rw-r--r--   0        0        0      941 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/check_response.py
+-rw-r--r--   0        0        0    22179 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/currency_code.py
+-rw-r--r--   0        0        0     1607 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_request.py
+-rw-r--r--   0        0        0     2026 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_response.py
+-rw-r--r--   0        0        0     1040 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/custom_payment_method_request.py
+-rw-r--r--   0        0        0     1028 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/custom_payment_method_response.py
+-rw-r--r--   0        0        0     1613 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_base_request.py
+-rw-r--r--   0        0        0     1071 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_request.py
+-rw-r--r--   0        0        0       87 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_id.py
+-rw-r--r--   0        0        0     1264 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_request.py
+-rw-r--r--   0        0        0     1298 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_response.py
+-rw-r--r--   0        0        0     1984 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_schema_field.py
+-rw-r--r--   0        0        0      682 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_schema_field_type.py
+-rw-r--r--   0        0        0       93 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_schema_id.py
+-rw-r--r--   0        0        0     1581 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_schema_request.py
+-rw-r--r--   0        0        0     1693 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_schema_response.py
+-rw-r--r--   0        0        0     1229 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_type.py
+-rw-r--r--   0        0        0      514 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_update_request.py
+-rw-r--r--   0        0        0     1042 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/plaid_link_request.py
+-rw-r--r--   0        0        0      271 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/transaction/__init__.py
+-rw-r--r--   0        0        0     6642 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/transaction/client.py
+-rw-r--r--   0        0        0      386 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/transaction/types/__init__.py
+-rw-r--r--   0        0        0       85 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/transaction/types/transaction_id.py
+-rw-r--r--   0        0        0     1138 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/transaction/types/transaction_response.py
+-rw-r--r--   0        0        0     1582 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/transaction/types/transaction_response_expanded.py
+-rw-r--r--   0        0        0     1261 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/transaction/types/transaction_status.py
+-rw-r--r--   0        0        0     2433 1970-01-01 00:00:00.000000 mercoa-0.2.8/PKG-INFO
```

### Comparing `mercoa-0.2.7/README.md` & `mercoa-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/__init__.py` & `mercoa-0.2.8/src/mercoa/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/client.py` & `mercoa-0.2.8/src/mercoa/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/core/datetime_utils.py` & `mercoa-0.2.8/src/mercoa/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/core/jsonable_encoder.py` & `mercoa-0.2.8/src/mercoa/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/__init__.py` & `mercoa-0.2.8/src/mercoa/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/bank_lookup/client.py` & `mercoa-0.2.8/src/mercoa/resources/bank_lookup/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/bank_lookup/types/bank_address.py` & `mercoa-0.2.8/src/mercoa/resources/bank_lookup/types/bank_address.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py` & `mercoa-0.2.8/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/commons/types/address.py` & `mercoa-0.2.8/src/mercoa/resources/commons/types/address.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/commons/types/birth_date.py` & `mercoa-0.2.8/src/mercoa/resources/commons/types/birth_date.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/commons/types/full_name.py` & `mercoa-0.2.8/src/mercoa/resources/commons/types/full_name.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/commons/types/individual_government_id.py` & `mercoa-0.2.8/src/mercoa/resources/commons/types/individual_government_id.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/commons/types/itin.py` & `mercoa-0.2.8/src/mercoa/resources/commons/types/itin.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/commons/types/phone_number.py` & `mercoa-0.2.8/src/mercoa/resources/commons/types/phone_number.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/commons/types/ssn.py` & `mercoa-0.2.8/src/mercoa/resources/commons/types/ssn.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity/__init__.py` & `mercoa-0.2.8/src/mercoa/resources/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity/client.py` & `mercoa-0.2.8/src/mercoa/resources/entity/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity/resources/approval_policy/client.py` & `mercoa-0.2.8/src/mercoa/resources/entity/resources/approval_policy/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity/resources/counterparty/client.py` & `mercoa-0.2.8/src/mercoa/resources/entity/resources/counterparty/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity/resources/invoice/client.py` & `mercoa-0.2.8/src/mercoa/resources/entity/resources/invoice/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity/resources/notification_policy/client.py` & `mercoa-0.2.8/src/mercoa/resources/entity/resources/notification_policy/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity/resources/payment_method/client.py` & `mercoa-0.2.8/src/mercoa/resources/entity/resources/payment_method/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity/resources/representative/client.py` & `mercoa-0.2.8/src/mercoa/resources/entity/resources/representative/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity/resources/user/client.py` & `mercoa-0.2.8/src/mercoa/resources/entity/resources/user/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity/resources/user/resources/notification_policy/client.py` & `mercoa-0.2.8/src/mercoa/resources/entity/resources/user/resources/notification_policy/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity/resources/user/resources/notifications/client.py` & `mercoa-0.2.8/src/mercoa/resources/entity/resources/user/resources/notifications/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/__init__.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/__init__.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/amount_trigger.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/amount_trigger.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/approval_policy_request.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/approval_policy_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/approval_policy_response.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/approval_policy_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/approval_policy_update_request.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/approval_policy_update_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/approver_rule.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/approver_rule.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/business_profile_request.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/business_profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/business_profile_response.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/business_profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/business_type.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/business_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/counterparty_response.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/counterparty_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/ein.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/ein.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/entity_add_payees_request.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/entity_add_payees_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/entity_request.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/entity_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/entity_response.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/entity_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/entity_status.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/entity_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/entity_update_request.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/entity_update_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/entity_user_request.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/entity_user_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/entity_user_response.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/entity_user_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/find_counterparties_response.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/find_counterparties_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/find_entity_response.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/find_entity_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/find_notification_response.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/find_notification_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/identifier_list.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/identifier_list.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/individual_profile_request.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/individual_profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/individual_profile_response.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/individual_profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/notification_policy_request.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/notification_policy_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/notification_policy_response.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/notification_policy_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/notification_response.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/notification_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/notification_type.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/notification_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/profile_request.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/profile_response.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/representative_request.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/representative_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/representative_response.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/representative_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/responsibilities.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/responsibilities.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/tax_id.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/tax_id.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/token_generation_invoice_options.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/token_generation_invoice_options.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/token_generation_options.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/token_generation_options.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/token_generation_pages_options.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/token_generation_pages_options.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/token_generation_style_options.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/token_generation_style_options.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/token_generation_vendor_options.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/token_generation_vendor_options.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/trigger.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/trigger.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/user_notification_policy_response.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/user_notification_policy_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/entity_types/types/vendor_network.py` & `mercoa-0.2.8/src/mercoa/resources/entity_types/types/vendor_network.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/invoice/client.py` & `mercoa-0.2.8/src/mercoa/resources/invoice/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/invoice/resources/approval/client.py` & `mercoa-0.2.8/src/mercoa/resources/invoice/resources/approval/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/invoice/resources/comment/client.py` & `mercoa-0.2.8/src/mercoa/resources/invoice/resources/comment/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/invoice/resources/document/client.py` & `mercoa-0.2.8/src/mercoa/resources/invoice/resources/document/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/invoice_types/__init__.py` & `mercoa-0.2.8/src/mercoa/resources/invoice_types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/invoice_types/types/__init__.py` & `mercoa-0.2.8/src/mercoa/resources/invoice_types/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/invoice_types/types/approval_request.py` & `mercoa-0.2.8/src/mercoa/resources/invoice_types/types/approval_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/invoice_types/types/approval_slot.py` & `mercoa-0.2.8/src/mercoa/resources/invoice_types/types/approval_slot.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/invoice_types/types/approval_slot_assignment.py` & `mercoa-0.2.8/src/mercoa/resources/invoice_types/types/approval_slot_assignment.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/invoice_types/types/approver_action.py` & `mercoa-0.2.8/src/mercoa/resources/invoice_types/types/approver_action.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/invoice_types/types/associated_approval_action.py` & `mercoa-0.2.8/src/mercoa/resources/invoice_types/types/associated_approval_action.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/invoice_types/types/comment_request.py` & `mercoa-0.2.8/src/mercoa/resources/invoice_types/types/comment_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/invoice_types/types/comment_response.py` & `mercoa-0.2.8/src/mercoa/resources/invoice_types/types/comment_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/invoice_types/types/document_response.py` & `mercoa-0.2.8/src/mercoa/resources/invoice_types/types/document_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/invoice_types/types/find_invoice_response.py` & `mercoa-0.2.8/src/mercoa/resources/invoice_types/types/find_invoice_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/invoice_types/types/invoice_line_item_request.py` & `mercoa-0.2.8/src/mercoa/resources/invoice_types/types/invoice_line_item_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/invoice_types/types/invoice_line_item_response.py` & `mercoa-0.2.8/src/mercoa/resources/invoice_types/types/invoice_line_item_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/invoice_types/types/invoice_metrics_response.py` & `mercoa-0.2.8/src/mercoa/resources/invoice_types/types/invoice_metrics_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/invoice_types/types/invoice_order_by_field.py` & `mercoa-0.2.8/src/mercoa/resources/invoice_types/types/invoice_order_by_field.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/invoice_types/types/invoice_request.py` & `mercoa-0.2.8/src/mercoa/resources/invoice_types/types/invoice_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/invoice_types/types/invoice_response.py` & `mercoa-0.2.8/src/mercoa/resources/invoice_types/types/invoice_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/invoice_types/types/invoice_status.py` & `mercoa-0.2.8/src/mercoa/resources/invoice_types/types/invoice_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/ocr/client.py` & `mercoa-0.2.8/src/mercoa/resources/ocr/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/ocr/types/ocr_response.py` & `mercoa-0.2.8/src/mercoa/resources/ocr/types/ocr_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/organization/client.py` & `mercoa-0.2.8/src/mercoa/resources/organization/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/organization/resources/notification_configuration/client.py` & `mercoa-0.2.8/src/mercoa/resources/organization/resources/notification_configuration/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/organization_types/__init__.py` & `mercoa-0.2.8/src/mercoa/resources/organization_types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/organization_types/types/__init__.py` & `mercoa-0.2.8/src/mercoa/resources/organization_types/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/organization_types/types/color_scheme_request.py` & `mercoa-0.2.8/src/mercoa/resources/organization_types/types/color_scheme_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/organization_types/types/color_scheme_response.py` & `mercoa-0.2.8/src/mercoa/resources/organization_types/types/color_scheme_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/organization_types/types/email_log_response.py` & `mercoa-0.2.8/src/mercoa/resources/organization_types/types/email_log_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/organization_types/types/email_provider_request.py` & `mercoa-0.2.8/src/mercoa/resources/organization_types/types/email_provider_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/organization_types/types/email_provider_response.py` & `mercoa-0.2.8/src/mercoa/resources/organization_types/types/email_provider_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/organization_types/types/email_sender_provider.py` & `mercoa-0.2.8/src/mercoa/resources/organization_types/types/email_sender_provider.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/organization_types/types/email_sender_request.py` & `mercoa-0.2.8/src/mercoa/resources/organization_types/types/email_sender_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/organization_types/types/email_sender_response.py` & `mercoa-0.2.8/src/mercoa/resources/organization_types/types/email_sender_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/organization_types/types/global_notification_configuration_request.py` & `mercoa-0.2.8/src/mercoa/resources/organization_types/types/global_notification_configuration_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/organization_types/types/invoice_notification_configuration_request.py` & `mercoa-0.2.8/src/mercoa/resources/organization_types/types/invoice_notification_configuration_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/organization_types/types/invoice_notification_configuration_response.py` & `mercoa-0.2.8/src/mercoa/resources/organization_types/types/invoice_notification_configuration_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/organization_types/types/notification_configuration_request.py` & `mercoa-0.2.8/src/mercoa/resources/organization_types/types/notification_configuration_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/organization_types/types/notification_configuration_response.py` & `mercoa-0.2.8/src/mercoa/resources/organization_types/types/notification_configuration_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/organization_types/types/organization_request.py` & `mercoa-0.2.8/src/mercoa/resources/organization_types/types/organization_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/organization_types/types/organization_response.py` & `mercoa-0.2.8/src/mercoa/resources/organization_types/types/organization_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/organization_types/types/payment_methods_request.py` & `mercoa-0.2.8/src/mercoa/resources/organization_types/types/payment_methods_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/organization_types/types/payment_methods_response.py` & `mercoa-0.2.8/src/mercoa/resources/organization_types/types/payment_methods_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/organization_types/types/payment_rail_markup.py` & `mercoa-0.2.8/src/mercoa/resources/organization_types/types/payment_rail_markup.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/organization_types/types/payment_rail_request.py` & `mercoa-0.2.8/src/mercoa/resources/organization_types/types/payment_rail_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/organization_types/types/payment_rail_response.py` & `mercoa-0.2.8/src/mercoa/resources/organization_types/types/payment_rail_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/payment_method_schema/client.py` & `mercoa-0.2.8/src/mercoa/resources/payment_method_schema/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/payment_method_types/__init__.py` & `mercoa-0.2.8/src/mercoa/resources/payment_method_types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/__init__.py` & `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/bank_account_base_request.py` & `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/bank_account_base_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/bank_account_base_response.py` & `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/bank_account_base_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/bank_account_request.py` & `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/bank_account_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/bank_account_response.py` & `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/bank_account_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/bank_status.py` & `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/bank_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/bank_type.py` & `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/bank_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/card_base_request.py` & `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/card_base_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/card_base_response.py` & `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/card_base_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/card_brand.py` & `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/card_brand.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/card_request.py` & `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/card_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/card_response.py` & `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/card_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/card_type.py` & `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/card_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/check_base_request.py` & `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/check_base_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/check_base_response.py` & `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/check_base_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/check_request.py` & `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/check_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/check_response.py` & `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/check_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/currency_code.py` & `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/currency_code.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_request.py` & `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_response.py` & `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/custom_payment_method_request.py` & `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/custom_payment_method_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/custom_payment_method_response.py` & `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/custom_payment_method_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_base_request.py` & `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_base_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_request.py` & `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_request.py` & `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_response.py` & `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_schema_field.py` & `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_schema_field.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_schema_field_type.py` & `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_schema_field_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_schema_request.py` & `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_schema_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_schema_response.py` & `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_schema_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_type.py` & `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/payment_method_update_request.py` & `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_update_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/payment_method_types/types/plaid_link_request.py` & `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/plaid_link_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/transaction/client.py` & `mercoa-0.2.8/src/mercoa/resources/transaction/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/transaction/types/transaction_response.py` & `mercoa-0.2.8/src/mercoa/resources/transaction/types/transaction_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/transaction/types/transaction_response_expanded.py` & `mercoa-0.2.8/src/mercoa/resources/transaction/types/transaction_response_expanded.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/src/mercoa/resources/transaction/types/transaction_status.py` & `mercoa-0.2.8/src/mercoa/resources/transaction/types/transaction_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.7/PKG-INFO` & `mercoa-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercoa
-Version: 0.2.7
+Version: 0.2.8
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

