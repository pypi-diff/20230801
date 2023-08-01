# Comparing `tmp/unstructured-0.8.7.tar.gz` & `tmp/unstructured-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured-0.8.7.tar", last modified: Fri Jul 28 16:42:16 2023, max compression
+gzip compressed data, was "unstructured-0.8.8.tar", last modified: Tue Aug  1 06:14:14 2023, max compression
```

## Comparing `unstructured-0.8.7.tar` & `unstructured-0.8.8.tar`

### file list

```diff
@@ -1,142 +1,192 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:16.215083 unstructured-0.8.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-28 16:42:06.000000 unstructured-0.8.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-28 16:42:06.000000 unstructured-0.8.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20030 2023-07-28 16:42:16.215083 unstructured-0.8.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16273 2023-07-28 16:42:06.000000 unstructured-0.8.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:16.203083 unstructured-0.8.7/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-28 16:42:06.000000 unstructured-0.8.7/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-28 16:42:06.000000 unstructured-0.8.7/requirements/huggingface.in
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-28 16:42:06.000000 unstructured-0.8.7/requirements/ingest-azure.in
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-28 16:42:06.000000 unstructured-0.8.7/requirements/ingest-discord.in
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-28 16:42:06.000000 unstructured-0.8.7/requirements/ingest-dropbox.in
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-28 16:42:06.000000 unstructured-0.8.7/requirements/ingest-gcs.in
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-28 16:42:06.000000 unstructured-0.8.7/requirements/ingest-github.in
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-28 16:42:06.000000 unstructured-0.8.7/requirements/ingest-gitlab.in
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-28 16:42:06.000000 unstructured-0.8.7/requirements/ingest-google-drive.in
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 16:42:06.000000 unstructured-0.8.7/requirements/ingest-onedrive.in
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 16:42:06.000000 unstructured-0.8.7/requirements/ingest-outlook.in
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-28 16:42:06.000000 unstructured-0.8.7/requirements/ingest-reddit.in
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-28 16:42:06.000000 unstructured-0.8.7/requirements/ingest-s3.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-28 16:42:06.000000 unstructured-0.8.7/requirements/ingest-slack.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-28 16:42:06.000000 unstructured-0.8.7/requirements/ingest-wikipedia.in
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-28 16:42:06.000000 unstructured-0.8.7/requirements/local-inference.in
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-28 16:42:16.215083 unstructured-0.8.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-07-28 16:42:06.000000 unstructured-0.8.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:16.203083 unstructured-0.8.7/test_unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:06.000000 unstructured-0.8.7/test_unstructured/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:16.203083 unstructured-0.8.7/test_unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:06.000000 unstructured-0.8.7/test_unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-28 16:42:06.000000 unstructured-0.8.7/test_unstructured/nlp/mock_nltk.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-28 16:42:06.000000 unstructured-0.8.7/test_unstructured/nlp/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-28 16:42:06.000000 unstructured-0.8.7/test_unstructured/nlp/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-28 16:42:06.000000 unstructured-0.8.7/test_unstructured/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:16.203083 unstructured-0.8.7/unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:16.203083 unstructured-0.8.7/unstructured/cleaners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/cleaners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/cleaners/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/cleaners/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/cleaners/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:16.203083 unstructured-0.8.7/unstructured/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/documents/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/documents/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/documents/email_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    16209 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/documents/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/documents/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:16.203083 unstructured-0.8.7/unstructured/file_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/file_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/file_utils/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/file_utils/exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/file_utils/file_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    20736 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/file_utils/filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/file_utils/google_filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/file_utils/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:16.203083 unstructured-0.8.7/unstructured/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:16.207083 unstructured-0.8.7/unstructured/ingest/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/biomed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/confluence.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/dropbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/google_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/onedrive.py
--rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/outlook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/connector/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:16.207083 unstructured-0.8.7/unstructured/ingest/doc_processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/doc_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/doc_processor/generalized.py
--rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33906 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/ingest/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:16.207083 unstructured-0.8.7/unstructured/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:16.211083 unstructured-0.8.7/unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/nlp/english-words.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/nlp/english_words.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/nlp/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/nlp/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/nlp/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:16.215083 unstructured-0.8.7/unstructured/partition/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11739 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)    10544 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12408 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/docx.py
--rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/epub.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/md.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/msg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/odt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/org.py
--rw-r--r--   0 runner    (1001) docker     (123)    17533 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/ppt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/pptx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/rst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/rtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/text_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/tsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/partition/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:16.215083 unstructured-0.8.7/unstructured/staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/staging/argilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/staging/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/staging/baseplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/staging/datasaur.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/staging/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/staging/label_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/staging/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/staging/prodigy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/staging/weaviate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-07-28 16:42:06.000000 unstructured-0.8.7/unstructured/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:42:16.203083 unstructured-0.8.7/unstructured.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20030 2023-07-28 16:42:15.000000 unstructured-0.8.7/unstructured.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-28 16:42:16.000000 unstructured-0.8.7/unstructured.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 16:42:15.000000 unstructured-0.8.7/unstructured.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 16:42:15.000000 unstructured-0.8.7/unstructured.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-28 16:42:15.000000 unstructured-0.8.7/unstructured.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 16:42:15.000000 unstructured-0.8.7/unstructured.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.225310 unstructured-0.8.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-08-01 06:14:04.000000 unstructured-0.8.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-08-01 06:14:04.000000 unstructured-0.8.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20050 2023-08-01 06:14:14.225310 unstructured-0.8.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16273 2023-08-01 06:14:04.000000 unstructured-0.8.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.205310 unstructured-0.8.8/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-01 06:14:05.000000 unstructured-0.8.8/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-01 06:14:05.000000 unstructured-0.8.8/requirements/huggingface.in
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-01 06:14:05.000000 unstructured-0.8.8/requirements/ingest-azure.in
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 06:14:05.000000 unstructured-0.8.8/requirements/ingest-box.in
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-01 06:14:05.000000 unstructured-0.8.8/requirements/ingest-discord.in
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 06:14:05.000000 unstructured-0.8.8/requirements/ingest-dropbox.in
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-01 06:14:05.000000 unstructured-0.8.8/requirements/ingest-gcs.in
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-01 06:14:05.000000 unstructured-0.8.8/requirements/ingest-github.in
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 06:14:05.000000 unstructured-0.8.8/requirements/ingest-gitlab.in
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-01 06:14:05.000000 unstructured-0.8.8/requirements/ingest-google-drive.in
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-01 06:14:05.000000 unstructured-0.8.8/requirements/ingest-onedrive.in
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-01 06:14:05.000000 unstructured-0.8.8/requirements/ingest-outlook.in
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 06:14:05.000000 unstructured-0.8.8/requirements/ingest-reddit.in
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 06:14:05.000000 unstructured-0.8.8/requirements/ingest-s3.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 06:14:05.000000 unstructured-0.8.8/requirements/ingest-slack.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 06:14:05.000000 unstructured-0.8.8/requirements/ingest-wikipedia.in
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-01 06:14:05.000000 unstructured-0.8.8/requirements/local-inference.in
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-01 06:14:14.225310 unstructured-0.8.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-08-01 06:14:05.000000 unstructured-0.8.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.205310 unstructured-0.8.8/test_unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:05.000000 unstructured-0.8.8/test_unstructured/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.205310 unstructured-0.8.8/test_unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:05.000000 unstructured-0.8.8/test_unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-08-01 06:14:05.000000 unstructured-0.8.8/test_unstructured/nlp/mock_nltk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-01 06:14:05.000000 unstructured-0.8.8/test_unstructured/nlp/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-08-01 06:14:05.000000 unstructured-0.8.8/test_unstructured/nlp/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-08-01 06:14:05.000000 unstructured-0.8.8/test_unstructured/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.209310 unstructured-0.8.8/unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.209310 unstructured-0.8.8/unstructured/cleaners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/cleaners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/cleaners/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/cleaners/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/cleaners/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.209310 unstructured-0.8.8/unstructured/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/documents/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15606 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/documents/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/documents/email_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16209 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/documents/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/documents/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.209310 unstructured-0.8.8/unstructured/file_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/file_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/file_utils/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/file_utils/exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/file_utils/file_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20754 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/file_utils/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/file_utils/google_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/file_utils/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.209310 unstructured-0.8.8/unstructured/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.209310 unstructured-0.8.8/unstructured/ingest/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.213310 unstructured-0.8.8/unstructured/ingest/cli/cmds/
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/biomed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/confluence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/onedrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/outlook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/cmds/wikipedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/cli/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.213310 unstructured-0.8.8/unstructured/ingest/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9521 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/biomed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/confluence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/onedrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/outlook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/connector/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.213310 unstructured-0.8.8/unstructured/ingest/doc_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/doc_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/doc_processor/generalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12492 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      143 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.217310 unstructured-0.8.8/unstructured/ingest/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/biomed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/confluence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/onedrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/outlook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/ingest/runner/wikipedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.217310 unstructured-0.8.8/unstructured/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.221310 unstructured-0.8.8/unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/nlp/english-words.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/nlp/english_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/nlp/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/nlp/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/nlp/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.221310 unstructured-0.8.8/unstructured/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11739 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10544 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12489 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/docx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14888 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/epub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/odt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/org.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17794 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/ppt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/pptx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/rtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10744 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/text_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/tsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/partition/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.225310 unstructured-0.8.8/unstructured/staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/staging/argilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/staging/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/staging/baseplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/staging/datasaur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/staging/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/staging/label_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/staging/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/staging/prodigy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/staging/weaviate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-08-01 06:14:05.000000 unstructured-0.8.8/unstructured/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:14.209310 unstructured-0.8.8/unstructured.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20050 2023-08-01 06:14:13.000000 unstructured-0.8.8/unstructured.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-08-01 06:14:14.000000 unstructured-0.8.8/unstructured.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 06:14:13.000000 unstructured-0.8.8/unstructured.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-01 06:14:13.000000 unstructured-0.8.8/unstructured.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-01 06:14:13.000000 unstructured-0.8.8/unstructured.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-01 06:14:13.000000 unstructured-0.8.8/unstructured.egg-info/top_level.txt
```

### Comparing `unstructured-0.8.7/LICENSE.md` & `unstructured-0.8.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/MANIFEST.in` & `unstructured-0.8.8/MANIFEST.in`

 * *Files 4% similar despite different names*

```diff
@@ -10,7 +10,8 @@
 include requirements/ingest-gitlab.in
 include requirements/ingest-reddit.in
 include requirements/ingest-slack.in
 include requirements/ingest-wikipedia.in
 include requirements/ingest-google-drive.in
 include requirements/ingest-outlook.in
 include requirements/ingest-onedrive.in
+include requirements/ingest-box.in
```

### Comparing `unstructured-0.8.7/PKG-INFO` & `unstructured-0.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.8.7
+Version: 0.8.8
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -320,10 +320,11 @@
 Provides-Extra: reddit
 Provides-Extra: slack
 Provides-Extra: wikipedia
 Provides-Extra: google-drive
 Provides-Extra: gcs
 Provides-Extra: elasticsearch
 Provides-Extra: dropbox
+Provides-Extra: box
 Provides-Extra: onedrive
 Provides-Extra: outlook
 Provides-Extra: confluence
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.8.7 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.8.8 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
@@ -217,9 +217,9 @@
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Requires-Python: >=3.7.0 Description-Content-Type:
 text/markdown Provides-Extra: huggingface Provides-Extra: local-inference
 Provides-Extra: s3 Provides-Extra: azure Provides-Extra: discord Provides-
 Extra: github Provides-Extra: gitlab Provides-Extra: reddit Provides-Extra:
 slack Provides-Extra: wikipedia Provides-Extra: google-drive Provides-Extra:
-gcs Provides-Extra: elasticsearch Provides-Extra: dropbox Provides-Extra:
-onedrive Provides-Extra: outlook Provides-Extra: confluence
+gcs Provides-Extra: elasticsearch Provides-Extra: dropbox Provides-Extra: box
+Provides-Extra: onedrive Provides-Extra: outlook Provides-Extra: confluence
```

### Comparing `unstructured-0.8.7/README.md` & `unstructured-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/setup.py` & `unstructured-0.8.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,14 +81,15 @@
         "reddit": load_requirements("requirements/ingest-reddit.in"),
         "slack": load_requirements("requirements/ingest-slack.in"),
         "wikipedia": load_requirements("requirements/ingest-wikipedia.in"),
         "google-drive": load_requirements("requirements/ingest-google-drive.in"),
         "gcs": load_requirements("requirements/ingest-gcs.in"),
         "elasticsearch": load_requirements("requirements/ingest-elasticsearch.in"),
         "dropbox": load_requirements("requirements/ingest-dropbox.in"),
+        "box": load_requirements("requirements/ingest-box.in"),
         "onedrive": load_requirements("requirements/ingest-onedrive.in"),
         "outlook": load_requirements("requirements/ingest-outlook.in"),
         "confluence": load_requirements("requirements/ingest-confluence.in"),
     },
     package_dir={"unstructured": "unstructured"},
     package_data={"unstructured": ["nlp/*.txt"]},
 )
```

### Comparing `unstructured-0.8.7/test_unstructured/nlp/mock_nltk.py` & `unstructured-0.8.8/test_unstructured/nlp/mock_nltk.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/test_unstructured/nlp/test_tokenize.py` & `unstructured-0.8.8/test_unstructured/nlp/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/test_unstructured/test_utils.py` & `unstructured-0.8.8/test_unstructured/test_utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/cleaners/core.py` & `unstructured-0.8.8/unstructured/cleaners/core.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/cleaners/extract.py` & `unstructured-0.8.8/unstructured/cleaners/extract.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/cleaners/translate.py` & `unstructured-0.8.8/unstructured/cleaners/translate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/documents/base.py` & `unstructured-0.8.8/unstructured/documents/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/documents/coordinates.py` & `unstructured-0.8.8/unstructured/documents/coordinates.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/documents/elements.py` & `unstructured-0.8.8/unstructured/documents/elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 
 @dataclass
 class ElementMetadata:
     coordinates: Optional[CoordinatesMetadata] = None
     data_source: Optional[DataSourceMetadata] = None
     filename: Optional[str] = None
     file_directory: Optional[str] = None
-    date: Optional[str] = None
+    last_modified: Optional[str] = None
     filetype: Optional[str] = None
     attached_to_filename: Optional[str] = None
 
     # Page numbers currenlty supported for PDF, HTML and PPT documents
     page_number: Optional[int] = None
 
     # Page name. The sheet name in XLXS documents.
@@ -182,19 +182,19 @@
 
     def merge(self, other: ElementMetadata):
         for k in self.__dict__:
             if getattr(self, k) is None:
                 setattr(self, k, getattr(other, k))
         return self
 
-    def get_date(self) -> Optional[datetime.datetime]:
+    def get_last_modified(self) -> Optional[datetime.datetime]:
         """Converts the date field to a datetime object."""
         dt = None
-        if self.date is not None:
-            dt = datetime.datetime.fromisoformat(self.date)
+        if self.last_modified is not None:
+            dt = datetime.datetime.fromisoformat(self.last_modified)
         return dt
 
 
 def process_metadata():
     """Decorator for processing metadata for document elements."""
 
     def decorator(func: Callable):
```

### Comparing `unstructured-0.8.7/unstructured/documents/email_elements.py` & `unstructured-0.8.8/unstructured/documents/email_elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/documents/html.py` & `unstructured-0.8.8/unstructured/documents/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/documents/xml.py` & `unstructured-0.8.8/unstructured/documents/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/file_utils/encoding.py` & `unstructured-0.8.8/unstructured/file_utils/encoding.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/file_utils/exploration.py` & `unstructured-0.8.8/unstructured/file_utils/exploration.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/file_utils/file_conversion.py` & `unstructured-0.8.8/unstructured/file_utils/file_conversion.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/file_utils/filetype.py` & `unstructured-0.8.8/unstructured/file_utils/filetype.py`

 * *Files 0% similar despite different names*

```diff
@@ -522,21 +522,21 @@
                 coordinate_system = None
 
             element = normalize_layout_element(layout_element, coordinate_system=coordinate_system)
 
             if isinstance(element, List):
                 for el in element:
                     if last_modification_date:
-                        el.metadata.date = last_modification_date
+                        el.metadata.last_modified = last_modification_date
                     el.metadata.page_number = i + 1
                 page_elements.extend(element)
                 continue
             else:
                 if last_modification_date:
-                    element.metadata.date = last_modification_date
+                    element.metadata.last_modified = last_modification_date
                 element.metadata.text_as_html = (
                     layout_element.text_as_html if hasattr(layout_element, "text_as_html") else None
                 )
                 page_elements.append(element)
             coordinates = (
                 element.metadata.coordinates.points if element.metadata.coordinates else None
             )
```

### Comparing `unstructured-0.8.7/unstructured/file_utils/metadata.py` & `unstructured-0.8.8/unstructured/file_utils/metadata.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/ingest/connector/azure.py` & `unstructured-0.8.8/unstructured/ingest/connector/azure.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/ingest/connector/biomed.py` & `unstructured-0.8.8/unstructured/ingest/connector/biomed.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import urllib.request
 from dataclasses import dataclass
 from ftplib import FTP, error_perm
 from pathlib import Path
-from typing import List, Union
+from typing import List, Optional, Union
 
 import requests
 from bs4 import BeautifulSoup
 from requests.adapters import HTTPAdapter
 from urllib3.util import Retry
 
 from unstructured.ingest.interfaces import (
@@ -37,19 +37,19 @@
 
 
 @dataclass
 class SimpleBiomedConfig(BaseConnectorConfig):
     """Connector config where path is the FTP directory path and
     id_, from_, until, format are API parameters."""
 
-    path: str
+    path: Optional[str]
     # OA Web Service API Options
-    id_: str
-    from_: str
-    until: str
+    id_: Optional[str]
+    from_: Optional[str]
+    until: Optional[str]
     max_retries: int = 5
     request_timeout: int = 45
     decay: float = 0.3
 
     def validate_api_inputs(self):
         valid = False
 
@@ -213,14 +213,18 @@
             files.extend(urls_to_metadata(urls))
 
         return files
 
     def _list_objects(self):
         files = []
 
+        # Conform to mypy, null check performed elsewhere.
+        # Wouldn't be in this method unless self.config.path exists
+        path: str = self.config.path if self.config.path else ""
+
         def traverse(path, download_dir, output_dir):
             full_path = Path(PMC_DIR) / path
             logger.debug(f"Traversing directory: {full_path}")
 
             ftp = FTP(DOMAIN)
             ftp.login()
 
@@ -257,27 +261,27 @@
                         traverse(sub_path, download_dir, output_dir)
 
             else:
                 raise ValueError(f"{full_path} is not a valid directory.")
 
         ftp_path = f"{FTP_DOMAIN}/{PMC_DIR}/{self.config.path}"
         if self.config.is_file:
-            local_path = "/".join(self.config.path.split("/")[1:])
+            local_path = "/".join(path.split("/")[1:])
             return [
                 BiomedFileMeta(
                     ftp_path=ftp_path,
                     download_filepath=(
                         Path(self.standard_config.download_dir) / local_path
                     ).resolve(),
                     output_filepath=(Path(self.standard_config.output_dir) / local_path).resolve(),
                 ),
             ]
         else:
             traverse(
-                Path(self.config.path),
+                Path(path),
                 Path(self.standard_config.download_dir),
                 Path(self.standard_config.output_dir),
             )
 
         return files
 
     def initialize(self):
```

### Comparing `unstructured-0.8.7/unstructured/ingest/connector/confluence.py` & `unstructured-0.8.8/unstructured/ingest/connector/confluence.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import math
 import os
 from dataclasses import dataclass
 from pathlib import Path
+from typing import Optional
 
 from atlassian import Confluence
 
 from unstructured.ingest.interfaces import (
     BaseConnector,
     BaseConnectorConfig,
     BaseIngestDoc,
@@ -27,15 +28,15 @@
     Check https://developer.atlassian.com/cloud/confluence/basic-auth-for-rest-apis/
     for more info on the api_token.
     """
 
     user_email: str
     api_token: str
     url: str
-    list_of_spaces: str
+    list_of_spaces: Optional[str]
     max_number_of_spaces: int
     max_number_of_docs_from_each_space: int
 
 
 @dataclass
 class ConfluenceFileMeta:
     """Metadata specifying:
```

### Comparing `unstructured-0.8.7/unstructured/ingest/connector/discord.py` & `unstructured-0.8.8/unstructured/ingest/connector/discord.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime as dt
 import os
 from dataclasses import dataclass
 from pathlib import Path
-from typing import List
+from typing import List, Optional
 
 from unstructured.ingest.interfaces import (
     BaseConnector,
     BaseConnectorConfig,
     BaseIngestDoc,
     ConnectorCleanupMixin,
     IngestDocCleanupMixin,
@@ -23,15 +23,15 @@
     """Connector config where channels is a comma separated list of
     Discord channels to pull messages from.
     """
 
     # Discord Specific Options
     channels: List[str]
     token: str
-    days: int
+    days: Optional[int]
     verbose: bool = False
 
     def __post_init__(self):
         if self.days:
             try:
                 self.days = int(self.days)
             except ValueError:
@@ -51,15 +51,15 @@
     doing the processing!).
     Also includes a cleanup method. When things go wrong and the cleanup
     method is not called, the file is left behind on the filesystem to assist debugging.
     """
 
     config: SimpleDiscordConfig
     channel: str
-    days: int
+    days: Optional[int]
     token: str
 
     # NOTE(crag): probably doesn't matter,  but intentionally not defining tmp_download_file
     # __post_init__ for multiprocessing simplicity (no Path objects in initially
     # instantiated object)
     def _tmp_download_file(self):
         channel_file = self.channel + ".txt"
```

### Comparing `unstructured-0.8.7/unstructured/ingest/connector/dropbox.py` & `unstructured-0.8.8/unstructured/ingest/connector/dropbox.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/ingest/connector/elasticsearch.py` & `unstructured-0.8.8/unstructured/ingest/connector/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/ingest/connector/fsspec.py` & `unstructured-0.8.8/unstructured/ingest/connector/fsspec.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 SUPPORTED_REMOTE_FSSPEC_PROTOCOLS = [
     "s3",
     "s3a",
     "abfs",
     "az",
     "gs",
     "gcs",
+    "box",
     "dropbox",
 ]
 
 
 @dataclass
 class SimpleFsspecConfig(BaseConnectorConfig):
     # fsspec specific options
```

### Comparing `unstructured-0.8.7/unstructured/ingest/connector/gcs.py` & `unstructured-0.8.8/unstructured/ingest/connector/gcs.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/ingest/connector/git.py` & `unstructured-0.8.8/unstructured/ingest/connector/git.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/ingest/connector/github.py` & `unstructured-0.8.8/unstructured/ingest/connector/github.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/ingest/connector/gitlab.py` & `unstructured-0.8.8/unstructured/ingest/connector/gitlab.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/ingest/connector/google_drive.py` & `unstructured-0.8.8/unstructured/ingest/connector/google_drive.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import io
 import json
 import os
 from dataclasses import dataclass
 from mimetypes import guess_extension
 from pathlib import Path
-from typing import Dict
+from typing import Dict, Optional
 
 from unstructured.file_utils.filetype import EXT_TO_FILETYPE
 from unstructured.file_utils.google_filetype import GOOGLE_DRIVE_EXPORT_TYPES
 from unstructured.ingest.interfaces import (
     BaseConnector,
     BaseConnectorConfig,
     BaseIngestDoc,
@@ -68,15 +68,15 @@
 class SimpleGoogleDriveConfig(BaseConnectorConfig):
     """Connector config where drive_id is the id of the document to process or
     the folder to process all documents from."""
 
     # Google Drive Specific Options
     drive_id: str
     service_account_key: str
-    extension: str
+    extension: Optional[str]
     recursive: bool = False
 
     def __post_init__(self):
         if self.extension and self.extension not in EXT_TO_FILETYPE.keys():
             raise ValueError(
                 f"Extension not supported. "
                 f"Value MUST be one of {', '.join([k for k in EXT_TO_FILETYPE if k is not None])}.",
```

### Comparing `unstructured-0.8.7/unstructured/ingest/connector/local.py` & `unstructured-0.8.8/unstructured/ingest/connector/local.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/ingest/connector/onedrive.py` & `unstructured-0.8.8/unstructured/ingest/connector/onedrive.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass, field
 from pathlib import Path
-from typing import TYPE_CHECKING, List
+from typing import TYPE_CHECKING, List, Optional
 
 from unstructured.file_utils.filetype import EXT_TO_FILETYPE
 from unstructured.ingest.interfaces import (
     BaseConnector,
     BaseConnectorConfig,
     BaseIngestDoc,
     ConnectorCleanupMixin,
@@ -22,22 +22,22 @@
 
 @dataclass
 class SimpleOneDriveConfig(BaseConnectorConfig):
     client_id: str
     client_credential: str = field(repr=False)
     user_pname: str
     tenant: str = field(repr=False)
-    authority_url: str = field(repr=False)
-    folder: str = field(default="")
+    authority_url: Optional[str] = field(repr=False)
+    folder: Optional[str] = field(default="")
     recursive: bool = False
 
     def __post_init__(self):
         if not (self.client_id and self.client_credential and self.user_pname):
             raise ValueError(
-                "Please provide one of the following mandatory values:"
+                "Please provide all the following mandatory values:"
                 "\n-ms-client_id\n-ms-client_cred\n-ms-user-pname",
             )
         self.token_factory = self._acquire_token
 
     @requires_dependencies(["msal"])
     def _acquire_token(self):
         from msal import ConfidentialClientApplication
```

### Comparing `unstructured-0.8.7/unstructured/ingest/connector/outlook.py` & `unstructured-0.8.8/unstructured/ingest/connector/outlook.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import hashlib
 import os
 from collections import defaultdict
 from dataclasses import dataclass, field
 from itertools import chain
 from pathlib import Path
-from typing import List
+from typing import List, Optional
 
 from office365.onedrive.driveitems.driveItem import DriveItem
 
 from unstructured.ingest.interfaces import (
     BaseConnector,
     BaseConnectorConfig,
     BaseIngestDoc,
@@ -26,27 +26,27 @@
     """There are no root folders with those names."""
 
 
 @dataclass
 class SimpleOutlookConfig(BaseConnectorConfig):
     """This class is getting the token."""
 
-    client_id: str
-    client_credential: str = field(repr=False)
+    client_id: Optional[str]
+    client_credential: Optional[str] = field(repr=False)
     user_email: str
-    tenant: str = field(repr=False)
-    authority_url: str = field(repr=False)
+    tenant: Optional[str] = field(repr=False)
+    authority_url: Optional[str] = field(repr=False)
     ms_outlook_folders: List[str]
     recursive: bool = False
 
     def __post_init__(self):
         if not (self.client_id and self.client_credential and self.user_email):
             raise ValueError(
                 "Please provide one of the following mandatory values:"
-                "\n--ms-client_id\n--ms-client_cred\n--ms-user-email",
+                "\n--client_id\n--client_cred\n--user-email",
             )
         self.token_factory = self._acquire_token
 
     @requires_dependencies(["msal"])
     def _acquire_token(self):
         from msal import ConfidentialClientApplication
```

### Comparing `unstructured-0.8.7/unstructured/ingest/connector/reddit.py` & `unstructured-0.8.8/unstructured/ingest/connector/reddit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from dataclasses import dataclass, field
 from pathlib import Path
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional
 
 from unstructured.ingest.interfaces import (
     BaseConnector,
     BaseConnectorConfig,
     BaseIngestDoc,
     ConnectorCleanupMixin,
     IngestDocCleanupMixin,
@@ -17,18 +17,18 @@
 if TYPE_CHECKING:
     from praw.models import Submission
 
 
 @dataclass
 class SimpleRedditConfig(BaseConnectorConfig):
     subreddit_name: str
-    client_id: str
-    client_secret: str
+    client_id: Optional[str]
+    client_secret: Optional[str]
     user_agent: str
-    search_query: str
+    search_query: Optional[str]
     num_posts: int
 
     def __post_init__(self):
         if self.num_posts <= 0:
             raise ValueError("The number of Reddit posts to fetch must be positive.")
```

### Comparing `unstructured-0.8.7/unstructured/ingest/connector/s3.py` & `unstructured-0.8.8/unstructured/ingest/connector/s3.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/ingest/connector/slack.py` & `unstructured-0.8.8/unstructured/ingest/connector/slack.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from dataclasses import dataclass
 from datetime import datetime
 from pathlib import Path
-from typing import List
+from typing import List, Optional
 
 from unstructured.ingest.interfaces import (
     BaseConnector,
     BaseConnectorConfig,
     BaseIngestDoc,
     ConnectorCleanupMixin,
     IngestDocCleanupMixin,
@@ -23,16 +23,16 @@
 
 @dataclass
 class SimpleSlackConfig(BaseConnectorConfig):
     """Connector config to process all messages by channel id's."""
 
     channels: List[str]
     token: str
-    oldest: str
-    latest: str
+    oldest: Optional[str]
+    latest: Optional[str]
     verbose: bool = False
 
     def validate_inputs(self):
         oldest_valid = True
         latest_valid = True
 
         if self.oldest:
@@ -64,16 +64,16 @@
     Also includes a cleanup method. When things go wrong and the cleanup
     method is not called, the file is left behind on the filesystem to assist debugging.
     """
 
     config: SimpleSlackConfig
     channel: str
     token: str
-    oldest: str
-    latest: str
+    oldest: Optional[str]
+    latest: Optional[str]
 
     # NOTE(crag): probably doesn't matter,  but intentionally not defining tmp_download_file
     # __post_init__ for multiprocessing simplicity (no Path objects in initially
     # instantiated object)
     def _tmp_download_file(self):
         channel_file = self.channel + ".txt"
         return Path(self.standard_config.download_dir) / channel_file
```

### Comparing `unstructured-0.8.7/unstructured/ingest/connector/wikipedia.py` & `unstructured-0.8.8/unstructured/ingest/connector/wikipedia.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/ingest/doc_processor/generalized.py` & `unstructured-0.8.8/unstructured/ingest/doc_processor/generalized.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/ingest/interfaces.py` & `unstructured-0.8.8/unstructured/ingest/interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,26 @@
 from unstructured.documents.elements import DataSourceMetadata
 from unstructured.ingest.logger import logger
 from unstructured.partition.auto import partition
 from unstructured.staging.base import convert_to_dict
 
 
 @dataclass
+class ProcessorConfigs:
+    """Common set of config required when running data connectors."""
+
+    partition_strategy: str
+    partition_ocr_languages: str
+    encoding: str
+    num_processes: int
+    reprocess: bool
+    max_docs: int
+
+
+@dataclass
 class StandardConnectorConfig:
     """Common set of config options passed to all connectors."""
 
     # where raw documents are stored for processing, and then removed if not preserve_downloads
     download_dir: str
     # where to write structured data outputs
     output_dir: str
```

### Comparing `unstructured-0.8.7/unstructured/nlp/english-words.txt` & `unstructured-0.8.8/unstructured/nlp/english-words.txt`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/nlp/english_words.py` & `unstructured-0.8.8/unstructured/nlp/english_words.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/nlp/patterns.py` & `unstructured-0.8.8/unstructured/nlp/patterns.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/nlp/tokenize.py` & `unstructured-0.8.8/unstructured/nlp/tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/partition/__init__.py` & `unstructured-0.8.8/unstructured/partition/__init__.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/partition/api.py` & `unstructured-0.8.8/unstructured/partition/api.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/partition/auto.py` & `unstructured-0.8.8/unstructured/partition/auto.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/partition/common.py` & `unstructured-0.8.8/unstructured/partition/common.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/partition/csv.py` & `unstructured-0.8.8/unstructured/partition/csv.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,29 +21,29 @@
 
 @process_metadata()
 @add_metadata_with_filetype(FileType.CSV)
 def partition_csv(
     filename: Optional[str] = None,
     file: Optional[Union[IO[bytes], SpooledTemporaryFile]] = None,
     metadata_filename: Optional[str] = None,
-    metadata_date: Optional[str] = None,
+    metadata_last_modified: Optional[str] = None,
     include_metadata: bool = True,
     **kwargs,
 ) -> List[Element]:
     """Partitions Microsoft Excel Documents in .csv format into its document elements.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
     metadata_filename
         The filename to use for the metadata.
-    metadata_date
+    metadata_last_modified
         The last modified date for the document.
     include_metadata
         Determines whether or not metadata is included in the output.
     """
     exactly_one(filename=filename, file=file)
 
     if filename:
@@ -60,13 +60,13 @@
     html_text = table.to_html(index=False, header=False, na_rep="")
     text = lxml.html.document_fromstring(html_text).text_content()
 
     if include_metadata:
         metadata = ElementMetadata(
             text_as_html=html_text,
             filename=metadata_filename or filename,
-            date=metadata_date or last_modification_date,
+            last_modified=metadata_last_modified or last_modification_date,
         )
     else:
         metadata = ElementMetadata()
 
     return [Table(text=text, metadata=metadata)]
```

### Comparing `unstructured-0.8.7/unstructured/partition/doc.py` & `unstructured-0.8.8/unstructured/partition/doc.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,27 +17,27 @@
 @add_metadata_with_filetype(FileType.DOC)
 def partition_doc(
     filename: Optional[str] = None,
     file: Optional[IO[bytes]] = None,
     include_page_breaks: bool = True,
     include_metadata: bool = True,
     metadata_filename: Optional[str] = None,
-    metadata_date: Optional[str] = None,
+    metadata_last_modified: Optional[str] = None,
     libre_office_filter: Optional[str] = "MS Word 2007 XML",
     **kwargs,
 ) -> List[Element]:
     """Partitions Microsoft Word Documents in .doc format into its document elements.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
-    metadata_date
+    metadata_last_modified
         The last modified date for the document.
     libre_office_filter
         The filter to use when coverting to .doc. The default is the
         filter that is required when using LibreOffice7. Pass in None
         if you do not want to apply any filter.
     """
     # Verify that only one of the arguments was provided
@@ -72,15 +72,15 @@
         )
         docx_filename = os.path.join(tmpdir, f"{base_filename}.docx")
         elements = partition_docx(
             filename=docx_filename,
             metadata_filename=metadata_filename,
             include_page_breaks=include_page_breaks,
             include_metadata=include_metadata,
-            metadata_date=metadata_date or last_modification_date,
+            metadata_last_modified=metadata_last_modified or last_modification_date,
         )
         # remove tmp.name from filename if parsing file
         if file:
             for element in elements:
                 element.metadata.filename = metadata_filename
 
     return elements
```

### Comparing `unstructured-0.8.7/unstructured/partition/docx.py` & `unstructured-0.8.8/unstructured/partition/docx.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,30 +109,30 @@
 @add_metadata_with_filetype(FileType.DOCX)
 def partition_docx(
     filename: Optional[str] = None,
     file: Optional[Union[IO[bytes], SpooledTemporaryFile]] = None,
     metadata_filename: Optional[str] = None,
     include_page_breaks: bool = True,
     include_metadata: bool = True,
-    metadata_date: Optional[str] = None,
+    metadata_last_modified: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
     """Partitions Microsoft Word Documents in .docx format into its document elements.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
     metadata_filename
         The filename to use for the metadata. Relevant because partition_doc converts the
         document to .docx before partition. We want the original source filename in the
         metadata.
-    metadata_date
+    metadata_last_modified
         The last modified date for the document.
     """
 
     # Verify that only one of the arguments was provided
     exactly_one(filename=filename, file=file)
 
     last_modification_date = None
@@ -168,28 +168,28 @@
             text_table = convert_ms_office_table_to_text(table, as_html=False)
             element = Table(text_table)
             if element is not None:
                 element.metadata = ElementMetadata(
                     text_as_html=html_table,
                     filename=metadata_filename,
                     page_number=page_number,
-                    date=metadata_date or last_modification_date,
+                    last_modified=metadata_last_modified or last_modification_date,
                 )
                 elements.append(element)
             table_index += 1
         elif element_item.tag.endswith("p"):
             if "<w:numPr>" in element_item.xml:
                 is_list = True
             paragraph = docx.text.paragraph.Paragraph(element_item, document)
             para_element: Optional[Text] = _paragraph_to_element(paragraph, is_list)
             if para_element is not None:
                 para_element.metadata = ElementMetadata(
                     filename=metadata_filename,
                     page_number=page_number,
-                    date=metadata_date or last_modification_date,
+                    last_modified=metadata_last_modified or last_modification_date,
                 )
                 elements.append(para_element)
             is_list = False
         elif element_item.tag.endswith("sectPr"):
             if len(headers_and_footers) > section:
                 footers = headers_and_footers[section][1]
                 elements.extend(footers)
@@ -308,15 +308,15 @@
 
 def convert_and_partition_docx(
     source_format: str,
     filename: Optional[str] = None,
     file: Optional[IO[bytes]] = None,
     include_metadata: bool = True,
     metadata_filename: Optional[str] = None,
-    metadata_date: Optional[str] = None,
+    metadata_last_modified: Optional[str] = None,
 ) -> List[Element]:
     """Converts a document to DOCX and then partitions it using partition_html. Works with
     any file format support by pandoc.
 
     Parameters
     ----------
     source_format
@@ -355,11 +355,11 @@
             format=source_format,
             outputfile=docx_filename,
         )
         elements = partition_docx(
             filename=docx_filename,
             metadata_filename=metadata_filename,
             include_metadata=include_metadata,
-            metadata_date=metadata_date,
+            metadata_last_modified=metadata_last_modified,
         )
 
     return elements
```

### Comparing `unstructured-0.8.7/unstructured/partition/email.py` & `unstructured-0.8.8/unstructured/partition/email.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 
     return elements
 
 
 def build_email_metadata(
     msg: Message,
     filename: Optional[str],
-    metadata_date: Optional[str] = None,
+    metadata_last_modified: Optional[str] = None,
 ) -> ElementMetadata:
     """Creates an ElementMetadata object from the header information in the email."""
     header_dict = dict(msg.raw_items())
     email_date = header_dict.get("Date")
     if email_date is not None:
         email_date = convert_to_iso_8601(email_date)
 
@@ -127,15 +127,15 @@
     if sent_to is not None:
         sent_to = [recipient.strip() for recipient in sent_to.split(",")]
 
     return ElementMetadata(
         sent_to=sent_to,
         sent_from=sent_from,
         subject=header_dict.get("Subject"),
-        date=metadata_date or email_date,
+        last_modified=metadata_last_modified or email_date,
         filename=filename,
     )
 
 
 def convert_to_iso_8601(time: str) -> Optional[str]:
     """Converts the datetime from the email output to ISO-8601 format."""
     cleaned_time = clean_extra_whitespace(time)
@@ -238,15 +238,15 @@
     text: Optional[str] = None,
     content_source: str = "text/html",
     encoding: Optional[str] = None,
     include_headers: bool = False,
     max_partition: Optional[int] = 1500,
     include_metadata: bool = True,
     metadata_filename: Optional[str] = None,
-    metadata_date: Optional[str] = None,
+    metadata_last_modified: Optional[str] = None,
     process_attachments: bool = False,
     attachment_partitioner: Optional[Callable] = None,
     min_partition: Optional[int] = 0,
     **kwargs,
 ) -> List[Element]:
     """Partitions an .eml documents into its constituent elements.
     Parameters
@@ -263,15 +263,15 @@
     encoding
         The encoding method used to decode the text input. If None, utf-8 will be used.
     max_partition
         The maximum number of characters to include in a partition. If None is passed,
         no maximum is applied. Only applies if processing the text/plain content.
     metadata_filename
         The filename to use for the metadata.
-    metadata_date
+    metadata_last_modified
         The last modified date for the document.
     process_attachments
         If True, partition_email will process email attachments in addition to
         processing the content of the email itself.
     attachment_partitioner
         The partitioning function to use to process attachments.
     min_partition
@@ -388,15 +388,15 @@
     if include_headers:
         header = partition_email_header(msg)
     all_elements = header + elements
 
     metadata = build_email_metadata(
         msg,
         filename=metadata_filename or filename,
-        metadata_date=metadata_date,
+        metadata_last_modified=metadata_last_modified,
     )
     for element in all_elements:
         element.metadata = metadata
 
     if process_attachments:
         with TemporaryDirectory() as tmpdir:
             extract_attachment_info(msg, tmpdir)
```

### Comparing `unstructured-0.8.7/unstructured/partition/epub.py` & `unstructured-0.8.8/unstructured/partition/epub.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,33 +9,33 @@
 @add_metadata_with_filetype(FileType.EPUB)
 def partition_epub(
     filename: Optional[str] = None,
     file: Optional[IO[bytes]] = None,
     include_page_breaks: bool = False,
     include_metadata: bool = True,
     metadata_filename: Optional[str] = None,
-    metadata_date: Optional[str] = None,
+    metadata_last_modified: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
     """Partitions an EPUB document. The document is first converted to HTML and then
     partitoned using partiton_html.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
     include_page_breaks
         If True, the output will include page breaks if the filetype supports it
-    metadata_date
+    metadata_last_modified
         The last modified date for the document.
 
     """
     return convert_and_partition_html(
         source_format="epub",
         filename=filename,
         file=file,
         include_page_breaks=include_page_breaks,
         metadata_filename=metadata_filename,
-        metadata_date=metadata_date,
+        metadata_last_modified=metadata_last_modified,
     )
```

### Comparing `unstructured-0.8.7/unstructured/partition/html.py` & `unstructured-0.8.8/unstructured/partition/html.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     include_page_breaks: bool = False,
     include_metadata: bool = True,
     headers: Dict[str, str] = {},
     ssl_verify: bool = True,
     parser: VALID_PARSERS = None,
     html_assemble_articles: bool = False,
     metadata_filename: Optional[str] = None,
-    metadata_date: Optional[str] = None,
+    metadata_last_modified: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
     """Partitions an HTML document into its constituent elements.
 
     Parameters
     ----------
     filename
@@ -59,15 +59,15 @@
     headers
         The headers to be used in conjunction with the HTTP request if URL is set.
     ssl_verify
         If the URL parameter is set, determines whether or not partition uses SSL verification
         in the HTTP request.
     parser
         The parser to use for parsing the HTML document. If None, default parser will be used.
-    metadata_date
+    metadata_last_modified
         The last modified date for the document.
     """
     if text is not None and text.strip() == "" and not file and not filename and not url:
         return []
     # Verify that only one of the arguments was provided
     exactly_one(filename=filename, file=file, text=text, url=url)
 
@@ -108,25 +108,25 @@
             raise ValueError(f"Expected content type text/html. Got {content_type}.")
 
         document = HTMLDocument.from_string(response.text, parser=parser)
 
     return document_to_element_list(
         document,
         include_page_breaks=include_page_breaks,
-        last_modification_date=metadata_date or last_modification_date,
+        last_modification_date=metadata_last_modified or last_modification_date,
     )
 
 
 def convert_and_partition_html(
     source_format: str,
     filename: Optional[str] = None,
     file: Optional[IO[bytes]] = None,
     include_page_breaks: bool = False,
     metadata_filename: Optional[str] = None,
-    metadata_date: Optional[str] = None,
+    metadata_last_modified: Optional[str] = None,
 ) -> List[Element]:
     """Converts a document to HTML and then partitions it using partition_html. Works with
     any file format support by pandoc.
 
     Parameters
     ----------
     source_format
@@ -156,9 +156,9 @@
     # NOTE(robinson) - pypandoc returns a text string with unicode encoding
     # ref: https://github.com/JessicaTegner/pypandoc#usage
     return partition_html(
         text=html_text,
         include_page_breaks=include_page_breaks,
         encoding="unicode",
         metadata_filename=metadata_filename,
-        metadata_date=metadata_date or last_modification_date,
+        metadata_last_modified=metadata_last_modified or last_modification_date,
     )
```

### Comparing `unstructured-0.8.7/unstructured/partition/image.py` & `unstructured-0.8.8/unstructured/partition/image.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def partition_image(
     filename: str = "",
     file: Optional[bytes] = None,
     include_page_breaks: bool = False,
     infer_table_structure: bool = False,
     ocr_languages: str = "eng",
     strategy: str = "auto",
-    metadata_date: Optional[str] = None,
+    metadata_last_modified: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
     """Parses an image into a list of interpreted elements.
 
     Parameters
     ----------
     filename
@@ -39,23 +39,23 @@
     strategy
         The strategy to use for partitioning the image. Valid strategies are "hi_res" and
         "ocr_only". When using the "hi_res" strategy, the function uses a layout detection
         model if to identify document elements. When using the "ocr_only" strategy,
         partition_image simply extracts the text from the document using OCR and processes it.
         The default strategy `auto` will determine when a image can be extracted using
         `ocr_only` mode, otherwise it will fall back to `hi_res`.
-    metadata_date
+    metadata_last_modified
         The last modified date for the document.
 
     """
     exactly_one(filename=filename, file=file)
 
     return partition_pdf_or_image(
         filename=filename,
         file=file,
         is_image=True,
         include_page_breaks=include_page_breaks,
         infer_table_structure=infer_table_structure,
         ocr_languages=ocr_languages,
         strategy=strategy,
-        metadata_date=metadata_date,
+        metadata_last_modified=metadata_last_modified,
     )
```

### Comparing `unstructured-0.8.7/unstructured/partition/json.py` & `unstructured-0.8.8/unstructured/partition/json.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,28 +19,28 @@
 @add_metadata_with_filetype(FileType.JSON)
 def partition_json(
     filename: Optional[str] = None,
     file: Optional[IO[bytes]] = None,
     text: Optional[str] = None,
     include_metadata: bool = True,
     metadata_filename: Optional[str] = None,
-    metadata_date: Optional[str] = None,
+    metadata_last_modified: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
     """Partitions an .json document into its constituent elements.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object as bytes --> open(filename, "rb").
     text
         The string representation of the .json document.
-    metadata_date
+    metadata_last_modified
         The last modified date for the document.
     """
     if text is not None and text.strip() == "" and not file and not filename:
         return []
 
     exactly_one(filename=filename, file=file, text=text)
 
@@ -71,12 +71,12 @@
     try:
         dict = json.loads(file_text)
         elements = dict_to_elements(dict)
     except json.JSONDecodeError:
         raise ValueError("Not a valid json")
 
     for element in elements:
-        element.metadata.date = metadata_date or last_modification_date
+        element.metadata.last_modified = metadata_last_modified or last_modification_date
     # NOTE(Nathan): in future PR, try extracting items that look like text
     #               if file_text is a valid json but not an unstructured json
 
     return elements
```

### Comparing `unstructured-0.8.7/unstructured/partition/md.py` & `unstructured-0.8.8/unstructured/partition/md.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     file: Optional[IO[bytes]] = None,
     text: Optional[str] = None,
     url: Optional[str] = None,
     include_page_breaks: bool = False,
     include_metadata: bool = True,
     parser: VALID_PARSERS = None,
     metadata_filename: Optional[str] = None,
-    metadata_date: Optional[str] = None,
+    metadata_last_modified: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
     """Partitions a markdown file into its constituent elements
 
     Parameters
     ----------
     filename
@@ -48,15 +48,15 @@
         The URL of a webpage to parse. Only for URLs that return a markdown document.
     include_page_breaks
         If True, the output will include page breaks if the filetype supports it.
     include_metadata
         Determines whether or not metadata is included in the output.
     parser
         The parser to use for parsing the markdown document. If None, default parser will be used.
-    metadata_date
+    metadata_last_modified
         The last modified date for the document.
     """
     # Verify that only one of the arguments was provided
     if text is None:
         text = ""
     exactly_one(filename=filename, file=file, text=text, url=url)
 
@@ -87,9 +87,9 @@
 
     return partition_html(
         text=html,
         include_page_breaks=include_page_breaks,
         include_metadata=include_metadata,
         parser=parser,
         metadata_filename=metadata_filename,
-        metadata_date=metadata_date or last_modification_date,
+        metadata_last_modified=metadata_last_modified or last_modification_date,
     )
```

### Comparing `unstructured-0.8.7/unstructured/partition/msg.py` & `unstructured-0.8.8/unstructured/partition/msg.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 @add_metadata_with_filetype(FileType.MSG)
 def partition_msg(
     filename: Optional[str] = None,
     file: Optional[IO[bytes]] = None,
     max_partition: Optional[int] = 1500,
     include_metadata: bool = True,
     metadata_filename: Optional[str] = None,
-    metadata_date: Optional[str] = None,
+    metadata_last_modified: Optional[str] = None,
     process_attachments: bool = False,
     attachment_partitioner: Optional[Callable] = None,
     min_partition: Optional[int] = 0,
     **kwargs,
 ) -> List[Element]:
     """Partitions a MSFT Outlook .msg file
 
@@ -40,15 +40,15 @@
     metadata_filename
         The filename to use for the metadata.
     process_attachments
         If True, partition_email will process email attachments in addition to
         processing the content of the email itself.
     attachment_partitioner
         The partitioning function to use to process attachments.
-    metadata_date
+    metadata_last_modified
         The last modified date for the document.
     min_partition
         The minimum number of characters to include in a partition. Only applies if
         processing text/plain content.
     """
     exactly_one(filename=filename, file=file)
 
@@ -69,15 +69,15 @@
             max_partition=max_partition,
             min_partition=min_partition,
         )
 
     metadata = build_msg_metadata(
         msg_obj,
         metadata_filename or filename,
-        metadata_date=metadata_date,
+        metadata_last_modified=metadata_last_modified,
     )
     for element in elements:
         element.metadata = metadata
 
     if process_attachments:
         with tempfile.TemporaryDirectory() as tmpdir:
             extract_msg_attachment_info(msg_obj=msg_obj, output_dir=tmpdir)
@@ -97,15 +97,15 @@
 
     return elements
 
 
 def build_msg_metadata(
     msg_obj: msg_parser.MsOxMessage,
     filename: Optional[str],
-    metadata_date: Optional[str],
+    metadata_last_modified: Optional[str],
 ) -> ElementMetadata:
     """Creates an ElementMetadata object from the header information in the email."""
     email_date = getattr(msg_obj, "sent_date", None)
     if email_date is not None:
         email_date = convert_to_iso_8601(email_date)
 
     sent_from = getattr(msg_obj, "sender", None)
@@ -116,15 +116,15 @@
     if sent_to is not None:
         sent_to = [str(recipient) for recipient in sent_to]
 
     return ElementMetadata(
         sent_to=sent_to,
         sent_from=sent_from,
         subject=getattr(msg_obj, "subject", None),
-        date=metadata_date or email_date,
+        last_modified=metadata_last_modified or email_date,
         filename=filename,
     )
 
 
 def extract_msg_attachment_info(
     filename: Optional[str] = None,
     file: Optional[IO[bytes]] = None,
```

### Comparing `unstructured-0.8.7/unstructured/partition/odt.py` & `unstructured-0.8.8/unstructured/partition/odt.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,35 +12,35 @@
 @process_metadata()
 @add_metadata_with_filetype(FileType.ODT)
 def partition_odt(
     filename: Optional[str] = None,
     file: Optional[IO[bytes]] = None,
     include_metadata: bool = True,
     metadata_filename: Optional[str] = None,
-    metadata_date: Optional[str] = None,
+    metadata_last_modified: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
     """Partitions Open Office Documents in .odt format into its document elements.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
-    metadata_date
+    metadata_last_modified
         The last modified date for the document.
     """
 
     last_modification_date = None
     if filename:
         last_modification_date = get_last_modified_date(filename)
     elif file:
         last_modification_date = get_last_modified_date_from_file(file)
 
     return convert_and_partition_docx(
         source_format="odt",
         filename=filename,
         file=file,
         metadata_filename=metadata_filename,
-        metadata_date=metadata_date or last_modification_date,
+        metadata_last_modified=metadata_last_modified or last_modification_date,
     )
```

### Comparing `unstructured-0.8.7/unstructured/partition/org.py` & `unstructured-0.8.8/unstructured/partition/rst.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 from typing import IO, List, Optional
 
-from unstructured.documents.elements import Element
+from unstructured.documents.elements import Element, process_metadata
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.partition.html import convert_and_partition_html
 
 
-@add_metadata_with_filetype(FileType.ORG)
-def partition_org(
+@process_metadata()
+@add_metadata_with_filetype(FileType.RST)
+def partition_rst(
     filename: Optional[str] = None,
     file: Optional[IO[bytes]] = None,
     include_page_breaks: bool = False,
     include_metadata: bool = True,
     metadata_filename: Optional[str] = None,
-    metadata_date: Optional[str] = None,
+    metadata_last_modified: Optional[str] = None,
+    **kwargs,
 ) -> List[Element]:
-    """Partitions an org document. The document is first converted to HTML and then
+    """Partitions an RST document. The document is first converted to HTML and then
     partitioned using partition_html.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
     include_page_breaks
-        If True, the output will include page breaks if the filetype supports it
-    metadata_date
+        If True, the output will include page breaks if the filetype supports it.
+    metadata_last_modified
         The last modified date for the document.
     """
     return convert_and_partition_html(
-        source_format="org",
+        source_format="rst",
         filename=filename,
         file=file,
         include_page_breaks=include_page_breaks,
         metadata_filename=metadata_filename,
-        metadata_date=metadata_date,
+        metadata_last_modified=metadata_last_modified,
     )
```

### Comparing `unstructured-0.8.7/unstructured/partition/pdf.py` & `unstructured-0.8.8/unstructured/partition/pdf.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     strategy: str = "auto",
     infer_table_structure: bool = False,
     ocr_languages: str = "eng",
     max_partition: Optional[int] = 1500,
     min_partition: Optional[int] = 0,
     include_metadata: bool = True,
     metadata_filename: Optional[str] = None,
-    metadata_date: Optional[str] = None,
+    metadata_last_modified: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
     """Parses a pdf document into a list of interpreted elements.
     Parameters
     ----------
     filename
         A string defining the target filename path.
@@ -84,43 +84,43 @@
         to isntall the appropriate Tesseract language pack.
     max_partition
         The maximum number of characters to include in a partition. If None is passed,
         no maximum is applied. Only applies to the "ocr_only" strategy.
     min_partition
         The minimum number of characters to include in a partition. Only applies if
         processing text/plain content.
-    metadata_date
+    metadata_last_modified
         The last modified date for the document.
     """
     exactly_one(filename=filename, file=file)
     return partition_pdf_or_image(
         filename=filename,
         file=file,
         include_page_breaks=include_page_breaks,
         strategy=strategy,
         infer_table_structure=infer_table_structure,
         ocr_languages=ocr_languages,
         max_partition=max_partition,
         min_partition=min_partition,
-        metadata_date=metadata_date,
+        metadata_last_modified=metadata_last_modified,
         **kwargs,
     )
 
 
 def extractable_elements(
     filename: str = "",
     file: Optional[Union[bytes, BinaryIO, SpooledTemporaryFile]] = None,
     include_page_breaks: bool = False,
-    metadata_date: Optional[str] = None,
+    metadata_last_modified: Optional[str] = None,
 ):
     return _partition_pdf_with_pdfminer(
         filename=filename,
         file=file,
         include_page_breaks=include_page_breaks,
-        metadata_date=metadata_date,
+        metadata_last_modified=metadata_last_modified,
     )
 
 
 def get_the_last_modification_date_pdf_or_img(
     file: Optional[Union[bytes, BinaryIO, SpooledTemporaryFile]] = None,
     filename: Optional[str] = "",
 ) -> Union[str, None]:
@@ -138,15 +138,15 @@
     is_image: bool = False,
     include_page_breaks: bool = False,
     strategy: str = "auto",
     infer_table_structure: bool = False,
     ocr_languages: str = "eng",
     max_partition: Optional[int] = 1500,
     min_partition: Optional[int] = 0,
-    metadata_date: Optional[str] = None,
+    metadata_last_modified: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
     """Parses a pdf or image document into a list of interpreted elements."""
     # TODO(alan): Extract information about the filetype to be processed from the template
     # route. Decoding the routing should probably be handled by a single function designed for
     # that task so as routing design changes, those changes are implemented in a single
     # function.
@@ -156,15 +156,15 @@
         filename=filename,
     )
     if not is_image:
         extracted_elements = extractable_elements(
             filename=filename,
             file=spooled_to_bytes_io_if_needed(file),
             include_page_breaks=include_page_breaks,
-            metadata_date=metadata_date or last_modification_date,
+            metadata_last_modified=metadata_last_modified or last_modification_date,
         )
         pdf_text_extractable = any(
             isinstance(el, Text) and el.text.strip() for el in extracted_elements
         )
     else:
         pdf_text_extractable = False
 
@@ -184,15 +184,15 @@
             layout_elements = _partition_pdf_or_image_local(
                 filename=filename,
                 file=spooled_to_bytes_io_if_needed(file),
                 is_image=is_image,
                 infer_table_structure=infer_table_structure,
                 include_page_breaks=include_page_breaks,
                 ocr_languages=ocr_languages,
-                metadata_date=metadata_date or last_modification_date,
+                metadata_last_modified=metadata_last_modified or last_modification_date,
                 **kwargs,
             )
 
     elif strategy == "fast":
         return extracted_elements
 
     elif strategy == "ocr_only":
@@ -202,29 +202,29 @@
                 filename=filename,
                 file=file,
                 include_page_breaks=include_page_breaks,
                 ocr_languages=ocr_languages,
                 is_image=is_image,
                 max_partition=max_partition,
                 min_partition=min_partition,
-                metadata_date=metadata_date or last_modification_date,
+                metadata_last_modified=metadata_last_modified or last_modification_date,
             )
     return layout_elements
 
 
 @requires_dependencies("unstructured_inference")
 def _partition_pdf_or_image_local(
     filename: str = "",
     file: Optional[Union[bytes, BinaryIO]] = None,
     is_image: bool = False,
     infer_table_structure: bool = False,
     include_page_breaks: bool = False,
     ocr_languages: str = "eng",
     model_name: Optional[str] = None,
-    metadata_date: Optional[str] = None,
+    metadata_last_modified: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
     """Partition using package installed locally."""
     from unstructured_inference.inference.layout import (
         process_data_with_model,
         process_file_with_model,
     )
@@ -252,15 +252,15 @@
             extract_tables=infer_table_structure,
             model_name=model_name,
         )
     elements = document_to_element_list(
         layout,
         include_page_breaks=include_page_breaks,
         sort=False,
-        last_modification_date=metadata_date,
+        last_modification_date=metadata_last_modified,
     )
     out_elements = []
 
     for el in elements:
         if (isinstance(el, PageBreak) and not include_page_breaks) or (
             # NOTE(crag): small chunks of text from Image elements tend to be garbage
             isinstance(el, Image)
@@ -281,15 +281,15 @@
 
 
 @requires_dependencies("pdfminer", "local-inference")
 def _partition_pdf_with_pdfminer(
     filename: str = "",
     file: Optional[BinaryIO] = None,
     include_page_breaks: bool = False,
-    metadata_date: Optional[str] = None,
+    metadata_last_modified: Optional[str] = None,
 ) -> List[Element]:
     """Partitions a PDF using PDFMiner instead of using a layoutmodel. Used for faster
     processing or detectron2 is not available.
 
     Implementation is based on the `extract_text` implemenation in pdfminer.six, but
     modified to support tracking page numbers and working with file-like objects.
 
@@ -299,24 +299,24 @@
     if filename:
         with open_filename(filename, "rb") as fp:
             fp = cast(BinaryIO, fp)
             elements = _process_pdfminer_pages(
                 fp=fp,
                 filename=filename,
                 include_page_breaks=include_page_breaks,
-                metadata_date=metadata_date,
+                metadata_last_modified=metadata_last_modified,
             )
 
     elif file:
         fp = cast(BinaryIO, file)
         elements = _process_pdfminer_pages(
             fp=fp,
             filename=filename,
             include_page_breaks=include_page_breaks,
-            metadata_date=metadata_date,
+            metadata_last_modified=metadata_last_modified,
         )
 
     return elements
 
 
 def _extract_text(item: LTItem) -> str:
     """Recursively extracts text from PDFMiner objects to account
@@ -337,15 +337,15 @@
     return "\n"
 
 
 def _process_pdfminer_pages(
     fp: BinaryIO,
     filename: str = "",
     include_page_breaks: bool = False,
-    metadata_date: Optional[str] = None,
+    metadata_last_modified: Optional[str] = None,
 ):
     """Uses PDF miner to split a document into pages and process them."""
     elements: List[Element] = []
 
     for i, page in enumerate(extract_pages(fp)):  # type: ignore
         width, height = page.width, page.height
 
@@ -380,15 +380,15 @@
                         points=points,
                         system=coordinate_system,
                     )
                     element.metadata = ElementMetadata(
                         filename=filename,
                         page_number=i + 1,
                         coordinates=coordinates_metadata,
-                        date=metadata_date,
+                        last_modified=metadata_last_modified,
                     )
                     page_elements.append(element)
 
         sorted_page_elements = sorted(
             page_elements,
             key=lambda el: (
                 el.metadata.coordinates.points[0][1] if el.metadata.coordinates else float("inf"),
@@ -443,15 +443,15 @@
     filename: str = "",
     file: Optional[Union[bytes, BinaryIO, SpooledTemporaryFile]] = None,
     include_page_breaks: bool = False,
     ocr_languages: str = "eng",
     is_image: bool = False,
     max_partition: Optional[int] = 1500,
     min_partition: Optional[int] = 0,
-    metadata_date: Optional[str] = None,
+    metadata_last_modified: Optional[str] = None,
 ):
     """Partitions and image or PDF using Tesseract OCR. For PDFs, each page is converted
     to an image prior to processing."""
     import pytesseract
 
     if is_image:
         if file is not None:
@@ -459,26 +459,26 @@
             text = pytesseract.image_to_string(image, config=f"-l '{ocr_languages}'")
         else:
             text = pytesseract.image_to_string(filename, config=f"-l '{ocr_languages}'")
         elements = partition_text(
             text=text,
             max_partition=max_partition,
             min_partition=min_partition,
-            metadata_date=metadata_date,
+            metadata_last_modified=metadata_last_modified,
         )
 
     else:
         elements = []
         page_number = 0
         for image in convert_pdf_to_images(filename, file):
             page_number += 1
             metadata = ElementMetadata(
                 filename=filename,
                 page_number=page_number,
-                date=metadata_date,
+                last_modified=metadata_last_modified,
             )
             text = pytesseract.image_to_string(image, config=f"-l '{ocr_languages}'")
 
             _elements = partition_text(
                 text=text,
                 max_partition=max_partition,
                 min_partition=min_partition,
```

### Comparing `unstructured-0.8.7/unstructured/partition/ppt.py` & `unstructured-0.8.8/unstructured/partition/ppt.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,28 +17,28 @@
 @add_metadata_with_filetype(FileType.PPT)
 def partition_ppt(
     filename: Optional[str] = None,
     file: Optional[IO[bytes]] = None,
     include_page_breaks: bool = False,
     include_metadata: bool = True,
     metadata_filename: Optional[str] = None,
-    metadata_date: Optional[str] = None,
+    metadata_last_modified: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
     """Partitions Microsoft PowerPoint Documents in .ppt format into their document elements.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
     include_page_breaks
         If True, includes a PageBreak element between slides
-    metadata_date
+    metadata_last_modified
         The last modified date for the document.
     """
     # Verify that only one of the arguments was provided
     if filename is None:
         filename = ""
     exactly_one(filename=filename, file=file)
 
@@ -67,15 +67,15 @@
             target_format="pptx",
             target_filter="Impress MS PowerPoint 2007 XML",
         )
         pptx_filename = os.path.join(tmpdir, f"{base_filename}.pptx")
         elements = partition_pptx(
             filename=pptx_filename,
             metadata_filename=metadata_filename,
-            metadata_date=metadata_date or last_modification_date,
+            metadata_last_modified=metadata_last_modified or last_modification_date,
         )
 
     # remove tmp.name from filename if parsing file
     if file:
         for element in elements:
             element.metadata.filename = metadata_filename
```

### Comparing `unstructured-0.8.7/unstructured/partition/pptx.py` & `unstructured-0.8.8/unstructured/partition/pptx.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 @add_metadata_with_filetype(FileType.PPTX)
 def partition_pptx(
     filename: Optional[str] = None,
     file: Optional[Union[IO[bytes], SpooledTemporaryFile]] = None,
     include_page_breaks: bool = True,
     metadata_filename: Optional[str] = None,
     include_metadata: bool = True,
-    metadata_date: Optional[str] = None,
+    metadata_last_modified: Optional[str] = None,
     include_slide_notes: bool = False,
     **kwargs,
 ) -> List[Element]:
     """Partitions Microsoft PowerPoint Documents in .pptx format into its document elements.
 
     Parameters
     ----------
@@ -52,15 +52,15 @@
         A file-like object using "rb" mode --> open(filename, "rb").
     include_page_breaks
         If True, includes a PageBreak element between slides
     metadata_filename
         The filename to use for the metadata. Relevant because partition_ppt converts the
         document .pptx before partition. We want the original source filename in the
         metadata.
-    metadata_date
+    metadata_last_modified
         The last modified date for the document.
 
 
     include_slide_notes
         If True, includes the slide notes as element
     """
 
@@ -81,15 +81,15 @@
         )
 
     elements: List[Element] = []
     metadata = ElementMetadata(filename=metadata_filename or filename)
     num_slides = len(presentation.slides)
     for i, slide in enumerate(presentation.slides):
         metadata = ElementMetadata.from_dict(metadata.to_dict())
-        metadata.date = metadata_date or last_modification_date
+        metadata.last_modified = metadata_last_modified or last_modification_date
         metadata.page_number = i + 1
         if include_slide_notes and slide.has_notes_slide is True:
             notes_slide = slide.notes_slide
             if notes_slide.notes_text_frame is not None:
                 notes_text_frame = notes_slide.notes_text_frame
                 notes_text = notes_text_frame.text
                 if notes_text.strip() != "":
@@ -101,15 +101,15 @@
                 html_table = convert_ms_office_table_to_text(table, as_html=True)
                 text_table = convert_ms_office_table_to_text(table, as_html=False)
                 if (text_table := text_table.strip()) != "":
                     metadata = ElementMetadata(
                         filename=metadata_filename or filename,
                         text_as_html=html_table,
                         page_number=metadata.page_number,
-                        date=metadata_date or last_modification_date,
+                        last_modified=metadata_last_modified or last_modification_date,
                     )
                     elements.append(Table(text=text_table, metadata=metadata))
                 continue
             if not shape.has_text_frame:
                 continue
             # NOTE(robinson) - avoid processing shapes that are not on the actual slide
             # NOTE - skip check if no top or left position (shape displayed top left)
```

### Comparing `unstructured-0.8.7/unstructured/partition/rst.py` & `unstructured-0.8.8/unstructured/partition/org.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 from typing import IO, List, Optional
 
-from unstructured.documents.elements import Element, process_metadata
+from unstructured.documents.elements import Element
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.partition.html import convert_and_partition_html
 
 
-@process_metadata()
-@add_metadata_with_filetype(FileType.RST)
-def partition_rst(
+@add_metadata_with_filetype(FileType.ORG)
+def partition_org(
     filename: Optional[str] = None,
     file: Optional[IO[bytes]] = None,
     include_page_breaks: bool = False,
     include_metadata: bool = True,
     metadata_filename: Optional[str] = None,
-    metadata_date: Optional[str] = None,
-    **kwargs,
+    metadata_last_modified: Optional[str] = None,
 ) -> List[Element]:
-    """Partitions an RST document. The document is first converted to HTML and then
+    """Partitions an org document. The document is first converted to HTML and then
     partitioned using partition_html.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
     include_page_breaks
-        If True, the output will include page breaks if the filetype supports it.
-    metadata_date
+        If True, the output will include page breaks if the filetype supports it
+    metadata_last_modified
         The last modified date for the document.
     """
     return convert_and_partition_html(
-        source_format="rst",
+        source_format="org",
         filename=filename,
         file=file,
         include_page_breaks=include_page_breaks,
         metadata_filename=metadata_filename,
-        metadata_date=metadata_date,
+        metadata_last_modified=metadata_last_modified,
     )
```

### Comparing `unstructured-0.8.7/unstructured/partition/rtf.py` & `unstructured-0.8.8/unstructured/partition/rtf.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,32 +9,32 @@
 @add_metadata_with_filetype(FileType.RTF)
 def partition_rtf(
     filename: Optional[str] = None,
     file: Optional[IO[bytes]] = None,
     include_page_breaks: bool = False,
     include_metadata: bool = True,
     metadata_filename: Optional[str] = None,
-    metadata_date: Optional[str] = None,
+    metadata_last_modified: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
     """Partitions an RTF document. The document is first converted to HTML and then
     partitioned using partiton_html.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
     include_page_breaks
         If True, the output will include page breaks if the filetype supports it
-    metadata_date
+    metadata_last_modified
         The last modified date for the document.
     """
     return convert_and_partition_html(
         source_format="rtf",
         filename=filename,
         file=file,
         include_page_breaks=include_page_breaks,
         metadata_filename=metadata_filename,
-        metadata_date=metadata_date,
+        metadata_last_modified=metadata_last_modified,
     )
```

### Comparing `unstructured-0.8.7/unstructured/partition/strategies.py` & `unstructured-0.8.8/unstructured/partition/strategies.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/partition/text.py` & `unstructured-0.8.8/unstructured/partition/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,15 +184,15 @@
     text: Optional[str] = None,
     encoding: Optional[str] = None,
     paragraph_grouper: Optional[Callable[[str], str]] = None,
     metadata_filename: Optional[str] = None,
     include_metadata: bool = True,
     max_partition: Optional[int] = 1500,
     min_partition: Optional[int] = 0,
-    metadata_date: Optional[str] = None,
+    metadata_last_modified: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
     """Partitions an .txt documents into its constituent paragraph elements.
     If paragraphs are below "min_partition" or above "max_partition" boundaries,
     they are combined or split.
     Parameters
     ----------
@@ -210,15 +210,15 @@
     include_metadata
         Determines whether or not metadata is included in the output.
     max_partition
         The maximum number of characters to include in a partition. If None is passed,
         no maximum is applied.
     min_partition
         The minimum number of characters to include in a partition.
-    metadata_date
+    metadata_last_modified
         The day of the last modification
     """
     if text is not None and text.strip() == "" and not file and not filename:
         return []
 
     if (
         min_partition is not None
@@ -258,15 +258,15 @@
         max_partition=max_partition,
     )
 
     elements: List[Element] = []
     metadata = (
         ElementMetadata(
             filename=metadata_filename or filename,
-            date=metadata_date or last_modification_date,
+            last_modified=metadata_last_modified or last_modification_date,
         )
         if include_metadata
         else ElementMetadata()
     )
     for ctext in file_content:
         ctext = ctext.strip()
```

### Comparing `unstructured-0.8.7/unstructured/partition/text_type.py` & `unstructured-0.8.8/unstructured/partition/text_type.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/partition/tsv.py` & `unstructured-0.8.8/unstructured/partition/tsv.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,29 +21,29 @@
 
 @process_metadata()
 @add_metadata_with_filetype(FileType.TSV)
 def partition_tsv(
     filename: Optional[str] = None,
     file: Optional[Union[IO[bytes], SpooledTemporaryFile]] = None,
     metadata_filename: Optional[str] = None,
-    metadata_date: Optional[str] = None,
+    metadata_last_modified: Optional[str] = None,
     include_metadata: bool = True,
     **kwargs,
 ) -> List[Element]:
     """Partitions TSV files into document elements.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
     include_metadata
         Determines whether or not metadata is included in the output.
-    metadata_date
+    metadata_last_modified
         The day of the last modification
     """
     exactly_one(filename=filename, file=file)
     last_modification_date = None
     if filename:
         table = pd.read_csv(filename, sep="\t")
         last_modification_date = get_last_modified_date(filename)
@@ -57,13 +57,13 @@
     html_text = table.to_html(index=False, header=False, na_rep="")
     text = lxml.html.document_fromstring(html_text).text_content()
 
     if include_metadata:
         metadata = ElementMetadata(
             text_as_html=html_text,
             filename=metadata_filename or filename,
-            date=metadata_date or last_modification_date,
+            last_modified=metadata_last_modified or last_modification_date,
         )
     else:
         metadata = ElementMetadata()
 
     return [Table(text=text, metadata=metadata)]
```

### Comparing `unstructured-0.8.7/unstructured/partition/xlsx.py` & `unstructured-0.8.8/unstructured/partition/xlsx.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,28 +22,28 @@
 @process_metadata()
 @add_metadata_with_filetype(FileType.XLSX)
 def partition_xlsx(
     filename: Optional[str] = None,
     file: Optional[Union[IO[bytes], SpooledTemporaryFile]] = None,
     metadata_filename: Optional[str] = None,
     include_metadata: bool = True,
-    metadata_date: Optional[str] = None,
+    metadata_last_modified: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
     """Partitions Microsoft Excel Documents in .xlsx format into its document elements.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
     include_metadata
         Determines whether or not metadata is included in the output.
-    metadata_date
+    metadata_last_modified
         The day of the last modification
     """
     exactly_one(filename=filename, file=file)
     last_modification_date = None
     if filename:
         sheets = pd.read_excel(filename, sheet_name=None)
         last_modification_date = get_last_modified_date(filename)
@@ -64,15 +64,15 @@
 
         if include_metadata:
             metadata = ElementMetadata(
                 text_as_html=html_text,
                 page_name=sheet_name,
                 page_number=page_number,
                 filename=metadata_filename or filename,
-                date=metadata_date or last_modification_date,
+                last_modified=metadata_last_modified or last_modification_date,
             )
         else:
             metadata = ElementMetadata()
 
         table = Table(text=text, metadata=metadata)
         elements.append(table)
```

### Comparing `unstructured-0.8.7/unstructured/partition/xml.py` & `unstructured-0.8.8/unstructured/partition/xml.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     xml_keep_tags: bool = False,
     xml_path: str = ".",
     metadata_filename: Optional[str] = None,
     include_metadata: bool = True,
     encoding: Optional[str] = None,
     max_partition: Optional[int] = 1500,
     min_partition: Optional[int] = 0,
-    metadata_date: Optional[str] = None,
+    metadata_last_modified: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
     """Partitions an XML document into its document elements.
 
     Parameters
     ----------
     filename
@@ -82,15 +82,15 @@
         Determines whether or not metadata is included in the metadata attribute on the
         elements in the output.
     max_partition
         The maximum number of characters to include in a partition. If None is passed,
         no maximum is applied.
     min_partition
         The minimum number of characters to include in a partition.
-    metadata_date
+    metadata_last_modified
         The day of the last modification
     """
     exactly_one(filename=filename, file=file)
 
     if xml_keep_tags:
         if filename:
             _, raw_text = read_txt_file(filename=filename, encoding=encoding)
@@ -112,11 +112,11 @@
 
     elements = partition_text(
         text=raw_text,
         metadata_filename=metadata_filename,
         include_metadata=include_metadata,
         max_partition=max_partition,
         min_partition=min_partition,
-        metadata_date=metadata_date or last_modification_date,
+        metadata_last_modified=metadata_last_modified or last_modification_date,
     )
 
     return elements
```

### Comparing `unstructured-0.8.7/unstructured/staging/argilla.py` & `unstructured-0.8.8/unstructured/staging/argilla.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/staging/base.py` & `unstructured-0.8.8/unstructured/staging/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/staging/baseplate.py` & `unstructured-0.8.8/unstructured/staging/baseplate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/staging/datasaur.py` & `unstructured-0.8.8/unstructured/staging/datasaur.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/staging/huggingface.py` & `unstructured-0.8.8/unstructured/staging/huggingface.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/staging/label_box.py` & `unstructured-0.8.8/unstructured/staging/label_box.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/staging/label_studio.py` & `unstructured-0.8.8/unstructured/staging/label_studio.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/staging/prodigy.py` & `unstructured-0.8.8/unstructured/staging/prodigy.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/staging/weaviate.py` & `unstructured-0.8.8/unstructured/staging/weaviate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured/utils.py` & `unstructured-0.8.8/unstructured/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.7/unstructured.egg-info/PKG-INFO` & `unstructured-0.8.8/unstructured.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.8.7
+Version: 0.8.8
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -320,10 +320,11 @@
 Provides-Extra: reddit
 Provides-Extra: slack
 Provides-Extra: wikipedia
 Provides-Extra: google-drive
 Provides-Extra: gcs
 Provides-Extra: elasticsearch
 Provides-Extra: dropbox
+Provides-Extra: box
 Provides-Extra: onedrive
 Provides-Extra: outlook
 Provides-Extra: confluence
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.8.7 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.8.8 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
@@ -217,9 +217,9 @@
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Requires-Python: >=3.7.0 Description-Content-Type:
 text/markdown Provides-Extra: huggingface Provides-Extra: local-inference
 Provides-Extra: s3 Provides-Extra: azure Provides-Extra: discord Provides-
 Extra: github Provides-Extra: gitlab Provides-Extra: reddit Provides-Extra:
 slack Provides-Extra: wikipedia Provides-Extra: google-drive Provides-Extra:
-gcs Provides-Extra: elasticsearch Provides-Extra: dropbox Provides-Extra:
-onedrive Provides-Extra: outlook Provides-Extra: confluence
+gcs Provides-Extra: elasticsearch Provides-Extra: dropbox Provides-Extra: box
+Provides-Extra: onedrive Provides-Extra: outlook Provides-Extra: confluence
```

### Comparing `unstructured-0.8.7/unstructured.egg-info/requires.txt` & `unstructured-0.8.8/unstructured.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 tabulate
 xlrd
 
 [azure]
 adlfs
 fsspec
 
+[box]
+boxfs
+fsspec
+
 [confluence]
 atlassian-python-api
 
 [discord]
 discord-py
 
 [dropbox]
```

