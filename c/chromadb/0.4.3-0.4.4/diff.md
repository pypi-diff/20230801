# Comparing `tmp/chromadb-0.4.3.tar.gz` & `tmp/chromadb-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromadb-0.4.3.tar", last modified: Tue Jul 25 05:11:15 2023, max compression
+gzip compressed data, was "chromadb-0.4.4.tar", last modified: Tue Aug  1 01:20:52 2023, max compression
```

## Comparing `chromadb-0.4.3.tar` & `chromadb-0.4.4.tar`

### file list

```diff
@@ -1,237 +1,246 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.670656 chromadb-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-25 05:10:58.000000 chromadb-0.4.3/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.610655 chromadb-0.4.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.622655 chromadb-0.4.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-25 05:10:58.000000 chromadb-0.4.3/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-25 05:10:58.000000 chromadb-0.4.3/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-25 05:10:58.000000 chromadb-0.4.3/.github/ISSUE_TEMPLATE/installation_trouble.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.622655 chromadb-0.4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-25 05:10:58.000000 chromadb-0.4.3/.github/workflows/chroma-client-integration-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-25 05:10:58.000000 chromadb-0.4.3/.github/workflows/chroma-integration-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-25 05:10:58.000000 chromadb-0.4.3/.github/workflows/chroma-release-python-client.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-25 05:10:58.000000 chromadb-0.4.3/.github/workflows/chroma-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-25 05:10:58.000000 chromadb-0.4.3/.github/workflows/chroma-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-25 05:10:58.000000 chromadb-0.4.3/.github/workflows/pr-review-checklist.yml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-25 05:10:58.000000 chromadb-0.4.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-25 05:10:58.000000 chromadb-0.4.3/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.622655 chromadb-0.4.3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-25 05:10:58.000000 chromadb-0.4.3/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-25 05:10:58.000000 chromadb-0.4.3/DEVELOP.md
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-25 05:10:58.000000 chromadb-0.4.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 05:10:58.000000 chromadb-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-07-25 05:11:15.670656 chromadb-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-25 05:10:58.000000 chromadb-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-25 05:10:58.000000 chromadb-0.4.3/RELEASE_PROCESS.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.626655 chromadb-0.4.3/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      110 2023-07-25 05:10:58.000000 chromadb-0.4.3/bin/build
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-07-25 05:10:58.000000 chromadb-0.4.3/bin/docker_entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-07-25 05:10:58.000000 chromadb-0.4.3/bin/generate_cloudformation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      487 2023-07-25 05:10:58.000000 chromadb-0.4.3/bin/integration-test
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.626655 chromadb-0.4.3/bin/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-25 05:10:58.000000 chromadb-0.4.3/bin/templates/docker-compose.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      451 2023-07-25 05:10:58.000000 chromadb-0.4.3/bin/test-package.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      321 2023-07-25 05:10:58.000000 chromadb-0.4.3/bin/test-remote
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-25 05:10:58.000000 chromadb-0.4.3/bin/test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      151 2023-07-25 05:10:58.000000 chromadb-0.4.3/bin/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.626655 chromadb-0.4.3/chromadb/
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.630655 chromadb-0.4.3/chromadb/api/
--rw-r--r--   0 runner    (1001) docker     (123)    13188 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/api/fastapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.630655 chromadb-0.4.3/chromadb/api/models/
--rw-r--r--   0 runner    (1001) docker     (123)    15200 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/api/models/Collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    22439 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/api/segment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12405 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/api/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.630655 chromadb-0.4.3/chromadb/db/
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/db/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.630655 chromadb-0.4.3/chromadb/db/impl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/db/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7727 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/db/impl/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/db/impl/sqlite_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/db/migrations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.630655 chromadb-0.4.3/chromadb/db/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/db/mixins/embeddings_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    16398 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/db/mixins/sysdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/db/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.630655 chromadb-0.4.3/chromadb/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)   368824 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/experimental/density_relevance.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.630655 chromadb-0.4.3/chromadb/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/ingest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.634655 chromadb-0.4.3/chromadb/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.634655 chromadb-0.4.3/chromadb/migrations/embeddings_queue/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/migrations/embeddings_queue/00001-embeddings.sqlite.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.634655 chromadb-0.4.3/chromadb/migrations/metadb/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/migrations/metadb/00001-embedding-metadata.sqlite.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.634655 chromadb-0.4.3/chromadb/migrations/sysdb/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/migrations/sysdb/00001-collections.sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/migrations/sysdb/00002-segments.sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/migrations/sysdb/00003-collection-dimension.sqlite.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.634655 chromadb-0.4.3/chromadb/segment/
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/segment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.614655 chromadb-0.4.3/chromadb/segment/impl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.634655 chromadb-0.4.3/chromadb/segment/impl/manager/
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/segment/impl/manager/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.634655 chromadb-0.4.3/chromadb/segment/impl/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    19069 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/segment/impl/metadata/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.634655 chromadb-0.4.3/chromadb/segment/impl/vector/
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/segment/impl/vector/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/segment/impl/vector/brute_force_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/segment/impl/vector/hnsw_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    10716 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/segment/impl/vector/local_hnsw.py
--rw-r--r--   0 runner    (1001) docker     (123)    15667 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/segment/impl/vector/local_persistent_hnsw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.634655 chromadb-0.4.3/chromadb/server/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.634655 chromadb-0.4.3/chromadb/server/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/server/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/server/fastapi/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.638655 chromadb-0.4.3/chromadb/telemetry/
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/telemetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/telemetry/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/telemetry/posthog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.638655 chromadb-0.4.3/chromadb/test/
--rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.638655 chromadb-0.4.3/chromadb/test/db/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.642655 chromadb-0.4.3/chromadb/test/db/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/db/migrations/00001-migration-1.psql.sql
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/db/migrations/00001-migration-1.sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/db/migrations/00002-migration-2.psql.sql
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/db/migrations/00002-migration-2.sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/db/migrations/00003-migration-3.psql.sql
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/db/migrations/00003-migration-3.sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/db/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/db/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/db/test_migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10090 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/db/test_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.642655 chromadb-0.4.3/chromadb/test/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/ingest/test_producer_consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.642655 chromadb-0.4.3/chromadb/test/property/
--rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/property/invariants.py
--rw-r--r--   0 runner    (1001) docker     (123)    19519 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/property/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/property/test_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/property/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/property/test_cross_version_persist.py
--rw-r--r--   0 runner    (1001) docker     (123)    13367 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/property/test_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/property/test_filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/property/test_persist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.642655 chromadb-0.4.3/chromadb/test/segment/
--rw-r--r--   0 runner    (1001) docker     (123)    15572 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/segment/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    14604 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/segment/test_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)    41277 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/test_chroma.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/test_multithreaded.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.646655 chromadb-0.4.3/chromadb/test/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/test/utils/test_messagid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.646655 chromadb-0.4.3/chromadb/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/utils/distance_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16228 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/utils/embedding_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/utils/messageid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-25 05:10:58.000000 chromadb-0.4.3/chromadb/utils/read_write_lock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.626655 chromadb-0.4.3/chromadb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-07-25 05:11:15.000000 chromadb-0.4.3/chromadb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-07-25 05:11:15.000000 chromadb-0.4.3/chromadb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 05:11:15.000000 chromadb-0.4.3/chromadb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-25 05:11:15.000000 chromadb-0.4.3/chromadb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 05:11:15.000000 chromadb-0.4.3/chromadb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.618655 chromadb-0.4.3/clients/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.650655 chromadb-0.4.3/clients/js/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/.prettierrc.json
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/DEVELOP.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.618655 chromadb-0.4.3/clients/js/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.654655 chromadb-0.4.3/clients/js/examples/browser/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/examples/browser/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/examples/browser/app.ts
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/examples/browser/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/examples/browser/package.json
--rw-r--r--   0 runner    (1001) docker     (123)    68042 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/examples/browser/yarn.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.654655 chromadb-0.4.3/clients/js/examples/node/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/examples/node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/examples/node/app.js
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/examples/node/package.json
--rw-r--r--   0 runner    (1001) docker     (123)    17080 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/examples/node/yarn.lock
--rwxr-xr-x   0 runner    (1001) docker     (123)     1247 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/genapi.sh
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/jest.config.ts
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/openapitools.json
--rw-r--r--   0 runner    (1001) docker     (123)   448020 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.658656 chromadb-0.4.3/clients/js/src/
--rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/src/ChromaClient.ts
--rw-r--r--   0 runner    (1001) docker     (123)    19757 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/src/Collection.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.658656 chromadb-0.4.3/clients/js/src/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/src/embeddings/CohereEmbeddingFunction.ts
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/src/embeddings/IEmbeddingFunction.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/src/embeddings/TransformersEmbeddingFunction.ts
--rwxr-xr-x   0 runner    (1001) docker     (123)     3402 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/src/embeddings/WebAIEmbeddingFunction.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.662655 chromadb-0.4.3/clients/js/src/generated/
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/src/generated/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    54547 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/src/generated/api.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/src/generated/configuration.ts
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/src/generated/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/src/generated/models.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/src/generated/runtime.ts
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/src/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/src/types.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/src/utils.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.666655 chromadb-0.4.3/clients/js/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/test/add.collections.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/test/client.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/test/collection.client.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/test/collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/test/data.ts
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/test/delete.collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/test/get.collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/test/initClient.ts
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/test/peek.collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/test/query.collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/test/update.collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/test/upsert.collections.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/tsconfig.module.json
--rw-r--r--   0 runner    (1001) docker     (123)   156893 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/js/yarn.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.666655 chromadb-0.4.3/clients/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/python/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     1257 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/python/build_python_thin_client.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      850 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/python/integration-test.sh
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/python/is_thin_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-25 05:10:58.000000 chromadb-0.4.3/clients/python/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-25 05:10:58.000000 chromadb-0.4.3/docker-compose.server.example.yml
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-25 05:10:58.000000 chromadb-0.4.3/docker-compose.test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-25 05:10:58.000000 chromadb-0.4.3/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.666655 chromadb-0.4.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-25 05:10:58.000000 chromadb-0.4.3/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.666655 chromadb-0.4.3/examples/basic_functionality/
--rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-07-25 05:10:58.000000 chromadb-0.4.3/examples/basic_functionality/alternative_embeddings.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-07-25 05:10:58.000000 chromadb-0.4.3/examples/basic_functionality/local_persistence.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-25 05:10:58.000000 chromadb-0.4.3/examples/basic_functionality/where_filtering.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.618655 chromadb-0.4.3/examples/deployments/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.670656 chromadb-0.4.3/examples/deployments/google-cloud-compute/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-25 05:10:58.000000 chromadb-0.4.3/examples/deployments/google-cloud-compute/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-25 05:10:58.000000 chromadb-0.4.3/examples/deployments/google-cloud-compute/chroma.tf
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-25 05:10:58.000000 chromadb-0.4.3/examples/deployments/google-cloud-compute/main.tf
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-25 05:10:58.000000 chromadb-0.4.3/examples/deployments/google-cloud-compute/startup.sh
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-25 05:10:58.000000 chromadb-0.4.3/examples/deployments/google-cloud-compute/variables.tf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.618655 chromadb-0.4.3/examples/use_with/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:11:15.670656 chromadb-0.4.3/examples/use_with/cohere/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-25 05:10:58.000000 chromadb-0.4.3/examples/use_with/cohere/cohere_js.js
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-07-25 05:10:58.000000 chromadb-0.4.3/examples/use_with/cohere/cohere_python.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-25 05:10:58.000000 chromadb-0.4.3/examples/use_with/cohere/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-25 05:10:58.000000 chromadb-0.4.3/log_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-25 05:10:58.000000 chromadb-0.4.3/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-25 05:10:58.000000 chromadb-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-25 05:10:58.000000 chromadb-0.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-25 05:10:58.000000 chromadb-0.4.3/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 05:11:15.670656 chromadb-0.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.204790 chromadb-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-01 01:20:33.000000 chromadb-0.4.4/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.164790 chromadb-0.4.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.172790 chromadb-0.4.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-08-01 01:20:33.000000 chromadb-0.4.4/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-08-01 01:20:33.000000 chromadb-0.4.4/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-08-01 01:20:33.000000 chromadb-0.4.4/.github/ISSUE_TEMPLATE/installation_trouble.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.172790 chromadb-0.4.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-08-01 01:20:33.000000 chromadb-0.4.4/.github/workflows/chroma-client-integration-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-01 01:20:33.000000 chromadb-0.4.4/.github/workflows/chroma-integration-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-08-01 01:20:33.000000 chromadb-0.4.4/.github/workflows/chroma-release-python-client.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-08-01 01:20:33.000000 chromadb-0.4.4/.github/workflows/chroma-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-08-01 01:20:33.000000 chromadb-0.4.4/.github/workflows/chroma-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-08-01 01:20:33.000000 chromadb-0.4.4/.github/workflows/pr-review-checklist.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-01 01:20:33.000000 chromadb-0.4.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-01 01:20:33.000000 chromadb-0.4.4/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.172790 chromadb-0.4.4/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-08-01 01:20:33.000000 chromadb-0.4.4/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-08-01 01:20:33.000000 chromadb-0.4.4/DEVELOP.md
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-01 01:20:33.000000 chromadb-0.4.4/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 01:20:33.000000 chromadb-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-08-01 01:20:52.204790 chromadb-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-08-01 01:20:33.000000 chromadb-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-08-01 01:20:33.000000 chromadb-0.4.4/RELEASE_PROCESS.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.172790 chromadb-0.4.4/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      110 2023-08-01 01:20:33.000000 chromadb-0.4.4/bin/build
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-08-01 01:20:33.000000 chromadb-0.4.4/bin/docker_entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-08-01 01:20:33.000000 chromadb-0.4.4/bin/generate_cloudformation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      487 2023-08-01 01:20:33.000000 chromadb-0.4.4/bin/integration-test
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.172790 chromadb-0.4.4/bin/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-01 01:20:33.000000 chromadb-0.4.4/bin/templates/docker-compose.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      451 2023-08-01 01:20:33.000000 chromadb-0.4.4/bin/test-package.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      321 2023-08-01 01:20:33.000000 chromadb-0.4.4/bin/test-remote
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-08-01 01:20:33.000000 chromadb-0.4.4/bin/test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      151 2023-08-01 01:20:33.000000 chromadb-0.4.4/bin/version
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-01 01:20:33.000000 chromadb-0.4.4/bin/windows_upgrade_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.172790 chromadb-0.4.4/chromadb/
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.176790 chromadb-0.4.4/chromadb/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11736 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/api/fastapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.176790 chromadb-0.4.4/chromadb/api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    14958 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/api/models/Collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22104 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/api/segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/api/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.176790 chromadb-0.4.4/chromadb/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/db/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.176790 chromadb-0.4.4/chromadb/db/impl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/db/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/db/impl/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/db/impl/sqlite_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/db/migrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.176790 chromadb-0.4.4/chromadb/db/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/db/mixins/embeddings_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16398 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/db/mixins/sysdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/db/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.176790 chromadb-0.4.4/chromadb/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)   368824 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/experimental/density_relevance.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.176790 chromadb-0.4.4/chromadb/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/ingest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.176790 chromadb-0.4.4/chromadb/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.176790 chromadb-0.4.4/chromadb/migrations/embeddings_queue/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/migrations/embeddings_queue/00001-embeddings.sqlite.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.180790 chromadb-0.4.4/chromadb/migrations/metadb/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/migrations/metadb/00001-embedding-metadata.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/migrations/metadb/00002-embedding-metadata.sqlite.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.180790 chromadb-0.4.4/chromadb/migrations/sysdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/migrations/sysdb/00001-collections.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/migrations/sysdb/00002-segments.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/migrations/sysdb/00003-collection-dimension.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.180790 chromadb-0.4.4/chromadb/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/segment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.168790 chromadb-0.4.4/chromadb/segment/impl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.180790 chromadb-0.4.4/chromadb/segment/impl/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/segment/impl/manager/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.180790 chromadb-0.4.4/chromadb/segment/impl/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    19999 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/segment/impl/metadata/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.180790 chromadb-0.4.4/chromadb/segment/impl/vector/
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/segment/impl/vector/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/segment/impl/vector/brute_force_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/segment/impl/vector/hnsw_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10716 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/segment/impl/vector/local_hnsw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16931 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/segment/impl/vector/local_persistent_hnsw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.184790 chromadb-0.4.4/chromadb/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.184790 chromadb-0.4.4/chromadb/server/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/server/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/server/fastapi/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.184790 chromadb-0.4.4/chromadb/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/telemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/telemetry/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/telemetry/posthog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.184790 chromadb-0.4.4/chromadb/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.184790 chromadb-0.4.4/chromadb/test/db/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.184790 chromadb-0.4.4/chromadb/test/db/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/test/db/migrations/00001-migration-1.psql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/test/db/migrations/00001-migration-1.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/test/db/migrations/00002-migration-2.psql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/test/db/migrations/00002-migration-2.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/test/db/migrations/00003-migration-3.psql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/test/db/migrations/00003-migration-3.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/test/db/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/test/db/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/test/db/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10090 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/test/db/test_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.188790 chromadb-0.4.4/chromadb/test/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/test/ingest/test_producer_consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.188790 chromadb-0.4.4/chromadb/test/property/
+-rw-r--r--   0 runner    (1001) docker     (123)    11885 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/test/property/invariants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/test/property/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/test/property/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/test/property/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10447 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/test/property/test_cross_version_persist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14079 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/test/property/test_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/test/property/test_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/test/property/test_persist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.188790 chromadb-0.4.4/chromadb/test/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)    15950 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/test/segment/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14604 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/test/segment/test_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.188790 chromadb-0.4.4/chromadb/test/stress/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/test/stress/test_many_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40439 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/test/test_chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/test/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/test/test_multithreaded.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.188790 chromadb-0.4.4/chromadb/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/test/utils/test_messagid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.188790 chromadb-0.4.4/chromadb/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/utils/delete_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/utils/distance_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/utils/embedding_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/utils/lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/utils/messageid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-08-01 01:20:33.000000 chromadb-0.4.4/chromadb/utils/read_write_lock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.176790 chromadb-0.4.4/chromadb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-08-01 01:20:52.000000 chromadb-0.4.4/chromadb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-08-01 01:20:52.000000 chromadb-0.4.4/chromadb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 01:20:52.000000 chromadb-0.4.4/chromadb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-08-01 01:20:52.000000 chromadb-0.4.4/chromadb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-01 01:20:52.000000 chromadb-0.4.4/chromadb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.168790 chromadb-0.4.4/clients/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.192790 chromadb-0.4.4/clients/js/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/.prettierrc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/DEVELOP.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.168790 chromadb-0.4.4/clients/js/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.192790 chromadb-0.4.4/clients/js/examples/browser/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/examples/browser/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/examples/browser/app.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/examples/browser/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/examples/browser/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)    68042 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/examples/browser/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.192790 chromadb-0.4.4/clients/js/examples/node/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/examples/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/examples/node/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/examples/node/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17080 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/examples/node/yarn.lock
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1247 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/genapi.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/jest.config.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/openapitools.json
+-rw-r--r--   0 runner    (1001) docker     (123)   448020 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.196790 chromadb-0.4.4/clients/js/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/src/ChromaClient.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    19757 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/src/Collection.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.196790 chromadb-0.4.4/clients/js/src/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/src/embeddings/CohereEmbeddingFunction.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/src/embeddings/IEmbeddingFunction.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/src/embeddings/TransformersEmbeddingFunction.ts
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3402 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/src/embeddings/WebAIEmbeddingFunction.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.196790 chromadb-0.4.4/clients/js/src/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/src/generated/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    54547 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/src/generated/api.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/src/generated/configuration.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/src/generated/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/src/generated/models.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/src/generated/runtime.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/src/types.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/src/utils.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.200790 chromadb-0.4.4/clients/js/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/test/add.collections.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/test/client.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/test/collection.client.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/test/collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/test/data.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/test/delete.collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/test/get.collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/test/initClient.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/test/peek.collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/test/query.collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/test/update.collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/test/upsert.collections.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/tsconfig.module.json
+-rw-r--r--   0 runner    (1001) docker     (123)   156893 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/js/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.200790 chromadb-0.4.4/clients/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/python/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1257 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/python/build_python_thin_client.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      850 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/python/integration-test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/python/is_thin_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-08-01 01:20:33.000000 chromadb-0.4.4/clients/python/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-08-01 01:20:33.000000 chromadb-0.4.4/docker-compose.server.example.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-08-01 01:20:33.000000 chromadb-0.4.4/docker-compose.test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-01 01:20:33.000000 chromadb-0.4.4/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.200790 chromadb-0.4.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-08-01 01:20:33.000000 chromadb-0.4.4/docs/CIP_Chroma_Improvment_Proposals.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.200790 chromadb-0.4.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-08-01 01:20:33.000000 chromadb-0.4.4/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.204790 chromadb-0.4.4/examples/basic_functionality/
+-rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-08-01 01:20:33.000000 chromadb-0.4.4/examples/basic_functionality/alternative_embeddings.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-08-01 01:20:33.000000 chromadb-0.4.4/examples/basic_functionality/local_persistence.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-08-01 01:20:33.000000 chromadb-0.4.4/examples/basic_functionality/where_filtering.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.168790 chromadb-0.4.4/examples/deployments/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.204790 chromadb-0.4.4/examples/deployments/google-cloud-compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-08-01 01:20:33.000000 chromadb-0.4.4/examples/deployments/google-cloud-compute/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-08-01 01:20:33.000000 chromadb-0.4.4/examples/deployments/google-cloud-compute/chroma.tf
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-01 01:20:33.000000 chromadb-0.4.4/examples/deployments/google-cloud-compute/main.tf
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-08-01 01:20:33.000000 chromadb-0.4.4/examples/deployments/google-cloud-compute/startup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-08-01 01:20:33.000000 chromadb-0.4.4/examples/deployments/google-cloud-compute/variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.168790 chromadb-0.4.4/examples/use_with/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:52.204790 chromadb-0.4.4/examples/use_with/cohere/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-08-01 01:20:33.000000 chromadb-0.4.4/examples/use_with/cohere/cohere_js.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-08-01 01:20:33.000000 chromadb-0.4.4/examples/use_with/cohere/cohere_python.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-01 01:20:33.000000 chromadb-0.4.4/examples/use_with/cohere/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-01 01:20:33.000000 chromadb-0.4.4/log_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-08-01 01:20:33.000000 chromadb-0.4.4/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-08-01 01:20:33.000000 chromadb-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-08-01 01:20:33.000000 chromadb-0.4.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-01 01:20:33.000000 chromadb-0.4.4/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 01:20:52.204790 chromadb-0.4.4/setup.cfg
```

### Comparing `chromadb-0.4.3/.github/ISSUE_TEMPLATE/bug_report.yaml` & `chromadb-0.4.4/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/.github/ISSUE_TEMPLATE/feature_request.yaml` & `chromadb-0.4.4/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/.github/ISSUE_TEMPLATE/installation_trouble.yaml` & `chromadb-0.4.4/.github/ISSUE_TEMPLATE/installation_trouble.yaml`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/.github/workflows/chroma-client-integration-test.yml` & `chromadb-0.4.4/.github/workflows/chroma-client-integration-test.yml`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 jobs:
   test:
     timeout-minutes: 90
     strategy:
       matrix:
         python: ['3.7', '3.8', '3.9', '3.10']
-        platform: [ubuntu-latest]
+        platform: [ubuntu-latest, windows-latest]
     runs-on: ${{ matrix.platform }}
     steps:
     - name: Checkout
       uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python }}
       uses: actions/setup-python@v4
       with:
```

### Comparing `chromadb-0.4.3/.github/workflows/chroma-integration-test.yml` & `chromadb-0.4.4/.github/workflows/chroma-integration-test.yml`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
       - '**'
 
 jobs:
   test:
     strategy:
       matrix:
         python: ['3.7']
-        platform: [ubuntu-latest]
+        platform: [ubuntu-latest, windows-latest]
         testfile: ["--ignore-glob 'chromadb/test/property/*'",
                    "chromadb/test/property/test_add.py",
                    "chromadb/test/property/test_collections.py",
                    "chromadb/test/property/test_cross_version_persist.py",
                    "chromadb/test/property/test_embeddings.py",
                    "chromadb/test/property/test_filtering.py",
                    "chromadb/test/property/test_persist.py"]
```

### Comparing `chromadb-0.4.3/.github/workflows/chroma-release-python-client.yml` & `chromadb-0.4.4/.github/workflows/chroma-release-python-client.yml`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/.github/workflows/chroma-release.yml` & `chromadb-0.4.4/.github/workflows/chroma-release.yml`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/.github/workflows/pr-review-checklist.yml` & `chromadb-0.4.4/.github/workflows/pr-review-checklist.yml`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/.pre-commit-config.yaml` & `chromadb-0.4.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/.vscode/settings.json` & `chromadb-0.4.4/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/DEVELOP.md` & `chromadb-0.4.4/DEVELOP.md`

 * *Files 10% similar despite different names*

```diff
@@ -32,30 +32,25 @@
 ```
 
 2. Standalone and in-memory with persistence:
 
 This by default saves your db and your indexes to a `.chroma` directory and can also load from them.
 ```python
 import chromadb
-from chromadb.config import Settings
-api = chromadb.Client(Settings(chroma_db_impl="duckdb+parquet",
-                      persist_directory="/path/to/persist/directory"))
+api = chromadb.PersistentClient(path="/path/to/persist/directory")
 print(api.heartbeat())
 ```
 
 
 3. With a persistent backend and a small frontend client
 
 Run `docker-compose up -d --build`
 ```python
 import chromadb
-from chromadb.config import Settings
-api = chromadb.Client(Settings(chroma_api_impl="rest",
-                              chroma_server_host="localhost",
-                              chroma_server_http_port="8000") )
+api = chromadb.HttpClient(host="localhost", port="8000")
 
 print(api.heartbeat())
 ```
 
 ## Testing
 
 Unit tests are in the `/chromadb/test` directory.
```

### Comparing `chromadb-0.4.3/Dockerfile` & `chromadb-0.4.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/LICENSE` & `chromadb-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/PKG-INFO` & `chromadb-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromadb
-Version: 0.4.3
+Version: 0.4.4
 Summary: Chroma.
 Author-email: Jeff Huber <jeff@trychroma.com>, Anton Troynikov <anton@trychroma.com>
 Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chromadb Version: 0.4.3 Summary: Chroma. Author-
+Metadata-Version: 2.1 Name: chromadb Version: 0.4.4 Summary: Chroma. Author-
 email: Jeff Huber
 trychroma.com>, Anton Troynikov
 trychroma.com> Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `chromadb-0.4.3/README.md` & `chromadb-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/RELEASE_PROCESS.md` & `chromadb-0.4.4/RELEASE_PROCESS.md`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/bin/generate_cloudformation.py` & `chromadb-0.4.4/bin/generate_cloudformation.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/chromadb/__init__.py` & `chromadb-0.4.4/chromadb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from chromadb.config import Settings, System
 from chromadb.api import API
 
 logger = logging.getLogger(__name__)
 
 __settings = Settings()
 
-__version__ = "0.4.3"
+__version__ = "0.4.4"
 
 # Workaround to deal with Colab's old sqlite3 version
 try:
     import google.colab  # noqa: F401
 
     IN_COLAB = True
 except ImportError:
```

### Comparing `chromadb-0.4.3/chromadb/api/__init__.py` & `chromadb-0.4.4/chromadb/api/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from abc import ABC, abstractmethod
 from typing import Sequence, Optional
-import pandas as pd
 from uuid import UUID
 from chromadb.api.models.Collection import Collection
 from chromadb.api.types import (
     CollectionMetadata,
     Documents,
     EmbeddingFunction,
     Embeddings,
@@ -178,15 +177,14 @@
     def _add(
         self,
         ids: IDs,
         collection_id: UUID,
         embeddings: Embeddings,
         metadatas: Optional[Metadatas] = None,
         documents: Optional[Documents] = None,
-        increment_index: bool = True,
     ) -> bool:
         """[Internal] Add embeddings to a collection specified by UUID.
         If (some) ids already exist, only the new embeddings will be added.
 
         Args:
             ids: The ids to associate with the embeddings.
             collection_id: The UUID of the collection to add the embeddings to.
@@ -226,28 +224,25 @@
     def _upsert(
         self,
         collection_id: UUID,
         ids: IDs,
         embeddings: Embeddings,
         metadatas: Optional[Metadatas] = None,
         documents: Optional[Documents] = None,
-        increment_index: bool = True,
     ) -> bool:
         """[Internal] Add or update entries in the a collection specified by UUID.
         If an entry with the same id already exists, it will be updated,
         otherwise it will be added.
 
         Args:
             collection_id: The collection to add the embeddings to
             ids: The ids to associate with the embeddings. Defaults to None.
             embeddings: The sequence of embeddings to add
             metadatas: The metadata to associate with the embeddings. Defaults to None.
             documents: The documents to associate with the embeddings. Defaults to None.
-            increment_index: If True, will incrementally add to the ANN index.
-                                          Defaults to True.
         """
         pass
 
     @abstractmethod
     def _count(self, collection_id: UUID) -> int:
         """[Internal] Returns the number of entries in a collection specified by UUID.
 
@@ -361,39 +356,14 @@
 
         Returns:
             bool: True if the database was reset successfully.
         """
         pass
 
     @abstractmethod
-    def raw_sql(self, sql: str) -> pd.DataFrame:
-        """Runs a raw SQL query against the database
-
-        Args:
-            sql: The SQL query to run
-
-        Returns:
-            pd.DataFrame: A pandas dataframe containing the results of the query
-        """
-        pass
-
-    @abstractmethod
-    def create_index(self, collection_name: str) -> bool:
-        """Creates an index for the given collection
-
-        Args:
-            collection_name: The collection to create the index for. Defaults to None.
-
-        Returns:
-            bool: True if the index was created successfully
-
-        """
-        pass
-
-    @abstractmethod
     def get_version(self) -> str:
         """Get the version of Chroma.
 
         Returns:
             str: The version of Chroma
 
         """
```

### Comparing `chromadb-0.4.3/chromadb/api/fastapi.py` & `chromadb-0.4.4/chromadb/api/fastapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     Where,
     WhereDocument,
     GetResult,
     QueryResult,
     CollectionMetadata,
 )
 import chromadb.utils.embedding_functions as ef
-import pandas as pd
 import requests
 import json
 from typing import Sequence
 from chromadb.api.models.Collection import Collection
 import chromadb.errors as errors
 from uuid import UUID
 from chromadb.telemetry import Telemetry
@@ -227,31 +226,27 @@
     def _add(
         self,
         ids: IDs,
         collection_id: UUID,
         embeddings: Embeddings,
         metadatas: Optional[Metadatas] = None,
         documents: Optional[Documents] = None,
-        increment_index: bool = True,
     ) -> bool:
         """
         Adds a batch of embeddings to the database
         - pass in column oriented data lists
-        - by default, the index is progressively built up as you add more data. If for ingestion performance reasons you want to disable this, set increment_index to False
-        -   and then manually create the index yourself with collection.create_index()
         """
         resp = self._session.post(
             self._api_url + "/collections/" + str(collection_id) + "/add",
             data=json.dumps(
                 {
                     "ids": ids,
                     "embeddings": embeddings,
                     "metadatas": metadatas,
                     "documents": documents,
-                    "increment_index": increment_index,
                 }
             ),
         )
 
         raise_chroma_error(resp)
         return True
 
@@ -287,29 +282,27 @@
     def _upsert(
         self,
         collection_id: UUID,
         ids: IDs,
         embeddings: Embeddings,
         metadatas: Optional[Metadatas] = None,
         documents: Optional[Documents] = None,
-        increment_index: bool = True,
     ) -> bool:
         """
         Upserts a batch of embeddings in the database
         - pass in column oriented data lists
         """
         resp = self._session.post(
             self._api_url + "/collections/" + str(collection_id) + "/upsert",
             data=json.dumps(
                 {
                     "ids": ids,
                     "embeddings": embeddings,
                     "metadatas": metadatas,
                     "documents": documents,
-                    "increment_index": increment_index,
                 }
             ),
         )
 
         resp.raise_for_status()
         return True
 
@@ -352,32 +345,14 @@
     def reset(self) -> bool:
         """Resets the database"""
         resp = self._session.post(self._api_url + "/reset")
         raise_chroma_error(resp)
         return cast(bool, resp.json())
 
     @override
-    def raw_sql(self, sql: str) -> pd.DataFrame:
-        """Runs a raw SQL query against the database"""
-        resp = self._session.post(
-            self._api_url + "/raw_sql", data=json.dumps({"raw_sql": sql})
-        )
-        raise_chroma_error(resp)
-        return pd.DataFrame.from_dict(resp.json())
-
-    @override
-    def create_index(self, collection_name: str) -> bool:
-        """Soon deprecated"""
-        resp = self._session.post(
-            self._api_url + "/collections/" + collection_name + "/create_index"
-        )
-        raise_chroma_error(resp)
-        return cast(bool, resp.json())
-
-    @override
     def get_version(self) -> str:
         """Returns the version of the server"""
         resp = self._session.get(self._api_url + "/version")
         raise_chroma_error(resp)
         return cast(str, resp.json())
 
     @override
```

### Comparing `chromadb-0.4.3/chromadb/api/models/Collection.py` & `chromadb-0.4.4/chromadb/api/models/Collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,14 @@
 
     def add(
         self,
         ids: OneOrMany[ID],
         embeddings: Optional[OneOrMany[Embedding]] = None,
         metadatas: Optional[OneOrMany[Metadata]] = None,
         documents: Optional[OneOrMany[Document]] = None,
-        increment_index: bool = True,
     ) -> None:
         """Add embeddings to the data store.
         Args:
             ids: The ids of the embeddings you wish to add
             embeddings: The embeddings to add. If None, embeddings will be computed based on the documents using the embedding_function set for the Collection. Optional.
             metadatas: The metadata to associate with the embeddings. When querying, you can filter on this metadata. Optional.
             documents: The documents to associate with the embeddings. Optional.
@@ -93,17 +92,15 @@
 
         """
 
         ids, embeddings, metadatas, documents = self._validate_embedding_set(
             ids, embeddings, metadatas, documents
         )
 
-        self._client._add(
-            ids, self.id, embeddings, metadatas, documents, increment_index
-        )
+        self._client._add(ids, self.id, embeddings, metadatas, documents)
 
     def get(
         self,
         ids: Optional[OneOrMany[ID]] = None,
         where: Optional[Where] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
@@ -277,15 +274,14 @@
 
     def upsert(
         self,
         ids: OneOrMany[ID],
         embeddings: Optional[OneOrMany[Embedding]] = None,
         metadatas: Optional[OneOrMany[Metadata]] = None,
         documents: Optional[OneOrMany[Document]] = None,
-        increment_index: bool = True,
     ) -> None:
         """Update the embeddings, metadatas or documents for provided ids, or create them if they don't exist.
 
         Args:
             ids: The ids of the embeddings to update
             embeddings: The embeddings to add. If None, embeddings will be computed based on the documents using the embedding_function set for the Collection. Optional.
             metadatas:  The metadata to associate with the embeddings. When querying, you can filter on this metadata. Optional.
@@ -301,15 +297,14 @@
 
         self._client._upsert(
             collection_id=self.id,
             ids=ids,
             embeddings=embeddings,
             metadatas=metadatas,
             documents=documents,
-            increment_index=increment_index,
         )
 
     def delete(
         self,
         ids: Optional[IDs] = None,
         where: Optional[Where] = None,
         where_document: Optional[WhereDocument] = None,
@@ -327,17 +322,14 @@
         ids = validate_ids(maybe_cast_one_to_many(ids)) if ids else None
         where = validate_where(where) if where else None
         where_document = (
             validate_where_document(where_document) if where_document else None
         )
         self._client._delete(self.id, ids, where, where_document)
 
-    def create_index(self) -> None:
-        self._client.create_index(self.name)
-
     def _validate_embedding_set(
         self,
         ids: OneOrMany[ID],
         embeddings: Optional[OneOrMany[Embedding]],
         metadatas: Optional[OneOrMany[Metadata]],
         documents: Optional[OneOrMany[Document]],
         require_embeddings_or_documents: bool = True,
```

### Comparing `chromadb-0.4.3/chromadb/api/segment.py` & `chromadb-0.4.4/chromadb/api/segment.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 from chromadb.telemetry.events import CollectionAddEvent, CollectionDeleteEvent
 
 import chromadb.types as t
 
 from typing import Optional, Sequence, Generator, List, cast, Set, Dict
 from overrides import override
 from uuid import UUID, uuid4
-import pandas as pd
 import time
 import logging
 import re
 
 logger = logging.getLogger(__name__)
 
 
@@ -235,15 +234,14 @@
     def _add(
         self,
         ids: IDs,
         collection_id: UUID,
         embeddings: Embeddings,
         metadatas: Optional[Metadatas] = None,
         documents: Optional[Documents] = None,
-        increment_index: bool = True,
     ) -> bool:
         coll = self._get_collection(collection_id)
         self._manager.hint_use_collection(collection_id, t.Operation.ADD)
 
         for r in _records(t.Operation.ADD, ids, embeddings, metadatas, documents):
             self._validate_embedding_record(coll, r)
             self._producer.submit_embedding(coll["topic"], r)
@@ -273,15 +271,14 @@
     def _upsert(
         self,
         collection_id: UUID,
         ids: IDs,
         embeddings: Embeddings,
         metadatas: Optional[Metadatas] = None,
         documents: Optional[Documents] = None,
-        increment_index: bool = True,
     ) -> bool:
         coll = self._get_collection(collection_id)
         self._manager.hint_use_collection(collection_id, t.Operation.UPSERT)
 
         for r in _records(t.Operation.UPSERT, ids, embeddings, metadatas, documents):
             self._validate_embedding_record(coll, r)
             self._producer.submit_embedding(coll["topic"], r)
@@ -322,15 +319,15 @@
             where=where,
             where_document=where_document,
             ids=ids,
             limit=limit,
             offset=offset,
         )
 
-        vectors = None
+        vectors: Sequence[t.VectorEmbeddingRecord] = []
         if "embeddings" in include:
             vector_ids = [r["id"] for r in records]
             vector_segment = self._manager.get_segment(collection_id, VectorReader)
             vectors = vector_segment.get_vectors(ids=vector_ids)
 
         # TODO: Fix type so we don't need to ignore
         # It is possible to have a set of records, some with metadata and some without
@@ -339,15 +336,17 @@
         metadatas = [r["metadata"] for r in records]
 
         if "documents" in include:
             documents = [_doc(m) for m in metadatas]
 
         return GetResult(
             ids=[r["id"] for r in records],
-            embeddings=[r["embedding"] for r in vectors] if vectors else None,
+            embeddings=[r["embedding"] for r in vectors]
+            if "embeddings" in include
+            else None,
             metadatas=_clean_metadatas(metadatas) if "metadatas" in include else None,  # type: ignore
             documents=documents if "documents" in include else None,  # type: ignore
         )
 
     @override
     def _delete(
         self,
@@ -491,25 +490,14 @@
 
     @override
     def reset(self) -> bool:
         self._system.reset_state()
         return True
 
     @override
-    def raw_sql(self, sql: str) -> pd.DataFrame:
-        raise NotImplementedError()
-
-    @override
-    def create_index(self, collection_name: str) -> bool:
-        logger.warning(
-            "Calling create_index is unnecessary, data is now automatically indexed"
-        )
-        return True
-
-    @override
     def get_settings(self) -> Settings:
         return self._settings
 
     def _topic(self, collection_id: UUID) -> str:
         return f"persistent://{self._tenant_id}/{self._topic_ns}/{collection_id}"
 
     # TODO: This could potentially cause race conditions in a distributed version of the
```

### Comparing `chromadb-0.4.3/chromadb/api/types.py` & `chromadb-0.4.4/chromadb/api/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,54 +119,57 @@
         raise errors.DuplicateIDError(
             f"Expected IDs to be unique, found duplicates for: {dups}"
         )
     return ids
 
 
 def validate_metadata(metadata: Metadata) -> Metadata:
-    """Validates metadata to ensure it is a dictionary of strings to strings, ints, or floats"""
+    """Validates metadata to ensure it is a dictionary of strings to strings, ints, floats or bools"""
     if not isinstance(metadata, dict) and metadata is not None:
         raise ValueError(f"Expected metadata to be a dict or None, got {metadata}")
     if metadata is None:
         return metadata
     if len(metadata) == 0:
         raise ValueError(f"Expected metadata to be a non-empty dict, got {metadata}")
     for key, value in metadata.items():
         if not isinstance(key, str):
             raise ValueError(
                 f"Expected metadata key to be a str, got {key} which is a {type(key)}"
             )
         # isinstance(True, int) evaluates to True, so we need to check for bools separately
-        if not isinstance(value, (str, int, float)) or isinstance(value, bool):
+        if not isinstance(value, bool) and not isinstance(value, (str, int, float)):
             raise ValueError(
-                f"Expected metadata value to be a str, int, or float, got {value} which is a {type(value)}"
+                f"Expected metadata value to be a str, int, float or bool, got {value} which is a {type(value)}"
             )
     return metadata
 
 
 def validate_update_metadata(metadata: UpdateMetadata) -> UpdateMetadata:
-    """Validates metadata to ensure it is a dictionary of strings to strings, ints, or floats"""
+    """Validates metadata to ensure it is a dictionary of strings to strings, ints, floats or bools"""
     if not isinstance(metadata, dict) and metadata is not None:
         raise ValueError(f"Expected metadata to be a dict or None, got {metadata}")
     if metadata is None:
         return metadata
     if len(metadata) == 0:
         raise ValueError(f"Expected metadata to be a non-empty dict, got {metadata}")
     for key, value in metadata.items():
         if not isinstance(key, str):
             raise ValueError(f"Expected metadata key to be a str, got {key}")
-        if not isinstance(value, (str, int, float, type(None))):
+        # isinstance(True, int) evaluates to True, so we need to check for bools separately
+        if not isinstance(value, bool) and not isinstance(
+            value, (str, int, float, type(None))
+        ):
             raise ValueError(
                 f"Expected metadata value to be a str, int, or float, got {value}"
             )
     return metadata
 
 
 def validate_metadatas(metadatas: Metadatas) -> Metadatas:
-    """Validates metadatas to ensure it is a list of dictionaries of strings to strings, ints, or floats"""
+    """Validates metadatas to ensure it is a list of dictionaries of strings to strings, ints, floats or bools"""
     if not isinstance(metadatas, list):
         raise ValueError(f"Expected metadatas to be a list, got {metadatas}")
     for metadata in metadatas:
         validate_metadata(metadata)
     return metadatas
```

### Comparing `chromadb-0.4.3/chromadb/config.py` & `chromadb-0.4.4/chromadb/config.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/chromadb/db/__init__.py` & `chromadb-0.4.4/chromadb/db/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,20 +56,14 @@
         metadatas: Optional[Metadatas],
         documents: Optional[Documents],
         ids: List[str],
     ) -> List[UUID]:
         pass
 
     @abstractmethod
-    def add_incremental(
-        self, collection_uuid: UUID, ids: List[UUID], embeddings: Embeddings
-    ) -> None:
-        pass
-
-    @abstractmethod
     def get(
         self,
         where: Where = {},
         collection_name: Optional[str] = None,
         collection_uuid: Optional[UUID] = None,
         ids: Optional[IDs] = None,
         sort: Optional[str] = None,
@@ -117,15 +111,7 @@
         pass
 
     @abstractmethod
     def get_by_ids(
         self, uuids: List[UUID], columns: Optional[List[str]] = None
     ) -> Sequence:  # type: ignore
         pass
-
-    @abstractmethod
-    def raw_sql(self, raw_sql):  # type: ignore
-        pass
-
-    @abstractmethod
-    def create_index(self, collection_uuid: UUID):  # type: ignore
-        pass
```

### Comparing `chromadb-0.4.3/chromadb/db/base.py` & `chromadb-0.4.4/chromadb/db/base.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/chromadb/db/impl/sqlite.py` & `chromadb-0.4.4/chromadb/db/impl/sqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from chromadb.db.impl.sqlite_pool import Connection, LockPool, PerThreadPool, Pool
 from chromadb.db.migrations import MigratableDB, Migration
 from chromadb.config import System, Settings
 import chromadb.db.base as base
 from chromadb.db.mixins.embeddings_queue import SqlEmbeddingsQueue
 from chromadb.db.mixins.sysdb import SqlSysDB
+from chromadb.utils.delete_file import delete_file
 import sqlite3
 from overrides import override
 import pypika
 from typing import Sequence, cast, Optional, Type, Any
 from typing_extensions import Literal
 from types import TracebackType
 import os
@@ -135,15 +136,15 @@
                 WHERE type='table'
                 """
             )
             for row in cur.fetchall():
                 cur.execute(f"DROP TABLE IF EXISTS {row[0]}")
         self._conn_pool.close()
         if self._is_persistent:
-            os.remove(self._db_file)
+            delete_file(self._db_file)
         self.start()
         super().reset_state()
 
     @override
     def setup_migrations(self) -> None:
         with self.tx() as cur:
             cur.execute(
```

### Comparing `chromadb-0.4.3/chromadb/db/impl/sqlite_pool.py` & `chromadb-0.4.4/chromadb/db/impl/sqlite_pool.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/chromadb/db/migrations.py` & `chromadb-0.4.4/chromadb/db/migrations.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/chromadb/db/mixins/embeddings_queue.py` & `chromadb-0.4.4/chromadb/db/mixins/embeddings_queue.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/chromadb/db/mixins/sysdb.py` & `chromadb-0.4.4/chromadb/db/mixins/sysdb.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/chromadb/db/system.py` & `chromadb-0.4.4/chromadb/db/system.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/chromadb/errors.py` & `chromadb-0.4.4/chromadb/errors.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/chromadb/experimental/density_relevance.ipynb` & `chromadb-0.4.4/chromadb/experimental/density_relevance.ipynb`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/chromadb/ingest/__init__.py` & `chromadb-0.4.4/chromadb/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/chromadb/migrations/metadb/00001-embedding-metadata.sqlite.sql` & `chromadb-0.4.4/chromadb/migrations/metadb/00001-embedding-metadata.sqlite.sql`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/chromadb/segment/__init__.py` & `chromadb-0.4.4/chromadb/segment/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/chromadb/segment/impl/manager/local.py` & `chromadb-0.4.4/chromadb/segment/impl/manager/local.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,18 +6,29 @@
     VectorReader,
     S,
 )
 from chromadb.config import System, get_class
 from chromadb.db.system import SysDB
 from overrides import override
 from enum import Enum
+from chromadb.segment.impl.vector.local_persistent_hnsw import (
+    PersistentLocalHnswSegment,
+)
 from chromadb.types import Collection, Operation, Segment, SegmentScope, Metadata
 from typing import Dict, Type, Sequence, Optional, cast
 from uuid import UUID, uuid4
 from collections import defaultdict
+import platform
+
+from chromadb.utils.lru_cache import LRUCache
+
+if platform.system() != "Windows":
+    import resource
+elif platform.system() == "Windows":
+    import ctypes
 
 
 class SegmentType(Enum):
     SQLITE = "urn:chroma:segment/metadata/sqlite"
     HNSW_LOCAL_MEMORY = "urn:chroma:segment/vector/hnsw-local-memory"
     HNSW_LOCAL_PERSISTED = "urn:chroma:segment/vector/hnsw-local-persisted"
 
@@ -29,28 +40,45 @@
 }
 
 
 class LocalSegmentManager(SegmentManager):
     _sysdb: SysDB
     _system: System
     _instances: Dict[UUID, SegmentImplementation]
-    _segment_cache: Dict[UUID, Dict[SegmentScope, Segment]]
+    _vector_instances_file_handle_cache: LRUCache[
+        UUID, PersistentLocalHnswSegment
+    ]  # LRU cache to manage file handles across vector segment instances
+    _segment_cache: Dict[
+        UUID, Dict[SegmentScope, Segment]
+    ]  # Tracks which segments are loaded for a given collection
     _vector_segment_type: SegmentType = SegmentType.HNSW_LOCAL_MEMORY
     _lock: Lock
+    _max_file_handles: int
 
     def __init__(self, system: System):
         super().__init__(system)
         self._sysdb = self.require(SysDB)
         self._system = system
         self._instances = {}
         self._segment_cache = defaultdict(dict)
         self._lock = Lock()
 
         if self._system.settings.require("is_persistent"):
             self._vector_segment_type = SegmentType.HNSW_LOCAL_PERSISTED
+            if platform.system() != "Windows":
+                self._max_file_handles = resource.getrlimit(resource.RLIMIT_NOFILE)[0]
+            else:
+                self._max_file_handles = ctypes.windll.msvcrt._getmaxstdio()  # type: ignore
+            segment_limit = (
+                self._max_file_handles
+                // PersistentLocalHnswSegment.get_file_handle_count()
+            )
+            self._vector_instances_file_handle_cache = LRUCache(
+                segment_limit, callback=lambda _, v: v.close_persistent_index()
+            )
 
     @override
     def start(self) -> None:
         for instance in self._instances.values():
             instance.start()
         super().start()
 
@@ -60,14 +88,15 @@
             instance.stop()
         super().stop()
 
     @override
     def reset_state(self) -> None:
         for instance in self._instances.values():
             instance.stop()
+            instance.reset_state()
         self._instances = {}
         self._segment_cache = defaultdict(dict)
         super().reset_state()
 
     @override
     def create_segments(self, collection: Collection) -> Sequence[Segment]:
         vector_segment = _segment(
@@ -114,15 +143,21 @@
 
     @override
     def hint_use_collection(self, collection_id: UUID, hint_type: Operation) -> None:
         # The local segment manager responds to hints by pre-loading both the metadata and vector
         # segments for the given collection.
         for type in [MetadataReader, VectorReader]:
             # Just use get_segment to load the segment into the cache
-            self.get_segment(collection_id, type)
+            instance = self.get_segment(collection_id, type)
+            # If the segment is a vector segment, we need to keep segments in an LRU cache
+            # to avoid hitting the OS file handle limit.
+            if type == VectorReader and self._system.settings.require("is_persistent"):
+                instance = cast(PersistentLocalHnswSegment, instance)
+                instance.open_persistent_index()
+                self._vector_instances_file_handle_cache.set(collection_id, instance)
 
     def _cls(self, segment: Segment) -> Type[SegmentImplementation]:
         classname = SEGMENT_TYPE_IMPLS[SegmentType(segment["type"])]
         cls = get_class(classname, SegmentImplementation)
         return cls
 
     def _instance(self, segment: Segment) -> SegmentImplementation:
```

### Comparing `chromadb-0.4.3/chromadb/segment/impl/metadata/sqlite.py` & `chromadb-0.4.4/chromadb/segment/impl/metadata/sqlite.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,14 +121,15 @@
                 embeddings_t.id,
                 embeddings_t.embedding_id,
                 embeddings_t.seq_id,
                 metadata_t.key,
                 metadata_t.string_value,
                 metadata_t.int_value,
                 metadata_t.float_value,
+                metadata_t.bool_value,
             )
             .where(
                 embeddings_t.segment_id == ParameterValue(self._db.uuid_to_db(self._id))
             )
             .orderby(embeddings_t.id)
         )
 
@@ -168,21 +169,26 @@
 
     def _record(self, rows: Sequence[Tuple[Any, ...]]) -> MetadataEmbeddingRecord:
         """Given a list of DB rows with the same ID, construct a
         MetadataEmbeddingRecord"""
         _, embedding_id, seq_id = rows[0][:3]
         metadata = {}
         for row in rows:
-            key, string_value, int_value, float_value = row[3:]
+            key, string_value, int_value, float_value, bool_value = row[3:]
             if string_value is not None:
                 metadata[key] = string_value
             elif int_value is not None:
                 metadata[key] = int_value
             elif float_value is not None:
                 metadata[key] = float_value
+            elif bool_value is not None:
+                if bool_value == 1:
+                    metadata[key] = True
+                else:
+                    metadata[key] = False
 
         return MetadataEmbeddingRecord(
             id=embedding_id,
             seq_id=_decode_seq_id(seq_id),
             metadata=metadata or None,
         )
 
@@ -250,40 +256,55 @@
 
     def _insert_metadata(self, cur: Cursor, id: int, metadata: UpdateMetadata) -> None:
         """Insert or update each metadata row for a single embedding record"""
         t = Table("embedding_metadata")
         q = (
             self._db.querybuilder()
             .into(t)
-            .columns(t.id, t.key, t.string_value, t.int_value, t.float_value)
+            .columns(
+                t.id, t.key, t.string_value, t.int_value, t.float_value, t.bool_value
+            )
         )
         for key, value in metadata.items():
             if isinstance(value, str):
                 q = q.insert(
                     ParameterValue(id),
                     ParameterValue(key),
                     ParameterValue(value),
                     None,
                     None,
+                    None,
+                )
+            # isinstance(True, int) evaluates to True, so we need to check for bools separately
+            elif isinstance(value, bool):
+                q = q.insert(
+                    ParameterValue(id),
+                    ParameterValue(key),
+                    None,
+                    None,
+                    None,
+                    ParameterValue(value),
                 )
             elif isinstance(value, int):
                 q = q.insert(
                     ParameterValue(id),
                     ParameterValue(key),
                     None,
                     ParameterValue(value),
                     None,
+                    None,
                 )
             elif isinstance(value, float):
                 q = q.insert(
                     ParameterValue(id),
                     ParameterValue(key),
                     None,
                     None,
                     ParameterValue(value),
+                    None,
                 )
 
         sql, params = get_sql(q)
         sql = sql.replace("INSERT", "INSERT OR REPLACE")
         if sql:
             cur.execute(sql, params)
 
@@ -490,28 +511,31 @@
 def _where_clause(
     expr: Union[LiteralValue, Dict[WhereOperator, LiteralValue]],
     table: Table,
 ) -> Criterion:
     """Given a field name, an expression, and a table, construct a Pypika Criterion"""
 
     # Literal value case
-    if isinstance(expr, (str, int, float)):
+    if isinstance(expr, (str, int, float, bool)):
         return _where_clause({"$eq": expr}, table)
 
     # Operator dict case
     operator, value = next(iter(expr.items()))
     return _value_criterion(value, operator, table)
 
 
 def _value_criterion(value: LiteralValue, op: WhereOperator, table: Table) -> Criterion:
     """Return a criterion to compare a value with the appropriate columns given its type
     and the operation type."""
 
     if isinstance(value, str):
         cols = [table.string_value]
+    # isinstance(True, int) evaluates to True, so we need to check for bools separately
+    elif isinstance(value, bool) and op in ("$eq", "$ne"):
+        cols = [table.bool_value]
     elif isinstance(value, int) and op in ("$eq", "$ne"):
         cols = [table.int_value]
     elif isinstance(value, float) and op in ("$eq", "$ne"):
         cols = [table.float_value]
     else:
         cols = [table.int_value, table.float_value]
```

### Comparing `chromadb-0.4.3/chromadb/segment/impl/vector/batch.py` & `chromadb-0.4.4/chromadb/segment/impl/vector/batch.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/chromadb/segment/impl/vector/brute_force_index.py` & `chromadb-0.4.4/chromadb/segment/impl/vector/brute_force_index.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/chromadb/segment/impl/vector/hnsw_params.py` & `chromadb-0.4.4/chromadb/segment/impl/vector/hnsw_params.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/chromadb/segment/impl/vector/local_hnsw.py` & `chromadb-0.4.4/chromadb/segment/impl/vector/local_hnsw.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/chromadb/segment/impl/vector/local_persistent_hnsw.py` & `chromadb-0.4.4/chromadb/segment/impl/vector/local_persistent_hnsw.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import shutil
 from overrides import override
 import pickle
 from typing import Dict, List, Optional, Sequence, Set, cast
 from chromadb.config import System
 from chromadb.segment.impl.vector.batch import Batch
 from chromadb.segment.impl.vector.hnsw_params import PersistentHnswParams
 from chromadb.segment.impl.vector.local_hnsw import (
@@ -257,45 +258,52 @@
             - self._curr_batch.delete_count
         )
 
     @override
     def get_vectors(
         self, ids: Optional[Sequence[str]] = None
     ) -> Sequence[VectorEmbeddingRecord]:
-        """Get the embeddings from the HNSW index and layered brute force batch index"""
-        results = []
+        """Get the embeddings from the HNSW index and layered brute force
+        batch index."""
+
         ids_hnsw: Set[str] = set()
         ids_bf: Set[str] = set()
 
         if self._index is not None:
             ids_hnsw = set(self._id_to_label.keys())
         if self._brute_force_index is not None:
             ids_bf = set(self._curr_batch.get_written_ids())
 
         target_ids = ids or list(ids_hnsw.union(ids_bf))
         self._brute_force_index = cast(BruteForceIndex, self._brute_force_index)
         hnsw_labels = []
 
-        for id in target_ids:
+        results: List[Optional[VectorEmbeddingRecord]] = []
+        id_to_index: Dict[str, int] = {}
+        for i, id in enumerate(target_ids):
             if id in ids_bf:
                 results.append(self._brute_force_index.get_vectors([id])[0])
             elif id in ids_hnsw and id not in self._curr_batch._deleted_ids:
                 hnsw_labels.append(self._id_to_label[id])
+                # Placeholder for hnsw results to be filled in down below so we
+                # can batch the hnsw get() call
+                results.append(None)
+            id_to_index[id] = i
 
         if len(hnsw_labels) > 0 and self._index is not None:
             vectors = cast(Sequence[Vector], self._index.get_items(hnsw_labels))
 
             for label, vector in zip(hnsw_labels, vectors):
                 id = self._label_to_id[label]
                 seq_id = self._id_to_seq_id[id]
-                results.append(
-                    VectorEmbeddingRecord(id=id, seq_id=seq_id, embedding=vector)
+                results[id_to_index[id]] = VectorEmbeddingRecord(
+                    id=id, seq_id=seq_id, embedding=vector
                 )
 
-        return results
+        return results  # type: ignore ## Python can't cast List with Optional to List with VectorEmbeddingRecord
 
     @override
     def query_vectors(
         self, query: VectorQuery
     ) -> Sequence[Sequence[VectorQueryResult]]:
         if self._index is None and self._brute_force_index is None:
             return [[] for _ in range(len(query["vectors"]))]
@@ -373,7 +381,31 @@
                                 curr_results.append(curr_hnsw_result[i])
                     elif remaining > 0 and bf_pointer < len(curr_bf_result):
                         curr_results.extend(
                             curr_bf_result[bf_pointer : bf_pointer + remaining]
                         )
                     results.append(curr_results)
             return results
+
+    @override
+    def reset_state(self) -> None:
+        data_path = self._get_storage_folder()
+        if os.path.exists(data_path):
+            shutil.rmtree(data_path, ignore_errors=True)
+
+    @staticmethod
+    def get_file_handle_count() -> int:
+        """Return how many file handles are used by the index"""
+        hnswlib_count = hnswlib.Index.file_handle_count
+        hnswlib_count = cast(int, hnswlib_count)
+        # One extra for the metadata file
+        return hnswlib_count + 1  # type: ignore
+
+    def open_persistent_index(self) -> None:
+        """Open the persistent index"""
+        if self._index is not None:
+            self._index.open_file_handles()
+
+    def close_persistent_index(self) -> None:
+        """Close the persistent index"""
+        if self._index is not None:
+            self._index.close_file_handles()
```

### Comparing `chromadb-0.4.3/chromadb/server/fastapi/__init__.py` & `chromadb-0.4.4/chromadb/server/fastapi/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from fastapi.responses import JSONResponse
 
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.routing import APIRoute
 from fastapi import HTTPException, status
 from uuid import UUID
 
-import pandas as pd
 
 import chromadb
 from chromadb.api.models.Collection import Collection
 from chromadb.api.types import GetResult, QueryResult
 from chromadb.config import Settings
 import chromadb.server
 import chromadb.api
@@ -22,15 +21,14 @@
     InvalidDimensionException,
 )
 from chromadb.server.fastapi.types import (
     AddEmbedding,
     DeleteEmbedding,
     GetEmbedding,
     QueryEmbedding,
-    RawSql,  # Results,
     CreateCollection,
     UpdateCollection,
     UpdateEmbedding,
 )
 from starlette.requests import Request
 
 import logging
@@ -88,17 +86,14 @@
 
         self.router = fastapi.APIRouter()
 
         self.router.add_api_route("/api/v1", self.root, methods=["GET"])
         self.router.add_api_route("/api/v1/reset", self.reset, methods=["POST"])
         self.router.add_api_route("/api/v1/version", self.version, methods=["GET"])
         self.router.add_api_route("/api/v1/heartbeat", self.heartbeat, methods=["GET"])
-        self.router.add_api_route(
-            "/api/v1/raw_sql", self.raw_sql, methods=["POST"], response_model=None
-        )
 
         self.router.add_api_route(
             "/api/v1/collections",
             self.list_collections,
             methods=["GET"],
             response_model=None,
         )
@@ -149,20 +144,14 @@
         self.router.add_api_route(
             "/api/v1/collections/{collection_id}/query",
             self.get_nearest_neighbors,
             methods=["POST"],
             response_model=None,
         )
         self.router.add_api_route(
-            "/api/v1/collections/{collection_name}/create_index",
-            self.create_index,
-            methods=["POST"],
-            response_model=None,
-        )
-        self.router.add_api_route(
             "/api/v1/collections/{collection_name}",
             self.get_collection,
             methods=["GET"],
             response_model=None,
         )
         self.router.add_api_route(
             "/api/v1/collections/{collection_id}",
@@ -222,15 +211,14 @@
         try:
             result = self._api._add(
                 collection_id=_uuid(collection_id),
                 embeddings=add.embeddings,
                 metadatas=add.metadatas,
                 documents=add.documents,
                 ids=add.ids,
-                increment_index=add.increment_index,
             )
         except InvalidDimensionException as e:
             raise HTTPException(status_code=500, detail=str(e))
         return result
 
     def update(self, collection_id: str, add: UpdateEmbedding) -> None:
         return self._api._update(
@@ -244,15 +232,14 @@
     def upsert(self, collection_id: str, upsert: AddEmbedding) -> None:
         return self._api._upsert(
             collection_id=_uuid(collection_id),
             ids=upsert.ids,
             embeddings=upsert.embeddings,
             documents=upsert.documents,
             metadatas=upsert.metadatas,
-            increment_index=upsert.increment_index,
         )
 
     def get(self, collection_id: str, get: GetEmbedding) -> GetResult:
         return self._api._get(
             collection_id=_uuid(collection_id),
             ids=get.ids,
             where=get.where,
@@ -285,13 +272,7 @@
             where=query.where,  # type: ignore
             where_document=query.where_document,  # type: ignore
             query_embeddings=query.query_embeddings,
             n_results=query.n_results,
             include=query.include,
         )
         return nnresult
-
-    def raw_sql(self, raw_sql: RawSql) -> pd.DataFrame:
-        return self._api.raw_sql(raw_sql.raw_sql)
-
-    def create_index(self, collection_name: str) -> bool:
-        return self._api.create_index(collection_name)
```

### Comparing `chromadb-0.4.3/chromadb/server/fastapi/types.py` & `chromadb-0.4.4/chromadb/server/fastapi/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,23 +10,21 @@
     # Pydantic doesn't handle Union types cleanly like Embeddings which has
     # Union[int, float] so we use Any here to ensure data is parsed
     # to its original type.
     embeddings: Optional[List[Any]] = None
     metadatas: Optional[List[Dict[Any, Any]]] = None
     documents: Optional[List[str]] = None
     ids: List[str]
-    increment_index: bool = True
 
 
 class UpdateEmbedding(BaseModel):  # type: ignore
     embeddings: Optional[List[Any]] = None
     metadatas: Optional[List[Dict[Any, Any]]] = None
     documents: Optional[List[str]] = None
     ids: List[str]
-    increment_index: bool = True
 
 
 class QueryEmbedding(BaseModel):  # type: ignore
     # TODO: Pydantic doesn't bode well with recursive types so we use generic Dicts
     # for Where and WhereDocument. This is not ideal, but it works for now since
     # there is a lot of downstream validation.
     where: Optional[Dict[Any, Any]] = {}
@@ -42,18 +40,14 @@
     where_document: Optional[Dict[Any, Any]] = None
     sort: Optional[str] = None
     limit: Optional[int] = None
     offset: Optional[int] = None
     include: Include = ["metadatas", "documents"]
 
 
-class RawSql(BaseModel):  # type: ignore
-    raw_sql: str
-
-
 class DeleteEmbedding(BaseModel):  # type: ignore
     ids: Optional[List[str]] = None
     where: Optional[Dict[Any, Any]] = None
     where_document: Optional[Dict[Any, Any]] = None
 
 
 class CreateCollection(BaseModel):  # type: ignore
```

### Comparing `chromadb-0.4.3/chromadb/telemetry/__init__.py` & `chromadb-0.4.4/chromadb/telemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/chromadb/telemetry/events.py` & `chromadb-0.4.4/chromadb/telemetry/events.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/chromadb/telemetry/posthog.py` & `chromadb-0.4.4/chromadb/telemetry/posthog.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/chromadb/test/conftest.py` & `chromadb-0.4.4/chromadb/test/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 root_logger.setLevel(logging.DEBUG)  # This will only run when testing
 
 
 logger = logging.getLogger(__name__)
 
 hypothesis.settings.register_profile(
     "dev",
-    deadline=30000,
+    deadline=45000,
     suppress_health_check=[
         hypothesis.HealthCheck.data_too_large,
         hypothesis.HealthCheck.large_base_example,
         hypothesis.HealthCheck.function_scoped_fixture,
     ],
 )
 hypothesis.settings.load_profile(os.getenv("HYPOTHESIS_PROFILE", "dev"))
```

### Comparing `chromadb-0.4.3/chromadb/test/db/test_base.py` & `chromadb-0.4.4/chromadb/test/db/test_base.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/chromadb/test/db/test_migrations.py` & `chromadb-0.4.4/chromadb/test/db/test_migrations.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/chromadb/test/db/test_system.py` & `chromadb-0.4.4/chromadb/test/db/test_system.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/chromadb/test/ingest/test_producer_consumer.py` & `chromadb-0.4.4/chromadb/test/ingest/test_producer_consumer.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/chromadb/test/property/invariants.py` & `chromadb-0.4.4/chromadb/test/property/invariants.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,25 +64,32 @@
     normalized_record_set = wrap_all(record_set)
     assert count == len(normalized_record_set["ids"])
 
 
 def _field_matches(
     collection: Collection,
     normalized_record_set: NormalizedRecordSet,
-    field_name: Union[Literal["documents"], Literal["metadatas"]],
+    field_name: Union[
+        Literal["documents"], Literal["metadatas"], Literal["embeddings"]
+    ],
 ) -> None:
     """
     The actual embedding field is equal to the expected field
     field_name: one of [documents, metadatas]
     """
     result = collection.get(ids=normalized_record_set["ids"], include=[field_name])
     # The test_out_of_order_ids test fails because of this in test_add.py
     # Here we sort by the ids to match the input order
     embedding_id_to_index = {id: i for i, id in enumerate(normalized_record_set["ids"])}
     actual_field = result[field_name]
+
+    if len(normalized_record_set["ids"]) == 0:
+        assert isinstance(actual_field, list) and len(actual_field) == 0
+        return
+
     # This assert should never happen, if we include metadatas/documents it will be
     # [None, None..] if there is no metadata. It will not be just None.
     assert actual_field is not None
     sorted_field = sorted(
         enumerate(actual_field),
         key=lambda index_and_field_value: embedding_id_to_index[
             result["ids"][index_and_field_value[0]]
@@ -91,15 +98,18 @@
     field_values = [field_value for _, field_value in sorted_field]
 
     expected_field = normalized_record_set[field_name]
     if expected_field is None:
         # Since an RecordSet is the user input, we need to convert the documents to
         # a List since thats what the API returns -> none per entry
         expected_field = [None] * len(normalized_record_set["ids"])  # type: ignore
-    assert field_values == expected_field
+    if field_name == "embeddings":
+        assert np.allclose(np.array(field_values), np.array(expected_field))
+    else:
+        assert field_values == expected_field
 
 
 def ids_match(collection: Collection, record_set: RecordSet) -> None:
     """The actual embedding ids is equal to the expected ids"""
     normalized_record_set = wrap_all(record_set)
     actual_ids = collection.get(ids=normalized_record_set["ids"], include=[])["ids"]
     # The test_out_of_order_ids test fails because of this in test_add.py
@@ -117,14 +127,20 @@
 
 def documents_match(collection: Collection, record_set: RecordSet) -> None:
     """The actual embedding documents is equal to the expected documents"""
     normalized_record_set = wrap_all(record_set)
     _field_matches(collection, normalized_record_set, "documents")
 
 
+def embeddings_match(collection: Collection, record_set: RecordSet) -> None:
+    """The actual embedding documents is equal to the expected documents"""
+    normalized_record_set = wrap_all(record_set)
+    _field_matches(collection, normalized_record_set, "embeddings")
+
+
 def no_duplicates(collection: Collection) -> None:
     ids = collection.get()["ids"]
     assert len(ids) == len(set(ids))
 
 
 def _exact_distances(
     query: types.Embeddings,
```

### Comparing `chromadb-0.4.3/chromadb/test/property/strategies.py` & `chromadb-0.4.4/chromadb/test/property/strategies.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,18 +106,19 @@
     allow_infinity=False,
     allow_nan=False,
     allow_subnormal=False,
     min_value=-1e6,
     max_value=1e6,
 )  # TODO: handle infinity and NAN
 
-safe_values: List[SearchStrategy[Union[int, float, str]]] = [
+safe_values: List[SearchStrategy[Union[int, float, str, bool]]] = [
     safe_text,
     safe_integers,
     safe_floats,
+    st.booleans(),
 ]
 
 
 def one_or_both(
     strategy_a: st.SearchStrategy[Any], strategy_b: st.SearchStrategy[Any]
 ) -> st.SearchStrategy[Any]:
     return st.one_of(
@@ -453,15 +454,15 @@
 
     known_keys = sorted(collection.known_metadata_keys.keys())
 
     key = draw(st.sampled_from(known_keys))
     value = collection.known_metadata_keys[key]
 
     legal_ops: List[Optional[str]] = [None, "$eq", "$ne"]
-    if not isinstance(value, str):
+    if not isinstance(value, str) and not isinstance(value, bool):
         legal_ops.extend(["$gt", "$lt", "$lte", "$gte"])
     if isinstance(value, float):
         # Add or subtract a small number to avoid floating point rounding errors
         value = value + draw(st.sampled_from([1e-6, -1e-6]))
 
     op: types.WhereOperator = draw(st.sampled_from(legal_ops))
```

### Comparing `chromadb-0.4.3/chromadb/test/property/test_add.py` & `chromadb-0.4.4/chromadb/test/property/test_add.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/chromadb/test/property/test_collections.py` & `chromadb-0.4.4/chromadb/test/property/test_collections.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/chromadb/test/property/test_cross_version_persist.py` & `chromadb-0.4.4/chromadb/test/property/test_cross_version_persist.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from multiprocessing.connection import Connection
 import sys
 import os
 import shutil
 import subprocess
 import tempfile
 from types import ModuleType
-from typing import Generator, List, Tuple
+from typing import Generator, List, Tuple, Dict, Any, Callable
 from hypothesis import given, settings
 import hypothesis.strategies as st
 import pytest
 import json
 from urllib import request
 from chromadb import config
 from chromadb.api import API
@@ -32,14 +32,59 @@
     versions = list(data["releases"].keys())
     # Older versions on pypi contain "devXYZ" suffixes
     versions = [v for v in versions if version_re.match(v)]
     versions.sort(key=packaging_version.Version)
     return [MINIMUM_VERSION, versions[-1]]
 
 
+def _bool_to_int(metadata: Dict[str, Any]) -> Dict[str, Any]:
+    metadata.update((k, 1) for k, v in metadata.items() if v is True)
+    metadata.update((k, 0) for k, v in metadata.items() if v is False)
+    return metadata
+
+
+def _patch_boolean_metadata(
+    collection: strategies.Collection, embeddings: strategies.RecordSet
+) -> None:
+    # Since the old version does not support boolean value metadata, we will convert
+    # boolean value metadata to int
+    collection_metadata = collection.metadata
+    if collection_metadata is not None:
+        _bool_to_int(collection_metadata)
+
+    if embeddings["metadatas"] is not None:
+        if isinstance(embeddings["metadatas"], list):
+            for metadata in embeddings["metadatas"]:
+                if metadata is not None and isinstance(metadata, dict):
+                    _bool_to_int(metadata)
+        elif isinstance(embeddings["metadatas"], dict):
+            metadata = embeddings["metadatas"]
+            _bool_to_int(metadata)
+
+
+version_patches: List[
+    Tuple[str, Callable[[strategies.Collection, strategies.RecordSet], None]]
+] = [
+    ("0.4.3", _patch_boolean_metadata),
+]
+
+
+def patch_for_version(
+    version: str, collection: strategies.Collection, embeddings: strategies.RecordSet
+) -> None:
+    """Override aspects of the collection and embeddings, before testing, to account for
+    breaking changes in old versions."""
+
+    for patch_version, patch in version_patches:
+        if packaging_version.Version(version) <= packaging_version.Version(
+            patch_version
+        ):
+            patch(collection, embeddings)
+
+
 def configurations(versions: List[str]) -> List[Tuple[str, Settings]]:
     return [
         (
             version,
             Settings(
                 chroma_api_impl="chromadb.api.segment.SegmentAPI",
                 chroma_sysdb_impl="chromadb.db.impl.sqlite.SqliteDB",
@@ -69,15 +114,15 @@
     yield configuration
     # Cleanup the installed version
     path = get_path_to_version_install(version)
     shutil.rmtree(path)
     # Cleanup the persisted data
     data_path = configuration[1].persist_directory
     if os.path.exists(data_path):
-        shutil.rmtree(data_path)
+        shutil.rmtree(data_path, ignore_errors=True)
 
 
 def get_path_to_version_install(version: str) -> str:
     return base_install_dir + "/" + version
 
 
 def get_path_to_version_library(version: str) -> str:
@@ -166,18 +211,16 @@
         assert coll.count() == len(check_embeddings["embeddings"] or [])
         # Check ids
         result = coll.get()
         actual_ids = result["ids"]
         embedding_id_to_index = {id: i for i, id in enumerate(check_embeddings["ids"])}
         actual_ids = sorted(actual_ids, key=lambda id: embedding_id_to_index[id])
         assert actual_ids == check_embeddings["ids"]
-
         # Shutdown system
         system.stop()
-
     except Exception as e:
         conn.send(e)
         raise e
 
 
 # Since we can't pickle the embedding function, we always generate record sets with embeddings
 collection_st: st.SearchStrategy[strategies.Collection] = st.shared(
@@ -195,28 +238,29 @@
     collection_strategy: strategies.Collection,
     embeddings_strategy: strategies.RecordSet,
 ) -> None:
     # Test backwards compatibility
     # For the current version, ensure that we can load a collection from
     # the previous versions
     version, settings = version_settings
-
     # The strategies can generate metadatas of malformed inputs. Other tests
     # will error check and cover these cases to make sure they error. Here we
     # just convert them to valid values since the error cases are already tested
     if embeddings_strategy["metadatas"] == {}:
         embeddings_strategy["metadatas"] = None
     if embeddings_strategy["metadatas"] is not None and isinstance(
         embeddings_strategy["metadatas"], list
     ):
         embeddings_strategy["metadatas"] = [
             m if m is None or len(m) > 0 else None  # type: ignore
             for m in embeddings_strategy["metadatas"]
         ]
 
+    patch_for_version(version, collection_strategy, embeddings_strategy)
+
     # Can't pickle a function, and we won't need them
     collection_strategy.embedding_function = None
     collection_strategy.known_metadata_keys = {}
 
     # Run the task in a separate process to avoid polluting the current process
     # with the old version. Using spawn instead of fork to avoid sharing the
     # current process memory which would cause the old version to be loaded
@@ -229,14 +273,16 @@
     p.start()
     p.join()
 
     if conn1.poll():
         e = conn1.recv()
         raise e
 
+    p.close()
+
     # Switch to the current version (local working directory) and check the invariants
     # are preserved for the collection
     system = config.System(settings)
     api = system.instance(API)
     system.start()
     coll = api.get_collection(
         name=collection_strategy.name,
```

### Comparing `chromadb-0.4.3/chromadb/test/property/test_embeddings.py` & `chromadb-0.4.4/chromadb/test/property/test_embeddings.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,14 +206,21 @@
         invariants.ann_accuracy(
             collection=self.collection,
             record_set=cast(strategies.RecordSet, self.record_set_state),
             min_recall=0.95,
             embedding_function=self.embedding_function,
         )
 
+    @invariant()
+    def fields_match(self) -> None:
+        self.record_set_state = cast(strategies.RecordSet, self.record_set_state)
+        invariants.embeddings_match(self.collection, self.record_set_state)
+        invariants.metadatas_match(self.collection, self.record_set_state)
+        invariants.documents_match(self.collection, self.record_set_state)
+
     def _upsert_embeddings(self, record_set: strategies.RecordSet) -> None:
         normalized_record_set: strategies.NormalizedRecordSet = invariants.wrap_all(
             record_set
         )
         for idx, id in enumerate(normalized_record_set["ids"]):
             # Update path
             if id in self.record_set_state["ids"]:
@@ -332,14 +339,24 @@
     )
     for field in fields:
         field_results = results[field]
         assert field_results is not None
         assert all([len(result) == 0 for result in field_results])
 
 
+def test_get_non_existent(api: API) -> None:
+    api.reset()
+    coll = api.create_collection(name="foo")
+    result = coll.get(ids=["a"], include=["documents", "metadatas", "embeddings"])
+    assert len(result["ids"]) == 0
+    assert len(result["metadatas"]) == 0
+    assert len(result["documents"]) == 0
+    assert len(result["embeddings"]) == 0
+
+
 # TODO: Use SQL escaping correctly internally
 @pytest.mark.xfail(reason="We don't properly escape SQL internally, causing problems")
 def test_escape_chars_in_ids(api: API) -> None:
     api.reset()
     id = "\x1f"
     coll = api.create_collection(name="foo")
     coll.add(ids=[id], embeddings=[[0.0]])
```

### Comparing `chromadb-0.4.3/chromadb/test/property/test_filtering.py` & `chromadb-0.4.4/chromadb/test/property/test_filtering.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,20 @@
 
 def _filter_where_clause(clause: Where, metadata: Metadata) -> bool:
     """Return true if the where clause is true for the given metadata map"""
 
     key, expr = list(clause.items())[0]
 
     # Handle the shorthand for equal: {key: val} where val is a simple value
-    if isinstance(expr, str) or isinstance(expr, int) or isinstance(expr, float):
+    if (
+        isinstance(expr, str)
+        or isinstance(expr, bool)
+        or isinstance(expr, int)
+        or isinstance(expr, float)
+    ):
         return _filter_where_clause({key: {"$eq": expr}}, metadata)
 
     # expr is a list of clauses
     if key == "$and":
         assert isinstance(expr, list)
         return all(_filter_where_clause(clause, metadata) for clause in expr)
 
@@ -149,15 +154,15 @@
     caplog, api: API, collection: strategies.Collection, record_set, filters
 ) -> None:
     caplog.set_level(logging.ERROR)
 
     api.reset()
     coll = api.create_collection(
         name=collection.name,
-        metadata=collection.metadata,
+        metadata=collection.metadata,  # type: ignore
         embedding_function=collection.embedding_function,
     )
 
     if not invariants.is_metadata_valid(invariants.wrap_all(record_set)):
         with pytest.raises(Exception):
             coll.add(**record_set)
         return
@@ -269,15 +274,14 @@
     )
     assert res["ids"] == [[], []]
     assert res["embeddings"] is None
     assert res["distances"] == [[], []]
     assert res["metadatas"] == [[], []]
 
 
-@pytest.mark.xfail(reason="Boolean metadata is not supported yet")
 def test_boolean_metadata(api: API) -> None:
     """Test that metadata with boolean values is correctly filtered"""
     api.reset()
     coll = api.create_collection(name="test")
 
     test_ids: IDs = ["1", "2", "3"]
     test_embeddings: Embeddings = [[1, 1], [2, 2], [3, 3]]
```

### Comparing `chromadb-0.4.3/chromadb/test/property/test_persist.py` & `chromadb-0.4.4/chromadb/test/property/test_persist.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from multiprocessing.connection import Connection
 from typing import Generator, Callable
 from hypothesis import given
 import hypothesis.strategies as st
 import pytest
 import chromadb
 from chromadb.api import API
-from chromadb.config import Settings
+from chromadb.config import Settings, System
 import chromadb.test.property.strategies as strategies
 import chromadb.test.property.invariants as invariants
 from chromadb.test.property.test_embeddings import (
     EmbeddingStateMachine,
     EmbeddingStateMachineStates,
     collection_st as embedding_collection_st,
     trace,
@@ -33,30 +33,30 @@
         chroma_api_impl="chromadb.api.segment.SegmentAPI",
         chroma_sysdb_impl="chromadb.db.impl.sqlite.SqliteDB",
         chroma_producer_impl="chromadb.db.impl.sqlite.SqliteDB",
         chroma_consumer_impl="chromadb.db.impl.sqlite.SqliteDB",
         chroma_segment_manager_impl="chromadb.segment.impl.manager.local.LocalSegmentManager",
         allow_reset=True,
         is_persistent=True,
-        persist_directory=tempfile.gettempdir() + "/tests",
+        persist_directory=tempfile.mkdtemp(),
     ),
 ]
 
 
 @pytest.fixture(scope="module", params=configurations)
 def settings(request: pytest.FixtureRequest) -> Generator[Settings, None, None]:
     configuration = request.param
     save_path = configuration.persist_directory
     # Create if it doesn't exist
     if not os.path.exists(save_path):
         os.makedirs(save_path, exist_ok=True)
     yield configuration
     # Remove if it exists
     if os.path.exists(save_path):
-        shutil.rmtree(save_path)
+        shutil.rmtree(save_path, ignore_errors=True)
 
 
 collection_st = st.shared(
     strategies.collections(with_hnsw_params=True, with_persistent_hnsw_params=True),
     key="coll",
 )
 
@@ -66,15 +66,18 @@
     embeddings_strategy=strategies.recordsets(collection_st),
 )
 def test_persist(
     settings: Settings,
     collection_strategy: strategies.Collection,
     embeddings_strategy: strategies.RecordSet,
 ) -> None:
-    api_1 = chromadb.Client(settings)
+    system_1 = System(settings)
+    api_1 = system_1.instance(API)
+    system_1.start()
+
     api_1.reset()
     coll = api_1.create_collection(
         name=collection_strategy.name,
         metadata=collection_strategy.metadata,
         embedding_function=collection_strategy.embedding_function,
     )
 
@@ -91,49 +94,63 @@
     invariants.ids_match(coll, embeddings_strategy)
     invariants.ann_accuracy(
         coll,
         embeddings_strategy,
         embedding_function=collection_strategy.embedding_function,
     )
 
+    system_1.stop()
     del api_1
+    del system_1
+
+    system_2 = System(settings)
+    api_2 = system_2.instance(API)
+    system_2.start()
 
-    api_2 = chromadb.Client(settings)
     coll = api_2.get_collection(
         name=collection_strategy.name,
         embedding_function=collection_strategy.embedding_function,
     )
     invariants.count(coll, embeddings_strategy)
     invariants.metadatas_match(coll, embeddings_strategy)
     invariants.documents_match(coll, embeddings_strategy)
     invariants.ids_match(coll, embeddings_strategy)
     invariants.ann_accuracy(
         coll,
         embeddings_strategy,
         embedding_function=collection_strategy.embedding_function,
     )
 
+    system_2.stop()
+    del api_2
+    del system_2
+
 
 def load_and_check(
     settings: Settings,
     collection_name: str,
     record_set: strategies.RecordSet,
     conn: Connection,
 ) -> None:
     try:
-        api = chromadb.Client(settings)
+        system = System(settings)
+        api = system.instance(API)
+        system.start()
+
         coll = api.get_collection(
             name=collection_name,
             embedding_function=strategies.not_implemented_embedding_function(),
         )
         invariants.count(coll, record_set)
         invariants.metadatas_match(coll, record_set)
         invariants.documents_match(coll, record_set)
         invariants.ids_match(coll, record_set)
         invariants.ann_accuracy(coll, record_set)
+
+        system.stop()
     except Exception as e:
         conn.send(e)
         raise e
 
 
 class PersistEmbeddingsStateMachineStates(EmbeddingStateMachineStates):
     persist = "persist"
@@ -184,14 +201,16 @@
         p.start()
         p.join()
 
         if conn1.poll():
             e = conn1.recv()
             raise e
 
+        p.close()
+
     def on_state_change(self, new_state: str) -> None:
         if new_state == PersistEmbeddingsStateMachineStates.persist:
             self.last_persist_delay = 10
         else:
             self.last_persist_delay -= 1
 
     def teardown(self) -> None:
```

### Comparing `chromadb-0.4.3/chromadb/test/segment/test_metadata.py` & `chromadb-0.4.4/chromadb/test/segment/test_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,21 +56,28 @@
     yield next(request.param())
 
 
 @pytest.fixture(scope="function")
 def sample_embeddings() -> Iterator[SubmitEmbeddingRecord]:
     def create_record(i: int) -> SubmitEmbeddingRecord:
         vector = [i + i * 0.1, i + 1 + i * 0.1]
-        metadata: Optional[Dict[str, Union[str, int, float]]]
+        metadata: Optional[Dict[str, Union[str, int, float, bool]]]
         if i == 0:
             metadata = None
         else:
-            metadata = {"str_key": f"value_{i}", "int_key": i, "float_key": i + i * 0.1}
+            metadata = {
+                "str_key": f"value_{i}",
+                "int_key": i,
+                "float_key": i + i * 0.1,
+                "bool_key": True,
+            }
             if i % 3 == 0:
                 metadata["div_by_three"] = "true"
+            if i % 2 == 0:
+                metadata["bool_key"] = False
             metadata["chroma:document"] = _build_document(i)
 
         record = SubmitEmbeddingRecord(
             id=f"embedding_{i}",
             embedding=vector,
             encoding=ScalarEncoding.FLOAT32,
             metadata=metadata,
@@ -172,14 +179,21 @@
         seq_ids.append(producer.submit_embedding(topic, e))
 
     segment = SqliteMetadataSegment(system, segment_definition)
     segment.start()
 
     sync(segment, seq_ids[-1])
 
+    # get with bool key
+    result = segment.get_metadata(where={"bool_key": True})
+    assert len(result) == 5
+
+    result = segment.get_metadata(where={"bool_key": False})
+    assert len(result) == 4
+
     # Get all records
     results = segment.get_metadata()
     assert seq_ids == [r["seq_id"] for r in results]
     assert_equiv_records(embeddings, results)
 
     # get by ID
     result = segment.get_metadata(ids=[e["id"] for e in embeddings[0:5]])
```

### Comparing `chromadb-0.4.3/chromadb/test/segment/test_vector.py` & `chromadb-0.4.4/chromadb/test/segment/test_vector.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/chromadb/test/test_api.py` & `chromadb-0.4.4/chromadb/test/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,51 +2,59 @@
 import chromadb
 from chromadb.api.types import QueryResult
 from chromadb.config import Settings
 import chromadb.server.fastapi
 import pytest
 import tempfile
 import numpy as np
+import os
+import shutil
 from datetime import datetime, timedelta
 from chromadb.utils.embedding_functions import (
     DefaultEmbeddingFunction,
 )
 
+persist_dir = tempfile.mkdtemp()
+
 
 @pytest.fixture
 def local_persist_api():
-    return chromadb.Client(
+    yield chromadb.Client(
         Settings(
             chroma_api_impl="chromadb.api.segment.SegmentAPI",
             chroma_sysdb_impl="chromadb.db.impl.sqlite.SqliteDB",
             chroma_producer_impl="chromadb.db.impl.sqlite.SqliteDB",
             chroma_consumer_impl="chromadb.db.impl.sqlite.SqliteDB",
             chroma_segment_manager_impl="chromadb.segment.impl.manager.local.LocalSegmentManager",
             allow_reset=True,
             is_persistent=True,
-            persist_directory=tempfile.gettempdir(),
+            persist_directory=persist_dir,
         ),
     )
+    if os.path.exists(persist_dir):
+        shutil.rmtree(persist_dir, ignore_errors=True)
 
 
 # https://docs.pytest.org/en/6.2.x/fixture.html#fixtures-can-be-requested-more-than-once-per-test-return-values-are-cached
 @pytest.fixture
 def local_persist_api_cache_bust():
-    return chromadb.Client(
+    yield chromadb.Client(
         Settings(
             chroma_api_impl="chromadb.api.segment.SegmentAPI",
             chroma_sysdb_impl="chromadb.db.impl.sqlite.SqliteDB",
             chroma_producer_impl="chromadb.db.impl.sqlite.SqliteDB",
             chroma_consumer_impl="chromadb.db.impl.sqlite.SqliteDB",
             chroma_segment_manager_impl="chromadb.segment.impl.manager.local.LocalSegmentManager",
             allow_reset=True,
             is_persistent=True,
-            persist_directory=tempfile.gettempdir(),
+            persist_directory=persist_dir,
         ),
     )
+    if os.path.exists(persist_dir):
+        shutil.rmtree(persist_dir, ignore_errors=True)
 
 
 def approx_equal(a, b, tolerance=1e-6) -> bool:
     return abs(a - b) < tolerance
 
 
 def vector_approx_equal(a, b, tolerance: float = 1e-6) -> bool:
@@ -224,15 +232,14 @@
     assert len(api.list_collections()) == 0
 
 
 def test_get_nearest_neighbors(api):
     api.reset()
     collection = api.create_collection("testspace")
     collection.add(**batch_records)
-    # assert api.create_index(collection_name="testspace") # default is auto now
 
     nn = collection.query(
         query_embeddings=[1.1, 2.3, 3.2],
         n_results=1,
         where={},
         include=["embeddings", "documents", "metadatas", "distances"],
     )
@@ -355,53 +362,23 @@
 def test_increment_index_on(api):
     api.reset()
     collection = api.create_collection("testspace")
     collection.add(**batch_records)
     assert collection.count() == 2
 
     # increment index
-    # collection.create_index(index_type="hnsw", index_params={"M": 16, "efConstruction": 200})
-    nn = collection.query(
-        query_embeddings=[[1.1, 2.3, 3.2]],
-        n_results=1,
-        include=["embeddings", "documents", "metadatas", "distances"],
-    )
-    for key in nn.keys():
-        assert len(nn[key]) == 1
-
-
-def test_increment_index_off(api):
-    api.reset()
-    collection = api.create_collection("testspace")
-    collection.add(**batch_records, increment_index=False)
-    assert collection.count() == 2
-
-    # incremental index
-    collection.create_index()
     nn = collection.query(
         query_embeddings=[[1.1, 2.3, 3.2]],
         n_results=1,
         include=["embeddings", "documents", "metadatas", "distances"],
     )
     for key in nn.keys():
         assert len(nn[key]) == 1
 
 
-def skipping_indexing_will_fail(api):
-    api.reset()
-    collection = api.create_collection("testspace")
-    collection.add(**batch_records, increment_index=False)
-    assert collection.count() == 2
-
-    # incremental index
-    with pytest.raises(Exception) as e:
-        collection.query(query_embeddings=[[1.1, 2.3, 3.2]], n_results=1)
-    assert str(e.value).__contains__("index not found")
-
-
 def test_add_a_collection(api):
     api.reset()
     api.create_collection("testspace")
 
     # get collection does not throw an error
     collection = api.get_collection("testspace")
     assert collection.name == "testspace"
```

### Comparing `chromadb-0.4.3/chromadb/test/test_chroma.py` & `chromadb-0.4.4/chromadb/test/test_chroma.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/chromadb/test/test_client.py` & `chromadb-0.4.4/chromadb/test/test_client.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/chromadb/test/test_config.py` & `chromadb-0.4.4/chromadb/test/test_config.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/chromadb/test/test_multithreaded.py` & `chromadb-0.4.4/chromadb/test/test_multithreaded.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/chromadb/test/utils/test_messagid.py` & `chromadb-0.4.4/chromadb/test/utils/test_messagid.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/chromadb/types.py` & `chromadb-0.4.4/chromadb/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional, Union, Sequence, Dict, Mapping, List
 from typing_extensions import Literal, TypedDict, TypeVar
 from uuid import UUID
 from enum import Enum
 
-Metadata = Mapping[str, Union[str, int, float]]
-UpdateMetadata = Mapping[str, Union[int, float, str, None]]
+Metadata = Mapping[str, Union[str, int, float, bool]]
+UpdateMetadata = Mapping[str, Union[int, float, str, bool, None]]
 
 # Namespaced Names are mechanically just strings, but we use this type to indicate that
 # the intent is for the value to be globally unique and semantically meaningful.
 NamespacedName = str
 
 
 class ScalarEncoding(Enum):
@@ -95,28 +95,28 @@
 class VectorQuery(TypedDict):
     """A KNN/ANN query"""
 
     vectors: Sequence[Vector]
     k: int
     allowed_ids: Optional[Sequence[str]]
     include_embeddings: bool
-    options: Optional[Dict[str, Union[str, int, float]]]
+    options: Optional[Dict[str, Union[str, int, float, bool]]]
 
 
 class VectorQueryResult(TypedDict):
     """A KNN/ANN query result"""
 
     id: str
     seq_id: SeqId
     distance: float
     embedding: Optional[Vector]
 
 
 # Metadata Query Grammar
-LiteralValue = Union[str, int, float]
+LiteralValue = Union[str, int, float, bool]
 LogicalOperator = Union[Literal["$and"], Literal["$or"]]
 WhereOperator = Union[
     Literal["$gt"],
     Literal["$gte"],
     Literal["$lt"],
     Literal["$lte"],
     Literal["$ne"],
```

### Comparing `chromadb-0.4.3/chromadb/utils/distance_functions.py` & `chromadb-0.4.4/chromadb/utils/distance_functions.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/chromadb/utils/embedding_functions.py` & `chromadb-0.4.4/chromadb/utils/embedding_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,30 +64,33 @@
     def __init__(
         self,
         api_key: Optional[str] = None,
         model_name: str = "text-embedding-ada-002",
         organization_id: Optional[str] = None,
         api_base: Optional[str] = None,
         api_type: Optional[str] = None,
+        api_version: Optional[str] = None,
     ):
         """
         Initialize the OpenAIEmbeddingFunction.
-
         Args:
             api_key (str, optional): Your API key for the OpenAI API. If not
                 provided, it will raise an error to provide an OpenAI API key.
             organization_id(str, optional): The OpenAI organization ID if applicable
             model_name (str, optional): The name of the model to use for text
                 embeddings. Defaults to "text-embedding-ada-002".
             api_base (str, optional): The base path for the API. If not provided,
                 it will use the base path for the OpenAI API. This can be used to
                 point to a different deployment, such as an Azure deployment.
             api_type (str, optional): The type of the API deployment. This can be
                 used to specify a different deployment, such as 'azure'. If not
                 provided, it will use the default OpenAI deployment.
+            api_version (str, optional): The api version for the API. If not provided,
+                it will use the api version for the OpenAI API. This can be used to
+                point to a different deployment, such as an Azure deployment.
 
         """
         try:
             import openai
         except ImportError:
             raise ValueError(
                 "The openai python package is not installed. Please install it with `pip install openai`"
@@ -100,14 +103,17 @@
             raise ValueError(
                 "Please provide an OpenAI API key. You can get one at https://platform.openai.com/account/api-keys"
             )
 
         if api_base is not None:
             openai.api_base = api_base
 
+        if api_version is not None:
+            openai.api_version = api_version
+
         if api_type is not None:
             openai.api_type = api_type
 
         if organization_id is not None:
             openai.organization = organization_id
 
         self._client = openai.Embedding
@@ -144,28 +150,54 @@
         return [
             embeddings
             for embeddings in self._client.embed(texts=texts, model=self._model_name)
         ]
 
 
 class HuggingFaceEmbeddingFunction(EmbeddingFunction):
+    """
+    This class is used to get embeddings for a list of texts using the HuggingFace API.
+    It requires an API key and a model name. The default model name is "sentence-transformers/all-MiniLM-L6-v2".
+    """
+
     def __init__(
         self, api_key: str, model_name: str = "sentence-transformers/all-MiniLM-L6-v2"
     ):
+        """
+        Initialize the HuggingFaceEmbeddingFunction.
+
+        Args:
+            api_key (str): Your API key for the HuggingFace API.
+            model_name (str, optional): The name of the model to use for text embeddings. Defaults to "sentence-transformers/all-MiniLM-L6-v2".
+        """
         try:
             import requests
         except ImportError:
             raise ValueError(
                 "The requests python package is not installed. Please install it with `pip install requests`"
             )
         self._api_url = f"https://api-inference.huggingface.co/pipeline/feature-extraction/{model_name}"
         self._session = requests.Session()
         self._session.headers.update({"Authorization": f"Bearer {api_key}"})
 
     def __call__(self, texts: Documents) -> Embeddings:
+        """
+        Get the embeddings for a list of texts.
+
+        Args:
+            texts (Documents): A list of texts to get embeddings for.
+
+        Returns:
+            Embeddings: The embeddings for the texts.
+
+        Example:
+            >>> hugging_face = HuggingFaceEmbeddingFunction(api_key="your_api_key")
+            >>> texts = ["Hello, world!", "How are you?"]
+            >>> embeddings = hugging_face(texts)
+        """
         # Call HuggingFace Embedding API for each document
         return self._session.post(  # type: ignore
             self._api_url, json={"inputs": texts, "options": {"wait_for_model": True}}
         ).json()
 
 
 class InstructorEmbeddingFunction(EmbeddingFunction):
@@ -365,23 +397,27 @@
     # Follow API Quickstart for Google Vertex AI
     # https://cloud.google.com/vertex-ai/docs/generative-ai/start/quickstarts/api-quickstart
     # Information about the text embedding modules in Google Vertex AI
     # https://cloud.google.com/vertex-ai/docs/generative-ai/embeddings/get-text-embeddings
     def __init__(
         self,
         api_key: str,
-        model_name: str = "textembedding-gecko-001",
+        model_name: str = "textembedding-gecko",
         project_id: str = "cloud-large-language-models",
         region: str = "us-central1",
     ):
-        self._api_url = f"https://{region}-aiplatform.googleapis.com/v1/projects/{project_id}/locations/{region}/endpoints/{model_name}:predict"
+        self._api_url = f"https://{region}-aiplatform.googleapis.com/v1/projects/{project_id}/locations/{region}/publishers/goole/models/{model_name}:predict"
         self._session = requests.Session()
         self._session.headers.update({"Authorization": f"Bearer {api_key}"})
 
     def __call__(self, texts: Documents) -> Embeddings:
-        response = self._session.post(
-            self._api_url, json={"instances": [{"content": texts}]}
-        ).json()
 
-        if "predictions" in response:
-            return response["predictions"]
-        return []
+        embeddings = []
+        for text in texts:
+            response = self._session.post(
+                self._api_url, json={"instances": [{"content": text}]}
+            ).json()
+
+            if "predictions" in response:
+                embeddings.append(response["predictions"]["embeddings"]["values"])
+
+        return embeddings
```

### Comparing `chromadb-0.4.3/chromadb/utils/messageid.py` & `chromadb-0.4.4/chromadb/utils/messageid.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/chromadb/utils/read_write_lock.py` & `chromadb-0.4.4/chromadb/utils/read_write_lock.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/chromadb.egg-info/PKG-INFO` & `chromadb-0.4.4/chromadb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromadb
-Version: 0.4.3
+Version: 0.4.4
 Summary: Chroma.
 Author-email: Jeff Huber <jeff@trychroma.com>, Anton Troynikov <anton@trychroma.com>
 Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chromadb Version: 0.4.3 Summary: Chroma. Author-
+Metadata-Version: 2.1 Name: chromadb Version: 0.4.4 Summary: Chroma. Author-
 email: Jeff Huber
 trychroma.com>, Anton Troynikov
 trychroma.com> Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `chromadb-0.4.3/chromadb.egg-info/SOURCES.txt` & `chromadb-0.4.4/chromadb.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -28,19 +28,21 @@
 bin/docker_entrypoint.sh
 bin/generate_cloudformation.py
 bin/integration-test
 bin/test-package.sh
 bin/test-remote
 bin/test.py
 bin/version
+bin/windows_upgrade_sqlite.py
 bin/templates/docker-compose.yml
 chromadb/__init__.py
 chromadb/app.py
 chromadb/config.py
 chromadb/errors.py
+chromadb/py.typed
 chromadb/types.py
 chromadb.egg-info/PKG-INFO
 chromadb.egg-info/SOURCES.txt
 chromadb.egg-info/dependency_links.txt
 chromadb.egg-info/requires.txt
 chromadb.egg-info/top_level.txt
 chromadb/api/__init__.py
@@ -58,14 +60,15 @@
 chromadb/db/mixins/embeddings_queue.py
 chromadb/db/mixins/sysdb.py
 chromadb/experimental/density_relevance.ipynb
 chromadb/ingest/__init__.py
 chromadb/migrations/__init__.py
 chromadb/migrations/embeddings_queue/00001-embeddings.sqlite.sql
 chromadb/migrations/metadb/00001-embedding-metadata.sqlite.sql
+chromadb/migrations/metadb/00002-embedding-metadata.sqlite.sql
 chromadb/migrations/sysdb/00001-collections.sqlite.sql
 chromadb/migrations/sysdb/00002-segments.sqlite.sql
 chromadb/migrations/sysdb/00003-collection-dimension.sqlite.sql
 chromadb/segment/__init__.py
 chromadb/segment/impl/manager/local.py
 chromadb/segment/impl/metadata/sqlite.py
 chromadb/segment/impl/vector/batch.py
@@ -102,18 +105,21 @@
 chromadb/test/property/test_collections.py
 chromadb/test/property/test_cross_version_persist.py
 chromadb/test/property/test_embeddings.py
 chromadb/test/property/test_filtering.py
 chromadb/test/property/test_persist.py
 chromadb/test/segment/test_metadata.py
 chromadb/test/segment/test_vector.py
+chromadb/test/stress/test_many_collections.py
 chromadb/test/utils/test_messagid.py
 chromadb/utils/__init__.py
+chromadb/utils/delete_file.py
 chromadb/utils/distance_functions.py
 chromadb/utils/embedding_functions.py
+chromadb/utils/lru_cache.py
 chromadb/utils/messageid.py
 chromadb/utils/read_write_lock.py
 clients/js/.gitignore
 clients/js/.prettierignore
 clients/js/.prettierrc.json
 clients/js/DEVELOP.md
 clients/js/LICENSE
@@ -165,14 +171,15 @@
 clients/js/test/update.collection.test.ts
 clients/js/test/upsert.collections.test.ts
 clients/python/README.md
 clients/python/build_python_thin_client.sh
 clients/python/integration-test.sh
 clients/python/is_thin_client.py
 clients/python/pyproject.toml
+docs/CIP_Chroma_Improvment_Proposals.md
 examples/README.md
 examples/basic_functionality/alternative_embeddings.ipynb
 examples/basic_functionality/local_persistence.ipynb
 examples/basic_functionality/where_filtering.ipynb
 examples/deployments/google-cloud-compute/README.md
 examples/deployments/google-cloud-compute/chroma.tf
 examples/deployments/google-cloud-compute/main.tf
```

### Comparing `chromadb-0.4.3/clients/js/DEVELOP.md` & `chromadb-0.4.4/clients/js/DEVELOP.md`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/js/LICENSE` & `chromadb-0.4.4/clients/js/LICENSE`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/js/README.md` & `chromadb-0.4.4/clients/js/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/js/examples/browser/app.ts` & `chromadb-0.4.4/clients/js/examples/browser/app.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/js/examples/browser/index.html` & `chromadb-0.4.4/clients/js/examples/browser/index.html`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/js/examples/browser/yarn.lock` & `chromadb-0.4.4/clients/js/examples/browser/yarn.lock`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/js/examples/node/app.js` & `chromadb-0.4.4/clients/js/examples/node/app.js`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/js/examples/node/yarn.lock` & `chromadb-0.4.4/clients/js/examples/node/yarn.lock`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/js/genapi.sh` & `chromadb-0.4.4/clients/js/genapi.sh`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/js/package-lock.json` & `chromadb-0.4.4/clients/js/package-lock.json`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/js/package.json` & `chromadb-0.4.4/clients/js/package.json`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/js/src/ChromaClient.ts` & `chromadb-0.4.4/clients/js/src/ChromaClient.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/js/src/Collection.ts` & `chromadb-0.4.4/clients/js/src/Collection.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/js/src/embeddings/CohereEmbeddingFunction.ts` & `chromadb-0.4.4/clients/js/src/embeddings/CohereEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts` & `chromadb-0.4.4/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/js/src/embeddings/TransformersEmbeddingFunction.ts` & `chromadb-0.4.4/clients/js/src/embeddings/TransformersEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/js/src/embeddings/WebAIEmbeddingFunction.ts` & `chromadb-0.4.4/clients/js/src/embeddings/WebAIEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/js/src/generated/README.md` & `chromadb-0.4.4/clients/js/src/generated/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/js/src/generated/api.ts` & `chromadb-0.4.4/clients/js/src/generated/api.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/js/src/generated/configuration.ts` & `chromadb-0.4.4/clients/js/src/generated/configuration.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/js/src/generated/models.ts` & `chromadb-0.4.4/clients/js/src/generated/models.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/js/src/generated/runtime.ts` & `chromadb-0.4.4/clients/js/src/generated/runtime.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/js/src/types.ts` & `chromadb-0.4.4/clients/js/src/types.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/js/src/utils.ts` & `chromadb-0.4.4/clients/js/src/utils.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/js/test/add.collections.test.ts` & `chromadb-0.4.4/clients/js/test/add.collections.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/js/test/client.test.ts` & `chromadb-0.4.4/clients/js/test/client.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/js/test/collection.client.test.ts` & `chromadb-0.4.4/clients/js/test/collection.client.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/js/test/collection.test.ts` & `chromadb-0.4.4/clients/js/test/collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/js/test/delete.collection.test.ts` & `chromadb-0.4.4/clients/js/test/delete.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/js/test/get.collection.test.ts` & `chromadb-0.4.4/clients/js/test/get.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/js/test/peek.collection.test.ts` & `chromadb-0.4.4/clients/js/test/peek.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/js/test/query.collection.test.ts` & `chromadb-0.4.4/clients/js/test/query.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/js/test/update.collection.test.ts` & `chromadb-0.4.4/clients/js/test/update.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/js/test/upsert.collections.test.ts` & `chromadb-0.4.4/clients/js/test/upsert.collections.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/js/yarn.lock` & `chromadb-0.4.4/clients/js/yarn.lock`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/python/README.md` & `chromadb-0.4.4/clients/python/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/python/build_python_thin_client.sh` & `chromadb-0.4.4/clients/python/build_python_thin_client.sh`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/python/integration-test.sh` & `chromadb-0.4.4/clients/python/integration-test.sh`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/clients/python/pyproject.toml` & `chromadb-0.4.4/clients/python/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  'pandas >= 1.3',
   'requests >= 2.28',
   'pydantic >= 1.9',
   'numpy >= 1.21.6',
   'posthog >= 2.4.0',
   'typing_extensions >= 4.5.0',
   'overrides >= 7.3.1',
 ]
```

### Comparing `chromadb-0.4.3/docker-compose.test.yml` & `chromadb-0.4.4/docker-compose.test.yml`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/examples/README.md` & `chromadb-0.4.4/examples/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/examples/basic_functionality/alternative_embeddings.ipynb` & `chromadb-0.4.4/examples/basic_functionality/alternative_embeddings.ipynb`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/examples/basic_functionality/local_persistence.ipynb` & `chromadb-0.4.4/examples/basic_functionality/local_persistence.ipynb`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/examples/basic_functionality/where_filtering.ipynb` & `chromadb-0.4.4/examples/basic_functionality/where_filtering.ipynb`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/examples/deployments/google-cloud-compute/README.md` & `chromadb-0.4.4/examples/deployments/google-cloud-compute/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/examples/deployments/google-cloud-compute/chroma.tf` & `chromadb-0.4.4/examples/deployments/google-cloud-compute/chroma.tf`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/examples/deployments/google-cloud-compute/startup.sh` & `chromadb-0.4.4/examples/deployments/google-cloud-compute/startup.sh`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/examples/use_with/cohere/cohere_js.js` & `chromadb-0.4.4/examples/use_with/cohere/cohere_js.js`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/examples/use_with/cohere/cohere_python.ipynb` & `chromadb-0.4.4/examples/use_with/cohere/cohere_python.ipynb`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.3/pyproject.toml` & `chromadb-0.4.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  'pandas >= 1.3',
   'requests >= 2.28',
   'pydantic>=1.9,<2.0',
-  'chroma-hnswlib==0.7.1',
+  'chroma-hnswlib==0.7.2',
   'fastapi>=0.95.2, <0.100.0',
   'uvicorn[standard] >= 0.18.3',
   'numpy >= 1.21.6',
   'posthog >= 2.4.0',
   'typing_extensions >= 4.5.0',
   'pulsar-client>=3.1.0',
   'onnxruntime >= 1.14.1',
```

