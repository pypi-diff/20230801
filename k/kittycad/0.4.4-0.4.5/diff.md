# Comparing `tmp/kittycad-0.4.4.tar.gz` & `tmp/kittycad-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kittycad-0.4.4.tar", max compression
+gzip compressed data, was "kittycad-0.4.5.tar", max compression
```

## Comparing `kittycad-0.4.4.tar` & `kittycad-0.4.5.tar`

### file list

```diff
@@ -1,240 +1,241 @@
--rw-r--r--   0        0        0     1065 2023-07-08 02:25:21.114181 kittycad-0.4.4/LICENSE
--rw-r--r--   0        0        0      875 2023-07-08 02:25:21.114181 kittycad-0.4.4/README.md
--rw-r--r--   0        0        0       48 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/__init__.py
--rw-r--r--   0        0        0       47 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/__init__.py
--rw-r--r--   0        0        0      119 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/ai/__init__.py
--rw-r--r--   0        0        0     3781 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/ai/create_image_to_3d.py
--rw-r--r--   0        0        0     3559 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/ai/create_text_to_3d.py
--rw-r--r--   0        0        0      199 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/api_calls/__init__.py
--rw-r--r--   0        0        0     3110 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/api_calls/get_api_call.py
--rw-r--r--   0        0        0     2799 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/api_calls/get_api_call_for_user.py
--rw-r--r--   0        0        0     3243 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/api_calls/get_api_call_metrics.py
--rw-r--r--   0        0        0     6149 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/api_calls/get_async_operation.py
--rw-r--r--   0        0        0     4236 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/api_calls/list_api_calls.py
--rw-r--r--   0        0        0     5005 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/api_calls/list_api_calls_for_user.py
--rw-r--r--   0        0        0     4815 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/api_calls/list_async_operations.py
--rw-r--r--   0        0        0     4351 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/api_calls/user_list_api_calls.py
--rw-r--r--   0        0        0      352 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/api_tokens/__init__.py
--rw-r--r--   0        0        0     2573 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/api_tokens/create_api_token_for_user.py
--rw-r--r--   0        0        0     2879 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/api_tokens/delete_api_token_for_user.py
--rw-r--r--   0        0        0     2784 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/api_tokens/get_api_token_for_user.py
--rw-r--r--   0        0        0     4284 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/api_tokens/list_api_tokens_for_user.py
--rw-r--r--   0        0        0      116 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/apps/__init__.py
--rw-r--r--   0        0        0     2597 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/apps/apps_github_callback.py
--rw-r--r--   0        0        0     2911 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/apps/apps_github_consent.py
--rw-r--r--   0        0        0     2338 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/apps/apps_github_webhook.py
--rw-r--r--   0        0        0      156 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/beta/__init__.py
--rw-r--r--   0        0        0      118 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/constant/__init__.py
--rw-r--r--   0        0        0     2758 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/constant/get_physics_constant.py
--rw-r--r--   0        0        0      161 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/executor/__init__.py
--rw-r--r--   0        0        0     1781 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/executor/create_executor_term.py
--rw-r--r--   0        0        0     3195 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/executor/create_file_execution.py
--rw-r--r--   0        0        0      233 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/file/__init__.py
--rw-r--r--   0        0        0     4635 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/file/create_file_center_of_mass.py
--rw-r--r--   0        0        0     4653 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/file/create_file_conversion.py
--rw-r--r--   0        0        0     1962 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/file/create_file_conversion_with_base64_helper.py
--rw-r--r--   0        0        0     5162 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/file/create_file_density.py
--rw-r--r--   0        0        0     5290 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/file/create_file_mass.py
--rw-r--r--   0        0        0     4559 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/file/create_file_surface_area.py
--rw-r--r--   0        0        0     4487 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/file/create_file_volume.py
--rw-r--r--   0        0        0     1341 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/file/get_file_conversion_with_base64_helper.py
--rw-r--r--   0        0        0      133 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/hidden/__init__.py
--rw-r--r--   0        0        0     2729 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/hidden/auth_email.py
--rw-r--r--   0        0        0     3220 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/hidden/auth_email_callback.py
--rw-r--r--   0        0        0     2139 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/hidden/logout.py
--rw-r--r--   0        0        0      105 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/meta/__init__.py
--rw-r--r--   0        0        0     2383 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/meta/get_ai_plugin_manifest.py
--rw-r--r--   0        0        0     2629 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/meta/get_metadata.py
--rw-r--r--   0        0        0     2564 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/meta/get_openai_schema.py
--rw-r--r--   0        0        0     2193 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/meta/get_schema.py
--rw-r--r--   0        0        0     2245 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/meta/ping.py
--rw-r--r--   0        0        0      144 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/modeling/__init__.py
--rw-r--r--   0        0        0     2794 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/modeling/cmd.py
--rw-r--r--   0        0        0     2701 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/modeling/cmd_batch.py
--rw-r--r--   0        0        0     1995 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/modeling/modeling_commands_ws.py
--rw-r--r--   0        0        0      123 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/oauth2/__init__.py
--rw-r--r--   0        0        0      117 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/payments/__init__.py
--rw-r--r--   0        0        0     2956 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/payments/create_payment_information_for_user.py
--rw-r--r--   0        0        0     2638 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/payments/create_payment_intent_for_user.py
--rw-r--r--   0        0        0     2431 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/payments/delete_payment_information_for_user.py
--rw-r--r--   0        0        0     2486 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/payments/delete_payment_method_for_user.py
--rw-r--r--   0        0        0     2655 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/payments/get_payment_balance_for_user.py
--rw-r--r--   0        0        0     2681 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/payments/get_payment_information_for_user.py
--rw-r--r--   0        0        0     2616 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/payments/list_invoices_for_user.py
--rw-r--r--   0        0        0     2684 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/payments/list_payment_methods_for_user.py
--rw-r--r--   0        0        0     2954 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/payments/update_payment_information_for_user.py
--rw-r--r--   0        0        0     2483 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/payments/validate_customer_tax_information_for_user.py
--rw-r--r--   0        0        0      101 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/unit/__init__.py
--rw-r--r--   0        0        0     3679 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/unit/get_angle_unit_conversion.py
--rw-r--r--   0        0        0     3653 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/unit/get_area_unit_conversion.py
--rw-r--r--   0        0        0     3729 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/unit/get_current_unit_conversion.py
--rw-r--r--   0        0        0     3703 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/unit/get_energy_unit_conversion.py
--rw-r--r--   0        0        0     3677 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/unit/get_force_unit_conversion.py
--rw-r--r--   0        0        0     3781 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/unit/get_frequency_unit_conversion.py
--rw-r--r--   0        0        0     3703 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/unit/get_length_unit_conversion.py
--rw-r--r--   0        0        0     3651 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/unit/get_mass_unit_conversion.py
--rw-r--r--   0        0        0     3677 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/unit/get_power_unit_conversion.py
--rw-r--r--   0        0        0     3755 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/unit/get_pressure_unit_conversion.py
--rw-r--r--   0        0        0     3833 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/unit/get_temperature_unit_conversion.py
--rw-r--r--   0        0        0     3703 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/unit/get_torque_unit_conversion.py
--rw-r--r--   0        0        0     3703 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/unit/get_volume_unit_conversion.py
--rw-r--r--   0        0        0      297 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/users/__init__.py
--rw-r--r--   0        0        0     2579 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/users/delete_user_self.py
--rw-r--r--   0        0        0     2757 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/users/get_session_for_user.py
--rw-r--r--   0        0        0     3061 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/users/get_user.py
--rw-r--r--   0        0        0     3185 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/users/get_user_extended.py
--rw-r--r--   0        0        0     2480 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/users/get_user_front_hash_self.py
--rw-r--r--   0        0        0     2506 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/users/get_user_onboarding_self.py
--rw-r--r--   0        0        0     2523 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/users/get_user_self.py
--rw-r--r--   0        0        0     2629 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/users/get_user_self_extended.py
--rw-r--r--   0        0        0     4105 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/users/list_users.py
--rw-r--r--   0        0        0     4187 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/users/list_users_extended.py
--rw-r--r--   0        0        0     2779 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/users/update_user_self.py
--rw-r--r--   0        0        0     2297 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/client.py
--rw-r--r--   0        0        0     5250 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/client_test.py
--rw-r--r--   0        0        0    96653 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/examples_test.py
--rw-r--r--   0        0        0     6234 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/__init__.py
--rw-r--r--   0        0        0      322 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/account_provider.py
--rw-r--r--   0        0        0     2258 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/ai_plugin_api.py
--rw-r--r--   0        0        0      242 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/ai_plugin_api_type.py
--rw-r--r--   0        0        0     2452 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/ai_plugin_auth.py
--rw-r--r--   0        0        0      413 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/ai_plugin_auth_type.py
--rw-r--r--   0        0        0      287 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/ai_plugin_http_auth_type.py
--rw-r--r--   0        0        0     4685 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/ai_plugin_manifest.py
--rw-r--r--   0        0        0     1720 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/api_call_query_group.py
--rw-r--r--   0        0        0      777 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/api_call_query_group_by.py
--rw-r--r--   0        0        0      620 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/api_call_status.py
--rw-r--r--   0        0        0     8592 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/api_call_with_price.py
--rw-r--r--   0        0        0     2128 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/api_call_with_price_results_page.py
--rw-r--r--   0        0        0     3455 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/api_token.py
--rw-r--r--   0        0        0     2004 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/api_token_results_page.py
--rw-r--r--   0        0        0     1447 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/app_client_info.py
--rw-r--r--   0        0        0     5928 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/async_api_call.py
--rw-r--r--   0        0        0    36592 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/async_api_call_output.py
--rw-r--r--   0        0        0     2066 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/async_api_call_results_page.py
--rw-r--r--   0        0        0      648 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/async_api_call_type.py
--rw-r--r--   0        0        0      421 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/axis.py
--rw-r--r--   0        0        0     2247 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/axis_direction_pair.py
--rw-r--r--   0        0        0     2127 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/billing_info.py
--rw-r--r--   0        0        0     1479 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/cache_metadata.py
--rw-r--r--   0        0        0      440 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/camera_drag_interaction_type.py
--rw-r--r--   0        0        0     3353 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/card_details.py
--rw-r--r--   0        0        0     2697 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/cluster.py
--rw-r--r--   0        0        0      409 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/code_language.py
--rw-r--r--   0        0        0     2244 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/code_output.py
--rw-r--r--   0        0        0     1732 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/commit.py
--rw-r--r--   0        0        0    14343 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/connection.py
--rw-r--r--   0        0        0    13513 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/country_code.py
--rw-r--r--   0        0        0     2120 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/coupon.py
--rw-r--r--   0        0        0      507 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/created_at_sort_mode.py
--rw-r--r--   0        0        0     8623 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/currency.py
--rw-r--r--   0        0        0     4314 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/customer.py
--rw-r--r--   0        0        0     4468 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/customer_balance.py
--rw-r--r--   0        0        0     2421 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/device_access_token_request_form.py
--rw-r--r--   0        0        0     1580 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/device_auth_request_form.py
--rw-r--r--   0        0        0     1606 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/device_auth_verify_params.py
--rw-r--r--   0        0        0      327 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/direction.py
--rw-r--r--   0        0        0     1684 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/discount.py
--rw-r--r--   0        0        0    21264 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/docker_system_info.py
--rw-r--r--   0        0        0     1789 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/email_authentication_form.py
--rw-r--r--   0        0        0     3860 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/engine_metadata.py
--rw-r--r--   0        0        0      529 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/environment.py
--rw-r--r--   0        0        0     1930 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/error.py
--rw-r--r--   0        0        0     2728 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/executor_metadata.py
--rw-r--r--   0        0        0     6069 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/extended_user.py
--rw-r--r--   0        0        0     2060 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/extended_user_results_page.py
--rw-r--r--   0        0        0     2120 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/extrude.py
--rw-r--r--   0        0        0     5881 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/file_center_of_mass.py
--rw-r--r--   0        0        0     7862 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/file_conversion.py
--rw-r--r--   0        0        0     5906 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/file_density.py
--rw-r--r--   0        0        0     1400 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/file_export_format.py
--rw-r--r--   0        0        0     1140 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/file_import_format.py
--rw-r--r--   0        0        0     5888 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/file_mass.py
--rw-r--r--   0        0        0     5703 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/file_surface_area.py
--rw-r--r--   0        0        0     1513 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/file_system_metadata.py
--rw-r--r--   0        0        0     5609 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/file_volume.py
--rw-r--r--   0        0        0     2304 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/gateway.py
--rw-r--r--   0        0        0      187 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/image_type.py
--rw-r--r--   0        0        0     2228 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/index_info.py
--rw-r--r--   0        0        0     6676 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/input_format.py
--rw-r--r--   0        0        0     8822 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/invoice.py
--rw-r--r--   0        0        0     2904 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/invoice_line_item.py
--rw-r--r--   0        0        0      563 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/invoice_status.py
--rw-r--r--   0        0        0     2666 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/jetstream.py
--rw-r--r--   0        0        0     1907 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/jetstream_api_stats.py
--rw-r--r--   0        0        0     2212 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/jetstream_config.py
--rw-r--r--   0        0        0     3174 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/jetstream_stats.py
--rw-r--r--   0        0        0     2125 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/leaf_node.py
--rw-r--r--   0        0        0     1337 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/mesh.py
--rw-r--r--   0        0        0     1923 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/meta_cluster_info.py
--rw-r--r--   0        0        0     5038 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/metadata.py
--rw-r--r--   0        0        0     1788 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/method.py
--rw-r--r--   0        0        0    12269 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/modeling_cmd.py
--rw-r--r--   0        0        0       76 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/modeling_cmd_id.py
--rw-r--r--   0        0        0     2456 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/modeling_cmd_req.py
--rw-r--r--   0        0        0     1752 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/modeling_cmd_req_batch.py
--rw-r--r--   0        0        0     2399 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/modeling_error.py
--rw-r--r--   0        0        0     1878 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/modeling_outcome.py
--rw-r--r--   0        0        0     1511 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/modeling_outcomes.py
--rw-r--r--   0        0        0     3094 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/new_address.py
--rw-r--r--   0        0        0     2038 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/o_auth2_client_info.py
--rw-r--r--   0        0        0      415 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/o_auth2_grant_type.py
--rw-r--r--   0        0        0     2509 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/onboarding.py
--rw-r--r--   0        0        0     1646 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/output_file.py
--rw-r--r--   0        0        0     7715 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/output_format.py
--rw-r--r--   0        0        0     6144 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/path_segment.py
--rw-r--r--   0        0        0     1527 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/payment_intent.py
--rw-r--r--   0        0        0     3760 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/payment_method.py
--rw-r--r--   0        0        0     2267 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/payment_method_card_checks.py
--rw-r--r--   0        0        0      294 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/payment_method_type.py
--rw-r--r--   0        0        0     5602 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/physics_constant.py
--rw-r--r--   0        0        0     4448 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/physics_constant_name.py
--rw-r--r--   0        0        0     2809 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/plugins_info.py
--rw-r--r--   0        0        0     1530 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/point2d.py
--rw-r--r--   0        0        0     1691 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/point3d.py
--rw-r--r--   0        0        0     1498 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/point_e_metadata.py
--rw-r--r--   0        0        0     1432 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/pong.py
--rw-r--r--   0        0        0     4187 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/registry_service_config.py
--rw-r--r--   0        0        0     2034 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/runtime.py
--rw-r--r--   0        0        0     3855 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/session.py
--rw-r--r--   0        0        0      656 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/storage.py
--rw-r--r--   0        0        0     2349 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/system.py
--rw-r--r--   0        0        0      214 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/system_info_cgroup_driver_enum.py
--rw-r--r--   0        0        0      175 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/system_info_cgroup_version_enum.py
--rw-r--r--   0        0        0     1663 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/system_info_default_address_pools.py
--rw-r--r--   0        0        0      213 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/system_info_isolation_enum.py
--rw-r--r--   0        0        0      377 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_angle.py
--rw-r--r--   0        0        0     6365 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_angle_conversion.py
--rw-r--r--   0        0        0     1937 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_area.py
--rw-r--r--   0        0        0     6354 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_area_conversion.py
--rw-r--r--   0        0        0      623 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_current.py
--rw-r--r--   0        0        0     6387 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_current_conversion.py
--rw-r--r--   0        0        0      934 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_energy.py
--rw-r--r--   0        0        0     6376 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_energy_conversion.py
--rw-r--r--   0        0        0      916 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_force.py
--rw-r--r--   0        0        0     6365 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_force_conversion.py
--rw-r--r--   0        0        0      997 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_frequency.py
--rw-r--r--   0        0        0     6409 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_frequency_conversion.py
--rw-r--r--   0        0        0     1522 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_length.py
--rw-r--r--   0        0        0     6376 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_length_conversion.py
--rw-r--r--   0        0        0     1754 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_mass.py
--rw-r--r--   0        0        0     6354 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_mass_conversion.py
--rw-r--r--   0        0        0     1014 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_power.py
--rw-r--r--   0        0        0     6365 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_power_conversion.py
--rw-r--r--   0        0        0      973 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_pressure.py
--rw-r--r--   0        0        0     6398 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_pressure_conversion.py
--rw-r--r--   0        0        0      593 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_temperature.py
--rw-r--r--   0        0        0     6431 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_temperature_conversion.py
--rw-r--r--   0        0        0      415 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_torque.py
--rw-r--r--   0        0        0     6376 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_torque_conversion.py
--rw-r--r--   0        0        0     2355 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_volume.py
--rw-r--r--   0        0        0     6376 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_volume_conversion.py
--rw-r--r--   0        0        0     2577 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/update_user.py
--rw-r--r--   0        0        0     5084 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/user.py
--rw-r--r--   0        0        0     1942 2023-07-08 02:25:21.858171 kittycad-0.4.4/kittycad/models/user_results_page.py
--rw-r--r--   0        0        0       67 2023-07-08 02:25:21.858171 kittycad-0.4.4/kittycad/models/uuid.py
--rw-r--r--   0        0        0     3448 2023-07-08 02:25:21.858171 kittycad-0.4.4/kittycad/models/verification_token.py
--rw-r--r--   0        0        0       26 2023-07-08 02:25:21.858171 kittycad-0.4.4/kittycad/py.typed
--rw-r--r--   0        0        0     1049 2023-07-08 02:25:21.858171 kittycad-0.4.4/kittycad/types.py
--rw-r--r--   0        0        0     2472 2023-07-08 02:25:21.858171 kittycad-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     1424 1970-01-01 00:00:00.000000 kittycad-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-01 01:14:07.377207 kittycad-0.4.5/LICENSE
+-rw-r--r--   0        0        0      875 2023-08-01 01:14:07.377207 kittycad-0.4.5/README.md
+-rw-r--r--   0        0        0       48 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/__init__.py
+-rw-r--r--   0        0        0       47 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/__init__.py
+-rw-r--r--   0        0        0      119 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/ai/__init__.py
+-rw-r--r--   0        0        0     3798 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/ai/create_image_to_3d.py
+-rw-r--r--   0        0        0     3569 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/ai/create_text_to_3d.py
+-rw-r--r--   0        0        0      199 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/api_calls/__init__.py
+-rw-r--r--   0        0        0     3133 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/api_calls/get_api_call.py
+-rw-r--r--   0        0        0     2822 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/api_calls/get_api_call_for_user.py
+-rw-r--r--   0        0        0     3259 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/api_calls/get_api_call_metrics.py
+-rw-r--r--   0        0        0     6182 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/api_calls/get_async_operation.py
+-rw-r--r--   0        0        0     4254 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/api_calls/list_api_calls.py
+-rw-r--r--   0        0        0     5041 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/api_calls/list_api_calls_for_user.py
+-rw-r--r--   0        0        0     4834 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/api_calls/list_async_operations.py
+-rw-r--r--   0        0        0     4379 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/api_calls/user_list_api_calls.py
+-rw-r--r--   0        0        0      352 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/api_tokens/__init__.py
+-rw-r--r--   0        0        0     2588 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/api_tokens/create_api_token_for_user.py
+-rw-r--r--   0        0        0     2898 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/api_tokens/delete_api_token_for_user.py
+-rw-r--r--   0        0        0     2793 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/api_tokens/get_api_token_for_user.py
+-rw-r--r--   0        0        0     4312 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/api_tokens/list_api_tokens_for_user.py
+-rw-r--r--   0        0        0      116 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/apps/__init__.py
+-rw-r--r--   0        0        0     2622 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/apps/apps_github_callback.py
+-rw-r--r--   0        0        0     2936 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/apps/apps_github_consent.py
+-rw-r--r--   0        0        0     2353 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/apps/apps_github_webhook.py
+-rw-r--r--   0        0        0      156 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/beta/__init__.py
+-rw-r--r--   0        0        0      118 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/constant/__init__.py
+-rw-r--r--   0        0        0     2765 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/constant/get_physics_constant.py
+-rw-r--r--   0        0        0      161 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/executor/__init__.py
+-rw-r--r--   0        0        0     1643 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/executor/create_executor_term.py
+-rw-r--r--   0        0        0     3217 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/executor/create_file_execution.py
+-rw-r--r--   0        0        0      233 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/file/__init__.py
+-rw-r--r--   0        0        0     5175 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/file/create_file_center_of_mass.py
+-rw-r--r--   0        0        0     4680 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/file/create_file_conversion.py
+-rw-r--r--   0        0        0     1962 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/file/create_file_conversion_with_base64_helper.py
+-rw-r--r--   0        0        0     6336 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/file/create_file_density.py
+-rw-r--r--   0        0        0     6518 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/file/create_file_mass.py
+-rw-r--r--   0        0        0     5085 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/file/create_file_surface_area.py
+-rw-r--r--   0        0        0     5027 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/file/create_file_volume.py
+-rw-r--r--   0        0        0     1341 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/file/get_file_conversion_with_base64_helper.py
+-rw-r--r--   0        0        0      133 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/hidden/__init__.py
+-rw-r--r--   0        0        0     2742 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/hidden/auth_email.py
+-rw-r--r--   0        0        0     3236 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/hidden/auth_email_callback.py
+-rw-r--r--   0        0        0     2154 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/hidden/logout.py
+-rw-r--r--   0        0        0      105 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/meta/__init__.py
+-rw-r--r--   0        0        0     2396 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/meta/get_ai_plugin_manifest.py
+-rw-r--r--   0        0        0     2644 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/meta/get_metadata.py
+-rw-r--r--   0        0        0     2579 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/meta/get_openai_schema.py
+-rw-r--r--   0        0        0     2206 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/meta/get_schema.py
+-rw-r--r--   0        0        0     2258 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/meta/ping.py
+-rw-r--r--   0        0        0      144 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/modeling/__init__.py
+-rw-r--r--   0        0        0     2809 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/modeling/cmd.py
+-rw-r--r--   0        0        0     2714 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/modeling/cmd_batch.py
+-rw-r--r--   0        0        0     1857 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/modeling/modeling_commands_ws.py
+-rw-r--r--   0        0        0      123 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/oauth2/__init__.py
+-rw-r--r--   0        0        0      117 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/payments/__init__.py
+-rw-r--r--   0        0        0     2981 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/payments/create_payment_information_for_user.py
+-rw-r--r--   0        0        0     2653 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/payments/create_payment_intent_for_user.py
+-rw-r--r--   0        0        0     2456 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/payments/delete_payment_information_for_user.py
+-rw-r--r--   0        0        0     2509 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/payments/delete_payment_method_for_user.py
+-rw-r--r--   0        0        0     2670 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/payments/get_payment_balance_for_user.py
+-rw-r--r--   0        0        0     2706 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/payments/get_payment_information_for_user.py
+-rw-r--r--   0        0        0     2631 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/payments/list_invoices_for_user.py
+-rw-r--r--   0        0        0     2699 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/payments/list_payment_methods_for_user.py
+-rw-r--r--   0        0        0     2979 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/payments/update_payment_information_for_user.py
+-rw-r--r--   0        0        0     2498 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/payments/validate_customer_tax_information_for_user.py
+-rw-r--r--   0        0        0      101 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/unit/__init__.py
+-rw-r--r--   0        0        0     3697 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/unit/get_angle_unit_conversion.py
+-rw-r--r--   0        0        0     3671 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/unit/get_area_unit_conversion.py
+-rw-r--r--   0        0        0     3747 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/unit/get_current_unit_conversion.py
+-rw-r--r--   0        0        0     3721 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/unit/get_energy_unit_conversion.py
+-rw-r--r--   0        0        0     3695 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/unit/get_force_unit_conversion.py
+-rw-r--r--   0        0        0     3799 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/unit/get_frequency_unit_conversion.py
+-rw-r--r--   0        0        0     3721 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/unit/get_length_unit_conversion.py
+-rw-r--r--   0        0        0     3669 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/unit/get_mass_unit_conversion.py
+-rw-r--r--   0        0        0     3695 2023-08-01 01:14:08.233211 kittycad-0.4.5/kittycad/api/unit/get_power_unit_conversion.py
+-rw-r--r--   0        0        0     3773 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/api/unit/get_pressure_unit_conversion.py
+-rw-r--r--   0        0        0     3851 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/api/unit/get_temperature_unit_conversion.py
+-rw-r--r--   0        0        0     3721 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/api/unit/get_torque_unit_conversion.py
+-rw-r--r--   0        0        0     3721 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/api/unit/get_volume_unit_conversion.py
+-rw-r--r--   0        0        0      297 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/api/users/__init__.py
+-rw-r--r--   0        0        0     2604 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/api/users/delete_user_self.py
+-rw-r--r--   0        0        0     2780 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/api/users/get_session_for_user.py
+-rw-r--r--   0        0        0     3084 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/api/users/get_user.py
+-rw-r--r--   0        0        0     3208 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/api/users/get_user_extended.py
+-rw-r--r--   0        0        0     2495 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/api/users/get_user_front_hash_self.py
+-rw-r--r--   0        0        0     2521 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/api/users/get_user_onboarding_self.py
+-rw-r--r--   0        0        0     2538 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/api/users/get_user_self.py
+-rw-r--r--   0        0        0     2644 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/api/users/get_user_self_extended.py
+-rw-r--r--   0        0        0     4123 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/api/users/list_users.py
+-rw-r--r--   0        0        0     4205 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/api/users/list_users_extended.py
+-rw-r--r--   0        0        0     2794 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/api/users/update_user_self.py
+-rw-r--r--   0        0        0     2297 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/client.py
+-rw-r--r--   0        0        0     5431 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/client_test.py
+-rw-r--r--   0        0        0    99484 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/examples_test.py
+-rw-r--r--   0        0        0     6272 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/__init__.py
+-rw-r--r--   0        0        0      322 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/account_provider.py
+-rw-r--r--   0        0        0     2262 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/ai_plugin_api.py
+-rw-r--r--   0        0        0      242 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/ai_plugin_api_type.py
+-rw-r--r--   0        0        0     2456 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/ai_plugin_auth.py
+-rw-r--r--   0        0        0      413 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/ai_plugin_auth_type.py
+-rw-r--r--   0        0        0      287 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/ai_plugin_http_auth_type.py
+-rw-r--r--   0        0        0     4719 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/ai_plugin_manifest.py
+-rw-r--r--   0        0        0     1724 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/api_call_query_group.py
+-rw-r--r--   0        0        0      777 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/api_call_query_group_by.py
+-rw-r--r--   0        0        0      620 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/api_call_status.py
+-rw-r--r--   0        0        0     8636 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/api_call_with_price.py
+-rw-r--r--   0        0        0     2132 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/api_call_with_price_results_page.py
+-rw-r--r--   0        0        0     3479 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/api_token.py
+-rw-r--r--   0        0        0     2008 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/api_token_results_page.py
+-rw-r--r--   0        0        0     1451 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/app_client_info.py
+-rw-r--r--   0        0        0     5952 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/async_api_call.py
+-rw-r--r--   0        0        0    42312 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/async_api_call_output.py
+-rw-r--r--   0        0        0     2070 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/async_api_call_results_page.py
+-rw-r--r--   0        0        0      648 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/async_api_call_type.py
+-rw-r--r--   0        0        0      426 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/axis.py
+-rw-r--r--   0        0        0     2251 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/axis_direction_pair.py
+-rw-r--r--   0        0        0     2145 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/billing_info.py
+-rw-r--r--   0        0        0     1483 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/cache_metadata.py
+-rw-r--r--   0        0        0      440 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/camera_drag_interaction_type.py
+-rw-r--r--   0        0        0     3358 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/card_details.py
+-rw-r--r--   0        0        0     2701 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/cluster.py
+-rw-r--r--   0        0        0      409 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/code_language.py
+-rw-r--r--   0        0        0     2248 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/code_output.py
+-rw-r--r--   0        0        0     1736 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/commit.py
+-rw-r--r--   0        0        0    14412 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/connection.py
+-rw-r--r--   0        0        0    13513 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/country_code.py
+-rw-r--r--   0        0        0     2124 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/coupon.py
+-rw-r--r--   0        0        0      507 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/created_at_sort_mode.py
+-rw-r--r--   0        0        0     8628 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/currency.py
+-rw-r--r--   0        0        0     4332 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/customer.py
+-rw-r--r--   0        0        0     4492 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/customer_balance.py
+-rw-r--r--   0        0        0     2425 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/device_access_token_request_form.py
+-rw-r--r--   0        0        0     1584 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/device_auth_request_form.py
+-rw-r--r--   0        0        0     1610 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/device_auth_verify_params.py
+-rw-r--r--   0        0        0      327 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/direction.py
+-rw-r--r--   0        0        0     1706 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/discount.py
+-rw-r--r--   0        0        0    21334 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/docker_system_info.py
+-rw-r--r--   0        0        0     1793 2023-08-01 01:14:08.237211 kittycad-0.4.5/kittycad/models/email_authentication_form.py
+-rw-r--r--   0        0        0     3895 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/engine_metadata.py
+-rw-r--r--   0        0        0      529 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/environment.py
+-rw-r--r--   0        0        0     1934 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/error.py
+-rw-r--r--   0        0        0     2740 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/executor_metadata.py
+-rw-r--r--   0        0        0     6078 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/extended_user.py
+-rw-r--r--   0        0        0     2064 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/extended_user_results_page.py
+-rw-r--r--   0        0        0     2135 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/extrude.py
+-rw-r--r--   0        0        0     6935 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/file_center_of_mass.py
+-rw-r--r--   0        0        0     7911 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/file_conversion.py
+-rw-r--r--   0        0        0     7412 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/file_density.py
+-rw-r--r--   0        0        0     1292 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/file_export_format.py
+-rw-r--r--   0        0        0     1032 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/file_import_format.py
+-rw-r--r--   0        0        0     7412 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/file_mass.py
+-rw-r--r--   0        0        0     6565 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/file_surface_area.py
+-rw-r--r--   0        0        0     1517 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/file_system_metadata.py
+-rw-r--r--   0        0        0     6420 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/file_volume.py
+-rw-r--r--   0        0        0     2308 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/gateway.py
+-rw-r--r--   0        0        0      187 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/image_type.py
+-rw-r--r--   0        0        0     2232 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/index_info.py
+-rw-r--r--   0        0        0     9802 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/input_format.py
+-rw-r--r--   0        0        0     8826 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/invoice.py
+-rw-r--r--   0        0        0     2908 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/invoice_line_item.py
+-rw-r--r--   0        0        0      563 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/invoice_status.py
+-rw-r--r--   0        0        0     2698 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/jetstream.py
+-rw-r--r--   0        0        0     1911 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/jetstream_api_stats.py
+-rw-r--r--   0        0        0     2216 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/jetstream_config.py
+-rw-r--r--   0        0        0     3185 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/jetstream_stats.py
+-rw-r--r--   0        0        0     2129 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/leaf_node.py
+-rw-r--r--   0        0        0     1341 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/mesh.py
+-rw-r--r--   0        0        0     1927 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/meta_cluster_info.py
+-rw-r--r--   0        0        0     5101 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/metadata.py
+-rw-r--r--   0        0        0     1793 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/method.py
+-rw-r--r--   0        0        0    19724 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/modeling_cmd.py
+-rw-r--r--   0        0        0       76 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/modeling_cmd_id.py
+-rw-r--r--   0        0        0     2471 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/modeling_cmd_req.py
+-rw-r--r--   0        0        0     1756 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/modeling_cmd_req_batch.py
+-rw-r--r--   0        0        0     2403 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/modeling_error.py
+-rw-r--r--   0        0        0     1893 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/modeling_outcome.py
+-rw-r--r--   0        0        0     1515 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/modeling_outcomes.py
+-rw-r--r--   0        0        0     3098 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/new_address.py
+-rw-r--r--   0        0        0     2042 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/o_auth2_client_info.py
+-rw-r--r--   0        0        0      415 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/o_auth2_grant_type.py
+-rw-r--r--   0        0        0     2513 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/onboarding.py
+-rw-r--r--   0        0        0     1650 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/output_file.py
+-rw-r--r--   0        0        0     9967 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/output_format.py
+-rw-r--r--   0        0        0     6241 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/path_segment.py
+-rw-r--r--   0        0        0     1531 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/payment_intent.py
+-rw-r--r--   0        0        0     3790 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/payment_method.py
+-rw-r--r--   0        0        0     2271 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/payment_method_card_checks.py
+-rw-r--r--   0        0        0      294 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/payment_method_type.py
+-rw-r--r--   0        0        0     5626 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/physics_constant.py
+-rw-r--r--   0        0        0     4448 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/physics_constant_name.py
+-rw-r--r--   0        0        0     2818 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/plugins_info.py
+-rw-r--r--   0        0        0     1534 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/point2d.py
+-rw-r--r--   0        0        0     1695 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/point3d.py
+-rw-r--r--   0        0        0     1502 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/point_e_metadata.py
+-rw-r--r--   0        0        0     1436 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/pong.py
+-rw-r--r--   0        0        0     4191 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/registry_service_config.py
+-rw-r--r--   0        0        0     2038 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/runtime.py
+-rw-r--r--   0        0        0     3879 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/session.py
+-rw-r--r--   0        0        0      656 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/storage.py
+-rw-r--r--   0        0        0     2372 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/system.py
+-rw-r--r--   0        0        0      214 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/system_info_cgroup_driver_enum.py
+-rw-r--r--   0        0        0      175 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/system_info_cgroup_version_enum.py
+-rw-r--r--   0        0        0     1667 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/system_info_default_address_pools.py
+-rw-r--r--   0        0        0      213 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/system_info_isolation_enum.py
+-rw-r--r--   0        0        0      377 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/unit_angle.py
+-rw-r--r--   0        0        0     6389 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/unit_angle_conversion.py
+-rw-r--r--   0        0        0     1013 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/unit_area.py
+-rw-r--r--   0        0        0     6378 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/unit_area_conversion.py
+-rw-r--r--   0        0        0      623 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/unit_current.py
+-rw-r--r--   0        0        0     6411 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/unit_current_conversion.py
+-rw-r--r--   0        0        0      322 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/unit_density.py
+-rw-r--r--   0        0        0      934 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/unit_energy.py
+-rw-r--r--   0        0        0     6400 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/unit_energy_conversion.py
+-rw-r--r--   0        0        0      916 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/unit_force.py
+-rw-r--r--   0        0        0     6389 2023-08-01 01:14:08.241211 kittycad-0.4.5/kittycad/models/unit_force_conversion.py
+-rw-r--r--   0        0        0      997 2023-08-01 01:14:08.245211 kittycad-0.4.5/kittycad/models/unit_frequency.py
+-rw-r--r--   0        0        0     6433 2023-08-01 01:14:08.245211 kittycad-0.4.5/kittycad/models/unit_frequency_conversion.py
+-rw-r--r--   0        0        0      708 2023-08-01 01:14:08.245211 kittycad-0.4.5/kittycad/models/unit_length.py
+-rw-r--r--   0        0        0     6400 2023-08-01 01:14:08.245211 kittycad-0.4.5/kittycad/models/unit_length_conversion.py
+-rw-r--r--   0        0        0      436 2023-08-01 01:14:08.245211 kittycad-0.4.5/kittycad/models/unit_mass.py
+-rw-r--r--   0        0        0     6378 2023-08-01 01:14:08.245211 kittycad-0.4.5/kittycad/models/unit_mass_conversion.py
+-rw-r--r--   0        0        0     1014 2023-08-01 01:14:08.245211 kittycad-0.4.5/kittycad/models/unit_power.py
+-rw-r--r--   0        0        0     6389 2023-08-01 01:14:08.245211 kittycad-0.4.5/kittycad/models/unit_power_conversion.py
+-rw-r--r--   0        0        0      973 2023-08-01 01:14:08.245211 kittycad-0.4.5/kittycad/models/unit_pressure.py
+-rw-r--r--   0        0        0     6422 2023-08-01 01:14:08.245211 kittycad-0.4.5/kittycad/models/unit_pressure_conversion.py
+-rw-r--r--   0        0        0      593 2023-08-01 01:14:08.245211 kittycad-0.4.5/kittycad/models/unit_temperature.py
+-rw-r--r--   0        0        0     6455 2023-08-01 01:14:08.245211 kittycad-0.4.5/kittycad/models/unit_temperature_conversion.py
+-rw-r--r--   0        0        0      415 2023-08-01 01:14:08.245211 kittycad-0.4.5/kittycad/models/unit_torque.py
+-rw-r--r--   0        0        0     6400 2023-08-01 01:14:08.245211 kittycad-0.4.5/kittycad/models/unit_torque_conversion.py
+-rw-r--r--   0        0        0     1131 2023-08-01 01:14:08.245211 kittycad-0.4.5/kittycad/models/unit_volume.py
+-rw-r--r--   0        0        0     6400 2023-08-01 01:14:08.245211 kittycad-0.4.5/kittycad/models/unit_volume_conversion.py
+-rw-r--r--   0        0        0     2581 2023-08-01 01:14:08.245211 kittycad-0.4.5/kittycad/models/update_user.py
+-rw-r--r--   0        0        0     5088 2023-08-01 01:14:08.245211 kittycad-0.4.5/kittycad/models/user.py
+-rw-r--r--   0        0        0     1946 2023-08-01 01:14:08.245211 kittycad-0.4.5/kittycad/models/user_results_page.py
+-rw-r--r--   0        0        0       67 2023-08-01 01:14:08.245211 kittycad-0.4.5/kittycad/models/uuid.py
+-rw-r--r--   0        0        0     3452 2023-08-01 01:14:08.245211 kittycad-0.4.5/kittycad/models/verification_token.py
+-rw-r--r--   0        0        0       26 2023-08-01 01:14:08.245211 kittycad-0.4.5/kittycad/py.typed
+-rw-r--r--   0        0        0     1049 2023-08-01 01:14:08.245211 kittycad-0.4.5/kittycad/types.py
+-rw-r--r--   0        0        0     2513 2023-08-01 01:14:08.245211 kittycad-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     1469 1970-01-01 00:00:00.000000 kittycad-0.4.5/PKG-INFO
```

### Comparing `kittycad-0.4.4/LICENSE` & `kittycad-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.4/README.md` & `kittycad-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.4/kittycad/api/ai/create_image_to_3d.py` & `kittycad-0.4.5/kittycad/api/ai/create_image_to_3d.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,17 @@
     input_format: ImageType,
     output_format: FileExportFormat,
     body: bytes,
     *,
     client: Client,
 ) -> Dict[str, Any]:
     url = "{}/ai/image-to-3d/{input_format}/{output_format}".format(
-        client.base_url, input_format=input_format, output_format=output_format
+        client.base_url,
+        input_format=input_format,
+        output_format=output_format,
     )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
```

### Comparing `kittycad-0.4.4/kittycad/api/ai/create_text_to_3d.py` & `kittycad-0.4.5/kittycad/api/ai/create_text_to_3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,18 @@
 def _get_kwargs(
     output_format: FileExportFormat,
     prompt: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
     url = "{}/ai/text-to-3d/{output_format}".format(
-        client.base_url, output_format=output_format
+        client.base_url,
+        output_format=output_format,
     )  # noqa: E501
+
     if prompt is not None:
         if "?" in url:
             url = url + "&prompt=" + str(prompt)
         else:
             url = url + "?prompt=" + str(prompt)
 
     headers: Dict[str, Any] = client.get_headers()
```

### Comparing `kittycad-0.4.4/kittycad/api/api_calls/get_api_call.py` & `kittycad-0.4.5/kittycad/api/api_calls/get_api_call.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,18 @@
 
 
 def _get_kwargs(
     id: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/api-calls/{id}".format(client.base_url, id=id)  # noqa: E501
+    url = "{}/api-calls/{id}".format(
+        client.base_url,
+        id=id,
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
```

### Comparing `kittycad-0.4.4/kittycad/api/api_calls/get_api_call_for_user.py` & `kittycad-0.4.5/kittycad/api/api_calls/get_api_call_for_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,18 @@
 
 
 def _get_kwargs(
     id: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/user/api-calls/{id}".format(client.base_url, id=id)  # noqa: E501
+    url = "{}/user/api-calls/{id}".format(
+        client.base_url,
+        id=id,
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
```

### Comparing `kittycad-0.4.4/kittycad/api/api_calls/get_api_call_metrics.py` & `kittycad-0.4.5/kittycad/api/api_calls/get_api_call_metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,18 @@
 
 
 def _get_kwargs(
     group_by: ApiCallQueryGroupBy,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/api-call-metrics".format(client.base_url)  # noqa: E501
+    url = "{}/api-call-metrics".format(
+        client.base_url,
+    )  # noqa: E501
+
     if group_by is not None:
         if "?" in url:
             url = url + "&group_by=" + str(group_by)
         else:
             url = url + "?group_by=" + str(group_by)
 
     headers: Dict[str, Any] = client.get_headers()
```

### Comparing `kittycad-0.4.4/kittycad/api/api_calls/get_async_operation.py` & `kittycad-0.4.5/kittycad/api/api_calls/get_async_operation.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,18 @@
 
 
 def _get_kwargs(
     id: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/async/operations/{id}".format(client.base_url, id=id)  # noqa: E501
+    url = "{}/async/operations/{id}".format(
+        client.base_url,
+        id=id,
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
@@ -176,15 +179,16 @@
         FileSurfaceArea,
         Error,
     ]
 ]:
     """Get the status and output of an async operation.
     This endpoint requires authentication by any KittyCAD user. It returns details of the requested async operation for the user.
     If the user is not authenticated to view the specified async operation, then it is not returned.
-    Only KittyCAD employees with the proper access can view async operations for other users."""  # noqa: E501
+    Only KittyCAD employees with the proper access can view async operations for other users.
+    """  # noqa: E501
 
     return sync_detailed(
         id=id,
         client=client,
     ).parsed
 
 
@@ -230,15 +234,16 @@
         FileSurfaceArea,
         Error,
     ]
 ]:
     """Get the status and output of an async operation.
     This endpoint requires authentication by any KittyCAD user. It returns details of the requested async operation for the user.
     If the user is not authenticated to view the specified async operation, then it is not returned.
-    Only KittyCAD employees with the proper access can view async operations for other users."""  # noqa: E501
+    Only KittyCAD employees with the proper access can view async operations for other users.
+    """  # noqa: E501
 
     return (
         await asyncio_detailed(
             id=id,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.4/kittycad/api/api_calls/list_api_calls.py` & `kittycad-0.4.5/kittycad/api/api_calls/list_api_calls.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,25 +12,30 @@
 def _get_kwargs(
     sort_by: CreatedAtSortMode,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
 ) -> Dict[str, Any]:
-    url = "{}/api-calls".format(client.base_url)  # noqa: E501
+    url = "{}/api-calls".format(
+        client.base_url,
+    )  # noqa: E501
+
     if limit is not None:
         if "?" in url:
             url = url + "&limit=" + str(limit)
         else:
             url = url + "?limit=" + str(limit)
+
     if page_token is not None:
         if "?" in url:
             url = url + "&page_token=" + str(page_token)
         else:
             url = url + "?page_token=" + str(page_token)
+
     if sort_by is not None:
         if "?" in url:
             url = url + "&sort_by=" + str(sort_by)
         else:
             url = url + "?sort_by=" + str(sort_by)
 
     headers: Dict[str, Any] = client.get_headers()
```

### Comparing `kittycad-0.4.4/kittycad/api/api_calls/list_api_calls_for_user.py` & `kittycad-0.4.5/kittycad/api/api_calls/list_api_calls_for_user.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,25 +13,31 @@
     id: str,
     sort_by: CreatedAtSortMode,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
 ) -> Dict[str, Any]:
-    url = "{}/users/{id}/api-calls".format(client.base_url, id=id)  # noqa: E501
+    url = "{}/users/{id}/api-calls".format(
+        client.base_url,
+        id=id,
+    )  # noqa: E501
+
     if limit is not None:
         if "?" in url:
             url = url + "&limit=" + str(limit)
         else:
             url = url + "?limit=" + str(limit)
+
     if page_token is not None:
         if "?" in url:
             url = url + "&page_token=" + str(page_token)
         else:
             url = url + "?page_token=" + str(page_token)
+
     if sort_by is not None:
         if "?" in url:
             url = url + "&sort_by=" + str(sort_by)
         else:
             url = url + "?sort_by=" + str(sort_by)
 
     headers: Dict[str, Any] = client.get_headers()
@@ -102,15 +108,16 @@
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
 ) -> Optional[Union[ApiCallWithPriceResultsPage, Error]]:
     """This endpoint requires authentication by any KittyCAD user. It returns the API calls for the authenticated user if "me" is passed as the user id.
     Alternatively, you can use the `/user/api-calls` endpoint to get the API calls for your user.
     If the authenticated user is a KittyCAD employee, then the API calls are returned for the user specified by the user id.
-    The API calls are returned in order of creation, with the most recently created API calls first."""  # noqa: E501
+    The API calls are returned in order of creation, with the most recently created API calls first.
+    """  # noqa: E501
 
     return sync_detailed(
         id=id,
         limit=limit,
         page_token=page_token,
         sort_by=sort_by,
         client=client,
@@ -146,15 +153,16 @@
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
 ) -> Optional[Union[ApiCallWithPriceResultsPage, Error]]:
     """This endpoint requires authentication by any KittyCAD user. It returns the API calls for the authenticated user if "me" is passed as the user id.
     Alternatively, you can use the `/user/api-calls` endpoint to get the API calls for your user.
     If the authenticated user is a KittyCAD employee, then the API calls are returned for the user specified by the user id.
-    The API calls are returned in order of creation, with the most recently created API calls first."""  # noqa: E501
+    The API calls are returned in order of creation, with the most recently created API calls first.
+    """  # noqa: E501
 
     return (
         await asyncio_detailed(
             id=id,
             limit=limit,
             page_token=page_token,
             sort_by=sort_by,
```

### Comparing `kittycad-0.4.4/kittycad/api/api_calls/list_async_operations.py` & `kittycad-0.4.5/kittycad/api/api_calls/list_async_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,30 +14,36 @@
     sort_by: CreatedAtSortMode,
     status: ApiCallStatus,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
 ) -> Dict[str, Any]:
-    url = "{}/async/operations".format(client.base_url)  # noqa: E501
+    url = "{}/async/operations".format(
+        client.base_url,
+    )  # noqa: E501
+
     if limit is not None:
         if "?" in url:
             url = url + "&limit=" + str(limit)
         else:
             url = url + "?limit=" + str(limit)
+
     if page_token is not None:
         if "?" in url:
             url = url + "&page_token=" + str(page_token)
         else:
             url = url + "?page_token=" + str(page_token)
+
     if sort_by is not None:
         if "?" in url:
             url = url + "&sort_by=" + str(sort_by)
         else:
             url = url + "?sort_by=" + str(sort_by)
+
     if status is not None:
         if "?" in url:
             url = url + "&status=" + str(status)
         else:
             url = url + "?status=" + str(status)
 
     headers: Dict[str, Any] = client.get_headers()
```

### Comparing `kittycad-0.4.4/kittycad/api/api_calls/user_list_api_calls.py` & `kittycad-0.4.5/kittycad/api/api_calls/user_list_api_calls.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,25 +12,30 @@
 def _get_kwargs(
     sort_by: CreatedAtSortMode,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
 ) -> Dict[str, Any]:
-    url = "{}/user/api-calls".format(client.base_url)  # noqa: E501
+    url = "{}/user/api-calls".format(
+        client.base_url,
+    )  # noqa: E501
+
     if limit is not None:
         if "?" in url:
             url = url + "&limit=" + str(limit)
         else:
             url = url + "?limit=" + str(limit)
+
     if page_token is not None:
         if "?" in url:
             url = url + "&page_token=" + str(page_token)
         else:
             url = url + "?page_token=" + str(page_token)
+
     if sort_by is not None:
         if "?" in url:
             url = url + "&sort_by=" + str(sort_by)
         else:
             url = url + "?sort_by=" + str(sort_by)
 
     headers: Dict[str, Any] = client.get_headers()
@@ -96,15 +101,16 @@
     sort_by: CreatedAtSortMode,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
 ) -> Optional[Union[ApiCallWithPriceResultsPage, Error]]:
     """This endpoint requires authentication by any KittyCAD user. It returns the API calls for the authenticated user.
-    The API calls are returned in order of creation, with the most recently created API calls first."""  # noqa: E501
+    The API calls are returned in order of creation, with the most recently created API calls first.
+    """  # noqa: E501
 
     return sync_detailed(
         limit=limit,
         page_token=page_token,
         sort_by=sort_by,
         client=client,
     ).parsed
@@ -134,15 +140,16 @@
     sort_by: CreatedAtSortMode,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
 ) -> Optional[Union[ApiCallWithPriceResultsPage, Error]]:
     """This endpoint requires authentication by any KittyCAD user. It returns the API calls for the authenticated user.
-    The API calls are returned in order of creation, with the most recently created API calls first."""  # noqa: E501
+    The API calls are returned in order of creation, with the most recently created API calls first.
+    """  # noqa: E501
 
     return (
         await asyncio_detailed(
             limit=limit,
             page_token=page_token,
             sort_by=sort_by,
             client=client,
```

### Comparing `kittycad-0.4.4/kittycad/api/api_tokens/create_api_token_for_user.py` & `kittycad-0.4.5/kittycad/api/api_tokens/create_api_token_for_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/user/api-tokens".format(client.base_url)  # noqa: E501
+    url = "{}/user/api-tokens".format(
+        client.base_url,
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
```

### Comparing `kittycad-0.4.4/kittycad/api/api_tokens/delete_api_token_for_user.py` & `kittycad-0.4.5/kittycad/api/api_tokens/delete_api_token_for_user.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 
 def _get_kwargs(
     token: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
     url = "{}/user/api-tokens/{token}".format(
-        client.base_url, token=token
+        client.base_url,
+        token=token,
     )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
@@ -67,15 +68,16 @@
 
 def sync(
     token: str,
     *,
     client: Client,
 ) -> Optional[Error]:
     """This endpoint requires authentication by any KittyCAD user. It deletes the requested API token for the user.
-    This endpoint does not actually delete the API token from the database. It merely marks the token as invalid. We still want to keep the token in the database for historical purposes."""  # noqa: E501
+    This endpoint does not actually delete the API token from the database. It merely marks the token as invalid. We still want to keep the token in the database for historical purposes.
+    """  # noqa: E501
 
     return sync_detailed(
         token=token,
         client=client,
     ).parsed
 
 
@@ -97,15 +99,16 @@
 
 async def asyncio(
     token: str,
     *,
     client: Client,
 ) -> Optional[Error]:
     """This endpoint requires authentication by any KittyCAD user. It deletes the requested API token for the user.
-    This endpoint does not actually delete the API token from the database. It merely marks the token as invalid. We still want to keep the token in the database for historical purposes."""  # noqa: E501
+    This endpoint does not actually delete the API token from the database. It merely marks the token as invalid. We still want to keep the token in the database for historical purposes.
+    """  # noqa: E501
 
     return (
         await asyncio_detailed(
             token=token,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.4/kittycad/api/api_tokens/get_api_token_for_user.py` & `kittycad-0.4.5/kittycad/api/api_tokens/get_api_token_for_user.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 
 def _get_kwargs(
     token: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
     url = "{}/user/api-tokens/{token}".format(
-        client.base_url, token=token
+        client.base_url,
+        token=token,
     )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
```

### Comparing `kittycad-0.4.4/kittycad/api/api_tokens/list_api_tokens_for_user.py` & `kittycad-0.4.5/kittycad/api/api_tokens/list_api_tokens_for_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,25 +12,30 @@
 def _get_kwargs(
     sort_by: CreatedAtSortMode,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
 ) -> Dict[str, Any]:
-    url = "{}/user/api-tokens".format(client.base_url)  # noqa: E501
+    url = "{}/user/api-tokens".format(
+        client.base_url,
+    )  # noqa: E501
+
     if limit is not None:
         if "?" in url:
             url = url + "&limit=" + str(limit)
         else:
             url = url + "?limit=" + str(limit)
+
     if page_token is not None:
         if "?" in url:
             url = url + "&page_token=" + str(page_token)
         else:
             url = url + "?page_token=" + str(page_token)
+
     if sort_by is not None:
         if "?" in url:
             url = url + "&sort_by=" + str(sort_by)
         else:
             url = url + "?sort_by=" + str(sort_by)
 
     headers: Dict[str, Any] = client.get_headers()
@@ -96,15 +101,16 @@
     sort_by: CreatedAtSortMode,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
 ) -> Optional[Union[ApiTokenResultsPage, Error]]:
     """This endpoint requires authentication by any KittyCAD user. It returns the API tokens for the authenticated user.
-    The API tokens are returned in order of creation, with the most recently created API tokens first."""  # noqa: E501
+    The API tokens are returned in order of creation, with the most recently created API tokens first.
+    """  # noqa: E501
 
     return sync_detailed(
         limit=limit,
         page_token=page_token,
         sort_by=sort_by,
         client=client,
     ).parsed
@@ -134,15 +140,16 @@
     sort_by: CreatedAtSortMode,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
 ) -> Optional[Union[ApiTokenResultsPage, Error]]:
     """This endpoint requires authentication by any KittyCAD user. It returns the API tokens for the authenticated user.
-    The API tokens are returned in order of creation, with the most recently created API tokens first."""  # noqa: E501
+    The API tokens are returned in order of creation, with the most recently created API tokens first.
+    """  # noqa: E501
 
     return (
         await asyncio_detailed(
             limit=limit,
             page_token=page_token,
             sort_by=sort_by,
             client=client,
```

### Comparing `kittycad-0.4.4/kittycad/api/apps/apps_github_callback.py` & `kittycad-0.4.5/kittycad/api/apps/apps_github_callback.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/apps/github/callback".format(client.base_url)  # noqa: E501
+    url = "{}/apps/github/callback".format(
+        client.base_url,
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
@@ -61,15 +63,16 @@
 
 
 def sync(
     *,
     client: Client,
 ) -> Optional[Error]:
     """This is different than OAuth 2.0 authentication for users. This endpoint grants access for KittyCAD to access user's repos.
-    The user doesn't need KittyCAD OAuth authorization for this endpoint, this is purely for the GitHub permissions to access repos."""  # noqa: E501
+    The user doesn't need KittyCAD OAuth authorization for this endpoint, this is purely for the GitHub permissions to access repos.
+    """  # noqa: E501
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
@@ -87,14 +90,15 @@
 
 
 async def asyncio(
     *,
     client: Client,
 ) -> Optional[Error]:
     """This is different than OAuth 2.0 authentication for users. This endpoint grants access for KittyCAD to access user's repos.
-    The user doesn't need KittyCAD OAuth authorization for this endpoint, this is purely for the GitHub permissions to access repos."""  # noqa: E501
+    The user doesn't need KittyCAD OAuth authorization for this endpoint, this is purely for the GitHub permissions to access repos.
+    """  # noqa: E501
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.4/kittycad/api/apps/apps_github_consent.py` & `kittycad-0.4.5/kittycad/api/users/get_user_front_hash_self.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,64 +1,63 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.app_client_info import AppClientInfo
 from ...models.error import Error
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/apps/github/consent".format(client.base_url)  # noqa: E501
+    url = "{}/user/front-hash".format(
+        client.base_url,
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[AppClientInfo, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[str, Error]]:
     if response.status_code == 200:
-        response_200 = AppClientInfo.from_dict(response.json())
+        response_200 = response.text
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
     return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Optional[Union[AppClientInfo, Error]]]:
+) -> Response[Optional[Union[str, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[Optional[Union[AppClientInfo, Error]]]:
+) -> Response[Optional[Union[str, Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
@@ -66,42 +65,40 @@
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: Client,
-) -> Optional[Union[AppClientInfo, Error]]:
-    """This is different than OAuth 2.0 authentication for users. This endpoint grants access for KittyCAD to access user's repos.
-    The user doesn't need KittyCAD OAuth authorization for this endpoint, this is purely for the GitHub permissions to access repos."""  # noqa: E501
+) -> Optional[Union[str, Error]]:
+    """This info is sent to front when initialing the front chat, it prevents impersonations using js hacks in the browser"""  # noqa: E501
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[Optional[Union[AppClientInfo, Error]]]:
+) -> Response[Optional[Union[str, Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-) -> Optional[Union[AppClientInfo, Error]]:
-    """This is different than OAuth 2.0 authentication for users. This endpoint grants access for KittyCAD to access user's repos.
-    The user doesn't need KittyCAD OAuth authorization for this endpoint, this is purely for the GitHub permissions to access repos."""  # noqa: E501
+) -> Optional[Union[str, Error]]:
+    """This info is sent to front when initialing the front chat, it prevents impersonations using js hacks in the browser"""  # noqa: E501
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.4/kittycad/api/apps/apps_github_webhook.py` & `kittycad-0.4.5/kittycad/api/apps/apps_github_webhook.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 
 
 def _get_kwargs(
     body: bytes,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/apps/github/webhook".format(client.base_url)  # noqa: E501
+    url = "{}/apps/github/webhook".format(
+        client.base_url,
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
```

### Comparing `kittycad-0.4.4/kittycad/api/constant/get_physics_constant.py` & `kittycad-0.4.5/kittycad/api/constant/get_physics_constant.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 
 def _get_kwargs(
     constant: PhysicsConstantName,
     *,
     client: Client,
 ) -> Dict[str, Any]:
     url = "{}/constant/physics/{constant}".format(
-        client.base_url, constant=constant
+        client.base_url,
+        constant=constant,
     )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
@@ -74,15 +75,14 @@
 
 
 def sync(
     constant: PhysicsConstantName,
     *,
     client: Client,
 ) -> Optional[Union[PhysicsConstant, Error]]:
-
     return sync_detailed(
         constant=constant,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
@@ -102,14 +102,13 @@
 
 
 async def asyncio(
     constant: PhysicsConstantName,
     *,
     client: Client,
 ) -> Optional[Union[PhysicsConstant, Error]]:
-
     return (
         await asyncio_detailed(
             constant=constant,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.4/kittycad/api/executor/create_executor_term.py` & `kittycad-0.4.5/kittycad/api/meta/get_schema.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,63 @@
-from typing import Any, Dict
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
+from ...models.error import Error
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/ws/executor/term".format(client.base_url)  # noqa: E501
+    url = "{}/".format(
+        client.base_url,
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(*, response: httpx.Response):
-    return
-
-
-def _build_response(*, response: httpx.Response) -> Response[Any]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[dict, Error]]:
+    if response.status_code == 200:
+        response_200 = response.json()
+        return response_200
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return Error.from_dict(response.json())
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Optional[Union[dict, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[Any]:
+) -> Response[Optional[Union[dict, Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
@@ -51,40 +65,36 @@
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: Client,
-):
-    """Attach to a docker container to create an interactive terminal."""  # noqa: E501
-
+) -> Optional[Union[dict, Error]]:
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[Any]:
+) -> Response[Optional[Union[dict, Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-):
-    """Attach to a docker container to create an interactive terminal."""  # noqa: E501
-
+) -> Optional[Union[dict, Error]]:
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.4/kittycad/api/executor/create_file_execution.py` & `kittycad-0.4.5/kittycad/api/executor/create_file_execution.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,19 @@
 def _get_kwargs(
     lang: CodeLanguage,
     body: bytes,
     *,
     client: Client,
     output: Optional[str] = None,
 ) -> Dict[str, Any]:
-    url = "{}/file/execute/{lang}".format(client.base_url, lang=lang)  # noqa: E501
+    url = "{}/file/execute/{lang}".format(
+        client.base_url,
+        lang=lang,
+    )  # noqa: E501
+
     if output is not None:
         if "?" in url:
             url = url + "&output=" + str(output)
         else:
             url = url + "?output=" + str(output)
 
     headers: Dict[str, Any] = client.get_headers()
@@ -84,15 +88,14 @@
 def sync(
     lang: CodeLanguage,
     body: bytes,
     *,
     client: Client,
     output: Optional[str] = None,
 ) -> Optional[Union[CodeOutput, Error]]:
-
     return sync_detailed(
         lang=lang,
         output=output,
         body=body,
         client=client,
     ).parsed
 
@@ -120,15 +123,14 @@
 async def asyncio(
     lang: CodeLanguage,
     body: bytes,
     *,
     client: Client,
     output: Optional[str] = None,
 ) -> Optional[Union[CodeOutput, Error]]:
-
     return (
         await asyncio_detailed(
             lang=lang,
             output=output,
             body=body,
             client=client,
         )
```

### Comparing `kittycad-0.4.4/kittycad/api/file/create_file_center_of_mass.py` & `kittycad-0.4.5/kittycad/api/file/create_file_center_of_mass.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,24 +2,35 @@
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
 from ...models.file_center_of_mass import FileCenterOfMass
 from ...models.file_import_format import FileImportFormat
+from ...models.unit_length import UnitLength
 from ...types import Response
 
 
 def _get_kwargs(
+    output_unit: UnitLength,
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/file/center-of-mass".format(client.base_url)  # noqa: E501
+    url = "{}/file/center-of-mass".format(
+        client.base_url,
+    )  # noqa: E501
+
+    if output_unit is not None:
+        if "?" in url:
+            url = url + "&output_unit=" + str(output_unit)
+        else:
+            url = url + "?output_unit=" + str(output_unit)
+
     if src_format is not None:
         if "?" in url:
             url = url + "&src_format=" + str(src_format)
         else:
             url = url + "?src_format=" + str(src_format)
 
     headers: Dict[str, Any] = client.get_headers()
@@ -57,82 +68,92 @@
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
+    output_unit: UnitLength,
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
 ) -> Response[Optional[Union[FileCenterOfMass, Error]]]:
     kwargs = _get_kwargs(
+        output_unit=output_unit,
         src_format=src_format,
         body=body,
         client=client,
     )
 
     response = httpx.post(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
+    output_unit: UnitLength,
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
 ) -> Optional[Union[FileCenterOfMass, Error]]:
     """We assume any file given to us has one consistent unit throughout. We also assume the file is at the proper scale.
     Currently, this endpoint returns the cartesian co-ordinate in world space measure units.
     In the future, we will use the units inside the file if they are given and do any conversions if necessary for the calculation. But currently, that is not supported.
     Get the center of mass of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
-    If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
+    If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint.
+    """  # noqa: E501
 
     return sync_detailed(
+        output_unit=output_unit,
         src_format=src_format,
         body=body,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
+    output_unit: UnitLength,
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
 ) -> Response[Optional[Union[FileCenterOfMass, Error]]]:
     kwargs = _get_kwargs(
+        output_unit=output_unit,
         src_format=src_format,
         body=body,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.post(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
+    output_unit: UnitLength,
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
 ) -> Optional[Union[FileCenterOfMass, Error]]:
     """We assume any file given to us has one consistent unit throughout. We also assume the file is at the proper scale.
     Currently, this endpoint returns the cartesian co-ordinate in world space measure units.
     In the future, we will use the units inside the file if they are given and do any conversions if necessary for the calculation. But currently, that is not supported.
     Get the center of mass of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
-    If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
+    If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint.
+    """  # noqa: E501
 
     return (
         await asyncio_detailed(
+            output_unit=output_unit,
             src_format=src_format,
             body=body,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.4/kittycad/api/file/create_file_conversion.py` & `kittycad-0.4.5/kittycad/api/file/create_file_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,17 @@
     output_format: FileExportFormat,
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
 ) -> Dict[str, Any]:
     url = "{}/file/conversion/{src_format}/{output_format}".format(
-        client.base_url, output_format=output_format, src_format=src_format
+        client.base_url,
+        output_format=output_format,
+        src_format=src_format,
     )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
@@ -87,15 +89,16 @@
     body: bytes,
     *,
     client: Client,
 ) -> Optional[Union[FileConversion, Error]]:
     """If you wish to specify the conversion options, use the `/file/conversion` endpoint instead.
     Convert a CAD file from one format to another. If the file being converted is larger than 25MB, it will be performed asynchronously.
     If the conversion is performed synchronously, the contents of the converted file (`output`) will be returned as a base64 encoded string.
-    If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
+    If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint.
+    """  # noqa: E501
 
     return sync_detailed(
         output_format=output_format,
         src_format=src_format,
         body=body,
         client=client,
     ).parsed
@@ -127,15 +130,16 @@
     body: bytes,
     *,
     client: Client,
 ) -> Optional[Union[FileConversion, Error]]:
     """If you wish to specify the conversion options, use the `/file/conversion` endpoint instead.
     Convert a CAD file from one format to another. If the file being converted is larger than 25MB, it will be performed asynchronously.
     If the conversion is performed synchronously, the contents of the converted file (`output`) will be returned as a base64 encoded string.
-    If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
+    If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint.
+    """  # noqa: E501
 
     return (
         await asyncio_detailed(
             output_format=output_format,
             src_format=src_format,
             body=body,
             client=client,
```

### Comparing `kittycad-0.4.4/kittycad/api/file/create_file_conversion_with_base64_helper.py` & `kittycad-0.4.5/kittycad/api/file/create_file_conversion_with_base64_helper.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.4/kittycad/api/file/create_file_density.py` & `kittycad-0.4.5/kittycad/api/file/create_file_density.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,30 +2,50 @@
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
 from ...models.file_density import FileDensity
 from ...models.file_import_format import FileImportFormat
+from ...models.unit_density import UnitDensity
+from ...models.unit_mass import UnitMass
 from ...types import Response
 
 
 def _get_kwargs(
     material_mass: float,
+    material_mass_unit: UnitMass,
+    output_unit: UnitDensity,
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/file/density".format(client.base_url)  # noqa: E501
+    url = "{}/file/density".format(
+        client.base_url,
+    )  # noqa: E501
+
     if material_mass is not None:
         if "?" in url:
             url = url + "&material_mass=" + str(material_mass)
         else:
             url = url + "?material_mass=" + str(material_mass)
+
+    if material_mass_unit is not None:
+        if "?" in url:
+            url = url + "&material_mass_unit=" + str(material_mass_unit)
+        else:
+            url = url + "?material_mass_unit=" + str(material_mass_unit)
+
+    if output_unit is not None:
+        if "?" in url:
+            url = url + "&output_unit=" + str(output_unit)
+        else:
+            url = url + "?output_unit=" + str(output_unit)
+
     if src_format is not None:
         if "?" in url:
             url = url + "&src_format=" + str(src_format)
         else:
             url = url + "?src_format=" + str(src_format)
 
     headers: Dict[str, Any] = client.get_headers()
@@ -62,21 +82,25 @@
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     material_mass: float,
+    material_mass_unit: UnitMass,
+    output_unit: UnitDensity,
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
 ) -> Response[Optional[Union[FileDensity, Error]]]:
     kwargs = _get_kwargs(
         material_mass=material_mass,
+        material_mass_unit=material_mass_unit,
+        output_unit=output_unit,
         src_format=src_format,
         body=body,
         client=client,
     )
 
     response = httpx.post(
         verify=client.verify_ssl,
@@ -84,67 +108,81 @@
     )
 
     return _build_response(response=response)
 
 
 def sync(
     material_mass: float,
+    material_mass_unit: UnitMass,
+    output_unit: UnitDensity,
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
 ) -> Optional[Union[FileDensity, Error]]:
     """We assume any file given to us has one consistent unit throughout. We also assume the file is at the proper scale.
     Currently, this endpoint assumes if you are giving a material mass in a specific mass units, we return a density in mass unit per cubic measure unit.
     In the future, we will use the units inside the file if they are given and do any conversions if necessary for the calculation. But currently, that is not supported.
     Get the density of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
-    If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
+    If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint.
+    """  # noqa: E501
 
     return sync_detailed(
         material_mass=material_mass,
+        material_mass_unit=material_mass_unit,
+        output_unit=output_unit,
         src_format=src_format,
         body=body,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     material_mass: float,
+    material_mass_unit: UnitMass,
+    output_unit: UnitDensity,
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
 ) -> Response[Optional[Union[FileDensity, Error]]]:
     kwargs = _get_kwargs(
         material_mass=material_mass,
+        material_mass_unit=material_mass_unit,
+        output_unit=output_unit,
         src_format=src_format,
         body=body,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.post(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     material_mass: float,
+    material_mass_unit: UnitMass,
+    output_unit: UnitDensity,
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
 ) -> Optional[Union[FileDensity, Error]]:
     """We assume any file given to us has one consistent unit throughout. We also assume the file is at the proper scale.
     Currently, this endpoint assumes if you are giving a material mass in a specific mass units, we return a density in mass unit per cubic measure unit.
     In the future, we will use the units inside the file if they are given and do any conversions if necessary for the calculation. But currently, that is not supported.
     Get the density of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
-    If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
+    If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint.
+    """  # noqa: E501
 
     return (
         await asyncio_detailed(
             material_mass=material_mass,
+            material_mass_unit=material_mass_unit,
+            output_unit=output_unit,
             src_format=src_format,
             body=body,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.4/kittycad/api/file/create_file_surface_area.py` & `kittycad-0.4.5/kittycad/api/file/create_file_surface_area.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,24 +2,35 @@
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
 from ...models.file_import_format import FileImportFormat
 from ...models.file_surface_area import FileSurfaceArea
+from ...models.unit_area import UnitArea
 from ...types import Response
 
 
 def _get_kwargs(
+    output_unit: UnitArea,
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/file/surface-area".format(client.base_url)  # noqa: E501
+    url = "{}/file/surface-area".format(
+        client.base_url,
+    )  # noqa: E501
+
+    if output_unit is not None:
+        if "?" in url:
+            url = url + "&output_unit=" + str(output_unit)
+        else:
+            url = url + "?output_unit=" + str(output_unit)
+
     if src_format is not None:
         if "?" in url:
             url = url + "&src_format=" + str(src_format)
         else:
             url = url + "?src_format=" + str(src_format)
 
     headers: Dict[str, Any] = client.get_headers()
@@ -57,82 +68,92 @@
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
+    output_unit: UnitArea,
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
 ) -> Response[Optional[Union[FileSurfaceArea, Error]]]:
     kwargs = _get_kwargs(
+        output_unit=output_unit,
         src_format=src_format,
         body=body,
         client=client,
     )
 
     response = httpx.post(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
+    output_unit: UnitArea,
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
 ) -> Optional[Union[FileSurfaceArea, Error]]:
     """We assume any file given to us has one consistent unit throughout. We also assume the file is at the proper scale.
     Currently, this endpoint returns the square measure units.
     In the future, we will use the units inside the file if they are given and do any conversions if necessary for the calculation. But currently, that is not supported.
     Get the surface area of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
-    If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
+    If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint.
+    """  # noqa: E501
 
     return sync_detailed(
+        output_unit=output_unit,
         src_format=src_format,
         body=body,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
+    output_unit: UnitArea,
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
 ) -> Response[Optional[Union[FileSurfaceArea, Error]]]:
     kwargs = _get_kwargs(
+        output_unit=output_unit,
         src_format=src_format,
         body=body,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.post(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
+    output_unit: UnitArea,
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
 ) -> Optional[Union[FileSurfaceArea, Error]]:
     """We assume any file given to us has one consistent unit throughout. We also assume the file is at the proper scale.
     Currently, this endpoint returns the square measure units.
     In the future, we will use the units inside the file if they are given and do any conversions if necessary for the calculation. But currently, that is not supported.
     Get the surface area of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
-    If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
+    If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint.
+    """  # noqa: E501
 
     return (
         await asyncio_detailed(
+            output_unit=output_unit,
             src_format=src_format,
             body=body,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.4/kittycad/api/file/get_file_conversion_with_base64_helper.py` & `kittycad-0.4.5/kittycad/api/file/get_file_conversion_with_base64_helper.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.4/kittycad/api/hidden/auth_email.py` & `kittycad-0.4.5/kittycad/api/users/get_user_self.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,114 +1,107 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.email_authentication_form import EmailAuthenticationForm
 from ...models.error import Error
-from ...models.verification_token import VerificationToken
+from ...models.user import User
 from ...types import Response
 
 
 def _get_kwargs(
-    body: EmailAuthenticationForm,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/auth/email".format(client.base_url)  # noqa: E501
+    url = "{}/user".format(
+        client.base_url,
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "content": body,
     }
 
 
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[VerificationToken, Error]]:
-    if response.status_code == 201:
-        response_201 = VerificationToken.from_dict(response.json())
-        return response_201
+def _parse_response(*, response: httpx.Response) -> Optional[Union[User, Error]]:
+    if response.status_code == 200:
+        response_200 = User.from_dict(response.json())
+        return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
     return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Optional[Union[VerificationToken, Error]]]:
+) -> Response[Optional[Union[User, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    body: EmailAuthenticationForm,
     *,
     client: Client,
-) -> Response[Optional[Union[VerificationToken, Error]]]:
+) -> Response[Optional[Union[User, Error]]]:
     kwargs = _get_kwargs(
-        body=body,
         client=client,
     )
 
-    response = httpx.post(
+    response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    body: EmailAuthenticationForm,
     *,
     client: Client,
-) -> Optional[Union[VerificationToken, Error]]:
+) -> Optional[Union[User, Error]]:
+    """Get the user information for the authenticated user.
+    Alternatively, you can also use the `/users/me` endpoint."""  # noqa: E501
 
     return sync_detailed(
-        body=body,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    body: EmailAuthenticationForm,
     *,
     client: Client,
-) -> Response[Optional[Union[VerificationToken, Error]]]:
+) -> Response[Optional[Union[User, Error]]]:
     kwargs = _get_kwargs(
-        body=body,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.post(**kwargs)
+        response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    body: EmailAuthenticationForm,
     *,
     client: Client,
-) -> Optional[Union[VerificationToken, Error]]:
+) -> Optional[Union[User, Error]]:
+    """Get the user information for the authenticated user.
+    Alternatively, you can also use the `/users/me` endpoint."""  # noqa: E501
 
     return (
         await asyncio_detailed(
-            body=body,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.4/kittycad/api/hidden/auth_email_callback.py` & `kittycad-0.4.5/kittycad/api/hidden/auth_email_callback.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,25 +10,30 @@
 def _get_kwargs(
     email: str,
     token: str,
     *,
     client: Client,
     callback_url: Optional[str] = None,
 ) -> Dict[str, Any]:
-    url = "{}/auth/email/callback".format(client.base_url)  # noqa: E501
+    url = "{}/auth/email/callback".format(
+        client.base_url,
+    )  # noqa: E501
+
     if callback_url is not None:
         if "?" in url:
             url = url + "&callback_url=" + str(callback_url)
         else:
             url = url + "?callback_url=" + str(callback_url)
+
     if email is not None:
         if "?" in url:
             url = url + "&email=" + str(email)
         else:
             url = url + "?email=" + str(email)
+
     if token is not None:
         if "?" in url:
             url = url + "&token=" + str(token)
         else:
             url = url + "?token=" + str(token)
 
     headers: Dict[str, Any] = client.get_headers()
@@ -87,15 +92,14 @@
 def sync(
     email: str,
     token: str,
     *,
     client: Client,
     callback_url: Optional[str] = None,
 ) -> Optional[Error]:
-
     return sync_detailed(
         callback_url=callback_url,
         email=email,
         token=token,
         client=client,
     ).parsed
 
@@ -123,15 +127,14 @@
 async def asyncio(
     email: str,
     token: str,
     *,
     client: Client,
     callback_url: Optional[str] = None,
 ) -> Optional[Error]:
-
     return (
         await asyncio_detailed(
             callback_url=callback_url,
             email=email,
             token=token,
             client=client,
         )
```

### Comparing `kittycad-0.4.4/kittycad/api/hidden/logout.py` & `kittycad-0.4.5/kittycad/api/hidden/logout.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/logout".format(client.base_url)  # noqa: E501
+    url = "{}/logout".format(
+        client.base_url,
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
```

### Comparing `kittycad-0.4.4/kittycad/api/meta/get_ai_plugin_manifest.py` & `kittycad-0.4.5/kittycad/api/meta/get_ai_plugin_manifest.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/.well-known/ai-plugin.json".format(client.base_url)  # noqa: E501
+    url = "{}/.well-known/ai-plugin.json".format(
+        client.base_url,
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
@@ -67,15 +69,14 @@
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: Client,
 ) -> Optional[Union[AiPluginManifest, Error]]:
-
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
@@ -91,13 +92,12 @@
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: Client,
 ) -> Optional[Union[AiPluginManifest, Error]]:
-
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.4/kittycad/api/meta/get_metadata.py` & `kittycad-0.4.5/kittycad/api/meta/get_metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/_meta/info".format(client.base_url)  # noqa: E501
+    url = "{}/_meta/info".format(
+        client.base_url,
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
```

### Comparing `kittycad-0.4.4/kittycad/api/meta/get_openai_schema.py` & `kittycad-0.4.5/kittycad/api/meta/get_openai_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/openai/openapi.json".format(client.base_url)  # noqa: E501
+    url = "{}/openai/openapi.json".format(
+        client.base_url,
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
```

### Comparing `kittycad-0.4.4/kittycad/api/meta/get_schema.py` & `kittycad-0.4.5/kittycad/api/payments/get_payment_balance_for_user.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,61 +1,66 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
+from ...models.customer_balance import CustomerBalance
 from ...models.error import Error
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/".format(client.base_url)  # noqa: E501
+    url = "{}/user/payment/balance".format(
+        client.base_url,
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[dict, Error]]:
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[CustomerBalance, Error]]:
     if response.status_code == 200:
-        response_200 = response.json()
+        response_200 = CustomerBalance.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
     return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Optional[Union[dict, Error]]]:
+) -> Response[Optional[Union[CustomerBalance, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[Optional[Union[dict, Error]]]:
+) -> Response[Optional[Union[CustomerBalance, Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
@@ -63,38 +68,40 @@
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: Client,
-) -> Optional[Union[dict, Error]]:
+) -> Optional[Union[CustomerBalance, Error]]:
+    """This endpoint requires authentication by any KittyCAD user. It gets the balance information for the authenticated user."""  # noqa: E501
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[Optional[Union[dict, Error]]]:
+) -> Response[Optional[Union[CustomerBalance, Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-) -> Optional[Union[dict, Error]]:
+) -> Optional[Union[CustomerBalance, Error]]:
+    """This endpoint requires authentication by any KittyCAD user. It gets the balance information for the authenticated user."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.4/kittycad/api/meta/ping.py` & `kittycad-0.4.5/kittycad/api/meta/ping.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/ping".format(client.base_url)  # noqa: E501
+    url = "{}/ping".format(
+        client.base_url,
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
@@ -65,15 +67,14 @@
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: Client,
 ) -> Optional[Union[Pong, Error]]:
-
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
@@ -89,13 +90,12 @@
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: Client,
 ) -> Optional[Union[Pong, Error]]:
-
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.4/kittycad/api/modeling/cmd.py` & `kittycad-0.4.5/kittycad/api/modeling/cmd.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 
 
 def _get_kwargs(
     body: ModelingCmdReq,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/modeling/cmd".format(client.base_url)  # noqa: E501
+    url = "{}/modeling/cmd".format(
+        client.base_url,
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
```

### Comparing `kittycad-0.4.4/kittycad/api/modeling/cmd_batch.py` & `kittycad-0.4.5/kittycad/api/modeling/cmd_batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 
 
 def _get_kwargs(
     body: ModelingCmdReqBatch,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/modeling/cmd_batch".format(client.base_url)  # noqa: E501
+    url = "{}/modeling/cmd_batch".format(
+        client.base_url,
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
@@ -73,15 +75,14 @@
 
 
 def sync(
     body: ModelingCmdReqBatch,
     *,
     client: Client,
 ) -> Optional[Union[ModelingOutcomes, Error]]:
-
     return sync_detailed(
         body=body,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
@@ -101,14 +102,13 @@
 
 
 async def asyncio(
     body: ModelingCmdReqBatch,
     *,
     client: Client,
 ) -> Optional[Union[ModelingOutcomes, Error]]:
-
     return (
         await asyncio_detailed(
             body=body,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.4/kittycad/api/modeling/modeling_commands_ws.py` & `kittycad-0.4.5/kittycad/api/payments/delete_payment_method_for_user.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,90 +1,110 @@
-from typing import Any, Dict
+from typing import Any, Dict, Optional
 
 import httpx
 
 from ...client import Client
+from ...models.error import Error
 from ...types import Response
 
 
 def _get_kwargs(
+    id: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/ws/modeling/commands".format(client.base_url)  # noqa: E501
+    url = "{}/user/payment/methods/{id}".format(
+        client.base_url,
+        id=id,
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(*, response: httpx.Response):
-    return
+def _parse_response(*, response: httpx.Response) -> Optional[Error]:
+    return None
+    if response.status_code == 400:
+        response_4XX = Error.from_dict(response.json())
+        return response_4XX
+    if response.status_code == 500:
+        response_5XX = Error.from_dict(response.json())
+        return response_5XX
+    return Error.from_dict(response.json())
 
 
-def _build_response(*, response: httpx.Response) -> Response[Any]:
+def _build_response(*, response: httpx.Response) -> Response[Optional[Error]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
+    id: str,
     *,
     client: Client,
-) -> Response[Any]:
+) -> Response[Optional[Error]]:
     kwargs = _get_kwargs(
+        id=id,
         client=client,
     )
 
-    response = httpx.get(
+    response = httpx.delete(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
+    id: str,
     *,
     client: Client,
-):
-    """Pass those commands to the engine via websocket, and pass responses back to the client. Basically, this is a websocket proxy between the frontend/client and the engine."""  # noqa: E501
+) -> Optional[Error]:
+    """This endpoint requires authentication by any KittyCAD user. It deletes the specified payment method for the authenticated user."""  # noqa: E501
 
     return sync_detailed(
+        id=id,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
+    id: str,
     *,
     client: Client,
-) -> Response[Any]:
+) -> Response[Optional[Error]]:
     kwargs = _get_kwargs(
+        id=id,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.get(**kwargs)
+        response = await _client.delete(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
+    id: str,
     *,
     client: Client,
-):
-    """Pass those commands to the engine via websocket, and pass responses back to the client. Basically, this is a websocket proxy between the frontend/client and the engine."""  # noqa: E501
+) -> Optional[Error]:
+    """This endpoint requires authentication by any KittyCAD user. It deletes the specified payment method for the authenticated user."""  # noqa: E501
 
     return (
         await asyncio_detailed(
+            id=id,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.4/kittycad/api/payments/create_payment_information_for_user.py` & `kittycad-0.4.5/kittycad/api/payments/update_payment_information_for_user.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,32 +10,34 @@
 
 
 def _get_kwargs(
     body: BillingInfo,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/user/payment".format(client.base_url)  # noqa: E501
+    url = "{}/user/payment".format(
+        client.base_url,
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "content": body,
     }
 
 
 def _parse_response(*, response: httpx.Response) -> Optional[Union[Customer, Error]]:
-    if response.status_code == 201:
-        response_201 = Customer.from_dict(response.json())
-        return response_201
+    if response.status_code == 200:
+        response_200 = Customer.from_dict(response.json())
+        return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
     return Error.from_dict(response.json())
@@ -58,29 +60,30 @@
     client: Client,
 ) -> Response[Optional[Union[Customer, Error]]]:
     kwargs = _get_kwargs(
         body=body,
         client=client,
     )
 
-    response = httpx.post(
+    response = httpx.put(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
     body: BillingInfo,
     *,
     client: Client,
 ) -> Optional[Union[Customer, Error]]:
     """This includes billing address, phone, and name.
-    This endpoint requires authentication by any KittyCAD user. It creates the payment information for the authenticated user."""  # noqa: E501
+    This endpoint requires authentication by any KittyCAD user. It updates the payment information for the authenticated user.
+    """  # noqa: E501
 
     return sync_detailed(
         body=body,
         client=client,
     ).parsed
 
 
@@ -91,26 +94,27 @@
 ) -> Response[Optional[Union[Customer, Error]]]:
     kwargs = _get_kwargs(
         body=body,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.post(**kwargs)
+        response = await _client.put(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     body: BillingInfo,
     *,
     client: Client,
 ) -> Optional[Union[Customer, Error]]:
     """This includes billing address, phone, and name.
-    This endpoint requires authentication by any KittyCAD user. It creates the payment information for the authenticated user."""  # noqa: E501
+    This endpoint requires authentication by any KittyCAD user. It updates the payment information for the authenticated user.
+    """  # noqa: E501
 
     return (
         await asyncio_detailed(
             body=body,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.4/kittycad/api/payments/create_payment_intent_for_user.py` & `kittycad-0.4.5/kittycad/api/payments/create_payment_intent_for_user.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/user/payment/intent".format(client.base_url)  # noqa: E501
+    url = "{}/user/payment/intent".format(
+        client.base_url,
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
```

### Comparing `kittycad-0.4.4/kittycad/api/payments/delete_payment_information_for_user.py` & `kittycad-0.4.5/kittycad/api/payments/delete_payment_information_for_user.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/user/payment".format(client.base_url)  # noqa: E501
+    url = "{}/user/payment".format(
+        client.base_url,
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
@@ -61,15 +63,16 @@
 
 
 def sync(
     *,
     client: Client,
 ) -> Optional[Error]:
     """This includes billing address, phone, and name.
-    This endpoint requires authentication by any KittyCAD user. It deletes the payment information for the authenticated user."""  # noqa: E501
+    This endpoint requires authentication by any KittyCAD user. It deletes the payment information for the authenticated user.
+    """  # noqa: E501
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
@@ -87,14 +90,15 @@
 
 
 async def asyncio(
     *,
     client: Client,
 ) -> Optional[Error]:
     """This includes billing address, phone, and name.
-    This endpoint requires authentication by any KittyCAD user. It deletes the payment information for the authenticated user."""  # noqa: E501
+    This endpoint requires authentication by any KittyCAD user. It deletes the payment information for the authenticated user.
+    """  # noqa: E501
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.4/kittycad/api/payments/delete_payment_method_for_user.py` & `kittycad-0.4.5/kittycad/api/users/get_user_onboarding_self.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,107 +1,105 @@
-from typing import Any, Dict, Optional
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
+from ...models.onboarding import Onboarding
 from ...types import Response
 
 
 def _get_kwargs(
-    id: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/user/payment/methods/{id}".format(client.base_url, id=id)  # noqa: E501
+    url = "{}/user/onboarding".format(
+        client.base_url,
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Error]:
-    return None
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Onboarding, Error]]:
+    if response.status_code == 200:
+        response_200 = Onboarding.from_dict(response.json())
+        return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
     return Error.from_dict(response.json())
 
 
-def _build_response(*, response: httpx.Response) -> Response[Optional[Error]]:
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Optional[Union[Onboarding, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    id: str,
     *,
     client: Client,
-) -> Response[Optional[Error]]:
+) -> Response[Optional[Union[Onboarding, Error]]]:
     kwargs = _get_kwargs(
-        id=id,
         client=client,
     )
 
-    response = httpx.delete(
+    response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    id: str,
     *,
     client: Client,
-) -> Optional[Error]:
-    """This endpoint requires authentication by any KittyCAD user. It deletes the specified payment method for the authenticated user."""  # noqa: E501
+) -> Optional[Union[Onboarding, Error]]:
+    """Checks key part of their api usage to determine their onboarding progress"""  # noqa: E501
 
     return sync_detailed(
-        id=id,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    id: str,
     *,
     client: Client,
-) -> Response[Optional[Error]]:
+) -> Response[Optional[Union[Onboarding, Error]]]:
     kwargs = _get_kwargs(
-        id=id,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.delete(**kwargs)
+        response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    id: str,
     *,
     client: Client,
-) -> Optional[Error]:
-    """This endpoint requires authentication by any KittyCAD user. It deletes the specified payment method for the authenticated user."""  # noqa: E501
+) -> Optional[Union[Onboarding, Error]]:
+    """Checks key part of their api usage to determine their onboarding progress"""  # noqa: E501
 
     return (
         await asyncio_detailed(
-            id=id,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.4/kittycad/api/payments/get_payment_balance_for_user.py` & `kittycad-0.4.5/kittycad/api/users/update_user_self.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,105 +1,116 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.customer_balance import CustomerBalance
 from ...models.error import Error
+from ...models.update_user import UpdateUser
+from ...models.user import User
 from ...types import Response
 
 
 def _get_kwargs(
+    body: UpdateUser,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/user/payment/balance".format(client.base_url)  # noqa: E501
+    url = "{}/user".format(
+        client.base_url,
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "content": body,
     }
 
 
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[CustomerBalance, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[User, Error]]:
     if response.status_code == 200:
-        response_200 = CustomerBalance.from_dict(response.json())
+        response_200 = User.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
     return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Optional[Union[CustomerBalance, Error]]]:
+) -> Response[Optional[Union[User, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
+    body: UpdateUser,
     *,
     client: Client,
-) -> Response[Optional[Union[CustomerBalance, Error]]]:
+) -> Response[Optional[Union[User, Error]]]:
     kwargs = _get_kwargs(
+        body=body,
         client=client,
     )
 
-    response = httpx.get(
+    response = httpx.put(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
+    body: UpdateUser,
     *,
     client: Client,
-) -> Optional[Union[CustomerBalance, Error]]:
-    """This endpoint requires authentication by any KittyCAD user. It gets the balance information for the authenticated user."""  # noqa: E501
+) -> Optional[Union[User, Error]]:
+    """This endpoint requires authentication by any KittyCAD user. It updates information about the authenticated user."""  # noqa: E501
 
     return sync_detailed(
+        body=body,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
+    body: UpdateUser,
     *,
     client: Client,
-) -> Response[Optional[Union[CustomerBalance, Error]]]:
+) -> Response[Optional[Union[User, Error]]]:
     kwargs = _get_kwargs(
+        body=body,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.get(**kwargs)
+        response = await _client.put(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
+    body: UpdateUser,
     *,
     client: Client,
-) -> Optional[Union[CustomerBalance, Error]]:
-    """This endpoint requires authentication by any KittyCAD user. It gets the balance information for the authenticated user."""  # noqa: E501
+) -> Optional[Union[User, Error]]:
+    """This endpoint requires authentication by any KittyCAD user. It updates information about the authenticated user."""  # noqa: E501
 
     return (
         await asyncio_detailed(
+            body=body,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.4/kittycad/api/payments/get_payment_information_for_user.py` & `kittycad-0.4.5/kittycad/api/payments/get_payment_information_for_user.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/user/payment".format(client.base_url)  # noqa: E501
+    url = "{}/user/payment".format(
+        client.base_url,
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
@@ -66,15 +68,16 @@
 
 
 def sync(
     *,
     client: Client,
 ) -> Optional[Union[Customer, Error]]:
     """This includes billing address, phone, and name.
-    This endpoint requires authentication by any KittyCAD user. It gets the payment information for the authenticated user."""  # noqa: E501
+    This endpoint requires authentication by any KittyCAD user. It gets the payment information for the authenticated user.
+    """  # noqa: E501
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
@@ -92,14 +95,15 @@
 
 
 async def asyncio(
     *,
     client: Client,
 ) -> Optional[Union[Customer, Error]]:
     """This includes billing address, phone, and name.
-    This endpoint requires authentication by any KittyCAD user. It gets the payment information for the authenticated user."""  # noqa: E501
+    This endpoint requires authentication by any KittyCAD user. It gets the payment information for the authenticated user.
+    """  # noqa: E501
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.4/kittycad/api/payments/list_invoices_for_user.py` & `kittycad-0.4.5/kittycad/api/payments/list_invoices_for_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/user/payment/invoices".format(client.base_url)  # noqa: E501
+    url = "{}/user/payment/invoices".format(
+        client.base_url,
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
```

### Comparing `kittycad-0.4.4/kittycad/api/payments/list_payment_methods_for_user.py` & `kittycad-0.4.5/kittycad/api/payments/list_payment_methods_for_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/user/payment/methods".format(client.base_url)  # noqa: E501
+    url = "{}/user/payment/methods".format(
+        client.base_url,
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
```

### Comparing `kittycad-0.4.4/kittycad/api/payments/update_payment_information_for_user.py` & `kittycad-0.4.5/kittycad/api/payments/create_payment_information_for_user.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,32 +10,34 @@
 
 
 def _get_kwargs(
     body: BillingInfo,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/user/payment".format(client.base_url)  # noqa: E501
+    url = "{}/user/payment".format(
+        client.base_url,
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "content": body,
     }
 
 
 def _parse_response(*, response: httpx.Response) -> Optional[Union[Customer, Error]]:
-    if response.status_code == 200:
-        response_200 = Customer.from_dict(response.json())
-        return response_200
+    if response.status_code == 201:
+        response_201 = Customer.from_dict(response.json())
+        return response_201
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
     return Error.from_dict(response.json())
@@ -58,29 +60,30 @@
     client: Client,
 ) -> Response[Optional[Union[Customer, Error]]]:
     kwargs = _get_kwargs(
         body=body,
         client=client,
     )
 
-    response = httpx.put(
+    response = httpx.post(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
     body: BillingInfo,
     *,
     client: Client,
 ) -> Optional[Union[Customer, Error]]:
     """This includes billing address, phone, and name.
-    This endpoint requires authentication by any KittyCAD user. It updates the payment information for the authenticated user."""  # noqa: E501
+    This endpoint requires authentication by any KittyCAD user. It creates the payment information for the authenticated user.
+    """  # noqa: E501
 
     return sync_detailed(
         body=body,
         client=client,
     ).parsed
 
 
@@ -91,26 +94,27 @@
 ) -> Response[Optional[Union[Customer, Error]]]:
     kwargs = _get_kwargs(
         body=body,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.put(**kwargs)
+        response = await _client.post(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     body: BillingInfo,
     *,
     client: Client,
 ) -> Optional[Union[Customer, Error]]:
     """This includes billing address, phone, and name.
-    This endpoint requires authentication by any KittyCAD user. It updates the payment information for the authenticated user."""  # noqa: E501
+    This endpoint requires authentication by any KittyCAD user. It creates the payment information for the authenticated user.
+    """  # noqa: E501
 
     return (
         await asyncio_detailed(
             body=body,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.4/kittycad/api/payments/validate_customer_tax_information_for_user.py` & `kittycad-0.4.5/kittycad/api/payments/validate_customer_tax_information_for_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/user/payment/tax".format(client.base_url)  # noqa: E501
+    url = "{}/user/payment/tax".format(
+        client.base_url,
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
```

### Comparing `kittycad-0.4.4/kittycad/api/unit/get_angle_unit_conversion.py` & `kittycad-0.4.5/kittycad/api/unit/get_angle_unit_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,19 @@
     input_unit: UnitAngle,
     output_unit: UnitAngle,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
     url = "{}/unit/conversion/angle/{input_unit}/{output_unit}".format(
-        client.base_url, input_unit=input_unit, output_unit=output_unit
+        client.base_url,
+        input_unit=input_unit,
+        output_unit=output_unit,
     )  # noqa: E501
+
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
 
     headers: Dict[str, Any] = client.get_headers()
```

### Comparing `kittycad-0.4.4/kittycad/api/unit/get_area_unit_conversion.py` & `kittycad-0.4.5/kittycad/api/unit/get_area_unit_conversion.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,16 +13,19 @@
     input_unit: UnitArea,
     output_unit: UnitArea,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
     url = "{}/unit/conversion/area/{input_unit}/{output_unit}".format(
-        client.base_url, input_unit=input_unit, output_unit=output_unit
+        client.base_url,
+        input_unit=input_unit,
+        output_unit=output_unit,
     )  # noqa: E501
+
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
 
     headers: Dict[str, Any] = client.get_headers()
```

### Comparing `kittycad-0.4.4/kittycad/api/unit/get_current_unit_conversion.py` & `kittycad-0.4.5/kittycad/api/unit/get_current_unit_conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,19 @@
     input_unit: UnitCurrent,
     output_unit: UnitCurrent,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
     url = "{}/unit/conversion/current/{input_unit}/{output_unit}".format(
-        client.base_url, input_unit=input_unit, output_unit=output_unit
+        client.base_url,
+        input_unit=input_unit,
+        output_unit=output_unit,
     )  # noqa: E501
+
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
 
     headers: Dict[str, Any] = client.get_headers()
```

### Comparing `kittycad-0.4.4/kittycad/api/unit/get_energy_unit_conversion.py` & `kittycad-0.4.5/kittycad/api/unit/get_energy_unit_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,19 @@
     input_unit: UnitEnergy,
     output_unit: UnitEnergy,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
     url = "{}/unit/conversion/energy/{input_unit}/{output_unit}".format(
-        client.base_url, input_unit=input_unit, output_unit=output_unit
+        client.base_url,
+        input_unit=input_unit,
+        output_unit=output_unit,
     )  # noqa: E501
+
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
 
     headers: Dict[str, Any] = client.get_headers()
```

### Comparing `kittycad-0.4.4/kittycad/api/unit/get_force_unit_conversion.py` & `kittycad-0.4.5/kittycad/api/unit/get_force_unit_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,19 @@
     input_unit: UnitForce,
     output_unit: UnitForce,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
     url = "{}/unit/conversion/force/{input_unit}/{output_unit}".format(
-        client.base_url, input_unit=input_unit, output_unit=output_unit
+        client.base_url,
+        input_unit=input_unit,
+        output_unit=output_unit,
     )  # noqa: E501
+
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
 
     headers: Dict[str, Any] = client.get_headers()
```

### Comparing `kittycad-0.4.4/kittycad/api/unit/get_frequency_unit_conversion.py` & `kittycad-0.4.5/kittycad/api/unit/get_frequency_unit_conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,19 @@
     input_unit: UnitFrequency,
     output_unit: UnitFrequency,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
     url = "{}/unit/conversion/frequency/{input_unit}/{output_unit}".format(
-        client.base_url, input_unit=input_unit, output_unit=output_unit
+        client.base_url,
+        input_unit=input_unit,
+        output_unit=output_unit,
     )  # noqa: E501
+
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
 
     headers: Dict[str, Any] = client.get_headers()
```

### Comparing `kittycad-0.4.4/kittycad/api/unit/get_length_unit_conversion.py` & `kittycad-0.4.5/kittycad/api/unit/get_length_unit_conversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,19 @@
     input_unit: UnitLength,
     output_unit: UnitLength,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
     url = "{}/unit/conversion/length/{input_unit}/{output_unit}".format(
-        client.base_url, input_unit=input_unit, output_unit=output_unit
+        client.base_url,
+        input_unit=input_unit,
+        output_unit=output_unit,
     )  # noqa: E501
+
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
 
     headers: Dict[str, Any] = client.get_headers()
```

### Comparing `kittycad-0.4.4/kittycad/api/unit/get_mass_unit_conversion.py` & `kittycad-0.4.5/kittycad/api/unit/get_mass_unit_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,19 @@
     input_unit: UnitMass,
     output_unit: UnitMass,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
     url = "{}/unit/conversion/mass/{input_unit}/{output_unit}".format(
-        client.base_url, input_unit=input_unit, output_unit=output_unit
+        client.base_url,
+        input_unit=input_unit,
+        output_unit=output_unit,
     )  # noqa: E501
+
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
 
     headers: Dict[str, Any] = client.get_headers()
```

### Comparing `kittycad-0.4.4/kittycad/api/unit/get_power_unit_conversion.py` & `kittycad-0.4.5/kittycad/api/unit/get_power_unit_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,19 @@
     input_unit: UnitPower,
     output_unit: UnitPower,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
     url = "{}/unit/conversion/power/{input_unit}/{output_unit}".format(
-        client.base_url, input_unit=input_unit, output_unit=output_unit
+        client.base_url,
+        input_unit=input_unit,
+        output_unit=output_unit,
     )  # noqa: E501
+
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
 
     headers: Dict[str, Any] = client.get_headers()
```

### Comparing `kittycad-0.4.4/kittycad/api/unit/get_pressure_unit_conversion.py` & `kittycad-0.4.5/kittycad/api/unit/get_pressure_unit_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,19 @@
     input_unit: UnitPressure,
     output_unit: UnitPressure,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
     url = "{}/unit/conversion/pressure/{input_unit}/{output_unit}".format(
-        client.base_url, input_unit=input_unit, output_unit=output_unit
+        client.base_url,
+        input_unit=input_unit,
+        output_unit=output_unit,
     )  # noqa: E501
+
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
 
     headers: Dict[str, Any] = client.get_headers()
```

### Comparing `kittycad-0.4.4/kittycad/api/unit/get_temperature_unit_conversion.py` & `kittycad-0.4.5/kittycad/api/unit/get_temperature_unit_conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,19 @@
     input_unit: UnitTemperature,
     output_unit: UnitTemperature,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
     url = "{}/unit/conversion/temperature/{input_unit}/{output_unit}".format(
-        client.base_url, input_unit=input_unit, output_unit=output_unit
+        client.base_url,
+        input_unit=input_unit,
+        output_unit=output_unit,
     )  # noqa: E501
+
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
 
     headers: Dict[str, Any] = client.get_headers()
```

### Comparing `kittycad-0.4.4/kittycad/api/unit/get_torque_unit_conversion.py` & `kittycad-0.4.5/kittycad/api/unit/get_torque_unit_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,19 @@
     input_unit: UnitTorque,
     output_unit: UnitTorque,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
     url = "{}/unit/conversion/torque/{input_unit}/{output_unit}".format(
-        client.base_url, input_unit=input_unit, output_unit=output_unit
+        client.base_url,
+        input_unit=input_unit,
+        output_unit=output_unit,
     )  # noqa: E501
+
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
 
     headers: Dict[str, Any] = client.get_headers()
```

### Comparing `kittycad-0.4.4/kittycad/api/unit/get_volume_unit_conversion.py` & `kittycad-0.4.5/kittycad/api/unit/get_volume_unit_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,19 @@
     input_unit: UnitVolume,
     output_unit: UnitVolume,
     value: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
     url = "{}/unit/conversion/volume/{input_unit}/{output_unit}".format(
-        client.base_url, input_unit=input_unit, output_unit=output_unit
+        client.base_url,
+        input_unit=input_unit,
+        output_unit=output_unit,
     )  # noqa: E501
+
     if value is not None:
         if "?" in url:
             url = url + "&value=" + str(value)
         else:
             url = url + "?value=" + str(value)
 
     headers: Dict[str, Any] = client.get_headers()
```

### Comparing `kittycad-0.4.4/kittycad/api/users/delete_user_self.py` & `kittycad-0.4.5/kittycad/api/users/delete_user_self.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/user".format(client.base_url)  # noqa: E501
+    url = "{}/user".format(
+        client.base_url,
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
@@ -61,15 +63,16 @@
 
 
 def sync(
     *,
     client: Client,
 ) -> Optional[Error]:
     """This endpoint requires authentication by any KittyCAD user. It deletes the authenticated user from KittyCAD's database.
-    This call will only succeed if all invoices associated with the user have been paid in full and there is no outstanding balance."""  # noqa: E501
+    This call will only succeed if all invoices associated with the user have been paid in full and there is no outstanding balance.
+    """  # noqa: E501
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
@@ -87,14 +90,15 @@
 
 
 async def asyncio(
     *,
     client: Client,
 ) -> Optional[Error]:
     """This endpoint requires authentication by any KittyCAD user. It deletes the authenticated user from KittyCAD's database.
-    This call will only succeed if all invoices associated with the user have been paid in full and there is no outstanding balance."""  # noqa: E501
+    This call will only succeed if all invoices associated with the user have been paid in full and there is no outstanding balance.
+    """  # noqa: E501
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.4/kittycad/api/users/get_session_for_user.py` & `kittycad-0.4.5/kittycad/api/users/get_session_for_user.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,18 @@
 
 
 def _get_kwargs(
     token: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/user/session/{token}".format(client.base_url, token=token)  # noqa: E501
+    url = "{}/user/session/{token}".format(
+        client.base_url,
+        token=token,
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
```

### Comparing `kittycad-0.4.4/kittycad/api/users/get_user.py` & `kittycad-0.4.5/kittycad/api/users/get_user.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,18 @@
 
 
 def _get_kwargs(
     id: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/users/{id}".format(client.base_url, id=id)  # noqa: E501
+    url = "{}/users/{id}".format(
+        client.base_url,
+        id=id,
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
```

### Comparing `kittycad-0.4.4/kittycad/api/users/get_user_extended.py` & `kittycad-0.4.5/kittycad/api/users/get_user_extended.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,18 @@
 
 
 def _get_kwargs(
     id: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/users-extended/{id}".format(client.base_url, id=id)  # noqa: E501
+    url = "{}/users-extended/{id}".format(
+        client.base_url,
+        id=id,
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
```

### Comparing `kittycad-0.4.4/kittycad/api/users/get_user_front_hash_self.py` & `kittycad-0.4.5/kittycad/api/hidden/auth_email.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,102 +1,114 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
+from ...models.email_authentication_form import EmailAuthenticationForm
 from ...models.error import Error
+from ...models.verification_token import VerificationToken
 from ...types import Response
 
 
 def _get_kwargs(
+    body: EmailAuthenticationForm,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/user/front-hash".format(client.base_url)  # noqa: E501
+    url = "{}/auth/email".format(
+        client.base_url,
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "content": body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[str, Error]]:
-    if response.status_code == 200:
-        response_200 = response.text
-        return response_200
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[VerificationToken, Error]]:
+    if response.status_code == 201:
+        response_201 = VerificationToken.from_dict(response.json())
+        return response_201
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
     return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Optional[Union[str, Error]]]:
+) -> Response[Optional[Union[VerificationToken, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
+    body: EmailAuthenticationForm,
     *,
     client: Client,
-) -> Response[Optional[Union[str, Error]]]:
+) -> Response[Optional[Union[VerificationToken, Error]]]:
     kwargs = _get_kwargs(
+        body=body,
         client=client,
     )
 
-    response = httpx.get(
+    response = httpx.post(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
+    body: EmailAuthenticationForm,
     *,
     client: Client,
-) -> Optional[Union[str, Error]]:
-    """This info is sent to front when initialing the front chat, it prevents impersonations using js hacks in the browser"""  # noqa: E501
-
+) -> Optional[Union[VerificationToken, Error]]:
     return sync_detailed(
+        body=body,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
+    body: EmailAuthenticationForm,
     *,
     client: Client,
-) -> Response[Optional[Union[str, Error]]]:
+) -> Response[Optional[Union[VerificationToken, Error]]]:
     kwargs = _get_kwargs(
+        body=body,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.get(**kwargs)
+        response = await _client.post(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
+    body: EmailAuthenticationForm,
     *,
     client: Client,
-) -> Optional[Union[str, Error]]:
-    """This info is sent to front when initialing the front chat, it prevents impersonations using js hacks in the browser"""  # noqa: E501
-
+) -> Optional[Union[VerificationToken, Error]]:
     return (
         await asyncio_detailed(
+            body=body,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.4/kittycad/api/users/get_user_self.py` & `kittycad-0.4.5/kittycad/api/users/get_user_self_extended.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,62 +1,66 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.user import User
+from ...models.extended_user import ExtendedUser
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/user".format(client.base_url)  # noqa: E501
+    url = "{}/user/extended".format(
+        client.base_url,
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[User, Error]]:
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[ExtendedUser, Error]]:
     if response.status_code == 200:
-        response_200 = User.from_dict(response.json())
+        response_200 = ExtendedUser.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
     return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Optional[Union[User, Error]]]:
+) -> Response[Optional[Union[ExtendedUser, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[Optional[Union[User, Error]]]:
+) -> Response[Optional[Union[ExtendedUser, Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
@@ -64,42 +68,42 @@
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: Client,
-) -> Optional[Union[User, Error]]:
+) -> Optional[Union[ExtendedUser, Error]]:
     """Get the user information for the authenticated user.
-    Alternatively, you can also use the `/users/me` endpoint."""  # noqa: E501
+    Alternatively, you can also use the `/users-extended/me` endpoint."""  # noqa: E501
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[Optional[Union[User, Error]]]:
+) -> Response[Optional[Union[ExtendedUser, Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-) -> Optional[Union[User, Error]]:
+) -> Optional[Union[ExtendedUser, Error]]:
     """Get the user information for the authenticated user.
-    Alternatively, you can also use the `/users/me` endpoint."""  # noqa: E501
+    Alternatively, you can also use the `/users-extended/me` endpoint."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.4/kittycad/api/users/get_user_self_extended.py` & `kittycad-0.4.5/kittycad/api/apps/apps_github_consent.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,66 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
+from ...models.app_client_info import AppClientInfo
 from ...models.error import Error
-from ...models.extended_user import ExtendedUser
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/user/extended".format(client.base_url)  # noqa: E501
+    url = "{}/apps/github/consent".format(
+        client.base_url,
+    )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[ExtendedUser, Error]]:
+) -> Optional[Union[AppClientInfo, Error]]:
     if response.status_code == 200:
-        response_200 = ExtendedUser.from_dict(response.json())
+        response_200 = AppClientInfo.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
     return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Optional[Union[ExtendedUser, Error]]]:
+) -> Response[Optional[Union[AppClientInfo, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[Optional[Union[ExtendedUser, Error]]]:
+) -> Response[Optional[Union[AppClientInfo, Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
@@ -66,42 +68,44 @@
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: Client,
-) -> Optional[Union[ExtendedUser, Error]]:
-    """Get the user information for the authenticated user.
-    Alternatively, you can also use the `/users-extended/me` endpoint."""  # noqa: E501
+) -> Optional[Union[AppClientInfo, Error]]:
+    """This is different than OAuth 2.0 authentication for users. This endpoint grants access for KittyCAD to access user's repos.
+    The user doesn't need KittyCAD OAuth authorization for this endpoint, this is purely for the GitHub permissions to access repos.
+    """  # noqa: E501
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[Optional[Union[ExtendedUser, Error]]]:
+) -> Response[Optional[Union[AppClientInfo, Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-) -> Optional[Union[ExtendedUser, Error]]:
-    """Get the user information for the authenticated user.
-    Alternatively, you can also use the `/users-extended/me` endpoint."""  # noqa: E501
+) -> Optional[Union[AppClientInfo, Error]]:
+    """This is different than OAuth 2.0 authentication for users. This endpoint grants access for KittyCAD to access user's repos.
+    The user doesn't need KittyCAD OAuth authorization for this endpoint, this is purely for the GitHub permissions to access repos.
+    """  # noqa: E501
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.4/kittycad/api/users/list_users.py` & `kittycad-0.4.5/kittycad/api/users/list_users.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,25 +12,30 @@
 def _get_kwargs(
     sort_by: CreatedAtSortMode,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
 ) -> Dict[str, Any]:
-    url = "{}/users".format(client.base_url)  # noqa: E501
+    url = "{}/users".format(
+        client.base_url,
+    )  # noqa: E501
+
     if limit is not None:
         if "?" in url:
             url = url + "&limit=" + str(limit)
         else:
             url = url + "?limit=" + str(limit)
+
     if page_token is not None:
         if "?" in url:
             url = url + "&page_token=" + str(page_token)
         else:
             url = url + "?page_token=" + str(page_token)
+
     if sort_by is not None:
         if "?" in url:
             url = url + "&sort_by=" + str(sort_by)
         else:
             url = url + "?sort_by=" + str(sort_by)
 
     headers: Dict[str, Any] = client.get_headers()
```

### Comparing `kittycad-0.4.4/kittycad/api/users/list_users_extended.py` & `kittycad-0.4.5/kittycad/api/users/list_users_extended.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,25 +12,30 @@
 def _get_kwargs(
     sort_by: CreatedAtSortMode,
     *,
     client: Client,
     limit: Optional[int] = None,
     page_token: Optional[str] = None,
 ) -> Dict[str, Any]:
-    url = "{}/users-extended".format(client.base_url)  # noqa: E501
+    url = "{}/users-extended".format(
+        client.base_url,
+    )  # noqa: E501
+
     if limit is not None:
         if "?" in url:
             url = url + "&limit=" + str(limit)
         else:
             url = url + "?limit=" + str(limit)
+
     if page_token is not None:
         if "?" in url:
             url = url + "&page_token=" + str(page_token)
         else:
             url = url + "?page_token=" + str(page_token)
+
     if sort_by is not None:
         if "?" in url:
             url = url + "&sort_by=" + str(sort_by)
         else:
             url = url + "?sort_by=" + str(sort_by)
 
     headers: Dict[str, Any] = client.get_headers()
```

### Comparing `kittycad-0.4.4/kittycad/client.py` & `kittycad-0.4.5/kittycad/client.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.4/kittycad/client_test.py` & `kittycad-0.4.5/kittycad/client_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,17 @@
     ExtendedUserResultsPage,
     FileConversion,
     FileExportFormat,
     FileImportFormat,
     FileMass,
     FileVolume,
     Pong,
+    UnitDensity,
+    UnitMass,
+    UnitVolume,
     User,
 )
 
 
 def test_get_session():
     # Create our client.
     client = ClientFromEnv()
@@ -167,14 +170,16 @@
 
     # Get the fc.
     result: Union[FileMass, Error, None] = create_file_mass.sync(
         client=client,
         body=content,
         src_format=FileImportFormat.OBJ,
         material_density=1.0,
+        material_density_unit=UnitDensity.KG_M3,
+        output_unit=UnitMass.G,
     )
 
     assert isinstance(result, FileMass)
 
     fm: FileMass = result
 
     print(f"FileMass: {fm}")
@@ -194,15 +199,18 @@
     dir_path = os.path.dirname(os.path.realpath(__file__))
     file = open(os.path.join(dir_path, "../assets/testing.obj"), "rb")
     content = file.read()
     file.close()
 
     # Get the fc.
     result: Union[FileVolume, Error, None] = create_file_volume.sync(
-        client=client, body=content, src_format=FileImportFormat.OBJ
+        client=client,
+        body=content,
+        src_format=FileImportFormat.OBJ,
+        output_unit=UnitVolume.CM3,
     )
 
     assert isinstance(result, FileVolume)
 
     fv: FileVolume = result
 
     print(f"FileVolume: {fv}")
```

### Comparing `kittycad-0.4.4/kittycad/examples_test.py` & `kittycad-0.4.5/kittycad/examples_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,22 +138,24 @@
 from kittycad.models.billing_info import BillingInfo
 from kittycad.models.code_language import CodeLanguage
 from kittycad.models.created_at_sort_mode import CreatedAtSortMode
 from kittycad.models.email_authentication_form import EmailAuthenticationForm
 from kittycad.models.file_export_format import FileExportFormat
 from kittycad.models.file_import_format import FileImportFormat
 from kittycad.models.image_type import ImageType
-from kittycad.models.modeling_cmd import ModelingCmd
+from kittycad.models.modeling_cmd import MovePathPen
 from kittycad.models.modeling_cmd_id import ModelingCmdId
 from kittycad.models.modeling_cmd_req import ModelingCmdReq
 from kittycad.models.modeling_cmd_req_batch import ModelingCmdReqBatch
 from kittycad.models.physics_constant_name import PhysicsConstantName
+from kittycad.models.point3d import Point3d
 from kittycad.models.unit_angle import UnitAngle
 from kittycad.models.unit_area import UnitArea
 from kittycad.models.unit_current import UnitCurrent
+from kittycad.models.unit_density import UnitDensity
 from kittycad.models.unit_energy import UnitEnergy
 from kittycad.models.unit_force import UnitForce
 from kittycad.models.unit_frequency import UnitFrequency
 from kittycad.models.unit_length import UnitLength
 from kittycad.models.unit_mass import UnitMass
 from kittycad.models.unit_power import UnitPower
 from kittycad.models.unit_pressure import UnitPressure
@@ -977,14 +979,15 @@
 @pytest.mark.skip
 def test_create_file_center_of_mass():
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[Union[FileCenterOfMass, Error]] = create_file_center_of_mass.sync(
         client=client,
+        output_unit=UnitLength.CM,
         src_format=FileImportFormat.DAE,
         body=bytes("some bytes", "utf-8"),
     )
 
     if isinstance(result, Error) or result is None:
         print(result)
         raise Exception("Error in response")
@@ -993,14 +996,15 @@
     print(body)
 
     # OR if you need more info (e.g. status_code)
     response: Response[
         Optional[Union[FileCenterOfMass, Error]]
     ] = create_file_center_of_mass.sync_detailed(
         client=client,
+        output_unit=UnitLength.CM,
         src_format=FileImportFormat.DAE,
         body=bytes("some bytes", "utf-8"),
     )
 
 
 # OR run async
 @pytest.mark.asyncio
@@ -1009,23 +1013,25 @@
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[
         Union[FileCenterOfMass, Error]
     ] = await create_file_center_of_mass.asyncio(
         client=client,
+        output_unit=UnitLength.CM,
         src_format=FileImportFormat.DAE,
         body=bytes("some bytes", "utf-8"),
     )
 
     # OR run async with more info
     response: Response[
         Optional[Union[FileCenterOfMass, Error]]
     ] = await create_file_center_of_mass.asyncio_detailed(
         client=client,
+        output_unit=UnitLength.CM,
         src_format=FileImportFormat.DAE,
         body=bytes("some bytes", "utf-8"),
     )
 
 
 @pytest.mark.skip
 def test_create_file_conversion_with_base64_helper():
@@ -1090,14 +1096,16 @@
 def test_create_file_density():
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[Union[FileDensity, Error]] = create_file_density.sync(
         client=client,
         material_mass=3.14,
+        material_mass_unit=UnitMass.G,
+        output_unit=UnitDensity.LB_FT3,
         src_format=FileImportFormat.DAE,
         body=bytes("some bytes", "utf-8"),
     )
 
     if isinstance(result, Error) or result is None:
         print(result)
         raise Exception("Error in response")
@@ -1107,14 +1115,16 @@
 
     # OR if you need more info (e.g. status_code)
     response: Response[
         Optional[Union[FileDensity, Error]]
     ] = create_file_density.sync_detailed(
         client=client,
         material_mass=3.14,
+        material_mass_unit=UnitMass.G,
+        output_unit=UnitDensity.LB_FT3,
         src_format=FileImportFormat.DAE,
         body=bytes("some bytes", "utf-8"),
     )
 
 
 # OR run async
 @pytest.mark.asyncio
@@ -1122,24 +1132,28 @@
 async def test_create_file_density_async():
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[Union[FileDensity, Error]] = await create_file_density.asyncio(
         client=client,
         material_mass=3.14,
+        material_mass_unit=UnitMass.G,
+        output_unit=UnitDensity.LB_FT3,
         src_format=FileImportFormat.DAE,
         body=bytes("some bytes", "utf-8"),
     )
 
     # OR run async with more info
     response: Response[
         Optional[Union[FileDensity, Error]]
     ] = await create_file_density.asyncio_detailed(
         client=client,
         material_mass=3.14,
+        material_mass_unit=UnitMass.G,
+        output_unit=UnitDensity.LB_FT3,
         src_format=FileImportFormat.DAE,
         body=bytes("some bytes", "utf-8"),
     )
 
 
 @pytest.mark.skip
 def test_create_file_execution():
@@ -1200,14 +1214,16 @@
 def test_create_file_mass():
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[Union[FileMass, Error]] = create_file_mass.sync(
         client=client,
         material_density=3.14,
+        material_density_unit=UnitDensity.LB_FT3,
+        output_unit=UnitMass.G,
         src_format=FileImportFormat.DAE,
         body=bytes("some bytes", "utf-8"),
     )
 
     if isinstance(result, Error) or result is None:
         print(result)
         raise Exception("Error in response")
@@ -1217,14 +1233,16 @@
 
     # OR if you need more info (e.g. status_code)
     response: Response[
         Optional[Union[FileMass, Error]]
     ] = create_file_mass.sync_detailed(
         client=client,
         material_density=3.14,
+        material_density_unit=UnitDensity.LB_FT3,
+        output_unit=UnitMass.G,
         src_format=FileImportFormat.DAE,
         body=bytes("some bytes", "utf-8"),
     )
 
 
 # OR run async
 @pytest.mark.asyncio
@@ -1232,36 +1250,41 @@
 async def test_create_file_mass_async():
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[Union[FileMass, Error]] = await create_file_mass.asyncio(
         client=client,
         material_density=3.14,
+        material_density_unit=UnitDensity.LB_FT3,
+        output_unit=UnitMass.G,
         src_format=FileImportFormat.DAE,
         body=bytes("some bytes", "utf-8"),
     )
 
     # OR run async with more info
     response: Response[
         Optional[Union[FileMass, Error]]
     ] = await create_file_mass.asyncio_detailed(
         client=client,
         material_density=3.14,
+        material_density_unit=UnitDensity.LB_FT3,
+        output_unit=UnitMass.G,
         src_format=FileImportFormat.DAE,
         body=bytes("some bytes", "utf-8"),
     )
 
 
 @pytest.mark.skip
 def test_create_file_surface_area():
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[Union[FileSurfaceArea, Error]] = create_file_surface_area.sync(
         client=client,
+        output_unit=UnitArea.CM2,
         src_format=FileImportFormat.DAE,
         body=bytes("some bytes", "utf-8"),
     )
 
     if isinstance(result, Error) or result is None:
         print(result)
         raise Exception("Error in response")
@@ -1270,14 +1293,15 @@
     print(body)
 
     # OR if you need more info (e.g. status_code)
     response: Response[
         Optional[Union[FileSurfaceArea, Error]]
     ] = create_file_surface_area.sync_detailed(
         client=client,
+        output_unit=UnitArea.CM2,
         src_format=FileImportFormat.DAE,
         body=bytes("some bytes", "utf-8"),
     )
 
 
 # OR run async
 @pytest.mark.asyncio
@@ -1286,35 +1310,38 @@
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[
         Union[FileSurfaceArea, Error]
     ] = await create_file_surface_area.asyncio(
         client=client,
+        output_unit=UnitArea.CM2,
         src_format=FileImportFormat.DAE,
         body=bytes("some bytes", "utf-8"),
     )
 
     # OR run async with more info
     response: Response[
         Optional[Union[FileSurfaceArea, Error]]
     ] = await create_file_surface_area.asyncio_detailed(
         client=client,
+        output_unit=UnitArea.CM2,
         src_format=FileImportFormat.DAE,
         body=bytes("some bytes", "utf-8"),
     )
 
 
 @pytest.mark.skip
 def test_create_file_volume():
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[Union[FileVolume, Error]] = create_file_volume.sync(
         client=client,
+        output_unit=UnitVolume.CM3,
         src_format=FileImportFormat.DAE,
         body=bytes("some bytes", "utf-8"),
     )
 
     if isinstance(result, Error) or result is None:
         print(result)
         raise Exception("Error in response")
@@ -1323,37 +1350,40 @@
     print(body)
 
     # OR if you need more info (e.g. status_code)
     response: Response[
         Optional[Union[FileVolume, Error]]
     ] = create_file_volume.sync_detailed(
         client=client,
+        output_unit=UnitVolume.CM3,
         src_format=FileImportFormat.DAE,
         body=bytes("some bytes", "utf-8"),
     )
 
 
 # OR run async
 @pytest.mark.asyncio
 @pytest.mark.skip
 async def test_create_file_volume_async():
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[Union[FileVolume, Error]] = await create_file_volume.asyncio(
         client=client,
+        output_unit=UnitVolume.CM3,
         src_format=FileImportFormat.DAE,
         body=bytes("some bytes", "utf-8"),
     )
 
     # OR run async with more info
     response: Response[
         Optional[Union[FileVolume, Error]]
     ] = await create_file_volume.asyncio_detailed(
         client=client,
+        output_unit=UnitVolume.CM3,
         src_format=FileImportFormat.DAE,
         body=bytes("some bytes", "utf-8"),
     )
 
 
 @pytest.mark.skip
 def test_logout():
@@ -1398,25 +1428,39 @@
 def test_cmd():
     # Create our client.
     client = ClientFromEnv()
 
     cmd.sync(
         client=client,
         body=ModelingCmdReq(
-            cmd=ModelingCmd.START_PATH,
+            cmd=MovePathPen(
+                path=ModelingCmdId("<uuid>"),
+                to=Point3d(
+                    x=3.14,
+                    y=3.14,
+                    z=3.14,
+                ),
+            ),
             cmd_id=ModelingCmdId("<uuid>"),
             file_id="<string>",
         ),
     )
 
     # OR if you need more info (e.g. status_code)
     cmd.sync_detailed(
         client=client,
         body=ModelingCmdReq(
-            cmd=ModelingCmd.START_PATH,
+            cmd=MovePathPen(
+                path=ModelingCmdId("<uuid>"),
+                to=Point3d(
+                    x=3.14,
+                    y=3.14,
+                    z=3.14,
+                ),
+            ),
             cmd_id=ModelingCmdId("<uuid>"),
             file_id="<string>",
         ),
     )
 
 
 # OR run async
@@ -1425,25 +1469,39 @@
 async def test_cmd_async():
     # Create our client.
     client = ClientFromEnv()
 
     await cmd.asyncio(
         client=client,
         body=ModelingCmdReq(
-            cmd=ModelingCmd.START_PATH,
+            cmd=MovePathPen(
+                path=ModelingCmdId("<uuid>"),
+                to=Point3d(
+                    x=3.14,
+                    y=3.14,
+                    z=3.14,
+                ),
+            ),
             cmd_id=ModelingCmdId("<uuid>"),
             file_id="<string>",
         ),
     )
 
     # OR run async with more info
     await cmd.asyncio_detailed(
         client=client,
         body=ModelingCmdReq(
-            cmd=ModelingCmd.START_PATH,
+            cmd=MovePathPen(
+                path=ModelingCmdId("<uuid>"),
+                to=Point3d(
+                    x=3.14,
+                    y=3.14,
+                    z=3.14,
+                ),
+            ),
             cmd_id=ModelingCmdId("<uuid>"),
             file_id="<string>",
         ),
     )
 
 
 @pytest.mark.skip
@@ -1452,15 +1510,22 @@
     client = ClientFromEnv()
 
     result: Optional[Union[ModelingOutcomes, Error]] = cmd_batch.sync(
         client=client,
         body=ModelingCmdReqBatch(
             cmds={
                 "<string>": ModelingCmdReq(
-                    cmd=ModelingCmd.START_PATH,
+                    cmd=MovePathPen(
+                        path=ModelingCmdId("<uuid>"),
+                        to=Point3d(
+                            x=3.14,
+                            y=3.14,
+                            z=3.14,
+                        ),
+                    ),
                     cmd_id=ModelingCmdId("<uuid>"),
                     file_id="<string>",
                 )
             },
             file_id="<string>",
         ),
     )
@@ -1476,15 +1541,22 @@
     response: Response[
         Optional[Union[ModelingOutcomes, Error]]
     ] = cmd_batch.sync_detailed(
         client=client,
         body=ModelingCmdReqBatch(
             cmds={
                 "<string>": ModelingCmdReq(
-                    cmd=ModelingCmd.START_PATH,
+                    cmd=MovePathPen(
+                        path=ModelingCmdId("<uuid>"),
+                        to=Point3d(
+                            x=3.14,
+                            y=3.14,
+                            z=3.14,
+                        ),
+                    ),
                     cmd_id=ModelingCmdId("<uuid>"),
                     file_id="<string>",
                 )
             },
             file_id="<string>",
         ),
     )
@@ -1498,15 +1570,22 @@
     client = ClientFromEnv()
 
     result: Optional[Union[ModelingOutcomes, Error]] = await cmd_batch.asyncio(
         client=client,
         body=ModelingCmdReqBatch(
             cmds={
                 "<string>": ModelingCmdReq(
-                    cmd=ModelingCmd.START_PATH,
+                    cmd=MovePathPen(
+                        path=ModelingCmdId("<uuid>"),
+                        to=Point3d(
+                            x=3.14,
+                            y=3.14,
+                            z=3.14,
+                        ),
+                    ),
                     cmd_id=ModelingCmdId("<uuid>"),
                     file_id="<string>",
                 )
             },
             file_id="<string>",
         ),
     )
@@ -1515,15 +1594,22 @@
     response: Response[
         Optional[Union[ModelingOutcomes, Error]]
     ] = await cmd_batch.asyncio_detailed(
         client=client,
         body=ModelingCmdReqBatch(
             cmds={
                 "<string>": ModelingCmdReq(
-                    cmd=ModelingCmd.START_PATH,
+                    cmd=MovePathPen(
+                        path=ModelingCmdId("<uuid>"),
+                        to=Point3d(
+                            x=3.14,
+                            y=3.14,
+                            z=3.14,
+                        ),
+                    ),
                     cmd_id=ModelingCmdId("<uuid>"),
                     file_id="<string>",
                 )
             },
             file_id="<string>",
         ),
     )
@@ -1662,16 +1748,16 @@
 @pytest.mark.skip
 def test_get_area_unit_conversion():
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[Union[UnitAreaConversion, Error]] = get_area_unit_conversion.sync(
         client=client,
-        input_unit=UnitArea.ACRES,
-        output_unit=UnitArea.ACRES,
+        input_unit=UnitArea.CM2,
+        output_unit=UnitArea.CM2,
         value=3.14,
     )
 
     if isinstance(result, Error) or result is None:
         print(result)
         raise Exception("Error in response")
 
@@ -1679,16 +1765,16 @@
     print(body)
 
     # OR if you need more info (e.g. status_code)
     response: Response[
         Optional[Union[UnitAreaConversion, Error]]
     ] = get_area_unit_conversion.sync_detailed(
         client=client,
-        input_unit=UnitArea.ACRES,
-        output_unit=UnitArea.ACRES,
+        input_unit=UnitArea.CM2,
+        output_unit=UnitArea.CM2,
         value=3.14,
     )
 
 
 # OR run async
 @pytest.mark.asyncio
 @pytest.mark.skip
@@ -1696,26 +1782,26 @@
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[
         Union[UnitAreaConversion, Error]
     ] = await get_area_unit_conversion.asyncio(
         client=client,
-        input_unit=UnitArea.ACRES,
-        output_unit=UnitArea.ACRES,
+        input_unit=UnitArea.CM2,
+        output_unit=UnitArea.CM2,
         value=3.14,
     )
 
     # OR run async with more info
     response: Response[
         Optional[Union[UnitAreaConversion, Error]]
     ] = await get_area_unit_conversion.asyncio_detailed(
         client=client,
-        input_unit=UnitArea.ACRES,
-        output_unit=UnitArea.ACRES,
+        input_unit=UnitArea.CM2,
+        output_unit=UnitArea.CM2,
         value=3.14,
     )
 
 
 @pytest.mark.skip
 def test_get_current_unit_conversion():
     # Create our client.
@@ -1957,16 +2043,16 @@
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[
         Union[UnitLengthConversion, Error]
     ] = get_length_unit_conversion.sync(
         client=client,
-        input_unit=UnitLength.CENTIMETRES,
-        output_unit=UnitLength.CENTIMETRES,
+        input_unit=UnitLength.CM,
+        output_unit=UnitLength.CM,
         value=3.14,
     )
 
     if isinstance(result, Error) or result is None:
         print(result)
         raise Exception("Error in response")
 
@@ -1974,16 +2060,16 @@
     print(body)
 
     # OR if you need more info (e.g. status_code)
     response: Response[
         Optional[Union[UnitLengthConversion, Error]]
     ] = get_length_unit_conversion.sync_detailed(
         client=client,
-        input_unit=UnitLength.CENTIMETRES,
-        output_unit=UnitLength.CENTIMETRES,
+        input_unit=UnitLength.CM,
+        output_unit=UnitLength.CM,
         value=3.14,
     )
 
 
 # OR run async
 @pytest.mark.asyncio
 @pytest.mark.skip
@@ -1991,39 +2077,39 @@
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[
         Union[UnitLengthConversion, Error]
     ] = await get_length_unit_conversion.asyncio(
         client=client,
-        input_unit=UnitLength.CENTIMETRES,
-        output_unit=UnitLength.CENTIMETRES,
+        input_unit=UnitLength.CM,
+        output_unit=UnitLength.CM,
         value=3.14,
     )
 
     # OR run async with more info
     response: Response[
         Optional[Union[UnitLengthConversion, Error]]
     ] = await get_length_unit_conversion.asyncio_detailed(
         client=client,
-        input_unit=UnitLength.CENTIMETRES,
-        output_unit=UnitLength.CENTIMETRES,
+        input_unit=UnitLength.CM,
+        output_unit=UnitLength.CM,
         value=3.14,
     )
 
 
 @pytest.mark.skip
 def test_get_mass_unit_conversion():
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[Union[UnitMassConversion, Error]] = get_mass_unit_conversion.sync(
         client=client,
-        input_unit=UnitMass.CARATS,
-        output_unit=UnitMass.CARATS,
+        input_unit=UnitMass.G,
+        output_unit=UnitMass.G,
         value=3.14,
     )
 
     if isinstance(result, Error) or result is None:
         print(result)
         raise Exception("Error in response")
 
@@ -2031,16 +2117,16 @@
     print(body)
 
     # OR if you need more info (e.g. status_code)
     response: Response[
         Optional[Union[UnitMassConversion, Error]]
     ] = get_mass_unit_conversion.sync_detailed(
         client=client,
-        input_unit=UnitMass.CARATS,
-        output_unit=UnitMass.CARATS,
+        input_unit=UnitMass.G,
+        output_unit=UnitMass.G,
         value=3.14,
     )
 
 
 # OR run async
 @pytest.mark.asyncio
 @pytest.mark.skip
@@ -2048,26 +2134,26 @@
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[
         Union[UnitMassConversion, Error]
     ] = await get_mass_unit_conversion.asyncio(
         client=client,
-        input_unit=UnitMass.CARATS,
-        output_unit=UnitMass.CARATS,
+        input_unit=UnitMass.G,
+        output_unit=UnitMass.G,
         value=3.14,
     )
 
     # OR run async with more info
     response: Response[
         Optional[Union[UnitMassConversion, Error]]
     ] = await get_mass_unit_conversion.asyncio_detailed(
         client=client,
-        input_unit=UnitMass.CARATS,
-        output_unit=UnitMass.CARATS,
+        input_unit=UnitMass.G,
+        output_unit=UnitMass.G,
         value=3.14,
     )
 
 
 @pytest.mark.skip
 def test_get_power_unit_conversion():
     # Create our client.
@@ -2309,16 +2395,16 @@
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[
         Union[UnitVolumeConversion, Error]
     ] = get_volume_unit_conversion.sync(
         client=client,
-        input_unit=UnitVolume.CUBIC_CENTIMETRES,
-        output_unit=UnitVolume.CUBIC_CENTIMETRES,
+        input_unit=UnitVolume.CM3,
+        output_unit=UnitVolume.CM3,
         value=3.14,
     )
 
     if isinstance(result, Error) or result is None:
         print(result)
         raise Exception("Error in response")
 
@@ -2326,16 +2412,16 @@
     print(body)
 
     # OR if you need more info (e.g. status_code)
     response: Response[
         Optional[Union[UnitVolumeConversion, Error]]
     ] = get_volume_unit_conversion.sync_detailed(
         client=client,
-        input_unit=UnitVolume.CUBIC_CENTIMETRES,
-        output_unit=UnitVolume.CUBIC_CENTIMETRES,
+        input_unit=UnitVolume.CM3,
+        output_unit=UnitVolume.CM3,
         value=3.14,
     )
 
 
 # OR run async
 @pytest.mark.asyncio
 @pytest.mark.skip
@@ -2343,26 +2429,26 @@
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[
         Union[UnitVolumeConversion, Error]
     ] = await get_volume_unit_conversion.asyncio(
         client=client,
-        input_unit=UnitVolume.CUBIC_CENTIMETRES,
-        output_unit=UnitVolume.CUBIC_CENTIMETRES,
+        input_unit=UnitVolume.CM3,
+        output_unit=UnitVolume.CM3,
         value=3.14,
     )
 
     # OR run async with more info
     response: Response[
         Optional[Union[UnitVolumeConversion, Error]]
     ] = await get_volume_unit_conversion.asyncio_detailed(
         client=client,
-        input_unit=UnitVolume.CUBIC_CENTIMETRES,
-        output_unit=UnitVolume.CUBIC_CENTIMETRES,
+        input_unit=UnitVolume.CM3,
+        output_unit=UnitVolume.CM3,
         value=3.14,
     )
 
 
 @pytest.mark.skip
 def test_delete_user_self():
     # Create our client.
@@ -3727,64 +3813,76 @@
 
 
 @pytest.mark.skip
 def test_create_executor_term():
     # Create our client.
     client = ClientFromEnv()
 
-    create_executor_term.sync(
+    # Connect to the websocket.
+    websocket = create_executor_term.sync(
         client=client,
     )
 
-    # OR if you need more info (e.g. status_code)
-    create_executor_term.sync_detailed(
-        client=client,
-    )
+    # Send a message.
+    websocket.send("{}")
+
+    # Get the messages.
+    for message in websocket:
+        print(message)
 
 
 # OR run async
 @pytest.mark.asyncio
 @pytest.mark.skip
 async def test_create_executor_term_async():
     # Create our client.
     client = ClientFromEnv()
 
-    await create_executor_term.asyncio(
+    # Connect to the websocket.
+    websocket = await create_executor_term.asyncio(
         client=client,
     )
 
-    # OR run async with more info
-    await create_executor_term.asyncio_detailed(
-        client=client,
-    )
+    # Send a message.
+    await websocket.send("{}")
+
+    # Get the messages.
+    async for message in websocket:
+        print(message)
 
 
 @pytest.mark.skip
 def test_modeling_commands_ws():
     # Create our client.
     client = ClientFromEnv()
 
-    modeling_commands_ws.sync(
+    # Connect to the websocket.
+    websocket = modeling_commands_ws.sync(
         client=client,
     )
 
-    # OR if you need more info (e.g. status_code)
-    modeling_commands_ws.sync_detailed(
-        client=client,
-    )
+    # Send a message.
+    websocket.send("{}")
+
+    # Get the messages.
+    for message in websocket:
+        print(message)
 
 
 # OR run async
 @pytest.mark.asyncio
 @pytest.mark.skip
 async def test_modeling_commands_ws_async():
     # Create our client.
     client = ClientFromEnv()
 
-    await modeling_commands_ws.asyncio(
+    # Connect to the websocket.
+    websocket = await modeling_commands_ws.asyncio(
         client=client,
     )
 
-    # OR run async with more info
-    await modeling_commands_ws.asyncio_detailed(
-        client=client,
-    )
+    # Send a message.
+    await websocket.send("{}")
+
+    # Get the messages.
+    async for message in websocket:
+        print(message)
```

### Comparing `kittycad-0.4.4/kittycad/models/__init__.py` & `kittycad-0.4.5/kittycad/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,15 @@
 from .system_info_isolation_enum import SystemInfoIsolationEnum
 from .unit_angle import UnitAngle
 from .unit_angle_conversion import UnitAngleConversion
 from .unit_area import UnitArea
 from .unit_area_conversion import UnitAreaConversion
 from .unit_current import UnitCurrent
 from .unit_current_conversion import UnitCurrentConversion
+from .unit_density import UnitDensity
 from .unit_energy import UnitEnergy
 from .unit_energy_conversion import UnitEnergyConversion
 from .unit_force import UnitForce
 from .unit_force_conversion import UnitForceConversion
 from .unit_frequency import UnitFrequency
 from .unit_frequency_conversion import UnitFrequencyConversion
 from .unit_length import UnitLength
```

### Comparing `kittycad-0.4.4/kittycad/models/ai_plugin_api.py` & `kittycad-0.4.5/kittycad/models/ai_plugin_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.ai_plugin_api_type import AiPluginApiType
 from ..types import UNSET, Unset
 
-S = TypeVar("S", bound="AiPluginApi")
+SB = TypeVar("SB", bound="AiPluginApi")
 
 
 @attr.s(auto_attribs=True)
 class AiPluginApi:
     """AI plugin api information."""  # noqa: E501
 
     is_user_authenticated: Union[Unset, bool] = False
@@ -33,15 +33,15 @@
             field_dict["type"] = type
         if url is not UNSET:
             field_dict["url"] = url
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[S], src_dict: Dict[str, Any]) -> S:
+    def from_dict(cls: Type[SB], src_dict: Dict[str, Any]) -> SB:
         d = src_dict.copy()
         is_user_authenticated = d.pop("is_user_authenticated", UNSET)
 
         _type = d.pop("type", UNSET)
         type: Union[Unset, AiPluginApiType]
         if isinstance(_type, Unset):
             type = UNSET
```

### Comparing `kittycad-0.4.4/kittycad/models/ai_plugin_auth.py` & `kittycad-0.4.5/kittycad/models/ai_plugin_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import attr
 
 from ..models.ai_plugin_auth_type import AiPluginAuthType
 from ..models.ai_plugin_http_auth_type import AiPluginHttpAuthType
 from ..types import UNSET, Unset
 
-B = TypeVar("B", bound="AiPluginAuth")
+NP = TypeVar("NP", bound="AiPluginAuth")
 
 
 @attr.s(auto_attribs=True)
 class AiPluginAuth:
     """AI plugin auth information."""  # noqa: E501
 
     authorization_type: Union[Unset, AiPluginHttpAuthType] = UNSET
@@ -31,15 +31,15 @@
             field_dict["authorization_type"] = authorization_type
         if type is not UNSET:
             field_dict["type"] = type
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[B], src_dict: Dict[str, Any]) -> B:
+    def from_dict(cls: Type[NP], src_dict: Dict[str, Any]) -> NP:
         d = src_dict.copy()
         _authorization_type = d.pop("authorization_type", UNSET)
         authorization_type: Union[Unset, AiPluginHttpAuthType]
         if isinstance(_authorization_type, Unset):
             authorization_type = UNSET
         else:
             authorization_type = _authorization_type  # type: ignore[arg-type]
```

### Comparing `kittycad-0.4.4/kittycad/models/ai_plugin_manifest.py` & `kittycad-0.4.5/kittycad/models/ai_plugin_manifest.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 
 import attr
 
 from ..models.ai_plugin_api import AiPluginApi
 from ..models.ai_plugin_auth import AiPluginAuth
 from ..types import UNSET, Unset
 
-N = TypeVar("N", bound="AiPluginManifest")
+SA = TypeVar("SA", bound="AiPluginManifest")
 
 
 @attr.s(auto_attribs=True)
 class AiPluginManifest:
     """AI plugin manifest.
 
-    This is used for OpenAI's ChatGPT plugins. You can read more about them [here](https://platform.openai.com/docs/plugins/getting-started/plugin-manifest)."""  # noqa: E501
+    This is used for OpenAI's ChatGPT plugins. You can read more about them [here](https://platform.openai.com/docs/plugins/getting-started/plugin-manifest).
+    """  # noqa: E501
 
     api: Union[Unset, AiPluginApi] = UNSET
     auth: Union[Unset, AiPluginAuth] = UNSET
     contact_email: Union[Unset, str] = UNSET
     description_for_human: Union[Unset, str] = UNSET
     description_for_model: Union[Unset, str] = UNSET
     legal_info_url: Union[Unset, str] = UNSET
@@ -65,29 +66,29 @@
             field_dict["name_for_model"] = name_for_model
         if schema_version is not UNSET:
             field_dict["schema_version"] = schema_version
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
+    def from_dict(cls: Type[SA], src_dict: Dict[str, Any]) -> SA:
         d = src_dict.copy()
         _api = d.pop("api", UNSET)
         api: Union[Unset, AiPluginApi]
         if isinstance(_api, Unset):
             api = UNSET
         else:
-            api = AiPluginApi(_api)
+            api = _api  # type: ignore[arg-type]
 
         _auth = d.pop("auth", UNSET)
         auth: Union[Unset, AiPluginAuth]
         if isinstance(_auth, Unset):
             auth = UNSET
         else:
-            auth = AiPluginAuth(_auth)
+            auth = _auth  # type: ignore[arg-type]
 
         contact_email = d.pop("contact_email", UNSET)
 
         description_for_human = d.pop("description_for_human", UNSET)
 
         description_for_model = d.pop("description_for_model", UNSET)
```

### Comparing `kittycad-0.4.4/kittycad/models/api_call_query_group.py` & `kittycad-0.4.5/kittycad/models/api_call_query_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-P = TypeVar("P", bound="ApiCallQueryGroup")
+GO = TypeVar("GO", bound="ApiCallQueryGroup")
 
 
 @attr.s(auto_attribs=True)
 class ApiCallQueryGroup:
     """A response for a query on the API call table that is grouped by something."""  # noqa: E501
 
     count: Union[Unset, int] = UNSET
@@ -27,15 +27,15 @@
             field_dict["count"] = count
         if query is not UNSET:
             field_dict["query"] = query
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[P], src_dict: Dict[str, Any]) -> P:
+    def from_dict(cls: Type[GO], src_dict: Dict[str, Any]) -> GO:
         d = src_dict.copy()
         count = d.pop("count", UNSET)
 
         query = d.pop("query", UNSET)
 
         api_call_query_group = cls(
             count=count,
```

### Comparing `kittycad-0.4.4/kittycad/models/api_call_query_group_by.py` & `kittycad-0.4.5/kittycad/models/api_call_query_group_by.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.4/kittycad/models/api_call_status.py` & `kittycad-0.4.5/kittycad/models/api_call_status.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.4/kittycad/models/api_call_with_price.py` & `kittycad-0.4.5/kittycad/models/api_call_with_price.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import attr
 from dateutil.parser import isoparse
 
 from ..models.method import Method
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-S = TypeVar("S", bound="ApiCallWithPrice")
+PI = TypeVar("PI", bound="ApiCallWithPrice")
 
 
 @attr.s(auto_attribs=True)
 class ApiCallWithPrice:
     """An API call with the price.
 
     This is a join of the `ApiCall` and `ApiCallPrice` tables."""  # noqa: E501
@@ -122,15 +122,15 @@
             field_dict["user_agent"] = user_agent
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[S], src_dict: Dict[str, Any]) -> S:
+    def from_dict(cls: Type[PI], src_dict: Dict[str, Any]) -> PI:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -149,15 +149,15 @@
         endpoint = d.pop("endpoint", UNSET)
 
         _id = d.pop("id", UNSET)
         id: Union[Unset, Uuid]
         if isinstance(_id, Unset):
             id = UNSET
         else:
-            id = Uuid(_id)
+            id = _id  # type: ignore[arg-type]
 
         ip_address = d.pop("ip_address", UNSET)
 
         litterbox = d.pop("litterbox", UNSET)
 
         _method = d.pop("method", UNSET)
         method: Union[Unset, Method]
@@ -190,15 +190,15 @@
         stripe_invoice_item_id = d.pop("stripe_invoice_item_id", UNSET)
 
         _token = d.pop("token", UNSET)
         token: Union[Unset, Uuid]
         if isinstance(_token, Unset):
             token = UNSET
         else:
-            token = Uuid(_token)
+            token = _token  # type: ignore[arg-type]
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
```

### Comparing `kittycad-0.4.4/kittycad/models/api_call_with_price_results_page.py` & `kittycad-0.4.5/kittycad/models/api_call_with_price_results_page.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
-A = TypeVar("A", bound="ApiCallWithPriceResultsPage")
+UZ = TypeVar("UZ", bound="ApiCallWithPriceResultsPage")
 
 
 @attr.s(auto_attribs=True)
 class ApiCallWithPriceResultsPage:
     """A single page of results"""  # noqa: E501
 
     from ..models.api_call_with_price import ApiCallWithPrice
@@ -33,15 +33,15 @@
             field_dict["items"] = items
         if next_page is not UNSET:
             field_dict["next_page"] = next_page
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[A], src_dict: Dict[str, Any]) -> A:
+    def from_dict(cls: Type[UZ], src_dict: Dict[str, Any]) -> UZ:
         d = src_dict.copy()
         from ..models.api_call_with_price import ApiCallWithPrice
 
         items = cast(List[ApiCallWithPrice], d.pop("items", UNSET))
 
         next_page = d.pop("next_page", UNSET)
```

### Comparing `kittycad-0.4.4/kittycad/models/api_token.py` & `kittycad-0.4.5/kittycad/models/api_token.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-G = TypeVar("G", bound="ApiToken")
+FB = TypeVar("FB", bound="ApiToken")
 
 
 @attr.s(auto_attribs=True)
 class ApiToken:
     """An API token.
 
     These are used to authenticate users with Bearer authentication."""  # noqa: E501
@@ -52,15 +52,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[G], src_dict: Dict[str, Any]) -> G:
+    def from_dict(cls: Type[FB], src_dict: Dict[str, Any]) -> FB:
         d = src_dict.copy()
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
@@ -70,15 +70,15 @@
         is_valid = d.pop("is_valid", UNSET)
 
         _token = d.pop("token", UNSET)
         token: Union[Unset, Uuid]
         if isinstance(_token, Unset):
             token = UNSET
         else:
-            token = Uuid(_token)
+            token = _token  # type: ignore[arg-type]
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
```

### Comparing `kittycad-0.4.4/kittycad/models/api_token_results_page.py` & `kittycad-0.4.5/kittycad/models/api_token_results_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
-P = TypeVar("P", bound="ApiTokenResultsPage")
+QP = TypeVar("QP", bound="ApiTokenResultsPage")
 
 
 @attr.s(auto_attribs=True)
 class ApiTokenResultsPage:
     """A single page of results"""  # noqa: E501
 
     from ..models.api_token import ApiToken
@@ -33,15 +33,15 @@
             field_dict["items"] = items
         if next_page is not UNSET:
             field_dict["next_page"] = next_page
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[P], src_dict: Dict[str, Any]) -> P:
+    def from_dict(cls: Type[QP], src_dict: Dict[str, Any]) -> QP:
         d = src_dict.copy()
         from ..models.api_token import ApiToken
 
         items = cast(List[ApiToken], d.pop("items", UNSET))
 
         next_page = d.pop("next_page", UNSET)
```

### Comparing `kittycad-0.4.4/kittycad/models/app_client_info.py` & `kittycad-0.4.5/kittycad/models/app_client_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-U = TypeVar("U", bound="AppClientInfo")
+KC = TypeVar("KC", bound="AppClientInfo")
 
 
 @attr.s(auto_attribs=True)
 class AppClientInfo:
     """Information about a third party app client."""  # noqa: E501
 
     url: Union[Unset, str] = UNSET
@@ -23,15 +23,15 @@
         field_dict.update({})
         if url is not UNSET:
             field_dict["url"] = url
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[U], src_dict: Dict[str, Any]) -> U:
+    def from_dict(cls: Type[KC], src_dict: Dict[str, Any]) -> KC:
         d = src_dict.copy()
         url = d.pop("url", UNSET)
 
         app_client_info = cls(
             url=url,
         )
```

### Comparing `kittycad-0.4.4/kittycad/models/async_api_call.py` & `kittycad-0.4.5/kittycad/models/async_api_call.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.async_api_call_type import AsyncApiCallType
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-Z = TypeVar("Z", bound="AsyncApiCall")
+HX = TypeVar("HX", bound="AsyncApiCall")
 
 
 @attr.s(auto_attribs=True)
 class AsyncApiCall:
     """An async API call."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
@@ -82,15 +82,15 @@
             field_dict["user_id"] = user_id
         if worker is not UNSET:
             field_dict["worker"] = worker
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[Z], src_dict: Dict[str, Any]) -> Z:
+    def from_dict(cls: Type[HX], src_dict: Dict[str, Any]) -> HX:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -105,15 +105,15 @@
         error = d.pop("error", UNSET)
 
         _id = d.pop("id", UNSET)
         id: Union[Unset, Uuid]
         if isinstance(_id, Unset):
             id = UNSET
         else:
-            id = Uuid(_id)
+            id = _id  # type: ignore[arg-type]
 
         input = d.pop("input", UNSET)
         output = d.pop("output", UNSET)
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
```

### Comparing `kittycad-0.4.4/kittycad/models/async_api_call_output.py` & `kittycad-0.4.5/kittycad/models/async_api_call_output.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.file_export_format import FileExportFormat
 from ..models.file_import_format import FileImportFormat
 from ..models.input_format import InputFormat
 from ..models.output_format import OutputFormat
+from ..models.point3d import Point3d
+from ..models.unit_area import UnitArea
+from ..models.unit_density import UnitDensity
+from ..models.unit_length import UnitLength
+from ..models.unit_mass import UnitMass
+from ..models.unit_volume import UnitVolume
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-F = TypeVar("F", bound="FileConversion")
+LB = TypeVar("LB", bound="FileConversion")
 
 
 @attr.s(auto_attribs=True)
 class FileConversion:
     """A file conversion."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
@@ -100,15 +106,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
+    def from_dict(cls: Type[LB], src_dict: Dict[str, Any]) -> LB:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -123,15 +129,15 @@
         error = d.pop("error", UNSET)
 
         _id = d.pop("id", UNSET)
         id: Union[Unset, Uuid]
         if isinstance(_id, Unset):
             id = UNSET
         else:
-            id = Uuid(_id)
+            id = _id  # type: ignore[arg-type]
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
         output_format: Union[Unset, FileExportFormat]
         if isinstance(_output_format, Unset):
             output_format = UNSET
@@ -139,30 +145,30 @@
             output_format = _output_format  # type: ignore[arg-type]
 
         _output_format_options = d.pop("output_format_options", UNSET)
         output_format_options: Union[Unset, OutputFormat]
         if isinstance(_output_format_options, Unset):
             output_format_options = UNSET
         else:
-            output_format_options = OutputFormat(_output_format_options)
+            output_format_options = _output_format_options  # type: ignore[arg-type]
 
         outputs = d.pop("outputs", UNSET)
         _src_format = d.pop("src_format", UNSET)
         src_format: Union[Unset, FileImportFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
             src_format = _src_format  # type: ignore[arg-type]
 
         _src_format_options = d.pop("src_format_options", UNSET)
         src_format_options: Union[Unset, InputFormat]
         if isinstance(_src_format_options, Unset):
             src_format_options = UNSET
         else:
-            src_format_options = InputFormat(_src_format_options)
+            src_format_options = _src_format_options  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -219,47 +225,51 @@
     def __delitem__(self, key: str) -> None:
         del self.additional_properties[key]
 
     def __contains__(self, key: str) -> bool:
         return key in self.additional_properties
 
 
-B = TypeVar("B", bound="FileCenterOfMass")
+NE = TypeVar("NE", bound="FileCenterOfMass")
 
 
 @attr.s(auto_attribs=True)
 class FileCenterOfMass:
     """File center of mass."""  # noqa: E501
 
-    center_of_mass: Union[Unset, List[float]] = UNSET
+    center_of_mass: Union[Unset, Point3d] = UNSET
+    centers_of_mass: Union[Unset, Any] = UNSET
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
+    output_unit: Union[Unset, UnitLength] = UNSET
     src_format: Union[Unset, FileImportFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     type: Union[Unset, str] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        center_of_mass: Union[Unset, List[float]] = UNSET
         if not isinstance(self.center_of_mass, Unset):
             center_of_mass = self.center_of_mass
+        centers_of_mass = self.centers_of_mass
         completed_at: Union[Unset, str] = UNSET
         if not isinstance(self.completed_at, Unset):
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
+        if not isinstance(self.output_unit, Unset):
+            output_unit = self.output_unit
         if not isinstance(self.src_format, Unset):
             src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
         if not isinstance(self.status, Unset):
             status = self.status
@@ -270,22 +280,26 @@
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if center_of_mass is not UNSET:
             field_dict["center_of_mass"] = center_of_mass
+        if centers_of_mass is not UNSET:
+            field_dict["centers_of_mass"] = centers_of_mass
         if completed_at is not UNSET:
             field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
             field_dict["created_at"] = created_at
         if error is not UNSET:
             field_dict["error"] = error
         if id is not UNSET:
             field_dict["id"] = id
+        if output_unit is not UNSET:
+            field_dict["output_unit"] = output_unit
         if src_format is not UNSET:
             field_dict["src_format"] = src_format
         if started_at is not UNSET:
             field_dict["started_at"] = started_at
         if status is not UNSET:
             field_dict["status"] = status
         if type is not UNSET:
@@ -294,18 +308,24 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[B], src_dict: Dict[str, Any]) -> B:
+    def from_dict(cls: Type[NE], src_dict: Dict[str, Any]) -> NE:
         d = src_dict.copy()
-        center_of_mass = cast(List[float], d.pop("center_of_mass", UNSET))
+        _center_of_mass = d.pop("center_of_mass", UNSET)
+        center_of_mass: Union[Unset, Point3d]
+        if isinstance(_center_of_mass, Unset):
+            center_of_mass = UNSET
+        else:
+            center_of_mass = _center_of_mass  # type: ignore[arg-type]
 
+        centers_of_mass = d.pop("centers_of_mass", UNSET)
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
 
@@ -319,15 +339,22 @@
         error = d.pop("error", UNSET)
 
         _id = d.pop("id", UNSET)
         id: Union[Unset, Uuid]
         if isinstance(_id, Unset):
             id = UNSET
         else:
-            id = Uuid(_id)
+            id = _id  # type: ignore[arg-type]
+
+        _output_unit = d.pop("output_unit", UNSET)
+        output_unit: Union[Unset, UnitLength]
+        if isinstance(_output_unit, Unset):
+            output_unit = UNSET
+        else:
+            output_unit = _output_unit  # type: ignore[arg-type]
 
         _src_format = d.pop("src_format", UNSET)
         src_format: Union[Unset, FileImportFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
             src_format = _src_format  # type: ignore[arg-type]
@@ -355,18 +382,20 @@
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
         file_center_of_mass = cls(
             center_of_mass=center_of_mass,
+            centers_of_mass=centers_of_mass,
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
+            output_unit=output_unit,
             src_format=src_format,
             started_at=started_at,
             status=status,
             type=type,
             updated_at=updated_at,
             user_id=user_id,
         )
@@ -387,27 +416,30 @@
     def __delitem__(self, key: str) -> None:
         del self.additional_properties[key]
 
     def __contains__(self, key: str) -> bool:
         return key in self.additional_properties
 
 
-Q = TypeVar("Q", bound="FileMass")
+TL = TypeVar("TL", bound="FileMass")
 
 
 @attr.s(auto_attribs=True)
 class FileMass:
     """A file mass."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     mass: Union[Unset, float] = UNSET
+    masses: Union[Unset, Any] = UNSET
     material_density: Union[Unset, float] = UNSET
+    material_density_unit: Union[Unset, UnitDensity] = UNSET
+    output_unit: Union[Unset, UnitMass] = UNSET
     src_format: Union[Unset, FileImportFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     type: Union[Unset, str] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
@@ -419,15 +451,20 @@
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         mass = self.mass
+        masses = self.masses
         material_density = self.material_density
+        if not isinstance(self.material_density_unit, Unset):
+            material_density_unit = self.material_density_unit
+        if not isinstance(self.output_unit, Unset):
+            output_unit = self.output_unit
         if not isinstance(self.src_format, Unset):
             src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
         if not isinstance(self.status, Unset):
             status = self.status
@@ -446,16 +483,22 @@
             field_dict["created_at"] = created_at
         if error is not UNSET:
             field_dict["error"] = error
         if id is not UNSET:
             field_dict["id"] = id
         if mass is not UNSET:
             field_dict["mass"] = mass
+        if masses is not UNSET:
+            field_dict["masses"] = masses
         if material_density is not UNSET:
             field_dict["material_density"] = material_density
+        if material_density_unit is not UNSET:
+            field_dict["material_density_unit"] = material_density_unit
+        if output_unit is not UNSET:
+            field_dict["output_unit"] = output_unit
         if src_format is not UNSET:
             field_dict["src_format"] = src_format
         if started_at is not UNSET:
             field_dict["started_at"] = started_at
         if status is not UNSET:
             field_dict["status"] = status
         if type is not UNSET:
@@ -464,15 +507,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[Q], src_dict: Dict[str, Any]) -> Q:
+    def from_dict(cls: Type[TL], src_dict: Dict[str, Any]) -> TL:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -487,20 +530,35 @@
         error = d.pop("error", UNSET)
 
         _id = d.pop("id", UNSET)
         id: Union[Unset, Uuid]
         if isinstance(_id, Unset):
             id = UNSET
         else:
-            id = Uuid(_id)
+            id = _id  # type: ignore[arg-type]
 
         mass = d.pop("mass", UNSET)
 
+        masses = d.pop("masses", UNSET)
         material_density = d.pop("material_density", UNSET)
 
+        _material_density_unit = d.pop("material_density_unit", UNSET)
+        material_density_unit: Union[Unset, UnitDensity]
+        if isinstance(_material_density_unit, Unset):
+            material_density_unit = UNSET
+        else:
+            material_density_unit = _material_density_unit  # type: ignore[arg-type]
+
+        _output_unit = d.pop("output_unit", UNSET)
+        output_unit: Union[Unset, UnitMass]
+        if isinstance(_output_unit, Unset):
+            output_unit = UNSET
+        else:
+            output_unit = _output_unit  # type: ignore[arg-type]
+
         _src_format = d.pop("src_format", UNSET)
         src_format: Union[Unset, FileImportFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
             src_format = _src_format  # type: ignore[arg-type]
 
@@ -531,15 +589,18 @@
 
         file_mass = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             mass=mass,
+            masses=masses,
             material_density=material_density,
+            material_density_unit=material_density_unit,
+            output_unit=output_unit,
             src_format=src_format,
             started_at=started_at,
             status=status,
             type=type,
             updated_at=updated_at,
             user_id=user_id,
         )
@@ -560,88 +621,97 @@
     def __delitem__(self, key: str) -> None:
         del self.additional_properties[key]
 
     def __contains__(self, key: str) -> bool:
         return key in self.additional_properties
 
 
-P = TypeVar("P", bound="FileVolume")
+MN = TypeVar("MN", bound="FileVolume")
 
 
 @attr.s(auto_attribs=True)
 class FileVolume:
     """A file volume."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
+    output_unit: Union[Unset, UnitVolume] = UNSET
     src_format: Union[Unset, FileImportFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     type: Union[Unset, str] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
     volume: Union[Unset, float] = UNSET
+    volumes: Union[Unset, Any] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         completed_at: Union[Unset, str] = UNSET
         if not isinstance(self.completed_at, Unset):
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
+        if not isinstance(self.output_unit, Unset):
+            output_unit = self.output_unit
         if not isinstance(self.src_format, Unset):
             src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
         if not isinstance(self.status, Unset):
             status = self.status
         type = self.type
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
         volume = self.volume
+        volumes = self.volumes
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
             field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
             field_dict["created_at"] = created_at
         if error is not UNSET:
             field_dict["error"] = error
         if id is not UNSET:
             field_dict["id"] = id
+        if output_unit is not UNSET:
+            field_dict["output_unit"] = output_unit
         if src_format is not UNSET:
             field_dict["src_format"] = src_format
         if started_at is not UNSET:
             field_dict["started_at"] = started_at
         if status is not UNSET:
             field_dict["status"] = status
         if type is not UNSET:
             field_dict["type"] = type
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
         if volume is not UNSET:
             field_dict["volume"] = volume
+        if volumes is not UNSET:
+            field_dict["volumes"] = volumes
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[P], src_dict: Dict[str, Any]) -> P:
+    def from_dict(cls: Type[MN], src_dict: Dict[str, Any]) -> MN:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -656,15 +726,22 @@
         error = d.pop("error", UNSET)
 
         _id = d.pop("id", UNSET)
         id: Union[Unset, Uuid]
         if isinstance(_id, Unset):
             id = UNSET
         else:
-            id = Uuid(_id)
+            id = _id  # type: ignore[arg-type]
+
+        _output_unit = d.pop("output_unit", UNSET)
+        output_unit: Union[Unset, UnitVolume]
+        if isinstance(_output_unit, Unset):
+            output_unit = UNSET
+        else:
+            output_unit = _output_unit  # type: ignore[arg-type]
 
         _src_format = d.pop("src_format", UNSET)
         src_format: Union[Unset, FileImportFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
             src_format = _src_format  # type: ignore[arg-type]
@@ -692,26 +769,30 @@
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
         volume = d.pop("volume", UNSET)
 
+        volumes = d.pop("volumes", UNSET)
+
         file_volume = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
+            output_unit=output_unit,
             src_format=src_format,
             started_at=started_at,
             status=status,
             type=type,
             updated_at=updated_at,
             user_id=user_id,
             volume=volume,
+            volumes=volumes,
         )
 
         file_volume.additional_properties = d
         return file_volume
 
     @property
     def additional_keys(self) -> List[str]:
@@ -726,27 +807,30 @@
     def __delitem__(self, key: str) -> None:
         del self.additional_properties[key]
 
     def __contains__(self, key: str) -> bool:
         return key in self.additional_properties
 
 
-K = TypeVar("K", bound="FileDensity")
+JV = TypeVar("JV", bound="FileDensity")
 
 
 @attr.s(auto_attribs=True)
 class FileDensity:
     """A file density."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
+    densities: Union[Unset, Any] = UNSET
     density: Union[Unset, float] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     material_mass: Union[Unset, float] = UNSET
+    material_mass_unit: Union[Unset, UnitMass] = UNSET
+    output_unit: Union[Unset, UnitDensity] = UNSET
     src_format: Union[Unset, FileImportFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     type: Union[Unset, str] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
@@ -755,18 +839,23 @@
     def to_dict(self) -> Dict[str, Any]:
         completed_at: Union[Unset, str] = UNSET
         if not isinstance(self.completed_at, Unset):
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
+        densities = self.densities
         density = self.density
         error = self.error
         id = self.id
         material_mass = self.material_mass
+        if not isinstance(self.material_mass_unit, Unset):
+            material_mass_unit = self.material_mass_unit
+        if not isinstance(self.output_unit, Unset):
+            output_unit = self.output_unit
         if not isinstance(self.src_format, Unset):
             src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
         if not isinstance(self.status, Unset):
             status = self.status
@@ -779,22 +868,28 @@
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
             field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
             field_dict["created_at"] = created_at
+        if densities is not UNSET:
+            field_dict["densities"] = densities
         if density is not UNSET:
             field_dict["density"] = density
         if error is not UNSET:
             field_dict["error"] = error
         if id is not UNSET:
             field_dict["id"] = id
         if material_mass is not UNSET:
             field_dict["material_mass"] = material_mass
+        if material_mass_unit is not UNSET:
+            field_dict["material_mass_unit"] = material_mass_unit
+        if output_unit is not UNSET:
+            field_dict["output_unit"] = output_unit
         if src_format is not UNSET:
             field_dict["src_format"] = src_format
         if started_at is not UNSET:
             field_dict["started_at"] = started_at
         if status is not UNSET:
             field_dict["status"] = status
         if type is not UNSET:
@@ -803,15 +898,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[K], src_dict: Dict[str, Any]) -> K:
+    def from_dict(cls: Type[JV], src_dict: Dict[str, Any]) -> JV:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -819,27 +914,42 @@
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
+        densities = d.pop("densities", UNSET)
         density = d.pop("density", UNSET)
 
         error = d.pop("error", UNSET)
 
         _id = d.pop("id", UNSET)
         id: Union[Unset, Uuid]
         if isinstance(_id, Unset):
             id = UNSET
         else:
-            id = Uuid(_id)
+            id = _id  # type: ignore[arg-type]
 
         material_mass = d.pop("material_mass", UNSET)
 
+        _material_mass_unit = d.pop("material_mass_unit", UNSET)
+        material_mass_unit: Union[Unset, UnitMass]
+        if isinstance(_material_mass_unit, Unset):
+            material_mass_unit = UNSET
+        else:
+            material_mass_unit = _material_mass_unit  # type: ignore[arg-type]
+
+        _output_unit = d.pop("output_unit", UNSET)
+        output_unit: Union[Unset, UnitDensity]
+        if isinstance(_output_unit, Unset):
+            output_unit = UNSET
+        else:
+            output_unit = _output_unit  # type: ignore[arg-type]
+
         _src_format = d.pop("src_format", UNSET)
         src_format: Union[Unset, FileImportFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
             src_format = _src_format  # type: ignore[arg-type]
 
@@ -867,18 +977,21 @@
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
         file_density = cls(
             completed_at=completed_at,
             created_at=created_at,
+            densities=densities,
             density=density,
             error=error,
             id=id,
             material_mass=material_mass,
+            material_mass_unit=material_mass_unit,
+            output_unit=output_unit,
             src_format=src_format,
             started_at=started_at,
             status=status,
             type=type,
             updated_at=updated_at,
             user_id=user_id,
         )
@@ -899,29 +1012,31 @@
     def __delitem__(self, key: str) -> None:
         del self.additional_properties[key]
 
     def __contains__(self, key: str) -> bool:
         return key in self.additional_properties
 
 
-C = TypeVar("C", bound="FileSurfaceArea")
+IO = TypeVar("IO", bound="FileSurfaceArea")
 
 
 @attr.s(auto_attribs=True)
 class FileSurfaceArea:
     """A file surface area."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
+    output_unit: Union[Unset, UnitArea] = UNSET
     src_format: Union[Unset, FileImportFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     surface_area: Union[Unset, float] = UNSET
+    surface_areas: Union[Unset, Any] = UNSET
     type: Union[Unset, str] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
@@ -929,22 +1044,25 @@
         if not isinstance(self.completed_at, Unset):
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
+        if not isinstance(self.output_unit, Unset):
+            output_unit = self.output_unit
         if not isinstance(self.src_format, Unset):
             src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
         if not isinstance(self.status, Unset):
             status = self.status
         surface_area = self.surface_area
+        surface_areas = self.surface_areas
         type = self.type
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
@@ -954,33 +1072,37 @@
             field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
             field_dict["created_at"] = created_at
         if error is not UNSET:
             field_dict["error"] = error
         if id is not UNSET:
             field_dict["id"] = id
+        if output_unit is not UNSET:
+            field_dict["output_unit"] = output_unit
         if src_format is not UNSET:
             field_dict["src_format"] = src_format
         if started_at is not UNSET:
             field_dict["started_at"] = started_at
         if status is not UNSET:
             field_dict["status"] = status
         if surface_area is not UNSET:
             field_dict["surface_area"] = surface_area
+        if surface_areas is not UNSET:
+            field_dict["surface_areas"] = surface_areas
         if type is not UNSET:
             field_dict["type"] = type
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[C], src_dict: Dict[str, Any]) -> C:
+    def from_dict(cls: Type[IO], src_dict: Dict[str, Any]) -> IO:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -995,15 +1117,22 @@
         error = d.pop("error", UNSET)
 
         _id = d.pop("id", UNSET)
         id: Union[Unset, Uuid]
         if isinstance(_id, Unset):
             id = UNSET
         else:
-            id = Uuid(_id)
+            id = _id  # type: ignore[arg-type]
+
+        _output_unit = d.pop("output_unit", UNSET)
+        output_unit: Union[Unset, UnitArea]
+        if isinstance(_output_unit, Unset):
+            output_unit = UNSET
+        else:
+            output_unit = _output_unit  # type: ignore[arg-type]
 
         _src_format = d.pop("src_format", UNSET)
         src_format: Union[Unset, FileImportFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
             src_format = _src_format  # type: ignore[arg-type]
@@ -1020,14 +1149,15 @@
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = _status  # type: ignore[arg-type]
 
         surface_area = d.pop("surface_area", UNSET)
 
+        surface_areas = d.pop("surface_areas", UNSET)
         type = d.pop("type", UNSET)
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
@@ -1036,18 +1166,20 @@
         user_id = d.pop("user_id", UNSET)
 
         file_surface_area = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
+            output_unit=output_unit,
             src_format=src_format,
             started_at=started_at,
             status=status,
             surface_area=surface_area,
+            surface_areas=surface_areas,
             type=type,
             updated_at=updated_at,
             user_id=user_id,
         )
 
         file_surface_area.additional_properties = d
         return file_surface_area
```

### Comparing `kittycad-0.4.4/kittycad/models/async_api_call_results_page.py` & `kittycad-0.4.5/kittycad/models/async_api_call_results_page.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
-H = TypeVar("H", bound="AsyncApiCallResultsPage")
+FV = TypeVar("FV", bound="AsyncApiCallResultsPage")
 
 
 @attr.s(auto_attribs=True)
 class AsyncApiCallResultsPage:
     """A single page of results"""  # noqa: E501
 
     from ..models.async_api_call import AsyncApiCall
@@ -33,15 +33,15 @@
             field_dict["items"] = items
         if next_page is not UNSET:
             field_dict["next_page"] = next_page
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
+    def from_dict(cls: Type[FV], src_dict: Dict[str, Any]) -> FV:
         d = src_dict.copy()
         from ..models.async_api_call import AsyncApiCall
 
         items = cast(List[AsyncApiCall], d.pop("items", UNSET))
 
         next_page = d.pop("next_page", UNSET)
```

### Comparing `kittycad-0.4.4/kittycad/models/async_api_call_type.py` & `kittycad-0.4.5/kittycad/models/async_api_call_type.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.4/kittycad/models/axis_direction_pair.py` & `kittycad-0.4.5/kittycad/models/axis_direction_pair.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import attr
 
 from ..models.axis import Axis
 from ..models.direction import Direction
 from ..types import UNSET, Unset
 
-X = TypeVar("X", bound="AxisDirectionPair")
+LE = TypeVar("LE", bound="AxisDirectionPair")
 
 
 @attr.s(auto_attribs=True)
 class AxisDirectionPair:
     """An [`Axis`] paired with a [`Direction`]."""  # noqa: E501
 
     axis: Union[Unset, Axis] = UNSET
@@ -31,15 +31,15 @@
             field_dict["axis"] = axis
         if direction is not UNSET:
             field_dict["direction"] = direction
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[X], src_dict: Dict[str, Any]) -> X:
+    def from_dict(cls: Type[LE], src_dict: Dict[str, Any]) -> LE:
         d = src_dict.copy()
         _axis = d.pop("axis", UNSET)
         axis: Union[Unset, Axis]
         if isinstance(_axis, Unset):
             axis = UNSET
         else:
             axis = _axis  # type: ignore[arg-type]
```

### Comparing `kittycad-0.4.4/kittycad/models/billing_info.py` & `kittycad-0.4.5/kittycad/models/billing_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.new_address import NewAddress
 from ..types import UNSET, Unset
 
-L = TypeVar("L", bound="BillingInfo")
+OY = TypeVar("OY", bound="BillingInfo")
 
 
 @attr.s(auto_attribs=True)
 class BillingInfo:
     """The billing information for payments."""  # noqa: E501
 
     address: Union[Unset, NewAddress] = UNSET
@@ -33,22 +33,22 @@
             field_dict["name"] = name
         if phone is not UNSET:
             field_dict["phone"] = phone
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
+    def from_dict(cls: Type[OY], src_dict: Dict[str, Any]) -> OY:
         d = src_dict.copy()
         _address = d.pop("address", UNSET)
         address: Union[Unset, NewAddress]
         if isinstance(_address, Unset):
             address = UNSET
         else:
-            address = NewAddress(_address)
+            address = _address  # type: ignore[arg-type]
 
         name = d.pop("name", UNSET)
 
         phone = d.pop("phone", UNSET)
 
         billing_info = cls(
             address=address,
```

### Comparing `kittycad-0.4.4/kittycad/models/cache_metadata.py` & `kittycad-0.4.5/kittycad/models/cache_metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-B = TypeVar("B", bound="CacheMetadata")
+HO = TypeVar("HO", bound="CacheMetadata")
 
 
 @attr.s(auto_attribs=True)
 class CacheMetadata:
     """Metadata about our cache.
 
     This is mostly used for internal purposes and debugging."""  # noqa: E501
@@ -25,15 +25,15 @@
         field_dict.update({})
         if ok is not UNSET:
             field_dict["ok"] = ok
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[B], src_dict: Dict[str, Any]) -> B:
+    def from_dict(cls: Type[HO], src_dict: Dict[str, Any]) -> HO:
         d = src_dict.copy()
         ok = d.pop("ok", UNSET)
 
         cache_metadata = cls(
             ok=ok,
         )
```

### Comparing `kittycad-0.4.4/kittycad/models/card_details.py` & `kittycad-0.4.5/kittycad/models/card_details.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.payment_method_card_checks import PaymentMethodCardChecks
 from ..types import UNSET, Unset
 
-N = TypeVar("N", bound="CardDetails")
+TM = TypeVar("TM", bound="CardDetails")
 
 
 @attr.s(auto_attribs=True)
 class CardDetails:
     """The card details of a payment method."""  # noqa: E501
 
     brand: Union[Unset, str] = UNSET
@@ -53,24 +53,24 @@
             field_dict["funding"] = funding
         if last4 is not UNSET:
             field_dict["last4"] = last4
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
+    def from_dict(cls: Type[TM], src_dict: Dict[str, Any]) -> TM:
         d = src_dict.copy()
         brand = d.pop("brand", UNSET)
 
         _checks = d.pop("checks", UNSET)
         checks: Union[Unset, PaymentMethodCardChecks]
         if isinstance(_checks, Unset):
             checks = UNSET
         else:
-            checks = PaymentMethodCardChecks(_checks)
+            checks = _checks  # type: ignore[arg-type]
 
         country = d.pop("country", UNSET)
 
         exp_month = d.pop("exp_month", UNSET)
 
         exp_year = d.pop("exp_year", UNSET)
```

### Comparing `kittycad-0.4.4/kittycad/models/cluster.py` & `kittycad-0.4.5/kittycad/models/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
-E = TypeVar("E", bound="Cluster")
+BS = TypeVar("BS", bound="Cluster")
 
 
 @attr.s(auto_attribs=True)
 class Cluster:
     """Cluster information."""  # noqa: E501
 
     addr: Union[Unset, str] = UNSET
@@ -45,15 +45,15 @@
             field_dict["tls_timeout"] = tls_timeout
         if urls is not UNSET:
             field_dict["urls"] = urls
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[E], src_dict: Dict[str, Any]) -> E:
+    def from_dict(cls: Type[BS], src_dict: Dict[str, Any]) -> BS:
         d = src_dict.copy()
         addr = d.pop("addr", UNSET)
 
         auth_timeout = d.pop("auth_timeout", UNSET)
 
         cluster_port = d.pop("cluster_port", UNSET)
```

### Comparing `kittycad-0.4.4/kittycad/models/code_output.py` & `kittycad-0.4.5/kittycad/models/code_output.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CodeOutput")
+AH = TypeVar("AH", bound="CodeOutput")
 
 
 @attr.s(auto_attribs=True)
 class CodeOutput:
     """Output of the code being executed."""  # noqa: E501
 
     from ..models.output_file import OutputFile
@@ -37,15 +37,15 @@
             field_dict["stderr"] = stderr
         if stdout is not UNSET:
             field_dict["stdout"] = stdout
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[AH], src_dict: Dict[str, Any]) -> AH:
         d = src_dict.copy()
         from ..models.output_file import OutputFile
 
         output_files = cast(List[OutputFile], d.pop("output_files", UNSET))
 
         stderr = d.pop("stderr", UNSET)
```

### Comparing `kittycad-0.4.4/kittycad/models/commit.py` & `kittycad-0.4.5/kittycad/models/commit.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-L = TypeVar("L", bound="Commit")
+EG = TypeVar("EG", bound="Commit")
 
 
 @attr.s(auto_attribs=True)
 class Commit:
     """Commit holds the Git-commit (SHA1) that a binary was built from, as reported in the version-string of external tools, such as `containerd`, or `runC`."""  # noqa: E501
 
     expected: Union[Unset, str] = UNSET
@@ -27,15 +27,15 @@
             field_dict["expected"] = expected
         if id is not UNSET:
             field_dict["id"] = id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
+    def from_dict(cls: Type[EG], src_dict: Dict[str, Any]) -> EG:
         d = src_dict.copy()
         expected = d.pop("expected", UNSET)
 
         id = d.pop("id", UNSET)
 
         commit = cls(
             expected=expected,
```

### Comparing `kittycad-0.4.4/kittycad/models/connection.py` & `kittycad-0.4.5/kittycad/models/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from ..models.cluster import Cluster
 from ..models.gateway import Gateway
 from ..models.jetstream import Jetstream
 from ..models.leaf_node import LeafNode
 from ..types import UNSET, Unset
 
-M = TypeVar("M", bound="Connection")
+JR = TypeVar("JR", bound="Connection")
 
 
 @attr.s(auto_attribs=True)
 class Connection:
     """Metadata about a pub-sub connection.
 
     This is mostly used for internal purposes and debugging."""  # noqa: E501
@@ -221,24 +221,24 @@
             field_dict["version"] = version
         if write_deadline is not UNSET:
             field_dict["write_deadline"] = write_deadline
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[M], src_dict: Dict[str, Any]) -> M:
+    def from_dict(cls: Type[JR], src_dict: Dict[str, Any]) -> JR:
         d = src_dict.copy()
         auth_timeout = d.pop("auth_timeout", UNSET)
 
         _cluster = d.pop("cluster", UNSET)
         cluster: Union[Unset, Cluster]
         if isinstance(_cluster, Unset):
             cluster = UNSET
         else:
-            cluster = Cluster(_cluster)
+            cluster = _cluster  # type: ignore[arg-type]
 
         _config_load_time = d.pop("config_load_time", UNSET)
         config_load_time: Union[Unset, datetime.datetime]
         if isinstance(_config_load_time, Unset):
             config_load_time = UNSET
         else:
             config_load_time = isoparse(_config_load_time)
@@ -250,15 +250,15 @@
         cpu = d.pop("cpu", UNSET)
 
         _gateway = d.pop("gateway", UNSET)
         gateway: Union[Unset, Gateway]
         if isinstance(_gateway, Unset):
             gateway = UNSET
         else:
-            gateway = Gateway(_gateway)
+            gateway = _gateway  # type: ignore[arg-type]
 
         git_commit = d.pop("git_commit", UNSET)
 
         go = d.pop("go", UNSET)
 
         gomaxprocs = d.pop("gomaxprocs", UNSET)
 
@@ -278,22 +278,22 @@
         in_msgs = d.pop("in_msgs", UNSET)
 
         _jetstream = d.pop("jetstream", UNSET)
         jetstream: Union[Unset, Jetstream]
         if isinstance(_jetstream, Unset):
             jetstream = UNSET
         else:
-            jetstream = Jetstream(_jetstream)
+            jetstream = _jetstream  # type: ignore[arg-type]
 
         _leaf = d.pop("leaf", UNSET)
         leaf: Union[Unset, LeafNode]
         if isinstance(_leaf, Unset):
             leaf = UNSET
         else:
-            leaf = LeafNode(_leaf)
+            leaf = _leaf  # type: ignore[arg-type]
 
         leafnodes = d.pop("leafnodes", UNSET)
 
         max_connections = d.pop("max_connections", UNSET)
 
         max_control_line = d.pop("max_control_line", UNSET)
```

### Comparing `kittycad-0.4.4/kittycad/models/country_code.py` & `kittycad-0.4.5/kittycad/models/country_code.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.4/kittycad/models/coupon.py` & `kittycad-0.4.5/kittycad/models/coupon.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-N = TypeVar("N", bound="Coupon")
+LY = TypeVar("LY", bound="Coupon")
 
 
 @attr.s(auto_attribs=True)
 class Coupon:
     """The resource representing a Coupon."""  # noqa: E501
 
     amount_off: Union[Unset, float] = UNSET
@@ -35,15 +35,15 @@
             field_dict["id"] = id
         if percent_off is not UNSET:
             field_dict["percent_off"] = percent_off
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
+    def from_dict(cls: Type[LY], src_dict: Dict[str, Any]) -> LY:
         d = src_dict.copy()
         amount_off = d.pop("amount_off", UNSET)
 
         deleted = d.pop("deleted", UNSET)
 
         id = d.pop("id", UNSET)
```

### Comparing `kittycad-0.4.4/kittycad/models/currency.py` & `kittycad-0.4.5/kittycad/models/currency.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from enum import Enum
 
 
 class Currency(str, Enum):
     """Currency is the list of supported currencies.
 
-    This comes from the Stripe API docs: For more details see <https://support.stripe.com/questions/which-currencies-does-stripe-support>."""  # noqa: E501
+    This comes from the Stripe API docs: For more details see <https://support.stripe.com/questions/which-currencies-does-stripe-support>.
+    """  # noqa: E501
 
     """# United Arab Emirates Dirham """  # noqa: E501
     AED = "aed"
     """# Afghan Afghani """  # noqa: E501
     AFN = "afn"
     """# Albanian Lek """  # noqa: E501
     ALL = "all"
```

### Comparing `kittycad-0.4.4/kittycad/models/customer.py` & `kittycad-0.4.5/kittycad/models/customer.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import attr
 from dateutil.parser import isoparse
 
 from ..models.currency import Currency
 from ..models.new_address import NewAddress
 from ..types import UNSET, Unset
 
-J = TypeVar("J", bound="Customer")
+HK = TypeVar("HK", bound="Customer")
 
 
 @attr.s(auto_attribs=True)
 class Customer:
     """The resource representing a payment "Customer"."""  # noqa: E501
 
     address: Union[Unset, NewAddress] = UNSET
@@ -67,22 +67,22 @@
             field_dict["name"] = name
         if phone is not UNSET:
             field_dict["phone"] = phone
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[J], src_dict: Dict[str, Any]) -> J:
+    def from_dict(cls: Type[HK], src_dict: Dict[str, Any]) -> HK:
         d = src_dict.copy()
         _address = d.pop("address", UNSET)
         address: Union[Unset, NewAddress]
         if isinstance(_address, Unset):
             address = UNSET
         else:
-            address = NewAddress(_address)
+            address = _address  # type: ignore[arg-type]
 
         balance = d.pop("balance", UNSET)
 
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
```

### Comparing `kittycad-0.4.4/kittycad/models/customer_balance.py` & `kittycad-0.4.5/kittycad/models/customer_balance.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-V = TypeVar("V", bound="CustomerBalance")
+VR = TypeVar("VR", bound="CustomerBalance")
 
 
 @attr.s(auto_attribs=True)
 class CustomerBalance:
     """A balance for a user.
 
     This holds information about the financial balance for the user."""  # noqa: E501
@@ -60,29 +60,29 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[V], src_dict: Dict[str, Any]) -> V:
+    def from_dict(cls: Type[VR], src_dict: Dict[str, Any]) -> VR:
         d = src_dict.copy()
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         _id = d.pop("id", UNSET)
         id: Union[Unset, Uuid]
         if isinstance(_id, Unset):
             id = UNSET
         else:
-            id = Uuid(_id)
+            id = _id  # type: ignore[arg-type]
 
         monthly_credits_remaining = d.pop("monthly_credits_remaining", UNSET)
 
         pre_pay_cash_remaining = d.pop("pre_pay_cash_remaining", UNSET)
 
         pre_pay_credits_remaining = d.pop("pre_pay_credits_remaining", UNSET)
```

### Comparing `kittycad-0.4.4/kittycad/models/device_access_token_request_form.py` & `kittycad-0.4.5/kittycad/models/device_access_token_request_form.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.o_auth2_grant_type import OAuth2GrantType
 from ..types import UNSET, Unset
 
-F = TypeVar("F", bound="DeviceAccessTokenRequestForm")
+ON = TypeVar("ON", bound="DeviceAccessTokenRequestForm")
 
 
 @attr.s(auto_attribs=True)
 class DeviceAccessTokenRequestForm:
     """The form for a device access token request."""  # noqa: E501
 
     client_id: Union[Unset, str] = UNSET
@@ -33,15 +33,15 @@
             field_dict["device_code"] = device_code
         if grant_type is not UNSET:
             field_dict["grant_type"] = grant_type
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
+    def from_dict(cls: Type[ON], src_dict: Dict[str, Any]) -> ON:
         d = src_dict.copy()
         client_id = d.pop("client_id", UNSET)
 
         device_code = d.pop("device_code", UNSET)
 
         _grant_type = d.pop("grant_type", UNSET)
         grant_type: Union[Unset, OAuth2GrantType]
```

### Comparing `kittycad-0.4.4/kittycad/models/device_auth_request_form.py` & `kittycad-0.4.5/kittycad/models/device_auth_request_form.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-V = TypeVar("V", bound="DeviceAuthRequestForm")
+PC = TypeVar("PC", bound="DeviceAuthRequestForm")
 
 
 @attr.s(auto_attribs=True)
 class DeviceAuthRequestForm:
     """The request parameters for the OAuth 2.0 Device Authorization Grant flow."""  # noqa: E501
 
     client_id: Union[Unset, str] = UNSET
@@ -23,15 +23,15 @@
         field_dict.update({})
         if client_id is not UNSET:
             field_dict["client_id"] = client_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[V], src_dict: Dict[str, Any]) -> V:
+    def from_dict(cls: Type[PC], src_dict: Dict[str, Any]) -> PC:
         d = src_dict.copy()
         client_id = d.pop("client_id", UNSET)
 
         device_auth_request_form = cls(
             client_id=client_id,
         )
```

### Comparing `kittycad-0.4.4/kittycad/models/device_auth_verify_params.py` & `kittycad-0.4.5/kittycad/models/device_auth_verify_params.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-J = TypeVar("J", bound="DeviceAuthVerifyParams")
+US = TypeVar("US", bound="DeviceAuthVerifyParams")
 
 
 @attr.s(auto_attribs=True)
 class DeviceAuthVerifyParams:
     """The request parameters to verify the `user_code` for the OAuth 2.0 Device Authorization Grant."""  # noqa: E501
 
     user_code: Union[Unset, str] = UNSET
@@ -23,15 +23,15 @@
         field_dict.update({})
         if user_code is not UNSET:
             field_dict["user_code"] = user_code
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[J], src_dict: Dict[str, Any]) -> J:
+    def from_dict(cls: Type[US], src_dict: Dict[str, Any]) -> US:
         d = src_dict.copy()
         user_code = d.pop("user_code", UNSET)
 
         device_auth_verify_params = cls(
             user_code=user_code,
         )
```

### Comparing `kittycad-0.4.4/kittycad/models/discount.py` & `kittycad-0.4.5/kittycad/models/discount.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.coupon import Coupon
 from ..types import UNSET, Unset
 
-V = TypeVar("V", bound="Discount")
+KQ = TypeVar("KQ", bound="Discount")
 
 
 @attr.s(auto_attribs=True)
 class Discount:
     """The resource representing a Discount."""  # noqa: E501
 
     coupon: Union[Unset, Coupon] = UNSET
@@ -25,22 +25,22 @@
         field_dict.update({})
         if coupon is not UNSET:
             field_dict["coupon"] = coupon
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[V], src_dict: Dict[str, Any]) -> V:
+    def from_dict(cls: Type[KQ], src_dict: Dict[str, Any]) -> KQ:
         d = src_dict.copy()
         _coupon = d.pop("coupon", UNSET)
         coupon: Union[Unset, Coupon]
         if isinstance(_coupon, Unset):
             coupon = UNSET
         else:
-            coupon = Coupon(_coupon)
+            coupon = _coupon  # type: ignore[arg-type]
 
         discount = cls(
             coupon=coupon,
         )
 
         discount.additional_properties = d
         return discount
```

### Comparing `kittycad-0.4.4/kittycad/models/docker_system_info.py` & `kittycad-0.4.5/kittycad/models/docker_system_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ..models.plugins_info import PluginsInfo
 from ..models.registry_service_config import RegistryServiceConfig
 from ..models.system_info_cgroup_driver_enum import SystemInfoCgroupDriverEnum
 from ..models.system_info_cgroup_version_enum import SystemInfoCgroupVersionEnum
 from ..models.system_info_isolation_enum import SystemInfoIsolationEnum
 from ..types import UNSET, Unset
 
-L = TypeVar("L", bound="DockerSystemInfo")
+FH = TypeVar("FH", bound="DockerSystemInfo")
 
 
 @attr.s(auto_attribs=True)
 class DockerSystemInfo:
     """Docker system info."""  # noqa: E501
 
     architecture: Union[Unset, str] = UNSET
@@ -289,46 +289,46 @@
             field_dict["system_time"] = system_time
         if warnings is not UNSET:
             field_dict["warnings"] = warnings
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
+    def from_dict(cls: Type[FH], src_dict: Dict[str, Any]) -> FH:
         d = src_dict.copy()
         architecture = d.pop("architecture", UNSET)
 
         bridge_nf_ip6tables = d.pop("bridge_nf_ip6tables", UNSET)
 
         bridge_nf_iptables = d.pop("bridge_nf_iptables", UNSET)
 
         _cgroup_driver = d.pop("cgroup_driver", UNSET)
         cgroup_driver: Union[Unset, SystemInfoCgroupDriverEnum]
         if isinstance(_cgroup_driver, Unset):
             cgroup_driver = UNSET
         else:
-            cgroup_driver = SystemInfoCgroupDriverEnum(_cgroup_driver)
+            cgroup_driver = _cgroup_driver  # type: ignore[arg-type]
 
         _cgroup_version = d.pop("cgroup_version", UNSET)
         cgroup_version: Union[Unset, SystemInfoCgroupVersionEnum]
         if isinstance(_cgroup_version, Unset):
             cgroup_version = UNSET
         else:
-            cgroup_version = SystemInfoCgroupVersionEnum(_cgroup_version)
+            cgroup_version = _cgroup_version  # type: ignore[arg-type]
 
         cluster_advertise = d.pop("cluster_advertise", UNSET)
 
         cluster_store = d.pop("cluster_store", UNSET)
 
         _containerd_commit = d.pop("containerd_commit", UNSET)
         containerd_commit: Union[Unset, Commit]
         if isinstance(_containerd_commit, Unset):
             containerd_commit = UNSET
         else:
-            containerd_commit = Commit(_containerd_commit)
+            containerd_commit = _containerd_commit  # type: ignore[arg-type]
 
         containers = d.pop("containers", UNSET)
 
         containers_paused = d.pop("containers_paused", UNSET)
 
         containers_running = d.pop("containers_running", UNSET)
 
@@ -375,24 +375,24 @@
         init_binary = d.pop("init_binary", UNSET)
 
         _init_commit = d.pop("init_commit", UNSET)
         init_commit: Union[Unset, Commit]
         if isinstance(_init_commit, Unset):
             init_commit = UNSET
         else:
-            init_commit = Commit(_init_commit)
+            init_commit = _init_commit  # type: ignore[arg-type]
 
         ipv4_forwarding = d.pop("ipv4_forwarding", UNSET)
 
         _isolation = d.pop("isolation", UNSET)
         isolation: Union[Unset, SystemInfoIsolationEnum]
         if isinstance(_isolation, Unset):
             isolation = UNSET
         else:
-            isolation = SystemInfoIsolationEnum(_isolation)
+            isolation = _isolation  # type: ignore[arg-type]
 
         kernel_memory = d.pop("kernel_memory", UNSET)
 
         kernel_memory_tcp = d.pop("kernel_memory_tcp", UNSET)
 
         kernel_version = d.pop("kernel_version", UNSET)
 
@@ -427,31 +427,31 @@
         pids_limit = d.pop("pids_limit", UNSET)
 
         _plugins = d.pop("plugins", UNSET)
         plugins: Union[Unset, PluginsInfo]
         if isinstance(_plugins, Unset):
             plugins = UNSET
         else:
-            plugins = PluginsInfo(_plugins)
+            plugins = _plugins  # type: ignore[arg-type]
 
         product_license = d.pop("product_license", UNSET)
 
         _registry_config = d.pop("registry_config", UNSET)
         registry_config: Union[Unset, RegistryServiceConfig]
         if isinstance(_registry_config, Unset):
             registry_config = UNSET
         else:
-            registry_config = RegistryServiceConfig(_registry_config)
+            registry_config = _registry_config  # type: ignore[arg-type]
 
         _runc_commit = d.pop("runc_commit", UNSET)
         runc_commit: Union[Unset, Commit]
         if isinstance(_runc_commit, Unset):
             runc_commit = UNSET
         else:
-            runc_commit = Commit(_runc_commit)
+            runc_commit = _runc_commit  # type: ignore[arg-type]
 
         runtimes = d.pop("runtimes", UNSET)
         security_options = cast(List[str], d.pop("security_options", UNSET))
 
         server_version = d.pop("server_version", UNSET)
 
         swap_limit = d.pop("swap_limit", UNSET)
```

### Comparing `kittycad-0.4.4/kittycad/models/email_authentication_form.py` & `kittycad-0.4.5/kittycad/models/email_authentication_form.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-E = TypeVar("E", bound="EmailAuthenticationForm")
+NH = TypeVar("NH", bound="EmailAuthenticationForm")
 
 
 @attr.s(auto_attribs=True)
 class EmailAuthenticationForm:
     """The body of the form for email authentication."""  # noqa: E501
 
     callback_url: Union[Unset, str] = UNSET
@@ -27,15 +27,15 @@
             field_dict["callback_url"] = callback_url
         if email is not UNSET:
             field_dict["email"] = email
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[E], src_dict: Dict[str, Any]) -> E:
+    def from_dict(cls: Type[NH], src_dict: Dict[str, Any]) -> NH:
         d = src_dict.copy()
         callback_url = d.pop("callback_url", UNSET)
 
         email = d.pop("email", UNSET)
 
         email_authentication_form = cls(
             callback_url=callback_url,
```

### Comparing `kittycad-0.4.4/kittycad/models/engine_metadata.py` & `kittycad-0.4.5/kittycad/models/engine_metadata.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ..models.cache_metadata import CacheMetadata
 from ..models.connection import Connection
 from ..models.environment import Environment
 from ..models.file_system_metadata import FileSystemMetadata
 from ..types import UNSET, Unset
 
-Y = TypeVar("Y", bound="EngineMetadata")
+BB = TypeVar("BB", bound="EngineMetadata")
 
 
 @attr.s(auto_attribs=True)
 class EngineMetadata:
     """Metadata about our currently running server.
 
     This is mostly used for internal purposes and debugging."""  # noqa: E501
@@ -53,47 +53,47 @@
             field_dict["git_hash"] = git_hash
         if pubsub is not UNSET:
             field_dict["pubsub"] = pubsub
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[Y], src_dict: Dict[str, Any]) -> Y:
+    def from_dict(cls: Type[BB], src_dict: Dict[str, Any]) -> BB:
         d = src_dict.copy()
         async_jobs_running = d.pop("async_jobs_running", UNSET)
 
         _cache = d.pop("cache", UNSET)
         cache: Union[Unset, CacheMetadata]
         if isinstance(_cache, Unset):
             cache = UNSET
         else:
-            cache = CacheMetadata(_cache)
+            cache = _cache  # type: ignore[arg-type]
 
         _environment = d.pop("environment", UNSET)
         environment: Union[Unset, Environment]
         if isinstance(_environment, Unset):
             environment = UNSET
         else:
             environment = _environment  # type: ignore[arg-type]
 
         _fs = d.pop("fs", UNSET)
         fs: Union[Unset, FileSystemMetadata]
         if isinstance(_fs, Unset):
             fs = UNSET
         else:
-            fs = FileSystemMetadata(_fs)
+            fs = _fs  # type: ignore[arg-type]
 
         git_hash = d.pop("git_hash", UNSET)
 
         _pubsub = d.pop("pubsub", UNSET)
         pubsub: Union[Unset, Connection]
         if isinstance(_pubsub, Unset):
             pubsub = UNSET
         else:
-            pubsub = Connection(_pubsub)
+            pubsub = _pubsub  # type: ignore[arg-type]
 
         engine_metadata = cls(
             async_jobs_running=async_jobs_running,
             cache=cache,
             environment=environment,
             fs=fs,
             git_hash=git_hash,
```

### Comparing `kittycad-0.4.4/kittycad/models/environment.py` & `kittycad-0.4.5/kittycad/models/environment.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.4/kittycad/models/error.py` & `kittycad-0.4.5/kittycad/models/error.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-H = TypeVar("H", bound="Error")
+PJ = TypeVar("PJ", bound="Error")
 
 
 @attr.s(auto_attribs=True)
 class Error:
     """Error information from a response."""  # noqa: E501
 
     error_code: Union[Unset, str] = UNSET
@@ -31,15 +31,15 @@
             field_dict["message"] = message
         if request_id is not UNSET:
             field_dict["request_id"] = request_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
+    def from_dict(cls: Type[PJ], src_dict: Dict[str, Any]) -> PJ:
         d = src_dict.copy()
         error_code = d.pop("error_code", UNSET)
 
         message = d.pop("message", UNSET)
 
         request_id = d.pop("request_id", UNSET)
```

### Comparing `kittycad-0.4.4/kittycad/models/executor_metadata.py` & `kittycad-0.4.5/kittycad/models/executor_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import attr
 
 from ..models.docker_system_info import DockerSystemInfo
 from ..models.environment import Environment
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ExecutorMetadata")
+TV = TypeVar("TV", bound="ExecutorMetadata")
 
 
 @attr.s(auto_attribs=True)
 class ExecutorMetadata:
     """Metadata about our currently running server.
 
     This is mostly used for internal purposes and debugging."""  # noqa: E501
@@ -37,22 +37,22 @@
             field_dict["environment"] = environment
         if git_hash is not UNSET:
             field_dict["git_hash"] = git_hash
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[TV], src_dict: Dict[str, Any]) -> TV:
         d = src_dict.copy()
         _docker_info = d.pop("docker_info", UNSET)
         docker_info: Union[Unset, DockerSystemInfo]
         if isinstance(_docker_info, Unset):
             docker_info = UNSET
         else:
-            docker_info = DockerSystemInfo(_docker_info)
+            docker_info = _docker_info  # type: ignore[arg-type]
 
         _environment = d.pop("environment", UNSET)
         environment: Union[Unset, Environment]
         if isinstance(_environment, Unset):
             environment = UNSET
         else:
             environment = _environment  # type: ignore[arg-type]
```

### Comparing `kittycad-0.4.4/kittycad/models/extended_user.py` & `kittycad-0.4.5/kittycad/models/extended_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..types import UNSET, Unset
 
-M = TypeVar("M", bound="ExtendedUser")
+CR = TypeVar("CR", bound="ExtendedUser")
 
 
 @attr.s(auto_attribs=True)
 class ExtendedUser:
     """Extended user information.
 
-    This is mostly used for internal purposes. It returns a mapping of the user's information, including that of our third party services we use for users: MailChimp, Stripe, and Front"""  # noqa: E501
+    This is mostly used for internal purposes. It returns a mapping of the user's information, including that of our third party services we use for users: MailChimp, Stripe, and Front
+    """  # noqa: E501
 
     company: Union[Unset, str] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     discord: Union[Unset, str] = UNSET
     email: Union[Unset, str] = UNSET
     email_verified: Union[Unset, datetime.datetime] = UNSET
     first_name: Union[Unset, str] = UNSET
@@ -93,15 +94,15 @@
             field_dict["stripe_id"] = stripe_id
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[M], src_dict: Dict[str, Any]) -> M:
+    def from_dict(cls: Type[CR], src_dict: Dict[str, Any]) -> CR:
         d = src_dict.copy()
         company = d.pop("company", UNSET)
 
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
```

### Comparing `kittycad-0.4.4/kittycad/models/extended_user_results_page.py` & `kittycad-0.4.5/kittycad/models/extended_user_results_page.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
-B = TypeVar("B", bound="ExtendedUserResultsPage")
+CE = TypeVar("CE", bound="ExtendedUserResultsPage")
 
 
 @attr.s(auto_attribs=True)
 class ExtendedUserResultsPage:
     """A single page of results"""  # noqa: E501
 
     from ..models.extended_user import ExtendedUser
@@ -33,15 +33,15 @@
             field_dict["items"] = items
         if next_page is not UNSET:
             field_dict["next_page"] = next_page
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[B], src_dict: Dict[str, Any]) -> B:
+    def from_dict(cls: Type[CE], src_dict: Dict[str, Any]) -> CE:
         d = src_dict.copy()
         from ..models.extended_user import ExtendedUser
 
         items = cast(List[ExtendedUser], d.pop("items", UNSET))
 
         next_page = d.pop("next_page", UNSET)
```

### Comparing `kittycad-0.4.4/kittycad/models/extrude.py` & `kittycad-0.4.5/kittycad/models/extrude.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.modeling_cmd_id import ModelingCmdId
 from ..types import UNSET, Unset
 
-S = TypeVar("S", bound="Extrude")
+MS = TypeVar("MS", bound="Extrude")
 
 
 @attr.s(auto_attribs=True)
 class Extrude:
     """Command for extruding a solid."""  # noqa: E501
 
     cap: Union[Unset, bool] = False
@@ -33,26 +33,26 @@
             field_dict["distance"] = distance
         if target is not UNSET:
             field_dict["target"] = target
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[S], src_dict: Dict[str, Any]) -> S:
+    def from_dict(cls: Type[MS], src_dict: Dict[str, Any]) -> MS:
         d = src_dict.copy()
         cap = d.pop("cap", UNSET)
 
         distance = d.pop("distance", UNSET)
 
         _target = d.pop("target", UNSET)
         target: Union[Unset, ModelingCmdId]
         if isinstance(_target, Unset):
             target = UNSET
         else:
-            target = ModelingCmdId(_target)
+            target = _target  # type: ignore[arg-type]
 
         extrude = cls(
             cap=cap,
             distance=distance,
             target=target,
         )
```

### Comparing `kittycad-0.4.4/kittycad/models/file_center_of_mass.py` & `kittycad-0.4.5/kittycad/models/file_volume.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,93 +1,99 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.file_import_format import FileImportFormat
+from ..models.unit_volume import UnitVolume
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-A = TypeVar("A", bound="FileCenterOfMass")
+NN = TypeVar("NN", bound="FileVolume")
 
 
 @attr.s(auto_attribs=True)
-class FileCenterOfMass:
-    """A file center of mass result."""  # noqa: E501
+class FileVolume:
+    """A file volume result."""  # noqa: E501
 
-    center_of_mass: Union[Unset, List[float]] = UNSET
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
+    output_unit: Union[Unset, UnitVolume] = UNSET
     src_format: Union[Unset, FileImportFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
+    volume: Union[Unset, float] = UNSET
+    volumes: Union[Unset, Any] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        center_of_mass: Union[Unset, List[float]] = UNSET
-        if not isinstance(self.center_of_mass, Unset):
-            center_of_mass = self.center_of_mass
         completed_at: Union[Unset, str] = UNSET
         if not isinstance(self.completed_at, Unset):
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
+        if not isinstance(self.output_unit, Unset):
+            output_unit = self.output_unit
         if not isinstance(self.src_format, Unset):
             src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
         if not isinstance(self.status, Unset):
             status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
+        volume = self.volume
+        volumes = self.volumes
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if center_of_mass is not UNSET:
-            field_dict["center_of_mass"] = center_of_mass
         if completed_at is not UNSET:
             field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
             field_dict["created_at"] = created_at
         if error is not UNSET:
             field_dict["error"] = error
         if id is not UNSET:
             field_dict["id"] = id
+        if output_unit is not UNSET:
+            field_dict["output_unit"] = output_unit
         if src_format is not UNSET:
             field_dict["src_format"] = src_format
         if started_at is not UNSET:
             field_dict["started_at"] = started_at
         if status is not UNSET:
             field_dict["status"] = status
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
+        if volume is not UNSET:
+            field_dict["volume"] = volume
+        if volumes is not UNSET:
+            field_dict["volumes"] = volumes
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[A], src_dict: Dict[str, Any]) -> A:
+    def from_dict(cls: Type[NN], src_dict: Dict[str, Any]) -> NN:
         d = src_dict.copy()
-        center_of_mass = cast(List[float], d.pop("center_of_mass", UNSET))
-
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
 
@@ -101,15 +107,22 @@
         error = d.pop("error", UNSET)
 
         _id = d.pop("id", UNSET)
         id: Union[Unset, Uuid]
         if isinstance(_id, Unset):
             id = UNSET
         else:
-            id = Uuid(_id)
+            id = _id  # type: ignore[arg-type]
+
+        _output_unit = d.pop("output_unit", UNSET)
+        output_unit: Union[Unset, UnitVolume]
+        if isinstance(_output_unit, Unset):
+            output_unit = UNSET
+        else:
+            output_unit = _output_unit  # type: ignore[arg-type]
 
         _src_format = d.pop("src_format", UNSET)
         src_format: Union[Unset, FileImportFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
             src_format = _src_format  # type: ignore[arg-type]
@@ -133,29 +146,35 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        file_center_of_mass = cls(
-            center_of_mass=center_of_mass,
+        volume = d.pop("volume", UNSET)
+
+        volumes = d.pop("volumes", UNSET)
+
+        file_volume = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
+            output_unit=output_unit,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
+            volume=volume,
+            volumes=volumes,
         )
 
-        file_center_of_mass.additional_properties = d
-        return file_center_of_mass
+        file_volume.additional_properties = d
+        return file_volume
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.4/kittycad/models/file_conversion.py` & `kittycad-0.4.5/kittycad/models/file_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from ..models.file_export_format import FileExportFormat
 from ..models.file_import_format import FileImportFormat
 from ..models.input_format import InputFormat
 from ..models.output_format import OutputFormat
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-H = TypeVar("H", bound="FileConversion")
+ED = TypeVar("ED", bound="FileConversion")
 
 
 @attr.s(auto_attribs=True)
 class FileConversion:
     """A file conversion."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
@@ -96,15 +96,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
+    def from_dict(cls: Type[ED], src_dict: Dict[str, Any]) -> ED:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -119,15 +119,15 @@
         error = d.pop("error", UNSET)
 
         _id = d.pop("id", UNSET)
         id: Union[Unset, Uuid]
         if isinstance(_id, Unset):
             id = UNSET
         else:
-            id = Uuid(_id)
+            id = _id  # type: ignore[arg-type]
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
         output_format: Union[Unset, FileExportFormat]
         if isinstance(_output_format, Unset):
             output_format = UNSET
@@ -135,30 +135,30 @@
             output_format = _output_format  # type: ignore[arg-type]
 
         _output_format_options = d.pop("output_format_options", UNSET)
         output_format_options: Union[Unset, OutputFormat]
         if isinstance(_output_format_options, Unset):
             output_format_options = UNSET
         else:
-            output_format_options = OutputFormat(_output_format_options)
+            output_format_options = _output_format_options  # type: ignore[arg-type]
 
         outputs = d.pop("outputs", UNSET)
         _src_format = d.pop("src_format", UNSET)
         src_format: Union[Unset, FileImportFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
             src_format = _src_format  # type: ignore[arg-type]
 
         _src_format_options = d.pop("src_format_options", UNSET)
         src_format_options: Union[Unset, InputFormat]
         if isinstance(_src_format_options, Unset):
             src_format_options = UNSET
         else:
-            src_format_options = InputFormat(_src_format_options)
+            src_format_options = _src_format_options  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
```

### Comparing `kittycad-0.4.4/kittycad/models/file_density.py` & `kittycad-0.4.5/kittycad/models/physics_constant.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,126 +1,118 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.file_import_format import FileImportFormat
+from ..models.physics_constant_name import PhysicsConstantName
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-E = TypeVar("E", bound="FileDensity")
+SS = TypeVar("SS", bound="PhysicsConstant")
 
 
 @attr.s(auto_attribs=True)
-class FileDensity:
-    """A file density result."""  # noqa: E501
+class PhysicsConstant:
+    """A physics constant."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
+    constant: Union[Unset, PhysicsConstantName] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
-    density: Union[Unset, float] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
-    material_mass: Union[Unset, float] = UNSET
-    src_format: Union[Unset, FileImportFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
+    value: Union[Unset, float] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         completed_at: Union[Unset, str] = UNSET
         if not isinstance(self.completed_at, Unset):
             completed_at = self.completed_at.isoformat()
+        if not isinstance(self.constant, Unset):
+            constant = self.constant
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
-        density = self.density
         error = self.error
         id = self.id
-        material_mass = self.material_mass
-        if not isinstance(self.src_format, Unset):
-            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
         if not isinstance(self.status, Unset):
             status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
+        value = self.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
             field_dict["completed_at"] = completed_at
+        if constant is not UNSET:
+            field_dict["constant"] = constant
         if created_at is not UNSET:
             field_dict["created_at"] = created_at
-        if density is not UNSET:
-            field_dict["density"] = density
         if error is not UNSET:
             field_dict["error"] = error
         if id is not UNSET:
             field_dict["id"] = id
-        if material_mass is not UNSET:
-            field_dict["material_mass"] = material_mass
-        if src_format is not UNSET:
-            field_dict["src_format"] = src_format
         if started_at is not UNSET:
             field_dict["started_at"] = started_at
         if status is not UNSET:
             field_dict["status"] = status
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
+        if value is not UNSET:
+            field_dict["value"] = value
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[E], src_dict: Dict[str, Any]) -> E:
+    def from_dict(cls: Type[SS], src_dict: Dict[str, Any]) -> SS:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
 
+        _constant = d.pop("constant", UNSET)
+        constant: Union[Unset, PhysicsConstantName]
+        if isinstance(_constant, Unset):
+            constant = UNSET
+        else:
+            constant = _constant  # type: ignore[arg-type]
+
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
-        density = d.pop("density", UNSET)
-
         error = d.pop("error", UNSET)
 
         _id = d.pop("id", UNSET)
         id: Union[Unset, Uuid]
         if isinstance(_id, Unset):
             id = UNSET
         else:
-            id = Uuid(_id)
-
-        material_mass = d.pop("material_mass", UNSET)
-
-        _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, FileImportFormat]
-        if isinstance(_src_format, Unset):
-            src_format = UNSET
-        else:
-            src_format = _src_format  # type: ignore[arg-type]
+            id = _id  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -137,30 +129,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        file_density = cls(
+        value = d.pop("value", UNSET)
+
+        physics_constant = cls(
             completed_at=completed_at,
+            constant=constant,
             created_at=created_at,
-            density=density,
             error=error,
             id=id,
-            material_mass=material_mass,
-            src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
+            value=value,
         )
 
-        file_density.additional_properties = d
-        return file_density
+        physics_constant.additional_properties = d
+        return physics_constant
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.4/kittycad/models/file_export_format.py` & `kittycad-0.4.5/kittycad/models/file_export_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 
 
 class FileExportFormat(str, Enum):
     """The valid types of output file formats."""  # noqa: E501
 
     """# The COLLADA/DAE file format. <https://en.wikipedia.org/wiki/COLLADA> """  # noqa: E501
     DAE = "dae"
-    """# The DXF file format. <https://en.wikipedia.org/wiki/AutoCAD_DXF> """  # noqa: E501
-    DXF = "dxf"
     """# The FBX file format. <https://en.wikipedia.org/wiki/FBX> """  # noqa: E501
     FBX = "fbx"
     """# The FBX file format (in binary). <https://en.wikipedia.org/wiki/FBX> """  # noqa: E501
     FBXB = "fbxb"
     """# glTF 2.0. We refer to this as glTF since that is how our customers refer to it, although by default it will be in binary format and thus technically (glb). """  # noqa: E501
     GLTF = "gltf"
     """# The OBJ file format. <https://en.wikipedia.org/wiki/Wavefront_.obj_file> It may or may not have an an attached material (mtl // mtllib) within the file, but we interact with it as if it does not. """  # noqa: E501
```

### Comparing `kittycad-0.4.4/kittycad/models/file_import_format.py` & `kittycad-0.4.5/kittycad/models/file_import_format.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 
 
 class FileImportFormat(str, Enum):
     """The valid types of source file formats."""  # noqa: E501
 
     """# The COLLADA/DAE file format. <https://en.wikipedia.org/wiki/COLLADA> """  # noqa: E501
     DAE = "dae"
-    """# The DXF file format. <https://en.wikipedia.org/wiki/AutoCAD_DXF> """  # noqa: E501
-    DXF = "dxf"
     """# The FBX file format. <https://en.wikipedia.org/wiki/FBX> """  # noqa: E501
     FBX = "fbx"
     """# glTF 2.0. """  # noqa: E501
     GLTF = "gltf"
     """# The OBJ file format. <https://en.wikipedia.org/wiki/Wavefront_.obj_file> It may or may not have an an attached material (mtl // mtllib) within the file, but we interact with it as if it does not. """  # noqa: E501
     OBJ = "obj"
     """# The PLY file format. <https://en.wikipedia.org/wiki/PLY_(file_format)> """  # noqa: E501
```

### Comparing `kittycad-0.4.4/kittycad/models/file_mass.py` & `kittycad-0.4.5/kittycad/models/unit_power_conversion.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.file_import_format import FileImportFormat
+from ..models.unit_power import UnitPower
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-G = TypeVar("G", bound="FileMass")
+NO = TypeVar("NO", bound="UnitPowerConversion")
 
 
 @attr.s(auto_attribs=True)
-class FileMass:
-    """A file mass result."""  # noqa: E501
+class UnitPowerConversion:
+    """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
-    mass: Union[Unset, float] = UNSET
-    material_density: Union[Unset, float] = UNSET
-    src_format: Union[Unset, FileImportFormat] = UNSET
+    input: Union[Unset, float] = UNSET
+    input_unit: Union[Unset, UnitPower] = UNSET
+    output: Union[Unset, float] = UNSET
+    output_unit: Union[Unset, UnitPower] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -35,18 +36,20 @@
         if not isinstance(self.completed_at, Unset):
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
-        mass = self.mass
-        material_density = self.material_density
-        if not isinstance(self.src_format, Unset):
-            src_format = self.src_format
+        input = self.input
+        if not isinstance(self.input_unit, Unset):
+            input_unit = self.input_unit
+        output = self.output
+        if not isinstance(self.output_unit, Unset):
+            output_unit = self.output_unit
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
         if not isinstance(self.status, Unset):
             status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
@@ -60,33 +63,35 @@
             field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
             field_dict["created_at"] = created_at
         if error is not UNSET:
             field_dict["error"] = error
         if id is not UNSET:
             field_dict["id"] = id
-        if mass is not UNSET:
-            field_dict["mass"] = mass
-        if material_density is not UNSET:
-            field_dict["material_density"] = material_density
-        if src_format is not UNSET:
-            field_dict["src_format"] = src_format
+        if input is not UNSET:
+            field_dict["input"] = input
+        if input_unit is not UNSET:
+            field_dict["input_unit"] = input_unit
+        if output is not UNSET:
+            field_dict["output"] = output
+        if output_unit is not UNSET:
+            field_dict["output_unit"] = output_unit
         if started_at is not UNSET:
             field_dict["started_at"] = started_at
         if status is not UNSET:
             field_dict["status"] = status
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[G], src_dict: Dict[str, Any]) -> G:
+    def from_dict(cls: Type[NO], src_dict: Dict[str, Any]) -> NO:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -101,26 +106,33 @@
         error = d.pop("error", UNSET)
 
         _id = d.pop("id", UNSET)
         id: Union[Unset, Uuid]
         if isinstance(_id, Unset):
             id = UNSET
         else:
-            id = Uuid(_id)
+            id = _id  # type: ignore[arg-type]
 
-        mass = d.pop("mass", UNSET)
+        input = d.pop("input", UNSET)
 
-        material_density = d.pop("material_density", UNSET)
+        _input_unit = d.pop("input_unit", UNSET)
+        input_unit: Union[Unset, UnitPower]
+        if isinstance(_input_unit, Unset):
+            input_unit = UNSET
+        else:
+            input_unit = _input_unit  # type: ignore[arg-type]
+
+        output = d.pop("output", UNSET)
 
-        _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, FileImportFormat]
-        if isinstance(_src_format, Unset):
-            src_format = UNSET
+        _output_unit = d.pop("output_unit", UNSET)
+        output_unit: Union[Unset, UnitPower]
+        if isinstance(_output_unit, Unset):
+            output_unit = UNSET
         else:
-            src_format = _src_format  # type: ignore[arg-type]
+            output_unit = _output_unit  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -137,30 +149,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        file_mass = cls(
+        unit_power_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
-            mass=mass,
-            material_density=material_density,
-            src_format=src_format,
+            input=input,
+            input_unit=input_unit,
+            output=output,
+            output_unit=output_unit,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        file_mass.additional_properties = d
-        return file_mass
+        unit_power_conversion.additional_properties = d
+        return unit_power_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.4/kittycad/models/file_surface_area.py` & `kittycad-0.4.5/kittycad/models/unit_area_conversion.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,60 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.file_import_format import FileImportFormat
+from ..models.unit_area import UnitArea
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-J = TypeVar("J", bound="FileSurfaceArea")
+CS = TypeVar("CS", bound="UnitAreaConversion")
 
 
 @attr.s(auto_attribs=True)
-class FileSurfaceArea:
-    """A file surface area result."""  # noqa: E501
+class UnitAreaConversion:
+    """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
-    src_format: Union[Unset, FileImportFormat] = UNSET
+    input: Union[Unset, float] = UNSET
+    input_unit: Union[Unset, UnitArea] = UNSET
+    output: Union[Unset, float] = UNSET
+    output_unit: Union[Unset, UnitArea] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
-    surface_area: Union[Unset, float] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         completed_at: Union[Unset, str] = UNSET
         if not isinstance(self.completed_at, Unset):
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
-        if not isinstance(self.src_format, Unset):
-            src_format = self.src_format
+        input = self.input
+        if not isinstance(self.input_unit, Unset):
+            input_unit = self.input_unit
+        output = self.output
+        if not isinstance(self.output_unit, Unset):
+            output_unit = self.output_unit
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
         if not isinstance(self.status, Unset):
             status = self.status
-        surface_area = self.surface_area
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
@@ -58,31 +63,35 @@
             field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
             field_dict["created_at"] = created_at
         if error is not UNSET:
             field_dict["error"] = error
         if id is not UNSET:
             field_dict["id"] = id
-        if src_format is not UNSET:
-            field_dict["src_format"] = src_format
+        if input is not UNSET:
+            field_dict["input"] = input
+        if input_unit is not UNSET:
+            field_dict["input_unit"] = input_unit
+        if output is not UNSET:
+            field_dict["output"] = output
+        if output_unit is not UNSET:
+            field_dict["output_unit"] = output_unit
         if started_at is not UNSET:
             field_dict["started_at"] = started_at
         if status is not UNSET:
             field_dict["status"] = status
-        if surface_area is not UNSET:
-            field_dict["surface_area"] = surface_area
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[J], src_dict: Dict[str, Any]) -> J:
+    def from_dict(cls: Type[CS], src_dict: Dict[str, Any]) -> CS:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -97,22 +106,33 @@
         error = d.pop("error", UNSET)
 
         _id = d.pop("id", UNSET)
         id: Union[Unset, Uuid]
         if isinstance(_id, Unset):
             id = UNSET
         else:
-            id = Uuid(_id)
+            id = _id  # type: ignore[arg-type]
 
-        _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, FileImportFormat]
-        if isinstance(_src_format, Unset):
-            src_format = UNSET
+        input = d.pop("input", UNSET)
+
+        _input_unit = d.pop("input_unit", UNSET)
+        input_unit: Union[Unset, UnitArea]
+        if isinstance(_input_unit, Unset):
+            input_unit = UNSET
         else:
-            src_format = _src_format  # type: ignore[arg-type]
+            input_unit = _input_unit  # type: ignore[arg-type]
+
+        output = d.pop("output", UNSET)
+
+        _output_unit = d.pop("output_unit", UNSET)
+        output_unit: Union[Unset, UnitArea]
+        if isinstance(_output_unit, Unset):
+            output_unit = UNSET
+        else:
+            output_unit = _output_unit  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -120,40 +140,40 @@
         _status = d.pop("status", UNSET)
         status: Union[Unset, ApiCallStatus]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = _status  # type: ignore[arg-type]
 
-        surface_area = d.pop("surface_area", UNSET)
-
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        file_surface_area = cls(
+        unit_area_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
-            src_format=src_format,
+            input=input,
+            input_unit=input_unit,
+            output=output,
+            output_unit=output_unit,
             started_at=started_at,
             status=status,
-            surface_area=surface_area,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        file_surface_area.additional_properties = d
-        return file_surface_area
+        unit_area_conversion.additional_properties = d
+        return unit_area_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.4/kittycad/models/file_system_metadata.py` & `kittycad-0.4.5/kittycad/models/file_system_metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-R = TypeVar("R", bound="FileSystemMetadata")
+GL = TypeVar("GL", bound="FileSystemMetadata")
 
 
 @attr.s(auto_attribs=True)
 class FileSystemMetadata:
     """Metadata about our file system.
 
     This is mostly used for internal purposes and debugging."""  # noqa: E501
@@ -25,15 +25,15 @@
         field_dict.update({})
         if ok is not UNSET:
             field_dict["ok"] = ok
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[R], src_dict: Dict[str, Any]) -> R:
+    def from_dict(cls: Type[GL], src_dict: Dict[str, Any]) -> GL:
         d = src_dict.copy()
         ok = d.pop("ok", UNSET)
 
         file_system_metadata = cls(
             ok=ok,
         )
```

### Comparing `kittycad-0.4.4/kittycad/models/file_volume.py` & `kittycad-0.4.5/kittycad/models/unit_angle_conversion.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,88 +1,97 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.file_import_format import FileImportFormat
+from ..models.unit_angle import UnitAngle
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-L = TypeVar("L", bound="FileVolume")
+LF = TypeVar("LF", bound="UnitAngleConversion")
 
 
 @attr.s(auto_attribs=True)
-class FileVolume:
-    """A file volume result."""  # noqa: E501
+class UnitAngleConversion:
+    """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
-    src_format: Union[Unset, FileImportFormat] = UNSET
+    input: Union[Unset, float] = UNSET
+    input_unit: Union[Unset, UnitAngle] = UNSET
+    output: Union[Unset, float] = UNSET
+    output_unit: Union[Unset, UnitAngle] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
-    volume: Union[Unset, float] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         completed_at: Union[Unset, str] = UNSET
         if not isinstance(self.completed_at, Unset):
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
-        if not isinstance(self.src_format, Unset):
-            src_format = self.src_format
+        input = self.input
+        if not isinstance(self.input_unit, Unset):
+            input_unit = self.input_unit
+        output = self.output
+        if not isinstance(self.output_unit, Unset):
+            output_unit = self.output_unit
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
         if not isinstance(self.status, Unset):
             status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
-        volume = self.volume
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
             field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
             field_dict["created_at"] = created_at
         if error is not UNSET:
             field_dict["error"] = error
         if id is not UNSET:
             field_dict["id"] = id
-        if src_format is not UNSET:
-            field_dict["src_format"] = src_format
+        if input is not UNSET:
+            field_dict["input"] = input
+        if input_unit is not UNSET:
+            field_dict["input_unit"] = input_unit
+        if output is not UNSET:
+            field_dict["output"] = output
+        if output_unit is not UNSET:
+            field_dict["output_unit"] = output_unit
         if started_at is not UNSET:
             field_dict["started_at"] = started_at
         if status is not UNSET:
             field_dict["status"] = status
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
-        if volume is not UNSET:
-            field_dict["volume"] = volume
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
+    def from_dict(cls: Type[LF], src_dict: Dict[str, Any]) -> LF:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -97,22 +106,33 @@
         error = d.pop("error", UNSET)
 
         _id = d.pop("id", UNSET)
         id: Union[Unset, Uuid]
         if isinstance(_id, Unset):
             id = UNSET
         else:
-            id = Uuid(_id)
+            id = _id  # type: ignore[arg-type]
 
-        _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, FileImportFormat]
-        if isinstance(_src_format, Unset):
-            src_format = UNSET
+        input = d.pop("input", UNSET)
+
+        _input_unit = d.pop("input_unit", UNSET)
+        input_unit: Union[Unset, UnitAngle]
+        if isinstance(_input_unit, Unset):
+            input_unit = UNSET
         else:
-            src_format = _src_format  # type: ignore[arg-type]
+            input_unit = _input_unit  # type: ignore[arg-type]
+
+        output = d.pop("output", UNSET)
+
+        _output_unit = d.pop("output_unit", UNSET)
+        output_unit: Union[Unset, UnitAngle]
+        if isinstance(_output_unit, Unset):
+            output_unit = UNSET
+        else:
+            output_unit = _output_unit  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -129,31 +149,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        volume = d.pop("volume", UNSET)
-
-        file_volume = cls(
+        unit_angle_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
-            src_format=src_format,
+            input=input,
+            input_unit=input_unit,
+            output=output,
+            output_unit=output_unit,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
-            volume=volume,
         )
 
-        file_volume.additional_properties = d
-        return file_volume
+        unit_angle_conversion.additional_properties = d
+        return unit_angle_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.4/kittycad/models/gateway.py` & `kittycad-0.4.5/kittycad/models/gateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-Y = TypeVar("Y", bound="Gateway")
+OH = TypeVar("OH", bound="Gateway")
 
 
 @attr.s(auto_attribs=True)
 class Gateway:
     """Gateway information."""  # noqa: E501
 
     auth_timeout: Union[Unset, int] = UNSET
@@ -39,15 +39,15 @@
             field_dict["port"] = port
         if tls_timeout is not UNSET:
             field_dict["tls_timeout"] = tls_timeout
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[Y], src_dict: Dict[str, Any]) -> Y:
+    def from_dict(cls: Type[OH], src_dict: Dict[str, Any]) -> OH:
         d = src_dict.copy()
         auth_timeout = d.pop("auth_timeout", UNSET)
 
         host = d.pop("host", UNSET)
 
         name = d.pop("name", UNSET)
```

### Comparing `kittycad-0.4.4/kittycad/models/index_info.py` & `kittycad-0.4.5/kittycad/models/index_info.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
-H = TypeVar("H", bound="IndexInfo")
+VI = TypeVar("VI", bound="IndexInfo")
 
 
 @attr.s(auto_attribs=True)
 class IndexInfo:
     """IndexInfo contains information about a registry."""  # noqa: E501
 
     mirrors: Union[Unset, List[str]] = UNSET
@@ -37,15 +37,15 @@
             field_dict["official"] = official
         if secure is not UNSET:
             field_dict["secure"] = secure
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
+    def from_dict(cls: Type[VI], src_dict: Dict[str, Any]) -> VI:
         d = src_dict.copy()
         mirrors = cast(List[str], d.pop("mirrors", UNSET))
 
         name = d.pop("name", UNSET)
 
         official = d.pop("official", UNSET)
```

### Comparing `kittycad-0.4.4/kittycad/models/input_format.py` & `kittycad-0.4.5/kittycad/models/path_segment.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,52 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.system import System
+from ..models.point2d import Point2d
+from ..models.point3d import Point3d
 from ..types import UNSET, Unset
 
-K = TypeVar("K", bound="Gltf")
+UQ = TypeVar("UQ", bound="Line")
 
 
 @attr.s(auto_attribs=True)
-class Gltf:
-    """Binary glTF 2.0. We refer to this as glTF since that is how our customers refer to it, but this can also import binary glTF (glb)."""  # noqa: E501
-
-    type: Union[Unset, str] = UNSET
+class Line:
+    end: Union[Unset, Point3d] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        type = self.type
+        if not isinstance(self.end, Unset):
+            end = self.end
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if type is not UNSET:
-            field_dict["type"] = type
+        if end is not UNSET:
+            field_dict["end"] = end
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[K], src_dict: Dict[str, Any]) -> K:
+    def from_dict(cls: Type[UQ], src_dict: Dict[str, Any]) -> UQ:
         d = src_dict.copy()
-        type = d.pop("type", UNSET)
+        _end = d.pop("end", UNSET)
+        end: Union[Unset, Point3d]
+        if isinstance(_end, Unset):
+            end = UNSET
+        else:
+            end = _end  # type: ignore[arg-type]
 
-        gltf = cls(
-            type=type,
+        line = cls(
+            end=end,
         )
 
-        gltf.additional_properties = d
-        return gltf
+        line.additional_properties = d
+        return line
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
@@ -52,124 +57,72 @@
     def __delitem__(self, key: str) -> None:
         del self.additional_properties[key]
 
     def __contains__(self, key: str) -> bool:
         return key in self.additional_properties
 
 
-V = TypeVar("V", bound="Step")
+QE = TypeVar("QE", bound="Arc")
 
 
 @attr.s(auto_attribs=True)
-class Step:
-    """ISO 10303-21 (STEP) format."""  # noqa: E501
-
-    coords: Union[Unset, System] = UNSET
-    type: Union[Unset, str] = UNSET
+class Arc:
+    angle_end: Union[Unset, float] = UNSET
+    angle_start: Union[Unset, float] = UNSET
+    center: Union[Unset, Point2d] = UNSET
+    radius: Union[Unset, float] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        if not isinstance(self.coords, Unset):
-            coords = self.coords
-        type = self.type
+        angle_end = self.angle_end
+        angle_start = self.angle_start
+        if not isinstance(self.center, Unset):
+            center = self.center
+        radius = self.radius
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if coords is not UNSET:
-            field_dict["coords"] = coords
-        if type is not UNSET:
-            field_dict["type"] = type
+        if angle_end is not UNSET:
+            field_dict["angle_end"] = angle_end
+        if angle_start is not UNSET:
+            field_dict["angle_start"] = angle_start
+        if center is not UNSET:
+            field_dict["center"] = center
+        if radius is not UNSET:
+            field_dict["radius"] = radius
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[V], src_dict: Dict[str, Any]) -> V:
+    def from_dict(cls: Type[QE], src_dict: Dict[str, Any]) -> QE:
         d = src_dict.copy()
-        _coords = d.pop("coords", UNSET)
-        coords: Union[Unset, System]
-        if isinstance(_coords, Unset):
-            coords = UNSET
-        else:
-            coords = System(_coords)
-
-        type = d.pop("type", UNSET)
-
-        step = cls(
-            coords=coords,
-            type=type,
-        )
-
-        step.additional_properties = d
-        return step
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
+        angle_end = d.pop("angle_end", UNSET)
 
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
+        angle_start = d.pop("angle_start", UNSET)
 
-
-R = TypeVar("R", bound="Obj")
-
-
-@attr.s(auto_attribs=True)
-class Obj:
-    """Wavefront OBJ format."""  # noqa: E501
-
-    coords: Union[Unset, System] = UNSET
-    type: Union[Unset, str] = UNSET
-
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        if not isinstance(self.coords, Unset):
-            coords = self.coords
-        type = self.type
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if coords is not UNSET:
-            field_dict["coords"] = coords
-        if type is not UNSET:
-            field_dict["type"] = type
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[R], src_dict: Dict[str, Any]) -> R:
-        d = src_dict.copy()
-        _coords = d.pop("coords", UNSET)
-        coords: Union[Unset, System]
-        if isinstance(_coords, Unset):
-            coords = UNSET
+        _center = d.pop("center", UNSET)
+        center: Union[Unset, Point2d]
+        if isinstance(_center, Unset):
+            center = UNSET
         else:
-            coords = System(_coords)
+            center = _center  # type: ignore[arg-type]
 
-        type = d.pop("type", UNSET)
+        radius = d.pop("radius", UNSET)
 
-        obj = cls(
-            coords=coords,
-            type=type,
+        arc = cls(
+            angle_end=angle_end,
+            angle_start=angle_start,
+            center=center,
+            radius=radius,
         )
 
-        obj.additional_properties = d
-        return obj
+        arc.additional_properties = d
+        return arc
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
@@ -180,60 +133,77 @@
     def __delitem__(self, key: str) -> None:
         del self.additional_properties[key]
 
     def __contains__(self, key: str) -> bool:
         return key in self.additional_properties
 
 
-N = TypeVar("N", bound="Stl")
+XH = TypeVar("XH", bound="Bezier")
 
 
 @attr.s(auto_attribs=True)
-class Stl:
-    """*ST**ereo**L**ithography format."""  # noqa: E501
-
-    coords: Union[Unset, System] = UNSET
-    type: Union[Unset, str] = UNSET
+class Bezier:
+    control1: Union[Unset, Point3d] = UNSET
+    control2: Union[Unset, Point3d] = UNSET
+    end: Union[Unset, Point3d] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        if not isinstance(self.coords, Unset):
-            coords = self.coords
-        type = self.type
+        if not isinstance(self.control1, Unset):
+            control1 = self.control1
+        if not isinstance(self.control2, Unset):
+            control2 = self.control2
+        if not isinstance(self.end, Unset):
+            end = self.end
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if coords is not UNSET:
-            field_dict["coords"] = coords
-        if type is not UNSET:
-            field_dict["type"] = type
+        if control1 is not UNSET:
+            field_dict["control1"] = control1
+        if control2 is not UNSET:
+            field_dict["control2"] = control2
+        if end is not UNSET:
+            field_dict["end"] = end
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
+    def from_dict(cls: Type[XH], src_dict: Dict[str, Any]) -> XH:
         d = src_dict.copy()
-        _coords = d.pop("coords", UNSET)
-        coords: Union[Unset, System]
-        if isinstance(_coords, Unset):
-            coords = UNSET
+        _control1 = d.pop("control1", UNSET)
+        control1: Union[Unset, Point3d]
+        if isinstance(_control1, Unset):
+            control1 = UNSET
         else:
-            coords = System(_coords)
+            control1 = _control1  # type: ignore[arg-type]
 
-        type = d.pop("type", UNSET)
+        _control2 = d.pop("control2", UNSET)
+        control2: Union[Unset, Point3d]
+        if isinstance(_control2, Unset):
+            control2 = UNSET
+        else:
+            control2 = _control2  # type: ignore[arg-type]
+
+        _end = d.pop("end", UNSET)
+        end: Union[Unset, Point3d]
+        if isinstance(_end, Unset):
+            end = UNSET
+        else:
+            end = _end  # type: ignore[arg-type]
 
-        stl = cls(
-            coords=coords,
-            type=type,
+        bezier = cls(
+            control1=control1,
+            control2=control2,
+            end=end,
         )
 
-        stl.additional_properties = d
-        return stl
+        bezier.additional_properties = d
+        return bezier
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
@@ -244,8 +214,8 @@
     def __delitem__(self, key: str) -> None:
         del self.additional_properties[key]
 
     def __contains__(self, key: str) -> bool:
         return key in self.additional_properties
 
 
-InputFormat = Union[Gltf, Step, Obj, Stl]
+PathSegment = Union[Line, Arc, Bezier]
```

### Comparing `kittycad-0.4.4/kittycad/models/invoice.py` & `kittycad-0.4.5/kittycad/models/invoice.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import attr
 from dateutil.parser import isoparse
 
 from ..models.currency import Currency
 from ..models.invoice_status import InvoiceStatus
 from ..types import UNSET, Unset
 
-P = TypeVar("P", bound="Invoice")
+YF = TypeVar("YF", bound="Invoice")
 
 
 @attr.s(auto_attribs=True)
 class Invoice:
     """An invoice."""  # noqa: E501
 
     amount_due: Union[Unset, float] = UNSET
@@ -139,15 +139,15 @@
             field_dict["total"] = total
         if url is not UNSET:
             field_dict["url"] = url
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[P], src_dict: Dict[str, Any]) -> P:
+    def from_dict(cls: Type[YF], src_dict: Dict[str, Any]) -> YF:
         d = src_dict.copy()
         amount_due = d.pop("amount_due", UNSET)
 
         amount_paid = d.pop("amount_paid", UNSET)
 
         amount_remaining = d.pop("amount_remaining", UNSET)
```

### Comparing `kittycad-0.4.4/kittycad/models/invoice_line_item.py` & `kittycad-0.4.5/kittycad/models/invoice_line_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.currency import Currency
 from ..types import UNSET, Unset
 
-C = TypeVar("C", bound="InvoiceLineItem")
+PY = TypeVar("PY", bound="InvoiceLineItem")
 
 
 @attr.s(auto_attribs=True)
 class InvoiceLineItem:
     """An invoice line item."""  # noqa: E501
 
     amount: Union[Unset, float] = UNSET
@@ -45,15 +45,15 @@
             field_dict["invoice_item"] = invoice_item
         if metadata is not UNSET:
             field_dict["metadata"] = metadata
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[C], src_dict: Dict[str, Any]) -> C:
+    def from_dict(cls: Type[PY], src_dict: Dict[str, Any]) -> PY:
         d = src_dict.copy()
         amount = d.pop("amount", UNSET)
 
         _currency = d.pop("currency", UNSET)
         currency: Union[Unset, Currency]
         if isinstance(_currency, Unset):
             currency = UNSET
```

### Comparing `kittycad-0.4.4/kittycad/models/invoice_status.py` & `kittycad-0.4.5/kittycad/models/invoice_status.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.4/kittycad/models/jetstream.py` & `kittycad-0.4.5/kittycad/models/jetstream.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import attr
 
 from ..models.jetstream_config import JetstreamConfig
 from ..models.jetstream_stats import JetstreamStats
 from ..models.meta_cluster_info import MetaClusterInfo
 from ..types import UNSET, Unset
 
-U = TypeVar("U", bound="Jetstream")
+LK = TypeVar("LK", bound="Jetstream")
 
 
 @attr.s(auto_attribs=True)
 class Jetstream:
     """Jetstream information."""  # noqa: E501
 
     config: Union[Unset, JetstreamConfig] = UNSET
@@ -37,36 +37,36 @@
             field_dict["meta"] = meta
         if stats is not UNSET:
             field_dict["stats"] = stats
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[U], src_dict: Dict[str, Any]) -> U:
+    def from_dict(cls: Type[LK], src_dict: Dict[str, Any]) -> LK:
         d = src_dict.copy()
         _config = d.pop("config", UNSET)
         config: Union[Unset, JetstreamConfig]
         if isinstance(_config, Unset):
             config = UNSET
         else:
-            config = JetstreamConfig(_config)
+            config = _config  # type: ignore[arg-type]
 
         _meta = d.pop("meta", UNSET)
         meta: Union[Unset, MetaClusterInfo]
         if isinstance(_meta, Unset):
             meta = UNSET
         else:
-            meta = MetaClusterInfo(_meta)
+            meta = _meta  # type: ignore[arg-type]
 
         _stats = d.pop("stats", UNSET)
         stats: Union[Unset, JetstreamStats]
         if isinstance(_stats, Unset):
             stats = UNSET
         else:
-            stats = JetstreamStats(_stats)
+            stats = _stats  # type: ignore[arg-type]
 
         jetstream = cls(
             config=config,
             meta=meta,
             stats=stats,
         )
```

### Comparing `kittycad-0.4.4/kittycad/models/jetstream_api_stats.py` & `kittycad-0.4.5/kittycad/models/jetstream_api_stats.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-S = TypeVar("S", bound="JetstreamApiStats")
+AR = TypeVar("AR", bound="JetstreamApiStats")
 
 
 @attr.s(auto_attribs=True)
 class JetstreamApiStats:
     """Jetstream API statistics."""  # noqa: E501
 
     errors: Union[Unset, int] = UNSET
@@ -31,15 +31,15 @@
             field_dict["inflight"] = inflight
         if total is not UNSET:
             field_dict["total"] = total
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[S], src_dict: Dict[str, Any]) -> S:
+    def from_dict(cls: Type[AR], src_dict: Dict[str, Any]) -> AR:
         d = src_dict.copy()
         errors = d.pop("errors", UNSET)
 
         inflight = d.pop("inflight", UNSET)
 
         total = d.pop("total", UNSET)
```

### Comparing `kittycad-0.4.4/kittycad/models/jetstream_config.py` & `kittycad-0.4.5/kittycad/models/jetstream_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-K = TypeVar("K", bound="JetstreamConfig")
+WB = TypeVar("WB", bound="JetstreamConfig")
 
 
 @attr.s(auto_attribs=True)
 class JetstreamConfig:
     """Jetstream configuration."""  # noqa: E501
 
     domain: Union[Unset, str] = UNSET
@@ -35,15 +35,15 @@
             field_dict["max_storage"] = max_storage
         if store_dir is not UNSET:
             field_dict["store_dir"] = store_dir
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[K], src_dict: Dict[str, Any]) -> K:
+    def from_dict(cls: Type[WB], src_dict: Dict[str, Any]) -> WB:
         d = src_dict.copy()
         domain = d.pop("domain", UNSET)
 
         max_memory = d.pop("max_memory", UNSET)
 
         max_storage = d.pop("max_storage", UNSET)
```

### Comparing `kittycad-0.4.4/kittycad/models/jetstream_stats.py` & `kittycad-0.4.5/kittycad/models/jetstream_stats.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.jetstream_api_stats import JetstreamApiStats
 from ..types import UNSET, Unset
 
-Q = TypeVar("Q", bound="JetstreamStats")
+KK = TypeVar("KK", bound="JetstreamStats")
 
 
 @attr.s(auto_attribs=True)
 class JetstreamStats:
     """Jetstream statistics."""  # noqa: E501
 
     accounts: Union[Unset, int] = UNSET
@@ -49,24 +49,24 @@
             field_dict["reserved_store"] = reserved_store
         if store is not UNSET:
             field_dict["store"] = store
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[Q], src_dict: Dict[str, Any]) -> Q:
+    def from_dict(cls: Type[KK], src_dict: Dict[str, Any]) -> KK:
         d = src_dict.copy()
         accounts = d.pop("accounts", UNSET)
 
         _api = d.pop("api", UNSET)
         api: Union[Unset, JetstreamApiStats]
         if isinstance(_api, Unset):
             api = UNSET
         else:
-            api = JetstreamApiStats(_api)
+            api = _api  # type: ignore[arg-type]
 
         ha_assets = d.pop("ha_assets", UNSET)
 
         memory = d.pop("memory", UNSET)
 
         reserved_memory = d.pop("reserved_memory", UNSET)
```

### Comparing `kittycad-0.4.4/kittycad/models/leaf_node.py` & `kittycad-0.4.5/kittycad/models/leaf_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-F = TypeVar("F", bound="LeafNode")
+HC = TypeVar("HC", bound="LeafNode")
 
 
 @attr.s(auto_attribs=True)
 class LeafNode:
     """Leaf node information."""  # noqa: E501
 
     auth_timeout: Union[Unset, int] = UNSET
@@ -35,15 +35,15 @@
             field_dict["port"] = port
         if tls_timeout is not UNSET:
             field_dict["tls_timeout"] = tls_timeout
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
+    def from_dict(cls: Type[HC], src_dict: Dict[str, Any]) -> HC:
         d = src_dict.copy()
         auth_timeout = d.pop("auth_timeout", UNSET)
 
         host = d.pop("host", UNSET)
 
         port = d.pop("port", UNSET)
```

### Comparing `kittycad-0.4.4/kittycad/models/mesh.py` & `kittycad-0.4.5/kittycad/models/mesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-H = TypeVar("H", bound="Mesh")
+FM = TypeVar("FM", bound="Mesh")
 
 
 @attr.s(auto_attribs=True)
 class Mesh:
     mesh: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
@@ -21,15 +21,15 @@
         field_dict.update({})
         if mesh is not UNSET:
             field_dict["mesh"] = mesh
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
+    def from_dict(cls: Type[FM], src_dict: Dict[str, Any]) -> FM:
         d = src_dict.copy()
         mesh = d.pop("mesh", UNSET)
 
         mesh = cls(
             mesh=mesh,
         )
```

### Comparing `kittycad-0.4.4/kittycad/models/meta_cluster_info.py` & `kittycad-0.4.5/kittycad/models/meta_cluster_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-N = TypeVar("N", bound="MetaClusterInfo")
+PV = TypeVar("PV", bound="MetaClusterInfo")
 
 
 @attr.s(auto_attribs=True)
 class MetaClusterInfo:
     """Jetstream statistics."""  # noqa: E501
 
     cluster_size: Union[Unset, int] = UNSET
@@ -31,15 +31,15 @@
             field_dict["leader"] = leader
         if name is not UNSET:
             field_dict["name"] = name
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
+    def from_dict(cls: Type[PV], src_dict: Dict[str, Any]) -> PV:
         d = src_dict.copy()
         cluster_size = d.pop("cluster_size", UNSET)
 
         leader = d.pop("leader", UNSET)
 
         name = d.pop("name", UNSET)
```

### Comparing `kittycad-0.4.4/kittycad/models/metadata.py` & `kittycad-0.4.5/kittycad/models/metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from ..models.engine_metadata import EngineMetadata
 from ..models.environment import Environment
 from ..models.executor_metadata import ExecutorMetadata
 from ..models.file_system_metadata import FileSystemMetadata
 from ..models.point_e_metadata import PointEMetadata
 from ..types import UNSET, Unset
 
-H = TypeVar("H", bound="Metadata")
+QI = TypeVar("QI", bound="Metadata")
 
 
 @attr.s(auto_attribs=True)
 class Metadata:
     """Metadata about our currently running server.
 
     This is mostly used for internal purposes and debugging."""  # noqa: E501
@@ -67,66 +67,66 @@
             field_dict["point_e"] = point_e
         if pubsub is not UNSET:
             field_dict["pubsub"] = pubsub
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
+    def from_dict(cls: Type[QI], src_dict: Dict[str, Any]) -> QI:
         d = src_dict.copy()
         _cache = d.pop("cache", UNSET)
         cache: Union[Unset, CacheMetadata]
         if isinstance(_cache, Unset):
             cache = UNSET
         else:
-            cache = CacheMetadata(_cache)
+            cache = _cache  # type: ignore[arg-type]
 
         _engine = d.pop("engine", UNSET)
         engine: Union[Unset, EngineMetadata]
         if isinstance(_engine, Unset):
             engine = UNSET
         else:
-            engine = EngineMetadata(_engine)
+            engine = _engine  # type: ignore[arg-type]
 
         _environment = d.pop("environment", UNSET)
         environment: Union[Unset, Environment]
         if isinstance(_environment, Unset):
             environment = UNSET
         else:
             environment = _environment  # type: ignore[arg-type]
 
         _executor = d.pop("executor", UNSET)
         executor: Union[Unset, ExecutorMetadata]
         if isinstance(_executor, Unset):
             executor = UNSET
         else:
-            executor = ExecutorMetadata(_executor)
+            executor = _executor  # type: ignore[arg-type]
 
         _fs = d.pop("fs", UNSET)
         fs: Union[Unset, FileSystemMetadata]
         if isinstance(_fs, Unset):
             fs = UNSET
         else:
-            fs = FileSystemMetadata(_fs)
+            fs = _fs  # type: ignore[arg-type]
 
         git_hash = d.pop("git_hash", UNSET)
 
         _point_e = d.pop("point_e", UNSET)
         point_e: Union[Unset, PointEMetadata]
         if isinstance(_point_e, Unset):
             point_e = UNSET
         else:
-            point_e = PointEMetadata(_point_e)
+            point_e = _point_e  # type: ignore[arg-type]
 
         _pubsub = d.pop("pubsub", UNSET)
         pubsub: Union[Unset, Connection]
         if isinstance(_pubsub, Unset):
             pubsub = UNSET
         else:
-            pubsub = Connection(_pubsub)
+            pubsub = _pubsub  # type: ignore[arg-type]
 
         metadata = cls(
             cache=cache,
             engine=engine,
             environment=environment,
             executor=executor,
             fs=fs,
```

### Comparing `kittycad-0.4.4/kittycad/models/method.py` & `kittycad-0.4.5/kittycad/models/method.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 
 class Method(str, Enum):
     """The Request Method (VERB)
 
     This type also contains constants for a number of common HTTP methods such as GET, POST, etc.
 
-    Currently includes 8 variants representing the 8 methods defined in [RFC 7230](https://tools.ietf.org/html/rfc7231#section-4.1), plus PATCH, and an Extension variant for all extensions."""  # noqa: E501
+    Currently includes 8 variants representing the 8 methods defined in [RFC 7230](https://tools.ietf.org/html/rfc7231#section-4.1), plus PATCH, and an Extension variant for all extensions.
+    """  # noqa: E501
 
     """# The `OPTIONS` method as defined in [RFC 7231](https://tools.ietf.org/html/rfc7231#section-4.2.1). """  # noqa: E501
     OPTIONS = "OPTIONS"
     """# The `GET` method as defined in [RFC 7231](https://tools.ietf.org/html/rfc7231#section-4.3.1). """  # noqa: E501
     GET = "GET"
     """# The `POST` method as defined in [RFC 7231](https://tools.ietf.org/html/rfc7231#section-4.3.1). """  # noqa: E501
     POST = "POST"
```

### Comparing `kittycad-0.4.4/kittycad/models/modeling_cmd.py` & `kittycad-0.4.5/kittycad/models/output_format.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,80 +1,61 @@
-from enum import Enum
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.camera_drag_interaction_type import CameraDragInteractionType
-from ..models.modeling_cmd_id import ModelingCmdId
-from ..models.path_segment import PathSegment
-from ..models.point2d import Point2d
-from ..models.point3d import Point3d
+from ..models.storage import Storage
+from ..models.system import System
 from ..types import UNSET, Unset
-from .extrude import Extrude
 
-
-class StartPath(str, Enum):
-    """Start a path."""  # noqa: E501
-
-    START_PATH = "StartPath"
-
-    def __str__(self) -> str:
-        return str(self.value)
-
-
-B = TypeVar("B", bound="MovePathPen")
+QO = TypeVar("QO", bound="Gltf")
 
 
 @attr.s(auto_attribs=True)
-class MovePathPen:
-    path: Union[Unset, ModelingCmdId] = UNSET
-    to: Union[Unset, Point3d] = UNSET
+class Gltf:
+    """glTF 2.0. We refer to this as glTF since that is how our customers refer to it, although by default it will be in binary format and thus technically (glb). If you prefer ascii output, you can set that option for the export."""  # noqa: E501
+
+    storage: Union[Unset, Storage] = UNSET
+    type: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        if not isinstance(self.path, Unset):
-            path = self.path
-        if not isinstance(self.to, Unset):
-            to = self.to
+        if not isinstance(self.storage, Unset):
+            storage = self.storage
+        type = self.type
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if path is not UNSET:
-            field_dict["path"] = path
-        if to is not UNSET:
-            field_dict["to"] = to
+        if storage is not UNSET:
+            field_dict["storage"] = storage
+        if type is not UNSET:
+            field_dict["type"] = type
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[B], src_dict: Dict[str, Any]) -> B:
+    def from_dict(cls: Type[QO], src_dict: Dict[str, Any]) -> QO:
         d = src_dict.copy()
-        _path = d.pop("path", UNSET)
-        path: Union[Unset, ModelingCmdId]
-        if isinstance(_path, Unset):
-            path = UNSET
+        _storage = d.pop("storage", UNSET)
+        storage: Union[Unset, Storage]
+        if isinstance(_storage, Unset):
+            storage = UNSET
         else:
-            path = ModelingCmdId(_path)
+            storage = _storage  # type: ignore[arg-type]
 
-        _to = d.pop("to", UNSET)
-        to: Union[Unset, Point3d]
-        if isinstance(_to, Unset):
-            to = UNSET
-        else:
-            to = Point3d(_to)
+        type = d.pop("type", UNSET)
 
-        move_path_pen = cls(
-            path=path,
-            to=to,
+        gltf = cls(
+            storage=storage,
+            type=type,
         )
 
-        move_path_pen.additional_properties = d
-        return move_path_pen
+        gltf.additional_properties = d
+        return gltf
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
@@ -85,64 +66,60 @@
     def __delitem__(self, key: str) -> None:
         del self.additional_properties[key]
 
     def __contains__(self, key: str) -> bool:
         return key in self.additional_properties
 
 
-B = TypeVar("B", bound="ExtendPath")
+KX = TypeVar("KX", bound="Obj")
 
 
 @attr.s(auto_attribs=True)
-class ExtendPath:
-    path: Union[Unset, ModelingCmdId] = UNSET
-    segment: Union[Unset, PathSegment] = UNSET
+class Obj:
+    """Wavefront OBJ format."""  # noqa: E501
+
+    coords: Union[Unset, System] = UNSET
+    type: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        if not isinstance(self.path, Unset):
-            path = self.path
-        if not isinstance(self.segment, Unset):
-            segment = self.segment
+        if not isinstance(self.coords, Unset):
+            coords = self.coords
+        type = self.type
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if path is not UNSET:
-            field_dict["path"] = path
-        if segment is not UNSET:
-            field_dict["segment"] = segment
+        if coords is not UNSET:
+            field_dict["coords"] = coords
+        if type is not UNSET:
+            field_dict["type"] = type
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[B], src_dict: Dict[str, Any]) -> B:
+    def from_dict(cls: Type[KX], src_dict: Dict[str, Any]) -> KX:
         d = src_dict.copy()
-        _path = d.pop("path", UNSET)
-        path: Union[Unset, ModelingCmdId]
-        if isinstance(_path, Unset):
-            path = UNSET
+        _coords = d.pop("coords", UNSET)
+        coords: Union[Unset, System]
+        if isinstance(_coords, Unset):
+            coords = UNSET
         else:
-            path = ModelingCmdId(_path)
+            coords = _coords  # type: ignore[arg-type]
 
-        _segment = d.pop("segment", UNSET)
-        segment: Union[Unset, PathSegment]
-        if isinstance(_segment, Unset):
-            segment = UNSET
-        else:
-            segment = _segment  # type: ignore[arg-type]
+        type = d.pop("type", UNSET)
 
-        extend_path = cls(
-            path=path,
-            segment=segment,
+        obj = cls(
+            coords=coords,
+            type=type,
         )
 
-        extend_path.additional_properties = d
-        return extend_path
+        obj.additional_properties = d
+        return obj
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
@@ -153,113 +130,73 @@
     def __delitem__(self, key: str) -> None:
         del self.additional_properties[key]
 
     def __contains__(self, key: str) -> bool:
         return key in self.additional_properties
 
 
-P = TypeVar("P", bound="ClosePath")
+IZ = TypeVar("IZ", bound="Ply")
 
 
 @attr.s(auto_attribs=True)
-class ClosePath:
-    path_id: Union[Unset, str] = UNSET
-
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        path_id = self.path_id
+class Ply:
+    """The PLY Polygon File Format."""  # noqa: E501
 
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if path_id is not UNSET:
-            field_dict["path_id"] = path_id
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[P], src_dict: Dict[str, Any]) -> P:
-        d = src_dict.copy()
-        path_id = d.pop("path_id", UNSET)
-
-        close_path = cls(
-            path_id=path_id,
-        )
-
-        close_path.additional_properties = d
-        return close_path
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-
-J = TypeVar("J", bound="CameraDragStart")
-
-
-@attr.s(auto_attribs=True)
-class CameraDragStart:
-    interaction: Union[Unset, CameraDragInteractionType] = UNSET
-    window: Union[Unset, Point2d] = UNSET
+    coords: Union[Unset, System] = UNSET
+    storage: Union[Unset, Storage] = UNSET
+    type: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        if not isinstance(self.interaction, Unset):
-            interaction = self.interaction
-        if not isinstance(self.window, Unset):
-            window = self.window
+        if not isinstance(self.coords, Unset):
+            coords = self.coords
+        if not isinstance(self.storage, Unset):
+            storage = self.storage
+        type = self.type
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if interaction is not UNSET:
-            field_dict["interaction"] = interaction
-        if window is not UNSET:
-            field_dict["window"] = window
+        if coords is not UNSET:
+            field_dict["coords"] = coords
+        if storage is not UNSET:
+            field_dict["storage"] = storage
+        if type is not UNSET:
+            field_dict["type"] = type
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[J], src_dict: Dict[str, Any]) -> J:
+    def from_dict(cls: Type[IZ], src_dict: Dict[str, Any]) -> IZ:
         d = src_dict.copy()
-        _interaction = d.pop("interaction", UNSET)
-        interaction: Union[Unset, CameraDragInteractionType]
-        if isinstance(_interaction, Unset):
-            interaction = UNSET
+        _coords = d.pop("coords", UNSET)
+        coords: Union[Unset, System]
+        if isinstance(_coords, Unset):
+            coords = UNSET
         else:
-            interaction = _interaction  # type: ignore[arg-type]
+            coords = _coords  # type: ignore[arg-type]
 
-        _window = d.pop("window", UNSET)
-        window: Union[Unset, Point2d]
-        if isinstance(_window, Unset):
-            window = UNSET
+        _storage = d.pop("storage", UNSET)
+        storage: Union[Unset, Storage]
+        if isinstance(_storage, Unset):
+            storage = UNSET
         else:
-            window = Point2d(_window)
+            storage = _storage  # type: ignore[arg-type]
 
-        camera_drag_start = cls(
-            interaction=interaction,
-            window=window,
+        type = d.pop("type", UNSET)
+
+        ply = cls(
+            coords=coords,
+            storage=storage,
+            type=type,
         )
 
-        camera_drag_start.additional_properties = d
-        return camera_drag_start
+        ply.additional_properties = d
+        return ply
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
@@ -270,71 +207,60 @@
     def __delitem__(self, key: str) -> None:
         del self.additional_properties[key]
 
     def __contains__(self, key: str) -> bool:
         return key in self.additional_properties
 
 
-T = TypeVar("T", bound="CameraDragMove")
+WO = TypeVar("WO", bound="Step")
 
 
 @attr.s(auto_attribs=True)
-class CameraDragMove:
-    interaction: Union[Unset, CameraDragInteractionType] = UNSET
-    sequence: Union[Unset, int] = UNSET
-    window: Union[Unset, Point2d] = UNSET
+class Step:
+    """ISO 10303-21 (STEP) format."""  # noqa: E501
+
+    coords: Union[Unset, System] = UNSET
+    type: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        if not isinstance(self.interaction, Unset):
-            interaction = self.interaction
-        sequence = self.sequence
-        if not isinstance(self.window, Unset):
-            window = self.window
+        if not isinstance(self.coords, Unset):
+            coords = self.coords
+        type = self.type
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if interaction is not UNSET:
-            field_dict["interaction"] = interaction
-        if sequence is not UNSET:
-            field_dict["sequence"] = sequence
-        if window is not UNSET:
-            field_dict["window"] = window
+        if coords is not UNSET:
+            field_dict["coords"] = coords
+        if type is not UNSET:
+            field_dict["type"] = type
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[WO], src_dict: Dict[str, Any]) -> WO:
         d = src_dict.copy()
-        _interaction = d.pop("interaction", UNSET)
-        interaction: Union[Unset, CameraDragInteractionType]
-        if isinstance(_interaction, Unset):
-            interaction = UNSET
+        _coords = d.pop("coords", UNSET)
+        coords: Union[Unset, System]
+        if isinstance(_coords, Unset):
+            coords = UNSET
         else:
-            interaction = _interaction  # type: ignore[arg-type]
-
-        sequence = d.pop("sequence", UNSET)
+            coords = _coords  # type: ignore[arg-type]
 
-        _window = d.pop("window", UNSET)
-        window: Union[Unset, Point2d]
-        if isinstance(_window, Unset):
-            window = UNSET
-        else:
-            window = Point2d(_window)
+        type = d.pop("type", UNSET)
 
-        camera_drag_move = cls(
-            interaction=interaction,
-            sequence=sequence,
-            window=window,
+        step = cls(
+            coords=coords,
+            type=type,
         )
 
-        camera_drag_move.additional_properties = d
-        return camera_drag_move
+        step.additional_properties = d
+        return step
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
@@ -345,64 +271,73 @@
     def __delitem__(self, key: str) -> None:
         del self.additional_properties[key]
 
     def __contains__(self, key: str) -> bool:
         return key in self.additional_properties
 
 
-V = TypeVar("V", bound="CameraDragEnd")
+NK = TypeVar("NK", bound="Stl")
 
 
 @attr.s(auto_attribs=True)
-class CameraDragEnd:
-    interaction: Union[Unset, CameraDragInteractionType] = UNSET
-    window: Union[Unset, Point2d] = UNSET
+class Stl:
+    """*ST**ereo**L**ithography format."""  # noqa: E501
+
+    coords: Union[Unset, System] = UNSET
+    storage: Union[Unset, Storage] = UNSET
+    type: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        if not isinstance(self.interaction, Unset):
-            interaction = self.interaction
-        if not isinstance(self.window, Unset):
-            window = self.window
+        if not isinstance(self.coords, Unset):
+            coords = self.coords
+        if not isinstance(self.storage, Unset):
+            storage = self.storage
+        type = self.type
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if interaction is not UNSET:
-            field_dict["interaction"] = interaction
-        if window is not UNSET:
-            field_dict["window"] = window
+        if coords is not UNSET:
+            field_dict["coords"] = coords
+        if storage is not UNSET:
+            field_dict["storage"] = storage
+        if type is not UNSET:
+            field_dict["type"] = type
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[V], src_dict: Dict[str, Any]) -> V:
+    def from_dict(cls: Type[NK], src_dict: Dict[str, Any]) -> NK:
         d = src_dict.copy()
-        _interaction = d.pop("interaction", UNSET)
-        interaction: Union[Unset, CameraDragInteractionType]
-        if isinstance(_interaction, Unset):
-            interaction = UNSET
+        _coords = d.pop("coords", UNSET)
+        coords: Union[Unset, System]
+        if isinstance(_coords, Unset):
+            coords = UNSET
         else:
-            interaction = _interaction  # type: ignore[arg-type]
+            coords = _coords  # type: ignore[arg-type]
 
-        _window = d.pop("window", UNSET)
-        window: Union[Unset, Point2d]
-        if isinstance(_window, Unset):
-            window = UNSET
+        _storage = d.pop("storage", UNSET)
+        storage: Union[Unset, Storage]
+        if isinstance(_storage, Unset):
+            storage = UNSET
         else:
-            window = Point2d(_window)
+            storage = _storage  # type: ignore[arg-type]
+
+        type = d.pop("type", UNSET)
 
-        camera_drag_end = cls(
-            interaction=interaction,
-            window=window,
+        stl = cls(
+            coords=coords,
+            storage=storage,
+            type=type,
         )
 
-        camera_drag_end.additional_properties = d
-        return camera_drag_end
+        stl.additional_properties = d
+        return stl
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
@@ -413,17 +348,8 @@
     def __delitem__(self, key: str) -> None:
         del self.additional_properties[key]
 
     def __contains__(self, key: str) -> bool:
         return key in self.additional_properties
 
 
-ModelingCmd = Union[
-    StartPath,
-    MovePathPen,
-    ExtendPath,
-    Extrude,
-    ClosePath,
-    CameraDragStart,
-    CameraDragMove,
-    CameraDragEnd,
-]
+OutputFormat = Union[Gltf, Obj, Ply, Step, Stl]
```

### Comparing `kittycad-0.4.4/kittycad/models/modeling_cmd_req.py` & `kittycad-0.4.5/kittycad/models/modeling_cmd_req.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import attr
 
 from ..models.modeling_cmd import ModelingCmd
 from ..models.modeling_cmd_id import ModelingCmdId
 from ..types import UNSET, Unset
 
-C = TypeVar("C", bound="ModelingCmdReq")
+DN = TypeVar("DN", bound="ModelingCmdReq")
 
 
 @attr.s(auto_attribs=True)
 class ModelingCmdReq:
     """A graphics command submitted to the KittyCAD engine via the Modeling API."""  # noqa: E501
 
     cmd: Union[Unset, ModelingCmd] = UNSET
@@ -35,29 +35,29 @@
             field_dict["cmd_id"] = cmd_id
         if file_id is not UNSET:
             field_dict["file_id"] = file_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[C], src_dict: Dict[str, Any]) -> C:
+    def from_dict(cls: Type[DN], src_dict: Dict[str, Any]) -> DN:
         d = src_dict.copy()
         _cmd = d.pop("cmd", UNSET)
         cmd: Union[Unset, ModelingCmd]
         if isinstance(_cmd, Unset):
             cmd = UNSET
         else:
             cmd = _cmd  # type: ignore[arg-type]
 
         _cmd_id = d.pop("cmd_id", UNSET)
         cmd_id: Union[Unset, ModelingCmdId]
         if isinstance(_cmd_id, Unset):
             cmd_id = UNSET
         else:
-            cmd_id = ModelingCmdId(_cmd_id)
+            cmd_id = _cmd_id  # type: ignore[arg-type]
 
         file_id = d.pop("file_id", UNSET)
 
         modeling_cmd_req = cls(
             cmd=cmd,
             cmd_id=cmd_id,
             file_id=file_id,
```

### Comparing `kittycad-0.4.4/kittycad/models/modeling_cmd_req_batch.py` & `kittycad-0.4.5/kittycad/models/modeling_cmd_req_batch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-R = TypeVar("R", bound="ModelingCmdReqBatch")
+BA = TypeVar("BA", bound="ModelingCmdReqBatch")
 
 
 @attr.s(auto_attribs=True)
 class ModelingCmdReqBatch:
     """A batch set of graphics commands submitted to the KittyCAD engine via the Modeling API."""  # noqa: E501
 
     cmds: Union[Unset, Any] = UNSET
@@ -27,15 +27,15 @@
             field_dict["cmds"] = cmds
         if file_id is not UNSET:
             field_dict["file_id"] = file_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[R], src_dict: Dict[str, Any]) -> R:
+    def from_dict(cls: Type[BA], src_dict: Dict[str, Any]) -> BA:
         d = src_dict.copy()
         cmds = d.pop("cmds", UNSET)
         file_id = d.pop("file_id", UNSET)
 
         modeling_cmd_req_batch = cls(
             cmds=cmds,
             file_id=file_id,
```

### Comparing `kittycad-0.4.4/kittycad/models/modeling_error.py` & `kittycad-0.4.5/kittycad/models/modeling_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-C = TypeVar("C", bound="ModelingError")
+OR = TypeVar("OR", bound="ModelingError")
 
 
 @attr.s(auto_attribs=True)
 class ModelingError:
     """Why a command submitted to the Modeling API failed."""  # noqa: E501
 
     error_code: Union[Unset, str] = UNSET
@@ -35,15 +35,15 @@
             field_dict["internal_message"] = internal_message
         if status_code is not UNSET:
             field_dict["status_code"] = status_code
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[C], src_dict: Dict[str, Any]) -> C:
+    def from_dict(cls: Type[OR], src_dict: Dict[str, Any]) -> OR:
         d = src_dict.copy()
         error_code = d.pop("error_code", UNSET)
 
         external_message = d.pop("external_message", UNSET)
 
         internal_message = d.pop("internal_message", UNSET)
```

### Comparing `kittycad-0.4.4/kittycad/models/modeling_outcome.py` & `kittycad-0.4.5/kittycad/models/modeling_outcome.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Success = Any
 
 
 Error = ModelingError
 
 
-E = TypeVar("E", bound="Cancelled")
+CB = TypeVar("CB", bound="Cancelled")
 
 
 @attr.s(auto_attribs=True)
 class Cancelled:
     what_failed: Union[Unset, ModelingCmdId] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
@@ -30,22 +30,22 @@
         field_dict.update({})
         if what_failed is not UNSET:
             field_dict["what_failed"] = what_failed
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[E], src_dict: Dict[str, Any]) -> E:
+    def from_dict(cls: Type[CB], src_dict: Dict[str, Any]) -> CB:
         d = src_dict.copy()
         _what_failed = d.pop("what_failed", UNSET)
         what_failed: Union[Unset, ModelingCmdId]
         if isinstance(_what_failed, Unset):
             what_failed = UNSET
         else:
-            what_failed = ModelingCmdId(_what_failed)
+            what_failed = _what_failed  # type: ignore[arg-type]
 
         cancelled = cls(
             what_failed=what_failed,
         )
 
         cancelled.additional_properties = d
         return cancelled
```

### Comparing `kittycad-0.4.4/kittycad/models/modeling_outcomes.py` & `kittycad-0.4.5/kittycad/models/modeling_outcomes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-M = TypeVar("M", bound="ModelingOutcomes")
+LC = TypeVar("LC", bound="ModelingOutcomes")
 
 
 @attr.s(auto_attribs=True)
 class ModelingOutcomes:
     """The result from a batch of modeling commands."""  # noqa: E501
 
     outcomes: Union[Unset, Any] = UNSET
@@ -23,15 +23,15 @@
         field_dict.update({})
         if outcomes is not UNSET:
             field_dict["outcomes"] = outcomes
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[M], src_dict: Dict[str, Any]) -> M:
+    def from_dict(cls: Type[LC], src_dict: Dict[str, Any]) -> LC:
         d = src_dict.copy()
         outcomes = d.pop("outcomes", UNSET)
 
         modeling_outcomes = cls(
             outcomes=outcomes,
         )
```

### Comparing `kittycad-0.4.4/kittycad/models/new_address.py` & `kittycad-0.4.5/kittycad/models/new_address.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.country_code import CountryCode
 from ..types import UNSET, Unset
 
-S = TypeVar("S", bound="NewAddress")
+TO = TypeVar("TO", bound="NewAddress")
 
 
 @attr.s(auto_attribs=True)
 class NewAddress:
     """The struct that is used to create a new record. This is automatically generated and has all the same fields as the main struct only it is missing the `id`."""  # noqa: E501
 
     city: Union[Unset, str] = UNSET
@@ -49,15 +49,15 @@
             field_dict["user_id"] = user_id
         if zip is not UNSET:
             field_dict["zip"] = zip
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[S], src_dict: Dict[str, Any]) -> S:
+    def from_dict(cls: Type[TO], src_dict: Dict[str, Any]) -> TO:
         d = src_dict.copy()
         city = d.pop("city", UNSET)
 
         _country = d.pop("country", UNSET)
         country: Union[Unset, CountryCode]
         if isinstance(_country, Unset):
             country = UNSET
```

### Comparing `kittycad-0.4.4/kittycad/models/o_auth2_client_info.py` & `kittycad-0.4.5/kittycad/models/o_auth2_client_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-L = TypeVar("L", bound="OAuth2ClientInfo")
+ZP = TypeVar("ZP", bound="OAuth2ClientInfo")
 
 
 @attr.s(auto_attribs=True)
 class OAuth2ClientInfo:
     """Information about an OAuth 2.0 client."""  # noqa: E501
 
     csrf_token: Union[Unset, str] = UNSET
@@ -31,15 +31,15 @@
             field_dict["pkce_code_verifier"] = pkce_code_verifier
         if url is not UNSET:
             field_dict["url"] = url
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
+    def from_dict(cls: Type[ZP], src_dict: Dict[str, Any]) -> ZP:
         d = src_dict.copy()
         csrf_token = d.pop("csrf_token", UNSET)
 
         pkce_code_verifier = d.pop("pkce_code_verifier", UNSET)
 
         url = d.pop("url", UNSET)
```

### Comparing `kittycad-0.4.4/kittycad/models/onboarding.py` & `kittycad-0.4.5/kittycad/models/onboarding.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="Onboarding")
+EO = TypeVar("EO", bound="Onboarding")
 
 
 @attr.s(auto_attribs=True)
 class Onboarding:
     """Onboarding details"""  # noqa: E501
 
     first_call_from__their_machine_date: Union[Unset, str] = UNSET
@@ -33,15 +33,15 @@
             field_dict["first_litterbox_execute_date"] = first_litterbox_execute_date
         if first_token_date is not UNSET:
             field_dict["first_token_date"] = first_token_date
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[EO], src_dict: Dict[str, Any]) -> EO:
         d = src_dict.copy()
         first_call_from__their_machine_date = d.pop(
             "first_call_from_their_machine_date", UNSET
         )
 
         first_litterbox_execute_date = d.pop("first_litterbox_execute_date", UNSET)
```

### Comparing `kittycad-0.4.4/kittycad/models/output_file.py` & `kittycad-0.4.5/kittycad/models/output_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-E = TypeVar("E", bound="OutputFile")
+NY = TypeVar("NY", bound="OutputFile")
 
 
 @attr.s(auto_attribs=True)
 class OutputFile:
     """Output file contents."""  # noqa: E501
 
     contents: Union[Unset, str] = UNSET
@@ -27,15 +27,15 @@
             field_dict["contents"] = contents
         if name is not UNSET:
             field_dict["name"] = name
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[E], src_dict: Dict[str, Any]) -> E:
+    def from_dict(cls: Type[NY], src_dict: Dict[str, Any]) -> NY:
         d = src_dict.copy()
         contents = d.pop("contents", UNSET)
 
         name = d.pop("name", UNSET)
 
         output_file = cls(
             contents=contents,
```

### Comparing `kittycad-0.4.4/kittycad/models/payment_intent.py` & `kittycad-0.4.5/kittycad/models/payment_intent.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-L = TypeVar("L", bound="PaymentIntent")
+KT = TypeVar("KT", bound="PaymentIntent")
 
 
 @attr.s(auto_attribs=True)
 class PaymentIntent:
     """A payment intent response."""  # noqa: E501
 
     client_secret: Union[Unset, str] = UNSET
@@ -23,15 +23,15 @@
         field_dict.update({})
         if client_secret is not UNSET:
             field_dict["client_secret"] = client_secret
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
+    def from_dict(cls: Type[KT], src_dict: Dict[str, Any]) -> KT:
         d = src_dict.copy()
         client_secret = d.pop("client_secret", UNSET)
 
         payment_intent = cls(
             client_secret=client_secret,
         )
```

### Comparing `kittycad-0.4.4/kittycad/models/payment_method.py` & `kittycad-0.4.5/kittycad/models/payment_method.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from dateutil.parser import isoparse
 
 from ..models.billing_info import BillingInfo
 from ..models.card_details import CardDetails
 from ..models.payment_method_type import PaymentMethodType
 from ..types import UNSET, Unset
 
-N = TypeVar("N", bound="PaymentMethod")
+BV = TypeVar("BV", bound="PaymentMethod")
 
 
 @attr.s(auto_attribs=True)
 class PaymentMethod:
     """A payment method."""  # noqa: E501
 
     billing_info: Union[Unset, BillingInfo] = UNSET
@@ -53,29 +53,29 @@
             field_dict["metadata"] = metadata
         if type is not UNSET:
             field_dict["type"] = type
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
+    def from_dict(cls: Type[BV], src_dict: Dict[str, Any]) -> BV:
         d = src_dict.copy()
         _billing_info = d.pop("billing_info", UNSET)
         billing_info: Union[Unset, BillingInfo]
         if isinstance(_billing_info, Unset):
             billing_info = UNSET
         else:
-            billing_info = BillingInfo(_billing_info)
+            billing_info = _billing_info  # type: ignore[arg-type]
 
         _card = d.pop("card", UNSET)
         card: Union[Unset, CardDetails]
         if isinstance(_card, Unset):
             card = UNSET
         else:
-            card = CardDetails(_card)
+            card = _card  # type: ignore[arg-type]
 
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
```

### Comparing `kittycad-0.4.4/kittycad/models/payment_method_card_checks.py` & `kittycad-0.4.5/kittycad/models/payment_method_card_checks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-N = TypeVar("N", bound="PaymentMethodCardChecks")
+GU = TypeVar("GU", bound="PaymentMethodCardChecks")
 
 
 @attr.s(auto_attribs=True)
 class PaymentMethodCardChecks:
     """Card checks."""  # noqa: E501
 
     address_line1_check: Union[Unset, str] = UNSET
@@ -31,15 +31,15 @@
             field_dict["address_postal_code_check"] = address_postal_code_check
         if cvc_check is not UNSET:
             field_dict["cvc_check"] = cvc_check
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
+    def from_dict(cls: Type[GU], src_dict: Dict[str, Any]) -> GU:
         d = src_dict.copy()
         address_line1_check = d.pop("address_line1_check", UNSET)
 
         address_postal_code_check = d.pop("address_postal_code_check", UNSET)
 
         cvc_check = d.pop("cvc_check", UNSET)
```

### Comparing `kittycad-0.4.4/kittycad/models/physics_constant.py` & `kittycad-0.4.5/kittycad/models/unit_torque_conversion.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,118 +1,138 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.physics_constant_name import PhysicsConstantName
+from ..models.unit_torque import UnitTorque
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-H = TypeVar("H", bound="PhysicsConstant")
+IT = TypeVar("IT", bound="UnitTorqueConversion")
 
 
 @attr.s(auto_attribs=True)
-class PhysicsConstant:
-    """A physics constant."""  # noqa: E501
+class UnitTorqueConversion:
+    """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
-    constant: Union[Unset, PhysicsConstantName] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
+    input: Union[Unset, float] = UNSET
+    input_unit: Union[Unset, UnitTorque] = UNSET
+    output: Union[Unset, float] = UNSET
+    output_unit: Union[Unset, UnitTorque] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
-    value: Union[Unset, float] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         completed_at: Union[Unset, str] = UNSET
         if not isinstance(self.completed_at, Unset):
             completed_at = self.completed_at.isoformat()
-        if not isinstance(self.constant, Unset):
-            constant = self.constant
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
+        input = self.input
+        if not isinstance(self.input_unit, Unset):
+            input_unit = self.input_unit
+        output = self.output
+        if not isinstance(self.output_unit, Unset):
+            output_unit = self.output_unit
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
         if not isinstance(self.status, Unset):
             status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
-        value = self.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
             field_dict["completed_at"] = completed_at
-        if constant is not UNSET:
-            field_dict["constant"] = constant
         if created_at is not UNSET:
             field_dict["created_at"] = created_at
         if error is not UNSET:
             field_dict["error"] = error
         if id is not UNSET:
             field_dict["id"] = id
+        if input is not UNSET:
+            field_dict["input"] = input
+        if input_unit is not UNSET:
+            field_dict["input_unit"] = input_unit
+        if output is not UNSET:
+            field_dict["output"] = output
+        if output_unit is not UNSET:
+            field_dict["output_unit"] = output_unit
         if started_at is not UNSET:
             field_dict["started_at"] = started_at
         if status is not UNSET:
             field_dict["status"] = status
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
-        if value is not UNSET:
-            field_dict["value"] = value
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
+    def from_dict(cls: Type[IT], src_dict: Dict[str, Any]) -> IT:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
 
-        _constant = d.pop("constant", UNSET)
-        constant: Union[Unset, PhysicsConstantName]
-        if isinstance(_constant, Unset):
-            constant = UNSET
-        else:
-            constant = _constant  # type: ignore[arg-type]
-
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
         _id = d.pop("id", UNSET)
         id: Union[Unset, Uuid]
         if isinstance(_id, Unset):
             id = UNSET
         else:
-            id = Uuid(_id)
+            id = _id  # type: ignore[arg-type]
+
+        input = d.pop("input", UNSET)
+
+        _input_unit = d.pop("input_unit", UNSET)
+        input_unit: Union[Unset, UnitTorque]
+        if isinstance(_input_unit, Unset):
+            input_unit = UNSET
+        else:
+            input_unit = _input_unit  # type: ignore[arg-type]
+
+        output = d.pop("output", UNSET)
+
+        _output_unit = d.pop("output_unit", UNSET)
+        output_unit: Union[Unset, UnitTorque]
+        if isinstance(_output_unit, Unset):
+            output_unit = UNSET
+        else:
+            output_unit = _output_unit  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -129,31 +149,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        value = d.pop("value", UNSET)
-
-        physics_constant = cls(
+        unit_torque_conversion = cls(
             completed_at=completed_at,
-            constant=constant,
             created_at=created_at,
             error=error,
             id=id,
+            input=input,
+            input_unit=input_unit,
+            output=output,
+            output_unit=output_unit,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
-            value=value,
         )
 
-        physics_constant.additional_properties = d
-        return physics_constant
+        unit_torque_conversion.additional_properties = d
+        return unit_torque_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.4/kittycad/models/physics_constant_name.py` & `kittycad-0.4.5/kittycad/models/physics_constant_name.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.4/kittycad/models/plugins_info.py` & `kittycad-0.4.5/kittycad/models/plugins_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
-V = TypeVar("V", bound="PluginsInfo")
+UP = TypeVar("UP", bound="PluginsInfo")
 
 
 @attr.s(auto_attribs=True)
 class PluginsInfo:
     """Available plugins per type.
 
-    **Note**: Only unmanaged (V1) plugins are included in this list. V1 plugins are \"lazily\" loaded, and are not returned in this list if there is no resource using the plugin."""  # noqa: E501
+    **Note**: Only unmanaged (V1) plugins are included in this list. V1 plugins are \"lazily\" loaded, and are not returned in this list if there is no resource using the plugin.
+    """  # noqa: E501
 
     authorization: Union[Unset, List[str]] = UNSET
     log: Union[Unset, List[str]] = UNSET
     network: Union[Unset, List[str]] = UNSET
     volume: Union[Unset, List[str]] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
@@ -45,15 +46,15 @@
             field_dict["network"] = network
         if volume is not UNSET:
             field_dict["volume"] = volume
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[V], src_dict: Dict[str, Any]) -> V:
+    def from_dict(cls: Type[UP], src_dict: Dict[str, Any]) -> UP:
         d = src_dict.copy()
         authorization = cast(List[str], d.pop("authorization", UNSET))
 
         log = cast(List[str], d.pop("log", UNSET))
 
         network = cast(List[str], d.pop("network", UNSET))
```

### Comparing `kittycad-0.4.4/kittycad/models/point2d.py` & `kittycad-0.4.5/kittycad/models/point2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-E = TypeVar("E", bound="Point2d")
+AZ = TypeVar("AZ", bound="Point2d")
 
 
 @attr.s(auto_attribs=True)
 class Point2d:
     """A point in 2D space"""  # noqa: E501
 
     x: Union[Unset, float] = UNSET
@@ -27,15 +27,15 @@
             field_dict["x"] = x
         if y is not UNSET:
             field_dict["y"] = y
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[E], src_dict: Dict[str, Any]) -> E:
+    def from_dict(cls: Type[AZ], src_dict: Dict[str, Any]) -> AZ:
         d = src_dict.copy()
         x = d.pop("x", UNSET)
 
         y = d.pop("y", UNSET)
 
         point2d = cls(
             x=x,
```

### Comparing `kittycad-0.4.4/kittycad/models/point3d.py` & `kittycad-0.4.5/kittycad/models/point3d.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="Point3d")
+DJ = TypeVar("DJ", bound="Point3d")
 
 
 @attr.s(auto_attribs=True)
 class Point3d:
     """A point in 3D space"""  # noqa: E501
 
     x: Union[Unset, float] = UNSET
@@ -31,15 +31,15 @@
             field_dict["y"] = y
         if z is not UNSET:
             field_dict["z"] = z
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[DJ], src_dict: Dict[str, Any]) -> DJ:
         d = src_dict.copy()
         x = d.pop("x", UNSET)
 
         y = d.pop("y", UNSET)
 
         z = d.pop("z", UNSET)
```

### Comparing `kittycad-0.4.4/kittycad/models/point_e_metadata.py` & `kittycad-0.4.5/kittycad/models/point_e_metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-Q = TypeVar("Q", bound="PointEMetadata")
+WJ = TypeVar("WJ", bound="PointEMetadata")
 
 
 @attr.s(auto_attribs=True)
 class PointEMetadata:
     """Metadata about our point-e instance.
 
     This is mostly used for internal purposes and debugging."""  # noqa: E501
@@ -25,15 +25,15 @@
         field_dict.update({})
         if ok is not UNSET:
             field_dict["ok"] = ok
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[Q], src_dict: Dict[str, Any]) -> Q:
+    def from_dict(cls: Type[WJ], src_dict: Dict[str, Any]) -> WJ:
         d = src_dict.copy()
         ok = d.pop("ok", UNSET)
 
         point_e_metadata = cls(
             ok=ok,
         )
```

### Comparing `kittycad-0.4.4/kittycad/models/pong.py` & `kittycad-0.4.5/kittycad/models/pong.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-F = TypeVar("F", bound="Pong")
+TR = TypeVar("TR", bound="Pong")
 
 
 @attr.s(auto_attribs=True)
 class Pong:
     """The response from the `/ping` endpoint."""  # noqa: E501
 
     message: Union[Unset, str] = UNSET
@@ -23,15 +23,15 @@
         field_dict.update({})
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
+    def from_dict(cls: Type[TR], src_dict: Dict[str, Any]) -> TR:
         d = src_dict.copy()
         message = d.pop("message", UNSET)
 
         pong = cls(
             message=message,
         )
```

### Comparing `kittycad-0.4.4/kittycad/models/registry_service_config.py` & `kittycad-0.4.5/kittycad/models/registry_service_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
-D = TypeVar("D", bound="RegistryServiceConfig")
+YD = TypeVar("YD", bound="RegistryServiceConfig")
 
 
 @attr.s(auto_attribs=True)
 class RegistryServiceConfig:
     """RegistryServiceConfig stores daemon registry services configuration."""  # noqa: E501
 
     allow_nondistributable_artifacts_cid_rs: Union[Unset, List[str]] = UNSET
@@ -55,15 +55,15 @@
             field_dict["insecure_registry_cid_rs"] = insecure_registry_cid_rs
         if mirrors is not UNSET:
             field_dict["mirrors"] = mirrors
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[D], src_dict: Dict[str, Any]) -> D:
+    def from_dict(cls: Type[YD], src_dict: Dict[str, Any]) -> YD:
         d = src_dict.copy()
         allow_nondistributable_artifacts_cid_rs = cast(
             List[str], d.pop("allow_nondistributable_artifacts_cid_rs", UNSET)
         )
 
         allow_nondistributable_artifacts_hostnames = cast(
             List[str], d.pop("allow_nondistributable_artifacts_hostnames", UNSET)
```

### Comparing `kittycad-0.4.4/kittycad/models/runtime.py` & `kittycad-0.4.5/kittycad/models/runtime.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
-J = TypeVar("J", bound="Runtime")
+JF = TypeVar("JF", bound="Runtime")
 
 
 @attr.s(auto_attribs=True)
 class Runtime:
     """Runtime describes an [OCI compliant](https://github.com/opencontainers/runtime-spec) runtime.  The runtime is invoked by the daemon via the `containerd` daemon. OCI runtimes act as an interface to the Linux kernel namespaces, cgroups, and SELinux."""  # noqa: E501
 
     path: Union[Unset, str] = UNSET
@@ -29,15 +29,15 @@
             field_dict["path"] = path
         if runtime_args is not UNSET:
             field_dict["runtime_args"] = runtime_args
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[J], src_dict: Dict[str, Any]) -> J:
+    def from_dict(cls: Type[JF], src_dict: Dict[str, Any]) -> JF:
         d = src_dict.copy()
         path = d.pop("path", UNSET)
 
         runtime_args = cast(List[str], d.pop("runtime_args", UNSET))
 
         runtime = cls(
             path=path,
```

### Comparing `kittycad-0.4.4/kittycad/models/session.py` & `kittycad-0.4.5/kittycad/models/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-F = TypeVar("F", bound="Session")
+VP = TypeVar("VP", bound="Session")
 
 
 @attr.s(auto_attribs=True)
 class Session:
     """An authentication session.
 
     For our UIs, these are automatically created by Next.js."""  # noqa: E501
@@ -54,15 +54,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
+    def from_dict(cls: Type[VP], src_dict: Dict[str, Any]) -> VP:
         d = src_dict.copy()
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
@@ -77,15 +77,15 @@
         id = d.pop("id", UNSET)
 
         _session_token = d.pop("session_token", UNSET)
         session_token: Union[Unset, Uuid]
         if isinstance(_session_token, Unset):
             session_token = UNSET
         else:
-            session_token = Uuid(_session_token)
+            session_token = _session_token  # type: ignore[arg-type]
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
```

### Comparing `kittycad-0.4.4/kittycad/models/storage.py` & `kittycad-0.4.5/kittycad/models/storage.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.4/kittycad/models/system.py` & `kittycad-0.4.5/kittycad/models/system.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.axis_direction_pair import AxisDirectionPair
 from ..types import UNSET, Unset
 
-V = TypeVar("V", bound="System")
+EL = TypeVar("EL", bound="System")
 
 
 @attr.s(auto_attribs=True)
 class System:
     """Co-ordinate system definition.
 
     The `up` axis must be orthogonal to the `forward` axis.
 
     See [cglearn.eu] for background reading.
 
-    [cglearn.eu](https://cglearn.eu/pub/computer-graphics/introduction-to-geometry#material-coordinate-systems-1)"""  # noqa: E501
+    [cglearn.eu](https://cglearn.eu/pub/computer-graphics/introduction-to-geometry#material-coordinate-systems-1)
+    """  # noqa: E501
 
     forward: Union[Unset, AxisDirectionPair] = UNSET
     up: Union[Unset, AxisDirectionPair] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
@@ -36,29 +37,29 @@
             field_dict["forward"] = forward
         if up is not UNSET:
             field_dict["up"] = up
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[V], src_dict: Dict[str, Any]) -> V:
+    def from_dict(cls: Type[EL], src_dict: Dict[str, Any]) -> EL:
         d = src_dict.copy()
         _forward = d.pop("forward", UNSET)
         forward: Union[Unset, AxisDirectionPair]
         if isinstance(_forward, Unset):
             forward = UNSET
         else:
-            forward = AxisDirectionPair(_forward)
+            forward = _forward  # type: ignore[arg-type]
 
         _up = d.pop("up", UNSET)
         up: Union[Unset, AxisDirectionPair]
         if isinstance(_up, Unset):
             up = UNSET
         else:
-            up = AxisDirectionPair(_up)
+            up = _up  # type: ignore[arg-type]
 
         system = cls(
             forward=forward,
             up=up,
         )
 
         system.additional_properties = d
```

### Comparing `kittycad-0.4.4/kittycad/models/system_info_default_address_pools.py` & `kittycad-0.4.5/kittycad/models/system_info_default_address_pools.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-U = TypeVar("U", bound="SystemInfoDefaultAddressPools")
+ZG = TypeVar("ZG", bound="SystemInfoDefaultAddressPools")
 
 
 @attr.s(auto_attribs=True)
 class SystemInfoDefaultAddressPools:
     base: Union[Unset, str] = UNSET
     size: Union[Unset, int] = UNSET
 
@@ -25,15 +25,15 @@
             field_dict["base"] = base
         if size is not UNSET:
             field_dict["size"] = size
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[U], src_dict: Dict[str, Any]) -> U:
+    def from_dict(cls: Type[ZG], src_dict: Dict[str, Any]) -> ZG:
         d = src_dict.copy()
         base = d.pop("base", UNSET)
 
         size = d.pop("size", UNSET)
 
         system_info_default_address_pools = cls(
             base=base,
```

### Comparing `kittycad-0.4.4/kittycad/models/unit_angle_conversion.py` & `kittycad-0.4.5/kittycad/models/unit_energy_conversion.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_angle import UnitAngle
+from ..models.unit_energy import UnitEnergy
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-F = TypeVar("F", bound="UnitAngleConversion")
+GD = TypeVar("GD", bound="UnitEnergyConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitAngleConversion:
+class UnitEnergyConversion:
     """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
-    input_unit: Union[Unset, UnitAngle] = UNSET
+    input_unit: Union[Unset, UnitEnergy] = UNSET
     output: Union[Unset, float] = UNSET
-    output_unit: Union[Unset, UnitAngle] = UNSET
+    output_unit: Union[Unset, UnitEnergy] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -83,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
+    def from_dict(cls: Type[GD], src_dict: Dict[str, Any]) -> GD:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -106,29 +106,29 @@
         error = d.pop("error", UNSET)
 
         _id = d.pop("id", UNSET)
         id: Union[Unset, Uuid]
         if isinstance(_id, Unset):
             id = UNSET
         else:
-            id = Uuid(_id)
+            id = _id  # type: ignore[arg-type]
 
         input = d.pop("input", UNSET)
 
         _input_unit = d.pop("input_unit", UNSET)
-        input_unit: Union[Unset, UnitAngle]
+        input_unit: Union[Unset, UnitEnergy]
         if isinstance(_input_unit, Unset):
             input_unit = UNSET
         else:
             input_unit = _input_unit  # type: ignore[arg-type]
 
         output = d.pop("output", UNSET)
 
         _output_unit = d.pop("output_unit", UNSET)
-        output_unit: Union[Unset, UnitAngle]
+        output_unit: Union[Unset, UnitEnergy]
         if isinstance(_output_unit, Unset):
             output_unit = UNSET
         else:
             output_unit = _output_unit  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
@@ -149,31 +149,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_angle_conversion = cls(
+        unit_energy_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             input_unit=input_unit,
             output=output,
             output_unit=output_unit,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_angle_conversion.additional_properties = d
-        return unit_angle_conversion
+        unit_energy_conversion.additional_properties = d
+        return unit_energy_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.4/kittycad/models/unit_area.py` & `kittycad-0.4.5/kittycad/models/unit_area.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,25 @@
 from enum import Enum
 
 
 class UnitArea(str, Enum):
     """The valid types of area units."""  # noqa: E501
 
-    """# Acres <https://en.wikipedia.org/wiki/Acre> """  # noqa: E501
-    ACRES = "acres"
-    """# Hectares <https://en.wikipedia.org/wiki/Hectare> """  # noqa: E501
-    HECTARES = "hectares"
     """# Square centimetres <https://en.wikipedia.org/wiki/Square_centimetre> """  # noqa: E501
-    SQUARE_CENTIMETRES = "square_centimetres"
+    CM2 = "cm2"
     """# Square decimetres <https://en.wikipedia.org/wiki/Square_decimetre> """  # noqa: E501
-    SQUARE_DECIMETRES = "square_decimetres"
+    DM2 = "dm2"
     """# Square feet <https://en.wikipedia.org/wiki/Square_foot> """  # noqa: E501
-    SQUARE_FEET = "square_feet"
-    """# Square hectometres <https://en.wikipedia.org/wiki/Square_hectometre> """  # noqa: E501
-    SQUARE_HECTOMETRES = "square_hectometres"
+    FT2 = "ft2"
     """# Square inches <https://en.wikipedia.org/wiki/Square_inch> """  # noqa: E501
-    SQUARE_INCHES = "square_inches"
+    IN2 = "in2"
     """# Square kilometres <https://en.wikipedia.org/wiki/Square_kilometre> """  # noqa: E501
-    SQUARE_KILOMETRES = "square_kilometres"
+    KM2 = "km2"
     """# Square metres <https://en.wikipedia.org/wiki/Square_metre> """  # noqa: E501
-    SQUARE_METRES = "square_metres"
-    """# Square micrometres <https://en.wikipedia.org/wiki/Square_micrometre> """  # noqa: E501
-    SQUARE_MICROMETRES = "square_micrometres"
-    """# Square miles <https://en.wikipedia.org/wiki/Square_mile> """  # noqa: E501
-    SQUARE_MILES = "square_miles"
+    M2 = "m2"
     """# Square millimetres <https://en.wikipedia.org/wiki/Square_millimetre> """  # noqa: E501
-    SQUARE_MILLIMETRES = "square_millimetres"
-    """# Square nanometres <https://en.wikipedia.org/wiki/Square_nanometre> """  # noqa: E501
-    SQUARE_NANOMETRES = "square_nanometres"
+    MM2 = "mm2"
     """# Square yards <https://en.wikipedia.org/wiki/Square_mile> """  # noqa: E501
-    SQUARE_YARDS = "square_yards"
+    YD2 = "yd2"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `kittycad-0.4.4/kittycad/models/unit_area_conversion.py` & `kittycad-0.4.5/kittycad/models/unit_current_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_area import UnitArea
+from ..models.unit_current import UnitCurrent
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-Y = TypeVar("Y", bound="UnitAreaConversion")
+GN = TypeVar("GN", bound="UnitCurrentConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitAreaConversion:
+class UnitCurrentConversion:
     """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
-    input_unit: Union[Unset, UnitArea] = UNSET
+    input_unit: Union[Unset, UnitCurrent] = UNSET
     output: Union[Unset, float] = UNSET
-    output_unit: Union[Unset, UnitArea] = UNSET
+    output_unit: Union[Unset, UnitCurrent] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -83,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[Y], src_dict: Dict[str, Any]) -> Y:
+    def from_dict(cls: Type[GN], src_dict: Dict[str, Any]) -> GN:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -106,29 +106,29 @@
         error = d.pop("error", UNSET)
 
         _id = d.pop("id", UNSET)
         id: Union[Unset, Uuid]
         if isinstance(_id, Unset):
             id = UNSET
         else:
-            id = Uuid(_id)
+            id = _id  # type: ignore[arg-type]
 
         input = d.pop("input", UNSET)
 
         _input_unit = d.pop("input_unit", UNSET)
-        input_unit: Union[Unset, UnitArea]
+        input_unit: Union[Unset, UnitCurrent]
         if isinstance(_input_unit, Unset):
             input_unit = UNSET
         else:
             input_unit = _input_unit  # type: ignore[arg-type]
 
         output = d.pop("output", UNSET)
 
         _output_unit = d.pop("output_unit", UNSET)
-        output_unit: Union[Unset, UnitArea]
+        output_unit: Union[Unset, UnitCurrent]
         if isinstance(_output_unit, Unset):
             output_unit = UNSET
         else:
             output_unit = _output_unit  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
@@ -149,31 +149,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_area_conversion = cls(
+        unit_current_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             input_unit=input_unit,
             output=output,
             output_unit=output_unit,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_area_conversion.additional_properties = d
-        return unit_area_conversion
+        unit_current_conversion.additional_properties = d
+        return unit_current_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.4/kittycad/models/unit_current.py` & `kittycad-0.4.5/kittycad/models/unit_current.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.4/kittycad/models/unit_current_conversion.py` & `kittycad-0.4.5/kittycad/models/unit_mass_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_current import UnitCurrent
+from ..models.unit_mass import UnitMass
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-F = TypeVar("F", bound="UnitCurrentConversion")
+QX = TypeVar("QX", bound="UnitMassConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitCurrentConversion:
+class UnitMassConversion:
     """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
-    input_unit: Union[Unset, UnitCurrent] = UNSET
+    input_unit: Union[Unset, UnitMass] = UNSET
     output: Union[Unset, float] = UNSET
-    output_unit: Union[Unset, UnitCurrent] = UNSET
+    output_unit: Union[Unset, UnitMass] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -83,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
+    def from_dict(cls: Type[QX], src_dict: Dict[str, Any]) -> QX:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -106,29 +106,29 @@
         error = d.pop("error", UNSET)
 
         _id = d.pop("id", UNSET)
         id: Union[Unset, Uuid]
         if isinstance(_id, Unset):
             id = UNSET
         else:
-            id = Uuid(_id)
+            id = _id  # type: ignore[arg-type]
 
         input = d.pop("input", UNSET)
 
         _input_unit = d.pop("input_unit", UNSET)
-        input_unit: Union[Unset, UnitCurrent]
+        input_unit: Union[Unset, UnitMass]
         if isinstance(_input_unit, Unset):
             input_unit = UNSET
         else:
             input_unit = _input_unit  # type: ignore[arg-type]
 
         output = d.pop("output", UNSET)
 
         _output_unit = d.pop("output_unit", UNSET)
-        output_unit: Union[Unset, UnitCurrent]
+        output_unit: Union[Unset, UnitMass]
         if isinstance(_output_unit, Unset):
             output_unit = UNSET
         else:
             output_unit = _output_unit  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
@@ -149,31 +149,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_current_conversion = cls(
+        unit_mass_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             input_unit=input_unit,
             output=output,
             output_unit=output_unit,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_current_conversion.additional_properties = d
-        return unit_current_conversion
+        unit_mass_conversion.additional_properties = d
+        return unit_mass_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.4/kittycad/models/unit_energy.py` & `kittycad-0.4.5/kittycad/models/unit_energy.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.4/kittycad/models/unit_energy_conversion.py` & `kittycad-0.4.5/kittycad/models/unit_length_conversion.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_energy import UnitEnergy
+from ..models.unit_length import UnitLength
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-P = TypeVar("P", bound="UnitEnergyConversion")
+YW = TypeVar("YW", bound="UnitLengthConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitEnergyConversion:
+class UnitLengthConversion:
     """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
-    input_unit: Union[Unset, UnitEnergy] = UNSET
+    input_unit: Union[Unset, UnitLength] = UNSET
     output: Union[Unset, float] = UNSET
-    output_unit: Union[Unset, UnitEnergy] = UNSET
+    output_unit: Union[Unset, UnitLength] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -83,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[P], src_dict: Dict[str, Any]) -> P:
+    def from_dict(cls: Type[YW], src_dict: Dict[str, Any]) -> YW:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -106,29 +106,29 @@
         error = d.pop("error", UNSET)
 
         _id = d.pop("id", UNSET)
         id: Union[Unset, Uuid]
         if isinstance(_id, Unset):
             id = UNSET
         else:
-            id = Uuid(_id)
+            id = _id  # type: ignore[arg-type]
 
         input = d.pop("input", UNSET)
 
         _input_unit = d.pop("input_unit", UNSET)
-        input_unit: Union[Unset, UnitEnergy]
+        input_unit: Union[Unset, UnitLength]
         if isinstance(_input_unit, Unset):
             input_unit = UNSET
         else:
             input_unit = _input_unit  # type: ignore[arg-type]
 
         output = d.pop("output", UNSET)
 
         _output_unit = d.pop("output_unit", UNSET)
-        output_unit: Union[Unset, UnitEnergy]
+        output_unit: Union[Unset, UnitLength]
         if isinstance(_output_unit, Unset):
             output_unit = UNSET
         else:
             output_unit = _output_unit  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
@@ -149,31 +149,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_energy_conversion = cls(
+        unit_length_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             input_unit=input_unit,
             output=output,
             output_unit=output_unit,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_energy_conversion.additional_properties = d
-        return unit_energy_conversion
+        unit_length_conversion.additional_properties = d
+        return unit_length_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.4/kittycad/models/unit_force.py` & `kittycad-0.4.5/kittycad/models/unit_force.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.4/kittycad/models/unit_force_conversion.py` & `kittycad-0.4.5/kittycad/models/unit_force_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.unit_force import UnitForce
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-Y = TypeVar("Y", bound="UnitForceConversion")
+VJ = TypeVar("VJ", bound="UnitForceConversion")
 
 
 @attr.s(auto_attribs=True)
 class UnitForceConversion:
     """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
@@ -83,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[Y], src_dict: Dict[str, Any]) -> Y:
+    def from_dict(cls: Type[VJ], src_dict: Dict[str, Any]) -> VJ:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -106,15 +106,15 @@
         error = d.pop("error", UNSET)
 
         _id = d.pop("id", UNSET)
         id: Union[Unset, Uuid]
         if isinstance(_id, Unset):
             id = UNSET
         else:
-            id = Uuid(_id)
+            id = _id  # type: ignore[arg-type]
 
         input = d.pop("input", UNSET)
 
         _input_unit = d.pop("input_unit", UNSET)
         input_unit: Union[Unset, UnitForce]
         if isinstance(_input_unit, Unset):
             input_unit = UNSET
```

### Comparing `kittycad-0.4.4/kittycad/models/unit_frequency.py` & `kittycad-0.4.5/kittycad/models/unit_frequency.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.4/kittycad/models/unit_frequency_conversion.py` & `kittycad-0.4.5/kittycad/models/unit_frequency_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.unit_frequency import UnitFrequency
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-L = TypeVar("L", bound="UnitFrequencyConversion")
+OX = TypeVar("OX", bound="UnitFrequencyConversion")
 
 
 @attr.s(auto_attribs=True)
 class UnitFrequencyConversion:
     """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
@@ -83,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
+    def from_dict(cls: Type[OX], src_dict: Dict[str, Any]) -> OX:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -106,15 +106,15 @@
         error = d.pop("error", UNSET)
 
         _id = d.pop("id", UNSET)
         id: Union[Unset, Uuid]
         if isinstance(_id, Unset):
             id = UNSET
         else:
-            id = Uuid(_id)
+            id = _id  # type: ignore[arg-type]
 
         input = d.pop("input", UNSET)
 
         _input_unit = d.pop("input_unit", UNSET)
         input_unit: Union[Unset, UnitFrequency]
         if isinstance(_input_unit, Unset):
             input_unit = UNSET
```

### Comparing `kittycad-0.4.4/kittycad/models/unit_length.py` & `kittycad-0.4.5/kittycad/models/unit_pressure.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,23 @@
 from enum import Enum
 
 
-class UnitLength(str, Enum):
-    """The valid types of length units."""  # noqa: E501
+class UnitPressure(str, Enum):
+    """The valid types of pressure units."""  # noqa: E501
 
-    """# Centimetres <https://en.wikipedia.org/wiki/Centimetre> """  # noqa: E501
-    CENTIMETRES = "centimetres"
-    """# Decimetres <https://en.wikipedia.org/wiki/Decimetre> """  # noqa: E501
-    DECIMETRES = "decimetres"
-    """# Feet <https://en.wikipedia.org/wiki/Foot_(unit)> """  # noqa: E501
-    FEET = "feet"
-    """# Furlongs <https://en.wikipedia.org/wiki/Furlong> """  # noqa: E501
-    FURLONGS = "furlongs"
-    """# Hectometres <https://en.wikipedia.org/wiki/Hectometre> """  # noqa: E501
-    HECTOMETRES = "hectometres"
-    """# Inches <https://en.wikipedia.org/wiki/Inch> """  # noqa: E501
-    INCHES = "inches"
-    """# Kilometres <https://en.wikipedia.org/wiki/Kilometre> """  # noqa: E501
-    KILOMETRES = "kilometres"
-    """# Metres <https://en.wikipedia.org/wiki/Metre> """  # noqa: E501
-    METRES = "metres"
-    """# Micrometres <https://en.wikipedia.org/wiki/Micrometre> """  # noqa: E501
-    MICROMETRES = "micrometres"
-    """# Miles <https://en.wikipedia.org/wiki/Mile> """  # noqa: E501
-    MILES = "miles"
-    """# Millimetres <https://en.wikipedia.org/wiki/Millimetre> """  # noqa: E501
-    MILLIMETRES = "millimetres"
-    """# Nanometres <https://en.wikipedia.org/wiki/Nanometre> """  # noqa: E501
-    NANOMETRES = "nanometres"
-    """# Yards <https://en.wikipedia.org/wiki/Yard> """  # noqa: E501
-    YARDS = "yards"
+    """# Atmospheres <https://en.wikipedia.org/wiki/Standard_atmosphere_(unit)> """  # noqa: E501
+    ATMOSPHERES = "atmospheres"
+    """# Bars <https://en.wikipedia.org/wiki/Bar_(unit)> """  # noqa: E501
+    BARS = "bars"
+    """# Hectopascals <https://en.wikipedia.org/wiki/Hectopascal> """  # noqa: E501
+    HECTOPASCALS = "hectopascals"
+    """# Kilopascals <https://en.wikipedia.org/wiki/Kilopascal> """  # noqa: E501
+    KILOPASCALS = "kilopascals"
+    """# Millibars <https://en.wikipedia.org/wiki/Bar_(unit)> """  # noqa: E501
+    MILLIBARS = "millibars"
+    """# Pascals <https://en.wikipedia.org/wiki/Pascal_(unit)> """  # noqa: E501
+    PASCALS = "pascals"
+    """# Pounds per square inch (PSI) - <https://en.wikipedia.org/wiki/Pound_per_square_inch> """  # noqa: E501
+    PSI = "psi"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `kittycad-0.4.4/kittycad/models/unit_length_conversion.py` & `kittycad-0.4.5/kittycad/models/unit_volume_conversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_length import UnitLength
+from ..models.unit_volume import UnitVolume
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-K = TypeVar("K", bound="UnitLengthConversion")
+LD = TypeVar("LD", bound="UnitVolumeConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitLengthConversion:
+class UnitVolumeConversion:
     """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
-    input_unit: Union[Unset, UnitLength] = UNSET
+    input_unit: Union[Unset, UnitVolume] = UNSET
     output: Union[Unset, float] = UNSET
-    output_unit: Union[Unset, UnitLength] = UNSET
+    output_unit: Union[Unset, UnitVolume] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -83,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[K], src_dict: Dict[str, Any]) -> K:
+    def from_dict(cls: Type[LD], src_dict: Dict[str, Any]) -> LD:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -106,29 +106,29 @@
         error = d.pop("error", UNSET)
 
         _id = d.pop("id", UNSET)
         id: Union[Unset, Uuid]
         if isinstance(_id, Unset):
             id = UNSET
         else:
-            id = Uuid(_id)
+            id = _id  # type: ignore[arg-type]
 
         input = d.pop("input", UNSET)
 
         _input_unit = d.pop("input_unit", UNSET)
-        input_unit: Union[Unset, UnitLength]
+        input_unit: Union[Unset, UnitVolume]
         if isinstance(_input_unit, Unset):
             input_unit = UNSET
         else:
             input_unit = _input_unit  # type: ignore[arg-type]
 
         output = d.pop("output", UNSET)
 
         _output_unit = d.pop("output_unit", UNSET)
-        output_unit: Union[Unset, UnitLength]
+        output_unit: Union[Unset, UnitVolume]
         if isinstance(_output_unit, Unset):
             output_unit = UNSET
         else:
             output_unit = _output_unit  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
@@ -149,31 +149,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_length_conversion = cls(
+        unit_volume_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             input_unit=input_unit,
             output=output,
             output_unit=output_unit,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_length_conversion.additional_properties = d
-        return unit_length_conversion
+        unit_volume_conversion.additional_properties = d
+        return unit_volume_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.4/kittycad/models/unit_mass.py` & `kittycad-0.4.5/kittycad/models/unit_volume.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,27 @@
 from enum import Enum
 
 
-class UnitMass(str, Enum):
-    """The valid types of mass units."""  # noqa: E501
+class UnitVolume(str, Enum):
+    """The valid types of volume units."""  # noqa: E501
 
-    """# Carats <https://en.wikipedia.org/wiki/Carat_(mass)> """  # noqa: E501
-    CARATS = "carats"
-    """# Grains <https://en.wikipedia.org/wiki/Grain_(unit)> """  # noqa: E501
-    GRAINS = "grains"
-    """# Grams <https://en.wikipedia.org/wiki/Gram> """  # noqa: E501
-    GRAMS = "grams"
-    """# Kilograms <https://en.wikipedia.org/wiki/Kilogram> """  # noqa: E501
-    KILOGRAMS = "kilograms"
-    """# Long tons <https://en.wikipedia.org/wiki/Long_ton> """  # noqa: E501
-    LONG_TONS = "long_tons"
-    """# Metric tons <https://en.wikipedia.org/wiki/Tonne> """  # noqa: E501
-    METRIC_TONS = "metric_tons"
-    """# Micrograms <https://en.wikipedia.org/wiki/Microgram> """  # noqa: E501
-    MICROGRAMS = "micrograms"
-    """# Milligrams <https://en.wikipedia.org/wiki/Milligram> """  # noqa: E501
-    MILLIGRAMS = "milligrams"
-    """# Ounces <https://en.wikipedia.org/wiki/Ounce> """  # noqa: E501
-    OUNCES = "ounces"
-    """# Pennyweights <https://en.wikipedia.org/wiki/Pennyweight> """  # noqa: E501
-    PENNYWEIGHTS = "pennyweights"
-    """# Pounds <https://en.wikipedia.org/wiki/Pound_(mass)> """  # noqa: E501
-    POUNDS = "pounds"
-    """# Short tons <https://en.wikipedia.org/wiki/Short_ton> """  # noqa: E501
-    SHORT_TONS = "short_tons"
-    """# Stones <https://en.wikipedia.org/wiki/Stone_(unit)> """  # noqa: E501
-    STONES = "stones"
-    """# Troy ounces <https://en.wikipedia.org/wiki/Troy_ounce> """  # noqa: E501
-    TROY_OUNCES = "troy_ounces"
-    """# Troy pounds <https://en.wikipedia.org/wiki/Troy_pound> """  # noqa: E501
-    TROY_POUNDS = "troy_pounds"
+    """# Cubic centimetres (cc or cm³) <https://en.wikipedia.org/wiki/Cubic_centimetre> """  # noqa: E501
+    CM3 = "cm3"
+    """# Cubic feet (ft³) <https://en.wikipedia.org/wiki/Cubic_foot> """  # noqa: E501
+    FT3 = "ft3"
+    """# Cubic inches (cu in or in³) <https://en.wikipedia.org/wiki/Cubic_inch> """  # noqa: E501
+    IN3 = "in3"
+    """# Cubic metres (m³) <https://en.wikipedia.org/wiki/Cubic_metre> """  # noqa: E501
+    M3 = "m3"
+    """# Cubic yards (yd³) <https://en.wikipedia.org/wiki/Cubic_yard> """  # noqa: E501
+    YD3 = "yd3"
+    """# US Fluid Ounces (fl oz) <https://en.wikipedia.org/wiki/Fluid_ounce> """  # noqa: E501
+    USFLOZ = "usfloz"
+    """# US Gallons (gal US) <https://en.wikipedia.org/wiki/Gallon> """  # noqa: E501
+    USGAL = "usgal"
+    """# Liters (l) <https://en.wikipedia.org/wiki/Litre> """  # noqa: E501
+    L = "l"
+    """# Milliliters (ml) <https://en.wikipedia.org/wiki/Litre> """  # noqa: E501
+    ML = "ml"
 
     def __str__(self) -> str:
         return str(self.value)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `kittycad-0.4.4/kittycad/models/unit_mass_conversion.py` & `kittycad-0.4.5/kittycad/models/unit_pressure_conversion.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_mass import UnitMass
+from ..models.unit_pressure import UnitPressure
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-N = TypeVar("N", bound="UnitMassConversion")
+VX = TypeVar("VX", bound="UnitPressureConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitMassConversion:
+class UnitPressureConversion:
     """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
-    input_unit: Union[Unset, UnitMass] = UNSET
+    input_unit: Union[Unset, UnitPressure] = UNSET
     output: Union[Unset, float] = UNSET
-    output_unit: Union[Unset, UnitMass] = UNSET
+    output_unit: Union[Unset, UnitPressure] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -83,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
+    def from_dict(cls: Type[VX], src_dict: Dict[str, Any]) -> VX:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -106,29 +106,29 @@
         error = d.pop("error", UNSET)
 
         _id = d.pop("id", UNSET)
         id: Union[Unset, Uuid]
         if isinstance(_id, Unset):
             id = UNSET
         else:
-            id = Uuid(_id)
+            id = _id  # type: ignore[arg-type]
 
         input = d.pop("input", UNSET)
 
         _input_unit = d.pop("input_unit", UNSET)
-        input_unit: Union[Unset, UnitMass]
+        input_unit: Union[Unset, UnitPressure]
         if isinstance(_input_unit, Unset):
             input_unit = UNSET
         else:
             input_unit = _input_unit  # type: ignore[arg-type]
 
         output = d.pop("output", UNSET)
 
         _output_unit = d.pop("output_unit", UNSET)
-        output_unit: Union[Unset, UnitMass]
+        output_unit: Union[Unset, UnitPressure]
         if isinstance(_output_unit, Unset):
             output_unit = UNSET
         else:
             output_unit = _output_unit  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
@@ -149,31 +149,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_mass_conversion = cls(
+        unit_pressure_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             input_unit=input_unit,
             output=output,
             output_unit=output_unit,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_mass_conversion.additional_properties = d
-        return unit_mass_conversion
+        unit_pressure_conversion.additional_properties = d
+        return unit_pressure_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.4/kittycad/models/unit_power.py` & `kittycad-0.4.5/kittycad/models/unit_power.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.4/kittycad/models/unit_power_conversion.py` & `kittycad-0.4.5/kittycad/models/unit_temperature_conversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_power import UnitPower
+from ..models.unit_temperature import UnitTemperature
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-H = TypeVar("H", bound="UnitPowerConversion")
+RG = TypeVar("RG", bound="UnitTemperatureConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitPowerConversion:
+class UnitTemperatureConversion:
     """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
-    input_unit: Union[Unset, UnitPower] = UNSET
+    input_unit: Union[Unset, UnitTemperature] = UNSET
     output: Union[Unset, float] = UNSET
-    output_unit: Union[Unset, UnitPower] = UNSET
+    output_unit: Union[Unset, UnitTemperature] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -83,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
+    def from_dict(cls: Type[RG], src_dict: Dict[str, Any]) -> RG:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -106,29 +106,29 @@
         error = d.pop("error", UNSET)
 
         _id = d.pop("id", UNSET)
         id: Union[Unset, Uuid]
         if isinstance(_id, Unset):
             id = UNSET
         else:
-            id = Uuid(_id)
+            id = _id  # type: ignore[arg-type]
 
         input = d.pop("input", UNSET)
 
         _input_unit = d.pop("input_unit", UNSET)
-        input_unit: Union[Unset, UnitPower]
+        input_unit: Union[Unset, UnitTemperature]
         if isinstance(_input_unit, Unset):
             input_unit = UNSET
         else:
             input_unit = _input_unit  # type: ignore[arg-type]
 
         output = d.pop("output", UNSET)
 
         _output_unit = d.pop("output_unit", UNSET)
-        output_unit: Union[Unset, UnitPower]
+        output_unit: Union[Unset, UnitTemperature]
         if isinstance(_output_unit, Unset):
             output_unit = UNSET
         else:
             output_unit = _output_unit  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
@@ -149,31 +149,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_power_conversion = cls(
+        unit_temperature_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             input_unit=input_unit,
             output=output,
             output_unit=output_unit,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_power_conversion.additional_properties = d
-        return unit_power_conversion
+        unit_temperature_conversion.additional_properties = d
+        return unit_temperature_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.4/kittycad/models/unit_pressure.py` & `kittycad-0.4.5/kittycad/models/unit_length.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from enum import Enum
 
 
-class UnitPressure(str, Enum):
-    """The valid types of pressure units."""  # noqa: E501
+class UnitLength(str, Enum):
+    """The valid types of length units."""  # noqa: E501
 
-    """# Atmospheres <https://en.wikipedia.org/wiki/Standard_atmosphere_(unit)> """  # noqa: E501
-    ATMOSPHERES = "atmospheres"
-    """# Bars <https://en.wikipedia.org/wiki/Bar_(unit)> """  # noqa: E501
-    BARS = "bars"
-    """# Hectopascals <https://en.wikipedia.org/wiki/Hectopascal> """  # noqa: E501
-    HECTOPASCALS = "hectopascals"
-    """# Kilopascals <https://en.wikipedia.org/wiki/Kilopascal> """  # noqa: E501
-    KILOPASCALS = "kilopascals"
-    """# Millibars <https://en.wikipedia.org/wiki/Bar_(unit)> """  # noqa: E501
-    MILLIBARS = "millibars"
-    """# Pascals <https://en.wikipedia.org/wiki/Pascal_(unit)> """  # noqa: E501
-    PASCALS = "pascals"
-    """# Pounds per square inch (PSI) - <https://en.wikipedia.org/wiki/Pound_per_square_inch> """  # noqa: E501
-    PSI = "psi"
+    """# Centimetres <https://en.wikipedia.org/wiki/Centimetre> """  # noqa: E501
+    CM = "cm"
+    """# Feet <https://en.wikipedia.org/wiki/Foot_(unit)> """  # noqa: E501
+    FT = "ft"
+    """# Inches <https://en.wikipedia.org/wiki/Inch> """  # noqa: E501
+    IN = "in"
+    """# Metres <https://en.wikipedia.org/wiki/Metre> """  # noqa: E501
+    M = "m"
+    """# Millimetres <https://en.wikipedia.org/wiki/Millimetre> """  # noqa: E501
+    MM = "mm"
+    """# Yards <https://en.wikipedia.org/wiki/Yard> """  # noqa: E501
+    YD = "yd"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `kittycad-0.4.4/kittycad/models/unit_pressure_conversion.py` & `kittycad-0.4.5/kittycad/models/file_surface_area.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,60 +1,61 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_pressure import UnitPressure
+from ..models.file_import_format import FileImportFormat
+from ..models.unit_area import UnitArea
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-A = TypeVar("A", bound="UnitPressureConversion")
+FZ = TypeVar("FZ", bound="FileSurfaceArea")
 
 
 @attr.s(auto_attribs=True)
-class UnitPressureConversion:
-    """Result of converting between units."""  # noqa: E501
+class FileSurfaceArea:
+    """A file surface area result."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
-    input: Union[Unset, float] = UNSET
-    input_unit: Union[Unset, UnitPressure] = UNSET
-    output: Union[Unset, float] = UNSET
-    output_unit: Union[Unset, UnitPressure] = UNSET
+    output_unit: Union[Unset, UnitArea] = UNSET
+    src_format: Union[Unset, FileImportFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
+    surface_area: Union[Unset, float] = UNSET
+    surface_areas: Union[Unset, Any] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         completed_at: Union[Unset, str] = UNSET
         if not isinstance(self.completed_at, Unset):
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
-        input = self.input
-        if not isinstance(self.input_unit, Unset):
-            input_unit = self.input_unit
-        output = self.output
         if not isinstance(self.output_unit, Unset):
             output_unit = self.output_unit
+        if not isinstance(self.src_format, Unset):
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
         if not isinstance(self.status, Unset):
             status = self.status
+        surface_area = self.surface_area
+        surface_areas = self.surface_areas
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
@@ -63,35 +64,35 @@
             field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
             field_dict["created_at"] = created_at
         if error is not UNSET:
             field_dict["error"] = error
         if id is not UNSET:
             field_dict["id"] = id
-        if input is not UNSET:
-            field_dict["input"] = input
-        if input_unit is not UNSET:
-            field_dict["input_unit"] = input_unit
-        if output is not UNSET:
-            field_dict["output"] = output
         if output_unit is not UNSET:
             field_dict["output_unit"] = output_unit
+        if src_format is not UNSET:
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
             field_dict["started_at"] = started_at
         if status is not UNSET:
             field_dict["status"] = status
+        if surface_area is not UNSET:
+            field_dict["surface_area"] = surface_area
+        if surface_areas is not UNSET:
+            field_dict["surface_areas"] = surface_areas
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[A], src_dict: Dict[str, Any]) -> A:
+    def from_dict(cls: Type[FZ], src_dict: Dict[str, Any]) -> FZ:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -106,74 +107,73 @@
         error = d.pop("error", UNSET)
 
         _id = d.pop("id", UNSET)
         id: Union[Unset, Uuid]
         if isinstance(_id, Unset):
             id = UNSET
         else:
-            id = Uuid(_id)
-
-        input = d.pop("input", UNSET)
-
-        _input_unit = d.pop("input_unit", UNSET)
-        input_unit: Union[Unset, UnitPressure]
-        if isinstance(_input_unit, Unset):
-            input_unit = UNSET
-        else:
-            input_unit = _input_unit  # type: ignore[arg-type]
-
-        output = d.pop("output", UNSET)
+            id = _id  # type: ignore[arg-type]
 
         _output_unit = d.pop("output_unit", UNSET)
-        output_unit: Union[Unset, UnitPressure]
+        output_unit: Union[Unset, UnitArea]
         if isinstance(_output_unit, Unset):
             output_unit = UNSET
         else:
             output_unit = _output_unit  # type: ignore[arg-type]
 
+        _src_format = d.pop("src_format", UNSET)
+        src_format: Union[Unset, FileImportFormat]
+        if isinstance(_src_format, Unset):
+            src_format = UNSET
+        else:
+            src_format = _src_format  # type: ignore[arg-type]
+
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, ApiCallStatus]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = _status  # type: ignore[arg-type]
 
+        surface_area = d.pop("surface_area", UNSET)
+
+        surface_areas = d.pop("surface_areas", UNSET)
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_pressure_conversion = cls(
+        file_surface_area = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
-            input=input,
-            input_unit=input_unit,
-            output=output,
             output_unit=output_unit,
+            src_format=src_format,
             started_at=started_at,
             status=status,
+            surface_area=surface_area,
+            surface_areas=surface_areas,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_pressure_conversion.additional_properties = d
-        return unit_pressure_conversion
+        file_surface_area.additional_properties = d
+        return file_surface_area
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.4/kittycad/models/unit_temperature.py` & `kittycad-0.4.5/kittycad/models/unit_temperature.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.4/kittycad/models/unit_temperature_conversion.py` & `kittycad-0.4.5/kittycad/models/file_center_of_mass.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,98 +1,109 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_temperature import UnitTemperature
+from ..models.file_import_format import FileImportFormat
+from ..models.point3d import Point3d
+from ..models.unit_length import UnitLength
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-R = TypeVar("R", bound="UnitTemperatureConversion")
+LT = TypeVar("LT", bound="FileCenterOfMass")
 
 
 @attr.s(auto_attribs=True)
-class UnitTemperatureConversion:
-    """Result of converting between units."""  # noqa: E501
+class FileCenterOfMass:
+    """A file center of mass result."""  # noqa: E501
 
+    center_of_mass: Union[Unset, Point3d] = UNSET
+    centers_of_mass: Union[Unset, Any] = UNSET
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
-    input: Union[Unset, float] = UNSET
-    input_unit: Union[Unset, UnitTemperature] = UNSET
-    output: Union[Unset, float] = UNSET
-    output_unit: Union[Unset, UnitTemperature] = UNSET
+    output_unit: Union[Unset, UnitLength] = UNSET
+    src_format: Union[Unset, FileImportFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
+        if not isinstance(self.center_of_mass, Unset):
+            center_of_mass = self.center_of_mass
+        centers_of_mass = self.centers_of_mass
         completed_at: Union[Unset, str] = UNSET
         if not isinstance(self.completed_at, Unset):
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
-        input = self.input
-        if not isinstance(self.input_unit, Unset):
-            input_unit = self.input_unit
-        output = self.output
         if not isinstance(self.output_unit, Unset):
             output_unit = self.output_unit
+        if not isinstance(self.src_format, Unset):
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
         if not isinstance(self.status, Unset):
             status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
+        if center_of_mass is not UNSET:
+            field_dict["center_of_mass"] = center_of_mass
+        if centers_of_mass is not UNSET:
+            field_dict["centers_of_mass"] = centers_of_mass
         if completed_at is not UNSET:
             field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
             field_dict["created_at"] = created_at
         if error is not UNSET:
             field_dict["error"] = error
         if id is not UNSET:
             field_dict["id"] = id
-        if input is not UNSET:
-            field_dict["input"] = input
-        if input_unit is not UNSET:
-            field_dict["input_unit"] = input_unit
-        if output is not UNSET:
-            field_dict["output"] = output
         if output_unit is not UNSET:
             field_dict["output_unit"] = output_unit
+        if src_format is not UNSET:
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
             field_dict["started_at"] = started_at
         if status is not UNSET:
             field_dict["status"] = status
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[R], src_dict: Dict[str, Any]) -> R:
+    def from_dict(cls: Type[LT], src_dict: Dict[str, Any]) -> LT:
         d = src_dict.copy()
+        _center_of_mass = d.pop("center_of_mass", UNSET)
+        center_of_mass: Union[Unset, Point3d]
+        if isinstance(_center_of_mass, Unset):
+            center_of_mass = UNSET
+        else:
+            center_of_mass = _center_of_mass  # type: ignore[arg-type]
+
+        centers_of_mass = d.pop("centers_of_mass", UNSET)
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
 
@@ -106,34 +117,30 @@
         error = d.pop("error", UNSET)
 
         _id = d.pop("id", UNSET)
         id: Union[Unset, Uuid]
         if isinstance(_id, Unset):
             id = UNSET
         else:
-            id = Uuid(_id)
-
-        input = d.pop("input", UNSET)
-
-        _input_unit = d.pop("input_unit", UNSET)
-        input_unit: Union[Unset, UnitTemperature]
-        if isinstance(_input_unit, Unset):
-            input_unit = UNSET
-        else:
-            input_unit = _input_unit  # type: ignore[arg-type]
-
-        output = d.pop("output", UNSET)
+            id = _id  # type: ignore[arg-type]
 
         _output_unit = d.pop("output_unit", UNSET)
-        output_unit: Union[Unset, UnitTemperature]
+        output_unit: Union[Unset, UnitLength]
         if isinstance(_output_unit, Unset):
             output_unit = UNSET
         else:
             output_unit = _output_unit  # type: ignore[arg-type]
 
+        _src_format = d.pop("src_format", UNSET)
+        src_format: Union[Unset, FileImportFormat]
+        if isinstance(_src_format, Unset):
+            src_format = UNSET
+        else:
+            src_format = _src_format  # type: ignore[arg-type]
+
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
 
@@ -149,31 +156,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_temperature_conversion = cls(
+        file_center_of_mass = cls(
+            center_of_mass=center_of_mass,
+            centers_of_mass=centers_of_mass,
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
-            input=input,
-            input_unit=input_unit,
-            output=output,
             output_unit=output_unit,
+            src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_temperature_conversion.additional_properties = d
-        return unit_temperature_conversion
+        file_center_of_mass.additional_properties = d
+        return file_center_of_mass
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.4/kittycad/models/unit_torque_conversion.py` & `kittycad-0.4.5/kittycad/models/file_mass.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_torque import UnitTorque
+from ..models.file_import_format import FileImportFormat
+from ..models.unit_density import UnitDensity
+from ..models.unit_mass import UnitMass
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-W = TypeVar("W", bound="UnitTorqueConversion")
+DO = TypeVar("DO", bound="FileMass")
 
 
 @attr.s(auto_attribs=True)
-class UnitTorqueConversion:
-    """Result of converting between units."""  # noqa: E501
+class FileMass:
+    """A file mass result."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
-    input: Union[Unset, float] = UNSET
-    input_unit: Union[Unset, UnitTorque] = UNSET
-    output: Union[Unset, float] = UNSET
-    output_unit: Union[Unset, UnitTorque] = UNSET
+    mass: Union[Unset, float] = UNSET
+    masses: Union[Unset, Any] = UNSET
+    material_density: Union[Unset, float] = UNSET
+    material_density_unit: Union[Unset, UnitDensity] = UNSET
+    output_unit: Union[Unset, UnitMass] = UNSET
+    src_format: Union[Unset, FileImportFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -36,20 +40,23 @@
         if not isinstance(self.completed_at, Unset):
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
-        input = self.input
-        if not isinstance(self.input_unit, Unset):
-            input_unit = self.input_unit
-        output = self.output
+        mass = self.mass
+        masses = self.masses
+        material_density = self.material_density
+        if not isinstance(self.material_density_unit, Unset):
+            material_density_unit = self.material_density_unit
         if not isinstance(self.output_unit, Unset):
             output_unit = self.output_unit
+        if not isinstance(self.src_format, Unset):
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
         if not isinstance(self.status, Unset):
             status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
@@ -63,35 +70,39 @@
             field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
             field_dict["created_at"] = created_at
         if error is not UNSET:
             field_dict["error"] = error
         if id is not UNSET:
             field_dict["id"] = id
-        if input is not UNSET:
-            field_dict["input"] = input
-        if input_unit is not UNSET:
-            field_dict["input_unit"] = input_unit
-        if output is not UNSET:
-            field_dict["output"] = output
+        if mass is not UNSET:
+            field_dict["mass"] = mass
+        if masses is not UNSET:
+            field_dict["masses"] = masses
+        if material_density is not UNSET:
+            field_dict["material_density"] = material_density
+        if material_density_unit is not UNSET:
+            field_dict["material_density_unit"] = material_density_unit
         if output_unit is not UNSET:
             field_dict["output_unit"] = output_unit
+        if src_format is not UNSET:
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
             field_dict["started_at"] = started_at
         if status is not UNSET:
             field_dict["status"] = status
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[W], src_dict: Dict[str, Any]) -> W:
+    def from_dict(cls: Type[DO], src_dict: Dict[str, Any]) -> DO:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -106,34 +117,42 @@
         error = d.pop("error", UNSET)
 
         _id = d.pop("id", UNSET)
         id: Union[Unset, Uuid]
         if isinstance(_id, Unset):
             id = UNSET
         else:
-            id = Uuid(_id)
+            id = _id  # type: ignore[arg-type]
 
-        input = d.pop("input", UNSET)
+        mass = d.pop("mass", UNSET)
 
-        _input_unit = d.pop("input_unit", UNSET)
-        input_unit: Union[Unset, UnitTorque]
-        if isinstance(_input_unit, Unset):
-            input_unit = UNSET
-        else:
-            input_unit = _input_unit  # type: ignore[arg-type]
+        masses = d.pop("masses", UNSET)
+        material_density = d.pop("material_density", UNSET)
 
-        output = d.pop("output", UNSET)
+        _material_density_unit = d.pop("material_density_unit", UNSET)
+        material_density_unit: Union[Unset, UnitDensity]
+        if isinstance(_material_density_unit, Unset):
+            material_density_unit = UNSET
+        else:
+            material_density_unit = _material_density_unit  # type: ignore[arg-type]
 
         _output_unit = d.pop("output_unit", UNSET)
-        output_unit: Union[Unset, UnitTorque]
+        output_unit: Union[Unset, UnitMass]
         if isinstance(_output_unit, Unset):
             output_unit = UNSET
         else:
             output_unit = _output_unit  # type: ignore[arg-type]
 
+        _src_format = d.pop("src_format", UNSET)
+        src_format: Union[Unset, FileImportFormat]
+        if isinstance(_src_format, Unset):
+            src_format = UNSET
+        else:
+            src_format = _src_format  # type: ignore[arg-type]
+
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
 
@@ -149,31 +168,33 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_torque_conversion = cls(
+        file_mass = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
-            input=input,
-            input_unit=input_unit,
-            output=output,
+            mass=mass,
+            masses=masses,
+            material_density=material_density,
+            material_density_unit=material_density_unit,
             output_unit=output_unit,
+            src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_torque_conversion.additional_properties = d
-        return unit_torque_conversion
+        file_mass.additional_properties = d
+        return file_mass
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.4/kittycad/models/unit_volume_conversion.py` & `kittycad-0.4.5/kittycad/models/file_density.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,62 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_volume import UnitVolume
+from ..models.file_import_format import FileImportFormat
+from ..models.unit_density import UnitDensity
+from ..models.unit_mass import UnitMass
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-B = TypeVar("B", bound="UnitVolumeConversion")
+YY = TypeVar("YY", bound="FileDensity")
 
 
 @attr.s(auto_attribs=True)
-class UnitVolumeConversion:
-    """Result of converting between units."""  # noqa: E501
+class FileDensity:
+    """A file density result."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
+    densities: Union[Unset, Any] = UNSET
+    density: Union[Unset, float] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
-    input: Union[Unset, float] = UNSET
-    input_unit: Union[Unset, UnitVolume] = UNSET
-    output: Union[Unset, float] = UNSET
-    output_unit: Union[Unset, UnitVolume] = UNSET
+    material_mass: Union[Unset, float] = UNSET
+    material_mass_unit: Union[Unset, UnitMass] = UNSET
+    output_unit: Union[Unset, UnitDensity] = UNSET
+    src_format: Union[Unset, FileImportFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         completed_at: Union[Unset, str] = UNSET
         if not isinstance(self.completed_at, Unset):
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
+        densities = self.densities
+        density = self.density
         error = self.error
         id = self.id
-        input = self.input
-        if not isinstance(self.input_unit, Unset):
-            input_unit = self.input_unit
-        output = self.output
+        material_mass = self.material_mass
+        if not isinstance(self.material_mass_unit, Unset):
+            material_mass_unit = self.material_mass_unit
         if not isinstance(self.output_unit, Unset):
             output_unit = self.output_unit
+        if not isinstance(self.src_format, Unset):
+            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
         if not isinstance(self.status, Unset):
             status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
@@ -59,39 +66,43 @@
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
             field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
             field_dict["created_at"] = created_at
+        if densities is not UNSET:
+            field_dict["densities"] = densities
+        if density is not UNSET:
+            field_dict["density"] = density
         if error is not UNSET:
             field_dict["error"] = error
         if id is not UNSET:
             field_dict["id"] = id
-        if input is not UNSET:
-            field_dict["input"] = input
-        if input_unit is not UNSET:
-            field_dict["input_unit"] = input_unit
-        if output is not UNSET:
-            field_dict["output"] = output
+        if material_mass is not UNSET:
+            field_dict["material_mass"] = material_mass
+        if material_mass_unit is not UNSET:
+            field_dict["material_mass_unit"] = material_mass_unit
         if output_unit is not UNSET:
             field_dict["output_unit"] = output_unit
+        if src_format is not UNSET:
+            field_dict["src_format"] = src_format
         if started_at is not UNSET:
             field_dict["started_at"] = started_at
         if status is not UNSET:
             field_dict["status"] = status
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[B], src_dict: Dict[str, Any]) -> B:
+    def from_dict(cls: Type[YY], src_dict: Dict[str, Any]) -> YY:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -99,41 +110,49 @@
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
+        densities = d.pop("densities", UNSET)
+        density = d.pop("density", UNSET)
+
         error = d.pop("error", UNSET)
 
         _id = d.pop("id", UNSET)
         id: Union[Unset, Uuid]
         if isinstance(_id, Unset):
             id = UNSET
         else:
-            id = Uuid(_id)
+            id = _id  # type: ignore[arg-type]
 
-        input = d.pop("input", UNSET)
+        material_mass = d.pop("material_mass", UNSET)
 
-        _input_unit = d.pop("input_unit", UNSET)
-        input_unit: Union[Unset, UnitVolume]
-        if isinstance(_input_unit, Unset):
-            input_unit = UNSET
+        _material_mass_unit = d.pop("material_mass_unit", UNSET)
+        material_mass_unit: Union[Unset, UnitMass]
+        if isinstance(_material_mass_unit, Unset):
+            material_mass_unit = UNSET
         else:
-            input_unit = _input_unit  # type: ignore[arg-type]
-
-        output = d.pop("output", UNSET)
+            material_mass_unit = _material_mass_unit  # type: ignore[arg-type]
 
         _output_unit = d.pop("output_unit", UNSET)
-        output_unit: Union[Unset, UnitVolume]
+        output_unit: Union[Unset, UnitDensity]
         if isinstance(_output_unit, Unset):
             output_unit = UNSET
         else:
             output_unit = _output_unit  # type: ignore[arg-type]
 
+        _src_format = d.pop("src_format", UNSET)
+        src_format: Union[Unset, FileImportFormat]
+        if isinstance(_src_format, Unset):
+            src_format = UNSET
+        else:
+            src_format = _src_format  # type: ignore[arg-type]
+
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
 
@@ -149,31 +168,33 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_volume_conversion = cls(
+        file_density = cls(
             completed_at=completed_at,
             created_at=created_at,
+            densities=densities,
+            density=density,
             error=error,
             id=id,
-            input=input,
-            input_unit=input_unit,
-            output=output,
+            material_mass=material_mass,
+            material_mass_unit=material_mass_unit,
             output_unit=output_unit,
+            src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_volume_conversion.additional_properties = d
-        return unit_volume_conversion
+        file_density.additional_properties = d
+        return file_density
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.4/kittycad/models/update_user.py` & `kittycad-0.4.5/kittycad/models/update_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-K = TypeVar("K", bound="UpdateUser")
+UA = TypeVar("UA", bound="UpdateUser")
 
 
 @attr.s(auto_attribs=True)
 class UpdateUser:
     """The user-modifiable parts of a User."""  # noqa: E501
 
     company: Union[Unset, str] = UNSET
@@ -43,15 +43,15 @@
             field_dict["last_name"] = last_name
         if phone is not UNSET:
             field_dict["phone"] = phone
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[K], src_dict: Dict[str, Any]) -> K:
+    def from_dict(cls: Type[UA], src_dict: Dict[str, Any]) -> UA:
         d = src_dict.copy()
         company = d.pop("company", UNSET)
 
         discord = d.pop("discord", UNSET)
 
         first_name = d.pop("first_name", UNSET)
```

### Comparing `kittycad-0.4.4/kittycad/models/user.py` & `kittycad-0.4.5/kittycad/models/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..types import UNSET, Unset
 
-K = TypeVar("K", bound="User")
+TN = TypeVar("TN", bound="User")
 
 
 @attr.s(auto_attribs=True)
 class User:
     """A user."""  # noqa: E501
 
     company: Union[Unset, str] = UNSET
@@ -79,15 +79,15 @@
             field_dict["phone"] = phone
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[K], src_dict: Dict[str, Any]) -> K:
+    def from_dict(cls: Type[TN], src_dict: Dict[str, Any]) -> TN:
         d = src_dict.copy()
         company = d.pop("company", UNSET)
 
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
```

### Comparing `kittycad-0.4.4/kittycad/models/user_results_page.py` & `kittycad-0.4.5/kittycad/models/user_results_page.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
-H = TypeVar("H", bound="UserResultsPage")
+MZ = TypeVar("MZ", bound="UserResultsPage")
 
 
 @attr.s(auto_attribs=True)
 class UserResultsPage:
     """A single page of results"""  # noqa: E501
 
     from ..models.user import User
@@ -33,15 +33,15 @@
             field_dict["items"] = items
         if next_page is not UNSET:
             field_dict["next_page"] = next_page
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
+    def from_dict(cls: Type[MZ], src_dict: Dict[str, Any]) -> MZ:
         d = src_dict.copy()
         from ..models.user import User
 
         items = cast(List[User], d.pop("items", UNSET))
 
         next_page = d.pop("next_page", UNSET)
```

### Comparing `kittycad-0.4.4/kittycad/models/verification_token.py` & `kittycad-0.4.5/kittycad/models/verification_token.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..types import UNSET, Unset
 
-C = TypeVar("C", bound="VerificationToken")
+UG = TypeVar("UG", bound="VerificationToken")
 
 
 @attr.s(auto_attribs=True)
 class VerificationToken:
     """A verification token for a user.
 
     This is typically used to verify a user's email address."""  # noqa: E501
@@ -49,15 +49,15 @@
             field_dict["identifier"] = identifier
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[C], src_dict: Dict[str, Any]) -> C:
+    def from_dict(cls: Type[UG], src_dict: Dict[str, Any]) -> UG:
         d = src_dict.copy()
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
```

### Comparing `kittycad-0.4.4/kittycad/types.py` & `kittycad-0.4.5/kittycad/types.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.4/pyproject.toml` & `kittycad-0.4.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kittycad"
-version = "0.4.4"
+version = "0.4.5"
 description = "A client library for accessing KittyCAD"
 
 authors = []
 
 readme = "README.md"
 packages = [
     {include = "kittycad"},
@@ -12,29 +12,31 @@
 include = ["CHANGELOG.md", "kittycad/py.typed"]
 
 [tool.poetry.dependencies]
 attrs = ">=20.1.0,<24.0.0"
 httpx = ">=0.15.4,<0.25.0"
 python = "^3.8"
 python-dateutil = "^2.8.0"
+websockets = "^11.0.3"
 
 [tool.poetry.dev-dependencies]
 autoclasstoc = "^1.6.0"
-black = "^22.0.0"
+black = "^23.7.0"
 isort = "^5.12.0"
+jinja2 = "^3.1.2"
 jsonpatch = "^1.32"
 mypy = "^1.2.0"
 openapi-parser = "^0.2.6"
-openapi-spec-validator = "^0.5.6"
+openapi-spec-validator = "^0.6.0"
 prance = "^23.6.21"
 pyenchant = "^3.2.2"
 pytest = "^7.0.1"
 pytest-asyncio = "^0.21.0"
 pytest-cov = "^4.0.0"
-ruff = "^0.0.277"
+ruff = "^0.0.280"
 Sphinx = "^6.2.1"
 sphinx-autoapi = "^2.0.1"
 sphinx-autodoc-typehints = "^1.12.0"
 sphinxcontrib-spelling = "^8.0.0"
 sphinx-copybutton = "^0.5.2"
 sphinxext-opengraph = "^0.8.2"
 sphinx-rtd-theme = "^1.0.0"
```

### Comparing `kittycad-0.4.4/PKG-INFO` & `kittycad-0.4.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: kittycad
-Version: 0.4.4
+Version: 0.4.5
 Summary: A client library for accessing KittyCAD
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: attrs (>=20.1.0,<24.0.0)
 Requires-Dist: httpx (>=0.15.4,<0.25.0)
 Requires-Dist: python-dateutil (>=2.8.0,<3.0.0)
+Requires-Dist: websockets (>=11.0.3,<12.0.0)
 Description-Content-Type: text/markdown
 
 ![image](https://user-images.githubusercontent.com/19377312/165883233-3bdbc9fb-ddf9-4173-8cf2-d1b70ab7127d.png)
 
 # kittycad.py
 
 The Python API client for KittyCAD.
```

