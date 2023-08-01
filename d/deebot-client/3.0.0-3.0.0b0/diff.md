# Comparing `tmp/deebot-client-3.0.0.tar.gz` & `tmp/deebot-client-3.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deebot-client-3.0.0.tar", last modified: Tue Aug  1 16:49:47 2023, max compression
+gzip compressed data, was "deebot-client-3.0.0b0.tar", last modified: Sat Jul 29 09:55:57 2023, max compression
```

## Comparing `deebot-client-3.0.0.tar` & `deebot-client-3.0.0b0.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:49:47.827419 deebot-client-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-08-01 16:49:43.000000 deebot-client-3.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-08-01 16:49:47.827419 deebot-client-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-08-01 16:49:43.000000 deebot-client-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:49:47.807418 deebot-client-3.0.0/deebot_client/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13794 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:49:47.815419 deebot-client-3.0.0/deebot_client/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/commands/advanced_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/commands/battery.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/commands/carpet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/commands/charge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/commands/charge_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/commands/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/commands/clean_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/commands/clean_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/commands/clean_preference.py
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/commands/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/commands/continuous_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/commands/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/commands/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/commands/fan_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/commands/life_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/commands/map.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/commands/multimap_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/commands/play_sound.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/commands/pos.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/commands/relocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/commands/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/commands/true_detect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/commands/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/commands/water_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:49:47.823419 deebot-client-3.0.0/deebot_client/events/
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/events/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/events/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/events/event_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/events/fan_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/events/map.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/events/water_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/logging_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21756 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:49:47.823419 deebot-client-3.0.0/deebot_client/messages/
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/messages/battery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/messages/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11224 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/mqtt_client.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-08-01 16:49:43.000000 deebot-client-3.0.0/deebot_client/vacuum_bot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:49:47.807418 deebot-client-3.0.0/deebot_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-08-01 16:49:47.000000 deebot-client-3.0.0/deebot_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-08-01 16:49:47.000000 deebot-client-3.0.0/deebot_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 16:49:47.000000 deebot-client-3.0.0/deebot_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-01 16:49:47.000000 deebot-client-3.0.0/deebot_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 16:49:47.000000 deebot-client-3.0.0/deebot_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 16:49:43.000000 deebot-client-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-08-01 16:49:47.827419 deebot-client-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-08-01 16:49:43.000000 deebot-client-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:49:47.799418 deebot-client-3.0.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:49:47.827419 deebot-client-3.0.0/tests/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-08-01 16:49:43.000000 deebot-client-3.0.0/tests/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-08-01 16:49:43.000000 deebot-client-3.0.0/tests/commands/test_advanced_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-08-01 16:49:43.000000 deebot-client-3.0.0/tests/commands/test_battery.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-08-01 16:49:43.000000 deebot-client-3.0.0/tests/commands/test_carpet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-08-01 16:49:43.000000 deebot-client-3.0.0/tests/commands/test_charge.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-01 16:49:43.000000 deebot-client-3.0.0/tests/commands/test_charge_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-08-01 16:49:43.000000 deebot-client-3.0.0/tests/commands/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-01 16:49:43.000000 deebot-client-3.0.0/tests/commands/test_clean_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-08-01 16:49:43.000000 deebot-client-3.0.0/tests/commands/test_clean_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-01 16:49:43.000000 deebot-client-3.0.0/tests/commands/test_clean_preference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-08-01 16:49:43.000000 deebot-client-3.0.0/tests/commands/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-08-01 16:49:43.000000 deebot-client-3.0.0/tests/commands/test_continuous_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-08-01 16:49:43.000000 deebot-client-3.0.0/tests/commands/test_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-01 16:49:43.000000 deebot-client-3.0.0/tests/commands/test_fan_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-01 16:49:43.000000 deebot-client-3.0.0/tests/commands/test_life_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-08-01 16:49:43.000000 deebot-client-3.0.0/tests/commands/test_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-01 16:49:43.000000 deebot-client-3.0.0/tests/commands/test_mulitmap_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-08-01 16:49:43.000000 deebot-client-3.0.0/tests/commands/test_true_detect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-08-01 16:49:43.000000 deebot-client-3.0.0/tests/commands/test_water_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:49:47.827419 deebot-client-3.0.0/tests/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 16:49:43.000000 deebot-client-3.0.0/tests/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-08-01 16:49:43.000000 deebot-client-3.0.0/tests/events/test_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-01 16:49:43.000000 deebot-client-3.0.0/tests/events/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-01 16:49:43.000000 deebot-client-3.0.0/tests/events/test_water_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:49:47.827419 deebot-client-3.0.0/tests/messages/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-01 16:49:43.000000 deebot-client-3.0.0/tests/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-01 16:49:43.000000 deebot-client-3.0.0/tests/messages/test_battery.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-08-01 16:49:43.000000 deebot-client-3.0.0/tests/messages/test_get_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-01 16:49:43.000000 deebot-client-3.0.0/tests/messages/test_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-08-01 16:49:43.000000 deebot-client-3.0.0/tests/messages/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:55:57.355691 deebot-client-3.0.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-29 09:55:57.355691 deebot-client-3.0.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:55:57.347691 deebot-client-3.0.0b0/deebot_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13794 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:55:57.347691 deebot-client-3.0.0b0/deebot_client/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/advanced_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/carpet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/charge_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/clean_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/clean_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/clean_preference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/continuous_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/fan_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/life_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/multimap_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/play_sound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/pos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/relocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/true_detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/water_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:55:57.347691 deebot-client-3.0.0b0/deebot_client/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/events/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/events/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/events/event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/events/fan_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/events/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/events/water_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/logging_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21756 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:55:57.347691 deebot-client-3.0.0b0/deebot_client/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/messages/battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/messages/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11224 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/mqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/vacuum_bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:55:57.347691 deebot-client-3.0.0b0/deebot_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-29 09:55:57.000000 deebot-client-3.0.0b0/deebot_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-29 09:55:57.000000 deebot-client-3.0.0b0/deebot_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 09:55:57.000000 deebot-client-3.0.0b0/deebot_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-29 09:55:57.000000 deebot-client-3.0.0b0/deebot_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 09:55:57.000000 deebot-client-3.0.0b0/deebot_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-29 09:55:57.355691 deebot-client-3.0.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:55:57.343691 deebot-client-3.0.0b0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:55:57.351691 deebot-client-3.0.0b0/tests/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_advanced_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_carpet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_charge_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_clean_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_clean_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_clean_preference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_continuous_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_fan_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_life_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_mulitmap_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_true_detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_water_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:55:57.351691 deebot-client-3.0.0b0/tests/events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/events/test_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/events/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/events/test_water_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:55:57.355691 deebot-client-3.0.0b0/tests/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/messages/test_battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/messages/test_get_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/messages/test_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/messages/test_stats.py
```

### Comparing `deebot-client-3.0.0/LICENSE.txt` & `deebot-client-3.0.0b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/PKG-INFO` & `deebot-client-3.0.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deebot-client
-Version: 3.0.0
+Version: 3.0.0b0
 Summary: a library for controlling certain deebot vacuums
 Home-page: https://github.com/DeebotUniverse/client.py
 Author: DeebotUniverse
 Author-email: deebotuniverse@knatschig-as-hell.info
 License: GPL-3.0
 Keywords: home automation vacuum robot deebot ecovacs
 Classifier: Development Status :: 4 - Beta
```

### Comparing `deebot-client-3.0.0/README.md` & `deebot-client-3.0.0b0/README.md`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/deebot_client/api_client.py` & `deebot-client-3.0.0b0/deebot_client/api_client.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/deebot_client/authentication.py` & `deebot-client-3.0.0b0/deebot_client/authentication.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/deebot_client/command.py` & `deebot-client-3.0.0b0/deebot_client/command.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/deebot_client/commands/__init__.py` & `deebot-client-3.0.0b0/deebot_client/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/deebot_client/commands/charge.py` & `deebot-client-3.0.0b0/deebot_client/commands/charge.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/deebot_client/commands/charge_state.py` & `deebot-client-3.0.0b0/deebot_client/commands/charge_state.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/deebot_client/commands/clean.py` & `deebot-client-3.0.0b0/deebot_client/commands/clean.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/deebot_client/commands/clean_count.py` & `deebot-client-3.0.0b0/deebot_client/commands/clean_count.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/deebot_client/commands/clean_logs.py` & `deebot-client-3.0.0b0/deebot_client/commands/clean_logs.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/deebot_client/commands/common.py` & `deebot-client-3.0.0b0/deebot_client/commands/common.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/deebot_client/commands/custom.py` & `deebot-client-3.0.0b0/deebot_client/commands/custom.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/deebot_client/commands/error.py` & `deebot-client-3.0.0b0/deebot_client/commands/error.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/deebot_client/commands/fan_speed.py` & `deebot-client-3.0.0b0/deebot_client/commands/fan_speed.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/deebot_client/commands/life_span.py` & `deebot-client-3.0.0b0/deebot_client/commands/life_span.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/deebot_client/commands/map.py` & `deebot-client-3.0.0b0/deebot_client/commands/map.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/deebot_client/commands/pos.py` & `deebot-client-3.0.0b0/deebot_client/commands/pos.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/deebot_client/commands/stats.py` & `deebot-client-3.0.0b0/deebot_client/commands/stats.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/deebot_client/commands/volume.py` & `deebot-client-3.0.0b0/deebot_client/commands/volume.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/deebot_client/commands/water_info.py` & `deebot-client-3.0.0b0/deebot_client/commands/water_info.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/deebot_client/events/__init__.py` & `deebot-client-3.0.0b0/deebot_client/events/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/deebot_client/events/const.py` & `deebot-client-3.0.0b0/deebot_client/events/const.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/deebot_client/events/event_bus.py` & `deebot-client-3.0.0b0/deebot_client/events/event_bus.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/deebot_client/events/map.py` & `deebot-client-3.0.0b0/deebot_client/events/map.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/deebot_client/logging_filter.py` & `deebot-client-3.0.0b0/deebot_client/logging_filter.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/deebot_client/map.py` & `deebot-client-3.0.0b0/deebot_client/map.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/deebot_client/message.py` & `deebot-client-3.0.0b0/deebot_client/message.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/deebot_client/messages/__init__.py` & `deebot-client-3.0.0b0/deebot_client/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/deebot_client/messages/battery.py` & `deebot-client-3.0.0b0/deebot_client/messages/battery.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/deebot_client/messages/stats.py` & `deebot-client-3.0.0b0/deebot_client/messages/stats.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/deebot_client/models.py` & `deebot-client-3.0.0b0/deebot_client/models.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/deebot_client/mqtt_client.py` & `deebot-client-3.0.0b0/deebot_client/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/deebot_client/util.py` & `deebot-client-3.0.0b0/deebot_client/util.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/deebot_client/vacuum_bot.py` & `deebot-client-3.0.0b0/deebot_client/vacuum_bot.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/deebot_client.egg-info/PKG-INFO` & `deebot-client-3.0.0b0/deebot_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deebot-client
-Version: 3.0.0
+Version: 3.0.0b0
 Summary: a library for controlling certain deebot vacuums
 Home-page: https://github.com/DeebotUniverse/client.py
 Author: DeebotUniverse
 Author-email: deebotuniverse@knatschig-as-hell.info
 License: GPL-3.0
 Keywords: home automation vacuum robot deebot ecovacs
 Classifier: Development Status :: 4 - Beta
```

### Comparing `deebot-client-3.0.0/deebot_client.egg-info/SOURCES.txt` & `deebot-client-3.0.0b0/deebot_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/setup.py` & `deebot-client-3.0.0b0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = file.read()
 
 with open("requirements.txt", encoding="utf-8") as file:
     install_requires = list(val.strip() for val in file)
 
 setup(
     name="deebot-client",
-    version="3.0.0",
+    version="3.0.0b0",
     url="https://github.com/DeebotUniverse/client.py",
     description="a library for controlling certain deebot vacuums",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="DeebotUniverse",
     author_email="deebotuniverse@knatschig-as-hell.info",
     license="GPL-3.0",
```

### Comparing `deebot-client-3.0.0/tests/commands/__init__.py` & `deebot-client-3.0.0b0/tests/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/tests/commands/test_advanced_mode.py` & `deebot-client-3.0.0b0/tests/commands/test_advanced_mode.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/tests/commands/test_carpet.py` & `deebot-client-3.0.0b0/tests/commands/test_carpet.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/tests/commands/test_charge.py` & `deebot-client-3.0.0b0/tests/commands/test_charge.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/tests/commands/test_clean.py` & `deebot-client-3.0.0b0/tests/commands/test_clean.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/tests/commands/test_clean_count.py` & `deebot-client-3.0.0b0/tests/commands/test_clean_count.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/tests/commands/test_clean_log.py` & `deebot-client-3.0.0b0/tests/commands/test_clean_log.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/tests/commands/test_clean_preference.py` & `deebot-client-3.0.0b0/tests/commands/test_clean_preference.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/tests/commands/test_common.py` & `deebot-client-3.0.0b0/tests/commands/test_common.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/tests/commands/test_continuous_cleaning.py` & `deebot-client-3.0.0b0/tests/commands/test_continuous_cleaning.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/tests/commands/test_custom.py` & `deebot-client-3.0.0b0/tests/commands/test_custom.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/tests/commands/test_fan_speed.py` & `deebot-client-3.0.0b0/tests/commands/test_fan_speed.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/tests/commands/test_life_span.py` & `deebot-client-3.0.0b0/tests/commands/test_life_span.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/tests/commands/test_map.py` & `deebot-client-3.0.0b0/tests/commands/test_map.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/tests/commands/test_mulitmap_state.py` & `deebot-client-3.0.0b0/tests/commands/test_mulitmap_state.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/tests/commands/test_true_detect.py` & `deebot-client-3.0.0b0/tests/commands/test_true_detect.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/tests/commands/test_water_info.py` & `deebot-client-3.0.0b0/tests/commands/test_water_info.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/tests/events/test_event_bus.py` & `deebot-client-3.0.0b0/tests/events/test_event_bus.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/tests/messages/test_battery.py` & `deebot-client-3.0.0b0/tests/messages/test_battery.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/tests/messages/test_get_messages.py` & `deebot-client-3.0.0b0/tests/messages/test_get_messages.py`

 * *Files identical despite different names*

### Comparing `deebot-client-3.0.0/tests/messages/test_stats.py` & `deebot-client-3.0.0b0/tests/messages/test_stats.py`

 * *Files identical despite different names*

