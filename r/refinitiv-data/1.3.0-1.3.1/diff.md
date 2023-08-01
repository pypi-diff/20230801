# Comparing `tmp/refinitiv-data-1.3.0.tar.gz` & `tmp/refinitiv-data-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refinitiv-data-1.3.0.tar", last modified: Wed Jun 21 15:15:09 2023, max compression
+gzip compressed data, was "refinitiv-data-1.3.1.tar", last modified: Mon Jul 31 10:28:23 2023, max compression
```

## Comparing `refinitiv-data-1.3.0.tar` & `refinitiv-data-1.3.1.tar`

### file list

```diff
@@ -1,1040 +1,1040 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.950217 refinitiv-data-1.3.0/
--rw-rw-rw-   0 root         (0) root         (0)    11615 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)    11358 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     9778 2023-06-21 15:15:09.950217 refinitiv-data-1.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     9061 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.650218 refinitiv-data-1.3.0/changes/
--rw-rw-rw-   0 root         (0) root         (0)      457 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/changes/template.jinja
--rw-rw-rw-   0 root         (0) root         (0)    21868 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.650218 refinitiv-data-1.3.0/refinitiv/
--rw-rw-rw-   0 root         (0) root         (0)       76 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.658218 refinitiv-data-1.3.0/refinitiv/data/
--rw-rw-rw-   0 root         (0) root         (0)     1106 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_base_enum.py
--rw-rw-rw-   0 root         (0) root         (0)    16816 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_config_defaults.py
--rw-rw-rw-   0 root         (0) root         (0)     1143 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_config_functions.py
--rw-rw-rw-   0 root         (0) root         (0)    15270 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_configure.py
--rw-rw-rw-   0 root         (0) root         (0)     4036 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_content_type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.658218 refinitiv-data-1.3.0/refinitiv/data/_core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1810 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/log_reporter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.670218 refinitiv-data-1.3.0/refinitiv/data/_core/session/
--rw-rw-rw-   0 root         (0) root         (0)      719 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      245 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/_dacs_params.py
--rw-rw-rw-   0 root         (0) root         (0)     3967 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/_default_session_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     5004 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/_desktop_session.py
--rw-rw-rw-   0 root         (0) root         (0)     9961 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/_platform_session.py
--rw-rw-rw-   0 root         (0) root         (0)    11808 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/_retry_transport.py
--rw-rw-rw-   0 root         (0) root         (0)    15808 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/_session.py
--rw-rw-rw-   0 root         (0) root         (0)     1078 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/_session_cxn_factory.py
--rw-rw-rw-   0 root         (0) root         (0)      188 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/_session_cxn_type.py
--rw-rw-rw-   0 root         (0) root         (0)     2472 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/_session_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    10130 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/_session_provider.py
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/_session_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1086 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/_user_uuid.py
--rw-rw-rw-   0 root         (0) root         (0)     3632 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/access_token_updater.py
--rw-rw-rw-   0 root         (0) root         (0)    11862 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/auth_manager.py
--rw-rw-rw-   0 root         (0) root         (0)    10563 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/connection.py
--rw-rw-rw-   0 root         (0) root         (0)      660 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/event.py
--rw-rw-rw-   0 root         (0) root         (0)     1411 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/event_code.py
--rw-rw-rw-   0 root         (0) root         (0)      489 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/global_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     1475 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/grant_password.py
--rw-rw-rw-   0 root         (0) root         (0)    12676 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/http_service.py
--rw-rw-rw-   0 root         (0) root         (0)      620 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/null_session.py
--rw-rw-rw-   0 root         (0) root         (0)     4281 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/refresh_token_updater.py
--rw-rw-rw-   0 root         (0) root         (0)     2487 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/tools.py
--rw-rw-rw-   0 root         (0) root         (0)     3990 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/updater.py
--rw-rw-rw-   0 root         (0) root         (0)     2300 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.670218 refinitiv-data-1.3.0/refinitiv/data/_external_libraries/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_external_libraries/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.670218 refinitiv-data-1.3.0/refinitiv/data/_external_libraries/python_configuration/
--rw-rw-rw-   0 root         (0) root         (0)     1071 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_external_libraries/python_configuration/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)    26229 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_external_libraries/python_configuration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11923 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_external_libraries/python_configuration/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     7238 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_external_libraries/python_configuration/configuration_set.py
--rw-rw-rw-   0 root         (0) root         (0)     5845 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_external_libraries/python_configuration/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.678218 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/
--rw-rw-rw-   0 root         (0) root         (0)      608 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5350 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_containers.py
--rw-rw-rw-   0 root         (0) root         (0)     2141 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_data_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)    12224 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     4588 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_history_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)      711 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_history_df_builder_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     1500 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_intervals_consts.py
--rw-rw-rw-   0 root         (0) root         (0)     3454 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_mixed_streams.py
--rw-rw-rw-   0 root         (0) root         (0)     5066 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_ohlc_builder.py
--rw-rw-rw-   0 root         (0) root         (0)    12099 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_pricing_recorder.py
--rw-rw-rw-   0 root         (0) root         (0)     5290 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_recording_control.py
--rw-rw-rw-   0 root         (0) root         (0)     3110 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_stream_update_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.682218 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/
--rw-rw-rw-   0 root         (0) root         (0)      335 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2993 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_adc_context.py
--rw-rw-rw-   0 root         (0) root         (0)     1950 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_adc_rdp_context.py
--rw-rw-rw-   0 root         (0) root         (0)     1979 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_adc_udf_context.py
--rw-rw-rw-   0 root         (0) root         (0)     1359 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_context.py
--rw-rw-rw-   0 root         (0) root         (0)     3186 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_context_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     4950 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_cust_inst_context.py
--rw-rw-rw-   0 root         (0) root         (0)     2854 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_cust_inst_rdp_context.py
--rw-rw-rw-   0 root         (0) root         (0)     2250 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_cust_inst_udf_context.py
--rw-rw-rw-   0 root         (0) root         (0)      755 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_hp_and_cust_inst_context.py
--rw-rw-rw-   0 root         (0) root         (0)     2678 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_hp_context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.682218 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/
--rw-rw-rw-   0 root         (0) root         (0)      659 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2482 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/_add_periods.py
--rw-rw-rw-   0 root         (0) root         (0)     2504 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/_count_periods.py
--rw-rw-rw-   0 root         (0) root         (0)     3621 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/_date_schedule.py
--rw-rw-rw-   0 root         (0) root         (0)     4581 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/_holidays.py
--rw-rw-rw-   0 root         (0) root         (0)     1410 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/_is_working_day.py
--rw-rw-rw-   0 root         (0) root         (0)     3914 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/get_data_func.py
--rw-rw-rw-   0 root         (0) root         (0)     7418 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/get_history_func.py
--rw-rw-rw-   0 root         (0) root         (0)     3417 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/get_stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.682218 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/news/
--rw-rw-rw-   0 root         (0) root         (0)      280 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/news/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2306 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/news/_news.py
--rw-rw-rw-   0 root         (0) root         (0)     2804 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/session.py
--rw-rw-rw-   0 root         (0) root         (0)    12912 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_log.py
--rw-rw-rw-   0 root         (0) root         (0)      338 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_open_state.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.686218 refinitiv-data-1.3.0/refinitiv/data/_qpl/
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_qpl/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      641 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_qpl/_bid_ask.py
--rw-rw-rw-   0 root         (0) root         (0)     2781 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_qpl/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)      766 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_qpl/_fx_spot_quote.py
--rw-rw-rw-   0 root         (0) root         (0)     2001 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_qpl/_fx_swap_points.py
--rw-rw-rw-   0 root         (0) root         (0)     3727 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_qpl/_fx_swp_to_swp.py
--rw-rw-rw-   0 root         (0) root         (0)      888 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_qpl/_serializer.py
--rw-rw-rw-   0 root         (0) root         (0)      760 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_qpl/_tenor_bid_ask.py
--rw-rw-rw-   0 root         (0) root         (0)      220 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_qpl/_tenor_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.690218 refinitiv-data-1.3.0/refinitiv/data/_tools/
--rw-rw-rw-   0 root         (0) root         (0)      213 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13407 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_tools/_common.py
--rw-rw-rw-   0 root         (0) root         (0)     1208 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_tools/_converter.py
--rw-rw-rw-   0 root         (0) root         (0)     6623 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_tools/_dataframe.py
--rw-rw-rw-   0 root         (0) root         (0)     4708 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_tools/_datetime.py
--rw-rw-rw-   0 root         (0) root         (0)       53 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_tools/_debug.py
--rw-rw-rw-   0 root         (0) root         (0)     1744 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_tools/_params.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_tools/_patterns.py
--rw-rw-rw-   0 root         (0) root         (0)     1083 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_tools/_repr.py
--rw-rw-rw-   0 root         (0) root         (0)     1317 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_tools/_specification.py
--rw-rw-rw-   0 root         (0) root         (0)     2196 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_tools/_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5257 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_tools/templates.py
--rw-rw-rw-   0 root         (0) root         (0)      731 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_types.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-06-21 15:15:09.000000 refinitiv-data-1.3.0/refinitiv/data/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.698217 refinitiv-data-1.3.0/refinitiv/data/content/
--rw-rw-rw-   0 root         (0) root         (0)     2082 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      510 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_content_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1195 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_content_data_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     1094 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_content_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     3533 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_content_provider_layer.py
--rw-rw-rw-   0 root         (0) root         (0)      620 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_content_response_factory.py
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_df_build_type.py
--rw-rw-rw-   0 root         (0) root         (0)    18497 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)     8547 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_df_builder_factory.py
--rw-rw-rw-   0 root         (0) root         (0)    18264 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_entire_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)      829 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_error_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     1970 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_historical_content_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     6441 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_historical_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     6937 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_historical_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)     2895 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_historical_raw_transf.py
--rw-rw-rw-   0 root         (0) root         (0)     3209 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_historical_response_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     3064 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_intervals.py
--rw-rw-rw-   0 root         (0) root         (0)     1593 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_universe_content_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     8436 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_universe_stream.py
--rw-rw-rw-   0 root         (0) root         (0)    18431 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_universe_streams.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.706218 refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/
--rw-rw-rw-   0 root         (0) root         (0)      467 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14446 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_custom_instruments_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     2160 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      801 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_enums.py
--rw-rw-rw-   0 root         (0) root         (0)     2415 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_events.py
--rw-rw-rw-   0 root         (0) root         (0)     6061 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_instrument_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12895 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_instrument_prop_classes.py
--rw-rw-rw-   0 root         (0) root         (0)    18090 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_manage.py
--rw-rw-rw-   0 root         (0) root         (0)     1323 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_search.py
--rw-rw-rw-   0 root         (0) root         (0)     8665 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_stream_facade.py
--rw-rw-rw-   0 root         (0) root         (0)     2941 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_summaries.py
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/events.py
--rw-rw-rw-   0 root         (0) root         (0)      662 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/manage.py
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/search.py
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/summaries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.710218 refinitiv-data-1.3.0/refinitiv/data/content/esg/
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1478 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/_base_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1674 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/_basic_overview_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1165 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/_esg_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     1631 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/_full_measures_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1665 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/_full_scores_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1911 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/_standard_measures_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1652 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/_standard_scores_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1189 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/_universe_definition.py
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/basic_overview.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.710218 refinitiv-data-1.3.0/refinitiv/data/content/esg/bulk/
--rw-rw-rw-   0 root         (0) root         (0)      143 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/bulk/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3858 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/bulk/_actions.py
--rw-rw-rw-   0 root         (0) root         (0)     9784 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/bulk/_db_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     1848 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/bulk/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      351 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/bulk/_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)      309 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/bulk/_errors.py
--rw-rw-rw-   0 root         (0) root         (0)     7363 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/bulk/_file_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     3264 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/bulk/_package_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     1333 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/bulk/_package_manager_facade.py
--rw-rw-rw-   0 root         (0) root         (0)     2562 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/bulk/_tools.py
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/full_measures.py
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/full_scores.py
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/standard_measures.py
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/standard_scores.py
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/universe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.714218 refinitiv-data-1.3.0/refinitiv/data/content/estimates/
--rw-rw-rw-   0 root         (0) root         (0)     1093 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1246 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)      475 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/_enums.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.714218 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_actuals/
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_actuals/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2175 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_actuals/_annual_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2156 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_actuals/_interim_definition.py
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_actuals/annual.py
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_actuals/interim.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.714218 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_actuals_kpi/
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_actuals_kpi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1789 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_actuals_kpi/_annual_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1793 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_actuals_kpi/_interim_definition.py
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_actuals_kpi/annual.py
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_actuals_kpi/interim.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.718217 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/
--rw-rw-rw-   0 root         (0) root         (0)      581 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2146 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/_annual_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2299 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/_historical_snapshots_non_periodic_measures_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2314 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/_historical_snapshots_periodic_measures_annual_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2305 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/_historical_snapshots_periodic_measures_interim_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2268 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/_historical_snapshots_recommendations_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2150 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/_interim_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2190 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/_non_periodic_measures_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2135 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/_recommendations_definition.py
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/annual.py
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/historical_snapshots_non_periodic_measures.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/historical_snapshots_periodic_measures_annual.py
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/historical_snapshots_periodic_measures_interim.py
--rw-rw-rw-   0 root         (0) root         (0)      100 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/historical_snapshots_recommendations.py
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/interim.py
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/non_periodic_measures.py
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/recommendations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.722218 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary_kpi/
--rw-rw-rw-   0 root         (0) root         (0)      117 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary_kpi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1771 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary_kpi/_annual_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1851 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary_kpi/_historical_snapshots_kpi_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1776 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary_kpi/_interim_definition.py
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary_kpi/annual.py
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary_kpi/historical_snapshots_kpi.py
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary_kpi/interim.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.726218 refinitiv-data-1.3.0/refinitiv/data/content/filings/
--rw-rw-rw-   0 root         (0) root         (0)      117 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/filings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/filings/_errors.py
--rw-rw-rw-   0 root         (0) root         (0)      304 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/filings/_feed_name.py
--rw-rw-rw-   0 root         (0) root         (0)     4584 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/filings/_filing_query.py
--rw-rw-rw-   0 root         (0) root         (0)    20076 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/filings/_retrieval_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     2697 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/filings/_retrieval_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     8827 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/filings/_search_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     4866 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/filings/_search_definition.py
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/filings/retrieval.py
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/filings/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.726218 refinitiv-data-1.3.0/refinitiv/data/content/fundamental_and_reference/
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/fundamental_and_reference/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3970 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/fundamental_and_reference/_content_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     2041 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/fundamental_and_reference/_data_grid_type.py
--rw-rw-rw-   0 root         (0) root         (0)      821 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/fundamental_and_reference/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)    10662 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/fundamental_and_reference/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2746 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/fundamental_and_reference/_request_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     2191 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/fundamental_and_reference/_response_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.730218 refinitiv-data-1.3.0/refinitiv/data/content/historical_pricing/
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/historical_pricing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3077 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/historical_pricing/_enums.py
--rw-rw-rw-   0 root         (0) root         (0)     2949 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/historical_pricing/_events_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      762 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/historical_pricing/_historical_pricing_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     3718 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/historical_pricing/_historical_pricing_request_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     3471 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/historical_pricing/_summaries_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      264 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/historical_pricing/events.py
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/historical_pricing/summaries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.730218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/
--rw-rw-rw-   0 root         (0) root         (0)      192 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5727 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_content_provider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.738217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/
--rw-rw-rw-   0 root         (0) root         (0)      383 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.738217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.742218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/
--rw-rw-rw-   0 root         (0) root         (0)      140 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1293 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_constituents.py
--rw-rw-rw-   0 root         (0) root         (0)    11462 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_curve_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    28240 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_curve_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2919 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.746218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/
--rw-rw-rw-   0 root         (0) root         (0)      565 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      311 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_basis_spline_smooth_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1833 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_business_sector.py
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_calendar_adjustment.py
--rw-rw-rw-   0 root         (0) root         (0)      217 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_calibration_model.py
--rw-rw-rw-   0 root         (0) root         (0)     2943 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_curve_sub_type.py
--rw-rw-rw-   0 root         (0) root         (0)      654 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_economic_sector.py
--rw-rw-rw-   0 root         (0) root         (0)     8933 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_industry.py
--rw-rw-rw-   0 root         (0) root         (0)     3834 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_industry_group.py
--rw-rw-rw-   0 root         (0) root         (0)     1223 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_interest_calculation_method.py
--rw-rw-rw-   0 root         (0) root         (0)      599 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_interpolation_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_issuer_type.py
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_main_constituent_asset_class.py
--rw-rw-rw-   0 root         (0) root         (0)      146 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_price_side.py
--rw-rw-rw-   0 root         (0) root         (0)     1283 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_rating.py
--rw-rw-rw-   0 root         (0) root         (0)      216 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_rating_scale_source.py
--rw-rw-rw-   0 root         (0) root         (0)      248 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_reference_entity_type.py
--rw-rw-rw-   0 root         (0) root         (0)      238 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_seniority.py
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.746218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.754217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/
--rw-rw-rw-   0 root         (0) root         (0)      514 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4482 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_butterfly_shift.py
--rw-rw-rw-   0 root         (0) root         (0)     6770 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_combined_shift.py
--rw-rw-rw-   0 root         (0) root         (0)     9677 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_curve_definition_pricing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.754217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/
--rw-rw-rw-   0 root         (0) root         (0)      179 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      194 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/_array_main_constituent_asset_class.py
--rw-rw-rw-   0 root         (0) root         (0)      146 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/_array_risk_type.py
--rw-rw-rw-   0 root         (0) root         (0)      216 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/_constituent_override_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      222 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/_shift_type.py
--rw-rw-rw-   0 root         (0) root         (0)      171 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/_shift_unit.py
--rw-rw-rw-   0 root         (0) root         (0)     3924 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_flattening_shift.py
--rw-rw-rw-   0 root         (0) root         (0)     1356 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_constituents.py
--rw-rw-rw-   0 root         (0) root         (0)     5452 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_curve_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     5860 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_curve_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2463 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_shift_scenario.py
--rw-rw-rw-   0 root         (0) root         (0)     3920 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_long_end_shift.py
--rw-rw-rw-   0 root         (0) root         (0)     3921 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_parallel_shift.py
--rw-rw-rw-   0 root         (0) root         (0)     3719 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_request.py
--rw-rw-rw-   0 root         (0) root         (0)     7749 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_shift_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     3921 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_short_end_shift.py
--rw-rw-rw-   0 root         (0) root         (0)     6772 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_time_bucket_shift.py
--rw-rw-rw-   0 root         (0) root         (0)     4477 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_twist_shift.py
--rw-rw-rw-   0 root         (0) root         (0)      483 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.762218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2943 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_base_definition_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     1236 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_bid_ask_fields_description.py
--rw-rw-rw-   0 root         (0) root         (0)     1158 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_bid_ask_fields_formula_description.py
--rw-rw-rw-   0 root         (0) root         (0)     3593 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_constituents_description.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.762218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3767 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/_curve_definition_description.py
--rw-rw-rw-   0 root         (0) root         (0)     1492 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/_request.py
--rw-rw-rw-   0 root         (0) root         (0)     1997 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_curve_parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.762218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_delete/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_delete/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_delete/_request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.762218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_enums/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_enums/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_enums/_quotation_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      186 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_enums/_standard_turn_period.py
--rw-rw-rw-   0 root         (0) root         (0)     1716 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_field_description.py
--rw-rw-rw-   0 root         (0) root         (0)     2176 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_field_formula_description.py
--rw-rw-rw-   0 root         (0) root         (0)     2164 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_formula_parameter_description.py
--rw-rw-rw-   0 root         (0) root         (0)     3621 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_instrument_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2568 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_instrument_description.py
--rw-rw-rw-   0 root         (0) root         (0)      940 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_turn_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     1899 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_spot_instrument_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2623 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_spot_instrument_description.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.766218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7044 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/_curve_definition_keys.py
--rw-rw-rw-   0 root         (0) root         (0)      915 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/_request.py
--rw-rw-rw-   0 root         (0) root         (0)     2871 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instrument_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2664 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instrument_description.py
--rw-rw-rw-   0 root         (0) root         (0)     2078 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instruments_segment.py
--rw-rw-rw-   0 root         (0) root         (0)     1193 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_mixin_request.py
--rw-rw-rw-   0 root         (0) root         (0)     1745 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_bid_ask.py
--rw-rw-rw-   0 root         (0) root         (0)     1038 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_bid_ask_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     2285 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_fx_forward_turn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.766218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_search/
--rw-rw-rw-   0 root         (0) root         (0)       42 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_search/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8798 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_search/_curve_get_definition_item.py
--rw-rw-rw-   0 root         (0) root         (0)      900 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_turn_adjustment.py
--rw-rw-rw-   0 root         (0) root         (0)      657 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.766218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3896 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/_curve_update_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1494 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/_request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.766218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_enums/
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_enums/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_enums/_interpolation_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      160 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_enums/_main_constituent_asset_class.py
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_enums/_risk_type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.766218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_triangulate_definitions/
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_triangulate_definitions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3353 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_triangulate_definitions/_request.py
--rw-rw-rw-   0 root         (0) root         (0)      186 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_types.py
--rw-rw-rw-   0 root         (0) root         (0)    21263 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_curves_builder_df.py
--rw-rw-rw-   0 root         (0) root         (0)    10677 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_curves_data_provider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.770218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_enums/
--rw-rw-rw-   0 root         (0) root         (0)      574 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_enums/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      171 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_enums/_calendar_adjustment.py
--rw-rw-rw-   0 root         (0) root         (0)      242 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_enums/_compounding_type.py
--rw-rw-rw-   0 root         (0) root         (0)      172 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_enums/_constituent_override_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_enums/_forward_curves_outputs.py
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_enums/_instrument_type.py
--rw-rw-rw-   0 root         (0) root         (0)      170 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_enums/_main_constituent_asset_class.py
--rw-rw-rw-   0 root         (0) root         (0)      253 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_enums/_market_data_access_denied_fallback.py
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_enums/_swap_price_side.py
--rw-rw-rw-   0 root         (0) root         (0)      201 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_enums/_zc_curves_outputs.py
--rw-rw-rw-   0 root         (0) root         (0)      616 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_enums/_zc_interpolation_mode.py
--rw-rw-rw-   0 root         (0) root         (0)     2832 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_forward_curve_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     3441 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_forward_curve_request_item.py
--rw-rw-rw-   0 root         (0) root         (0)      930 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_forward_curve_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.774217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/
--rw-rw-rw-   0 root         (0) root         (0)      234 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_constituents.py
--rw-rw-rw-   0 root         (0) root         (0)     1567 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_convexity.py
--rw-rw-rw-   0 root         (0) root         (0)     3893 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_curve.py
--rw-rw-rw-   0 root         (0) root         (0)      261 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_curve_point.py
--rw-rw-rw-   0 root         (0) root         (0)      746 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_instrument.py
--rw-rw-rw-   0 root         (0) root         (0)    13718 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_interest_rate_curve_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     1737 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_par_rate_shift.py
--rw-rw-rw-   0 root         (0) root         (0)     1085 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1426 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_turn.py
--rw-rw-rw-   0 root         (0) root         (0)     3014 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_valuation_time.py
--rw-rw-rw-   0 root         (0) root         (0)     2213 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_shift_scenario.py
--rw-rw-rw-   0 root         (0) root         (0)    10434 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_swap_zc_curve_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    19827 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_swap_zc_curve_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     8802 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_zc_curve_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     4209 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_zc_curve_definition_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12838 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_zc_curve_definitions.py
--rw-rw-rw-   0 root         (0) root         (0)    19563 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_zc_curve_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2988 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_zc_curve_request_item.py
--rw-rw-rw-   0 root         (0) root         (0)      726 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_zc_curve_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.794217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/
--rw-rw-rw-   0 root         (0) root         (0)     3130 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      185 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_adjust_interest_to_payment_date.py
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_american_monte_carlo_method.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_amortization_frequency.py
--rw-rw-rw-   0 root         (0) root         (0)      208 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_amortization_type.py
--rw-rw-rw-   0 root         (0) root         (0)      154 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_asset_class.py
--rw-rw-rw-   0 root         (0) root         (0)      273 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_average_type.py
--rw-rw-rw-   0 root         (0) root         (0)      365 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_axis.py
--rw-rw-rw-   0 root         (0) root         (0)      281 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_barrier_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      184 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_barrier_style.py
--rw-rw-rw-   0 root         (0) root         (0)      251 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_barrier_type.py
--rw-rw-rw-   0 root         (0) root         (0)      185 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_benchmark_yield_selection_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_binary_type.py
--rw-rw-rw-   0 root         (0) root         (0)      960 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_business_day_convention.py
--rw-rw-rw-   0 root         (0) root         (0)      415 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_buy_sell.py
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_calibration_strategy.py
--rw-rw-rw-   0 root         (0) root         (0)      405 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_call_put.py
--rw-rw-rw-   0 root         (0) root         (0)      390 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_cds_convention.py
--rw-rw-rw-   0 root         (0) root         (0)      763 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_common_tools.py
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_credit_spread_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1085 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_date_moving_convention.py
--rw-rw-rw-   0 root         (0) root         (0)      735 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_date_rolling_convention.py
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_dates_calendars_frequency.py
--rw-rw-rw-   0 root         (0) root         (0)     1225 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_day_count_basis.py
--rw-rw-rw-   0 root         (0) root         (0)      726 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_day_of_week.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_direction.py
--rw-rw-rw-   0 root         (0) root         (0)      201 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_discounting_type.py
--rw-rw-rw-   0 root         (0) root         (0)      250 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_dividend_extrapolation.py
--rw-rw-rw-   0 root         (0) root         (0)      342 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_dividend_type.py
--rw-rw-rw-   0 root         (0) root         (0)      456 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_doc_clause.py
--rw-rw-rw-   0 root         (0) root         (0)      175 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_double_binary_type.py
--rw-rw-rw-   0 root         (0) root         (0)      381 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_end_of_month_convention.py
--rw-rw-rw-   0 root         (0) root         (0)      191 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_equity_dividend_type.py
--rw-rw-rw-   0 root         (0) root         (0)      194 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_eti_input_volatility_type.py
--rw-rw-rw-   0 root         (0) root         (0)      210 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_exercise_schedule_type.py
--rw-rw-rw-   0 root         (0) root         (0)      645 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_exercise_style.py
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_extrapolation_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      289 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_fixing_frequency.py
--rw-rw-rw-   0 root         (0) root         (0)      282 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_format.py
--rw-rw-rw-   0 root         (0) root         (0)      269 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_forward_compute_method.py
--rw-rw-rw-   0 root         (0) root         (0)      299 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_forward_extrapolation.py
--rw-rw-rw-   0 root         (0) root         (0)      906 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_frequency.py
--rw-rw-rw-   0 root         (0) root         (0)      393 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_funding_spread_method.py
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_fx_binary_type.py
--rw-rw-rw-   0 root         (0) root         (0)      299 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_fx_cross_type.py
--rw-rw-rw-   0 root         (0) root         (0)      274 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_fx_leg_type.py
--rw-rw-rw-   0 root         (0) root         (0)      644 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_fx_swap_calculation_method.py
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_fx_volatility_model.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_holiday_outupts.py
--rw-rw-rw-   0 root         (0) root         (0)      233 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_implied_deposit_date_convention.py
--rw-rw-rw-   0 root         (0) root         (0)      140 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_in_or_out.py
--rw-rw-rw-   0 root         (0) root         (0)      319 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_index_average_method.py
--rw-rw-rw-   0 root         (0) root         (0)      644 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_index_compounding_method.py
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_index_convexity_adjustment_integration_method.py
--rw-rw-rw-   0 root         (0) root         (0)      260 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_index_convexity_adjustment_method.py
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_index_convexity_adjustment_type.py
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_index_observation_method.py
--rw-rw-rw-   0 root         (0) root         (0)      337 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_index_reset_type.py
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_index_spread_compounding_method.py
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_inflation_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      248 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_input_volatility_type.py
--rw-rw-rw-   0 root         (0) root         (0)      211 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_interest_calculation_convention.py
--rw-rw-rw-   0 root         (0) root         (0)      301 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_interest_type.py
--rw-rw-rw-   0 root         (0) root         (0)      311 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_interpolation_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      380 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_local_volatility_method.py
--rw-rw-rw-   0 root         (0) root         (0)      248 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_method.py
--rw-rw-rw-   0 root         (0) root         (0)      227 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_notional_exchange.py
--rw-rw-rw-   0 root         (0) root         (0)      281 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_numeraire_type.py
--rw-rw-rw-   0 root         (0) root         (0)      207 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_option_volatility_type.py
--rw-rw-rw-   0 root         (0) root         (0)      625 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_period_type.py
--rw-rw-rw-   0 root         (0) root         (0)      192 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_premium_settlement_type.py
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_price_side.py
--rw-rw-rw-   0 root         (0) root         (0)      301 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_pricing_model_type.py
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_projected_index_calculation_method.py
--rw-rw-rw-   0 root         (0) root         (0)      614 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_quote_fallback_logic.py
--rw-rw-rw-   0 root         (0) root         (0)     2113 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_redemption_date_type.py
--rw-rw-rw-   0 root         (0) root         (0)      213 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_repo_curve_type.py
--rw-rw-rw-   0 root         (0) root         (0)      145 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_risk_type.py
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_rounding.py
--rw-rw-rw-   0 root         (0) root         (0)      304 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_rounding_type.py
--rw-rw-rw-   0 root         (0) root         (0)      757 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_seniority.py
--rw-rw-rw-   0 root         (0) root         (0)      208 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_settlement_type.py
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_status.py
--rw-rw-rw-   0 root         (0) root         (0)     1545 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_stub_rule.py
--rw-rw-rw-   0 root         (0) root         (0)      184 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_swaption_settlement_type.py
--rw-rw-rw-   0 root         (0) root         (0)      160 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_swaption_type.py
--rw-rw-rw-   0 root         (0) root         (0)      205 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_swaption_volatility_type.py
--rw-rw-rw-   0 root         (0) root         (0)      185 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_tenor_reference_date.py
--rw-rw-rw-   0 root         (0) root         (0)      316 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_time_stamp.py
--rw-rw-rw-   0 root         (0) root         (0)      189 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_underlying_type.py
--rw-rw-rw-   0 root         (0) root         (0)      143 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_up_or_down.py
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_vol_type.py
--rw-rw-rw-   0 root         (0) root         (0)      343 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_volatility_adjustment_type.py
--rw-rw-rw-   0 root         (0) root         (0)      222 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_volatility_model.py
--rw-rw-rw-   0 root         (0) root         (0)      184 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_volatility_term_structure_type.py
--rw-rw-rw-   0 root         (0) root         (0)      172 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_volatility_type.py
--rw-rw-rw-   0 root         (0) root         (0)      913 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_yield_type.py
--rw-rw-rw-   0 root         (0) root         (0)    10539 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_ipa_content_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     1402 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_ipa_content_validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.798217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/
--rw-rw-rw-   0 root         (0) root         (0)      433 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1898 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_american_monte_carlo_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     3960 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_amortization_item.py
--rw-rw-rw-   0 root         (0) root         (0)     2188 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_barrier_definition_element.py
--rw-rw-rw-   0 root         (0) root         (0)      917 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_basket_item.py
--rw-rw-rw-   0 root         (0) root         (0)     1163 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_bid_ask_mid.py
--rw-rw-rw-   0 root         (0) root         (0)     5046 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_bond_rounding_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_day_weight.py
--rw-rw-rw-   0 root         (0) root         (0)     2295 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_fx_point.py
--rw-rw-rw-   0 root         (0) root         (0)     2157 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_input_flow.py
--rw-rw-rw-   0 root         (0) root         (0)     1846 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_interpolation_weight.py
--rw-rw-rw-   0 root         (0) root         (0)     1531 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_numerical_method.py
--rw-rw-rw-   0 root         (0) root         (0)      948 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_payout_scaling.py
--rw-rw-rw-   0 root         (0) root         (0)     1359 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_pde_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     4806 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_object_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.806218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1842 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_cap_surface_request_item.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.806218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_enums/
--rw-rw-rw-   0 root         (0) root         (0)      423 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_enums/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      246 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_enums/_calibration_type.py
--rw-rw-rw-   0 root         (0) root         (0)      180 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_enums/_moneyness_type.py
--rw-rw-rw-   0 root         (0) root         (0)      485 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_enums/_outputs.py
--rw-rw-rw-   0 root         (0) root         (0)      146 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_enums/_strike_type.py
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_enums/_volatility_type.py
--rw-rw-rw-   0 root         (0) root         (0)     3061 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_eti_surface_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     9016 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_eti_surface_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     1692 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_eti_surface_request_item.py
--rw-rw-rw-   0 root         (0) root         (0)     1708 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_fx_statistics_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)      777 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_fx_surface_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    13552 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_fx_surface_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2545 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_fx_surface_request_item.py
--rw-rw-rw-   0 root         (0) root         (0)     2694 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_i_ir_vol_model_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     9639 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_i_ir_vol_model_pricing_parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.810217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/
--rw-rw-rw-   0 root         (0) root         (0)      351 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2541 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/_maturity_filter.py
--rw-rw-rw-   0 root         (0) root         (0)     2477 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/_moneyness_weight.py
--rw-rw-rw-   0 root         (0) root         (0)     1214 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/_strike_filter.py
--rw-rw-rw-   0 root         (0) root         (0)     2290 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/_strike_filter_range.py
--rw-rw-rw-   0 root         (0) root         (0)     5195 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/_surface.py
--rw-rw-rw-   0 root         (0) root         (0)     6749 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/_surface_filters.py
--rw-rw-rw-   0 root         (0) root         (0)     5848 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/_surface_output.py
--rw-rw-rw-   0 root         (0) root         (0)      294 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/_surface_point.py
--rw-rw-rw-   0 root         (0) root         (0)     1145 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/_volatility_surface_point.py
--rw-rw-rw-   0 root         (0) root         (0)     1575 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_surface_request_item.py
--rw-rw-rw-   0 root         (0) root         (0)      468 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_surface_types.py
--rw-rw-rw-   0 root         (0) root         (0)    11119 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_surfaces_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)    14482 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_swaption_calculation_params.py
--rw-rw-rw-   0 root         (0) root         (0)     3498 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_swaption_surface_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1853 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_swaption_surface_request_item.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.810217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/
--rw-rw-rw-   0 root         (0) root         (0)      284 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.810217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_bond_curves/
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_bond_curves/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.810217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_bond_curves/curves/
--rw-rw-rw-   0 root         (0) root         (0)     1181 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_bond_curves/curves/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2737 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_bond_curves/curves/_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.814217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      472 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/_arg_enums.py
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/_base_data_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.814217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/curves/
--rw-rw-rw-   0 root         (0) root         (0)     1424 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/curves/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3000 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/curves/_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.814217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/
--rw-rw-rw-   0 root         (0) root         (0)     2037 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7353 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_data_classes.py
--rw-rw-rw-   0 root         (0) root         (0)    11268 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_manage.py
--rw-rw-rw-   0 root         (0) root         (0)     4906 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_search.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/manage.py
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.818217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5917 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     2900 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/_search.py
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.818217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/forward_curves/
--rw-rw-rw-   0 root         (0) root         (0)      945 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/forward_curves/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6123 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/forward_curves/_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.818217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/zc_curve_definitions/
--rw-rw-rw-   0 root         (0) root         (0)      186 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/zc_curve_definitions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5023 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/zc_curve_definitions/_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.818217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/zc_curves/
--rw-rw-rw-   0 root         (0) root         (0)     1282 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/zc_curves/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4232 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/zc_curves/_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.822218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/
--rw-rw-rw-   0 root         (0) root         (0)      196 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1829 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/_base_request_items.py
--rw-rw-rw-   0 root         (0) root         (0)      976 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/_content_data_validator.py
--rw-rw-rw-   0 root         (0) root         (0)      560 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/_request_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.822218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/add_periods/
--rw-rw-rw-   0 root         (0) root         (0)      260 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/add_periods/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2081 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/add_periods/_add_periods_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)    10019 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/add_periods/_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.822218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/count_periods/
--rw-rw-rw-   0 root         (0) root         (0)      172 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/count_periods/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8278 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/count_periods/_count_periods.py
--rw-rw-rw-   0 root         (0) root         (0)     1860 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/count_periods/_count_periods_data_provider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.822218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/
--rw-rw-rw-   0 root         (0) root         (0)      158 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6938 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/_date_schedule.py
--rw-rw-rw-   0 root         (0) root         (0)      933 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/_date_schedule_data_provider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.826218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/holidays/
--rw-rw-rw-   0 root         (0) root         (0)      143 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/holidays/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7269 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/holidays/_holidays.py
--rw-rw-rw-   0 root         (0) root         (0)     3486 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/holidays/_holidays_data_provider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.826218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6928 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/_is_working_day.py
--rw-rw-rw-   0 root         (0) root         (0)     2388 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/_is_working_day_data_provider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.830217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/
--rw-rw-rw-   0 root         (0) root         (0)      483 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2463 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/_base_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     8331 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/_contracts_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     3681 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1036 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/_instrument_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     3717 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/_quantitative_data_stream.py
--rw-rw-rw-   0 root         (0) root         (0)     3615 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/_stream_facade.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.830217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/bond/
--rw-rw-rw-   0 root         (0) root         (0)     1524 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/bond/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22987 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/bond/_bond_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    90634 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/bond/_bond_pricing_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    14745 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/bond/_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.834217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/
--rw-rw-rw-   0 root         (0) root         (0)     1152 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22217 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/_cap_floor_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     7701 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/_cap_floor_pricing_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    12529 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.838217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cds/
--rw-rw-rw-   0 root         (0) root         (0)      678 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cds/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12297 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cds/_cds_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     7675 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cds/_cds_pricing_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     7116 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cds/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    13741 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cds/_premium_leg_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     9673 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cds/_protection_leg_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.838217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cross/
--rw-rw-rw-   0 root         (0) root         (0)      558 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cross/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6350 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cross/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     8601 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     7426 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_leg_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    10264 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_pricing_parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.842217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/
--rw-rw-rw-   0 root         (0) root         (0)     2174 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.846217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_base/
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_base/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_base/_barrier_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_base/_binary_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_base/_info.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_base/_underlying_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     9706 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.846217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_enums/
--rw-rw-rw-   0 root         (0) root         (0)      557 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_enums/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      406 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_enums/_double_binary_type.py
--rw-rw-rw-   0 root         (0) root         (0)      875 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_enums/_fx_binary_type.py
--rw-rw-rw-   0 root         (0) root         (0)      298 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_enums/_settlement_type.py
--rw-rw-rw-   0 root         (0) root         (0)      287 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_enums/_underlying_type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.850217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/
--rw-rw-rw-   0 root         (0) root         (0)      390 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1899 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_barrier_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1861 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_binary_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      989 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_cbbc_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    14031 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      875 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_double_barriers_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     4829 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_fixing_info.py
--rw-rw-rw-   0 root         (0) root         (0)      708 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_underlying_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.854217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4298 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_average_info.py
--rw-rw-rw-   0 root         (0) root         (0)     3798 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_barrier_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2514 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_binary_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    17334 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2164 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_double_barrier_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1303 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_double_barrier_info.py
--rw-rw-rw-   0 root         (0) root         (0)     3848 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_double_binary_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1382 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_dual_currency_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1886 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_forward_start.py
--rw-rw-rw-   0 root         (0) root         (0)      779 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_underlying_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     4201 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_option_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     3709 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_option_instrument_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    30588 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_option_pricing_parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.854217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/repo/
--rw-rw-rw-   0 root         (0) root         (0)      531 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/repo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5861 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/repo/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     8173 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     4865 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     4504 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_pricing_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2984 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_underlying_contract.py
--rw-rw-rw-   0 root         (0) root         (0)     5020 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_underlying_pricing_parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.858217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swap/
--rw-rw-rw-   0 root         (0) root         (0)     1533 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1792 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swap/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     5276 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swap/_swap_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    35872 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swap/_swap_leg_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    10061 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swap/_swap_pricing_parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.862217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swaption/
--rw-rw-rw-   0 root         (0) root         (0)      761 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swaption/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1681 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swaption/_bermudan_swaption_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     7951 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swaption/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    12111 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      612 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_market_data_rule.py
--rw-rw-rw-   0 root         (0) root         (0)     6428 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_pricing_parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.862217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/term_deposit/
--rw-rw-rw-   0 root         (0) root         (0)      400 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/term_deposit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7290 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/term_deposit/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    12438 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/term_deposit/_term_deposit_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     3946 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/term_deposit/_term_deposit_pricing_parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.862217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/
--rw-rw-rw-   0 root         (0) root         (0)      338 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      734 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.862217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/cap/
--rw-rw-rw-   0 root         (0) root         (0)      767 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/cap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2921 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/cap/_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.866217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/eti/
--rw-rw-rw-   0 root         (0) root         (0)      937 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/eti/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2628 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/eti/_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.866217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/fx/
--rw-rw-rw-   0 root         (0) root         (0)      904 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/fx/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2635 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/fx/_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.866217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/swaption/
--rw-rw-rw-   0 root         (0) root         (0)      827 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/swaption/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2994 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/swaption/_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.866217 refinitiv-data-1.3.0/refinitiv/data/content/news/
--rw-rw-rw-   0 root         (0) root         (0)      180 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      343 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/_content_validator_udf.py
--rw-rw-rw-   0 root         (0) root         (0)      289 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)     1455 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/_news_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2464 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/_news_data_provider_layer.py
--rw-rw-rw-   0 root         (0) root         (0)     3276 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/_tools.py
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/_urgency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.870217 refinitiv-data-1.3.0/refinitiv/data/content/news/headlines/
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/headlines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3216 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/headlines/_data.py
--rw-rw-rw-   0 root         (0) root         (0)     5481 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/headlines/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     4929 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/headlines/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2579 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/headlines/_request_factory.py
--rw-rw-rw-   0 root         (0) root         (0)      151 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/headlines/_sort_order.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.870217 refinitiv-data-1.3.0/refinitiv/data/content/news/images/
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/images/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3478 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/images/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     1391 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/images/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2821 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/images/_image.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.874217 refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1295 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     1345 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1120 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)      517 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/_image_data.py
--rw-rw-rw-   0 root         (0) root         (0)      229 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/_news_item.py
--rw-rw-rw-   0 root         (0) root         (0)     1267 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/_report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.874217 refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/hierarchy/
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/hierarchy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      975 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/hierarchy/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)      949 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/hierarchy/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      702 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/hierarchy/_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)      355 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/hierarchy/_report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.874217 refinitiv-data-1.3.0/refinitiv/data/content/news/story/
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/story/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3375 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/story/_data.py
--rw-rw-rw-   0 root         (0) root         (0)      788 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/story/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     1084 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/story/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1752 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/story/_request_factory.py
--rw-rw-rw-   0 root         (0) root         (0)      377 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/story/_response.py
--rw-rw-rw-   0 root         (0) root         (0)      826 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/story/_response_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     1383 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/story/_udf_html_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.878217 refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1316 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     1242 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)      877 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/_top_news_headline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.878217 refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/hierarchy/
--rw-rw-rw-   0 root         (0) root         (0)      111 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/hierarchy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1290 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/hierarchy/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     1271 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/hierarchy/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      898 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/hierarchy/_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)      470 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/hierarchy/_subcategory.py
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/hierarchy/_top_news_id.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.878217 refinitiv-data-1.3.0/refinitiv/data/content/ownership/
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      319 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)      394 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/_enums.py
--rw-rw-rw-   0 root         (0) root         (0)     1721 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/_org_info_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     3986 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/_ownership_data_provider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.882217 refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/
--rw-rw-rw-   0 root         (0) root         (0)      353 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2432 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/_breakdown_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1788 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/_concentration_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2129 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/_investors_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2043 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/_recent_activity_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     3285 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/_shareholders_history_report_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2095 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/_shareholders_report_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1977 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/_top_n_concentration_definition.py
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/breakdown.py
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/concentration.py
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/investors.py
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/recent_activity.py
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/shareholders_history_report.py
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/shareholders_report.py
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/top_n_concentration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.890217 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/
--rw-rw-rw-   0 root         (0) root         (0)      383 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2410 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/_breakdown_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1771 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/_concentration_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2024 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/_holdings_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2156 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/_investors_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2043 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/_recent_activity_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     3197 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/_shareholders_history_report_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2084 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/_shareholders_report_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1945 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/_top_n_concentration_definition.py
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/breakdown.py
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/concentration.py
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/holdings.py
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/investors.py
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/recent_activity.py
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/shareholders_history_report.py
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/shareholders_report.py
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/top_n_concentration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.890217 refinitiv-data-1.3.0/refinitiv/data/content/ownership/insider/
--rw-rw-rw-   0 root         (0) root         (0)      111 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/insider/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2140 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/insider/_shareholders_report_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     3238 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/insider/_transaction_report_definition.py
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/insider/shareholders_report.py
--rw-rw-rw-   0 root         (0) root         (0)       82 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/insider/transaction_report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.890217 refinitiv-data-1.3.0/refinitiv/data/content/ownership/investor/
--rw-rw-rw-   0 root         (0) root         (0)       48 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/investor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2116 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/investor/_holdings_definition.py
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/investor/holdings.py
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/org_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.890217 refinitiv-data-1.3.0/refinitiv/data/content/pricing/
--rw-rw-rw-   0 root         (0) root         (0)      775 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/pricing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3453 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/pricing/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     5313 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/pricing/_pricing_content_provider.py
--rw-rw-rw-   0 root         (0) root         (0)    17807 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/pricing/_stream_facade.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.894217 refinitiv-data-1.3.0/refinitiv/data/content/pricing/chain/
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/pricing/chain/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8116 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/pricing/chain/_chain_record.py
--rw-rw-rw-   0 root         (0) root         (0)     5139 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/pricing/chain/_chain_records.py
--rw-rw-rw-   0 root         (0) root         (0)     1776 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/pricing/chain/_chains_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     3987 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/pricing/chain/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    55563 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/pricing/chain/_display_template.py
--rw-rw-rw-   0 root         (0) root         (0)     8373 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/pricing/chain/_stream.py
--rw-rw-rw-   0 root         (0) root         (0)     4789 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/pricing/chain/_stream_facade.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.898217 refinitiv-data-1.3.0/refinitiv/data/content/search/
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/search/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11914 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/search/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     4249 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/search/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2029 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/search/_lookup_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1066 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/search/_metadata_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1943 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/search/_views.py
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/search/lookup.py
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/search/metadata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.902217 refinitiv-data-1.3.0/refinitiv/data/content/symbol_conversion/
--rw-rw-rw-   0 root         (0) root         (0)      483 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/symbol_conversion/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2824 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/symbol_conversion/_asset_class.py
--rw-rw-rw-   0 root         (0) root         (0)      552 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/symbol_conversion/_asset_state.py
--rw-rw-rw-   0 root         (0) root         (0)     4444 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/symbol_conversion/_country_code.py
--rw-rw-rw-   0 root         (0) root         (0)     7513 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/symbol_conversion/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/symbol_conversion/_symbol_type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.902217 refinitiv-data-1.3.0/refinitiv/data/content/trade_data_service/
--rw-rw-rw-   0 root         (0) root         (0)      227 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/trade_data_service/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3723 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/trade_data_service/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     7718 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/trade_data_service/_stream.py
--rw-rw-rw-   0 root         (0) root         (0)    10810 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/trade_data_service/_stream_facade.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.902217 refinitiv-data-1.3.0/refinitiv/data/delivery/
--rw-rw-rw-   0 root         (0) root         (0)     1266 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.910217 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      654 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_api_type.py
--rw-rw-rw-   0 root         (0) root         (0)      609 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_connection.py
--rw-rw-rw-   0 root         (0) root         (0)     1040 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_data_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     3271 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)    26935 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_data_provider_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     6693 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_data_provider_layer.py
--rw-rw-rw-   0 root         (0) root         (0)      199 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_data_type.py
--rw-rw-rw-   0 root         (0) root         (0)      753 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_endpoint_data.py
--rw-rw-rw-   0 root         (0) root         (0)      914 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_endpoint_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     5634 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_endpoint_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2091 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_parsed_data.py
--rw-rw-rw-   0 root         (0) root         (0)     4021 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_raw_data_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     1411 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_request.py
--rw-rw-rw-   0 root         (0) root         (0)     5778 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_request_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     2097 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_response.py
--rw-rw-rw-   0 root         (0) root         (0)     2506 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_response_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     3617 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_validators.py
--rw-rw-rw-   0 root         (0) root         (0)      363 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_dictionary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.922217 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/
--rw-rw-rw-   0 root         (0) root         (0)      651 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12942 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/_omm_stream.py
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/_protocol_type.py
--rw-rw-rw-   0 root         (0) root         (0)     4906 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/_rdp_stream.py
--rw-rw-rw-   0 root         (0) root         (0)    10068 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/_stream_cxn_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     5401 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/_stream_cxn_config_data.py
--rw-rw-rw-   0 root         (0) root         (0)    11913 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/_stream_cxn_config_provider.py
--rw-rw-rw-   0 root         (0) root         (0)    11442 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/_stream_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     9547 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/_stream_listener.py
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/_stream_type.py
--rw-rw-rw-   0 root         (0) root         (0)      252 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/_validator_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2590 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/base_stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.922217 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/contrib/
--rw-rw-rw-   0 root         (0) root         (0)      216 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/contrib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5529 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/contrib/_funcs.py
--rw-rw-rw-   0 root         (0) root         (0)     2625 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/contrib/_offstream.py
--rw-rw-rw-   0 root         (0) root         (0)     2740 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/contrib/_response.py
--rw-rw-rw-   0 root         (0) root         (0)      185 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/contrib/_stream_connection.py
--rw-rw-rw-   0 root         (0) root         (0)      334 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/contrib/_type.py
--rw-rw-rw-   0 root         (0) root         (0)     2351 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/event.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.926217 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/metadata/
--rw-rw-rw-   0 root         (0) root         (0)      535 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/metadata/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14643 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/metadata/_dictionary.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/metadata/_dictionary_type.py
--rw-rw-rw-   0 root         (0) root         (0)      575 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/metadata/_enum_type_entry.py
--rw-rw-rw-   0 root         (0) root         (0)     1225 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/metadata/_field_description.py
--rw-rw-rw-   0 root         (0) root         (0)      462 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/metadata/_stream.py
--rw-rw-rw-   0 root         (0) root         (0)     6746 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/metadata/_types.py
--rw-rw-rw-   0 root         (0) root         (0)     9811 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/metadata/_validator.py
--rw-rw-rw-   0 root         (0) root         (0)    15911 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/omm_stream.py
--rw-rw-rw-   0 root         (0) root         (0)     6985 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/omm_stream_connection.py
--rw-rw-rw-   0 root         (0) root         (0)     2666 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/omm_stream_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     3929 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/proxy_info.py
--rw-rw-rw-   0 root         (0) root         (0)    10724 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/rdp_stream.py
--rw-rw-rw-   0 root         (0) root         (0)     3085 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/rdp_stream_connection.py
--rw-rw-rw-   0 root         (0) root         (0)     2374 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/rdp_stream_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.926217 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/rwf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/rwf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      779 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/rwf/conversion.py
--rw-rw-rw-   0 root         (0) root         (0)     5403 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/rwf/ema.py
--rw-rw-rw-   0 root         (0) root         (0)     9506 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/rwf/socket.py
--rw-rw-rw-   0 root         (0) root         (0)     4741 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/stream.py
--rw-rw-rw-   0 root         (0) root         (0)     4073 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/stream_cache.py
--rw-rw-rw-   0 root         (0) root         (0)    16512 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/stream_connection.py
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/stream_cxn_state.py
--rw-rw-rw-   0 root         (0) root         (0)      175 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/stream_state.py
--rw-rw-rw-   0 root         (0) root         (0)     3508 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/stream_state_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.926217 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/ws/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/ws/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1344 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/ws/ws_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.934217 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/
--rw-rw-rw-   0 root         (0) root         (0)      824 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3105 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_buckets_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     3480 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_cfs_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     1801 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_data_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1404 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_data_types.py
--rw-rw-rw-   0 root         (0) root         (0)     1120 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_file_downloader.py
--rw-rw-rw-   0 root         (0) root         (0)     1353 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_file_downloader_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      993 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_file_downloader_facade.py
--rw-rw-rw-   0 root         (0) root         (0)     3893 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_file_sets_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2442 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_files_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     4212 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_iter_object.py
--rw-rw-rw-   0 root         (0) root         (0)     2829 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_packages_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_stream.py
--rw-rw-rw-   0 root         (0) root         (0)     1789 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     1140 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_unpacker.py
--rw-rw-rw-   0 root         (0) root         (0)     1036 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/buckets.py
--rw-rw-rw-   0 root         (0) root         (0)      160 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/file_downloader.py
--rw-rw-rw-   0 root         (0) root         (0)     1035 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/file_sets.py
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/files.py
--rw-rw-rw-   0 root         (0) root         (0)      507 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/packages.py
--rw-rw-rw-   0 root         (0) root         (0)      455 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/endpoint_request.py
--rw-rw-rw-   0 root         (0) root         (0)      773 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/omm_stream.py
--rw-rw-rw-   0 root         (0) root         (0)      429 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/rdp_stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.934217 refinitiv-data-1.3.0/refinitiv/data/discovery/
--rw-rw-rw-   0 root         (0) root         (0)      520 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2471 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_convert_symbols.py
--rw-rw-rw-   0 root         (0) root         (0)     2803 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.934217 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_explorer/
--rw-rw-rw-   0 root         (0) root         (0)       94 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_explorer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      608 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_explorer/_buckets_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3509 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_explorer/_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_explorer/_navigator.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_explorer/_properties.py
--rw-rw-rw-   0 root         (0) root         (0)     3610 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_explorer/_property.py
--rw-rw-rw-   0 root         (0) root         (0)      175 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_explorer/_property_type.py
--rw-rw-rw-   0 root         (0) root         (0)     3409 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_explorer/_search_explorer.py
--rw-rw-rw-   0 root         (0) root         (0)     8754 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_explorer/_search_explorer_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.938217 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_templates/
--rw-rw-rw-   0 root         (0) root         (0)      383 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12658 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_templates/base.py
--rw-rw-rw-   0 root         (0) root         (0)     8134 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_templates/embedded.py
--rw-rw-rw-   0 root         (0) root         (0)     5266 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_templates/manage.py
--rw-rw-rw-   0 root         (0) root         (0)     1555 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_templates/namespaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2235 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_templates/search.py
--rw-rw-rw-   0 root         (0) root         (0)      653 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_templates/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.938217 refinitiv-data-1.3.0/refinitiv/data/discovery/_stakeholders/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_stakeholders/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      490 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_stakeholders/_customers.py
--rw-rw-rw-   0 root         (0) root         (0)     4911 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_stakeholders/_fetch_data.py
--rw-rw-rw-   0 root         (0) root         (0)      121 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_stakeholders/_relationship_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1675 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_stakeholders/_stakeholder_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1169 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_stakeholders/_stakeholders.py
--rw-rw-rw-   0 root         (0) root         (0)      491 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_stakeholders/_suppliers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.942217 refinitiv-data-1.3.0/refinitiv/data/discovery/_universe_expanders/
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_universe_expanders/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4156 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_universe_expanders/_chain.py
--rw-rw-rw-   0 root         (0) root         (0)     2562 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_universe_expanders/_discovery_universe.py
--rw-rw-rw-   0 root         (0) root         (0)      393 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_universe_expanders/_peers.py
--rw-rw-rw-   0 root         (0) root         (0)      514 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_universe_expanders/_screener.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_universe_expanders/_universe_expander.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.942217 refinitiv-data-1.3.0/refinitiv/data/early_access/
--rw-rw-rw-   0 root         (0) root         (0)     1298 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/early_access/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.942217 refinitiv-data-1.3.0/refinitiv/data/early_access/discovery/
--rw-rw-rw-   0 root         (0) root         (0)      243 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/early_access/discovery/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.946217 refinitiv-data-1.3.0/refinitiv/data/eikon/
--rw-rw-rw-   0 root         (0) root         (0)      479 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/eikon/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9549 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/eikon/_data_grid.py
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/eikon/_errors.py
--rw-rw-rw-   0 root         (0) root         (0)     8917 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/eikon/_json_requests.py
--rw-rw-rw-   0 root         (0) root         (0)     7401 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/eikon/_news_request.py
--rw-rw-rw-   0 root         (0) root         (0)     1099 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/eikon/_streaming_prices.py
--rw-rw-rw-   0 root         (0) root         (0)     5234 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/eikon/_symbology.py
--rw-rw-rw-   0 root         (0) root         (0)    13670 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/eikon/_time_series.py
--rw-rw-rw-   0 root         (0) root         (0)     4829 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/eikon/_tools.py
--rw-rw-rw-   0 root         (0) root         (0)      780 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.946217 refinitiv-data-1.3.0/refinitiv/data/session/
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/session/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1742 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/session/desktop.py
--rw-rw-rw-   0 root         (0) root         (0)     4202 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/session/platform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.946217 refinitiv-data-1.3.0/refinitiv/data/usage_collection/
--rw-rw-rw-   0 root         (0) root         (0)      359 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/usage_collection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      472 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/usage_collection/_abstract_logger.py
--rw-rw-rw-   0 root         (0) root         (0)      342 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/usage_collection/_filter_types.py
--rw-rw-rw-   0 root         (0) root         (0)     6287 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/usage_collection/_logger.py
--rw-rw-rw-   0 root         (0) root         (0)     1555 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/usage_collection/_utils.py
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/warnings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.950217 refinitiv-data-1.3.0/refinitiv_data.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9778 2023-06-21 15:15:09.000000 refinitiv-data-1.3.0/refinitiv_data.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    55616 2023-06-21 15:15:09.000000 refinitiv-data-1.3.0/refinitiv_data.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 15:15:09.000000 refinitiv-data-1.3.0/refinitiv_data.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      345 2023-06-21 15:15:09.000000 refinitiv-data-1.3.0/refinitiv_data.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-21 15:15:09.000000 refinitiv-data-1.3.0/refinitiv_data.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 15:15:09.950217 refinitiv-data-1.3.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.719793 refinitiv-data-1.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11851 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)    11358 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     9778 2023-07-31 10:28:23.719793 refinitiv-data-1.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     9061 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.399793 refinitiv-data-1.3.1/changes/
+-rw-rw-rw-   0 root         (0) root         (0)      457 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/changes/template.jinja
+-rw-rw-rw-   0 root         (0) root         (0)    21868 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.399793 refinitiv-data-1.3.1/refinitiv/
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.403793 refinitiv-data-1.3.1/refinitiv/data/
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      247 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_base_enum.py
+-rw-rw-rw-   0 root         (0) root         (0)    16816 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_config_defaults.py
+-rw-rw-rw-   0 root         (0) root         (0)     1143 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_config_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)    15270 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_configure.py
+-rw-rw-rw-   0 root         (0) root         (0)     4036 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_content_type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.403793 refinitiv-data-1.3.1/refinitiv/data/_core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-31 10:28:02.000000 refinitiv-data-1.3.1/refinitiv/data/_core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1810 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_core/log_reporter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.415793 refinitiv-data-1.3.1/refinitiv/data/_core/session/
+-rw-rw-rw-   0 root         (0) root         (0)      719 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_core/session/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      245 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_core/session/_dacs_params.py
+-rw-rw-rw-   0 root         (0) root         (0)     3967 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_core/session/_default_session_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     5004 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_core/session/_desktop_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     9961 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_core/session/_platform_session.py
+-rw-rw-rw-   0 root         (0) root         (0)    11808 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_core/session/_retry_transport.py
+-rw-rw-rw-   0 root         (0) root         (0)    15808 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_core/session/_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_core/session/_session_cxn_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_core/session/_session_cxn_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     2472 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_core/session/_session_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    10130 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_core/session/_session_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_core/session/_session_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1086 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_core/session/_user_uuid.py
+-rw-rw-rw-   0 root         (0) root         (0)     3632 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_core/session/access_token_updater.py
+-rw-rw-rw-   0 root         (0) root         (0)    11862 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_core/session/auth_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    10563 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_core/session/connection.py
+-rw-rw-rw-   0 root         (0) root         (0)      660 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_core/session/event.py
+-rw-rw-rw-   0 root         (0) root         (0)     1411 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_core/session/event_code.py
+-rw-rw-rw-   0 root         (0) root         (0)      489 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_core/session/global_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1475 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_core/session/grant_password.py
+-rw-rw-rw-   0 root         (0) root         (0)    12676 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_core/session/http_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      620 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_core/session/null_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     4281 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_core/session/refresh_token_updater.py
+-rw-rw-rw-   0 root         (0) root         (0)     2487 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_core/session/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     3990 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_core/session/updater.py
+-rw-rw-rw-   0 root         (0) root         (0)     2300 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.415793 refinitiv-data-1.3.1/refinitiv/data/_external_libraries/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-31 10:28:02.000000 refinitiv-data-1.3.1/refinitiv/data/_external_libraries/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.419793 refinitiv-data-1.3.1/refinitiv/data/_external_libraries/python_configuration/
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_external_libraries/python_configuration/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)    26229 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_external_libraries/python_configuration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11923 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_external_libraries/python_configuration/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     7238 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_external_libraries/python_configuration/configuration_set.py
+-rw-rw-rw-   0 root         (0) root         (0)     5845 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_external_libraries/python_configuration/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.427793 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/
+-rw-rw-rw-   0 root         (0) root         (0)      608 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5350 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/_containers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2141 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/_data_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)    12224 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     4588 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/_history_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)      711 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/_history_df_builder_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1500 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/_intervals_consts.py
+-rw-rw-rw-   0 root         (0) root         (0)     3454 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/_mixed_streams.py
+-rw-rw-rw-   0 root         (0) root         (0)     5066 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/_ohlc_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)    12099 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/_pricing_recorder.py
+-rw-rw-rw-   0 root         (0) root         (0)     5290 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/_recording_control.py
+-rw-rw-rw-   0 root         (0) root         (0)     3110 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/_stream_update_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.431793 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/context_collection/
+-rw-rw-rw-   0 root         (0) root         (0)      335 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/context_collection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2993 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/context_collection/_adc_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     1950 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/context_collection/_adc_rdp_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     1979 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/context_collection/_adc_udf_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/context_collection/_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     3186 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/context_collection/_context_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     4950 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/context_collection/_cust_inst_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     2854 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/context_collection/_cust_inst_rdp_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     2250 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/context_collection/_cust_inst_udf_context.py
+-rw-rw-rw-   0 root         (0) root         (0)      755 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/context_collection/_hp_and_cust_inst_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     2678 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/context_collection/_hp_context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.431793 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/dates_and_calendars/
+-rw-rw-rw-   0 root         (0) root         (0)      659 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/dates_and_calendars/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2482 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/dates_and_calendars/_add_periods.py
+-rw-rw-rw-   0 root         (0) root         (0)     2504 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/dates_and_calendars/_count_periods.py
+-rw-rw-rw-   0 root         (0) root         (0)     3621 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/dates_and_calendars/_date_schedule.py
+-rw-rw-rw-   0 root         (0) root         (0)     4581 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/dates_and_calendars/_holidays.py
+-rw-rw-rw-   0 root         (0) root         (0)     1410 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/dates_and_calendars/_is_working_day.py
+-rw-rw-rw-   0 root         (0) root         (0)     3914 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/get_data_func.py
+-rw-rw-rw-   0 root         (0) root         (0)     7418 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/get_history_func.py
+-rw-rw-rw-   0 root         (0) root         (0)     3417 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/get_stream.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.431793 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/news/
+-rw-rw-rw-   0 root         (0) root         (0)      280 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/news/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2306 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/news/_news.py
+-rw-rw-rw-   0 root         (0) root         (0)     2804 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/session.py
+-rw-rw-rw-   0 root         (0) root         (0)    12912 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_log.py
+-rw-rw-rw-   0 root         (0) root         (0)      338 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_open_state.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.435793 refinitiv-data-1.3.1/refinitiv/data/_qpl/
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_qpl/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      641 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_qpl/_bid_ask.py
+-rw-rw-rw-   0 root         (0) root         (0)     2781 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_qpl/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)      766 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_qpl/_fx_spot_quote.py
+-rw-rw-rw-   0 root         (0) root         (0)     2001 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_qpl/_fx_swap_points.py
+-rw-rw-rw-   0 root         (0) root         (0)     3727 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_qpl/_fx_swp_to_swp.py
+-rw-rw-rw-   0 root         (0) root         (0)      888 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_qpl/_serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)      760 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_qpl/_tenor_bid_ask.py
+-rw-rw-rw-   0 root         (0) root         (0)      220 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_qpl/_tenor_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.439793 refinitiv-data-1.3.1/refinitiv/data/_tools/
+-rw-rw-rw-   0 root         (0) root         (0)      213 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13407 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_tools/_common.py
+-rw-rw-rw-   0 root         (0) root         (0)     1208 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_tools/_converter.py
+-rw-rw-rw-   0 root         (0) root         (0)     6623 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_tools/_dataframe.py
+-rw-rw-rw-   0 root         (0) root         (0)     4708 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_tools/_datetime.py
+-rw-rw-rw-   0 root         (0) root         (0)       53 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_tools/_debug.py
+-rw-rw-rw-   0 root         (0) root         (0)     1744 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_tools/_params.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_tools/_patterns.py
+-rw-rw-rw-   0 root         (0) root         (0)     1083 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_tools/_repr.py
+-rw-rw-rw-   0 root         (0) root         (0)     1317 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_tools/_specification.py
+-rw-rw-rw-   0 root         (0) root         (0)     2196 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_tools/_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5257 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_tools/templates.py
+-rw-rw-rw-   0 root         (0) root         (0)      731 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/_types.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-07-31 10:28:22.000000 refinitiv-data-1.3.1/refinitiv/data/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.447793 refinitiv-data-1.3.1/refinitiv/data/content/
+-rw-rw-rw-   0 root         (0) root         (0)     2082 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      510 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/_content_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1195 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/_content_data_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1094 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/_content_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     3533 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/_content_provider_layer.py
+-rw-rw-rw-   0 root         (0) root         (0)      620 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/_content_response_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/_df_build_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    18497 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)     8547 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/_df_builder_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)    18264 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/_entire_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)      829 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/_error_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1970 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/_historical_content_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     6441 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/_historical_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     6937 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/_historical_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)     2895 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/_historical_raw_transf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3209 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/_historical_response_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3064 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/_intervals.py
+-rw-rw-rw-   0 root         (0) root         (0)     1593 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/_universe_content_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     8436 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/_universe_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)    18431 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/_universe_streams.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.455793 refinitiv-data-1.3.1/refinitiv/data/content/custom_instruments/
+-rw-rw-rw-   0 root         (0) root         (0)      467 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/custom_instruments/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14446 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/custom_instruments/_custom_instruments_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     2160 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/custom_instruments/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      801 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/custom_instruments/_enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     2415 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/custom_instruments/_events.py
+-rw-rw-rw-   0 root         (0) root         (0)     6061 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/custom_instruments/_instrument_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12895 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/custom_instruments/_instrument_prop_classes.py
+-rw-rw-rw-   0 root         (0) root         (0)    18090 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/custom_instruments/_manage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/custom_instruments/_search.py
+-rw-rw-rw-   0 root         (0) root         (0)     8665 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/custom_instruments/_stream_facade.py
+-rw-rw-rw-   0 root         (0) root         (0)     2941 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/custom_instruments/_summaries.py
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/custom_instruments/events.py
+-rw-rw-rw-   0 root         (0) root         (0)      662 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/custom_instruments/manage.py
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/custom_instruments/search.py
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/custom_instruments/summaries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.459793 refinitiv-data-1.3.1/refinitiv/data/content/esg/
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/esg/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1478 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/esg/_base_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/esg/_basic_overview_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1165 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/esg/_esg_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     1631 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/esg/_full_measures_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1665 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/esg/_full_scores_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1911 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/esg/_standard_measures_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1652 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/esg/_standard_scores_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1189 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/esg/_universe_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/esg/basic_overview.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.463793 refinitiv-data-1.3.1/refinitiv/data/content/esg/bulk/
+-rw-rw-rw-   0 root         (0) root         (0)      143 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/esg/bulk/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3858 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/esg/bulk/_actions.py
+-rw-rw-rw-   0 root         (0) root         (0)     9784 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/esg/bulk/_db_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1848 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/esg/bulk/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      351 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/esg/bulk/_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)      309 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/esg/bulk/_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     7363 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/esg/bulk/_file_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     3264 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/esg/bulk/_package_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1333 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/esg/bulk/_package_manager_facade.py
+-rw-rw-rw-   0 root         (0) root         (0)     2562 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/esg/bulk/_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/esg/full_measures.py
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/esg/full_scores.py
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/esg/standard_measures.py
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/esg/standard_scores.py
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/esg/universe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.463793 refinitiv-data-1.3.1/refinitiv/data/content/estimates/
+-rw-rw-rw-   0 root         (0) root         (0)     1093 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1246 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)      475 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/_enums.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.463793 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_actuals/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_actuals/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2175 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_actuals/_annual_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2156 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_actuals/_interim_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_actuals/annual.py
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_actuals/interim.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.463793 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_actuals_kpi/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_actuals_kpi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1789 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_actuals_kpi/_annual_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1793 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_actuals_kpi/_interim_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_actuals_kpi/annual.py
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_actuals_kpi/interim.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.467793 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary/
+-rw-rw-rw-   0 root         (0) root         (0)      581 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2146 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary/_annual_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2299 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary/_historical_snapshots_non_periodic_measures_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2314 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary/_historical_snapshots_periodic_measures_annual_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2305 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary/_historical_snapshots_periodic_measures_interim_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2268 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary/_historical_snapshots_recommendations_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2150 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary/_interim_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2190 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary/_non_periodic_measures_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2135 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary/_recommendations_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary/annual.py
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary/historical_snapshots_non_periodic_measures.py
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary/historical_snapshots_periodic_measures_annual.py
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary/historical_snapshots_periodic_measures_interim.py
+-rw-rw-rw-   0 root         (0) root         (0)      100 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary/historical_snapshots_recommendations.py
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary/interim.py
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary/non_periodic_measures.py
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary/recommendations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.471793 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary_kpi/
+-rw-rw-rw-   0 root         (0) root         (0)      117 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary_kpi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1771 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary_kpi/_annual_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1851 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary_kpi/_historical_snapshots_kpi_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1776 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary_kpi/_interim_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary_kpi/annual.py
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary_kpi/historical_snapshots_kpi.py
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary_kpi/interim.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.475793 refinitiv-data-1.3.1/refinitiv/data/content/filings/
+-rw-rw-rw-   0 root         (0) root         (0)      117 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/filings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/filings/_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)      304 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/filings/_feed_name.py
+-rw-rw-rw-   0 root         (0) root         (0)     4584 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/filings/_filing_query.py
+-rw-rw-rw-   0 root         (0) root         (0)    20076 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/filings/_retrieval_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     2697 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/filings/_retrieval_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     8827 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/filings/_search_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     4866 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/filings/_search_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/filings/retrieval.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/filings/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.479793 refinitiv-data-1.3.1/refinitiv/data/content/fundamental_and_reference/
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/fundamental_and_reference/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3970 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/fundamental_and_reference/_content_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2041 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/fundamental_and_reference/_data_grid_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      821 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/fundamental_and_reference/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)    10675 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/fundamental_and_reference/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2746 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/fundamental_and_reference/_request_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/fundamental_and_reference/_response_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.479793 refinitiv-data-1.3.1/refinitiv/data/content/historical_pricing/
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/historical_pricing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3077 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/historical_pricing/_enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     2949 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/historical_pricing/_events_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      762 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/historical_pricing/_historical_pricing_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     3718 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/historical_pricing/_historical_pricing_request_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3471 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/historical_pricing/_summaries_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      264 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/historical_pricing/events.py
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/historical_pricing/summaries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.483793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/
+-rw-rw-rw-   0 root         (0) root         (0)      192 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5727 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_content_provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.491793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/
+-rw-rw-rw-   0 root         (0) root         (0)      383 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.491793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.495793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/
+-rw-rw-rw-   0 root         (0) root         (0)      140 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1293 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_constituents.py
+-rw-rw-rw-   0 root         (0) root         (0)    11462 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_curve_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    28240 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_curve_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2919 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.503793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/
+-rw-rw-rw-   0 root         (0) root         (0)      565 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      311 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_basis_spline_smooth_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1833 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_business_sector.py
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_calendar_adjustment.py
+-rw-rw-rw-   0 root         (0) root         (0)      217 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_calibration_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2943 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_curve_sub_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      654 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_economic_sector.py
+-rw-rw-rw-   0 root         (0) root         (0)     8933 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_industry.py
+-rw-rw-rw-   0 root         (0) root         (0)     3834 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_industry_group.py
+-rw-rw-rw-   0 root         (0) root         (0)     1223 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_interest_calculation_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      599 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_interpolation_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_issuer_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_main_constituent_asset_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      146 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_price_side.py
+-rw-rw-rw-   0 root         (0) root         (0)     1283 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_rating.py
+-rw-rw-rw-   0 root         (0) root         (0)      216 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_rating_scale_source.py
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_reference_entity_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      238 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_seniority.py
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.503793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.507793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/
+-rw-rw-rw-   0 root         (0) root         (0)      514 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4482 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_butterfly_shift.py
+-rw-rw-rw-   0 root         (0) root         (0)     6770 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_combined_shift.py
+-rw-rw-rw-   0 root         (0) root         (0)     9677 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_curve_definition_pricing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.511793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/
+-rw-rw-rw-   0 root         (0) root         (0)      179 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      194 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/_array_main_constituent_asset_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      146 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/_array_risk_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      216 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/_constituent_override_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      222 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/_shift_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      171 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/_shift_unit.py
+-rw-rw-rw-   0 root         (0) root         (0)     3924 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_flattening_shift.py
+-rw-rw-rw-   0 root         (0) root         (0)     1356 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_constituents.py
+-rw-rw-rw-   0 root         (0) root         (0)     5452 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_curve_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     5860 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_curve_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2463 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_shift_scenario.py
+-rw-rw-rw-   0 root         (0) root         (0)     3920 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_long_end_shift.py
+-rw-rw-rw-   0 root         (0) root         (0)     3921 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_parallel_shift.py
+-rw-rw-rw-   0 root         (0) root         (0)     3719 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     7749 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_shift_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     3921 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_short_end_shift.py
+-rw-rw-rw-   0 root         (0) root         (0)     6772 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_time_bucket_shift.py
+-rw-rw-rw-   0 root         (0) root         (0)     4477 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_twist_shift.py
+-rw-rw-rw-   0 root         (0) root         (0)      483 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.519793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2943 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_base_definition_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1236 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_bid_ask_fields_description.py
+-rw-rw-rw-   0 root         (0) root         (0)     1158 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_bid_ask_fields_formula_description.py
+-rw-rw-rw-   0 root         (0) root         (0)     3593 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_constituents_description.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.519793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3767 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/_curve_definition_description.py
+-rw-rw-rw-   0 root         (0) root         (0)     1492 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     1997 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_curve_parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.519793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_delete/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_delete/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_delete/_request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.519793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_enums/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_enums/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_enums/_quotation_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      186 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_enums/_standard_turn_period.py
+-rw-rw-rw-   0 root         (0) root         (0)     1716 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_field_description.py
+-rw-rw-rw-   0 root         (0) root         (0)     2176 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_field_formula_description.py
+-rw-rw-rw-   0 root         (0) root         (0)     2164 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_formula_parameter_description.py
+-rw-rw-rw-   0 root         (0) root         (0)     3621 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_instrument_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2568 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_instrument_description.py
+-rw-rw-rw-   0 root         (0) root         (0)      940 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_turn_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     1899 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_spot_instrument_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2623 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_spot_instrument_description.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.519793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7044 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/_curve_definition_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)      915 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     2871 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instrument_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2664 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instrument_description.py
+-rw-rw-rw-   0 root         (0) root         (0)     2078 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instruments_segment.py
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_mixin_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     1745 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_bid_ask.py
+-rw-rw-rw-   0 root         (0) root         (0)     1038 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_bid_ask_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     2285 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_fx_forward_turn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.519793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_search/
+-rw-rw-rw-   0 root         (0) root         (0)       42 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_search/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8798 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_search/_curve_get_definition_item.py
+-rw-rw-rw-   0 root         (0) root         (0)      900 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_turn_adjustment.py
+-rw-rw-rw-   0 root         (0) root         (0)      657 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.523793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3896 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/_curve_update_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1494 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/_request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.523793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_enums/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_enums/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_enums/_interpolation_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      160 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_enums/_main_constituent_asset_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_enums/_risk_type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.523793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_triangulate_definitions/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_triangulate_definitions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3353 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_triangulate_definitions/_request.py
+-rw-rw-rw-   0 root         (0) root         (0)      186 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_types.py
+-rw-rw-rw-   0 root         (0) root         (0)    21263 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_curves_builder_df.py
+-rw-rw-rw-   0 root         (0) root         (0)    10677 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_curves_data_provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.527793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_enums/
+-rw-rw-rw-   0 root         (0) root         (0)      574 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_enums/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      171 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_enums/_calendar_adjustment.py
+-rw-rw-rw-   0 root         (0) root         (0)      242 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_enums/_compounding_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      172 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_enums/_constituent_override_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_enums/_forward_curves_outputs.py
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_enums/_instrument_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      170 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_enums/_main_constituent_asset_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_enums/_market_data_access_denied_fallback.py
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_enums/_swap_price_side.py
+-rw-rw-rw-   0 root         (0) root         (0)      201 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_enums/_zc_curves_outputs.py
+-rw-rw-rw-   0 root         (0) root         (0)      616 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_enums/_zc_interpolation_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)     2832 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_forward_curve_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     3441 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_forward_curve_request_item.py
+-rw-rw-rw-   0 root         (0) root         (0)      930 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_forward_curve_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.531793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_models/
+-rw-rw-rw-   0 root         (0) root         (0)      234 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_models/_constituents.py
+-rw-rw-rw-   0 root         (0) root         (0)     1567 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_models/_convexity.py
+-rw-rw-rw-   0 root         (0) root         (0)     3893 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_models/_curve.py
+-rw-rw-rw-   0 root         (0) root         (0)      261 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_models/_curve_point.py
+-rw-rw-rw-   0 root         (0) root         (0)      746 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_models/_instrument.py
+-rw-rw-rw-   0 root         (0) root         (0)    13718 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_models/_interest_rate_curve_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1737 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_models/_par_rate_shift.py
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_models/_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1426 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_models/_turn.py
+-rw-rw-rw-   0 root         (0) root         (0)     3014 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_models/_valuation_time.py
+-rw-rw-rw-   0 root         (0) root         (0)     2213 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_shift_scenario.py
+-rw-rw-rw-   0 root         (0) root         (0)    10434 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_swap_zc_curve_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    19827 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_swap_zc_curve_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     8802 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_zc_curve_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     4209 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_zc_curve_definition_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    12838 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_zc_curve_definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)    19563 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_zc_curve_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2988 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_zc_curve_request_item.py
+-rw-rw-rw-   0 root         (0) root         (0)      726 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_zc_curve_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.551793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/
+-rw-rw-rw-   0 root         (0) root         (0)     3130 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_adjust_interest_to_payment_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_american_monte_carlo_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_amortization_frequency.py
+-rw-rw-rw-   0 root         (0) root         (0)      208 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_amortization_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_asset_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      273 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_average_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      365 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_axis.py
+-rw-rw-rw-   0 root         (0) root         (0)      281 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_barrier_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      184 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_barrier_style.py
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_barrier_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_benchmark_yield_selection_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_binary_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      960 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_business_day_convention.py
+-rw-rw-rw-   0 root         (0) root         (0)      415 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_buy_sell.py
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_calibration_strategy.py
+-rw-rw-rw-   0 root         (0) root         (0)      405 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_call_put.py
+-rw-rw-rw-   0 root         (0) root         (0)      390 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_cds_convention.py
+-rw-rw-rw-   0 root         (0) root         (0)      763 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_common_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_credit_spread_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_date_moving_convention.py
+-rw-rw-rw-   0 root         (0) root         (0)      735 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_date_rolling_convention.py
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_dates_calendars_frequency.py
+-rw-rw-rw-   0 root         (0) root         (0)     1225 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_day_count_basis.py
+-rw-rw-rw-   0 root         (0) root         (0)      726 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_day_of_week.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_direction.py
+-rw-rw-rw-   0 root         (0) root         (0)      201 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_discounting_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      250 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_dividend_extrapolation.py
+-rw-rw-rw-   0 root         (0) root         (0)      342 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_dividend_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      456 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_doc_clause.py
+-rw-rw-rw-   0 root         (0) root         (0)      175 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_double_binary_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      381 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_end_of_month_convention.py
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_equity_dividend_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      194 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_eti_input_volatility_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      210 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_exercise_schedule_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      645 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_exercise_style.py
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_extrapolation_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      289 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_fixing_frequency.py
+-rw-rw-rw-   0 root         (0) root         (0)      282 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_format.py
+-rw-rw-rw-   0 root         (0) root         (0)      269 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_forward_compute_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      299 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_forward_extrapolation.py
+-rw-rw-rw-   0 root         (0) root         (0)      906 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_frequency.py
+-rw-rw-rw-   0 root         (0) root         (0)      393 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_funding_spread_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_fx_binary_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      299 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_fx_cross_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      274 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_fx_leg_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      644 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_fx_swap_calculation_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_fx_volatility_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      823 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_holiday_outupts.py
+-rw-rw-rw-   0 root         (0) root         (0)      233 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_implied_deposit_date_convention.py
+-rw-rw-rw-   0 root         (0) root         (0)      140 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_in_or_out.py
+-rw-rw-rw-   0 root         (0) root         (0)      319 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_index_average_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      644 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_index_compounding_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_index_convexity_adjustment_integration_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      260 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_index_convexity_adjustment_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_index_convexity_adjustment_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_index_observation_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      337 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_index_reset_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_index_spread_compounding_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_inflation_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_input_volatility_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      211 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_interest_calculation_convention.py
+-rw-rw-rw-   0 root         (0) root         (0)      301 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_interest_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      311 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_interpolation_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      380 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_local_volatility_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      227 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_notional_exchange.py
+-rw-rw-rw-   0 root         (0) root         (0)      281 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_numeraire_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      207 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_option_volatility_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      625 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_period_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      192 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_premium_settlement_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_price_side.py
+-rw-rw-rw-   0 root         (0) root         (0)      301 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_pricing_model_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_projected_index_calculation_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      614 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_quote_fallback_logic.py
+-rw-rw-rw-   0 root         (0) root         (0)     2113 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_redemption_date_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      213 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_repo_curve_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      145 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_risk_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_rounding.py
+-rw-rw-rw-   0 root         (0) root         (0)      304 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_rounding_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      757 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_seniority.py
+-rw-rw-rw-   0 root         (0) root         (0)      208 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_settlement_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      247 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_status.py
+-rw-rw-rw-   0 root         (0) root         (0)     1545 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_stub_rule.py
+-rw-rw-rw-   0 root         (0) root         (0)      184 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_swaption_settlement_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      160 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_swaption_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      205 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_swaption_volatility_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_tenor_reference_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      316 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_time_stamp.py
+-rw-rw-rw-   0 root         (0) root         (0)      189 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_underlying_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      143 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_up_or_down.py
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_vol_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      343 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_volatility_adjustment_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      222 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_volatility_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      184 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_volatility_term_structure_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      172 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_volatility_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      913 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_yield_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    10539 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_ipa_content_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     1402 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_ipa_content_validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.555793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_models/
+-rw-rw-rw-   0 root         (0) root         (0)      433 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1898 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_models/_american_monte_carlo_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     3960 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_models/_amortization_item.py
+-rw-rw-rw-   0 root         (0) root         (0)     2188 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_models/_barrier_definition_element.py
+-rw-rw-rw-   0 root         (0) root         (0)      917 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_models/_basket_item.py
+-rw-rw-rw-   0 root         (0) root         (0)     1163 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_models/_bid_ask_mid.py
+-rw-rw-rw-   0 root         (0) root         (0)     5046 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_models/_bond_rounding_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_models/_day_weight.py
+-rw-rw-rw-   0 root         (0) root         (0)     2295 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_models/_fx_point.py
+-rw-rw-rw-   0 root         (0) root         (0)     2157 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_models/_input_flow.py
+-rw-rw-rw-   0 root         (0) root         (0)     1846 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_models/_interpolation_weight.py
+-rw-rw-rw-   0 root         (0) root         (0)     1531 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_models/_numerical_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      948 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_models/_payout_scaling.py
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_models/_pde_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     4806 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_object_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.563793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1842 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_cap_surface_request_item.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.567793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_enums/
+-rw-rw-rw-   0 root         (0) root         (0)      423 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_enums/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      246 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_enums/_calibration_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_enums/_moneyness_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      485 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_enums/_outputs.py
+-rw-rw-rw-   0 root         (0) root         (0)      146 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_enums/_strike_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_enums/_volatility_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     3061 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_eti_surface_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     9016 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_eti_surface_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1692 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_eti_surface_request_item.py
+-rw-rw-rw-   0 root         (0) root         (0)     1708 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_fx_statistics_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)      777 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_fx_surface_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    13552 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_fx_surface_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2545 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_fx_surface_request_item.py
+-rw-rw-rw-   0 root         (0) root         (0)     2694 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_i_ir_vol_model_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     9639 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_i_ir_vol_model_pricing_parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.567793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_models/
+-rw-rw-rw-   0 root         (0) root         (0)      351 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2541 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_models/_maturity_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2477 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_models/_moneyness_weight.py
+-rw-rw-rw-   0 root         (0) root         (0)     1214 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_models/_strike_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2290 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_models/_strike_filter_range.py
+-rw-rw-rw-   0 root         (0) root         (0)     5195 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_models/_surface.py
+-rw-rw-rw-   0 root         (0) root         (0)     6749 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_models/_surface_filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     5848 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_models/_surface_output.py
+-rw-rw-rw-   0 root         (0) root         (0)      294 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_models/_surface_point.py
+-rw-rw-rw-   0 root         (0) root         (0)     1145 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_models/_volatility_surface_point.py
+-rw-rw-rw-   0 root         (0) root         (0)     1575 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_surface_request_item.py
+-rw-rw-rw-   0 root         (0) root         (0)      468 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_surface_types.py
+-rw-rw-rw-   0 root         (0) root         (0)    11119 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_surfaces_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)    14482 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_swaption_calculation_params.py
+-rw-rw-rw-   0 root         (0) root         (0)     3498 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_swaption_surface_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1853 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_swaption_surface_request_item.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.567793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.571793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/_bond_curves/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/_bond_curves/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.571793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/_bond_curves/curves/
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/_bond_curves/curves/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2737 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/_bond_curves/curves/_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.571793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      472 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/_arg_enums.py
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/_base_data_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.571793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/curves/
+-rw-rw-rw-   0 root         (0) root         (0)     1424 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/curves/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3000 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/curves/_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.575793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/
+-rw-rw-rw-   0 root         (0) root         (0)     2037 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7353 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_data_classes.py
+-rw-rw-rw-   0 root         (0) root         (0)    11268 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_manage.py
+-rw-rw-rw-   0 root         (0) root         (0)     4906 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_search.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/manage.py
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.575793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5917 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     2900 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/_search.py
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.575793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/forward_curves/
+-rw-rw-rw-   0 root         (0) root         (0)      945 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/forward_curves/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6123 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/forward_curves/_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.575793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/zc_curve_definitions/
+-rw-rw-rw-   0 root         (0) root         (0)      186 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/zc_curve_definitions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5023 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/zc_curve_definitions/_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.575793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/zc_curves/
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/zc_curves/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4232 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/zc_curves/_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.579793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1829 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/_base_request_items.py
+-rw-rw-rw-   0 root         (0) root         (0)      976 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/_content_data_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)      560 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/_request_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.579793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/add_periods/
+-rw-rw-rw-   0 root         (0) root         (0)      260 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/add_periods/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2081 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/add_periods/_add_periods_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)    10019 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/add_periods/_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.579793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/count_periods/
+-rw-rw-rw-   0 root         (0) root         (0)      172 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/count_periods/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8278 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/count_periods/_count_periods.py
+-rw-rw-rw-   0 root         (0) root         (0)     1860 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/count_periods/_count_periods_data_provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.579793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/
+-rw-rw-rw-   0 root         (0) root         (0)      158 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6938 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/_date_schedule.py
+-rw-rw-rw-   0 root         (0) root         (0)      933 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/_date_schedule_data_provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.583793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/holidays/
+-rw-rw-rw-   0 root         (0) root         (0)      143 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/holidays/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7269 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/holidays/_holidays.py
+-rw-rw-rw-   0 root         (0) root         (0)     3486 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/holidays/_holidays_data_provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.583793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6928 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/_is_working_day.py
+-rw-rw-rw-   0 root         (0) root         (0)     2388 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/_is_working_day_data_provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.587793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/
+-rw-rw-rw-   0 root         (0) root         (0)      483 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2463 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/_base_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     8331 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/_contracts_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     3681 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1036 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/_instrument_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     3717 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/_quantitative_data_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)     3615 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/_stream_facade.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.587793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/bond/
+-rw-rw-rw-   0 root         (0) root         (0)     1524 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/bond/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22987 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/bond/_bond_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    90634 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/bond/_bond_pricing_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    14745 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/bond/_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.591793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/cap_floor/
+-rw-rw-rw-   0 root         (0) root         (0)     1152 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/cap_floor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22217 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/cap_floor/_cap_floor_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     7701 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/cap_floor/_cap_floor_pricing_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    12529 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/cap_floor/_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.595793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/cds/
+-rw-rw-rw-   0 root         (0) root         (0)      678 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/cds/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12297 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/cds/_cds_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     7675 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/cds/_cds_pricing_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     7116 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/cds/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    13741 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/cds/_premium_leg_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     9673 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/cds/_protection_leg_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.599793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/cross/
+-rw-rw-rw-   0 root         (0) root         (0)      558 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/cross/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6350 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/cross/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     8601 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     7426 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_leg_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    10264 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_pricing_parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.599793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/
+-rw-rw-rw-   0 root         (0) root         (0)     2174 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.603793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_base/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_base/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_base/_barrier_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_base/_binary_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_base/_info.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_base/_underlying_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     9706 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.603793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_enums/
+-rw-rw-rw-   0 root         (0) root         (0)      557 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_enums/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      406 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_enums/_double_binary_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      875 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_enums/_fx_binary_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      298 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_enums/_settlement_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      287 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_enums/_underlying_type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.607793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_eti/
+-rw-rw-rw-   0 root         (0) root         (0)      390 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_eti/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1899 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_barrier_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1861 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_binary_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      989 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_cbbc_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    14031 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      875 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_double_barriers_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     4829 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_fixing_info.py
+-rw-rw-rw-   0 root         (0) root         (0)      708 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_underlying_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.611793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_fx/
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_fx/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4298 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_average_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     3798 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_barrier_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2514 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_binary_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    17334 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2164 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_double_barrier_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_double_barrier_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     3848 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_double_binary_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1382 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_dual_currency_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1886 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_forward_start.py
+-rw-rw-rw-   0 root         (0) root         (0)      779 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_underlying_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     4201 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_option_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     3709 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_option_instrument_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    30588 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_option_pricing_parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.611793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/repo/
+-rw-rw-rw-   0 root         (0) root         (0)      531 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/repo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5861 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/repo/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     8173 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/repo/_repo_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     4865 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/repo/_repo_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     4504 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/repo/_repo_pricing_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2984 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/repo/_repo_underlying_contract.py
+-rw-rw-rw-   0 root         (0) root         (0)     5020 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/repo/_repo_underlying_pricing_parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.615793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/swap/
+-rw-rw-rw-   0 root         (0) root         (0)     1533 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/swap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1792 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/swap/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     5276 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/swap/_swap_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    35872 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/swap/_swap_leg_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    10061 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/swap/_swap_pricing_parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.619793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/swaption/
+-rw-rw-rw-   0 root         (0) root         (0)      761 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/swaption/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/swaption/_bermudan_swaption_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     7951 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/swaption/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    12111 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      612 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_market_data_rule.py
+-rw-rw-rw-   0 root         (0) root         (0)     6428 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_pricing_parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.619793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/term_deposit/
+-rw-rw-rw-   0 root         (0) root         (0)      400 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/term_deposit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7290 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/term_deposit/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    12438 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/term_deposit/_term_deposit_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     3946 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/term_deposit/_term_deposit_pricing_parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.619793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/surfaces/
+-rw-rw-rw-   0 root         (0) root         (0)      338 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/surfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      734 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/surfaces/_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.623793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/surfaces/cap/
+-rw-rw-rw-   0 root         (0) root         (0)      767 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/surfaces/cap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2921 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/surfaces/cap/_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.623793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/surfaces/eti/
+-rw-rw-rw-   0 root         (0) root         (0)      937 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/surfaces/eti/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2628 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/surfaces/eti/_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.623793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/surfaces/fx/
+-rw-rw-rw-   0 root         (0) root         (0)      904 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/surfaces/fx/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2635 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/surfaces/fx/_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.623793 refinitiv-data-1.3.1/refinitiv/data/content/ipa/surfaces/swaption/
+-rw-rw-rw-   0 root         (0) root         (0)      827 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/surfaces/swaption/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2994 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ipa/surfaces/swaption/_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.623793 refinitiv-data-1.3.1/refinitiv/data/content/news/
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      343 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/_content_validator_udf.py
+-rw-rw-rw-   0 root         (0) root         (0)      289 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)     1455 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/_news_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2464 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/_news_data_provider_layer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3276 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/_urgency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.627793 refinitiv-data-1.3.1/refinitiv/data/content/news/headlines/
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/headlines/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3216 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/headlines/_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     5481 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/headlines/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     4929 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/headlines/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2579 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/headlines/_request_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)      151 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/headlines/_sort_order.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.627793 refinitiv-data-1.3.1/refinitiv/data/content/news/images/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/images/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3478 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/images/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     1391 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/images/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2821 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/images/_image.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.631793 refinitiv-data-1.3.1/refinitiv/data/content/news/online_reports/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/online_reports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1295 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/online_reports/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     1345 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/online_reports/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1120 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/online_reports/_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)      517 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/online_reports/_image_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      229 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/online_reports/_news_item.py
+-rw-rw-rw-   0 root         (0) root         (0)     1267 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/online_reports/_report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.631793 refinitiv-data-1.3.1/refinitiv/data/content/news/online_reports/hierarchy/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/online_reports/hierarchy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      975 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/online_reports/hierarchy/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)      949 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/online_reports/hierarchy/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      702 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/online_reports/hierarchy/_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)      355 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/online_reports/hierarchy/_report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.635793 refinitiv-data-1.3.1/refinitiv/data/content/news/story/
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/story/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3375 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/story/_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      788 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/story/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     1084 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/story/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1752 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/story/_request_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)      377 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/story/_response.py
+-rw-rw-rw-   0 root         (0) root         (0)      826 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/story/_response_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1383 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/story/_udf_html_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.635793 refinitiv-data-1.3.1/refinitiv/data/content/news/top_news/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/top_news/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1316 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/top_news/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     1242 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/top_news/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      823 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/top_news/_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)      877 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/top_news/_top_news_headline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.635793 refinitiv-data-1.3.1/refinitiv/data/content/news/top_news/hierarchy/
+-rw-rw-rw-   0 root         (0) root         (0)      111 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/top_news/hierarchy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1290 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/top_news/hierarchy/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     1271 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/top_news/hierarchy/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      898 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/top_news/hierarchy/_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)      470 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/top_news/hierarchy/_subcategory.py
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/news/top_news/hierarchy/_top_news_id.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.639793 refinitiv-data-1.3.1/refinitiv/data/content/ownership/
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      319 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)      394 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/_enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     1721 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/_org_info_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     3986 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/_ownership_data_provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.643793 refinitiv-data-1.3.1/refinitiv/data/content/ownership/consolidated/
+-rw-rw-rw-   0 root         (0) root         (0)      353 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/consolidated/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2432 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/consolidated/_breakdown_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1788 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/consolidated/_concentration_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2129 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/consolidated/_investors_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2043 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/consolidated/_recent_activity_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     3285 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/consolidated/_shareholders_history_report_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2095 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/consolidated/_shareholders_report_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1977 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/consolidated/_top_n_concentration_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/consolidated/breakdown.py
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/consolidated/concentration.py
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/consolidated/investors.py
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/consolidated/recent_activity.py
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/consolidated/shareholders_history_report.py
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/consolidated/shareholders_report.py
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/consolidated/top_n_concentration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.647793 refinitiv-data-1.3.1/refinitiv/data/content/ownership/fund/
+-rw-rw-rw-   0 root         (0) root         (0)      383 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/fund/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2410 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/fund/_breakdown_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1771 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/fund/_concentration_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2024 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/fund/_holdings_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2156 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/fund/_investors_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2043 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/fund/_recent_activity_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     3197 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/fund/_shareholders_history_report_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2084 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/fund/_shareholders_report_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1945 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/fund/_top_n_concentration_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/fund/breakdown.py
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/fund/concentration.py
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/fund/holdings.py
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/fund/investors.py
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/fund/recent_activity.py
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/fund/shareholders_history_report.py
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/fund/shareholders_report.py
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/fund/top_n_concentration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.647793 refinitiv-data-1.3.1/refinitiv/data/content/ownership/insider/
+-rw-rw-rw-   0 root         (0) root         (0)      111 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/insider/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2140 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/insider/_shareholders_report_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     3238 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/insider/_transaction_report_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/insider/shareholders_report.py
+-rw-rw-rw-   0 root         (0) root         (0)       82 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/insider/transaction_report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.647793 refinitiv-data-1.3.1/refinitiv/data/content/ownership/investor/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/investor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2116 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/investor/_holdings_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/investor/holdings.py
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/ownership/org_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.651793 refinitiv-data-1.3.1/refinitiv/data/content/pricing/
+-rw-rw-rw-   0 root         (0) root         (0)      775 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/pricing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3453 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/pricing/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     5313 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/pricing/_pricing_content_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)    17807 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/pricing/_stream_facade.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.655793 refinitiv-data-1.3.1/refinitiv/data/content/pricing/chain/
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/pricing/chain/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8116 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/pricing/chain/_chain_record.py
+-rw-rw-rw-   0 root         (0) root         (0)     5139 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/pricing/chain/_chain_records.py
+-rw-rw-rw-   0 root         (0) root         (0)     1776 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/pricing/chain/_chains_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     3987 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/pricing/chain/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    55563 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/pricing/chain/_display_template.py
+-rw-rw-rw-   0 root         (0) root         (0)     8373 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/pricing/chain/_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)     4789 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/pricing/chain/_stream_facade.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.659793 refinitiv-data-1.3.1/refinitiv/data/content/search/
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/search/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11914 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/search/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     4249 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/search/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2029 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/search/_lookup_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1066 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/search/_metadata_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1943 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/search/_views.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/search/lookup.py
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/search/metadata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.659793 refinitiv-data-1.3.1/refinitiv/data/content/symbol_conversion/
+-rw-rw-rw-   0 root         (0) root         (0)      483 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/symbol_conversion/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2824 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/symbol_conversion/_asset_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      552 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/symbol_conversion/_asset_state.py
+-rw-rw-rw-   0 root         (0) root         (0)     4444 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/symbol_conversion/_country_code.py
+-rw-rw-rw-   0 root         (0) root         (0)     7513 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/symbol_conversion/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/symbol_conversion/_symbol_type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.659793 refinitiv-data-1.3.1/refinitiv/data/content/trade_data_service/
+-rw-rw-rw-   0 root         (0) root         (0)      227 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/trade_data_service/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3723 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/trade_data_service/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     7718 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/trade_data_service/_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)    10810 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/content/trade_data_service/_stream_facade.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.663793 refinitiv-data-1.3.1/refinitiv/data/delivery/
+-rw-rw-rw-   0 root         (0) root         (0)     1266 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.671793 refinitiv-data-1.3.1/refinitiv/data/delivery/_data/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      654 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_data/_api_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      609 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_data/_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     1040 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_data/_data_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3271 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_data/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)    26935 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_data/_data_provider_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     6693 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_data/_data_provider_layer.py
+-rw-rw-rw-   0 root         (0) root         (0)      199 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_data/_data_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      753 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_data/_endpoint_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      914 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_data/_endpoint_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     5634 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_data/_endpoint_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2091 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_data/_parsed_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     4021 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_data/_raw_data_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1411 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_data/_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     5778 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_data/_request_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     2097 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_data/_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     2506 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_data/_response_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3617 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_data/_validators.py
+-rw-rw-rw-   0 root         (0) root         (0)      363 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_dictionary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.687793 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/
+-rw-rw-rw-   0 root         (0) root         (0)      651 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12942 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/_omm_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/_protocol_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     4906 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/_rdp_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)    10068 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/_stream_cxn_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     5401 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/_stream_cxn_config_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    11913 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/_stream_cxn_config_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)    11442 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/_stream_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     9547 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/_stream_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/_stream_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/_validator_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2590 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/base_stream.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.687793 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/contrib/
+-rw-rw-rw-   0 root         (0) root         (0)      216 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/contrib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5529 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/contrib/_funcs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2625 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/contrib/_offstream.py
+-rw-rw-rw-   0 root         (0) root         (0)     2740 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/contrib/_response.py
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/contrib/_stream_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)      334 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/contrib/_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     2351 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/event.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.691793 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/metadata/
+-rw-rw-rw-   0 root         (0) root         (0)      535 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/metadata/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14643 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/metadata/_dictionary.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/metadata/_dictionary_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      575 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/metadata/_enum_type_entry.py
+-rw-rw-rw-   0 root         (0) root         (0)     1225 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/metadata/_field_description.py
+-rw-rw-rw-   0 root         (0) root         (0)      462 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/metadata/_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)     6746 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/metadata/_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     9811 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/metadata/_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)    15911 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/omm_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)     6985 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/omm_stream_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     2666 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/omm_stream_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     3929 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/proxy_info.py
+-rw-rw-rw-   0 root         (0) root         (0)    10724 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/rdp_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)     3085 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/rdp_stream_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     2374 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/rdp_stream_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.695793 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/rwf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-31 10:28:02.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/rwf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      779 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/rwf/conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)     5403 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/rwf/ema.py
+-rw-rw-rw-   0 root         (0) root         (0)     9506 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/rwf/socket.py
+-rw-rw-rw-   0 root         (0) root         (0)     4741 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/stream.py
+-rw-rw-rw-   0 root         (0) root         (0)     4073 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/stream_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    16512 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/stream_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/stream_cxn_state.py
+-rw-rw-rw-   0 root         (0) root         (0)      175 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/stream_state.py
+-rw-rw-rw-   0 root         (0) root         (0)     3508 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/stream_state_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.695793 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/ws/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-31 10:28:02.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/ws/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/ws/ws_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.699793 refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/
+-rw-rw-rw-   0 root         (0) root         (0)      824 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3105 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/_buckets_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     3480 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/_cfs_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     1801 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/_data_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1404 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/_data_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     1120 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/_file_downloader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1353 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/_file_downloader_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      993 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/_file_downloader_facade.py
+-rw-rw-rw-   0 root         (0) root         (0)     3893 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/_file_sets_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2442 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/_files_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     4212 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/_iter_object.py
+-rw-rw-rw-   0 root         (0) root         (0)     2829 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/_packages_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)     1789 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     1140 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/_unpacker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1036 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/buckets.py
+-rw-rw-rw-   0 root         (0) root         (0)      160 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/file_downloader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1035 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/file_sets.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/files.py
+-rw-rw-rw-   0 root         (0) root         (0)      507 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/packages.py
+-rw-rw-rw-   0 root         (0) root         (0)      455 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/endpoint_request.py
+-rw-rw-rw-   0 root         (0) root         (0)      773 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/omm_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)      429 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/delivery/rdp_stream.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.699793 refinitiv-data-1.3.1/refinitiv/data/discovery/
+-rw-rw-rw-   0 root         (0) root         (0)      520 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/discovery/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2471 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/discovery/_convert_symbols.py
+-rw-rw-rw-   0 root         (0) root         (0)     2803 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/discovery/_search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.703793 refinitiv-data-1.3.1/refinitiv/data/discovery/_search_explorer/
+-rw-rw-rw-   0 root         (0) root         (0)       94 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/discovery/_search_explorer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      608 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/discovery/_search_explorer/_buckets_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3509 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/discovery/_search_explorer/_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/discovery/_search_explorer/_navigator.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/discovery/_search_explorer/_properties.py
+-rw-rw-rw-   0 root         (0) root         (0)     3610 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/discovery/_search_explorer/_property.py
+-rw-rw-rw-   0 root         (0) root         (0)      175 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/discovery/_search_explorer/_property_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     3409 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/discovery/_search_explorer/_search_explorer.py
+-rw-rw-rw-   0 root         (0) root         (0)     8754 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/discovery/_search_explorer/_search_explorer_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.707793 refinitiv-data-1.3.1/refinitiv/data/discovery/_search_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      383 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/discovery/_search_templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12658 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/discovery/_search_templates/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8134 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/discovery/_search_templates/embedded.py
+-rw-rw-rw-   0 root         (0) root         (0)     5266 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/discovery/_search_templates/manage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1555 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/discovery/_search_templates/namespaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2235 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/discovery/_search_templates/search.py
+-rw-rw-rw-   0 root         (0) root         (0)      653 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/discovery/_search_templates/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.707793 refinitiv-data-1.3.1/refinitiv/data/discovery/_stakeholders/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/discovery/_stakeholders/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      490 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/discovery/_stakeholders/_customers.py
+-rw-rw-rw-   0 root         (0) root         (0)     4911 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/discovery/_stakeholders/_fetch_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/discovery/_stakeholders/_relationship_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1675 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/discovery/_stakeholders/_stakeholder_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1169 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/discovery/_stakeholders/_stakeholders.py
+-rw-rw-rw-   0 root         (0) root         (0)      491 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/discovery/_stakeholders/_suppliers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.711793 refinitiv-data-1.3.1/refinitiv/data/discovery/_universe_expanders/
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/discovery/_universe_expanders/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4156 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/discovery/_universe_expanders/_chain.py
+-rw-rw-rw-   0 root         (0) root         (0)     2562 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/discovery/_universe_expanders/_discovery_universe.py
+-rw-rw-rw-   0 root         (0) root         (0)      393 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/discovery/_universe_expanders/_peers.py
+-rw-rw-rw-   0 root         (0) root         (0)      514 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/discovery/_universe_expanders/_screener.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/discovery/_universe_expanders/_universe_expander.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.711793 refinitiv-data-1.3.1/refinitiv/data/early_access/
+-rw-rw-rw-   0 root         (0) root         (0)     1298 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/early_access/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.711793 refinitiv-data-1.3.1/refinitiv/data/early_access/discovery/
+-rw-rw-rw-   0 root         (0) root         (0)      243 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/early_access/discovery/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.715793 refinitiv-data-1.3.1/refinitiv/data/eikon/
+-rw-rw-rw-   0 root         (0) root         (0)      479 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/eikon/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9549 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/eikon/_data_grid.py
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/eikon/_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     8917 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/eikon/_json_requests.py
+-rw-rw-rw-   0 root         (0) root         (0)     7401 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/eikon/_news_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     1099 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/eikon/_streaming_prices.py
+-rw-rw-rw-   0 root         (0) root         (0)     5234 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/eikon/_symbology.py
+-rw-rw-rw-   0 root         (0) root         (0)    13670 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/eikon/_time_series.py
+-rw-rw-rw-   0 root         (0) root         (0)     4829 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/eikon/_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)      780 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.715793 refinitiv-data-1.3.1/refinitiv/data/session/
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/session/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1742 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/session/desktop.py
+-rw-rw-rw-   0 root         (0) root         (0)     4202 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/session/platform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.715793 refinitiv-data-1.3.1/refinitiv/data/usage_collection/
+-rw-rw-rw-   0 root         (0) root         (0)      359 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/usage_collection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      472 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/usage_collection/_abstract_logger.py
+-rw-rw-rw-   0 root         (0) root         (0)      342 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/usage_collection/_filter_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     6287 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/usage_collection/_logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     1555 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/usage_collection/_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-07-31 10:28:01.000000 refinitiv-data-1.3.1/refinitiv/data/warnings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:28:23.719793 refinitiv-data-1.3.1/refinitiv_data.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9778 2023-07-31 10:28:23.000000 refinitiv-data-1.3.1/refinitiv_data.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    55616 2023-07-31 10:28:23.000000 refinitiv-data-1.3.1/refinitiv_data.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 10:28:23.000000 refinitiv-data-1.3.1/refinitiv_data.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      345 2023-07-31 10:28:23.000000 refinitiv-data-1.3.1/refinitiv_data.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-31 10:28:23.000000 refinitiv-data-1.3.1/refinitiv_data.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 10:28:23.719793 refinitiv-data-1.3.1/setup.cfg
```

### Comparing `refinitiv-data-1.3.0/CHANGELOG.md` & `refinitiv-data-1.3.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 <!-- towncrier release notes start -->
 
+## [1.3.1] - 2023-07-31
+
+### Fixed
+
+- RIC with upper case register letters passed to pricing endpoint in `rd.get_data` request, if mix of register letters were defined by User ([eapi-5733](https://jira.refinitiv.com/browse/eapi-5733))
+
 
 ## [1.3.0] - 2023-06-21
 
 ### Added
 
 - `datetime` types for date measuring parameters to `refinitiv.data.content.ipa` objects ([eapi-5062](https://jira.refinitiv.com/browse/eapi-5062))
 - Fields validation option to the `contribute()` method for updating instrument(RIC) ([eapi-5213](https://jira.refinitiv.com/browse/eapi-5213))
```

### Comparing `refinitiv-data-1.3.0/LICENSE` & `refinitiv-data-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/PKG-INFO` & `refinitiv-data-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refinitiv-data
-Version: 1.3.0
+Version: 1.3.1
 Summary: Client for Refinitiv Data Platform API's
 Author: REFINITIV
 License: Apache 2.0
 Project-URL: Homepage, https://developers.refinitiv.com/en/api-catalog/refinitiv-data-platform/refinitiv-data-library-for-python
 Project-URL: Documentation, https://developers.refinitiv.com/en/api-catalog/refinitiv-data-platform/refinitiv-data-library-for-python/documentation
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `refinitiv-data-1.3.0/README.md` & `refinitiv-data-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/pyproject.toml` & `refinitiv-data-1.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_config_defaults.py` & `refinitiv-data-1.3.1/refinitiv/data/_config_defaults.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_config_functions.py` & `refinitiv-data-1.3.1/refinitiv/data/_config_functions.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_configure.py` & `refinitiv-data-1.3.1/refinitiv/data/_configure.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_content_type.py` & `refinitiv-data-1.3.1/refinitiv/data/_content_type.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_core/log_reporter.py` & `refinitiv-data-1.3.1/refinitiv/data/_core/log_reporter.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_core/session/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/_core/session/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_core/session/_default_session_manager.py` & `refinitiv-data-1.3.1/refinitiv/data/_core/session/_default_session_manager.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_core/session/_desktop_session.py` & `refinitiv-data-1.3.1/refinitiv/data/_core/session/_desktop_session.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_core/session/_platform_session.py` & `refinitiv-data-1.3.1/refinitiv/data/_core/session/_platform_session.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_core/session/_retry_transport.py` & `refinitiv-data-1.3.1/refinitiv/data/_core/session/_retry_transport.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_core/session/_session.py` & `refinitiv-data-1.3.1/refinitiv/data/_core/session/_session.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_core/session/_session_cxn_factory.py` & `refinitiv-data-1.3.1/refinitiv/data/_core/session/_session_cxn_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_core/session/_session_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/_core/session/_session_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_core/session/_session_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/_core/session/_session_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_core/session/_user_uuid.py` & `refinitiv-data-1.3.1/refinitiv/data/_core/session/_user_uuid.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_core/session/access_token_updater.py` & `refinitiv-data-1.3.1/refinitiv/data/_core/session/access_token_updater.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_core/session/auth_manager.py` & `refinitiv-data-1.3.1/refinitiv/data/_core/session/auth_manager.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_core/session/connection.py` & `refinitiv-data-1.3.1/refinitiv/data/_core/session/connection.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_core/session/event.py` & `refinitiv-data-1.3.1/refinitiv/data/_core/session/event.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_core/session/event_code.py` & `refinitiv-data-1.3.1/refinitiv/data/_core/session/event_code.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_core/session/grant_password.py` & `refinitiv-data-1.3.1/refinitiv/data/_core/session/grant_password.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_core/session/http_service.py` & `refinitiv-data-1.3.1/refinitiv/data/_core/session/http_service.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_core/session/null_session.py` & `refinitiv-data-1.3.1/refinitiv/data/_core/session/null_session.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_core/session/refresh_token_updater.py` & `refinitiv-data-1.3.1/refinitiv/data/_core/session/refresh_token_updater.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_core/session/tools.py` & `refinitiv-data-1.3.1/refinitiv/data/_core/session/tools.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_core/session/updater.py` & `refinitiv-data-1.3.1/refinitiv/data/_core/session/updater.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_errors.py` & `refinitiv-data-1.3.1/refinitiv/data/_errors.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_external_libraries/python_configuration/LICENSE` & `refinitiv-data-1.3.1/refinitiv/data/_external_libraries/python_configuration/LICENSE`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_external_libraries/python_configuration/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/_external_libraries/python_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_external_libraries/python_configuration/configuration.py` & `refinitiv-data-1.3.1/refinitiv/data/_external_libraries/python_configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_external_libraries/python_configuration/configuration_set.py` & `refinitiv-data-1.3.1/refinitiv/data/_external_libraries/python_configuration/configuration_set.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_external_libraries/python_configuration/helpers.py` & `refinitiv-data-1.3.1/refinitiv/data/_external_libraries/python_configuration/helpers.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_containers.py` & `refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/_containers.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_data_df_builder.py` & `refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/_data_df_builder.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_data_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_history_df_builder.py` & `refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/_history_df_builder.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_history_df_builder_factory.py` & `refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/_history_df_builder_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_intervals_consts.py` & `refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/_intervals_consts.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_mixed_streams.py` & `refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/_mixed_streams.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_ohlc_builder.py` & `refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/_ohlc_builder.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_pricing_recorder.py` & `refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/_pricing_recorder.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_recording_control.py` & `refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/_recording_control.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_stream_update_handler.py` & `refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/_stream_update_handler.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_adc_context.py` & `refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/context_collection/_adc_context.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_adc_rdp_context.py` & `refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/context_collection/_adc_rdp_context.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_adc_udf_context.py` & `refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/context_collection/_adc_udf_context.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_context.py` & `refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/context_collection/_context.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_context_factory.py` & `refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/context_collection/_context_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_cust_inst_context.py` & `refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/context_collection/_cust_inst_context.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_cust_inst_rdp_context.py` & `refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/context_collection/_cust_inst_rdp_context.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_cust_inst_udf_context.py` & `refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/context_collection/_cust_inst_udf_context.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_hp_and_cust_inst_context.py` & `refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/context_collection/_hp_and_cust_inst_context.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_hp_context.py` & `refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/context_collection/_hp_context.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/dates_and_calendars/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/_add_periods.py` & `refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/dates_and_calendars/_add_periods.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/_count_periods.py` & `refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/dates_and_calendars/_count_periods.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/_date_schedule.py` & `refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/dates_and_calendars/_date_schedule.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/_holidays.py` & `refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/dates_and_calendars/_holidays.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/_is_working_day.py` & `refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/dates_and_calendars/_is_working_day.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/get_data_func.py` & `refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/get_data_func.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/get_history_func.py` & `refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/get_history_func.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/get_stream.py` & `refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/get_stream.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/news/_news.py` & `refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/news/_news.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/session.py` & `refinitiv-data-1.3.1/refinitiv/data/_fin_coder_layer/session.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_log.py` & `refinitiv-data-1.3.1/refinitiv/data/_log.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_qpl/_bid_ask.py` & `refinitiv-data-1.3.1/refinitiv/data/_qpl/_bid_ask.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_qpl/_data_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/_qpl/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_qpl/_fx_spot_quote.py` & `refinitiv-data-1.3.1/refinitiv/data/_qpl/_fx_spot_quote.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_qpl/_fx_swap_points.py` & `refinitiv-data-1.3.1/refinitiv/data/_qpl/_fx_swap_points.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_qpl/_fx_swp_to_swp.py` & `refinitiv-data-1.3.1/refinitiv/data/_qpl/_fx_swp_to_swp.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_qpl/_serializer.py` & `refinitiv-data-1.3.1/refinitiv/data/_qpl/_serializer.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_qpl/_tenor_bid_ask.py` & `refinitiv-data-1.3.1/refinitiv/data/_qpl/_tenor_bid_ask.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_tools/_common.py` & `refinitiv-data-1.3.1/refinitiv/data/_tools/_common.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_tools/_converter.py` & `refinitiv-data-1.3.1/refinitiv/data/_tools/_converter.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_tools/_dataframe.py` & `refinitiv-data-1.3.1/refinitiv/data/_tools/_dataframe.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_tools/_datetime.py` & `refinitiv-data-1.3.1/refinitiv/data/_tools/_datetime.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_tools/_params.py` & `refinitiv-data-1.3.1/refinitiv/data/_tools/_params.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_tools/_patterns.py` & `refinitiv-data-1.3.1/refinitiv/data/_tools/_patterns.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_tools/_repr.py` & `refinitiv-data-1.3.1/refinitiv/data/_tools/_repr.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_tools/_specification.py` & `refinitiv-data-1.3.1/refinitiv/data/_tools/_specification.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_tools/_utils.py` & `refinitiv-data-1.3.1/refinitiv/data/_tools/_utils.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_tools/templates.py` & `refinitiv-data-1.3.1/refinitiv/data/_tools/templates.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/_types.py` & `refinitiv-data-1.3.1/refinitiv/data/_types.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/content/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/_content_data_factory.py` & `refinitiv-data-1.3.1/refinitiv/data/content/_content_data_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/_content_data_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/content/_content_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/_content_provider_layer.py` & `refinitiv-data-1.3.1/refinitiv/data/content/_content_provider_layer.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/_content_response_factory.py` & `refinitiv-data-1.3.1/refinitiv/data/content/_content_response_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/_df_builder.py` & `refinitiv-data-1.3.1/refinitiv/data/content/_df_builder.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/_df_builder_factory.py` & `refinitiv-data-1.3.1/refinitiv/data/content/_df_builder_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/_entire_data_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/content/_entire_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/_error_parser.py` & `refinitiv-data-1.3.1/refinitiv/data/content/_error_parser.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/_historical_content_validator.py` & `refinitiv-data-1.3.1/refinitiv/data/content/_historical_content_validator.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/_historical_data_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/content/_historical_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/_historical_df_builder.py` & `refinitiv-data-1.3.1/refinitiv/data/content/_historical_df_builder.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/_historical_raw_transf.py` & `refinitiv-data-1.3.1/refinitiv/data/content/_historical_raw_transf.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/_historical_response_factory.py` & `refinitiv-data-1.3.1/refinitiv/data/content/_historical_response_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/_intervals.py` & `refinitiv-data-1.3.1/refinitiv/data/content/_intervals.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/_universe_content_validator.py` & `refinitiv-data-1.3.1/refinitiv/data/content/_universe_content_validator.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/_universe_stream.py` & `refinitiv-data-1.3.1/refinitiv/data/content/_universe_stream.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/_universe_streams.py` & `refinitiv-data-1.3.1/refinitiv/data/content/_universe_streams.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_custom_instruments_data_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/content/custom_instruments/_custom_instruments_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/custom_instruments/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_enums.py` & `refinitiv-data-1.3.1/refinitiv/data/content/custom_instruments/_enums.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_events.py` & `refinitiv-data-1.3.1/refinitiv/data/content/custom_instruments/_events.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_instrument_class.py` & `refinitiv-data-1.3.1/refinitiv/data/content/custom_instruments/_instrument_class.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_instrument_prop_classes.py` & `refinitiv-data-1.3.1/refinitiv/data/content/custom_instruments/_instrument_prop_classes.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_manage.py` & `refinitiv-data-1.3.1/refinitiv/data/content/custom_instruments/_manage.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_search.py` & `refinitiv-data-1.3.1/refinitiv/data/content/custom_instruments/_search.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_stream_facade.py` & `refinitiv-data-1.3.1/refinitiv/data/content/custom_instruments/_stream_facade.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_summaries.py` & `refinitiv-data-1.3.1/refinitiv/data/content/custom_instruments/_summaries.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/manage.py` & `refinitiv-data-1.3.1/refinitiv/data/content/custom_instruments/manage.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/esg/_base_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/esg/_base_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/esg/_basic_overview_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/esg/_basic_overview_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/esg/_esg_data_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/content/esg/_esg_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/esg/_full_measures_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/esg/_full_measures_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/esg/_full_scores_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/esg/_full_scores_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/esg/_standard_measures_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/esg/_standard_measures_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/esg/_standard_scores_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/esg/_standard_scores_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/esg/_universe_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/esg/_universe_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/esg/bulk/_actions.py` & `refinitiv-data-1.3.1/refinitiv/data/content/esg/bulk/_actions.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/esg/bulk/_db_manager.py` & `refinitiv-data-1.3.1/refinitiv/data/content/esg/bulk/_db_manager.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/esg/bulk/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/esg/bulk/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/esg/bulk/_file_manager.py` & `refinitiv-data-1.3.1/refinitiv/data/content/esg/bulk/_file_manager.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/esg/bulk/_package_manager.py` & `refinitiv-data-1.3.1/refinitiv/data/content/esg/bulk/_package_manager.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/esg/bulk/_package_manager_facade.py` & `refinitiv-data-1.3.1/refinitiv/data/content/esg/bulk/_package_manager_facade.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/esg/bulk/_tools.py` & `refinitiv-data-1.3.1/refinitiv/data/content/esg/bulk/_tools.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/estimates/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/content/estimates/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/estimates/_data_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/content/estimates/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_actuals/_annual_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_actuals/_annual_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_actuals/_interim_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_actuals/_interim_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_actuals_kpi/_annual_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_actuals_kpi/_annual_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_actuals_kpi/_interim_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_actuals_kpi/_interim_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/_annual_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary/_annual_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/_historical_snapshots_non_periodic_measures_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary/_historical_snapshots_non_periodic_measures_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/_historical_snapshots_periodic_measures_annual_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary/_historical_snapshots_periodic_measures_annual_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/_historical_snapshots_periodic_measures_interim_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary/_historical_snapshots_periodic_measures_interim_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/_historical_snapshots_recommendations_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary/_historical_snapshots_recommendations_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/_interim_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary/_interim_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/_non_periodic_measures_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary/_non_periodic_measures_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/_recommendations_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary/_recommendations_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary_kpi/_annual_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary_kpi/_annual_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary_kpi/_historical_snapshots_kpi_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary_kpi/_historical_snapshots_kpi_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary_kpi/_interim_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/estimates/view_summary_kpi/_interim_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/filings/_filing_query.py` & `refinitiv-data-1.3.1/refinitiv/data/content/filings/_filing_query.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/filings/_retrieval_data_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/content/filings/_retrieval_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/filings/_retrieval_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/filings/_retrieval_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/filings/_search_data_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/content/filings/_search_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/filings/_search_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/filings/_search_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/fundamental_and_reference/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/content/fundamental_and_reference/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/fundamental_and_reference/_content_validator.py` & `refinitiv-data-1.3.1/refinitiv/data/content/fundamental_and_reference/_content_validator.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/fundamental_and_reference/_data_grid_type.py` & `refinitiv-data-1.3.1/refinitiv/data/content/fundamental_and_reference/_data_grid_type.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/fundamental_and_reference/_data_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/content/fundamental_and_reference/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/fundamental_and_reference/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/fundamental_and_reference/_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 import asyncio
 import time
 from enum import unique
 from typing import Callable, List, Union, TYPE_CHECKING, Optional, Any
 
-from ._data_grid_type import (
-    DataGridType,
-    determine_content_type_and_flag,
-    use_field_names_in_headers_arg_parser,
-)
+from ._data_grid_type import DataGridType, determine_content_type_and_flag, use_field_names_in_headers_arg_parser
 from .._content_data import Data
 from .._content_provider_layer import ContentUsageLoggerMixin
 from .._df_build_type import DFBuildType
 from ..._base_enum import StrEnum
 from ..._content_type import ContentType
 from ..._core.session import get_valid_session
 from ..._tools import (
@@ -142,15 +138,15 @@
         row_headers: OptRowHeaders = None,
         use_field_names_in_headers: bool = False,
         extended_params: "ExtendedParams" = None,
     ):
         extended_params = extended_params or {}
         universe = extended_params.get("universe") or try_copy_to_list(universe)
         universe = universe_arg_parser.get_list(universe)
-        universe = [value.upper() for value in universe]
+        universe = [value.upper() if value.islower() else value for value in universe]
         self.universe = universe
         self.fields = fields_arg_parser.get_list(try_copy_to_list(fields))
 
         if parameters is not None and not isinstance(parameters, dict):
             raise ValueError(f"Arg parameters must be a dictionary")
 
         self.parameters = parameters
```

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/fundamental_and_reference/_request_factory.py` & `refinitiv-data-1.3.1/refinitiv/data/content/fundamental_and_reference/_request_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/fundamental_and_reference/_response_factory.py` & `refinitiv-data-1.3.1/refinitiv/data/content/fundamental_and_reference/_response_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/historical_pricing/_enums.py` & `refinitiv-data-1.3.1/refinitiv/data/content/historical_pricing/_enums.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/historical_pricing/_events_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/historical_pricing/_events_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/historical_pricing/_historical_pricing_data_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/content/historical_pricing/_historical_pricing_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/historical_pricing/_historical_pricing_request_factory.py` & `refinitiv-data-1.3.1/refinitiv/data/content/historical_pricing/_historical_pricing_request_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/historical_pricing/_summaries_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/historical_pricing/_summaries_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_content_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_content_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_constituents.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_constituents.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_curve_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_curve_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_curve_parameters.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_curve_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_request.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_request.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_business_sector.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_business_sector.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_curve_sub_type.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_curve_sub_type.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_economic_sector.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_economic_sector.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_industry.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_industry.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_industry_group.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_industry_group.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_interest_calculation_method.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_interest_calculation_method.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_interpolation_mode.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_interpolation_mode.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_rating.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_rating.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_butterfly_shift.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_butterfly_shift.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_combined_shift.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_combined_shift.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_curve_definition_pricing.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_curve_definition_pricing.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_flattening_shift.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_flattening_shift.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_constituents.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_constituents.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_curve_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_curve_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_curve_parameters.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_curve_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_shift_scenario.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_shift_scenario.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_long_end_shift.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_long_end_shift.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_parallel_shift.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_parallel_shift.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_request.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_request.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_shift_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_shift_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_short_end_shift.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_short_end_shift.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_time_bucket_shift.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_time_bucket_shift.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_twist_shift.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_twist_shift.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_base_definition_mixin.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_base_definition_mixin.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_bid_ask_fields_description.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_bid_ask_fields_description.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_bid_ask_fields_formula_description.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_bid_ask_fields_formula_description.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_constituents_description.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_constituents_description.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/_curve_definition_description.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/_curve_definition_description.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/_request.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/_request.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_curve_parameters.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_curve_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_delete/_request.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_delete/_request.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_field_description.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_field_description.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_field_formula_description.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_field_formula_description.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_formula_parameter_description.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_formula_parameter_description.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_instrument_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_instrument_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_instrument_description.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_instrument_description.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_turn_fields.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_turn_fields.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_spot_instrument_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_spot_instrument_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_spot_instrument_description.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_spot_instrument_description.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/_curve_definition_keys.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/_curve_definition_keys.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/_request.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/_request.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instrument_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instrument_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instrument_description.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instrument_description.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instruments_segment.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instruments_segment.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_mixin_request.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_mixin_request.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_bid_ask.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_bid_ask.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_bid_ask_fields.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_bid_ask_fields.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_fx_forward_turn.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_fx_forward_turn.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_search/_curve_get_definition_item.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_search/_curve_get_definition_item.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_turn_adjustment.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_turn_adjustment.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_types.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_types.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/_curve_update_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/_curve_update_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/_request.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/_request.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_triangulate_definitions/_request.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_triangulate_definitions/_request.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_curves_builder_df.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_curves_builder_df.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_curves_data_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_curves_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_enums/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_enums/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_enums/_instrument_type.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_enums/_instrument_type.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_enums/_zc_interpolation_mode.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_enums/_zc_interpolation_mode.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_forward_curve_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_forward_curve_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_forward_curve_request_item.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_forward_curve_request_item.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_forward_curve_types.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_forward_curve_types.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_convexity.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_models/_convexity.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_curve.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_models/_curve.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_instrument.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_models/_instrument.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_interest_rate_curve_parameters.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_models/_interest_rate_curve_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_par_rate_shift.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_models/_par_rate_shift.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_step.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_models/_step.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_turn.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_models/_turn.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_valuation_time.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_models/_valuation_time.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_shift_scenario.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_shift_scenario.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_swap_zc_curve_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_swap_zc_curve_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_swap_zc_curve_parameters.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_swap_zc_curve_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_zc_curve_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_zc_curve_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_zc_curve_definition_request.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_zc_curve_definition_request.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_zc_curve_definitions.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_zc_curve_definitions.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_zc_curve_parameters.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_zc_curve_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_zc_curve_request_item.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_zc_curve_request_item.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_zc_curve_types.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_curves/_zc_curve_types.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_business_day_convention.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_business_day_convention.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_common_tools.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_common_tools.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_date_moving_convention.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_date_moving_convention.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_date_rolling_convention.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_date_rolling_convention.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_day_count_basis.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_day_count_basis.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_day_of_week.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_day_of_week.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_direction.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_direction.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_exercise_style.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_exercise_style.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_frequency.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_frequency.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_fx_swap_calculation_method.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_fx_swap_calculation_method.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_holiday_outupts.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_holiday_outupts.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_index_compounding_method.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_index_compounding_method.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_period_type.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_period_type.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_quote_fallback_logic.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_quote_fallback_logic.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_redemption_date_type.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_redemption_date_type.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_seniority.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_seniority.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_stub_rule.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_stub_rule.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_yield_type.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_enums/_yield_type.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_ipa_content_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_ipa_content_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_ipa_content_validator.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_ipa_content_validator.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_american_monte_carlo_parameters.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_models/_american_monte_carlo_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_amortization_item.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_models/_amortization_item.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_barrier_definition_element.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_models/_barrier_definition_element.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_basket_item.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_models/_basket_item.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_bid_ask_mid.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_models/_bid_ask_mid.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_bond_rounding_parameters.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_models/_bond_rounding_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_day_weight.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_models/_day_weight.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_fx_point.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_models/_fx_point.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_input_flow.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_models/_input_flow.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_interpolation_weight.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_models/_interpolation_weight.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_numerical_method.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_models/_numerical_method.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_payout_scaling.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_models/_payout_scaling.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_pde_parameters.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_models/_pde_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_object_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_object_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_cap_surface_request_item.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_cap_surface_request_item.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_eti_surface_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_eti_surface_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_eti_surface_parameters.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_eti_surface_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_eti_surface_request_item.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_eti_surface_request_item.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_fx_statistics_parameters.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_fx_statistics_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_fx_surface_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_fx_surface_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_fx_surface_parameters.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_fx_surface_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_fx_surface_request_item.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_fx_surface_request_item.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_i_ir_vol_model_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_i_ir_vol_model_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_i_ir_vol_model_pricing_parameters.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_i_ir_vol_model_pricing_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/_maturity_filter.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_models/_maturity_filter.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/_moneyness_weight.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_models/_moneyness_weight.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/_strike_filter.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_models/_strike_filter.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/_strike_filter_range.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_models/_strike_filter_range.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/_surface.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_models/_surface.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/_surface_filters.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_models/_surface_filters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/_surface_output.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_models/_surface_output.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/_volatility_surface_point.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_models/_volatility_surface_point.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_surface_request_item.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_surface_request_item.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_surfaces_data_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_surfaces_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_swaption_calculation_params.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_swaption_calculation_params.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_swaption_surface_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_swaption_surface_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_swaption_surface_request_item.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/_surfaces/_swaption_surface_request_item.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_bond_curves/curves/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/_bond_curves/curves/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_bond_curves/curves/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/_bond_curves/curves/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/curves/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/curves/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/curves/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/curves/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_data_classes.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_data_classes.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_manage.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_manage.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_search.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_search.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/_data_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/_search.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/_search.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/forward_curves/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/forward_curves/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/forward_curves/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/forward_curves/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/zc_curve_definitions/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/zc_curve_definitions/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/zc_curves/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/zc_curves/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/zc_curves/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/curves/zc_curves/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/_base_request_items.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/_base_request_items.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/_content_data_validator.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/_content_data_validator.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/_request_factory.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/_request_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/add_periods/_add_periods_data_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/add_periods/_add_periods_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/add_periods/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/add_periods/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/count_periods/_count_periods.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/count_periods/_count_periods.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/count_periods/_count_periods_data_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/count_periods/_count_periods_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/_date_schedule.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/_date_schedule.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/_date_schedule_data_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/_date_schedule_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/holidays/_holidays.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/holidays/_holidays.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/holidays/_holidays_data_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/holidays/_holidays_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/_is_working_day.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/_is_working_day.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/_is_working_day_data_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/_is_working_day_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/_base_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/_base_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/_contracts_data_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/_contracts_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/_instrument_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/_instrument_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/_quantitative_data_stream.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/_quantitative_data_stream.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/_stream_facade.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/_stream_facade.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/bond/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/bond/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/bond/_bond_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/bond/_bond_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/bond/_bond_pricing_parameters.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/bond/_bond_pricing_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/bond/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/bond/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/cap_floor/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/_cap_floor_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/cap_floor/_cap_floor_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/_cap_floor_pricing_parameters.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/cap_floor/_cap_floor_pricing_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/cap_floor/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cds/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/cds/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cds/_cds_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/cds/_cds_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cds/_cds_pricing_parameters.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/cds/_cds_pricing_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cds/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/cds/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cds/_premium_leg_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/cds/_premium_leg_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cds/_protection_leg_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/cds/_protection_leg_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cross/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/cross/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cross/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/cross/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_leg_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_leg_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_pricing_parameters.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_pricing_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_enums/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_enums/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_enums/_fx_binary_type.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_enums/_fx_binary_type.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_barrier_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_barrier_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_binary_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_binary_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_cbbc_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_cbbc_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_double_barriers_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_double_barriers_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_fixing_info.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_fixing_info.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_underlying_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_underlying_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_fx/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_average_info.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_average_info.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_barrier_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_barrier_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_binary_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_binary_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_double_barrier_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_double_barrier_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_double_barrier_info.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_double_barrier_info.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_double_binary_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_double_binary_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_dual_currency_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_dual_currency_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_forward_start.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_forward_start.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_underlying_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_underlying_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_option_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_option_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_option_instrument_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_option_instrument_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_option_pricing_parameters.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/option/_option_pricing_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/repo/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/repo/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/repo/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/repo/_repo_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_parameters.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/repo/_repo_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_pricing_parameters.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/repo/_repo_pricing_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_underlying_contract.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/repo/_repo_underlying_contract.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_underlying_pricing_parameters.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/repo/_repo_underlying_pricing_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swap/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/swap/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swap/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/swap/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swap/_swap_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/swap/_swap_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swap/_swap_leg_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/swap/_swap_leg_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swap/_swap_pricing_parameters.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/swap/_swap_pricing_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swaption/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/swaption/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swaption/_bermudan_swaption_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/swaption/_bermudan_swaption_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swaption/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/swaption/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_market_data_rule.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_market_data_rule.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_pricing_parameters.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_pricing_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/term_deposit/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/term_deposit/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/term_deposit/_term_deposit_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/term_deposit/_term_deposit_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/term_deposit/_term_deposit_pricing_parameters.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/financial_contracts/term_deposit/_term_deposit_pricing_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/surfaces/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/cap/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/surfaces/cap/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/cap/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/surfaces/cap/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/eti/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/surfaces/eti/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/eti/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/surfaces/eti/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/fx/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/surfaces/fx/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/fx/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/surfaces/fx/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/swaption/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/surfaces/swaption/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/swaption/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ipa/surfaces/swaption/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/news/_news_data.py` & `refinitiv-data-1.3.1/refinitiv/data/content/news/_news_data.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/news/_news_data_provider_layer.py` & `refinitiv-data-1.3.1/refinitiv/data/content/news/_news_data_provider_layer.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/news/_tools.py` & `refinitiv-data-1.3.1/refinitiv/data/content/news/_tools.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/news/headlines/_data.py` & `refinitiv-data-1.3.1/refinitiv/data/content/news/headlines/_data.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/news/headlines/_data_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/content/news/headlines/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/news/headlines/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/news/headlines/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/news/headlines/_request_factory.py` & `refinitiv-data-1.3.1/refinitiv/data/content/news/headlines/_request_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/news/images/_data_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/content/news/images/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/news/images/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/news/images/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/news/images/_image.py` & `refinitiv-data-1.3.1/refinitiv/data/content/news/images/_image.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/_data_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/content/news/online_reports/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/news/online_reports/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/_df_builder.py` & `refinitiv-data-1.3.1/refinitiv/data/content/news/online_reports/_df_builder.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/_image_data.py` & `refinitiv-data-1.3.1/refinitiv/data/content/news/online_reports/_image_data.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/_report.py` & `refinitiv-data-1.3.1/refinitiv/data/content/news/online_reports/_report.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/hierarchy/_data_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/content/news/online_reports/hierarchy/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/hierarchy/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/news/online_reports/hierarchy/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/hierarchy/_df_builder.py` & `refinitiv-data-1.3.1/refinitiv/data/content/news/online_reports/hierarchy/_df_builder.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/news/story/_data.py` & `refinitiv-data-1.3.1/refinitiv/data/content/news/story/_data.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/news/story/_data_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/content/news/story/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/news/story/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/news/story/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/news/story/_request_factory.py` & `refinitiv-data-1.3.1/refinitiv/data/content/news/story/_request_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/news/story/_response_factory.py` & `refinitiv-data-1.3.1/refinitiv/data/content/news/story/_response_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/news/story/_udf_html_parser.py` & `refinitiv-data-1.3.1/refinitiv/data/content/news/story/_udf_html_parser.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/_data_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/content/news/top_news/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/news/top_news/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/_df_builder.py` & `refinitiv-data-1.3.1/refinitiv/data/content/news/top_news/_df_builder.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/_top_news_headline.py` & `refinitiv-data-1.3.1/refinitiv/data/content/news/top_news/_top_news_headline.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/hierarchy/_data_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/content/news/top_news/hierarchy/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/hierarchy/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/news/top_news/hierarchy/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/hierarchy/_df_builder.py` & `refinitiv-data-1.3.1/refinitiv/data/content/news/top_news/hierarchy/_df_builder.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ownership/_org_info_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ownership/_org_info_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ownership/_ownership_data_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ownership/_ownership_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/_breakdown_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ownership/consolidated/_breakdown_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/_concentration_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ownership/consolidated/_concentration_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/_investors_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ownership/consolidated/_investors_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/_recent_activity_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ownership/consolidated/_recent_activity_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/_shareholders_history_report_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ownership/consolidated/_shareholders_history_report_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/_shareholders_report_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ownership/consolidated/_shareholders_report_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/_top_n_concentration_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ownership/consolidated/_top_n_concentration_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/_breakdown_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ownership/fund/_breakdown_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/_concentration_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ownership/fund/_concentration_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/_holdings_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ownership/fund/_holdings_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/_investors_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ownership/fund/_investors_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/_recent_activity_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ownership/fund/_recent_activity_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/_shareholders_history_report_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ownership/fund/_shareholders_history_report_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/_shareholders_report_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ownership/fund/_shareholders_report_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/_top_n_concentration_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ownership/fund/_top_n_concentration_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ownership/insider/_shareholders_report_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ownership/insider/_shareholders_report_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ownership/insider/_transaction_report_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ownership/insider/_transaction_report_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/ownership/investor/_holdings_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/ownership/investor/_holdings_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/pricing/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/content/pricing/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/pricing/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/pricing/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/pricing/_pricing_content_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/content/pricing/_pricing_content_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/pricing/_stream_facade.py` & `refinitiv-data-1.3.1/refinitiv/data/content/pricing/_stream_facade.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/pricing/chain/_chain_record.py` & `refinitiv-data-1.3.1/refinitiv/data/content/pricing/chain/_chain_record.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/pricing/chain/_chain_records.py` & `refinitiv-data-1.3.1/refinitiv/data/content/pricing/chain/_chain_records.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/pricing/chain/_chains_data_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/content/pricing/chain/_chains_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/pricing/chain/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/pricing/chain/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/pricing/chain/_display_template.py` & `refinitiv-data-1.3.1/refinitiv/data/content/pricing/chain/_display_template.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/pricing/chain/_stream.py` & `refinitiv-data-1.3.1/refinitiv/data/content/pricing/chain/_stream.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/pricing/chain/_stream_facade.py` & `refinitiv-data-1.3.1/refinitiv/data/content/pricing/chain/_stream_facade.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/search/_data_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/content/search/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/search/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/search/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/search/_lookup_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/search/_lookup_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/search/_metadata_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/search/_metadata_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/search/_views.py` & `refinitiv-data-1.3.1/refinitiv/data/content/search/_views.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/symbol_conversion/_asset_class.py` & `refinitiv-data-1.3.1/refinitiv/data/content/symbol_conversion/_asset_class.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/symbol_conversion/_asset_state.py` & `refinitiv-data-1.3.1/refinitiv/data/content/symbol_conversion/_asset_state.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/symbol_conversion/_country_code.py` & `refinitiv-data-1.3.1/refinitiv/data/content/symbol_conversion/_country_code.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/symbol_conversion/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/symbol_conversion/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/symbol_conversion/_symbol_type.py` & `refinitiv-data-1.3.1/refinitiv/data/content/symbol_conversion/_symbol_type.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/trade_data_service/_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/content/trade_data_service/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/trade_data_service/_stream.py` & `refinitiv-data-1.3.1/refinitiv/data/content/trade_data_service/_stream.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/content/trade_data_service/_stream_facade.py` & `refinitiv-data-1.3.1/refinitiv/data/content/trade_data_service/_stream_facade.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_api_type.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_data/_api_type.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_connection.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_data/_connection.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_data_factory.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_data/_data_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_data_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_data/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_data_provider_factory.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_data/_data_provider_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_data_provider_layer.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_data/_data_provider_layer.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_endpoint_data.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_data/_endpoint_data.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_endpoint_data_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_data/_endpoint_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_endpoint_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_data/_endpoint_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_parsed_data.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_data/_parsed_data.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_raw_data_parser.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_data/_raw_data_parser.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_request.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_data/_request.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_request_factory.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_data/_request_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_response.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_data/_response.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_response_factory.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_data/_response_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_validators.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_data/_validators.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/_omm_stream.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/_omm_stream.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/_rdp_stream.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/_rdp_stream.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/_stream_cxn_cache.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/_stream_cxn_cache.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/_stream_cxn_config_data.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/_stream_cxn_config_data.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/_stream_cxn_config_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/_stream_cxn_config_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/_stream_factory.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/_stream_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/_stream_listener.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/_stream_listener.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/base_stream.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/base_stream.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/contrib/_funcs.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/contrib/_funcs.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/contrib/_offstream.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/contrib/_offstream.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/contrib/_response.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/contrib/_response.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/event.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/event.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/metadata/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/metadata/_dictionary.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/metadata/_dictionary.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/metadata/_enum_type_entry.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/metadata/_enum_type_entry.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/metadata/_field_description.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/metadata/_field_description.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/metadata/_types.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/metadata/_types.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/metadata/_validator.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/metadata/_validator.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/omm_stream.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/omm_stream.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/omm_stream_connection.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/omm_stream_connection.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/omm_stream_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/omm_stream_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/proxy_info.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/proxy_info.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/rdp_stream.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/rdp_stream.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/rdp_stream_connection.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/rdp_stream_connection.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/rdp_stream_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/rdp_stream_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/rwf/conversion.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/rwf/conversion.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/rwf/ema.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/rwf/ema.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/rwf/socket.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/rwf/socket.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/stream.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/stream.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/stream_cache.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/stream_cache.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/stream_connection.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/stream_connection.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/stream_state_manager.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/stream_state_manager.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/ws/ws_client.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/_stream/ws/ws_client.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_buckets_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/_buckets_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_cfs_data_provider.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/_cfs_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_data_class.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/_data_class.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_data_types.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/_data_types.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_file_downloader.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/_file_downloader.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_file_downloader_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/_file_downloader_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_file_downloader_facade.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/_file_downloader_facade.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_file_sets_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/_file_sets_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_files_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/_files_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_iter_object.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/_iter_object.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_packages_definition.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/_packages_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_tools.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/_tools.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_unpacker.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/_unpacker.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/buckets.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/buckets.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/file_sets.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/cfs/file_sets.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/delivery/omm_stream.py` & `refinitiv-data-1.3.1/refinitiv/data/delivery/omm_stream.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/discovery/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/discovery/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/discovery/_convert_symbols.py` & `refinitiv-data-1.3.1/refinitiv/data/discovery/_convert_symbols.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/discovery/_search.py` & `refinitiv-data-1.3.1/refinitiv/data/discovery/_search.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/discovery/_search_explorer/_buckets_data.py` & `refinitiv-data-1.3.1/refinitiv/data/discovery/_search_explorer/_buckets_data.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/discovery/_search_explorer/_df_builder.py` & `refinitiv-data-1.3.1/refinitiv/data/discovery/_search_explorer/_df_builder.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/discovery/_search_explorer/_property.py` & `refinitiv-data-1.3.1/refinitiv/data/discovery/_search_explorer/_property.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/discovery/_search_explorer/_search_explorer.py` & `refinitiv-data-1.3.1/refinitiv/data/discovery/_search_explorer/_search_explorer.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/discovery/_search_explorer/_search_explorer_response.py` & `refinitiv-data-1.3.1/refinitiv/data/discovery/_search_explorer/_search_explorer_response.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/discovery/_search_templates/base.py` & `refinitiv-data-1.3.1/refinitiv/data/discovery/_search_templates/base.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/discovery/_search_templates/embedded.py` & `refinitiv-data-1.3.1/refinitiv/data/discovery/_search_templates/embedded.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/discovery/_search_templates/manage.py` & `refinitiv-data-1.3.1/refinitiv/data/discovery/_search_templates/manage.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/discovery/_search_templates/namespaces.py` & `refinitiv-data-1.3.1/refinitiv/data/discovery/_search_templates/namespaces.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/discovery/_search_templates/search.py` & `refinitiv-data-1.3.1/refinitiv/data/discovery/_search_templates/search.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/discovery/_search_templates/utils.py` & `refinitiv-data-1.3.1/refinitiv/data/discovery/_search_templates/utils.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/discovery/_stakeholders/_fetch_data.py` & `refinitiv-data-1.3.1/refinitiv/data/discovery/_stakeholders/_fetch_data.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/discovery/_stakeholders/_stakeholder_data.py` & `refinitiv-data-1.3.1/refinitiv/data/discovery/_stakeholders/_stakeholder_data.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/discovery/_stakeholders/_stakeholders.py` & `refinitiv-data-1.3.1/refinitiv/data/discovery/_stakeholders/_stakeholders.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/discovery/_universe_expanders/_chain.py` & `refinitiv-data-1.3.1/refinitiv/data/discovery/_universe_expanders/_chain.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/discovery/_universe_expanders/_discovery_universe.py` & `refinitiv-data-1.3.1/refinitiv/data/discovery/_universe_expanders/_discovery_universe.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/discovery/_universe_expanders/_screener.py` & `refinitiv-data-1.3.1/refinitiv/data/discovery/_universe_expanders/_screener.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/early_access/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/early_access/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/eikon/_data_grid.py` & `refinitiv-data-1.3.1/refinitiv/data/eikon/_data_grid.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/eikon/_json_requests.py` & `refinitiv-data-1.3.1/refinitiv/data/eikon/_json_requests.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/eikon/_news_request.py` & `refinitiv-data-1.3.1/refinitiv/data/eikon/_news_request.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/eikon/_streaming_prices.py` & `refinitiv-data-1.3.1/refinitiv/data/eikon/_streaming_prices.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/eikon/_symbology.py` & `refinitiv-data-1.3.1/refinitiv/data/eikon/_symbology.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/eikon/_time_series.py` & `refinitiv-data-1.3.1/refinitiv/data/eikon/_time_series.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/eikon/_tools.py` & `refinitiv-data-1.3.1/refinitiv/data/eikon/_tools.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/errors.py` & `refinitiv-data-1.3.1/refinitiv/data/errors.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/session/__init__.py` & `refinitiv-data-1.3.1/refinitiv/data/session/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/session/desktop.py` & `refinitiv-data-1.3.1/refinitiv/data/session/desktop.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/session/platform.py` & `refinitiv-data-1.3.1/refinitiv/data/session/platform.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/usage_collection/_logger.py` & `refinitiv-data-1.3.1/refinitiv/data/usage_collection/_logger.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv/data/usage_collection/_utils.py` & `refinitiv-data-1.3.1/refinitiv/data/usage_collection/_utils.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.3.0/refinitiv_data.egg-info/PKG-INFO` & `refinitiv-data-1.3.1/refinitiv_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refinitiv-data
-Version: 1.3.0
+Version: 1.3.1
 Summary: Client for Refinitiv Data Platform API's
 Author: REFINITIV
 License: Apache 2.0
 Project-URL: Homepage, https://developers.refinitiv.com/en/api-catalog/refinitiv-data-platform/refinitiv-data-library-for-python
 Project-URL: Documentation, https://developers.refinitiv.com/en/api-catalog/refinitiv-data-platform/refinitiv-data-library-for-python/documentation
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `refinitiv-data-1.3.0/refinitiv_data.egg-info/SOURCES.txt` & `refinitiv-data-1.3.1/refinitiv_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

