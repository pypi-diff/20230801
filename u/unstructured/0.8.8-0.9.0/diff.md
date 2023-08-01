# Comparing `tmp/unstructured-0.8.8.tar.gz` & `tmp/unstructured-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured-0.8.8.tar", last modified: Tue Aug  1 06:14:14 2023, max compression
+gzip compressed data, was "unstructured-0.9.0.tar", last modified: Tue Aug  1 15:33:39 2023, max compression
```

## Comparing `unstructured-0.8.8.tar` & `unstructured-0.9.0.tar`

### file list

```diff
@@ -1,192 +1,191 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.225310 unstructured-0.8.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-08-01 06:14:04.000000 unstructured-0.8.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-08-01 06:14:04.000000 unstructured-0.8.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20050 2023-08-01 06:14:14.225310 unstructured-0.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16273 2023-08-01 06:14:04.000000 unstructured-0.8.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.205310 unstructured-0.8.8/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-01 06:14:05.000000 unstructured-0.8.8/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-01 06:14:05.000000 unstructured-0.8.8/requirements/huggingface.in
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-01 06:14:05.000000 unstructured-0.8.8/requirements/ingest-azure.in
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 06:14:05.000000 unstructured-0.8.8/requirements/ingest-box.in
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-01 06:14:05.000000 unstructured-0.8.8/requirements/ingest-discord.in
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 06:14:05.000000 unstructured-0.8.8/requirements/ingest-dropbox.in
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-01 06:14:05.000000 unstructured-0.8.8/requirements/ingest-gcs.in
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-01 06:14:05.000000 unstructured-0.8.8/requirements/ingest-github.in
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 06:14:05.000000 unstructured-0.8.8/requirements/ingest-gitlab.in
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-01 06:14:05.000000 unstructured-0.8.8/requirements/ingest-google-drive.in
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-01 06:14:05.000000 unstructured-0.8.8/requirements/ingest-onedrive.in
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-01 06:14:05.000000 unstructured-0.8.8/requirements/ingest-outlook.in
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 06:14:05.000000 unstructured-0.8.8/requirements/ingest-reddit.in
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 06:14:05.000000 unstructured-0.8.8/requirements/ingest-s3.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 06:14:05.000000 unstructured-0.8.8/requirements/ingest-slack.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 06:14:05.000000 unstructured-0.8.8/requirements/ingest-wikipedia.in
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-01 06:14:05.000000 unstructured-0.8.8/requirements/local-inference.in
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-01 06:14:14.225310 unstructured-0.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-08-01 06:14:05.000000 unstructured-0.8.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.205310 unstructured-0.8.8/test_unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:05.000000 unstructured-0.8.8/test_unstructured/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.205310 unstructured-0.8.8/test_unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:05.000000 unstructured-0.8.8/test_unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-08-01 06:14:05.000000 unstructured-0.8.8/test_unstructured/nlp/mock_nltk.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-01 06:14:05.000000 unstructured-0.8.8/test_unstructured/nlp/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-08-01 06:14:05.000000 unstructured-0.8.8/test_unstructured/nlp/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-08-01 06:14:05.000000 unstructured-0.8.8/test_unstructured/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.209310 unstructured-0.8.8/unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.209310 unstructured-0.8.8/unstructured/cleaners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/cleaners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/cleaners/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/cleaners/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/cleaners/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.209310 unstructured-0.8.8/unstructured/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/documents/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    15606 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/documents/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/documents/email_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    16209 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/documents/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/documents/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.209310 unstructured-0.8.8/unstructured/file_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/file_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/file_utils/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/file_utils/exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/file_utils/file_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    20754 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/file_utils/filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/file_utils/google_filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/file_utils/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.209310 unstructured-0.8.8/unstructured/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.209310 unstructured-0.8.8/unstructured/ingest/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.213310 unstructured-0.8.8/unstructured/ingest/cli/cmds/
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/biomed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/box.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/confluence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/dropbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/google_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/onedrive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/outlook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/wikipedia.py
--rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.213310 unstructured-0.8.8/unstructured/ingest/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     9521 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/biomed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/box.py
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/confluence.py
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/dropbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/google_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/onedrive.py
--rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/outlook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.213310 unstructured-0.8.8/unstructured/ingest/doc_processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/doc_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/doc_processor/generalized.py
--rw-r--r--   0 runner    (1001) docker     (123)    12492 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      143 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.217310 unstructured-0.8.8/unstructured/ingest/runner/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/biomed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/box.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/confluence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/dropbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/google_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/onedrive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/outlook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/wikipedia.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.217310 unstructured-0.8.8/unstructured/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.221310 unstructured-0.8.8/unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/nlp/english-words.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/nlp/english_words.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/nlp/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/nlp/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/nlp/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.221310 unstructured-0.8.8/unstructured/partition/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11739 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)    10544 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12489 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/docx.py
--rw-r--r--   0 runner    (1001) docker     (123)    14888 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/epub.py
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/md.py
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/msg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/odt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/org.py
--rw-r--r--   0 runner    (1001) docker     (123)    17794 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/ppt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/pptx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/rst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/rtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)    10744 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/text_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/tsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.225310 unstructured-0.8.8/unstructured/staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/staging/argilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/staging/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/staging/baseplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/staging/datasaur.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/staging/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/staging/label_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/staging/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/staging/prodigy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/staging/weaviate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.209310 unstructured-0.8.8/unstructured.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20050 2023-08-01 06:14:13.000000 unstructured-0.8.8/unstructured.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-08-01 06:14:14.000000 unstructured-0.8.8/unstructured.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 06:14:13.000000 unstructured-0.8.8/unstructured.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-01 06:14:13.000000 unstructured-0.8.8/unstructured.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-01 06:14:13.000000 unstructured-0.8.8/unstructured.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-01 06:14:13.000000 unstructured-0.8.8/unstructured.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:33:39.452572 unstructured-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-08-01 15:33:28.000000 unstructured-0.9.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-08-01 15:33:28.000000 unstructured-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20360 2023-08-01 15:33:39.456573 unstructured-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16273 2023-08-01 15:33:28.000000 unstructured-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:33:39.432571 unstructured-0.9.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-01 15:33:28.000000 unstructured-0.9.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-01 15:33:28.000000 unstructured-0.9.0/requirements/huggingface.in
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-01 15:33:28.000000 unstructured-0.9.0/requirements/ingest-azure.in
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 15:33:28.000000 unstructured-0.9.0/requirements/ingest-box.in
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-01 15:33:28.000000 unstructured-0.9.0/requirements/ingest-discord.in
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 15:33:28.000000 unstructured-0.9.0/requirements/ingest-dropbox.in
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-01 15:33:28.000000 unstructured-0.9.0/requirements/ingest-gcs.in
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-01 15:33:28.000000 unstructured-0.9.0/requirements/ingest-github.in
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 15:33:28.000000 unstructured-0.9.0/requirements/ingest-gitlab.in
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-01 15:33:28.000000 unstructured-0.9.0/requirements/ingest-google-drive.in
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-01 15:33:28.000000 unstructured-0.9.0/requirements/ingest-onedrive.in
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-01 15:33:28.000000 unstructured-0.9.0/requirements/ingest-outlook.in
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 15:33:28.000000 unstructured-0.9.0/requirements/ingest-reddit.in
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 15:33:28.000000 unstructured-0.9.0/requirements/ingest-s3.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 15:33:28.000000 unstructured-0.9.0/requirements/ingest-slack.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 15:33:28.000000 unstructured-0.9.0/requirements/ingest-wikipedia.in
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-01 15:33:39.456573 unstructured-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-08-01 15:33:28.000000 unstructured-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:33:39.432571 unstructured-0.9.0/test_unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:33:28.000000 unstructured-0.9.0/test_unstructured/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:33:39.432571 unstructured-0.9.0/test_unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:33:28.000000 unstructured-0.9.0/test_unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-08-01 15:33:28.000000 unstructured-0.9.0/test_unstructured/nlp/mock_nltk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-01 15:33:28.000000 unstructured-0.9.0/test_unstructured/nlp/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-08-01 15:33:28.000000 unstructured-0.9.0/test_unstructured/nlp/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-08-01 15:33:28.000000 unstructured-0.9.0/test_unstructured/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:33:39.432571 unstructured-0.9.0/unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:33:39.432571 unstructured-0.9.0/unstructured/cleaners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/cleaners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/cleaners/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/cleaners/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/cleaners/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:33:39.436571 unstructured-0.9.0/unstructured/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/documents/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15606 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/documents/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/documents/email_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16209 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/documents/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/documents/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:33:39.436571 unstructured-0.9.0/unstructured/file_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/file_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/file_utils/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/file_utils/exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/file_utils/file_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20754 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/file_utils/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/file_utils/google_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/file_utils/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:33:39.436571 unstructured-0.9.0/unstructured/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:33:39.436571 unstructured-0.9.0/unstructured/ingest/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:33:39.440572 unstructured-0.9.0/unstructured/ingest/cli/cmds/
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/cli/cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/cli/cmds/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/cli/cmds/biomed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/cli/cmds/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/cli/cmds/confluence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/cli/cmds/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/cli/cmds/dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/cli/cmds/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/cli/cmds/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/cli/cmds/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/cli/cmds/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/cli/cmds/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/cli/cmds/google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/cli/cmds/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/cli/cmds/onedrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/cli/cmds/outlook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/cli/cmds/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/cli/cmds/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/cli/cmds/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/cli/cmds/wikipedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/cli/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:33:39.440572 unstructured-0.9.0/unstructured/ingest/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/connector/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9521 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/connector/biomed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/connector/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/connector/confluence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/connector/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/connector/dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/connector/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/connector/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/connector/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/connector/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/connector/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/connector/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/connector/google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/connector/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/connector/onedrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/connector/outlook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/connector/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/connector/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/connector/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/connector/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:33:39.440572 unstructured-0.9.0/unstructured/ingest/doc_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/doc_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/doc_processor/generalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12492 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      143 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:33:39.444572 unstructured-0.9.0/unstructured/ingest/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/runner/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/runner/biomed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/runner/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/runner/confluence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/runner/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/runner/dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/runner/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/runner/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/runner/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/runner/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/runner/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/runner/google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/runner/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/runner/onedrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/runner/outlook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/runner/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/runner/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/runner/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/runner/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/ingest/runner/wikipedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:33:39.444572 unstructured-0.9.0/unstructured/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:33:39.448572 unstructured-0.9.0/unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/nlp/english-words.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/nlp/english_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/nlp/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/nlp/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/nlp/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:33:39.452572 unstructured-0.9.0/unstructured/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/partition/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/partition/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10643 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/partition/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/partition/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/partition/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/partition/docx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14888 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/partition/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/partition/epub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/partition/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/partition/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/partition/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/partition/md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/partition/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/partition/odt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/partition/org.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17794 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/partition/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/partition/ppt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/partition/pptx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/partition/rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/partition/rtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/partition/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10744 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/partition/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/partition/text_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/partition/tsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/partition/xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/partition/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:33:39.452572 unstructured-0.9.0/unstructured/staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/staging/argilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/staging/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/staging/baseplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/staging/datasaur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/staging/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/staging/label_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/staging/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/staging/prodigy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/staging/weaviate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-08-01 15:33:28.000000 unstructured-0.9.0/unstructured/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:33:39.432571 unstructured-0.9.0/unstructured.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20360 2023-08-01 15:33:39.000000 unstructured-0.9.0/unstructured.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-08-01 15:33:39.000000 unstructured-0.9.0/unstructured.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 15:33:39.000000 unstructured-0.9.0/unstructured.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-01 15:33:39.000000 unstructured-0.9.0/unstructured.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-08-01 15:33:39.000000 unstructured-0.9.0/unstructured.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-01 15:33:39.000000 unstructured-0.9.0/unstructured.egg-info/top_level.txt
```

### Comparing `unstructured-0.8.8/LICENSE.md` & `unstructured-0.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/MANIFEST.in` & `unstructured-0.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/PKG-INFO` & `unstructured-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.8.8
+Version: 0.9.0
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -306,16 +306,29 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
-Provides-Extra: huggingface
-Provides-Extra: local-inference
+Provides-Extra: all-docs
+Provides-Extra: csv
+Provides-Extra: docx
+Provides-Extra: epub
+Provides-Extra: image
+Provides-Extra: md
+Provides-Extra: msg
+Provides-Extra: odt
+Provides-Extra: org
+Provides-Extra: pdf
+Provides-Extra: pptx
+Provides-Extra: rtf
+Provides-Extra: rst
+Provides-Extra: tsv
+Provides-Extra: xlsx
 Provides-Extra: s3
 Provides-Extra: azure
 Provides-Extra: discord
 Provides-Extra: github
 Provides-Extra: gitlab
 Provides-Extra: reddit
 Provides-Extra: slack
@@ -324,7 +337,9 @@
 Provides-Extra: gcs
 Provides-Extra: elasticsearch
 Provides-Extra: dropbox
 Provides-Extra: box
 Provides-Extra: onedrive
 Provides-Extra: outlook
 Provides-Extra: confluence
+Provides-Extra: huggingface
+Provides-Extra: local-inference
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.8.8 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.9.0 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
@@ -213,13 +213,17 @@
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Requires-Python: >=3.7.0 Description-Content-Type:
-text/markdown Provides-Extra: huggingface Provides-Extra: local-inference
-Provides-Extra: s3 Provides-Extra: azure Provides-Extra: discord Provides-
-Extra: github Provides-Extra: gitlab Provides-Extra: reddit Provides-Extra:
-slack Provides-Extra: wikipedia Provides-Extra: google-drive Provides-Extra:
-gcs Provides-Extra: elasticsearch Provides-Extra: dropbox Provides-Extra: box
-Provides-Extra: onedrive Provides-Extra: outlook Provides-Extra: confluence
+text/markdown Provides-Extra: all-docs Provides-Extra: csv Provides-Extra: docx
+Provides-Extra: epub Provides-Extra: image Provides-Extra: md Provides-Extra:
+msg Provides-Extra: odt Provides-Extra: org Provides-Extra: pdf Provides-Extra:
+pptx Provides-Extra: rtf Provides-Extra: rst Provides-Extra: tsv Provides-
+Extra: xlsx Provides-Extra: s3 Provides-Extra: azure Provides-Extra: discord
+Provides-Extra: github Provides-Extra: gitlab Provides-Extra: reddit Provides-
+Extra: slack Provides-Extra: wikipedia Provides-Extra: google-drive Provides-
+Extra: gcs Provides-Extra: elasticsearch Provides-Extra: dropbox Provides-
+Extra: box Provides-Extra: onedrive Provides-Extra: outlook Provides-Extra:
+confluence Provides-Extra: huggingface Provides-Extra: local-inference
```

### Comparing `unstructured-0.8.8/README.md` & `unstructured-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/test_unstructured/nlp/mock_nltk.py` & `unstructured-0.9.0/test_unstructured/nlp/mock_nltk.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/test_unstructured/nlp/test_tokenize.py` & `unstructured-0.9.0/test_unstructured/nlp/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/test_unstructured/test_utils.py` & `unstructured-0.9.0/test_unstructured/test_utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/cleaners/core.py` & `unstructured-0.9.0/unstructured/cleaners/core.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/cleaners/extract.py` & `unstructured-0.9.0/unstructured/cleaners/extract.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/cleaners/translate.py` & `unstructured-0.9.0/unstructured/cleaners/translate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/documents/base.py` & `unstructured-0.9.0/unstructured/documents/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/documents/coordinates.py` & `unstructured-0.9.0/unstructured/documents/coordinates.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/documents/elements.py` & `unstructured-0.9.0/unstructured/documents/elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/documents/email_elements.py` & `unstructured-0.9.0/unstructured/documents/email_elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/documents/html.py` & `unstructured-0.9.0/unstructured/documents/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/documents/xml.py` & `unstructured-0.9.0/unstructured/documents/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/file_utils/encoding.py` & `unstructured-0.9.0/unstructured/file_utils/encoding.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/file_utils/exploration.py` & `unstructured-0.9.0/unstructured/file_utils/exploration.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/file_utils/file_conversion.py` & `unstructured-0.9.0/unstructured/file_utils/file_conversion.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import tempfile
 from typing import IO, Optional
 
-import pypandoc
-
 from unstructured.partition.common import exactly_one
+from unstructured.utils import dependency_exists, requires_dependencies
+
+if dependency_exists("pypandoc"):
+    import pypandoc
 
 
+@requires_dependencies(["pypandoc"])
 def convert_file_to_text(filename: str, source_format: str, target_format: str) -> str:
     """Uses pandoc to convert the source document to a raw text string."""
     try:
         text = pypandoc.convert_file(filename, target_format, format=source_format)
     except FileNotFoundError as err:
         msg = (
             "Error converting the file to text. Ensure you have the pandoc "
```

### Comparing `unstructured-0.8.8/unstructured/file_utils/filetype.py` & `unstructured-0.9.0/unstructured/file_utils/filetype.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/file_utils/metadata.py` & `unstructured-0.9.0/unstructured/file_utils/metadata.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/cli/cli.py` & `unstructured-0.9.0/unstructured/ingest/cli/cli.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/cli/cmds/__init__.py` & `unstructured-0.9.0/unstructured/ingest/cli/cmds/__init__.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/cli/cmds/azure.py` & `unstructured-0.9.0/unstructured/ingest/cli/cmds/azure.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/cli/cmds/biomed.py` & `unstructured-0.9.0/unstructured/ingest/cli/cmds/biomed.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/cli/cmds/box.py` & `unstructured-0.9.0/unstructured/ingest/cli/cmds/box.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/cli/cmds/confluence.py` & `unstructured-0.9.0/unstructured/ingest/cli/cmds/confluence.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/cli/cmds/discord.py` & `unstructured-0.9.0/unstructured/ingest/cli/cmds/discord.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/cli/cmds/dropbox.py` & `unstructured-0.9.0/unstructured/ingest/cli/cmds/dropbox.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/cli/cmds/elasticsearch.py` & `unstructured-0.9.0/unstructured/ingest/cli/cmds/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/cli/cmds/fsspec.py` & `unstructured-0.9.0/unstructured/ingest/cli/cmds/fsspec.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/cli/cmds/gcs.py` & `unstructured-0.9.0/unstructured/ingest/cli/cmds/gcs.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/cli/cmds/github.py` & `unstructured-0.9.0/unstructured/ingest/cli/cmds/github.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/cli/cmds/gitlab.py` & `unstructured-0.9.0/unstructured/ingest/cli/cmds/gitlab.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/cli/cmds/google_drive.py` & `unstructured-0.9.0/unstructured/ingest/cli/cmds/google_drive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/cli/cmds/local.py` & `unstructured-0.9.0/unstructured/ingest/cli/cmds/local.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/cli/cmds/onedrive.py` & `unstructured-0.9.0/unstructured/ingest/cli/cmds/onedrive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/cli/cmds/outlook.py` & `unstructured-0.9.0/unstructured/ingest/cli/cmds/outlook.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/cli/cmds/reddit.py` & `unstructured-0.9.0/unstructured/ingest/cli/cmds/reddit.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/cli/cmds/s3.py` & `unstructured-0.9.0/unstructured/ingest/cli/cmds/s3.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/cli/cmds/slack.py` & `unstructured-0.9.0/unstructured/ingest/cli/cmds/slack.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/cli/cmds/wikipedia.py` & `unstructured-0.9.0/unstructured/ingest/cli/cmds/wikipedia.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/cli/common.py` & `unstructured-0.9.0/unstructured/ingest/cli/common.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/connector/azure.py` & `unstructured-0.9.0/unstructured/ingest/connector/azure.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/connector/biomed.py` & `unstructured-0.9.0/unstructured/ingest/connector/biomed.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/connector/box.py` & `unstructured-0.9.0/unstructured/ingest/connector/box.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/connector/confluence.py` & `unstructured-0.9.0/unstructured/ingest/connector/confluence.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/connector/discord.py` & `unstructured-0.9.0/unstructured/ingest/connector/discord.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/connector/dropbox.py` & `unstructured-0.9.0/unstructured/ingest/connector/dropbox.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/connector/elasticsearch.py` & `unstructured-0.9.0/unstructured/ingest/connector/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/connector/fsspec.py` & `unstructured-0.9.0/unstructured/ingest/connector/fsspec.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/connector/gcs.py` & `unstructured-0.9.0/unstructured/ingest/connector/gcs.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/connector/git.py` & `unstructured-0.9.0/unstructured/ingest/connector/git.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/connector/github.py` & `unstructured-0.9.0/unstructured/ingest/connector/github.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/connector/gitlab.py` & `unstructured-0.9.0/unstructured/ingest/connector/gitlab.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/connector/google_drive.py` & `unstructured-0.9.0/unstructured/ingest/connector/google_drive.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     # Google Drive Specific Options
     drive_id: str
     service_account_key: str
     extension: Optional[str]
     recursive: bool = False
 
     def __post_init__(self):
-        if self.extension and self.extension not in EXT_TO_FILETYPE.keys():
+        if self.extension and self.extension not in EXT_TO_FILETYPE:
             raise ValueError(
                 f"Extension not supported. "
                 f"Value MUST be one of {', '.join([k for k in EXT_TO_FILETYPE if k is not None])}.",
             )
         self.service = create_service_account_object(self.service_account_key, self.drive_id)
```

### Comparing `unstructured-0.8.8/unstructured/ingest/connector/local.py` & `unstructured-0.9.0/unstructured/ingest/connector/local.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/connector/onedrive.py` & `unstructured-0.9.0/unstructured/ingest/connector/onedrive.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     file: "DriveItem"
 
     def __post_init__(self):
         self.ext = "".join(Path(self.file.name).suffixes)
         if not self.ext:
             raise ValueError("Unsupported file without extension.")
 
-        if self.ext not in EXT_TO_FILETYPE.keys():
+        if self.ext not in EXT_TO_FILETYPE:
             raise ValueError(
                 f"Extension not supported. "
                 f"Value MUST be one of {', '.join([k for k in EXT_TO_FILETYPE if k is not None])}.",
             )
         self._set_download_paths()
 
     def _set_download_paths(self) -> None:
```

### Comparing `unstructured-0.8.8/unstructured/ingest/connector/outlook.py` & `unstructured-0.9.0/unstructured/ingest/connector/outlook.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/connector/reddit.py` & `unstructured-0.9.0/unstructured/ingest/connector/reddit.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/connector/s3.py` & `unstructured-0.9.0/unstructured/ingest/connector/s3.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/connector/slack.py` & `unstructured-0.9.0/unstructured/ingest/connector/slack.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/connector/wikipedia.py` & `unstructured-0.9.0/unstructured/ingest/connector/wikipedia.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/doc_processor/generalized.py` & `unstructured-0.9.0/unstructured/ingest/doc_processor/generalized.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/interfaces.py` & `unstructured-0.9.0/unstructured/ingest/interfaces.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/processor.py` & `unstructured-0.9.0/unstructured/ingest/processor.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/runner/__init__.py` & `unstructured-0.9.0/unstructured/ingest/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/runner/azure.py` & `unstructured-0.9.0/unstructured/ingest/runner/azure.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/runner/biomed.py` & `unstructured-0.9.0/unstructured/ingest/runner/biomed.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/runner/box.py` & `unstructured-0.9.0/unstructured/ingest/runner/box.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/runner/confluence.py` & `unstructured-0.9.0/unstructured/ingest/runner/confluence.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/runner/discord.py` & `unstructured-0.9.0/unstructured/ingest/runner/discord.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/runner/dropbox.py` & `unstructured-0.9.0/unstructured/ingest/runner/dropbox.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/runner/elasticsearch.py` & `unstructured-0.9.0/unstructured/ingest/runner/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/runner/fsspec.py` & `unstructured-0.9.0/unstructured/ingest/runner/fsspec.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/runner/gcs.py` & `unstructured-0.9.0/unstructured/ingest/runner/gcs.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/runner/github.py` & `unstructured-0.9.0/unstructured/ingest/runner/github.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/runner/gitlab.py` & `unstructured-0.9.0/unstructured/ingest/runner/gitlab.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/runner/google_drive.py` & `unstructured-0.9.0/unstructured/ingest/runner/google_drive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/runner/local.py` & `unstructured-0.9.0/unstructured/ingest/runner/local.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/runner/onedrive.py` & `unstructured-0.9.0/unstructured/ingest/runner/onedrive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/runner/outlook.py` & `unstructured-0.9.0/unstructured/ingest/runner/outlook.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/runner/reddit.py` & `unstructured-0.9.0/unstructured/ingest/runner/reddit.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/runner/s3.py` & `unstructured-0.9.0/unstructured/ingest/runner/s3.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/runner/slack.py` & `unstructured-0.9.0/unstructured/ingest/runner/slack.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/runner/utils.py` & `unstructured-0.9.0/unstructured/ingest/runner/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/ingest/runner/wikipedia.py` & `unstructured-0.9.0/unstructured/ingest/runner/wikipedia.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/nlp/english-words.txt` & `unstructured-0.9.0/unstructured/nlp/english-words.txt`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/nlp/english_words.py` & `unstructured-0.9.0/unstructured/nlp/english_words.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/nlp/patterns.py` & `unstructured-0.9.0/unstructured/nlp/patterns.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/nlp/tokenize.py` & `unstructured-0.9.0/unstructured/nlp/tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/partition/__init__.py` & `unstructured-0.9.0/unstructured/partition/__init__.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/partition/api.py` & `unstructured-0.9.0/unstructured/partition/api.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/partition/auto.py` & `unstructured-0.9.0/unstructured/partition/auto.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,35 +9,66 @@
     STR_TO_FILETYPE,
     FileType,
     detect_filetype,
     is_json_processable,
 )
 from unstructured.logger import logger
 from unstructured.partition.common import exactly_one
-from unstructured.partition.csv import partition_csv
-from unstructured.partition.doc import partition_doc
-from unstructured.partition.docx import partition_docx
 from unstructured.partition.email import partition_email
-from unstructured.partition.epub import partition_epub
 from unstructured.partition.html import partition_html
-from unstructured.partition.image import partition_image
 from unstructured.partition.json import partition_json
-from unstructured.partition.md import partition_md
-from unstructured.partition.msg import partition_msg
-from unstructured.partition.odt import partition_odt
-from unstructured.partition.org import partition_org
-from unstructured.partition.pdf import partition_pdf
-from unstructured.partition.ppt import partition_ppt
-from unstructured.partition.pptx import partition_pptx
-from unstructured.partition.rst import partition_rst
-from unstructured.partition.rtf import partition_rtf
 from unstructured.partition.text import partition_text
-from unstructured.partition.tsv import partition_tsv
-from unstructured.partition.xlsx import partition_xlsx
 from unstructured.partition.xml import partition_xml
+from unstructured.utils import dependency_exists
+
+if dependency_exists("pandas"):
+    from unstructured.partition.csv import partition_csv
+    from unstructured.partition.tsv import partition_tsv
+
+
+if dependency_exists("docx"):
+    from unstructured.partition.doc import partition_doc
+    from unstructured.partition.docx import partition_docx
+
+
+if dependency_exists("docx") and dependency_exists("pypandoc"):
+    from unstructured.partition.odt import partition_odt
+
+
+if dependency_exists("pypandoc"):
+    from unstructured.partition.epub import partition_epub
+    from unstructured.partition.org import partition_org
+    from unstructured.partition.rst import partition_rst
+    from unstructured.partition.rtf import partition_rtf
+
+
+if dependency_exists("markdown"):
+    from unstructured.partition.md import partition_md
+
+
+if dependency_exists("msg_parser"):
+    from unstructured.partition.msg import partition_msg
+
+
+pdf_imports = ["pdf2image", "pdfminer", "PIL"]
+if all(dependency_exists(dep) for dep in pdf_imports):
+    from unstructured.partition.pdf import partition_pdf
+
+
+if dependency_exists("unstructured_inference"):
+    from unstructured.partition.image import partition_image
+
+
+if dependency_exists("pptx"):
+    from unstructured.partition.ppt import partition_ppt
+    from unstructured.partition.pptx import partition_pptx
+
+
+if dependency_exists("pandas") and dependency_exists("openpyxl"):
+    from unstructured.partition.xlsx import partition_xlsx
 
 
 def partition(
     filename: Optional[str] = None,
     content_type: Optional[str] = None,
     file: Optional[IO[bytes]] = None,
     file_filename: Optional[str] = None,
```

### Comparing `unstructured-0.8.8/unstructured/partition/common.py` & `unstructured-0.9.0/unstructured/partition/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import os
 import subprocess
 from datetime import datetime
 from io import BufferedReader, BytesIO, TextIOWrapper
 from tempfile import SpooledTemporaryFile
 from typing import IO, TYPE_CHECKING, Any, BinaryIO, Dict, List, Optional, Tuple, Union
 
-from docx import table as docxtable
 from tabulate import tabulate
 
 from unstructured.documents.coordinates import CoordinateSystem
 from unstructured.documents.elements import (
     TYPE_TO_TEXT_ELEMENT_MAP,
     CheckBox,
     CoordinatesMetadata,
@@ -19,14 +18,18 @@
     ElementMetadata,
     ListItem,
     PageBreak,
     Text,
 )
 from unstructured.logger import logger
 from unstructured.nlp.patterns import ENUMERATED_BULLETS_RE, UNICODE_BULLETS_RE
+from unstructured.utils import dependency_exists
+
+if dependency_exists("docx"):
+    import docx.table as docxtable
 
 if TYPE_CHECKING:
     from unstructured_inference.inference.layoutelement import (
         LayoutElement,
         LocationlessLayoutElement,
     )
 
@@ -299,20 +302,20 @@
             f_bytes = f.read()
     else:
         raise ValueError("Invalid file-like object type")
 
     return f_bytes
 
 
-def convert_ms_office_table_to_text(table: docxtable.Table, as_html: bool = True):
+def convert_ms_office_table_to_text(table: "docxtable.Table", as_html: bool = True) -> str:
     """
     Convert a table object from a Word document to an HTML table string using the tabulate library.
 
     Args:
-        table (Table): A Table object.
+        table (Table): A docx.table.Table object.
         as_html (bool): Whether to return the table as an HTML string (True) or a
             plain text string (False)
 
     Returns:
         str: An table string representation of the input table.
     """
     fmt = "html" if as_html else "plain"
```

### Comparing `unstructured-0.8.8/unstructured/partition/csv.py` & `unstructured-0.9.0/unstructured/partition/csv.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/partition/doc.py` & `unstructured-0.9.0/unstructured/partition/doc.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/partition/docx.py` & `unstructured-0.9.0/unstructured/partition/docx.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 import tempfile
 from tempfile import SpooledTemporaryFile
 from typing import IO, BinaryIO, List, Optional, Tuple, Union, cast
 
 import docx
-import pypandoc
 from docx.oxml.shared import qn
 from docx.text.paragraph import Paragraph
 from docx.text.run import Run
 
 from unstructured.cleaners.core import clean_bullets
 from unstructured.documents.elements import (
     Address,
@@ -34,14 +33,18 @@
 )
 from unstructured.partition.text_type import (
     is_bulleted_text,
     is_possible_narrative_text,
     is_possible_title,
     is_us_city_state_zip,
 )
+from unstructured.utils import dependency_exists
+
+if dependency_exists("pypandoc"):
+    import pypandoc
 
 # NOTE(robinson) - documentation on built in styles can be found at the link below
 # ref: https://python-docx.readthedocs.io/en/latest/user/
 #   styles-understanding.html#paragraph-styles-in-default-template
 STYLE_TO_ELEMENT_MAPPING = {
     "Caption": Text,  # TODO(robinson) - add caption element type
     "Heading 1": Title,
@@ -310,15 +313,15 @@
     source_format: str,
     filename: Optional[str] = None,
     file: Optional[IO[bytes]] = None,
     include_metadata: bool = True,
     metadata_filename: Optional[str] = None,
     metadata_last_modified: Optional[str] = None,
 ) -> List[Element]:
-    """Converts a document to DOCX and then partitions it using partition_html. Works with
+    """Converts a document to DOCX and then partitions it using partition_docx. Works with
     any file format support by pandoc.
 
     Parameters
     ----------
     source_format
         The format of the source document, .e.g. odt
     filename
```

### Comparing `unstructured-0.8.8/unstructured/partition/email.py` & `unstructured-0.9.0/unstructured/partition/email.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/partition/epub.py` & `unstructured-0.9.0/unstructured/partition/epub.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/partition/html.py` & `unstructured-0.9.0/unstructured/partition/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/partition/image.py` & `unstructured-0.9.0/unstructured/partition/image.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/partition/json.py` & `unstructured-0.9.0/unstructured/partition/json.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/partition/md.py` & `unstructured-0.9.0/unstructured/partition/md.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/partition/msg.py` & `unstructured-0.9.0/unstructured/partition/msg.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/partition/odt.py` & `unstructured-0.9.0/unstructured/partition/odt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/partition/org.py` & `unstructured-0.9.0/unstructured/partition/org.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/partition/pdf.py` & `unstructured-0.9.0/unstructured/partition/pdf.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/partition/ppt.py` & `unstructured-0.9.0/unstructured/partition/ppt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/partition/pptx.py` & `unstructured-0.9.0/unstructured/partition/pptx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/partition/rst.py` & `unstructured-0.9.0/unstructured/partition/rst.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/partition/rtf.py` & `unstructured-0.9.0/unstructured/partition/rtf.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/partition/strategies.py` & `unstructured-0.9.0/unstructured/partition/strategies.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/partition/text.py` & `unstructured-0.9.0/unstructured/partition/text.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/partition/text_type.py` & `unstructured-0.9.0/unstructured/partition/text_type.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/partition/tsv.py` & `unstructured-0.9.0/unstructured/partition/tsv.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/partition/xlsx.py` & `unstructured-0.9.0/unstructured/partition/xlsx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/partition/xml.py` & `unstructured-0.9.0/unstructured/partition/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/staging/argilla.py` & `unstructured-0.9.0/unstructured/staging/argilla.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/staging/base.py` & `unstructured-0.9.0/unstructured/staging/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import csv
 import io
 import json
 from typing import Any, Dict, List, Optional
 
-import pandas as pd
-
 from unstructured.documents.elements import (
     TYPE_TO_TEXT_ELEMENT_MAP,
     CheckBox,
     Element,
     ElementMetadata,
     NoID,
 )
 from unstructured.partition.common import exactly_one
+from unstructured.utils import dependency_exists, requires_dependencies
+
+if dependency_exists("pandas"):
+    import pandas as pd
 
 
 def _get_metadata_table_fieldnames():
     metadata_fields = list(ElementMetadata.__annotations__.keys())
     metadata_fields.remove("coordinates")
     metadata_fields.extend(
         [
@@ -157,34 +159,37 @@
         metadata = row.pop("metadata")
         for key, value in flatten_dict(metadata).items():
             if key in table_fieldnames:
                 row[key] = value
 
         if row.get("sent_from"):
             row["sender"] = row.get("sent_from")
-            if type(row["sender"]) == list:
+            if isinstance(row["sender"], list):
                 row["sender"] = row["sender"][0]
 
     with io.StringIO() as buffer:
         csv_writer = csv.DictWriter(buffer, fieldnames=table_fieldnames)
         csv_writer.writeheader()
         csv_writer.writerows(rows)
         return buffer.getvalue()
 
 
 def convert_to_csv(elements: List[Element]) -> str:
     """Converts a list of elements to a CSV."""
     return convert_to_isd_csv(elements)
 
 
-def convert_to_dataframe(elements: List[Element], drop_empty_cols: bool = True) -> pd.DataFrame:
+@requires_dependencies(["pandas"])
+def convert_to_dataframe(elements: List[Element], drop_empty_cols: bool = True) -> "pd.DataFrame":
     """Converts document elements to a pandas DataFrame. The dataframe contains the
     following columns:
         text: the element text
         type: the text type (NarrativeText, Title, etc)
+
+    Output is pd.DataFrame
     """
     csv_string = convert_to_isd_csv(elements)
     csv_string_io = io.StringIO(csv_string)
     df = pd.read_csv(csv_string_io, sep=",")
     if drop_empty_cols:
         df.dropna(axis=1, how="all", inplace=True)
     return df
```

### Comparing `unstructured-0.8.8/unstructured/staging/baseplate.py` & `unstructured-0.9.0/unstructured/staging/baseplate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/staging/datasaur.py` & `unstructured-0.9.0/unstructured/staging/datasaur.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/staging/huggingface.py` & `unstructured-0.9.0/unstructured/staging/huggingface.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/staging/label_box.py` & `unstructured-0.9.0/unstructured/staging/label_box.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/staging/label_studio.py` & `unstructured-0.9.0/unstructured/staging/label_studio.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/staging/prodigy.py` & `unstructured-0.9.0/unstructured/staging/prodigy.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/staging/weaviate.py` & `unstructured-0.9.0/unstructured/staging/weaviate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured/utils.py` & `unstructured-0.9.0/unstructured/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.8/unstructured.egg-info/PKG-INFO` & `unstructured-0.9.0/unstructured.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.8.8
+Version: 0.9.0
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -306,16 +306,29 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
-Provides-Extra: huggingface
-Provides-Extra: local-inference
+Provides-Extra: all-docs
+Provides-Extra: csv
+Provides-Extra: docx
+Provides-Extra: epub
+Provides-Extra: image
+Provides-Extra: md
+Provides-Extra: msg
+Provides-Extra: odt
+Provides-Extra: org
+Provides-Extra: pdf
+Provides-Extra: pptx
+Provides-Extra: rtf
+Provides-Extra: rst
+Provides-Extra: tsv
+Provides-Extra: xlsx
 Provides-Extra: s3
 Provides-Extra: azure
 Provides-Extra: discord
 Provides-Extra: github
 Provides-Extra: gitlab
 Provides-Extra: reddit
 Provides-Extra: slack
@@ -324,7 +337,9 @@
 Provides-Extra: gcs
 Provides-Extra: elasticsearch
 Provides-Extra: dropbox
 Provides-Extra: box
 Provides-Extra: onedrive
 Provides-Extra: outlook
 Provides-Extra: confluence
+Provides-Extra: huggingface
+Provides-Extra: local-inference
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.8.8 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.9.0 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
@@ -213,13 +213,17 @@
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Requires-Python: >=3.7.0 Description-Content-Type:
-text/markdown Provides-Extra: huggingface Provides-Extra: local-inference
-Provides-Extra: s3 Provides-Extra: azure Provides-Extra: discord Provides-
-Extra: github Provides-Extra: gitlab Provides-Extra: reddit Provides-Extra:
-slack Provides-Extra: wikipedia Provides-Extra: google-drive Provides-Extra:
-gcs Provides-Extra: elasticsearch Provides-Extra: dropbox Provides-Extra: box
-Provides-Extra: onedrive Provides-Extra: outlook Provides-Extra: confluence
+text/markdown Provides-Extra: all-docs Provides-Extra: csv Provides-Extra: docx
+Provides-Extra: epub Provides-Extra: image Provides-Extra: md Provides-Extra:
+msg Provides-Extra: odt Provides-Extra: org Provides-Extra: pdf Provides-Extra:
+pptx Provides-Extra: rtf Provides-Extra: rst Provides-Extra: tsv Provides-
+Extra: xlsx Provides-Extra: s3 Provides-Extra: azure Provides-Extra: discord
+Provides-Extra: github Provides-Extra: gitlab Provides-Extra: reddit Provides-
+Extra: slack Provides-Extra: wikipedia Provides-Extra: google-drive Provides-
+Extra: gcs Provides-Extra: elasticsearch Provides-Extra: dropbox Provides-
+Extra: box Provides-Extra: onedrive Provides-Extra: outlook Provides-Extra:
+confluence Provides-Extra: huggingface Provides-Extra: local-inference
```

### Comparing `unstructured-0.8.8/unstructured.egg-info/SOURCES.txt` & `unstructured-0.9.0/unstructured.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 requirements/ingest-google-drive.in
 requirements/ingest-onedrive.in
 requirements/ingest-outlook.in
 requirements/ingest-reddit.in
 requirements/ingest-s3.in
 requirements/ingest-slack.in
 requirements/ingest-wikipedia.in
-requirements/local-inference.in
 test_unstructured/__init__.py
 test_unstructured/test_utils.py
 test_unstructured/nlp/__init__.py
 test_unstructured/nlp/mock_nltk.py
 test_unstructured/nlp/test_partition.py
 test_unstructured/nlp/test_tokenize.py
 unstructured/__init__.py
```

