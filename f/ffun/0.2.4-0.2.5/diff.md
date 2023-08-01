# Comparing `tmp/ffun-0.2.4.tar.gz` & `tmp/ffun-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffun-0.2.4.tar", max compression
+gzip compressed data, was "ffun-0.2.5.tar", max compression
```

## Comparing `ffun-0.2.4.tar` & `ffun-0.2.5.tar`

### file list

```diff
@@ -1,133 +1,133 @@
--rw-r--r--   0        0        0      260 2023-08-01 17:22:19.102962 ffun-0.2.4/README.md
--rw-r--r--   0        0        0        0 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/__init__.py
--rw-r--r--   0        0        0        0 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/api/__init__.py
--rw-r--r--   0        0        0     9871 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/api/entities.py
--rw-r--r--   0        0        0    13179 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/api/http_handlers.py
--rw-r--r--   0        0        0        0 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/application/__init__.py
--rw-r--r--   0        0        0     4340 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/application/application.py
--rw-r--r--   0        0        0      115 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/application/errors.py
--rw-r--r--   0        0        0      180 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/application/resources.py
--rw-r--r--   0        0        0     1276 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/application/settings.py
--rw-r--r--   0        0        0     3112 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/application/user_settings.py
--rw-r--r--   0        0        0      278 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/application/utils.py
--rw-r--r--   0        0        0     1460 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/application/workers.py
--rw-r--r--   0        0        0        0 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/auth/__init__.py
--rw-r--r--   0        0        0     1056 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/auth/dependencies.py
--rw-r--r--   0        0        0      802 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/auth/settings.py
--rw-r--r--   0        0        0     2883 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/auth/supertokens.py
--rw-r--r--   0        0        0        0 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/cli/__init__.py
--rw-r--r--   0        0        0      256 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/cli/application.py
--rw-r--r--   0        0        0      240 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/cli/cli.py
--rw-r--r--   0        0        0        0 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/cli/commands/__init__.py
--rw-r--r--   0        0        0      851 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/cli/commands/configs.py
--rw-r--r--   0        0        0      939 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/cli/commands/supertokens.py
--rw-r--r--   0        0        0      878 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/cli/commands/workers.py
--rw-r--r--   0        0        0      858 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/cli/commands/yoyo.py
--rw-r--r--   0        0        0        0 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/core/__init__.py
--rw-r--r--   0        0        0      874 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/core/api.py
--rw-r--r--   0        0        0     3132 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/core/background_tasks.py
--rw-r--r--   0        0        0      372 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/core/errors.py
--rw-r--r--   0        0        0     2583 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/core/json.py
--rw-r--r--   0        0        0     5474 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/core/logging.py
--rw-r--r--   0        0        0     1517 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/core/middlewares.py
--rw-r--r--   0        0        0     3978 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/core/postgresql.py
--rw-r--r--   0        0        0      702 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/core/register.py
--rw-r--r--   0        0        0     1499 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/core/sentry.py
--rw-r--r--   0        0        0      363 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/core/settings.py
--rw-r--r--   0        0        0      486 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/core/text.py
--rw-r--r--   0        0        0     1116 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/core/utils.py
--rw-r--r--   0        0        0        0 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds/__init__.py
--rw-r--r--   0        0        0      307 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds/domain.py
--rw-r--r--   0        0        0     1429 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds/entities.py
--rw-r--r--   0        0        0     1028 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds/migrations/20230329_01_ilwfq-feeds-table.py
--rw-r--r--   0        0        0      642 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds/migrations/20230426_01_IiF5m-add-title-and-description.py
--rw-r--r--   0        0        0     3559 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds/operations.py
--rw-r--r--   0        0        0        0 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds_collections/__init__.py
--rw-r--r--   0        0        0      495 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds_collections/collections/artificial_intelligence.py
--rw-r--r--   0        0        0     1357 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds_collections/collections/gamedev.py
--rw-r--r--   0        0        0      276 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds_collections/domain.py
--rw-r--r--   0        0        0      156 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds_collections/entities.py
--rw-r--r--   0        0        0      530 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds_collections/predefines.py
--rw-r--r--   0        0        0        0 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds_discoverer/__init__.py
--rw-r--r--   0        0        0     3975 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds_discoverer/domain.py
--rw-r--r--   0        0        0        0 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds_links/__init__.py
--rw-r--r--   0        0        0      189 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds_links/domain.py
--rw-r--r--   0        0        0      163 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds_links/entities.py
--rw-r--r--   0        0        0      811 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds_links/migrations/20230427_01_9HuHj-add-feeds-links.py
--rw-r--r--   0        0        0     1488 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds_links/operations.py
--rw-r--r--   0        0        0        0 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/librarian/__init__.py
--rw-r--r--   0        0        0     3235 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/librarian/background_processors.py
--rw-r--r--   0        0        0     1575 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/librarian/domain.py
--rw-r--r--   0        0        0      159 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/librarian/errors.py
--rw-r--r--   0        0        0     4637 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/librarian/history_of_gpt_rules.py
--rw-r--r--   0        0        0        0 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/librarian/processors/__init__.py
--rw-r--r--   0        0        0      418 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/librarian/processors/base.py
--rw-r--r--   0        0        0     1526 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/librarian/processors/domain.py
--rw-r--r--   0        0        0      445 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/librarian/processors/native_tags.py
--rw-r--r--   0        0        0     3351 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/librarian/processors/openai_chat_3_5.py
--rw-r--r--   0        0        0     4686 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/librarian/processors/openai_chat_3_5_functions.py
--rw-r--r--   0        0        0      889 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/librarian/settings.py
--rw-r--r--   0        0        0        0 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/library/__init__.py
--rw-r--r--   0        0        0      432 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/library/domain.py
--rw-r--r--   0        0        0      705 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/library/entities.py
--rw-r--r--   0        0        0     1499 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/library/migrations/20230331_01_UsHwp-entries-table.py
--rw-r--r--   0        0        0     1220 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/library/migrations/20230427_01_pv33u-fix-entries-unique-index.py
--rw-r--r--   0        0        0      711 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/library/migrations/20230514_01_Bwb35-processed-state.py
--rw-r--r--   0        0        0     4824 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/library/operations.py
--rw-r--r--   0        0        0      256 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/library/settings.py
--rw-r--r--   0        0        0        0 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/loader/__init__.py
--rw-r--r--   0        0        0      895 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/loader/background_loader.py
--rw-r--r--   0        0        0     7734 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/loader/domain.py
--rw-r--r--   0        0        0      181 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/loader/errors.py
--rw-r--r--   0        0        0      423 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/loader/settings.py
--rw-r--r--   0        0        0        0 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/markers/__init__.py
--rw-r--r--   0        0        0      140 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/markers/domain.py
--rw-r--r--   0        0        0       57 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/markers/entities.py
--rw-r--r--   0        0        0      856 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/markers/migrations/20230419_01_9vMm5-markers-tables.py
--rw-r--r--   0        0        0     1536 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/markers/operations.py
--rw-r--r--   0        0        0        0 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/ontology/__init__.py
--rw-r--r--   0        0        0     3271 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/ontology/domain.py
--rw-r--r--   0        0        0     1683 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/ontology/entities.py
--rw-r--r--   0        0        0     1093 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/ontology/migrations/20230404_01_ZUBsm-ontology-tables.py
--rw-r--r--   0        0        0      521 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/ontology/migrations/20230617_01_XDdNG-rename-tags-names-to-uid.py
--rw-r--r--   0        0        0      800 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/ontology/migrations/20230617_02_L0MmA-tags-relationship-processor-tracking.py
--rw-r--r--   0        0        0     1009 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/ontology/migrations/20230617_03_de7vS-tags-properties.py
--rw-r--r--   0        0        0     4237 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/ontology/operations.py
--rw-r--r--   0        0        0        0 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/openai/__init__.py
--rw-r--r--   0        0        0     6404 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/openai/client.py
--rw-r--r--   0        0        0      383 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/openai/entities.py
--rw-r--r--   0        0        0      196 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/openai/errors.py
--rw-r--r--   0        0        0     7016 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/openai/keys_rotator.py
--rw-r--r--   0        0        0        0 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/parsers/__init__.py
--rw-r--r--   0        0        0      231 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/parsers/domain.py
--rw-r--r--   0        0        0      560 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/parsers/entities.py
--rw-r--r--   0        0        0     1922 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/parsers/feed.py
--rw-r--r--   0        0        0     1325 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/parsers/feedly.py
--rw-r--r--   0        0        0        0 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/resources/__init__.py
--rw-r--r--   0        0        0      486 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/resources/domain.py
--rw-r--r--   0        0        0      292 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/resources/entities.py
--rw-r--r--   0        0        0      866 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/resources/migrations/20230702_01_LEEES-resources-table.py
--rw-r--r--   0        0        0     3716 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/resources/operations.py
--rw-r--r--   0        0        0        0 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/scores/__init__.py
--rw-r--r--   0        0        0      593 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/scores/domain.py
--rw-r--r--   0        0        0      188 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/scores/entities.py
--rw-r--r--   0        0        0      852 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/scores/migrations/20230417_01_0XYOQ-scores-tables.py
--rw-r--r--   0        0        0     1952 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/scores/operations.py
--rw-r--r--   0        0        0        0 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/tags/__init__.py
--rw-r--r--   0        0        0     1305 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/tags/converters.py
--rw-r--r--   0        0        0        0 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/user_settings/__init__.py
--rw-r--r--   0        0        0     1165 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/user_settings/domain.py
--rw-r--r--   0        0        0       55 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/user_settings/entities.py
--rw-r--r--   0        0        0      733 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/user_settings/migrations/20230701_01_7zBP0-settings-table.py
--rw-r--r--   0        0        0     1469 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/user_settings/operations.py
--rw-r--r--   0        0        0      530 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/user_settings/settings.py
--rw-r--r--   0        0        0     2134 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/user_settings/types.py
--rw-r--r--   0        0        0      434 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/user_settings/values.py
--rw-r--r--   0        0        0        0 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/users/__init__.py
--rw-r--r--   0        0        0      568 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/users/domain.py
--rw-r--r--   0        0        0      161 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/users/entities.py
--rw-r--r--   0        0        0      157 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/users/errors.py
--rw-r--r--   0        0        0      719 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/users/migrations/20230527_01_soIr3-users-mapping.py
--rw-r--r--   0        0        0     1264 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/users/operations.py
--rw-r--r--   0        0        0     3208 2023-08-01 17:22:28.715035 ffun-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     2703 1970-01-01 00:00:00.000000 ffun-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      260 2023-08-01 18:30:57.724228 ffun-0.2.5/README.md
+-rw-r--r--   0        0        0        0 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/api/__init__.py
+-rw-r--r--   0        0        0     9871 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/api/entities.py
+-rw-r--r--   0        0        0    13179 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/api/http_handlers.py
+-rw-r--r--   0        0        0        0 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/application/__init__.py
+-rw-r--r--   0        0        0     4507 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/application/application.py
+-rw-r--r--   0        0        0      115 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/application/errors.py
+-rw-r--r--   0        0        0      180 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/application/resources.py
+-rw-r--r--   0        0        0     1239 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/application/settings.py
+-rw-r--r--   0        0        0     3112 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/application/user_settings.py
+-rw-r--r--   0        0        0      278 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/application/utils.py
+-rw-r--r--   0        0        0     1460 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/application/workers.py
+-rw-r--r--   0        0        0        0 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/auth/__init__.py
+-rw-r--r--   0        0        0     1056 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/auth/dependencies.py
+-rw-r--r--   0        0        0      802 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/auth/settings.py
+-rw-r--r--   0        0        0     2883 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/auth/supertokens.py
+-rw-r--r--   0        0        0        0 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/cli/__init__.py
+-rw-r--r--   0        0        0      256 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/cli/application.py
+-rw-r--r--   0        0        0      240 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/cli/cli.py
+-rw-r--r--   0        0        0        0 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/cli/commands/__init__.py
+-rw-r--r--   0        0        0      851 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/cli/commands/configs.py
+-rw-r--r--   0        0        0      939 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/cli/commands/supertokens.py
+-rw-r--r--   0        0        0      878 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/cli/commands/workers.py
+-rw-r--r--   0        0        0      858 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/cli/commands/yoyo.py
+-rw-r--r--   0        0        0        0 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/core/__init__.py
+-rw-r--r--   0        0        0      874 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/core/api.py
+-rw-r--r--   0        0        0     3132 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/core/background_tasks.py
+-rw-r--r--   0        0        0      372 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/core/errors.py
+-rw-r--r--   0        0        0     2583 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/core/json.py
+-rw-r--r--   0        0        0     5474 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/core/logging.py
+-rw-r--r--   0        0        0     1517 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/core/middlewares.py
+-rw-r--r--   0        0        0     3978 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/core/postgresql.py
+-rw-r--r--   0        0        0      702 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/core/register.py
+-rw-r--r--   0        0        0     1499 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/core/sentry.py
+-rw-r--r--   0        0        0      363 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/core/settings.py
+-rw-r--r--   0        0        0      486 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/core/text.py
+-rw-r--r--   0        0        0     1116 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/core/utils.py
+-rw-r--r--   0        0        0        0 2023-08-01 18:30:57.724228 ffun-0.2.5/ffun/feeds/__init__.py
+-rw-r--r--   0        0        0      307 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/feeds/domain.py
+-rw-r--r--   0        0        0     1429 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/feeds/entities.py
+-rw-r--r--   0        0        0     1028 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/feeds/migrations/20230329_01_ilwfq-feeds-table.py
+-rw-r--r--   0        0        0      642 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/feeds/migrations/20230426_01_IiF5m-add-title-and-description.py
+-rw-r--r--   0        0        0     3559 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/feeds/operations.py
+-rw-r--r--   0        0        0        0 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/feeds_collections/__init__.py
+-rw-r--r--   0        0        0      495 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/feeds_collections/collections/artificial_intelligence.py
+-rw-r--r--   0        0        0     1357 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/feeds_collections/collections/gamedev.py
+-rw-r--r--   0        0        0      276 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/feeds_collections/domain.py
+-rw-r--r--   0        0        0      156 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/feeds_collections/entities.py
+-rw-r--r--   0        0        0      530 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/feeds_collections/predefines.py
+-rw-r--r--   0        0        0        0 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/feeds_discoverer/__init__.py
+-rw-r--r--   0        0        0     3975 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/feeds_discoverer/domain.py
+-rw-r--r--   0        0        0        0 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/feeds_links/__init__.py
+-rw-r--r--   0        0        0      189 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/feeds_links/domain.py
+-rw-r--r--   0        0        0      163 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/feeds_links/entities.py
+-rw-r--r--   0        0        0      811 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/feeds_links/migrations/20230427_01_9HuHj-add-feeds-links.py
+-rw-r--r--   0        0        0     1488 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/feeds_links/operations.py
+-rw-r--r--   0        0        0        0 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/librarian/__init__.py
+-rw-r--r--   0        0        0     3235 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/librarian/background_processors.py
+-rw-r--r--   0        0        0     1575 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/librarian/domain.py
+-rw-r--r--   0        0        0      159 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/librarian/errors.py
+-rw-r--r--   0        0        0     4637 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/librarian/history_of_gpt_rules.py
+-rw-r--r--   0        0        0        0 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/librarian/processors/__init__.py
+-rw-r--r--   0        0        0      418 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/librarian/processors/base.py
+-rw-r--r--   0        0        0     1526 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/librarian/processors/domain.py
+-rw-r--r--   0        0        0      445 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/librarian/processors/native_tags.py
+-rw-r--r--   0        0        0     3351 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/librarian/processors/openai_chat_3_5.py
+-rw-r--r--   0        0        0     4686 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/librarian/processors/openai_chat_3_5_functions.py
+-rw-r--r--   0        0        0      889 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/librarian/settings.py
+-rw-r--r--   0        0        0        0 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/library/__init__.py
+-rw-r--r--   0        0        0      432 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/library/domain.py
+-rw-r--r--   0        0        0      705 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/library/entities.py
+-rw-r--r--   0        0        0     1499 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/library/migrations/20230331_01_UsHwp-entries-table.py
+-rw-r--r--   0        0        0     1220 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/library/migrations/20230427_01_pv33u-fix-entries-unique-index.py
+-rw-r--r--   0        0        0      711 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/library/migrations/20230514_01_Bwb35-processed-state.py
+-rw-r--r--   0        0        0     4824 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/library/operations.py
+-rw-r--r--   0        0        0      256 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/library/settings.py
+-rw-r--r--   0        0        0        0 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/loader/__init__.py
+-rw-r--r--   0        0        0      895 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/loader/background_loader.py
+-rw-r--r--   0        0        0     7734 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/loader/domain.py
+-rw-r--r--   0        0        0      181 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/loader/errors.py
+-rw-r--r--   0        0        0      423 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/loader/settings.py
+-rw-r--r--   0        0        0        0 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/markers/__init__.py
+-rw-r--r--   0        0        0      140 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/markers/domain.py
+-rw-r--r--   0        0        0       57 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/markers/entities.py
+-rw-r--r--   0        0        0      856 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/markers/migrations/20230419_01_9vMm5-markers-tables.py
+-rw-r--r--   0        0        0     1536 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/markers/operations.py
+-rw-r--r--   0        0        0        0 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/ontology/__init__.py
+-rw-r--r--   0        0        0     3271 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/ontology/domain.py
+-rw-r--r--   0        0        0     1683 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/ontology/entities.py
+-rw-r--r--   0        0        0     1093 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/ontology/migrations/20230404_01_ZUBsm-ontology-tables.py
+-rw-r--r--   0        0        0      521 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/ontology/migrations/20230617_01_XDdNG-rename-tags-names-to-uid.py
+-rw-r--r--   0        0        0      800 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/ontology/migrations/20230617_02_L0MmA-tags-relationship-processor-tracking.py
+-rw-r--r--   0        0        0     1009 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/ontology/migrations/20230617_03_de7vS-tags-properties.py
+-rw-r--r--   0        0        0     4237 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/ontology/operations.py
+-rw-r--r--   0        0        0        0 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/openai/__init__.py
+-rw-r--r--   0        0        0     6404 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/openai/client.py
+-rw-r--r--   0        0        0      383 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/openai/entities.py
+-rw-r--r--   0        0        0      196 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/openai/errors.py
+-rw-r--r--   0        0        0     7016 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/openai/keys_rotator.py
+-rw-r--r--   0        0        0        0 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/parsers/__init__.py
+-rw-r--r--   0        0        0      231 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/parsers/domain.py
+-rw-r--r--   0        0        0      560 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/parsers/entities.py
+-rw-r--r--   0        0        0     1922 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/parsers/feed.py
+-rw-r--r--   0        0        0     1325 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/parsers/feedly.py
+-rw-r--r--   0        0        0        0 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/resources/__init__.py
+-rw-r--r--   0        0        0      486 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/resources/domain.py
+-rw-r--r--   0        0        0      292 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/resources/entities.py
+-rw-r--r--   0        0        0      866 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/resources/migrations/20230702_01_LEEES-resources-table.py
+-rw-r--r--   0        0        0     3716 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/resources/operations.py
+-rw-r--r--   0        0        0        0 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/scores/__init__.py
+-rw-r--r--   0        0        0      593 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/scores/domain.py
+-rw-r--r--   0        0        0      188 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/scores/entities.py
+-rw-r--r--   0        0        0      852 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/scores/migrations/20230417_01_0XYOQ-scores-tables.py
+-rw-r--r--   0        0        0     1952 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/scores/operations.py
+-rw-r--r--   0        0        0        0 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/tags/__init__.py
+-rw-r--r--   0        0        0     1305 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/tags/converters.py
+-rw-r--r--   0        0        0        0 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/user_settings/__init__.py
+-rw-r--r--   0        0        0     1165 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/user_settings/domain.py
+-rw-r--r--   0        0        0       55 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/user_settings/entities.py
+-rw-r--r--   0        0        0      733 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/user_settings/migrations/20230701_01_7zBP0-settings-table.py
+-rw-r--r--   0        0        0     1469 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/user_settings/operations.py
+-rw-r--r--   0        0        0      530 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/user_settings/settings.py
+-rw-r--r--   0        0        0     2134 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/user_settings/types.py
+-rw-r--r--   0        0        0      434 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/user_settings/values.py
+-rw-r--r--   0        0        0        0 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/users/__init__.py
+-rw-r--r--   0        0        0      568 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/users/domain.py
+-rw-r--r--   0        0        0      161 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/users/entities.py
+-rw-r--r--   0        0        0      157 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/users/errors.py
+-rw-r--r--   0        0        0      719 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/users/migrations/20230527_01_soIr3-users-mapping.py
+-rw-r--r--   0        0        0     1264 2023-08-01 18:30:57.728227 ffun-0.2.5/ffun/users/operations.py
+-rw-r--r--   0        0        0     3208 2023-08-01 18:31:06.776225 ffun-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2703 1970-01-01 00:00:00.000000 ffun-0.2.5/PKG-INFO
```

### Comparing `ffun-0.2.4/ffun/api/entities.py` & `ffun-0.2.5/ffun/api/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/api/http_handlers.py` & `ffun-0.2.5/ffun/api/http_handlers.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/application/application.py` & `ffun-0.2.5/ffun/application/application.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from typing import AsyncGenerator, Generator
 
 import fastapi
 from fastapi.middleware.cors import CORSMiddleware
 
 from ffun.api import http_handlers as api_http_handlers
 from ffun.auth import supertokens as st
+from ffun.auth.settings import AuthMode
+from ffun.auth.settings import settings as auth_settings
 from ffun.core import logging, middlewares, postgresql, sentry
 from ffun.librarian.background_processors import create_background_processors
 from ffun.loader.background_loader import FeedsLoader
 
 from . import errors
 from .settings import settings
 
@@ -102,15 +104,15 @@
     async def lifespan(app: fastapi.FastAPI) -> AsyncGenerator[None, None]:
         async with contextlib.AsyncExitStack() as stack:
             await stack.enter_async_context(use_postgresql())
 
             if settings.enable_sentry:
                 await stack.enter_async_context(use_sentry())
 
-            if settings.enable_supertokens:
+            if auth_settings.mode == AuthMode.supertokens:
                 api_domain = smart_url(settings.app_domain, settings.api_port)
                 website_domain = smart_url(settings.app_domain, settings.app_port)
 
                 await stack.enter_async_context(
                     st.use_supertokens(
                         app_name=settings.app_name, api_domain=api_domain, website_domain=website_domain
                     )
@@ -130,15 +132,16 @@
         docs_url=None,
         redoc_url=None,
         openapi_url=None,
     )
 
     middlewares.initialize_error_processors(app)
 
-    st.add_middlewares(app)
+    if auth_settings.mode == AuthMode.supertokens:
+        st.add_middlewares(app)
 
     app.middleware("http")(middlewares.final_errors_middleware)
 
     app.add_middleware(
         CORSMiddleware,
         allow_origins=["http://localhost", "http://localhost:5173", "http://127.0.0.1", "http://127.0.0.1:5173"],
         allow_credentials=True,
```

### Comparing `ffun-0.2.4/ffun/application/settings.py` & `ffun-0.2.5/ffun/application/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,15 +40,14 @@
     app_port: int = 5173
 
     environment: str = "local"
 
     api_port: int = 5174
 
     enable_api: bool = False
-    enable_supertokens: bool = False
     enable_sentry: bool = False
 
     postgresql: PostgreSQL = PostgreSQL()
     sentry: Sentry = Sentry()
 
     class Config:
         env_prefix = "FFUN_"
```

### Comparing `ffun-0.2.4/ffun/application/user_settings.py` & `ffun-0.2.5/ffun/application/user_settings.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/application/workers.py` & `ffun-0.2.5/ffun/application/workers.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/auth/dependencies.py` & `ffun-0.2.5/ffun/auth/dependencies.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/auth/settings.py` & `ffun-0.2.5/ffun/auth/settings.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/auth/supertokens.py` & `ffun-0.2.5/ffun/auth/supertokens.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/cli/commands/configs.py` & `ffun-0.2.5/ffun/cli/commands/configs.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/cli/commands/supertokens.py` & `ffun-0.2.5/ffun/cli/commands/supertokens.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/cli/commands/workers.py` & `ffun-0.2.5/ffun/cli/commands/workers.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/cli/commands/yoyo.py` & `ffun-0.2.5/ffun/cli/commands/yoyo.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/core/api.py` & `ffun-0.2.5/ffun/core/api.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/core/background_tasks.py` & `ffun-0.2.5/ffun/core/background_tasks.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/core/json.py` & `ffun-0.2.5/ffun/core/json.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/core/logging.py` & `ffun-0.2.5/ffun/core/logging.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/core/middlewares.py` & `ffun-0.2.5/ffun/core/middlewares.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/core/postgresql.py` & `ffun-0.2.5/ffun/core/postgresql.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/core/register.py` & `ffun-0.2.5/ffun/core/register.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/core/sentry.py` & `ffun-0.2.5/ffun/core/sentry.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/core/utils.py` & `ffun-0.2.5/ffun/core/utils.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/feeds/entities.py` & `ffun-0.2.5/ffun/feeds/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/feeds/migrations/20230329_01_ilwfq-feeds-table.py` & `ffun-0.2.5/ffun/feeds/migrations/20230329_01_ilwfq-feeds-table.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/feeds/migrations/20230426_01_IiF5m-add-title-and-description.py` & `ffun-0.2.5/ffun/feeds/migrations/20230426_01_IiF5m-add-title-and-description.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/feeds/operations.py` & `ffun-0.2.5/ffun/feeds/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/feeds_collections/collections/gamedev.py` & `ffun-0.2.5/ffun/feeds_collections/collections/gamedev.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/feeds_collections/predefines.py` & `ffun-0.2.5/ffun/feeds_collections/predefines.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/feeds_discoverer/domain.py` & `ffun-0.2.5/ffun/feeds_discoverer/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/feeds_links/migrations/20230427_01_9HuHj-add-feeds-links.py` & `ffun-0.2.5/ffun/feeds_links/migrations/20230427_01_9HuHj-add-feeds-links.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/feeds_links/operations.py` & `ffun-0.2.5/ffun/feeds_links/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/librarian/background_processors.py` & `ffun-0.2.5/ffun/librarian/background_processors.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/librarian/domain.py` & `ffun-0.2.5/ffun/librarian/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/librarian/history_of_gpt_rules.py` & `ffun-0.2.5/ffun/librarian/history_of_gpt_rules.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/librarian/processors/domain.py` & `ffun-0.2.5/ffun/librarian/processors/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/librarian/processors/openai_chat_3_5.py` & `ffun-0.2.5/ffun/librarian/processors/openai_chat_3_5.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/librarian/processors/openai_chat_3_5_functions.py` & `ffun-0.2.5/ffun/librarian/processors/openai_chat_3_5_functions.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/librarian/settings.py` & `ffun-0.2.5/ffun/librarian/settings.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/library/entities.py` & `ffun-0.2.5/ffun/library/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/library/migrations/20230331_01_UsHwp-entries-table.py` & `ffun-0.2.5/ffun/library/migrations/20230331_01_UsHwp-entries-table.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/library/migrations/20230427_01_pv33u-fix-entries-unique-index.py` & `ffun-0.2.5/ffun/library/migrations/20230427_01_pv33u-fix-entries-unique-index.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/library/migrations/20230514_01_Bwb35-processed-state.py` & `ffun-0.2.5/ffun/library/migrations/20230514_01_Bwb35-processed-state.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/library/operations.py` & `ffun-0.2.5/ffun/library/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/loader/background_loader.py` & `ffun-0.2.5/ffun/loader/background_loader.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/loader/domain.py` & `ffun-0.2.5/ffun/loader/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/markers/migrations/20230419_01_9vMm5-markers-tables.py` & `ffun-0.2.5/ffun/markers/migrations/20230419_01_9vMm5-markers-tables.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/markers/operations.py` & `ffun-0.2.5/ffun/markers/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/ontology/domain.py` & `ffun-0.2.5/ffun/ontology/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/ontology/entities.py` & `ffun-0.2.5/ffun/ontology/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/ontology/migrations/20230404_01_ZUBsm-ontology-tables.py` & `ffun-0.2.5/ffun/ontology/migrations/20230404_01_ZUBsm-ontology-tables.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/ontology/migrations/20230617_01_XDdNG-rename-tags-names-to-uid.py` & `ffun-0.2.5/ffun/ontology/migrations/20230617_01_XDdNG-rename-tags-names-to-uid.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/ontology/migrations/20230617_02_L0MmA-tags-relationship-processor-tracking.py` & `ffun-0.2.5/ffun/ontology/migrations/20230617_02_L0MmA-tags-relationship-processor-tracking.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/ontology/migrations/20230617_03_de7vS-tags-properties.py` & `ffun-0.2.5/ffun/ontology/migrations/20230617_03_de7vS-tags-properties.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/ontology/operations.py` & `ffun-0.2.5/ffun/ontology/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/openai/client.py` & `ffun-0.2.5/ffun/openai/client.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/openai/keys_rotator.py` & `ffun-0.2.5/ffun/openai/keys_rotator.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/parsers/entities.py` & `ffun-0.2.5/ffun/parsers/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/parsers/feed.py` & `ffun-0.2.5/ffun/parsers/feed.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/parsers/feedly.py` & `ffun-0.2.5/ffun/parsers/feedly.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/resources/migrations/20230702_01_LEEES-resources-table.py` & `ffun-0.2.5/ffun/resources/migrations/20230702_01_LEEES-resources-table.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/resources/operations.py` & `ffun-0.2.5/ffun/resources/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/scores/domain.py` & `ffun-0.2.5/ffun/scores/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/scores/migrations/20230417_01_0XYOQ-scores-tables.py` & `ffun-0.2.5/ffun/scores/migrations/20230417_01_0XYOQ-scores-tables.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/scores/operations.py` & `ffun-0.2.5/ffun/scores/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/tags/converters.py` & `ffun-0.2.5/ffun/tags/converters.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/user_settings/domain.py` & `ffun-0.2.5/ffun/user_settings/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/user_settings/migrations/20230701_01_7zBP0-settings-table.py` & `ffun-0.2.5/ffun/user_settings/migrations/20230701_01_7zBP0-settings-table.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/user_settings/operations.py` & `ffun-0.2.5/ffun/user_settings/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/user_settings/settings.py` & `ffun-0.2.5/ffun/user_settings/settings.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/user_settings/types.py` & `ffun-0.2.5/ffun/user_settings/types.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/users/domain.py` & `ffun-0.2.5/ffun/users/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/users/migrations/20230527_01_soIr3-users-mapping.py` & `ffun-0.2.5/ffun/users/migrations/20230527_01_soIr3-users-mapping.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/ffun/users/operations.py` & `ffun-0.2.5/ffun/users/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.4/pyproject.toml` & `ffun-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ffun"
-version = "0.2.4"
+version = "0.2.5"
 description = "Backend for the Feeds Fun — web-based news reader"
 repository = "https://github.com/Tiendil/feeds.fun"
 authors = ["Aliaksei Yaletski (Tiendil) <a.eletsky@gmail.com>"]
 license = " BSD-3-Clause"
 readme = "README.md"
 homepage = "https://feeds.fun"
 keywords = ["news", "news-reader", "news-aggregator",
```

### Comparing `ffun-0.2.4/PKG-INFO` & `ffun-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffun
-Version: 0.2.4
+Version: 0.2.5
 Summary: Backend for the Feeds Fun — web-based news reader
 Home-page: https://feeds.fun
 License:  BSD-3-Clause
 Keywords: news,news-reader,news-aggregator,rss,rss-reader,rss-aggregator,feed,feed-reader,feed-aggregator,atom,self-hosted
 Author: Aliaksei Yaletski (Tiendil)
 Author-email: a.eletsky@gmail.com
 Requires-Python: >=3.11,<4.0
```

