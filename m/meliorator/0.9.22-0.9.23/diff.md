# Comparing `tmp/meliorator-0.9.22.tar.gz` & `tmp/meliorator-0.9.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meliorator-0.9.22.tar", max compression
+gzip compressed data, was "meliorator-0.9.23.tar", max compression
```

## Comparing `meliorator-0.9.22.tar` & `meliorator-0.9.23.tar`

### file list

```diff
@@ -1,146 +1,146 @@
--rw-r--r--   0        0        0     1062 2023-07-21 20:39:52.702169 meliorator-0.9.22/LICENSE
--rw-r--r--   0        0        0    20599 2023-07-21 20:39:52.702169 meliorator-0.9.22/README.rst
--rw-r--r--   0        0        0      298 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/__init__.py
--rw-r--r--   0        0        0       24 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/commands/__init__.py
--rw-r--r--   0        0        0      785 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/commands/application.py
--rw-r--r--   0        0        0     3453 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/commands/command.py
--rw-r--r--   0        0        0      330 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/commands/migrations/__init__.py
--rw-r--r--   0        0        0      186 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/commands/migrations/base_command.py
--rw-r--r--   0        0        0      626 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/commands/migrations/install_command.py
--rw-r--r--   0        0        0     1301 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/commands/migrations/make_command.py
--rw-r--r--   0        0        0     2343 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/commands/migrations/migrate_command.py
--rw-r--r--   0        0        0     1886 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/commands/migrations/refresh_command.py
--rw-r--r--   0        0        0     1308 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/commands/migrations/reset_command.py
--rw-r--r--   0        0        0     1315 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/commands/migrations/rollback_command.py
--rw-r--r--   0        0        0     1642 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/commands/migrations/status_command.py
--rw-r--r--   0        0        0       68 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/commands/models/__init__.py
--rw-r--r--   0        0        0     2217 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/commands/models/make_command.py
--rw-r--r--   0        0        0      115 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/commands/models/stubs.py
--rw-r--r--   0        0        0      108 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/commands/seeds/__init__.py
--rw-r--r--   0        0        0      178 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/commands/seeds/base_command.py
--rw-r--r--   0        0        0     2204 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/commands/seeds/make_command.py
--rw-r--r--   0        0        0     1923 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/commands/seeds/seed_command.py
--rw-r--r--   0        0        0      206 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/connections/__init__.py
--rw-r--r--   0        0        0    15863 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/connections/connection.py
--rw-r--r--   0        0        0     4112 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/connections/connection_interface.py
--rw-r--r--   0        0        0      298 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/connections/connection_resolver_interface.py
--rw-r--r--   0        0        0     2218 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/connections/mysql_connection.py
--rw-r--r--   0        0        0     2480 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/connections/postgres_connection.py
--rw-r--r--   0        0        0     1588 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/connections/sqlite_connection.py
--rw-r--r--   0        0        0      198 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/connectors/__init__.py
--rw-r--r--   0        0        0     3133 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/connectors/connection_factory.py
--rw-r--r--   0        0        0     3106 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/connectors/connector.py
--rw-r--r--   0        0        0     3886 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/connectors/mysql_connector.py
--rw-r--r--   0        0        0     3280 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/connectors/postgres_connector.py
--rw-r--r--   0        0        0     2065 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/connectors/sqlite_connector.py
--rw-r--r--   0        0        0     5089 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/database_manager.py
--rw-r--r--   0        0        0       24 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/dbal/__init__.py
--rw-r--r--   0        0        0     2372 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/dbal/abstract_asset.py
--rw-r--r--   0        0        0     3447 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/dbal/column.py
--rw-r--r--   0        0        0      545 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/dbal/column_diff.py
--rw-r--r--   0        0        0    11219 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/dbal/comparator.py
--rw-r--r--   0        0        0     1943 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/dbal/exceptions/__init__.py
--rw-r--r--   0        0        0     8193 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/dbal/foreign_key_constraint.py
--rw-r--r--   0        0        0      173 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/dbal/identifier.py
--rw-r--r--   0        0        0     7094 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/dbal/index.py
--rw-r--r--   0        0        0     5260 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/dbal/mysql_schema_manager.py
--rw-r--r--   0        0        0      205 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/dbal/platforms/__init__.py
--rw-r--r--   0        0        0       24 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/dbal/platforms/keywords/__init__.py
--rw-r--r--   0        0        0      209 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/dbal/platforms/keywords/keyword_list.py
--rw-r--r--   0        0        0     4383 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/dbal/platforms/keywords/mysql_keywords.py
--rw-r--r--   0        0        0     1730 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/dbal/platforms/keywords/postgresql_keywords.py
--rw-r--r--   0        0        0     2315 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/dbal/platforms/keywords/sqlite_keywords.py
--rw-r--r--   0        0        0     1254 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/dbal/platforms/mysql57_platform.py
--rw-r--r--   0        0        0     9489 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/dbal/platforms/mysql_platform.py
--rw-r--r--   0        0        0    21672 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/dbal/platforms/platform.py
--rw-r--r--   0        0        0    14126 2023-07-21 20:39:52.702169 meliorator-0.9.22/orator/dbal/platforms/postgres_platform.py
--rw-r--r--   0        0        0    20833 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/dbal/platforms/sqlite_platform.py
--rw-r--r--   0        0        0     6014 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/dbal/postgres_schema_manager.py
--rw-r--r--   0        0        0     4240 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/dbal/schema_manager.py
--rw-r--r--   0        0        0     5458 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/dbal/sqlite_schema_manager.py
--rw-r--r--   0        0        0    17146 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/dbal/table.py
--rw-r--r--   0        0        0     1436 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/dbal/table_diff.py
--rw-r--r--   0        0        0       24 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/dbal/types/__init__.py
--rw-r--r--   0        0        0      992 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/events/__init__.py
--rw-r--r--   0        0        0       68 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/exceptions/__init__.py
--rw-r--r--   0        0        0      193 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/exceptions/connection.py
--rw-r--r--   0        0        0      822 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/exceptions/connectors.py
--rw-r--r--   0        0        0      551 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/exceptions/orm.py
--rw-r--r--   0        0        0      494 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/exceptions/query.py
--rw-r--r--   0        0        0      208 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/migrations/__init__.py
--rw-r--r--   0        0        0     2730 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/migrations/database_migration_repository.py
--rw-r--r--   0        0        0      425 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/migrations/migration.py
--rw-r--r--   0        0        0     2588 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/migrations/migration_creator.py
--rw-r--r--   0        0        0     7754 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/migrations/migrator.py
--rw-r--r--   0        0        0     1114 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/migrations/stubs.py
--rw-r--r--   0        0        0      419 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/orm/__init__.py
--rw-r--r--   0        0        0    32311 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/orm/builder.py
--rw-r--r--   0        0        0      814 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/orm/collection.py
--rw-r--r--   0        0        0     7481 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/orm/factory.py
--rw-r--r--   0        0        0     2579 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/orm/factory_builder.py
--rw-r--r--   0        0        0       63 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/orm/mixins/__init__.py
--rw-r--r--   0        0        0     3532 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/orm/mixins/soft_deletes.py
--rw-r--r--   0        0        0    75367 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/orm/model.py
--rw-r--r--   0        0        0      371 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/orm/relations/__init__.py
--rw-r--r--   0        0        0     5427 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/orm/relations/belongs_to.py
--rw-r--r--   0        0        0    23246 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/orm/relations/belongs_to_many.py
--rw-r--r--   0        0        0     1012 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/orm/relations/has_many.py
--rw-r--r--   0        0        0     5126 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/orm/relations/has_many_through.py
--rw-r--r--   0        0        0      955 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/orm/relations/has_one.py
--rw-r--r--   0        0        0     8617 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/orm/relations/has_one_or_many.py
--rw-r--r--   0        0        0      899 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/orm/relations/morph_many.py
--rw-r--r--   0        0        0      843 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/orm/relations/morph_one.py
--rw-r--r--   0        0        0     5377 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/orm/relations/morph_one_or_many.py
--rw-r--r--   0        0        0      984 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/orm/relations/morph_pivot.py
--rw-r--r--   0        0        0     5293 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/orm/relations/morph_to.py
--rw-r--r--   0        0        0     3555 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/orm/relations/morph_to_many.py
--rw-r--r--   0        0        0     2978 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/orm/relations/pivot.py
--rw-r--r--   0        0        0     5956 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/orm/relations/relation.py
--rw-r--r--   0        0        0      685 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/orm/relations/result.py
--rw-r--r--   0        0        0     1106 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/orm/relations/wrapper.py
--rw-r--r--   0        0        0       95 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/orm/scopes/__init__.py
--rw-r--r--   0        0        0      348 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/orm/scopes/scope.py
--rw-r--r--   0        0        0     3900 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/orm/scopes/soft_deleting.py
--rw-r--r--   0        0        0    13604 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/orm/utils.py
--rw-r--r--   0        0        0      115 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/pagination/__init__.py
--rw-r--r--   0        0        0     2251 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/pagination/base.py
--rw-r--r--   0        0        0     2426 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/pagination/length_aware_paginator.py
--rw-r--r--   0        0        0     2216 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/pagination/paginator.py
--rw-r--r--   0        0        0       59 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/query/__init__.py
--rw-r--r--   0        0        0    43978 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/query/builder.py
--rw-r--r--   0        0        0      230 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/query/expression.py
--rw-r--r--   0        0        0      202 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/query/grammars/__init__.py
--rw-r--r--   0        0        0    13999 2023-07-21 20:39:52.706169 meliorator-0.9.22/orator/query/grammars/grammar.py
--rw-r--r--   0        0        0     3559 2023-07-21 20:39:52.710169 meliorator-0.9.22/orator/query/grammars/mysql_grammar.py
--rw-r--r--   0        0        0     4461 2023-07-21 20:39:52.710169 meliorator-0.9.22/orator/query/grammars/postgres_grammar.py
--rw-r--r--   0        0        0     4204 2023-07-21 20:39:52.710169 meliorator-0.9.22/orator/query/grammars/sqlite_grammar.py
--rw-r--r--   0        0        0     1407 2023-07-21 20:39:52.710169 meliorator-0.9.22/orator/query/join_clause.py
--rw-r--r--   0        0        0      218 2023-07-21 20:39:52.710169 meliorator-0.9.22/orator/query/processors/__init__.py
--rw-r--r--   0        0        0     1790 2023-07-21 20:39:52.710169 meliorator-0.9.22/orator/query/processors/mysql_processor.py
--rw-r--r--   0        0        0     1160 2023-07-21 20:39:52.710169 meliorator-0.9.22/orator/query/processors/postgres_processor.py
--rw-r--r--   0        0        0     1423 2023-07-21 20:39:52.710169 meliorator-0.9.22/orator/query/processors/processor.py
--rw-r--r--   0        0        0      422 2023-07-21 20:39:52.710169 meliorator-0.9.22/orator/query/processors/sqlite_processor.py
--rw-r--r--   0        0        0      166 2023-07-21 20:39:52.710169 meliorator-0.9.22/orator/schema/__init__.py
--rw-r--r--   0        0        0    19840 2023-07-21 20:39:52.710169 meliorator-0.9.22/orator/schema/blueprint.py
--rw-r--r--   0        0        0     3617 2023-07-21 20:39:52.710169 meliorator-0.9.22/orator/schema/builder.py
--rw-r--r--   0        0        0      206 2023-07-21 20:39:52.710169 meliorator-0.9.22/orator/schema/grammars/__init__.py
--rw-r--r--   0        0        0     9880 2023-07-21 20:39:52.710169 meliorator-0.9.22/orator/schema/grammars/grammar.py
--rw-r--r--   0        0        0     8503 2023-07-21 20:39:52.710169 meliorator-0.9.22/orator/schema/grammars/mysql_grammar.py
--rw-r--r--   0        0        0     7304 2023-07-21 20:39:52.710169 meliorator-0.9.22/orator/schema/grammars/postgres_grammar.py
--rw-r--r--   0        0        0     8321 2023-07-21 20:39:52.710169 meliorator-0.9.22/orator/schema/grammars/sqlite_grammar.py
--rw-r--r--   0        0        0     1229 2023-07-21 20:39:52.710169 meliorator-0.9.22/orator/schema/mysql_builder.py
--rw-r--r--   0        0        0      645 2023-07-21 20:39:52.710169 meliorator-0.9.22/orator/schema/schema.py
--rw-r--r--   0        0        0       52 2023-07-21 20:39:52.710169 meliorator-0.9.22/orator/seeds/__init__.py
--rw-r--r--   0        0        0     1730 2023-07-21 20:39:52.710169 meliorator-0.9.22/orator/seeds/seeder.py
--rw-r--r--   0        0        0      203 2023-07-21 20:39:52.710169 meliorator-0.9.22/orator/seeds/stubs.py
--rw-r--r--   0        0        0       60 2023-07-21 20:39:52.710169 meliorator-0.9.22/orator/support/__init__.py
--rw-r--r--   0        0        0      121 2023-07-21 20:39:52.710169 meliorator-0.9.22/orator/support/collection.py
--rw-r--r--   0        0        0     2193 2023-07-21 20:39:52.710169 meliorator-0.9.22/orator/support/fluent.py
--rw-r--r--   0        0        0     2614 2023-07-21 20:39:52.710169 meliorator-0.9.22/orator/support/grammar.py
--rw-r--r--   0        0        0     2833 2023-07-21 20:39:52.710169 meliorator-0.9.22/orator/utils/__init__.py
--rw-r--r--   0        0        0     4398 2023-07-21 20:39:52.710169 meliorator-0.9.22/orator/utils/command_formatter.py
--rw-r--r--   0        0        0      749 2023-07-21 20:39:52.710169 meliorator-0.9.22/orator/utils/helpers.py
--rw-r--r--   0        0        0      714 2023-07-21 20:39:52.710169 meliorator-0.9.22/orator/utils/qmarker.py
--rw-r--r--   0        0        0     7566 2023-07-21 20:39:52.710169 meliorator-0.9.22/orator/utils/url.py
--rw-r--r--   0        0        0     1283 2023-07-21 20:39:52.710169 meliorator-0.9.22/pyproject.toml
--rw-r--r--   0        0        0    22163 1970-01-01 00:00:00.000000 meliorator-0.9.22/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-08-01 18:40:04.098684 meliorator-0.9.23/LICENSE
+-rw-r--r--   0        0        0    20599 2023-08-01 18:40:04.098684 meliorator-0.9.23/README.rst
+-rw-r--r--   0        0        0      298 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/__init__.py
+-rw-r--r--   0        0        0       24 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/commands/__init__.py
+-rw-r--r--   0        0        0      785 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/commands/application.py
+-rw-r--r--   0        0        0     3453 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/commands/command.py
+-rw-r--r--   0        0        0      330 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/commands/migrations/__init__.py
+-rw-r--r--   0        0        0      186 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/commands/migrations/base_command.py
+-rw-r--r--   0        0        0      626 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/commands/migrations/install_command.py
+-rw-r--r--   0        0        0     1301 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/commands/migrations/make_command.py
+-rw-r--r--   0        0        0     2343 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/commands/migrations/migrate_command.py
+-rw-r--r--   0        0        0     1886 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/commands/migrations/refresh_command.py
+-rw-r--r--   0        0        0     1308 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/commands/migrations/reset_command.py
+-rw-r--r--   0        0        0     1315 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/commands/migrations/rollback_command.py
+-rw-r--r--   0        0        0     1642 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/commands/migrations/status_command.py
+-rw-r--r--   0        0        0       68 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/commands/models/__init__.py
+-rw-r--r--   0        0        0     2217 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/commands/models/make_command.py
+-rw-r--r--   0        0        0      115 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/commands/models/stubs.py
+-rw-r--r--   0        0        0      108 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/commands/seeds/__init__.py
+-rw-r--r--   0        0        0      178 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/commands/seeds/base_command.py
+-rw-r--r--   0        0        0     2204 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/commands/seeds/make_command.py
+-rw-r--r--   0        0        0     1923 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/commands/seeds/seed_command.py
+-rw-r--r--   0        0        0      206 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/connections/__init__.py
+-rw-r--r--   0        0        0    15578 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/connections/connection.py
+-rw-r--r--   0        0        0     4112 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/connections/connection_interface.py
+-rw-r--r--   0        0        0      298 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/connections/connection_resolver_interface.py
+-rw-r--r--   0        0        0     2218 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/connections/mysql_connection.py
+-rw-r--r--   0        0        0     2095 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/connections/postgres_connection.py
+-rw-r--r--   0        0        0     1588 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/connections/sqlite_connection.py
+-rw-r--r--   0        0        0      198 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/connectors/__init__.py
+-rw-r--r--   0        0        0     3133 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/connectors/connection_factory.py
+-rw-r--r--   0        0        0     3106 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/connectors/connector.py
+-rw-r--r--   0        0        0     3886 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/connectors/mysql_connector.py
+-rw-r--r--   0        0        0     3280 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/connectors/postgres_connector.py
+-rw-r--r--   0        0        0     2065 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/connectors/sqlite_connector.py
+-rw-r--r--   0        0        0     5089 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/database_manager.py
+-rw-r--r--   0        0        0       24 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/dbal/__init__.py
+-rw-r--r--   0        0        0     2372 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/dbal/abstract_asset.py
+-rw-r--r--   0        0        0     3447 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/dbal/column.py
+-rw-r--r--   0        0        0      545 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/dbal/column_diff.py
+-rw-r--r--   0        0        0    11219 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/dbal/comparator.py
+-rw-r--r--   0        0        0     1943 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/dbal/exceptions/__init__.py
+-rw-r--r--   0        0        0     8193 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/dbal/foreign_key_constraint.py
+-rw-r--r--   0        0        0      173 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/dbal/identifier.py
+-rw-r--r--   0        0        0     7094 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/dbal/index.py
+-rw-r--r--   0        0        0     5260 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/dbal/mysql_schema_manager.py
+-rw-r--r--   0        0        0      205 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/dbal/platforms/__init__.py
+-rw-r--r--   0        0        0       24 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/dbal/platforms/keywords/__init__.py
+-rw-r--r--   0        0        0      209 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/dbal/platforms/keywords/keyword_list.py
+-rw-r--r--   0        0        0     4383 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/dbal/platforms/keywords/mysql_keywords.py
+-rw-r--r--   0        0        0     1730 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/dbal/platforms/keywords/postgresql_keywords.py
+-rw-r--r--   0        0        0     2315 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/dbal/platforms/keywords/sqlite_keywords.py
+-rw-r--r--   0        0        0     1254 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/dbal/platforms/mysql57_platform.py
+-rw-r--r--   0        0        0     9489 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/dbal/platforms/mysql_platform.py
+-rw-r--r--   0        0        0    21672 2023-08-01 18:40:04.098684 meliorator-0.9.23/orator/dbal/platforms/platform.py
+-rw-r--r--   0        0        0    14126 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/dbal/platforms/postgres_platform.py
+-rw-r--r--   0        0        0    20833 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/dbal/platforms/sqlite_platform.py
+-rw-r--r--   0        0        0     6014 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/dbal/postgres_schema_manager.py
+-rw-r--r--   0        0        0     4240 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/dbal/schema_manager.py
+-rw-r--r--   0        0        0     5458 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/dbal/sqlite_schema_manager.py
+-rw-r--r--   0        0        0    17146 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/dbal/table.py
+-rw-r--r--   0        0        0     1436 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/dbal/table_diff.py
+-rw-r--r--   0        0        0       24 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/dbal/types/__init__.py
+-rw-r--r--   0        0        0      992 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/events/__init__.py
+-rw-r--r--   0        0        0       68 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/exceptions/__init__.py
+-rw-r--r--   0        0        0      193 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/exceptions/connection.py
+-rw-r--r--   0        0        0      822 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/exceptions/connectors.py
+-rw-r--r--   0        0        0      551 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/exceptions/orm.py
+-rw-r--r--   0        0        0      494 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/exceptions/query.py
+-rw-r--r--   0        0        0      208 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/migrations/__init__.py
+-rw-r--r--   0        0        0     2730 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/migrations/database_migration_repository.py
+-rw-r--r--   0        0        0      425 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/migrations/migration.py
+-rw-r--r--   0        0        0     2588 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/migrations/migration_creator.py
+-rw-r--r--   0        0        0     7754 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/migrations/migrator.py
+-rw-r--r--   0        0        0     1114 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/migrations/stubs.py
+-rw-r--r--   0        0        0      419 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/orm/__init__.py
+-rw-r--r--   0        0        0    32311 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/orm/builder.py
+-rw-r--r--   0        0        0      814 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/orm/collection.py
+-rw-r--r--   0        0        0     7481 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/orm/factory.py
+-rw-r--r--   0        0        0     2579 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/orm/factory_builder.py
+-rw-r--r--   0        0        0       63 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/orm/mixins/__init__.py
+-rw-r--r--   0        0        0     3532 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/orm/mixins/soft_deletes.py
+-rw-r--r--   0        0        0    75367 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/orm/model.py
+-rw-r--r--   0        0        0      371 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/orm/relations/__init__.py
+-rw-r--r--   0        0        0     5427 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/orm/relations/belongs_to.py
+-rw-r--r--   0        0        0    23246 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/orm/relations/belongs_to_many.py
+-rw-r--r--   0        0        0     1012 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/orm/relations/has_many.py
+-rw-r--r--   0        0        0     5126 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/orm/relations/has_many_through.py
+-rw-r--r--   0        0        0      955 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/orm/relations/has_one.py
+-rw-r--r--   0        0        0     8617 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/orm/relations/has_one_or_many.py
+-rw-r--r--   0        0        0      899 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/orm/relations/morph_many.py
+-rw-r--r--   0        0        0      843 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/orm/relations/morph_one.py
+-rw-r--r--   0        0        0     5377 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/orm/relations/morph_one_or_many.py
+-rw-r--r--   0        0        0      984 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/orm/relations/morph_pivot.py
+-rw-r--r--   0        0        0     5293 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/orm/relations/morph_to.py
+-rw-r--r--   0        0        0     3555 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/orm/relations/morph_to_many.py
+-rw-r--r--   0        0        0     2978 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/orm/relations/pivot.py
+-rw-r--r--   0        0        0     5956 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/orm/relations/relation.py
+-rw-r--r--   0        0        0      685 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/orm/relations/result.py
+-rw-r--r--   0        0        0     1106 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/orm/relations/wrapper.py
+-rw-r--r--   0        0        0       95 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/orm/scopes/__init__.py
+-rw-r--r--   0        0        0      348 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/orm/scopes/scope.py
+-rw-r--r--   0        0        0     3900 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/orm/scopes/soft_deleting.py
+-rw-r--r--   0        0        0    13604 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/orm/utils.py
+-rw-r--r--   0        0        0      115 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/pagination/__init__.py
+-rw-r--r--   0        0        0     2251 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/pagination/base.py
+-rw-r--r--   0        0        0     2426 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/pagination/length_aware_paginator.py
+-rw-r--r--   0        0        0     2216 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/pagination/paginator.py
+-rw-r--r--   0        0        0       59 2023-08-01 18:40:04.102684 meliorator-0.9.23/orator/query/__init__.py
+-rw-r--r--   0        0        0    43978 2023-08-01 18:40:04.106684 meliorator-0.9.23/orator/query/builder.py
+-rw-r--r--   0        0        0      230 2023-08-01 18:40:04.106684 meliorator-0.9.23/orator/query/expression.py
+-rw-r--r--   0        0        0      202 2023-08-01 18:40:04.106684 meliorator-0.9.23/orator/query/grammars/__init__.py
+-rw-r--r--   0        0        0    13999 2023-08-01 18:40:04.106684 meliorator-0.9.23/orator/query/grammars/grammar.py
+-rw-r--r--   0        0        0     3559 2023-08-01 18:40:04.106684 meliorator-0.9.23/orator/query/grammars/mysql_grammar.py
+-rw-r--r--   0        0        0     4461 2023-08-01 18:40:04.106684 meliorator-0.9.23/orator/query/grammars/postgres_grammar.py
+-rw-r--r--   0        0        0     4204 2023-08-01 18:40:04.106684 meliorator-0.9.23/orator/query/grammars/sqlite_grammar.py
+-rw-r--r--   0        0        0     1407 2023-08-01 18:40:04.106684 meliorator-0.9.23/orator/query/join_clause.py
+-rw-r--r--   0        0        0      218 2023-08-01 18:40:04.106684 meliorator-0.9.23/orator/query/processors/__init__.py
+-rw-r--r--   0        0        0     1790 2023-08-01 18:40:04.106684 meliorator-0.9.23/orator/query/processors/mysql_processor.py
+-rw-r--r--   0        0        0     1160 2023-08-01 18:40:04.106684 meliorator-0.9.23/orator/query/processors/postgres_processor.py
+-rw-r--r--   0        0        0     1423 2023-08-01 18:40:04.106684 meliorator-0.9.23/orator/query/processors/processor.py
+-rw-r--r--   0        0        0      422 2023-08-01 18:40:04.106684 meliorator-0.9.23/orator/query/processors/sqlite_processor.py
+-rw-r--r--   0        0        0      166 2023-08-01 18:40:04.106684 meliorator-0.9.23/orator/schema/__init__.py
+-rw-r--r--   0        0        0    19840 2023-08-01 18:40:04.106684 meliorator-0.9.23/orator/schema/blueprint.py
+-rw-r--r--   0        0        0     3617 2023-08-01 18:40:04.106684 meliorator-0.9.23/orator/schema/builder.py
+-rw-r--r--   0        0        0      206 2023-08-01 18:40:04.106684 meliorator-0.9.23/orator/schema/grammars/__init__.py
+-rw-r--r--   0        0        0     9880 2023-08-01 18:40:04.106684 meliorator-0.9.23/orator/schema/grammars/grammar.py
+-rw-r--r--   0        0        0     8503 2023-08-01 18:40:04.106684 meliorator-0.9.23/orator/schema/grammars/mysql_grammar.py
+-rw-r--r--   0        0        0     7304 2023-08-01 18:40:04.106684 meliorator-0.9.23/orator/schema/grammars/postgres_grammar.py
+-rw-r--r--   0        0        0     8321 2023-08-01 18:40:04.106684 meliorator-0.9.23/orator/schema/grammars/sqlite_grammar.py
+-rw-r--r--   0        0        0     1229 2023-08-01 18:40:04.106684 meliorator-0.9.23/orator/schema/mysql_builder.py
+-rw-r--r--   0        0        0      645 2023-08-01 18:40:04.106684 meliorator-0.9.23/orator/schema/schema.py
+-rw-r--r--   0        0        0       52 2023-08-01 18:40:04.106684 meliorator-0.9.23/orator/seeds/__init__.py
+-rw-r--r--   0        0        0     1730 2023-08-01 18:40:04.106684 meliorator-0.9.23/orator/seeds/seeder.py
+-rw-r--r--   0        0        0      203 2023-08-01 18:40:04.106684 meliorator-0.9.23/orator/seeds/stubs.py
+-rw-r--r--   0        0        0       60 2023-08-01 18:40:04.106684 meliorator-0.9.23/orator/support/__init__.py
+-rw-r--r--   0        0        0      121 2023-08-01 18:40:04.106684 meliorator-0.9.23/orator/support/collection.py
+-rw-r--r--   0        0        0     2193 2023-08-01 18:40:04.106684 meliorator-0.9.23/orator/support/fluent.py
+-rw-r--r--   0        0        0     2614 2023-08-01 18:40:04.106684 meliorator-0.9.23/orator/support/grammar.py
+-rw-r--r--   0        0        0     2833 2023-08-01 18:40:04.106684 meliorator-0.9.23/orator/utils/__init__.py
+-rw-r--r--   0        0        0     4398 2023-08-01 18:40:04.106684 meliorator-0.9.23/orator/utils/command_formatter.py
+-rw-r--r--   0        0        0      749 2023-08-01 18:40:04.106684 meliorator-0.9.23/orator/utils/helpers.py
+-rw-r--r--   0        0        0      714 2023-08-01 18:40:04.106684 meliorator-0.9.23/orator/utils/qmarker.py
+-rw-r--r--   0        0        0     7566 2023-08-01 18:40:04.106684 meliorator-0.9.23/orator/utils/url.py
+-rw-r--r--   0        0        0     1283 2023-08-01 18:40:04.106684 meliorator-0.9.23/pyproject.toml
+-rw-r--r--   0        0        0    22163 1970-01-01 00:00:00.000000 meliorator-0.9.23/PKG-INFO
```

### Comparing `meliorator-0.9.22/LICENSE` & `meliorator-0.9.23/LICENSE`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/README.rst` & `meliorator-0.9.23/README.rst`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/commands/application.py` & `meliorator-0.9.23/orator/commands/application.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/commands/command.py` & `meliorator-0.9.23/orator/commands/command.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/commands/migrations/install_command.py` & `meliorator-0.9.23/orator/commands/migrations/install_command.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/commands/migrations/make_command.py` & `meliorator-0.9.23/orator/commands/migrations/make_command.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/commands/migrations/migrate_command.py` & `meliorator-0.9.23/orator/commands/migrations/migrate_command.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/commands/migrations/refresh_command.py` & `meliorator-0.9.23/orator/commands/migrations/refresh_command.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/commands/migrations/reset_command.py` & `meliorator-0.9.23/orator/commands/migrations/reset_command.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/commands/migrations/rollback_command.py` & `meliorator-0.9.23/orator/commands/migrations/rollback_command.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/commands/migrations/status_command.py` & `meliorator-0.9.23/orator/commands/migrations/status_command.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/commands/models/make_command.py` & `meliorator-0.9.23/orator/commands/models/make_command.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/commands/seeds/make_command.py` & `meliorator-0.9.23/orator/commands/seeds/make_command.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/commands/seeds/seed_command.py` & `meliorator-0.9.23/orator/commands/seeds/seed_command.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/connections/connection.py` & `meliorator-0.9.23/orator/connections/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
         start = time.time()
         try:
 
             result = wrapped(self, query, bindings, *args, **kwargs)
         except Exception as e:
             result = self._try_again_if_caused_by_lost_connection(
-                e, query, bindings, wrapped
+                e, query, bindings, wrapped, *args, **kwargs
             )
 
         t = self._get_elapsed_time(start)
         self.log_query(query, bindings, t)
 
         return result
 
@@ -222,19 +222,15 @@
             bindings = self.prepare_bindings(bindings)
             cursor = self._get_cursor_for_select(use_read_connection)
 
             try:
                 cursor.execute(query, bindings)
             except Exception as e:
                 if self._caused_by_lost_connection(e) and not abort:
-                    _transaction_aux = self._transactions
-                    _connection_autocommit = self._connection.autocommit
                     self.reconnect()
-                    self._transactions = _transaction_aux
-                    self._connection.autocommit = _connection_autocommit
 
                     for results in self.select_many(
                         size, query, bindings, use_read_connection, True
                     ):
                         yield results
                 else:
                     raise
@@ -358,14 +354,15 @@
     ):
         if self._caused_by_lost_connection(e):
             _transaction_aux = self._transactions
             _connection_autocommit = self._connection.autocommit
             self.reconnect()
             self._transactions = _transaction_aux
             self._connection.autocommit = _connection_autocommit
+
             return callback(self, query, bindings, *args, **kwargs)
 
         raise QueryException(query, bindings, e)
 
     def _caused_by_lost_connection(self, e):
         message = str(e).lower()
 
@@ -408,15 +405,14 @@
         if self._reconnector is not None and callable(self._reconnector):
             return self._reconnector(self)
 
         raise Exception("Lost connection and no reconnector available")
 
     def _reconnect_if_missing_connection(self):
         if self.get_connection() is None or self.get_read_connection() is None:
-            self._lost_connection = True
             self.reconnect()
 
     def log_query(self, query, bindings, time_=None):
         if self.pretending():
             self._logged_queries.append(self._get_cursor_query(query, bindings))
 
         if not self._logging_queries:
```

### Comparing `meliorator-0.9.22/orator/connections/connection_interface.py` & `meliorator-0.9.23/orator/connections/connection_interface.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/connections/mysql_connection.py` & `meliorator-0.9.23/orator/connections/mysql_connection.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/connections/postgres_connection.py` & `meliorator-0.9.23/orator/connections/postgres_connection.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,27 +33,16 @@
         bindings = self.prepare_bindings(bindings)
 
         self._new_cursor().execute(query, bindings)
 
         return True
 
     def begin_transaction(self):
-        self._reconnect_if_missing_connection()
-
-        try:
-            if not self._transactions:
-                self._connection.autocommit = False
-        except Exception as e:
-            if self._caused_by_lost_connection(e):
-                _transaction_aux = self._transactions
-                self.reconnect()
-                self._transactions = _transaction_aux
-                self._connection.autocommit = False
-            else:
-                raise
+        if not self._transactions:
+            self._connection.autocommit = False
 
         super(PostgresConnection, self).begin_transaction()
 
     def commit(self):
         if self._transactions == 1:
             self._connection.commit()
             self._connection.autocommit = True
```

### Comparing `meliorator-0.9.22/orator/connections/sqlite_connection.py` & `meliorator-0.9.23/orator/connections/sqlite_connection.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/connectors/connection_factory.py` & `meliorator-0.9.23/orator/connectors/connection_factory.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/connectors/connector.py` & `meliorator-0.9.23/orator/connectors/connector.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/connectors/mysql_connector.py` & `meliorator-0.9.23/orator/connectors/mysql_connector.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/connectors/postgres_connector.py` & `meliorator-0.9.23/orator/connectors/postgres_connector.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/connectors/sqlite_connector.py` & `meliorator-0.9.23/orator/connectors/sqlite_connector.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/database_manager.py` & `meliorator-0.9.23/orator/database_manager.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/dbal/abstract_asset.py` & `meliorator-0.9.23/orator/dbal/abstract_asset.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/dbal/column.py` & `meliorator-0.9.23/orator/dbal/column.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/dbal/column_diff.py` & `meliorator-0.9.23/orator/dbal/column_diff.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/dbal/comparator.py` & `meliorator-0.9.23/orator/dbal/comparator.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/dbal/exceptions/__init__.py` & `meliorator-0.9.23/orator/dbal/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/dbal/foreign_key_constraint.py` & `meliorator-0.9.23/orator/dbal/foreign_key_constraint.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/dbal/index.py` & `meliorator-0.9.23/orator/dbal/index.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/dbal/mysql_schema_manager.py` & `meliorator-0.9.23/orator/dbal/mysql_schema_manager.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/dbal/platforms/keywords/mysql_keywords.py` & `meliorator-0.9.23/orator/dbal/platforms/keywords/mysql_keywords.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/dbal/platforms/keywords/postgresql_keywords.py` & `meliorator-0.9.23/orator/dbal/platforms/keywords/postgresql_keywords.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/dbal/platforms/keywords/sqlite_keywords.py` & `meliorator-0.9.23/orator/dbal/platforms/keywords/sqlite_keywords.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/dbal/platforms/mysql57_platform.py` & `meliorator-0.9.23/orator/dbal/platforms/mysql57_platform.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/dbal/platforms/mysql_platform.py` & `meliorator-0.9.23/orator/dbal/platforms/mysql_platform.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/dbal/platforms/platform.py` & `meliorator-0.9.23/orator/dbal/platforms/platform.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/dbal/platforms/postgres_platform.py` & `meliorator-0.9.23/orator/dbal/platforms/postgres_platform.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/dbal/platforms/sqlite_platform.py` & `meliorator-0.9.23/orator/dbal/platforms/sqlite_platform.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/dbal/postgres_schema_manager.py` & `meliorator-0.9.23/orator/dbal/postgres_schema_manager.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/dbal/schema_manager.py` & `meliorator-0.9.23/orator/dbal/schema_manager.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/dbal/sqlite_schema_manager.py` & `meliorator-0.9.23/orator/dbal/sqlite_schema_manager.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/dbal/table.py` & `meliorator-0.9.23/orator/dbal/table.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/dbal/table_diff.py` & `meliorator-0.9.23/orator/dbal/table_diff.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/events/__init__.py` & `meliorator-0.9.23/orator/events/__init__.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/exceptions/connectors.py` & `meliorator-0.9.23/orator/exceptions/connectors.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/exceptions/orm.py` & `meliorator-0.9.23/orator/exceptions/orm.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/migrations/database_migration_repository.py` & `meliorator-0.9.23/orator/migrations/database_migration_repository.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/migrations/migration_creator.py` & `meliorator-0.9.23/orator/migrations/migration_creator.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/migrations/migrator.py` & `meliorator-0.9.23/orator/migrations/migrator.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/migrations/stubs.py` & `meliorator-0.9.23/orator/migrations/stubs.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/orm/builder.py` & `meliorator-0.9.23/orator/orm/builder.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/orm/collection.py` & `meliorator-0.9.23/orator/orm/collection.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/orm/factory.py` & `meliorator-0.9.23/orator/orm/factory.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/orm/factory_builder.py` & `meliorator-0.9.23/orator/orm/factory_builder.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/orm/mixins/soft_deletes.py` & `meliorator-0.9.23/orator/orm/mixins/soft_deletes.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/orm/model.py` & `meliorator-0.9.23/orator/orm/model.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/orm/relations/belongs_to.py` & `meliorator-0.9.23/orator/orm/relations/belongs_to.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/orm/relations/belongs_to_many.py` & `meliorator-0.9.23/orator/orm/relations/belongs_to_many.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/orm/relations/has_many.py` & `meliorator-0.9.23/orator/orm/relations/has_many.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/orm/relations/has_many_through.py` & `meliorator-0.9.23/orator/orm/relations/has_many_through.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/orm/relations/has_one.py` & `meliorator-0.9.23/orator/orm/relations/has_one.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/orm/relations/has_one_or_many.py` & `meliorator-0.9.23/orator/orm/relations/has_one_or_many.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/orm/relations/morph_many.py` & `meliorator-0.9.23/orator/orm/relations/morph_many.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/orm/relations/morph_one.py` & `meliorator-0.9.23/orator/orm/relations/morph_one.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/orm/relations/morph_one_or_many.py` & `meliorator-0.9.23/orator/orm/relations/morph_one_or_many.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/orm/relations/morph_pivot.py` & `meliorator-0.9.23/orator/orm/relations/morph_pivot.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/orm/relations/morph_to.py` & `meliorator-0.9.23/orator/orm/relations/morph_to.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/orm/relations/morph_to_many.py` & `meliorator-0.9.23/orator/orm/relations/morph_to_many.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/orm/relations/pivot.py` & `meliorator-0.9.23/orator/orm/relations/pivot.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/orm/relations/relation.py` & `meliorator-0.9.23/orator/orm/relations/relation.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/orm/relations/result.py` & `meliorator-0.9.23/orator/orm/relations/result.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/orm/relations/wrapper.py` & `meliorator-0.9.23/orator/orm/relations/wrapper.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/orm/scopes/soft_deleting.py` & `meliorator-0.9.23/orator/orm/scopes/soft_deleting.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/orm/utils.py` & `meliorator-0.9.23/orator/orm/utils.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/pagination/base.py` & `meliorator-0.9.23/orator/pagination/base.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/pagination/length_aware_paginator.py` & `meliorator-0.9.23/orator/pagination/length_aware_paginator.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/pagination/paginator.py` & `meliorator-0.9.23/orator/pagination/paginator.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/query/builder.py` & `meliorator-0.9.23/orator/query/builder.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/query/grammars/grammar.py` & `meliorator-0.9.23/orator/query/grammars/grammar.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/query/grammars/mysql_grammar.py` & `meliorator-0.9.23/orator/query/grammars/mysql_grammar.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/query/grammars/postgres_grammar.py` & `meliorator-0.9.23/orator/query/grammars/postgres_grammar.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/query/grammars/sqlite_grammar.py` & `meliorator-0.9.23/orator/query/grammars/sqlite_grammar.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/query/join_clause.py` & `meliorator-0.9.23/orator/query/join_clause.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/query/processors/mysql_processor.py` & `meliorator-0.9.23/orator/query/processors/mysql_processor.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/query/processors/postgres_processor.py` & `meliorator-0.9.23/orator/query/processors/postgres_processor.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/query/processors/processor.py` & `meliorator-0.9.23/orator/query/processors/processor.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/schema/blueprint.py` & `meliorator-0.9.23/orator/schema/blueprint.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/schema/builder.py` & `meliorator-0.9.23/orator/schema/builder.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/schema/grammars/grammar.py` & `meliorator-0.9.23/orator/schema/grammars/grammar.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/schema/grammars/mysql_grammar.py` & `meliorator-0.9.23/orator/schema/grammars/mysql_grammar.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/schema/grammars/postgres_grammar.py` & `meliorator-0.9.23/orator/schema/grammars/postgres_grammar.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/schema/grammars/sqlite_grammar.py` & `meliorator-0.9.23/orator/schema/grammars/sqlite_grammar.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/schema/mysql_builder.py` & `meliorator-0.9.23/orator/schema/mysql_builder.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/schema/schema.py` & `meliorator-0.9.23/orator/schema/schema.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/seeds/seeder.py` & `meliorator-0.9.23/orator/seeds/seeder.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/support/fluent.py` & `meliorator-0.9.23/orator/support/fluent.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/support/grammar.py` & `meliorator-0.9.23/orator/support/grammar.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/utils/__init__.py` & `meliorator-0.9.23/orator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/utils/command_formatter.py` & `meliorator-0.9.23/orator/utils/command_formatter.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/utils/helpers.py` & `meliorator-0.9.23/orator/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/utils/qmarker.py` & `meliorator-0.9.23/orator/utils/qmarker.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/orator/utils/url.py` & `meliorator-0.9.23/orator/utils/url.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.22/pyproject.toml` & `meliorator-0.9.23/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meliorator"
-version = "0.9.22"
+version = "0.9.23"
 description = "This is a fork from Orator ORM used by Méliuz."
 
 license = "MIT"
 
 authors = [
     "Sébastien Eustace <sebastien@eustace.io>"
 ]
```

### Comparing `meliorator-0.9.22/PKG-INFO` & `meliorator-0.9.23/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meliorator
-Version: 0.9.22
+Version: 0.9.23
 Summary: This is a fork from Orator ORM used by Méliuz.
 Home-page: https://orator-orm.com/
 License: MIT
 Keywords: database,orm
 Author: Sébastien Eustace
 Author-email: sebastien@eustace.io
 Maintainer: Matheus Oliveira
```

