# Comparing `tmp/clustaar.schemas-1.0.9.tar.gz` & `tmp/clustaar.schemas-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clustaar.schemas-1.0.9.tar", last modified: Tue Jan 31 14:38:20 2023, max compression
+gzip compressed data, was "clustaar.schemas-1.1.0.tar", last modified: Tue Aug  1 15:01:10 2023, max compression
```

## Comparing `clustaar.schemas-1.0.9.tar` & `clustaar.schemas-1.1.0.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:38:20.257786 clustaar.schemas-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:38:20.241786 clustaar.schemas-1.0.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:38:20.245786 clustaar.schemas-1.0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/.github/workflows/build_dev_package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/.github/workflows/build_package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/.github/workflows/launch_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-01-31 14:38:20.257786 clustaar.schemas-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:38:20.245786 clustaar.schemas-1.0.9/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:38:20.245786 clustaar.schemas-1.0.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-01-31 14:38:20.257786 clustaar.schemas-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:38:20.241786 clustaar.schemas-1.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:38:20.245786 clustaar.schemas-1.0.9/src/clustaar/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/src/clustaar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:38:20.249786 clustaar.schemas-1.0.9/src/clustaar/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/src/clustaar/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/src/clustaar/schemas/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/src/clustaar/schemas/custom_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/src/clustaar/schemas/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/src/clustaar/schemas/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/src/clustaar/schemas/processors.py
--rw-r--r--   0 runner    (1001) docker     (123)    40130 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/src/clustaar/schemas/v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/src/clustaar/schemas/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:38:20.245786 clustaar.schemas-1.0.9/src/clustaar.schemas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-01-31 14:38:20.000000 clustaar.schemas-1.0.9/src/clustaar.schemas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-01-31 14:38:20.000000 clustaar.schemas-1.0.9/src/clustaar.schemas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 14:38:20.000000 clustaar.schemas-1.0.9/src/clustaar.schemas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 14:38:20.000000 clustaar.schemas-1.0.9/src/clustaar.schemas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-01-31 14:38:20.000000 clustaar.schemas-1.0.9/src/clustaar.schemas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-31 14:38:20.000000 clustaar.schemas-1.0.9/src/clustaar.schemas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:38:20.249786 clustaar.schemas-1.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:38:20.249786 clustaar.schemas-1.0.9/tests/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/test_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:38:20.253786 clustaar.schemas-1.0.9/tests/schemas/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_ask_location_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_assign_intercom_conversation_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_close_iadvize_conversation_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_close_intercom_conversation_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_contain_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_create_user_request_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_create_zendesk_ticket_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_custom_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_customer_satisfaction_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_customer_satisfaction_callback_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_equals_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_flow_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_flow_connection_predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_flow_connection_team_predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_flow_connection_user_predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_go_to_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_google_custom_search_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_is_greater_than_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_is_greater_than_or_equal_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_is_less_than_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_is_less_than_or_equal_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_is_logged_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_is_not_logged_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_is_not_set_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_is_number_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_is_offline_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_is_online_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_is_set_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_jump_to_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_legacy_reply_to_message_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_match_intent_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_match_regexp_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_open_url_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_pause_bot_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_predicate_message_getter.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_predicate_session_value_getter.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_predicate_user_attribute_getter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_send_cards_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_send_choices_list_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_send_email_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_send_image_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_send_js_event_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_send_quick_replies_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_send_simple_cards_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_send_text_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_send_webhook_request_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_set_user_attribute_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_share_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_step_target.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_store_session_value_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_story_target.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_transfer_iadvize_conversation_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_url_loaded_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_video.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_wait_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_webhook_interlocutor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/v1/test_webhook_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:38:20.257786 clustaar.schemas-1.0.9/tests/schemas/validators/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/validators/test_is_regexp.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/schemas/validators/test_object_id.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-01-31 14:38:10.000000 clustaar.schemas-1.0.9/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:01:10.521566 clustaar.schemas-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:01:10.481566 clustaar.schemas-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:01:10.489566 clustaar.schemas-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/.github/workflows/build_dev_package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/.github/workflows/build_package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/.github/workflows/launch_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-08-01 15:01:10.521566 clustaar.schemas-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:01:10.489566 clustaar.schemas-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:01:10.493566 clustaar.schemas-1.1.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-08-01 15:01:10.521566 clustaar.schemas-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:01:10.481566 clustaar.schemas-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:01:10.493566 clustaar.schemas-1.1.0/src/clustaar/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/src/clustaar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:01:10.497566 clustaar.schemas-1.1.0/src/clustaar/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/src/clustaar/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/src/clustaar/schemas/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/src/clustaar/schemas/custom_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/src/clustaar/schemas/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/src/clustaar/schemas/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/src/clustaar/schemas/processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39960 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/src/clustaar/schemas/v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/src/clustaar/schemas/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:01:10.493566 clustaar.schemas-1.1.0/src/clustaar.schemas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-08-01 15:01:10.000000 clustaar.schemas-1.1.0/src/clustaar.schemas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-08-01 15:01:10.000000 clustaar.schemas-1.1.0/src/clustaar.schemas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 15:01:10.000000 clustaar.schemas-1.1.0/src/clustaar.schemas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 15:01:10.000000 clustaar.schemas-1.1.0/src/clustaar.schemas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-01 15:01:10.000000 clustaar.schemas-1.1.0/src/clustaar.schemas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-01 15:01:10.000000 clustaar.schemas-1.1.0/src/clustaar.schemas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:01:10.497566 clustaar.schemas-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:01:10.497566 clustaar.schemas-1.1.0/tests/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:01:10.517567 clustaar.schemas-1.1.0/tests/schemas/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_ask_location_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_assign_intercom_conversation_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_close_iadvize_conversation_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_close_intercom_conversation_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_contain_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_create_user_request_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_create_zendesk_ticket_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_custom_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_customer_satisfaction_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_customer_satisfaction_callback_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_equals_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_flow_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_flow_connection_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_flow_connection_team_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_flow_connection_user_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_go_to_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_google_custom_search_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_is_greater_than_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_is_greater_than_or_equal_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_is_less_than_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_is_less_than_or_equal_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_is_logged_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_is_not_logged_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_is_not_set_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_is_number_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_is_offline_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_is_online_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_is_set_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_jump_to_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_legacy_reply_to_message_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_match_intent_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_match_regexp_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_open_url_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_pause_bot_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_predicate_message_getter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_predicate_session_value_getter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_predicate_user_attribute_getter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_send_cards_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_send_choices_list_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_send_email_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_send_image_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_send_js_event_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_send_quick_replies_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_send_simple_cards_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_send_text_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_send_webhook_request_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_set_user_attribute_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_share_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_step_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_store_session_value_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_story_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_transfer_iadvize_conversation_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_url_loaded_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_wait_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_webhook_interlocutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/v1/test_webhook_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:01:10.517567 clustaar.schemas-1.1.0/tests/schemas/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/validators/test_is_regexp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/schemas/validators/test_object_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-01 15:01:01.000000 clustaar.schemas-1.1.0/tox.ini
```

### Comparing `clustaar.schemas-1.0.9/.coveragerc` & `clustaar.schemas-1.1.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/.github/workflows/build_dev_package.yml` & `clustaar.schemas-1.1.0/.github/workflows/build_dev_package.yml`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/.github/workflows/build_package.yml` & `clustaar.schemas-1.1.0/.github/workflows/build_package.yml`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/.github/workflows/launch_tests.yml` & `clustaar.schemas-1.1.0/.github/workflows/launch_tests.yml`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/.gitignore` & `clustaar.schemas-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/LICENSE.txt` & `clustaar.schemas-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/PKG-INFO` & `clustaar.schemas-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clustaar.schemas
-Version: 1.0.9
+Version: 1.1.0
 Summary: Clustaar objects schemas
 Home-page: https://github.com/Clustaar/clustaar.schemas
 Author: Aurélien
 Author-email: aurelien@clustaar.com
 License: mit
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `clustaar.schemas-1.0.9/docs/Makefile` & `clustaar.schemas-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/docs/conf.py` & `clustaar.schemas-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/docs/index.rst` & `clustaar.schemas-1.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/requirements.txt` & `clustaar.schemas-1.1.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/setup.cfg` & `clustaar.schemas-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/setup.py` & `clustaar.schemas-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/src/clustaar/schemas/constants.py` & `clustaar.schemas-1.1.0/src/clustaar/schemas/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 SEND_EMAIL_ACTION_CONTENT_MAX_LENGTH = 1500
 SEND_EMAIL_ACTION_RECIPIENT_MAX_LENGTH = 150
 SEND_EMAIL_ACTION_REPLY_TO_EMAIL_MAX_LENGTH = 150
 SEND_EMAIL_ACTION_REPLY_TO_NAME_MAX_LENGTH = 50
 
 EXTERNAL_URL_MAX_LENGTH = 500
 
-SEND_TEXT_ACTION_MESSAGE_MAX_LENGTH = 500
+SEND_TEXT_ACTION_MESSAGE_MAX_LENGTH = 1000
 SEND_TEXT_ACTION_MAX_MESSAGES_COUNT = 10
 
 SEND_QUICK_REPLIES_ACTION_MAX_BUTTONS_COUNT = 11
 QUICK_REPLY_TITLE_MAX_LENGTH = 60
 
 BUTTON_TITLE_MAX_LENGTH = 20
```

### Comparing `clustaar.schemas-1.0.9/src/clustaar/schemas/custom_schemas.py` & `clustaar.schemas-1.1.0/src/clustaar/schemas/custom_schemas.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/src/clustaar/schemas/fields.py` & `clustaar.schemas-1.1.0/src/clustaar/schemas/fields.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/src/clustaar/schemas/models.py` & `clustaar.schemas-1.1.0/src/clustaar/schemas/models.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/src/clustaar/schemas/processors.py` & `clustaar.schemas-1.1.0/src/clustaar/schemas/processors.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/src/clustaar/schemas/v1.py` & `clustaar.schemas-1.1.0/src/clustaar/schemas/v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -453,21 +453,15 @@
 
 QUICK_REPLY = Schema(
     {
         "title": f.String(
             validators=v.Length(min=1, max=QUICK_REPLY_TITLE_MAX_LENGTH),
             pre_load=[html_sanitize, unicode_normalize],
         ),
-        "action": f.PolymorphicObject(
-            on="type",
-            schemas={
-                "go_to_action": GO_TO_ACTION,
-                "customer_satisfaction_callback_action": CUSTOMER_SATISFACTION_CALLBACK_ACTION,
-            },
-        ),
+        "action": f.PolymorphicObject(on="type", schemas=BUTTON_ACTIONS_SCHEMAS),
         "type": f.Constant(value="quick_reply", read_only=True, optional=True),
     },
     name="quick_reply",
 )
 
 
 SEND_QUICK_REPLIES_ACTION = Schema(
```

### Comparing `clustaar.schemas-1.0.9/src/clustaar/schemas/validators.py` & `clustaar.schemas-1.1.0/src/clustaar/schemas/validators.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/src/clustaar.schemas.egg-info/PKG-INFO` & `clustaar.schemas-1.1.0/src/clustaar.schemas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clustaar.schemas
-Version: 1.0.9
+Version: 1.1.0
 Summary: Clustaar objects schemas
 Home-page: https://github.com/Clustaar/clustaar.schemas
 Author: Aurélien
 Author-email: aurelien@clustaar.com
 License: mit
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `clustaar.schemas-1.0.9/src/clustaar.schemas.egg-info/SOURCES.txt` & `clustaar.schemas-1.1.0/src/clustaar.schemas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_ask_location_action.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_ask_location_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_assign_intercom_conversation_action.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_assign_intercom_conversation_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_audio.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_audio.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_close_iadvize_conversation_action.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_close_iadvize_conversation_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_close_intercom_conversation_action.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_close_intercom_conversation_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_contain_condition.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_contain_condition.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_coordinates.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_coordinates.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_create_user_request_action.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_create_user_request_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_create_zendesk_ticket_action.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_create_zendesk_ticket_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_custom_event.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_custom_event.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_customer_satisfaction_action.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_customer_satisfaction_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_customer_satisfaction_callback_action.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_customer_satisfaction_callback_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_equals_condition.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_equals_condition.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_file.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_file.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_flow_connection.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_flow_connection.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_flow_connection_predicate.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_flow_connection_predicate.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_flow_connection_team_predicate.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_flow_connection_team_predicate.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_flow_connection_user_predicate.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_flow_connection_user_predicate.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_go_to_action.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_go_to_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_google_custom_search_action.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_google_custom_search_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_image.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_image.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_is_greater_than_condition.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_is_greater_than_condition.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_is_greater_than_or_equal_condition.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_is_greater_than_or_equal_condition.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_is_less_than_condition.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_is_less_than_condition.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_is_less_than_or_equal_condition.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_is_less_than_or_equal_condition.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_is_logged_condition.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_is_logged_condition.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_is_not_logged_condition.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_is_not_logged_condition.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_is_not_set_condition.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_is_not_set_condition.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_is_number_condition.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_is_number_condition.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_is_offline_condition.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_is_offline_condition.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_is_online_condition.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_is_online_condition.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_is_set_condition.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_is_set_condition.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_jump_to_action.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_jump_to_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_legacy_reply_to_message_action.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_legacy_reply_to_message_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_match_intent_condition.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_match_intent_condition.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_match_regexp_condition.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_match_regexp_condition.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_message.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_message.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_open_url_action.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_open_url_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_pause_bot_action.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_pause_bot_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_predicate_message_getter.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_predicate_message_getter.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_predicate_session_value_getter.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_predicate_session_value_getter.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_predicate_user_attribute_getter.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_predicate_user_attribute_getter.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_send_cards_action.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_send_cards_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_send_choices_list_action.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_send_choices_list_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_send_email_action.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_send_email_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_send_image_action.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_send_image_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_send_js_event_action.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_send_js_event_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_send_quick_replies_action.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_send_quick_replies_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_send_simple_cards_action.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_send_simple_cards_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_send_text_action.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_send_text_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_send_webhook_request_action.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_send_webhook_request_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_set_user_attribute_action.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_set_user_attribute_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_share_action.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_share_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_step_target.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_step_target.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_store_session_value_action.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_store_session_value_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_story_target.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_story_target.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_transfer_iadvize_conversation_action.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_transfer_iadvize_conversation_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from clustaar.schemas.v1 import TRANSFER_IADVIZE_CONVERSATION_ACTION
 from clustaar.schemas.models import TransferIAdvizeConversationAction, IAdvizeDistributionRule
 import pytest
 
 
 @pytest.fixture
 def action():
-
     return TransferIAdvizeConversationAction(
         failed_transfer_message="sorry",
         distribution_rule=IAdvizeDistributionRule(id="234", label="Human"),
     )
 
 
 @pytest.fixture
```

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_url_loaded_event.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_url_loaded_event.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_video.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_video.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_wait_action.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_wait_action.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_webhook_interlocutor.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_webhook_interlocutor.py`

 * *Files identical despite different names*

### Comparing `clustaar.schemas-1.0.9/tests/schemas/v1/test_webhook_request.py` & `clustaar.schemas-1.1.0/tests/schemas/v1/test_webhook_request.py`

 * *Files identical despite different names*

