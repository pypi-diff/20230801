# Comparing `tmp/ffun-0.2.3.tar.gz` & `tmp/ffun-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffun-0.2.3.tar", max compression
+gzip compressed data, was "ffun-0.2.4.tar", max compression
```

## Comparing `ffun-0.2.3.tar` & `ffun-0.2.4.tar`

### file list

```diff
@@ -1,132 +1,133 @@
--rw-r--r--   0        0        0      260 2023-07-31 18:52:31.893327 ffun-0.2.3/README.md
--rw-r--r--   0        0        0        0 2023-07-31 18:52:31.893327 ffun-0.2.3/ffun/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 18:52:31.893327 ffun-0.2.3/ffun/api/__init__.py
--rw-r--r--   0        0        0     9871 2023-07-31 18:52:31.893327 ffun-0.2.3/ffun/api/entities.py
--rw-r--r--   0        0        0    13179 2023-07-31 18:52:31.893327 ffun-0.2.3/ffun/api/http_handlers.py
--rw-r--r--   0        0        0        0 2023-07-31 18:52:31.893327 ffun-0.2.3/ffun/application/__init__.py
--rw-r--r--   0        0        0     4340 2023-07-31 18:52:31.893327 ffun-0.2.3/ffun/application/application.py
--rw-r--r--   0        0        0      115 2023-07-31 18:52:31.893327 ffun-0.2.3/ffun/application/errors.py
--rw-r--r--   0        0        0      180 2023-07-31 18:52:31.893327 ffun-0.2.3/ffun/application/resources.py
--rw-r--r--   0        0        0     1274 2023-07-31 18:52:31.893327 ffun-0.2.3/ffun/application/settings.py
--rw-r--r--   0        0        0     3112 2023-07-31 18:52:31.893327 ffun-0.2.3/ffun/application/user_settings.py
--rw-r--r--   0        0        0      278 2023-07-31 18:52:31.893327 ffun-0.2.3/ffun/application/utils.py
--rw-r--r--   0        0        0     1460 2023-07-31 18:52:31.893327 ffun-0.2.3/ffun/application/workers.py
--rw-r--r--   0        0        0        0 2023-07-31 18:52:31.893327 ffun-0.2.3/ffun/auth/__init__.py
--rw-r--r--   0        0        0     1056 2023-07-31 18:52:31.893327 ffun-0.2.3/ffun/auth/dependencies.py
--rw-r--r--   0        0        0      802 2023-07-31 18:52:31.893327 ffun-0.2.3/ffun/auth/settings.py
--rw-r--r--   0        0        0     2883 2023-07-31 18:52:31.893327 ffun-0.2.3/ffun/auth/supertokens.py
--rw-r--r--   0        0        0        0 2023-07-31 18:52:31.893327 ffun-0.2.3/ffun/cli/__init__.py
--rw-r--r--   0        0        0      256 2023-07-31 18:52:31.893327 ffun-0.2.3/ffun/cli/application.py
--rw-r--r--   0        0        0      196 2023-07-31 18:52:31.893327 ffun-0.2.3/ffun/cli/cli.py
--rw-r--r--   0        0        0        0 2023-07-31 18:52:31.893327 ffun-0.2.3/ffun/cli/commands/__init__.py
--rw-r--r--   0        0        0      939 2023-07-31 18:52:31.893327 ffun-0.2.3/ffun/cli/commands/supertokens.py
--rw-r--r--   0        0        0      878 2023-07-31 18:52:31.893327 ffun-0.2.3/ffun/cli/commands/workers.py
--rw-r--r--   0        0        0      858 2023-07-31 18:52:31.893327 ffun-0.2.3/ffun/cli/commands/yoyo.py
--rw-r--r--   0        0        0        0 2023-07-31 18:52:31.893327 ffun-0.2.3/ffun/core/__init__.py
--rw-r--r--   0        0        0      874 2023-07-31 18:52:31.893327 ffun-0.2.3/ffun/core/api.py
--rw-r--r--   0        0        0     3132 2023-07-31 18:52:31.893327 ffun-0.2.3/ffun/core/background_tasks.py
--rw-r--r--   0        0        0      372 2023-07-31 18:52:31.893327 ffun-0.2.3/ffun/core/errors.py
--rw-r--r--   0        0        0     2583 2023-07-31 18:52:31.893327 ffun-0.2.3/ffun/core/json.py
--rw-r--r--   0        0        0     5474 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/core/logging.py
--rw-r--r--   0        0        0     1517 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/core/middlewares.py
--rw-r--r--   0        0        0     3978 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/core/postgresql.py
--rw-r--r--   0        0        0      702 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/core/register.py
--rw-r--r--   0        0        0     1499 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/core/sentry.py
--rw-r--r--   0        0        0      363 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/core/settings.py
--rw-r--r--   0        0        0      486 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/core/text.py
--rw-r--r--   0        0        0      109 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/core/utils.py
--rw-r--r--   0        0        0        0 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/feeds/__init__.py
--rw-r--r--   0        0        0      307 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/feeds/domain.py
--rw-r--r--   0        0        0     1429 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/feeds/entities.py
--rw-r--r--   0        0        0     1028 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/feeds/migrations/20230329_01_ilwfq-feeds-table.py
--rw-r--r--   0        0        0      642 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/feeds/migrations/20230426_01_IiF5m-add-title-and-description.py
--rw-r--r--   0        0        0     3559 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/feeds/operations.py
--rw-r--r--   0        0        0        0 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/feeds_collections/__init__.py
--rw-r--r--   0        0        0      495 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/feeds_collections/collections/artificial_intelligence.py
--rw-r--r--   0        0        0     1357 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/feeds_collections/collections/gamedev.py
--rw-r--r--   0        0        0      276 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/feeds_collections/domain.py
--rw-r--r--   0        0        0      156 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/feeds_collections/entities.py
--rw-r--r--   0        0        0      530 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/feeds_collections/predefines.py
--rw-r--r--   0        0        0        0 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/feeds_discoverer/__init__.py
--rw-r--r--   0        0        0     3975 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/feeds_discoverer/domain.py
--rw-r--r--   0        0        0        0 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/feeds_links/__init__.py
--rw-r--r--   0        0        0      189 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/feeds_links/domain.py
--rw-r--r--   0        0        0      163 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/feeds_links/entities.py
--rw-r--r--   0        0        0      811 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/feeds_links/migrations/20230427_01_9HuHj-add-feeds-links.py
--rw-r--r--   0        0        0     1488 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/feeds_links/operations.py
--rw-r--r--   0        0        0        0 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/librarian/__init__.py
--rw-r--r--   0        0        0     3235 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/librarian/background_processors.py
--rw-r--r--   0        0        0     1575 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/librarian/domain.py
--rw-r--r--   0        0        0      159 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/librarian/errors.py
--rw-r--r--   0        0        0     4637 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/librarian/history_of_gpt_rules.py
--rw-r--r--   0        0        0        0 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/librarian/processors/__init__.py
--rw-r--r--   0        0        0      418 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/librarian/processors/base.py
--rw-r--r--   0        0        0     1526 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/librarian/processors/domain.py
--rw-r--r--   0        0        0      445 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/librarian/processors/native_tags.py
--rw-r--r--   0        0        0     3351 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/librarian/processors/openai_chat_3_5.py
--rw-r--r--   0        0        0     4686 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/librarian/processors/openai_chat_3_5_functions.py
--rw-r--r--   0        0        0      889 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/librarian/settings.py
--rw-r--r--   0        0        0        0 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/library/__init__.py
--rw-r--r--   0        0        0      432 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/library/domain.py
--rw-r--r--   0        0        0      705 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/library/entities.py
--rw-r--r--   0        0        0     1499 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/library/migrations/20230331_01_UsHwp-entries-table.py
--rw-r--r--   0        0        0     1220 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/library/migrations/20230427_01_pv33u-fix-entries-unique-index.py
--rw-r--r--   0        0        0      711 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/library/migrations/20230514_01_Bwb35-processed-state.py
--rw-r--r--   0        0        0     4824 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/library/operations.py
--rw-r--r--   0        0        0      256 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/library/settings.py
--rw-r--r--   0        0        0        0 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/loader/__init__.py
--rw-r--r--   0        0        0      895 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/loader/background_loader.py
--rw-r--r--   0        0        0     7734 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/loader/domain.py
--rw-r--r--   0        0        0      181 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/loader/errors.py
--rw-r--r--   0        0        0      423 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/loader/settings.py
--rw-r--r--   0        0        0        0 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/markers/__init__.py
--rw-r--r--   0        0        0      140 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/markers/domain.py
--rw-r--r--   0        0        0       57 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/markers/entities.py
--rw-r--r--   0        0        0      856 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/markers/migrations/20230419_01_9vMm5-markers-tables.py
--rw-r--r--   0        0        0     1536 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/markers/operations.py
--rw-r--r--   0        0        0        0 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/ontology/__init__.py
--rw-r--r--   0        0        0     3271 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/ontology/domain.py
--rw-r--r--   0        0        0     1683 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/ontology/entities.py
--rw-r--r--   0        0        0     1093 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/ontology/migrations/20230404_01_ZUBsm-ontology-tables.py
--rw-r--r--   0        0        0      521 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/ontology/migrations/20230617_01_XDdNG-rename-tags-names-to-uid.py
--rw-r--r--   0        0        0      800 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/ontology/migrations/20230617_02_L0MmA-tags-relationship-processor-tracking.py
--rw-r--r--   0        0        0     1009 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/ontology/migrations/20230617_03_de7vS-tags-properties.py
--rw-r--r--   0        0        0     4237 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/ontology/operations.py
--rw-r--r--   0        0        0        0 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/openai/__init__.py
--rw-r--r--   0        0        0     6404 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/openai/client.py
--rw-r--r--   0        0        0      383 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/openai/entities.py
--rw-r--r--   0        0        0      196 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/openai/errors.py
--rw-r--r--   0        0        0     7016 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/openai/keys_rotator.py
--rw-r--r--   0        0        0        0 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/parsers/__init__.py
--rw-r--r--   0        0        0      231 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/parsers/domain.py
--rw-r--r--   0        0        0      560 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/parsers/entities.py
--rw-r--r--   0        0        0     1922 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/parsers/feed.py
--rw-r--r--   0        0        0     1325 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/parsers/feedly.py
--rw-r--r--   0        0        0        0 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/resources/__init__.py
--rw-r--r--   0        0        0      486 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/resources/domain.py
--rw-r--r--   0        0        0      292 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/resources/entities.py
--rw-r--r--   0        0        0      866 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/resources/migrations/20230702_01_LEEES-resources-table.py
--rw-r--r--   0        0        0     3716 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/resources/operations.py
--rw-r--r--   0        0        0        0 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/scores/__init__.py
--rw-r--r--   0        0        0      593 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/scores/domain.py
--rw-r--r--   0        0        0      188 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/scores/entities.py
--rw-r--r--   0        0        0      852 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/scores/migrations/20230417_01_0XYOQ-scores-tables.py
--rw-r--r--   0        0        0     1952 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/scores/operations.py
--rw-r--r--   0        0        0        0 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/tags/__init__.py
--rw-r--r--   0        0        0     1305 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/tags/converters.py
--rw-r--r--   0        0        0        0 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/user_settings/__init__.py
--rw-r--r--   0        0        0     1165 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/user_settings/domain.py
--rw-r--r--   0        0        0       55 2023-07-31 18:52:31.897327 ffun-0.2.3/ffun/user_settings/entities.py
--rw-r--r--   0        0        0      733 2023-07-31 18:52:31.901327 ffun-0.2.3/ffun/user_settings/migrations/20230701_01_7zBP0-settings-table.py
--rw-r--r--   0        0        0     1469 2023-07-31 18:52:31.901327 ffun-0.2.3/ffun/user_settings/operations.py
--rw-r--r--   0        0        0      530 2023-07-31 18:52:31.901327 ffun-0.2.3/ffun/user_settings/settings.py
--rw-r--r--   0        0        0     2134 2023-07-31 18:52:31.901327 ffun-0.2.3/ffun/user_settings/types.py
--rw-r--r--   0        0        0      434 2023-07-31 18:52:31.901327 ffun-0.2.3/ffun/user_settings/values.py
--rw-r--r--   0        0        0        0 2023-07-31 18:52:31.901327 ffun-0.2.3/ffun/users/__init__.py
--rw-r--r--   0        0        0      568 2023-07-31 18:52:31.901327 ffun-0.2.3/ffun/users/domain.py
--rw-r--r--   0        0        0      161 2023-07-31 18:52:31.901327 ffun-0.2.3/ffun/users/entities.py
--rw-r--r--   0        0        0      157 2023-07-31 18:52:31.901327 ffun-0.2.3/ffun/users/errors.py
--rw-r--r--   0        0        0      719 2023-07-31 18:52:31.901327 ffun-0.2.3/ffun/users/migrations/20230527_01_soIr3-users-mapping.py
--rw-r--r--   0        0        0     1264 2023-07-31 18:52:31.901327 ffun-0.2.3/ffun/users/operations.py
--rw-r--r--   0        0        0     3171 2023-07-31 18:52:45.745562 ffun-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2703 1970-01-01 00:00:00.000000 ffun-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      260 2023-08-01 17:22:19.102962 ffun-0.2.4/README.md
+-rw-r--r--   0        0        0        0 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/api/__init__.py
+-rw-r--r--   0        0        0     9871 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/api/entities.py
+-rw-r--r--   0        0        0    13179 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/api/http_handlers.py
+-rw-r--r--   0        0        0        0 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/application/__init__.py
+-rw-r--r--   0        0        0     4340 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/application/application.py
+-rw-r--r--   0        0        0      115 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/application/errors.py
+-rw-r--r--   0        0        0      180 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/application/resources.py
+-rw-r--r--   0        0        0     1276 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/application/settings.py
+-rw-r--r--   0        0        0     3112 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/application/user_settings.py
+-rw-r--r--   0        0        0      278 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/application/utils.py
+-rw-r--r--   0        0        0     1460 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/application/workers.py
+-rw-r--r--   0        0        0        0 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/auth/__init__.py
+-rw-r--r--   0        0        0     1056 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/auth/dependencies.py
+-rw-r--r--   0        0        0      802 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/auth/settings.py
+-rw-r--r--   0        0        0     2883 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/auth/supertokens.py
+-rw-r--r--   0        0        0        0 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/cli/__init__.py
+-rw-r--r--   0        0        0      256 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/cli/application.py
+-rw-r--r--   0        0        0      240 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/cli/cli.py
+-rw-r--r--   0        0        0        0 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/cli/commands/__init__.py
+-rw-r--r--   0        0        0      851 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/cli/commands/configs.py
+-rw-r--r--   0        0        0      939 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/cli/commands/supertokens.py
+-rw-r--r--   0        0        0      878 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/cli/commands/workers.py
+-rw-r--r--   0        0        0      858 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/cli/commands/yoyo.py
+-rw-r--r--   0        0        0        0 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/core/__init__.py
+-rw-r--r--   0        0        0      874 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/core/api.py
+-rw-r--r--   0        0        0     3132 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/core/background_tasks.py
+-rw-r--r--   0        0        0      372 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/core/errors.py
+-rw-r--r--   0        0        0     2583 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/core/json.py
+-rw-r--r--   0        0        0     5474 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/core/logging.py
+-rw-r--r--   0        0        0     1517 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/core/middlewares.py
+-rw-r--r--   0        0        0     3978 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/core/postgresql.py
+-rw-r--r--   0        0        0      702 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/core/register.py
+-rw-r--r--   0        0        0     1499 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/core/sentry.py
+-rw-r--r--   0        0        0      363 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/core/settings.py
+-rw-r--r--   0        0        0      486 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/core/text.py
+-rw-r--r--   0        0        0     1116 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/core/utils.py
+-rw-r--r--   0        0        0        0 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds/__init__.py
+-rw-r--r--   0        0        0      307 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds/domain.py
+-rw-r--r--   0        0        0     1429 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds/entities.py
+-rw-r--r--   0        0        0     1028 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds/migrations/20230329_01_ilwfq-feeds-table.py
+-rw-r--r--   0        0        0      642 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds/migrations/20230426_01_IiF5m-add-title-and-description.py
+-rw-r--r--   0        0        0     3559 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds/operations.py
+-rw-r--r--   0        0        0        0 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds_collections/__init__.py
+-rw-r--r--   0        0        0      495 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds_collections/collections/artificial_intelligence.py
+-rw-r--r--   0        0        0     1357 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds_collections/collections/gamedev.py
+-rw-r--r--   0        0        0      276 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds_collections/domain.py
+-rw-r--r--   0        0        0      156 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds_collections/entities.py
+-rw-r--r--   0        0        0      530 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds_collections/predefines.py
+-rw-r--r--   0        0        0        0 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds_discoverer/__init__.py
+-rw-r--r--   0        0        0     3975 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds_discoverer/domain.py
+-rw-r--r--   0        0        0        0 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds_links/__init__.py
+-rw-r--r--   0        0        0      189 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds_links/domain.py
+-rw-r--r--   0        0        0      163 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds_links/entities.py
+-rw-r--r--   0        0        0      811 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds_links/migrations/20230427_01_9HuHj-add-feeds-links.py
+-rw-r--r--   0        0        0     1488 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/feeds_links/operations.py
+-rw-r--r--   0        0        0        0 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/librarian/__init__.py
+-rw-r--r--   0        0        0     3235 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/librarian/background_processors.py
+-rw-r--r--   0        0        0     1575 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/librarian/domain.py
+-rw-r--r--   0        0        0      159 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/librarian/errors.py
+-rw-r--r--   0        0        0     4637 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/librarian/history_of_gpt_rules.py
+-rw-r--r--   0        0        0        0 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/librarian/processors/__init__.py
+-rw-r--r--   0        0        0      418 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/librarian/processors/base.py
+-rw-r--r--   0        0        0     1526 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/librarian/processors/domain.py
+-rw-r--r--   0        0        0      445 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/librarian/processors/native_tags.py
+-rw-r--r--   0        0        0     3351 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/librarian/processors/openai_chat_3_5.py
+-rw-r--r--   0        0        0     4686 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/librarian/processors/openai_chat_3_5_functions.py
+-rw-r--r--   0        0        0      889 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/librarian/settings.py
+-rw-r--r--   0        0        0        0 2023-08-01 17:22:19.102962 ffun-0.2.4/ffun/library/__init__.py
+-rw-r--r--   0        0        0      432 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/library/domain.py
+-rw-r--r--   0        0        0      705 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/library/entities.py
+-rw-r--r--   0        0        0     1499 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/library/migrations/20230331_01_UsHwp-entries-table.py
+-rw-r--r--   0        0        0     1220 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/library/migrations/20230427_01_pv33u-fix-entries-unique-index.py
+-rw-r--r--   0        0        0      711 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/library/migrations/20230514_01_Bwb35-processed-state.py
+-rw-r--r--   0        0        0     4824 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/library/operations.py
+-rw-r--r--   0        0        0      256 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/library/settings.py
+-rw-r--r--   0        0        0        0 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/loader/__init__.py
+-rw-r--r--   0        0        0      895 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/loader/background_loader.py
+-rw-r--r--   0        0        0     7734 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/loader/domain.py
+-rw-r--r--   0        0        0      181 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/loader/errors.py
+-rw-r--r--   0        0        0      423 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/loader/settings.py
+-rw-r--r--   0        0        0        0 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/markers/__init__.py
+-rw-r--r--   0        0        0      140 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/markers/domain.py
+-rw-r--r--   0        0        0       57 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/markers/entities.py
+-rw-r--r--   0        0        0      856 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/markers/migrations/20230419_01_9vMm5-markers-tables.py
+-rw-r--r--   0        0        0     1536 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/markers/operations.py
+-rw-r--r--   0        0        0        0 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/ontology/__init__.py
+-rw-r--r--   0        0        0     3271 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/ontology/domain.py
+-rw-r--r--   0        0        0     1683 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/ontology/entities.py
+-rw-r--r--   0        0        0     1093 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/ontology/migrations/20230404_01_ZUBsm-ontology-tables.py
+-rw-r--r--   0        0        0      521 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/ontology/migrations/20230617_01_XDdNG-rename-tags-names-to-uid.py
+-rw-r--r--   0        0        0      800 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/ontology/migrations/20230617_02_L0MmA-tags-relationship-processor-tracking.py
+-rw-r--r--   0        0        0     1009 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/ontology/migrations/20230617_03_de7vS-tags-properties.py
+-rw-r--r--   0        0        0     4237 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/ontology/operations.py
+-rw-r--r--   0        0        0        0 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/openai/__init__.py
+-rw-r--r--   0        0        0     6404 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/openai/client.py
+-rw-r--r--   0        0        0      383 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/openai/entities.py
+-rw-r--r--   0        0        0      196 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/openai/errors.py
+-rw-r--r--   0        0        0     7016 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/openai/keys_rotator.py
+-rw-r--r--   0        0        0        0 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/parsers/__init__.py
+-rw-r--r--   0        0        0      231 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/parsers/domain.py
+-rw-r--r--   0        0        0      560 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/parsers/entities.py
+-rw-r--r--   0        0        0     1922 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/parsers/feed.py
+-rw-r--r--   0        0        0     1325 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/parsers/feedly.py
+-rw-r--r--   0        0        0        0 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/resources/__init__.py
+-rw-r--r--   0        0        0      486 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/resources/domain.py
+-rw-r--r--   0        0        0      292 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/resources/entities.py
+-rw-r--r--   0        0        0      866 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/resources/migrations/20230702_01_LEEES-resources-table.py
+-rw-r--r--   0        0        0     3716 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/resources/operations.py
+-rw-r--r--   0        0        0        0 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/scores/__init__.py
+-rw-r--r--   0        0        0      593 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/scores/domain.py
+-rw-r--r--   0        0        0      188 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/scores/entities.py
+-rw-r--r--   0        0        0      852 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/scores/migrations/20230417_01_0XYOQ-scores-tables.py
+-rw-r--r--   0        0        0     1952 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/scores/operations.py
+-rw-r--r--   0        0        0        0 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/tags/__init__.py
+-rw-r--r--   0        0        0     1305 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/tags/converters.py
+-rw-r--r--   0        0        0        0 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/user_settings/__init__.py
+-rw-r--r--   0        0        0     1165 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/user_settings/domain.py
+-rw-r--r--   0        0        0       55 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/user_settings/entities.py
+-rw-r--r--   0        0        0      733 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/user_settings/migrations/20230701_01_7zBP0-settings-table.py
+-rw-r--r--   0        0        0     1469 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/user_settings/operations.py
+-rw-r--r--   0        0        0      530 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/user_settings/settings.py
+-rw-r--r--   0        0        0     2134 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/user_settings/types.py
+-rw-r--r--   0        0        0      434 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/user_settings/values.py
+-rw-r--r--   0        0        0        0 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/users/__init__.py
+-rw-r--r--   0        0        0      568 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/users/domain.py
+-rw-r--r--   0        0        0      161 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/users/entities.py
+-rw-r--r--   0        0        0      157 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/users/errors.py
+-rw-r--r--   0        0        0      719 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/users/migrations/20230527_01_soIr3-users-mapping.py
+-rw-r--r--   0        0        0     1264 2023-08-01 17:22:19.106962 ffun-0.2.4/ffun/users/operations.py
+-rw-r--r--   0        0        0     3208 2023-08-01 17:22:28.715035 ffun-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2703 1970-01-01 00:00:00.000000 ffun-0.2.4/PKG-INFO
```

### Comparing `ffun-0.2.3/ffun/api/entities.py` & `ffun-0.2.4/ffun/api/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/api/http_handlers.py` & `ffun-0.2.4/ffun/api/http_handlers.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/application/application.py` & `ffun-0.2.4/ffun/application/application.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/application/settings.py` & `ffun-0.2.4/ffun/application/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     port: int = 5432
     user: str = "ffun"
     password: str = "ffun"
     database: str = "ffun"
 
     pool_min_size: int = 20
     pool_max_size: int | None = None
-    pool_timeout: float = 1
+    pool_timeout: float = 1.0
     pool_num_workers: int = 1
     pool_max_lifetime: int = 9 * 60
     pool_check_period: int = 60
 
     @property
     def dsn(self) -> str:
         return f"postgresql://{self.user}:{self.password}@{self.host}:{self.port}/{self.database}"
```

### Comparing `ffun-0.2.3/ffun/application/user_settings.py` & `ffun-0.2.4/ffun/application/user_settings.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/application/workers.py` & `ffun-0.2.4/ffun/application/workers.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/auth/dependencies.py` & `ffun-0.2.4/ffun/auth/dependencies.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/auth/settings.py` & `ffun-0.2.4/ffun/auth/settings.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/auth/supertokens.py` & `ffun-0.2.4/ffun/auth/supertokens.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/cli/commands/supertokens.py` & `ffun-0.2.4/ffun/cli/commands/supertokens.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/cli/commands/workers.py` & `ffun-0.2.4/ffun/cli/commands/workers.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/cli/commands/yoyo.py` & `ffun-0.2.4/ffun/cli/commands/yoyo.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/core/api.py` & `ffun-0.2.4/ffun/core/api.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/core/background_tasks.py` & `ffun-0.2.4/ffun/core/background_tasks.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/core/json.py` & `ffun-0.2.4/ffun/core/json.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/core/logging.py` & `ffun-0.2.4/ffun/core/logging.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/core/middlewares.py` & `ffun-0.2.4/ffun/core/middlewares.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/core/postgresql.py` & `ffun-0.2.4/ffun/core/postgresql.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/core/register.py` & `ffun-0.2.4/ffun/core/register.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/core/sentry.py` & `ffun-0.2.4/ffun/core/sentry.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/feeds/entities.py` & `ffun-0.2.4/ffun/feeds/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/feeds/migrations/20230329_01_ilwfq-feeds-table.py` & `ffun-0.2.4/ffun/feeds/migrations/20230329_01_ilwfq-feeds-table.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/feeds/migrations/20230426_01_IiF5m-add-title-and-description.py` & `ffun-0.2.4/ffun/feeds/migrations/20230426_01_IiF5m-add-title-and-description.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/feeds/operations.py` & `ffun-0.2.4/ffun/feeds/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/feeds_collections/collections/gamedev.py` & `ffun-0.2.4/ffun/feeds_collections/collections/gamedev.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/feeds_collections/predefines.py` & `ffun-0.2.4/ffun/feeds_collections/predefines.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/feeds_discoverer/domain.py` & `ffun-0.2.4/ffun/feeds_discoverer/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/feeds_links/migrations/20230427_01_9HuHj-add-feeds-links.py` & `ffun-0.2.4/ffun/feeds_links/migrations/20230427_01_9HuHj-add-feeds-links.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/feeds_links/operations.py` & `ffun-0.2.4/ffun/feeds_links/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/librarian/background_processors.py` & `ffun-0.2.4/ffun/librarian/background_processors.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/librarian/domain.py` & `ffun-0.2.4/ffun/librarian/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/librarian/history_of_gpt_rules.py` & `ffun-0.2.4/ffun/librarian/history_of_gpt_rules.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/librarian/processors/domain.py` & `ffun-0.2.4/ffun/librarian/processors/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/librarian/processors/openai_chat_3_5.py` & `ffun-0.2.4/ffun/librarian/processors/openai_chat_3_5.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/librarian/processors/openai_chat_3_5_functions.py` & `ffun-0.2.4/ffun/librarian/processors/openai_chat_3_5_functions.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/librarian/settings.py` & `ffun-0.2.4/ffun/librarian/settings.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/library/entities.py` & `ffun-0.2.4/ffun/library/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/library/migrations/20230331_01_UsHwp-entries-table.py` & `ffun-0.2.4/ffun/library/migrations/20230331_01_UsHwp-entries-table.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/library/migrations/20230427_01_pv33u-fix-entries-unique-index.py` & `ffun-0.2.4/ffun/library/migrations/20230427_01_pv33u-fix-entries-unique-index.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/library/migrations/20230514_01_Bwb35-processed-state.py` & `ffun-0.2.4/ffun/library/migrations/20230514_01_Bwb35-processed-state.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/library/operations.py` & `ffun-0.2.4/ffun/library/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/loader/background_loader.py` & `ffun-0.2.4/ffun/loader/background_loader.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/loader/domain.py` & `ffun-0.2.4/ffun/loader/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/markers/migrations/20230419_01_9vMm5-markers-tables.py` & `ffun-0.2.4/ffun/markers/migrations/20230419_01_9vMm5-markers-tables.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/markers/operations.py` & `ffun-0.2.4/ffun/markers/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/ontology/domain.py` & `ffun-0.2.4/ffun/ontology/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/ontology/entities.py` & `ffun-0.2.4/ffun/ontology/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/ontology/migrations/20230404_01_ZUBsm-ontology-tables.py` & `ffun-0.2.4/ffun/ontology/migrations/20230404_01_ZUBsm-ontology-tables.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/ontology/migrations/20230617_01_XDdNG-rename-tags-names-to-uid.py` & `ffun-0.2.4/ffun/ontology/migrations/20230617_01_XDdNG-rename-tags-names-to-uid.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/ontology/migrations/20230617_02_L0MmA-tags-relationship-processor-tracking.py` & `ffun-0.2.4/ffun/ontology/migrations/20230617_02_L0MmA-tags-relationship-processor-tracking.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/ontology/migrations/20230617_03_de7vS-tags-properties.py` & `ffun-0.2.4/ffun/ontology/migrations/20230617_03_de7vS-tags-properties.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/ontology/operations.py` & `ffun-0.2.4/ffun/ontology/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/openai/client.py` & `ffun-0.2.4/ffun/openai/client.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/openai/keys_rotator.py` & `ffun-0.2.4/ffun/openai/keys_rotator.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/parsers/entities.py` & `ffun-0.2.4/ffun/parsers/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/parsers/feed.py` & `ffun-0.2.4/ffun/parsers/feed.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/parsers/feedly.py` & `ffun-0.2.4/ffun/parsers/feedly.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/resources/migrations/20230702_01_LEEES-resources-table.py` & `ffun-0.2.4/ffun/resources/migrations/20230702_01_LEEES-resources-table.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/resources/operations.py` & `ffun-0.2.4/ffun/resources/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/scores/domain.py` & `ffun-0.2.4/ffun/scores/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/scores/migrations/20230417_01_0XYOQ-scores-tables.py` & `ffun-0.2.4/ffun/scores/migrations/20230417_01_0XYOQ-scores-tables.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/scores/operations.py` & `ffun-0.2.4/ffun/scores/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/tags/converters.py` & `ffun-0.2.4/ffun/tags/converters.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/user_settings/domain.py` & `ffun-0.2.4/ffun/user_settings/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/user_settings/migrations/20230701_01_7zBP0-settings-table.py` & `ffun-0.2.4/ffun/user_settings/migrations/20230701_01_7zBP0-settings-table.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/user_settings/operations.py` & `ffun-0.2.4/ffun/user_settings/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/user_settings/settings.py` & `ffun-0.2.4/ffun/user_settings/settings.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/user_settings/types.py` & `ffun-0.2.4/ffun/user_settings/types.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/users/domain.py` & `ffun-0.2.4/ffun/users/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/users/migrations/20230527_01_soIr3-users-mapping.py` & `ffun-0.2.4/ffun/users/migrations/20230527_01_soIr3-users-mapping.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/ffun/users/operations.py` & `ffun-0.2.4/ffun/users/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-0.2.3/pyproject.toml` & `ffun-0.2.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ffun"
-version = "0.2.3"
+version = "0.2.4"
 description = "Backend for the Feeds Fun — web-based news reader"
 repository = "https://github.com/Tiendil/feeds.fun"
 authors = ["Aliaksei Yaletski (Tiendil) <a.eletsky@gmail.com>"]
 license = " BSD-3-Clause"
 readme = "README.md"
 homepage = "https://feeds.fun"
 keywords = ["news", "news-reader", "news-aggregator",
@@ -79,15 +79,17 @@
 
 [tool.poetry.dev-dependencies]
 
 pytest = "7.4.*"
 
 isort = "5.12.*"
 black = "23.7.*"
-mypy = "1.4.*"
+
+# mypy fails in the latest versions
+mypy = "1.3.*"
 
 types-python-slugify = "8.0.*"
 types-beautifulsoup4 = "4.12.*"
 types-markdown = "3.4.*"
 types-pkg-resources = "0.1.*"
 types-tabulate = "0.9.*"
```

### Comparing `ffun-0.2.3/PKG-INFO` & `ffun-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffun
-Version: 0.2.3
+Version: 0.2.4
 Summary: Backend for the Feeds Fun — web-based news reader
 Home-page: https://feeds.fun
 License:  BSD-3-Clause
 Keywords: news,news-reader,news-aggregator,rss,rss-reader,rss-aggregator,feed,feed-reader,feed-aggregator,atom,self-hosted
 Author: Aliaksei Yaletski (Tiendil)
 Author-email: a.eletsky@gmail.com
 Requires-Python: >=3.11,<4.0
```

