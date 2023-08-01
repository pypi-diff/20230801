# Comparing `tmp/sign-language-datasets-0.1.7.tar.gz` & `tmp/sign-language-datasets-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sign-language-datasets-0.1.7.tar", last modified: Thu Mar 30 09:38:39 2023, max compression
+gzip compressed data, was "sign-language-datasets-0.1.8.tar", last modified: Tue Aug  1 16:11:14 2023, max compression
```

## Comparing `sign-language-datasets-0.1.7.tar` & `sign-language-datasets-0.1.8.tar`

### file list

```diff
@@ -1,183 +1,188 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.048385 sign-language-datasets-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-03-30 09:38:39.048385 sign-language-datasets-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.004382 sign-language-datasets-0.1.7/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.008383 sign-language-datasets-0.1.7/examples/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/examples/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/examples/datasets/dgs_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/examples/datasets/sign2mint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/examples/datasets/signsuisse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/examples/load_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/examples/run-holistic.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 09:38:39.048385 sign-language-datasets-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.008383 sign-language-datasets-0.1.7/sign_language_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.008383 sign-language-datasets-0.1.7/sign_language_datasets/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.012383 sign-language-datasets-0.1.7/sign_language_datasets/datasets/asl_lex/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/asl_lex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/asl_lex/asl_lex.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/asl_lex/asl_lex_test.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/asl_lex/checksums.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    45325 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/asl_lex/data-key.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.012383 sign-language-datasets-0.1.7/sign_language_datasets/datasets/aslg_pc12/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/aslg_pc12/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/aslg_pc12/aslg_pc12.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/aslg_pc12/aslg_pc12_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/aslg_pc12/checksums.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.012383 sign-language-datasets-0.1.7/sign_language_datasets/datasets/autsl/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/autsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/autsl/autsl.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/autsl/autsl_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/autsl/checksums.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.012383 sign-language-datasets-0.1.7/sign_language_datasets/datasets/autsl/dummy_data/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/autsl/dummy_data/labels.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/autsl/holistic.poseheader
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/autsl/openpose_135.poseheader
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.012383 sign-language-datasets-0.1.7/sign_language_datasets/datasets/bsl_corpus/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/bsl_corpus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/bsl_corpus/bsl_corpus.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/bsl_corpus/bsl_corpus_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16808 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/bsl_corpus/bsl_corpus_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/bsl_corpus/checksums.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.016383 sign-language-datasets-0.1.7/sign_language_datasets/datasets/chicagofswild/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/chicagofswild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/chicagofswild/checksums.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/chicagofswild/chicagofswild.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/chicagofswild/chicagofswild_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.016383 sign-language-datasets-0.1.7/sign_language_datasets/datasets/dgs_corpus/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/dgs_corpus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/dgs_corpus/checksums.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/dgs_corpus/create_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/dgs_corpus/dgs_corpus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/dgs_corpus/dgs_corpus_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/dgs_corpus/dgs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/dgs_corpus/holistic.poseheader
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/dgs_corpus/openpose.poseheader
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.016383 sign-language-datasets-0.1.7/sign_language_datasets/datasets/dgs_corpus/splits/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/dgs_corpus/splits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/dgs_corpus/splits/create_document_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     8673 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/dgs_corpus/splits/split.3.0.0-uzh-document.json
--rw-r--r--   0 runner    (1001) docker     (123)  1561636 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/dgs_corpus/splits/split.3.0.0-uzh-sentence.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.020383 sign-language-datasets-0.1.7/sign_language_datasets/datasets/dgs_types/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/dgs_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/dgs_types/checksums.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/dgs_types/dgs_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/dgs_types/dgs_types_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14805 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/dgs_types/holistic.poseheader
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/dgs_types/make_poses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.020383 sign-language-datasets-0.1.7/sign_language_datasets/datasets/dicta_sign/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/dicta_sign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/dicta_sign/checksums.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/dicta_sign/dicta_sign.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/dicta_sign/dicta_sign_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/dicta_sign/holistic.header
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.024383 sign-language-datasets-0.1.7/sign_language_datasets/datasets/how2sign/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/how2sign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/how2sign/checksums.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/how2sign/how2sign.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/how2sign/how2sign_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/how2sign/openpose.header
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.024383 sign-language-datasets-0.1.7/sign_language_datasets/datasets/ngt_corpus/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/ngt_corpus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/ngt_corpus/create_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/ngt_corpus/ngt_corpus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/ngt_corpus/ngt_corpus_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/ngt_corpus/ngt_corpus_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.024383 sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/checksums.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.000382 sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.000382 sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.000382 sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.000382 sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.000382 sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/annotations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.024383 sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/annotations/manual/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/annotations/manual/PHOENIX-2014-T.dev.corpus.csv
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/annotations/manual/PHOENIX-2014-T.test.corpus.csv
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/annotations/manual/PHOENIX-2014-T.train.corpus.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.000382 sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.004382 sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.000382 sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/dev/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.028384 sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/dev/25October_2010_Monday_tagesschau-17/
--rw-r--r--   0 runner    (1001) docker     (123)    39272 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/dev/25October_2010_Monday_tagesschau-17/images0001.png
--rw-r--r--   0 runner    (1001) docker     (123)    40578 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/dev/25October_2010_Monday_tagesschau-17/images0002.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.004382 sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.028384 sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/test/25October_2010_Monday_tagesschau-17/
--rw-r--r--   0 runner    (1001) docker     (123)    39272 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/test/25October_2010_Monday_tagesschau-17/images0001.png
--rw-r--r--   0 runner    (1001) docker     (123)    40578 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/test/25October_2010_Monday_tagesschau-17/images0002.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.004382 sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/train/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.028384 sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/train/25October_2010_Monday_tagesschau-17/
--rw-r--r--   0 runner    (1001) docker     (123)    39272 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/train/25October_2010_Monday_tagesschau-17/images0001.png
--rw-r--r--   0 runner    (1001) docker     (123)    40578 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/train/25October_2010_Monday_tagesschau-17/images0002.png
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/pose.header
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/rwth_phoenix2014_t.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/rwth_phoenix2014_t_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.028384 sign-language-datasets-0.1.7/sign_language_datasets/datasets/sign2mint/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/sign2mint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   211538 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/sign2mint/checksums.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/sign2mint/sign2mint.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/sign2mint/sign2mint_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.028384 sign-language-datasets-0.1.7/sign_language_datasets/datasets/signbank/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/signbank/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11484 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/signbank/signbank.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/signbank/signbank_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.028384 sign-language-datasets-0.1.7/sign_language_datasets/datasets/signsuisse/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/signsuisse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/signsuisse/checksums.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/signsuisse/signsuisse.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/signsuisse/signsuisse_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.032384 sign-language-datasets-0.1.7/sign_language_datasets/datasets/signtyp/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/signtyp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/signtyp/checksums.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/signtyp/signtyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/signtyp/signtyp_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.032384 sign-language-datasets-0.1.7/sign_language_datasets/datasets/swojs_glossario/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/swojs_glossario/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49569 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/swojs_glossario/checksums.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/swojs_glossario/swojs_glossario.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/swojs_glossario/swojs_glossario_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/warning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.032384 sign-language-datasets-0.1.7/sign_language_datasets/datasets/wlasl/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/wlasl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/wlasl/checksums.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/wlasl/wlasl.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/wlasl/wlasl_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.036384 sign-language-datasets-0.1.7/sign_language_datasets/datasets/wmt_slt/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/wmt_slt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/wmt_slt/checksums.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/wmt_slt/holistic.poseheader
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/wmt_slt/openpose_135.poseheader
--rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/wmt_slt/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/wmt_slt/wmt_slt.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/datasets/wmt_slt/wmt_slt_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.036384 sign-language-datasets-0.1.7/sign_language_datasets/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.036384 sign-language-datasets-0.1.7/sign_language_datasets/utils/downloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/utils/downloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/utils/downloaders/aslpro.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/utils/downloaders/youtube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.036384 sign-language-datasets-0.1.7/sign_language_datasets/utils/features/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/utils/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/utils/features/pose_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/utils/get_pose_header.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.036384 sign-language-datasets-0.1.7/sign_language_datasets/utils/signwriting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/utils/signwriting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.036384 sign-language-datasets-0.1.7/sign_language_datasets/utils/signwriting/ocr/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/utils/signwriting/ocr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.048385 sign-language-datasets-0.1.7/sign_language_datasets/utils/signwriting/ocr/assets/
--rw-r--r--   0 runner    (1001) docker     (123)  8206192 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/utils/signwriting/ocr/assets/SuttonSignWritingOneD.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/utils/signwriting/ocr/assets/sign.png
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/utils/signwriting/ocr/ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/utils/signwriting/ocr/ocr_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-03-30 09:38:30.000000 sign-language-datasets-0.1.7/sign_language_datasets/utils/torch_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:38:39.008383 sign-language-datasets-0.1.7/sign_language_datasets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-03-30 09:38:38.000000 sign-language-datasets-0.1.7/sign_language_datasets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-03-30 09:38:38.000000 sign-language-datasets-0.1.7/sign_language_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 09:38:38.000000 sign-language-datasets-0.1.7/sign_language_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-30 09:38:38.000000 sign-language-datasets-0.1.7/sign_language_datasets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-30 09:38:38.000000 sign-language-datasets-0.1.7/sign_language_datasets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.828267 sign-language-datasets-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-08-01 16:11:14.828267 sign-language-datasets-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.800265 sign-language-datasets-0.1.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.800265 sign-language-datasets-0.1.8/examples/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/examples/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/examples/datasets/dgs_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/examples/datasets/sign2mint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/examples/load_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/examples/run-holistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 16:11:14.828267 sign-language-datasets-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.800265 sign-language-datasets-0.1.8/sign_language_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.800265 sign-language-datasets-0.1.8/sign_language_datasets/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.800265 sign-language-datasets-0.1.8/sign_language_datasets/datasets/asl_lex/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/asl_lex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/asl_lex/asl_lex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/asl_lex/asl_lex_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/asl_lex/checksums.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    45325 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/asl_lex/data-key.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.800265 sign-language-datasets-0.1.8/sign_language_datasets/datasets/aslg_pc12/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/aslg_pc12/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/aslg_pc12/aslg_pc12.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/aslg_pc12/aslg_pc12_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/aslg_pc12/checksums.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.800265 sign-language-datasets-0.1.8/sign_language_datasets/datasets/autsl/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/autsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/autsl/autsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/autsl/autsl_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/autsl/checksums.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.800265 sign-language-datasets-0.1.8/sign_language_datasets/datasets/autsl/dummy_data/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/autsl/dummy_data/labels.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/autsl/holistic.poseheader
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/autsl/openpose_135.poseheader
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.804265 sign-language-datasets-0.1.8/sign_language_datasets/datasets/bsl_corpus/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/bsl_corpus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/bsl_corpus/bsl_corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/bsl_corpus/bsl_corpus_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16808 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/bsl_corpus/bsl_corpus_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/bsl_corpus/checksums.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.804265 sign-language-datasets-0.1.8/sign_language_datasets/datasets/chicagofswild/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/chicagofswild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/chicagofswild/checksums.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/chicagofswild/chicagofswild.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/chicagofswild/chicagofswild_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.804265 sign-language-datasets-0.1.8/sign_language_datasets/datasets/dgs_corpus/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/dgs_corpus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/dgs_corpus/checksums.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/dgs_corpus/create_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18919 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/dgs_corpus/dgs_corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/dgs_corpus/dgs_corpus_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/dgs_corpus/dgs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68590 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/dgs_corpus/file_sizes.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/dgs_corpus/holistic.poseheader
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/dgs_corpus/openpose.poseheader
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.804265 sign-language-datasets-0.1.8/sign_language_datasets/datasets/dgs_corpus/splits/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/dgs_corpus/splits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/dgs_corpus/splits/create_document_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8673 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/dgs_corpus/splits/split.3.0.0-uzh-document.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1561636 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/dgs_corpus/splits/split.3.0.0-uzh-sentence.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.808266 sign-language-datasets-0.1.8/sign_language_datasets/datasets/dgs_types/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/dgs_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/dgs_types/checksums.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/dgs_types/dgs_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/dgs_types/dgs_types_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14805 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/dgs_types/holistic.poseheader
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/dgs_types/make_poses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.808266 sign-language-datasets-0.1.8/sign_language_datasets/datasets/dicta_sign/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/dicta_sign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/dicta_sign/checksums.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/dicta_sign/dicta_sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/dicta_sign/dicta_sign_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/dicta_sign/holistic.header
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.808266 sign-language-datasets-0.1.8/sign_language_datasets/datasets/how2sign/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/how2sign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/how2sign/checksums.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/how2sign/how2sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/how2sign/how2sign_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/how2sign/openpose.header
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.808266 sign-language-datasets-0.1.8/sign_language_datasets/datasets/ngt_corpus/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/ngt_corpus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/ngt_corpus/create_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/ngt_corpus/ngt_corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/ngt_corpus/ngt_corpus_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/ngt_corpus/ngt_corpus_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.808266 sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/checksums.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.796265 sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.796265 sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.796265 sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.796265 sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.796265 sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/annotations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.808266 sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/annotations/manual/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/annotations/manual/PHOENIX-2014-T.dev.corpus.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/annotations/manual/PHOENIX-2014-T.test.corpus.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/annotations/manual/PHOENIX-2014-T.train.corpus.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.796265 sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.796265 sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.796265 sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/dev/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.808266 sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/dev/25October_2010_Monday_tagesschau-17/
+-rw-r--r--   0 runner    (1001) docker     (123)    39272 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/dev/25October_2010_Monday_tagesschau-17/images0001.png
+-rw-r--r--   0 runner    (1001) docker     (123)    40578 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/dev/25October_2010_Monday_tagesschau-17/images0002.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.796265 sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.812266 sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/test/25October_2010_Monday_tagesschau-17/
+-rw-r--r--   0 runner    (1001) docker     (123)    39272 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/test/25October_2010_Monday_tagesschau-17/images0001.png
+-rw-r--r--   0 runner    (1001) docker     (123)    40578 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/test/25October_2010_Monday_tagesschau-17/images0002.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.796265 sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/train/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.812266 sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/train/25October_2010_Monday_tagesschau-17/
+-rw-r--r--   0 runner    (1001) docker     (123)    39272 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/train/25October_2010_Monday_tagesschau-17/images0001.png
+-rw-r--r--   0 runner    (1001) docker     (123)    40578 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/train/25October_2010_Monday_tagesschau-17/images0002.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/pose.header
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/rwth_phoenix2014_t.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/rwth_phoenix2014_t_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.812266 sign-language-datasets-0.1.8/sign_language_datasets/datasets/sign2mint/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/sign2mint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   211538 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/sign2mint/checksums.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/sign2mint/sign2mint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/sign2mint/sign2mint_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.812266 sign-language-datasets-0.1.8/sign_language_datasets/datasets/signbank/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/signbank/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/signbank/signbank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/signbank/signbank_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.812266 sign-language-datasets-0.1.8/sign_language_datasets/datasets/signsuisse/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/signsuisse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/signsuisse/checksums.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/signsuisse/download_holistic_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.812266 sign-language-datasets-0.1.8/sign_language_datasets/datasets/signsuisse/dummy_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/signsuisse/dummy_data/de.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/signsuisse/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14203 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/signsuisse/holistic.poseheader
+-rw-r--r--   0 runner    (1001) docker     (123)    10205 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/signsuisse/signsuisse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/signsuisse/signsuisse_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.812266 sign-language-datasets-0.1.8/sign_language_datasets/datasets/signtyp/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/signtyp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/signtyp/checksums.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/signtyp/signtyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/signtyp/signtyp_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.812266 sign-language-datasets-0.1.8/sign_language_datasets/datasets/swojs_glossario/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/swojs_glossario/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49569 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/swojs_glossario/checksums.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/swojs_glossario/swojs_glossario.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/swojs_glossario/swojs_glossario_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/warning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.816266 sign-language-datasets-0.1.8/sign_language_datasets/datasets/wlasl/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/wlasl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/wlasl/checksums.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/wlasl/wlasl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/wlasl/wlasl_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.816266 sign-language-datasets-0.1.8/sign_language_datasets/datasets/wmt_slt/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/wmt_slt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/wmt_slt/checksums.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/wmt_slt/holistic.poseheader
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/wmt_slt/openpose_135.poseheader
+-rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/wmt_slt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/wmt_slt/wmt_slt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/datasets/wmt_slt/wmt_slt_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.816266 sign-language-datasets-0.1.8/sign_language_datasets/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.816266 sign-language-datasets-0.1.8/sign_language_datasets/utils/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/utils/downloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/utils/downloaders/aslpro.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/utils/downloaders/youtube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.816266 sign-language-datasets-0.1.8/sign_language_datasets/utils/features/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/utils/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7274 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/utils/features/pose_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/utils/get_pose_header.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.816266 sign-language-datasets-0.1.8/sign_language_datasets/utils/signwriting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/utils/signwriting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.816266 sign-language-datasets-0.1.8/sign_language_datasets/utils/signwriting/ocr/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/utils/signwriting/ocr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.828267 sign-language-datasets-0.1.8/sign_language_datasets/utils/signwriting/ocr/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)  8206192 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/utils/signwriting/ocr/assets/SuttonSignWritingOneD.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/utils/signwriting/ocr/assets/sign.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/utils/signwriting/ocr/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/utils/signwriting/ocr/ocr_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-08-01 16:11:07.000000 sign-language-datasets-0.1.8/sign_language_datasets/utils/torch_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:11:14.800265 sign-language-datasets-0.1.8/sign_language_datasets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-08-01 16:11:13.000000 sign-language-datasets-0.1.8/sign_language_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-08-01 16:11:13.000000 sign-language-datasets-0.1.8/sign_language_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 16:11:13.000000 sign-language-datasets-0.1.8/sign_language_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-01 16:11:13.000000 sign-language-datasets-0.1.8/sign_language_datasets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-01 16:11:13.000000 sign-language-datasets-0.1.8/sign_language_datasets.egg-info/top_level.txt
```

### Comparing `sign-language-datasets-0.1.7/PKG-INFO` & `sign-language-datasets-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sign-language-datasets
-Version: 0.1.7
+Version: 0.1.8
 Summary: TFDS Datasets for sign language
 Home-page: https://github.com/sign-language-processing/datasets
 Author: Amit Moryossef
 Author-email: amitmoryossef@gmail.com
 License: UNKNOWN
 Description: # Sign Language Datasets
```

### Comparing `sign-language-datasets-0.1.7/README.md` & `sign-language-datasets-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/examples/datasets/dgs_types.py` & `sign-language-datasets-0.1.8/examples/datasets/dgs_types.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/examples/datasets/sign2mint.py` & `sign-language-datasets-0.1.8/examples/datasets/sign2mint.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/examples/load_all.py` & `sign-language-datasets-0.1.8/examples/load_all.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/examples/run-holistic.py` & `sign-language-datasets-0.1.8/examples/run-holistic.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/setup.py` & `sign-language-datasets-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 packages = find_packages()
 print(packages)
 
 setup(
     name="sign-language-datasets",
     packages=packages,
-    version="0.1.7",
+    version="0.1.8",
     description="TFDS Datasets for sign language",
     author="Amit Moryossef",
     author_email="amitmoryossef@gmail.com",
     url="https://github.com/sign-language-processing/datasets",
     keywords=[],
     install_requires=["typing-extensions", "python-dotenv", "tqdm", "pose-format", "tfds-nightly", "tensorflow",
                       "numpy", "pympi-ling", "Pillow", "opencv-python==4.5.5.64"],
```

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/__init__.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/asl_lex/asl_lex.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/asl_lex/asl_lex.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/asl_lex/asl_lex_test.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/asl_lex/asl_lex_test.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/asl_lex/data-key.csv` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/asl_lex/data-key.csv`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/aslg_pc12/aslg_pc12.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/aslg_pc12/aslg_pc12.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/autsl/autsl.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/autsl/autsl.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/autsl/autsl_test.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/autsl/autsl_test.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/autsl/checksums.tsv` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/autsl/checksums.tsv`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/autsl/holistic.poseheader` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/autsl/holistic.poseheader`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/autsl/openpose_135.poseheader` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/autsl/openpose_135.poseheader`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/bsl_corpus/bsl_corpus.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/bsl_corpus/bsl_corpus.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/bsl_corpus/bsl_corpus_test.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/bsl_corpus/bsl_corpus_test.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/bsl_corpus/bsl_corpus_utils.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/bsl_corpus/bsl_corpus_utils.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/chicagofswild/chicagofswild.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/chicagofswild/chicagofswild.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/chicagofswild/chicagofswild_test.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/chicagofswild/chicagofswild_test.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/config.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     def __init__(
         self,
         include_video: bool = True,
         process_video: bool = None,
         include_pose: Optional[str] = None,
         fps: Optional[float] = None,
         resolution: Optional[Tuple[int, int]] = None,
+        sample_size: Optional[int] = None,
         extra: dict = {},
         **kwargs,
     ):
         """Constructs a RWTHPhoenix2014TConfig.
         Args:
           include_video: bool, whether to include videos in the data.
           process_video: bool, whether to load the videos as tensors or paths
@@ -30,14 +31,15 @@
         super(SignDatasetConfig, self).__init__(**kwargs)
         self.include_video = include_video
         self.process_video = process_video if process_video is not None else include_video
         self.include_pose = include_pose.lower() if include_pose is not None else None
 
         self.fps = fps
         self.resolution = resolution
+        self.sample_size = sample_size
         self.extra = extra
 
     def ffmpeg_args(self):
         args: List[str] = []
 
         if self.fps is not None:
             args += ["-r", str(self.fps)]
```

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/dgs_corpus/create_index.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/dgs_corpus/create_index.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/dgs_corpus/dgs_corpus.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/dgs_corpus/dgs_corpus.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import json
 from copy import copy
 
 import cv2
 import math
 
 import numpy as np
+import os
 import tensorflow as tf
 import tensorflow_datasets as tfds
 
 from os import path
 from typing import Dict, Any, Set, Optional, List
 
 from pose_format.numpy import NumPyPoseBody
@@ -249,14 +250,35 @@
             description=_DESCRIPTION,
             features=tfds.features.FeaturesDict(features),
             homepage=_HOMEPAGE,
             supervised_keys=None,
             citation=_CITATION,
         )
 
+    def validate_downloaded_files(self, dl_manager: tfds.download.DownloadManager, url_local: Dict[str, str]):
+        # It seems like sometimes, holistic poses are not downloaded correctly.
+        with open(path.join(path.dirname(path.realpath(__file__)), "file_sizes.json"), "r") as f:
+            expected_sizes = json.load(f)
+
+        is_valid = True
+        for url, size in expected_sizes.items():
+            if url in url_local:
+                local_size = os.path.getsize(url_local[url])
+                if size != local_size:
+                    is_valid = False
+                    print(f"Downloaded file {url} has size {size} but expected {expected_sizes[url]}")
+                    # Delete file
+                    os.remove(url_local[url])
+                    os.remove(str(url_local[url]) + ".INFO")
+                    # Re-download file
+                    url_local[url] = dl_manager.download(url)
+
+        if not is_valid:
+            self.validate_downloaded_files(dl_manager, url_local)
+
     def _split_generators(self, dl_manager: tfds.download.DownloadManager):
         """Returns SplitGenerators."""
         dataset_warning(self)
 
         index_path = dl_manager.download(INDEX_URL)
 
         with open(index_path, "r", encoding="utf-8") as f:
@@ -284,16 +306,18 @@
             for datum in index_data.values():
                 del datum["holistic_a"]
                 del datum["holistic_b"]
 
         urls = {url: url for datum in index_data.values() for url in datum.values() if url is not None}
 
         local_paths = dl_manager.download(urls)
+        self.validate_downloaded_files(dl_manager, local_paths)
 
-        data = {_id: {k: local_paths[v] if v is not None else None for k, v in datum.items()} for _id, datum in index_data.items()}
+        data = {_id: {k: local_paths[v] if v is not None else None for k, v in datum.items()}
+                for _id, datum in index_data.items()}
 
         if self._builder_config.split is not None:
             split = load_split(self._builder_config.split)
 
             train_args = {"data": data, "split": split["train"]}
             dev_args = {"data": data, "split": split["dev"]}
             test_args = {"data": data, "split": split["test"]}
@@ -365,14 +389,21 @@
                     for person in ["a", "b"]:
                         if datum["holistic_" + person] is not None:
                             with open(datum["holistic_" + person], "rb") as f:
                                 poses[person] = Pose.read(f.read())
                         else:
                             poses[person] = None
 
+                    # Validate that the poses are synchronized
+                    poses_values = [p for p in poses.values() if p is not None]
+                    if len(poses_values) > 0:
+                        first_pose = poses_values[0]
+                        assert all(p.body.data.shape == first_pose.body.data.shape for p in poses_values), \
+                            f"Document {document_id}: The poses are not synchronized ({[p.body.data.shape for p in poses_values]})"
+
             if self._builder_config.data_type == "document":
                 if poses is not None:
                     features["poses"] = poses
                 if self._builder_config.process_video:
                     features["videos"] = {t: v if v != "" else default_video for t, v in features["paths"]["videos"].items()}
                 features["id"] = document_id
                 yield document_id, features
```

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/dgs_corpus/dgs_corpus_test.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/dgs_corpus/dgs_corpus_test.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/dgs_corpus/dgs_utils.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/dgs_corpus/dgs_utils.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/dgs_corpus/holistic.poseheader` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/dgs_corpus/holistic.poseheader`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/dgs_corpus/openpose.poseheader` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/dgs_corpus/openpose.poseheader`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/dgs_corpus/splits/create_document_split.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/dgs_corpus/splits/create_document_split.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/dgs_corpus/splits/split.3.0.0-uzh-document.json` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/dgs_corpus/splits/split.3.0.0-uzh-document.json`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/dgs_corpus/splits/split.3.0.0-uzh-sentence.json` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/dgs_corpus/splits/split.3.0.0-uzh-sentence.json`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/dgs_types/dgs_types.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/dgs_types/dgs_types.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/dgs_types/dgs_types_test.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/dgs_types/dgs_types_test.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/dgs_types/holistic.poseheader` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/dgs_types/holistic.poseheader`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/dgs_types/make_poses.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/dgs_types/make_poses.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/dicta_sign/dicta_sign.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/dicta_sign/dicta_sign.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/dicta_sign/dicta_sign_test.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/dicta_sign/dicta_sign_test.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/dicta_sign/holistic.header` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/dicta_sign/holistic.header`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/how2sign/checksums.tsv` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/how2sign/checksums.tsv`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/how2sign/how2sign.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/how2sign/how2sign.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/how2sign/how2sign_test.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/how2sign/how2sign_test.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/how2sign/openpose.header` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/how2sign/openpose.header`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/ngt_corpus/create_index.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/ngt_corpus/create_index.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/ngt_corpus/ngt_corpus.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/ngt_corpus/ngt_corpus.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/ngt_corpus/ngt_corpus_test.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/ngt_corpus/ngt_corpus_test.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/ngt_corpus/ngt_corpus_utils.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/ngt_corpus/ngt_corpus_utils.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/checksums.tsv` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/checksums.tsv`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/dev/25October_2010_Monday_tagesschau-17/images0001.png` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/dev/25October_2010_Monday_tagesschau-17/images0001.png`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/dev/25October_2010_Monday_tagesschau-17/images0002.png` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/dev/25October_2010_Monday_tagesschau-17/images0002.png`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/test/25October_2010_Monday_tagesschau-17/images0001.png` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/test/25October_2010_Monday_tagesschau-17/images0001.png`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/test/25October_2010_Monday_tagesschau-17/images0002.png` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/test/25October_2010_Monday_tagesschau-17/images0002.png`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/train/25October_2010_Monday_tagesschau-17/images0001.png` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/train/25October_2010_Monday_tagesschau-17/images0001.png`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/train/25October_2010_Monday_tagesschau-17/images0002.png` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/dummy_data/annotations/PHOENIX-2014-T-release-v3/PHOENIX-2014-T/features/fullFrame-210x260px/train/25October_2010_Monday_tagesschau-17/images0002.png`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/pose.header` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/pose.header`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/rwth_phoenix2014_t.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/rwth_phoenix2014_t.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/rwth_phoenix2014_t/rwth_phoenix2014_t_test.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/rwth_phoenix2014_t/rwth_phoenix2014_t_test.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/sign2mint/checksums.tsv` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/sign2mint/checksums.tsv`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/sign2mint/sign2mint.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/sign2mint/sign2mint.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/sign2mint/sign2mint_test.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/sign2mint/sign2mint_test.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/signbank/signbank.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/signbank/signbank.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,28 +225,28 @@
             "train": self._generate_examples(spmls),
         }
 
     def _generate_examples(self, spmls: List[str]):
         """Yields examples."""
 
         i = 0
-        for spml in tqdm(spmls):
+        for spml in tqdm(reversed(spmls)):
             tree = ET.parse(spml)
             root = tree.getroot()
 
             puddle = int(root.attrib["puddle"])
 
             children = root.iter()
             for child in children:
                 if child.tag == "entry":
                     _id = child.attrib["id"]
                     mdt = int(child.attrib["mdt"]) if "mdt" in child.attrib and child.attrib["mdt"] != "" else 0
                     cdt = int(child.attrib["cdt"]) if "cdt" in child.attrib and child.attrib["cdt"] != "" else mdt
                     usr = child.attrib["usr"] if "usr" in child.attrib else ""
-                    texts = [c.text for c in child.iter() if c.tag != "src" and c.text is not None]
+                    texts = [c.text for c in child.iter() if c.tag != "src" and c.text is not None and c.text.strip() != ""]
 
                     signwriting_texts = []
                     spoken_texts = []
                     for text in texts:
                         if is_signwriting(text):
                             signwriting_texts.append(text)
                         else:
```

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/signbank/signbank_test.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/signbank/signbank_test.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/signsuisse/signsuisse.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/signtyp/signtyp.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,167 +1,119 @@
-"""A Swiss Sign Language Lexicon, combines all three Swiss sign languages: the German-Swiss Sign Language (DSGS), the Langue des Signes Française (LSF) and the Lingua Italiana dei Segni (LIS). ."""
-import json
+"""SignTyp dataset."""
 import re
-import string
+from datetime import datetime
 
+import requests
+import tensorflow as tf
 import tensorflow_datasets as tfds
-from tqdm import tqdm
 
 from ..warning import dataset_warning
 from ...datasets import SignDatasetConfig
 
 _DESCRIPTION = """
-Ein umfangreiches interaktives Lexikon der drei Gebärdensprachen der Schweiz (Deutschschweizerische Gebärdensprache DSGS, Langue des Signes Française LSF und Lingua Italiana dei Segni LIS). Herausgegeben vom Schweizerischen Gehörlosenbund (SGB-FSS)."""
+SignTyp is a work in progress. We currently have over 20,000 videos for signers from Brazil, China, Croatia, Denmark, Egypt, Estonia, Ethiopia, France, Germany, Haiti, Honduras, Iraq, Italy,Lithuania, Nepal, Nicaragua, the Philippines, Portugal, Russia, Rwanda, Sri Lanka, Turkey, Uganda, the United States and Venezuela. We have complete sets of approximately 1000 video recordings each for China, Denmark, Egypt, Ethiopia, Haiti, Honduras, Iraq, Lithuania, Portugal,the Phillipines, Russia (2 signers), Turkey, and the United States. Clipping has been completed for all sets except a second Russian signer.
 
-# TODO(signsuisse): BibTeX citation
-_CITATION = """
+We currently have SignWriting transcriptions for approximately 9,000 signs, with more in progress. Each transcription includes detailed information on handshapes, orientation, actions, locations, as well as special sequencing and articulator relationship information. There is a downloadable file for all transcribed information for sign language researchers.
+
+SignWriting transcription can be seen in our SignPuddles - see link below.
+
+The project is sponsored by NSF (National Science Foundation) and is made possible by grant BCS-1049510 to the University of Connecticut and Harry van der Hulst.
 """
 
-SITE_URL = "https://signsuisse.sgb-fss.ch"
+# TODO(SignTyp): BibTeX citation
+_CITATION = """
+"""
 
 
-class SignSuisse(tfds.core.GeneratorBasedBuilder):
-    """DatasetBuilder for signsuisse dataset."""
+class SignTyp(tfds.core.GeneratorBasedBuilder):
+    """DatasetBuilder for SignTyp dataset."""
 
-    MAX_SIMULTANEOUS_DOWNLOADS = 100  # Default is 50, but it is slow
     VERSION = tfds.core.Version("1.0.0")
     RELEASE_NOTES = {
-        "1.0.0": "Initial crawl.",
+        "1.0.0": "Initial release.",
     }
 
     BUILDER_CONFIGS = [
-        SignDatasetConfig(name="default", include_video=True),
-        SignDatasetConfig(name="annotations", include_video=False),
+        SignDatasetConfig(name="default", include_video=True, process_video=False, extra={"PHPSESSID": "hj9co07ct7f5noq529no9u09l4"})
     ]
 
     def _info(self) -> tfds.core.DatasetInfo:
-        """Return s the dataset metadata."""
+        """Returns the dataset metadata."""
 
         features = {
-            "id": tfds.features.Text(),
-            "name": tfds.features.Text(),
-            "category": tfds.features.Text(),
-            "spokenLanguage": tfds.features.Text(),
-            "signedLanguage": tfds.features.Text(),
-            "url": tfds.features.Text(),
-            "paraphrase": tfds.features.Text(),
-            "definition": tfds.features.Text(),
-            "exampleText": tfds.features.Text(),
-            "exampleVideo": tfds.features.Text(),
+            "id": tf.int32,
+            "created_date": tfds.features.Text(),
+            "modified_date": tfds.features.Text(),
+            "sign_writing": tfds.features.Text(),
+            "sign_language": tfds.features.Text(),
+            "video": tfds.features.Text(),
         }
 
-        if self._builder_config.include_video and self._builder_config.process_video:
-            features["video"] = self._builder_config.video_feature((640, 480))
-        else:
-            features["video"] = tfds.features.Text()
-
         return tfds.core.DatasetInfo(
             builder=self,
             description=_DESCRIPTION,
             features=tfds.features.FeaturesDict(features),
-            homepage=SITE_URL,
+            homepage="https://signtyp.uconn.edu/",
             supervised_keys=None,
             citation=_CITATION,
         )
 
-    def _list_all_lexicon_items(self, dl_manager: tfds.download.DownloadManager):
-        language = ['de', 'fr', 'it']
-        dl_links = [f"https://signsuisse.sgb-fss.ch/index.php?eID=sitemap&lang={l}&format=json" for l in language]
-
-        indexes = dl_manager.download(dl_links)
-        results = []
-        for index in indexes:
-            with open(index, "r", encoding="utf-8") as f:
-                index = json.load(f)
-            results.extend(index)
-
-        return results
-
-    def _parse_item(self, item, item_page):
-        item["name"] = item["name"].replace("   ", " ").replace("  ", " ")
-        with open(item_page, "r", encoding="utf-8") as f:
-            html = f.read()
-
-        # Verify that the page matches the item
-        title = re.search(r"<h1.*?>(.*?)</h1>", html).group(1).strip()
-        title = title.replace("&amp;", "&")
-        if title != item["name"]:
-            raise ValueError("Title does not match item name")
-
-        assert title == item["name"]
-
-        example = re.search(r"Beispiel</h2> <p>(.*?)</p>.*?<video.*?src=\"(.*?)\"", html)
-        if example is not None:
-            example_text = example.group(1).strip()
-            example_video = SITE_URL + example.group(2).strip()
-        else:
-            # This happens on: https://signsuisse.sgb-fss.ch/de/lexikon/g/shakespeare-william/
-            # Because the page is formatted differently. I requested a change to the page.
-            example_text = ""
-            example_video = ""
-
-        if item["uid"] in ["131220", "131073", "120731", "115584", "121152", "121125", "126042"]:
-            # This is a special case where the video is not available.
-            return None
-
-        video = SITE_URL + re.search(r"<video id=\"video-main\".*?src=\"(.*?)\"", html).group(1).strip()
-        paraphrase_match = re.search(r"Umschreibung</h2> <p>(.*?)</p>", html)
-        paraphrase = paraphrase_match.group(1).strip() if paraphrase_match else ""
-        definition_match = re.search(r"Definition</h2> <p>(.*?)</p>", html)
-        definition = definition_match.group(1).strip() if definition_match else ""
-        spoken_language = item["sprache"]
-        url_path = re.search(rf"<a href=\"(\/{spoken_language}\/.*?)\"", html).group(1).strip()
+    def _split_generators(self, dl_manager: tfds.download.DownloadManager):
+        """Returns SplitGenerators."""
+        dataset_warning(self)
+
+        if "PHPSESSID" not in self._builder_config.extra:
+            raise Exception(
+                "Missing PHPSESSID extra parameter. Go to https://signtyp.uconn.edu/signpuddle/ and copy your PHPSESSID from any network request."
+            )
+
+        cookies = {"PHPSESSID": self._builder_config.extra["PHPSESSID"]}
+
+        headers = {
+            "Connection": "keep-alive",
+            "Cache-Control": "max-age=0",
+            "sec-ch-ua": '" Not A;Brand";v="99", "Chromium";v="96", "Google Chrome";v="96"',
+            "sec-ch-ua-mobile": "?0",
+            "sec-ch-ua-platform": '"Windows"',
+            "Upgrade-Insecure-Requests": "1",
+            "Origin": "https://signtyp.uconn.edu",
+            "Content-Type": "application/x-www-form-urlencoded",
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/96.0.4664.45 Safari/537.36",
+            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9",
+            "Sec-Fetch-Site": "same-origin",
+            "Sec-Fetch-Mode": "navigate",
+            "Sec-Fetch-User": "?1",
+            "Sec-Fetch-Dest": "document",
+            "Referer": "https://signtyp.uconn.edu/signpuddle/export.php?ui=1&sgn=9032",
+            "Accept-Language": "en-US,en;q=0.9,he;q=0.8",
+        }
+
+        data = {"ex_source": "All", "action": "Download"}
+
+        res = requests.post("https://signtyp.uconn.edu/signpuddle/export.php", data=data, headers=headers, cookies=cookies)
+
+        spml = res.text
+
+        if not spml.startswith('<?xml version="1.0" encoding="UTF-8"?>'):
+            raise Exception("PHPSESSID might be expired.")
 
         return {
-            "id": item["uid"],
-            "name": item["name"],
-            "category": item["kategorie"],
-            "spokenLanguage": spoken_language,
-            "signedLanguage": "ch-" + spoken_language,
-            "url": SITE_URL + url_path,
-            "paraphrase": paraphrase,
-            "definition": definition,
-            "exampleText": example_text,
-            "exampleVideo": example_video,
-            "video": video
+            "train": self._generate_examples(spml),
         }
 
-    def _split_generators(self, dl_manager: tfds.download.DownloadManager):
-        dataset_warning(self)
-        print(
-            "The lexicon is available free of charge, so we look forward to your donation! https://www.sgb-fss.ch/spenden/jetzt-spenden/")
+    def _generate_examples(self, spml):
+        regex = '<entry id="(.*?)".*?cdt="(.*?)" mdt="(.*?)".*?term>(.*?)<.*?lxsg: (.*?)].*(http.*?)"'
+
+        for row in spml.splitlines():
+            datum = re.search(regex, row)
+
+            if datum is not None:
+                _id = datum.group(1)
 
-        lexicon_items = self._list_all_lexicon_items(dl_manager)
-        print("Found", len(lexicon_items), "lexicon items.")
-        item_urls = [item["link"] for item in lexicon_items]
-        # Item URLS are actually too long. We need to shorten them.
-        item_urls = [url[:url.find("&tx_issignsuisselexikon_anzeige%5Baction")] for url in item_urls]
-        items_pages = dl_manager.download(item_urls)
-
-        data = []
-        for item, item_page in zip(lexicon_items, items_pages):
-            try:
-                item = self._parse_item(item, item_page)
-                if item is not None:
-                    data.append(item)
-            except Exception as e:
-                print("Failed to parse item")
-                print(item)
-                print(item_page)
-                print(e)
-                print("\n\n\n\n\n\n")
-                # raise e
-
-        # Download videos if requested
-        if self._builder_config.include_video:
-            video_urls = [item["video"] for item in data]
-            videos = dl_manager.download(video_urls)
-            for datum, video in zip(data, videos):
-                datum["video"] = video
-                if not self._builder_config.process_video:
-                    datum["video"] = str(datum["video"])
-
-        return {"train": self._generate_examples(data)}
-
-    def _generate_examples(self, data):
-        for datum in data:
-            yield datum["id"], datum
+                yield _id, {
+                    "id": int(_id),
+                    "created_date": str(datetime.fromtimestamp(int(datum.group(2)))),
+                    "modified_date": str(datetime.fromtimestamp(int(datum.group(3)))),
+                    "sign_writing": datum.group(4),
+                    "sign_language": datum.group(5),
+                    "video": datum.group(6),
+                }
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/signsuisse/signsuisse_test.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/signsuisse/signsuisse_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 class SignSuisseTest(tfds.testing.DatasetBuilderTestCase):
     """Tests for signsuisse dataset."""
 
     # TODO(signsuisse):
     DATASET_CLASS = signsuisse.SignSuisse
     SPLITS = {
-        "train": 3,  # Number of fake train example
-        "test": 1,  # Number of fake test example
+        "train": 1,  # Number of fake train example
     }
+    DL_EXTRACT_RESULT = ['de.json']
 
     # If you are calling `download/download_and_extract` with a dict, like:
     #   dl_manager.download({'some_key': 'http://a.org/out.txt', ...})
     # then the tests needs to provide the fake output paths relative to the
     # fake data directory
     # DL_EXTRACT_RESULT = {'some_key': 'output_file1.txt', ...}
```

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/signtyp/signtyp_test.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/signtyp/signtyp_test.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/swojs_glossario/checksums.tsv` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/swojs_glossario/checksums.tsv`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/swojs_glossario/swojs_glossario.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/swojs_glossario/swojs_glossario.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/swojs_glossario/swojs_glossario_test.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/swojs_glossario/swojs_glossario_test.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/wlasl/wlasl.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/wlasl/wlasl.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/wlasl/wlasl_test.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/wlasl/wlasl_test.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/wmt_slt/holistic.poseheader` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/wmt_slt/holistic.poseheader`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/wmt_slt/openpose_135.poseheader` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/wmt_slt/openpose_135.poseheader`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/wmt_slt/utils.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/wmt_slt/utils.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/wmt_slt/wmt_slt.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/wmt_slt/wmt_slt.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/datasets/wmt_slt/wmt_slt_test.py` & `sign-language-datasets-0.1.8/sign_language_datasets/datasets/wmt_slt/wmt_slt_test.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/utils/downloaders/aslpro.py` & `sign-language-datasets-0.1.8/sign_language_datasets/utils/downloaders/aslpro.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/utils/features/pose_feature.py` & `sign-language-datasets-0.1.8/sign_language_datasets/utils/features/pose_feature.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from typing import Optional
 
 import numpy as np
 import numpy.ma as ma
 import tensorflow as tf
-from pose_format import Pose, PoseHeader
+from pose_format import Pose, PoseHeader, PoseBody
 from pose_format.numpy.pose_body import NumPyPoseBody
 from pose_format.utils.reader import BufferReader
 from tensorflow_datasets.core.features import feature
 from tensorflow_datasets.core.features.feature import Documentation
 from tensorflow_datasets.core.utils import Json
 from etils import epath
 
@@ -67,15 +67,19 @@
       yield {
           "input": "path/to/img.jpg",
           "target": np.ones(shape=(64, 64, 1), dtype=np.uint8),
       }
       ```
     """
 
-    def __init__(self, *, shape=None, header_path: str = None, encoding_format: str = None, stride: int = 1,
+    def __init__(self, *, shape=None,
+                 header_path: str = None,
+                 encoding_format: str = None,
+                 stride: int = 1,
+                 include_path: bool = False,
                  dtype=tf.float32):
         """Construct the connector.
 
         Args:
           shape: tuple of ints or None, the shape of decoded image.
             For GIF images: (num_frames, height, width, channels=3). num_frames,
               height and width can be None.
@@ -92,14 +96,15 @@
         Raises:
           ValueError: If the shape is invalid
         """
         # Set and validate values
         self._shape = shape or (None, None, None, 3)
         self._dtype = dtype
         self._encoding_format = encoding_format or "pose"
+        self._include_path = include_path
 
         self._doc = Documentation()
 
         assert int(stride) == stride, "Video fps must be divisible by custom fps, when loading poses"
         self.stride = int(stride)
 
         if header_path is not None:
@@ -108,62 +113,71 @@
             self._header, self._read_offset = None, None
 
         self._runner = None
 
     def get_tensor_info(self):
         # Image is returned as a 3-d uint8 tf.Tensor.
         conf_shape = tuple(list(self._shape)[:3])
-        return {
+        features = {
             "data": feature.TensorInfo(shape=self._shape, dtype=self._dtype),
             "conf": feature.TensorInfo(shape=conf_shape, dtype=self._dtype),
             "fps": feature.TensorInfo(shape=(), dtype=tf.int32),
         }
 
+        if self._include_path:
+            features["path"] = feature.TensorInfo(shape=(), dtype=tf.string)
+
+        return features
+
     def __getstate__(self):
         state = self.__dict__.copy()
         state["_runner"] = None
         return state
 
-    def encode_body(self, body: NumPyPoseBody):
-        # print("shape", body.data.shape, np.isfinite(body.data).all())
-
+    def encode_body(self, file_path: str, body: PoseBody):
         if self.stride != 1:
             body = body.slice_step(self.stride)
 
         data = body.data.data
         confidence = body.confidence
 
-        return {"data": data, "conf": confidence, "fps": int(body.fps)}
+        encoded = {"data": data, "conf": confidence, "fps": int(body.fps)}
+        if self._include_path:
+            encoded["path"] = file_path
+        return encoded
 
     def encode_example(self, pose_path_or_fobj):
         """Convert the given image into a dict convertible to tf example."""
 
         if pose_path_or_fobj is None:
             # Create 0 size tensors
             data_shape = list(self._shape)
             data_shape[0] = 0
             conf_shape = tuple(data_shape[:3])
             data_shape = tuple(data_shape)
 
             pose_body = NumPyPoseBody(data=ma.zeros(data_shape), confidence=np.zeros(conf_shape), fps=0)
-            return self.encode_body(pose_body)
+            return self.encode_body("empty", pose_body)
         elif isinstance(pose_path_or_fobj, Pose):
-            return self.encode_body(pose_path_or_fobj.body)
+            return self.encode_body("Pose", pose_path_or_fobj.body)
         elif isinstance(pose_path_or_fobj, epath.PathLikeCls):
             pose_path_or_fobj = os.fspath(pose_path_or_fobj)
             with tf.io.gfile.GFile(pose_path_or_fobj, "rb") as pose_f:
                 encoded_pose = pose_f.read()
+                pose_path = str(pose_path_or_fobj)
         elif isinstance(pose_path_or_fobj, bytes):
             encoded_pose = pose_path_or_fobj
+            pose_path = "bytes"
         else:
             encoded_pose = pose_path_or_fobj.read()
+            pose_path = "buffer"
 
         if self._encoding_format == "pose":
             pose_body = read_body(encoded_pose, self._header, self._read_offset)
-            return self.encode_body(pose_body)
+            return self.encode_body(pose_path, pose_body)
         else:
             raise Exception("Unknown encoding format '%s'" % self._encoding_format)
 
     # def decode_example(self, example):
     #     """Reconstruct the image from the tf example."""
     #     print("Decoding", example)
     #     print(example["data"].shape)
@@ -174,15 +188,18 @@
     #     img.set_shape(self._shape)
     #     return img
 
     @classmethod
     def from_json_content(cls, value: Json) -> "Pose":
         shape = tuple(value["shape"])
         encoding_format = value["encoding_format"]
-        return cls(shape=shape, encoding_format=encoding_format)
+        include_path = value["include_path"] if "include_path" in value else False
+        return cls(shape=shape, encoding_format=encoding_format, include_path=include_path)
 
     def to_json_content(self) -> Json:
-        print("to_json_content", {"shape": list(self._shape), "encoding_format": self._encoding_format, })
-        return {
+        content =  {
             "shape": list(self._shape),
             "encoding_format": self._encoding_format,
+            "include_path": self._include_path,
         }
+        print("to_json_content", content)
+        return content
```

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/utils/signwriting/ocr/assets/SuttonSignWritingOneD.ttf` & `sign-language-datasets-0.1.8/sign_language_datasets/utils/signwriting/ocr/assets/SuttonSignWritingOneD.ttf`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/utils/signwriting/ocr/assets/sign.png` & `sign-language-datasets-0.1.8/sign_language_datasets/utils/signwriting/ocr/assets/sign.png`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/utils/signwriting/ocr/ocr.py` & `sign-language-datasets-0.1.8/sign_language_datasets/utils/signwriting/ocr/ocr.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/utils/signwriting/ocr/ocr_test.py` & `sign-language-datasets-0.1.8/sign_language_datasets/utils/signwriting/ocr/ocr_test.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets/utils/torch_dataset.py` & `sign-language-datasets-0.1.8/sign_language_datasets/utils/torch_dataset.py`

 * *Files identical despite different names*

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets.egg-info/PKG-INFO` & `sign-language-datasets-0.1.8/sign_language_datasets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sign-language-datasets
-Version: 0.1.7
+Version: 0.1.8
 Summary: TFDS Datasets for sign language
 Home-page: https://github.com/sign-language-processing/datasets
 Author: Amit Moryossef
 Author-email: amitmoryossef@gmail.com
 License: UNKNOWN
 Description: # Sign Language Datasets
```

### Comparing `sign-language-datasets-0.1.7/sign_language_datasets.egg-info/SOURCES.txt` & `sign-language-datasets-0.1.8/sign_language_datasets.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 setup.py
 examples/__init__.py
 examples/load_all.py
 examples/run-holistic.py
 examples/datasets/__init__.py
 examples/datasets/dgs_types.py
 examples/datasets/sign2mint.py
-examples/datasets/signsuisse.py
 sign_language_datasets/__init__.py
 sign_language_datasets.egg-info/PKG-INFO
 sign_language_datasets.egg-info/SOURCES.txt
 sign_language_datasets.egg-info/dependency_links.txt
 sign_language_datasets.egg-info/requires.txt
 sign_language_datasets.egg-info/top_level.txt
 sign_language_datasets/datasets/__init__.py
@@ -44,14 +43,15 @@
 sign_language_datasets/datasets/chicagofswild/chicagofswild_test.py
 sign_language_datasets/datasets/dgs_corpus/__init__.py
 sign_language_datasets/datasets/dgs_corpus/checksums.tsv
 sign_language_datasets/datasets/dgs_corpus/create_index.py
 sign_language_datasets/datasets/dgs_corpus/dgs_corpus.py
 sign_language_datasets/datasets/dgs_corpus/dgs_corpus_test.py
 sign_language_datasets/datasets/dgs_corpus/dgs_utils.py
+sign_language_datasets/datasets/dgs_corpus/file_sizes.json
 sign_language_datasets/datasets/dgs_corpus/holistic.poseheader
 sign_language_datasets/datasets/dgs_corpus/openpose.poseheader
 sign_language_datasets/datasets/dgs_corpus/splits/__init__.py
 sign_language_datasets/datasets/dgs_corpus/splits/create_document_split.py
 sign_language_datasets/datasets/dgs_corpus/splits/split.3.0.0-uzh-document.json
 sign_language_datasets/datasets/dgs_corpus/splits/split.3.0.0-uzh-sentence.json
 sign_language_datasets/datasets/dgs_types/__init__.py
@@ -94,16 +94,20 @@
 sign_language_datasets/datasets/sign2mint/sign2mint.py
 sign_language_datasets/datasets/sign2mint/sign2mint_test.py
 sign_language_datasets/datasets/signbank/__init__.py
 sign_language_datasets/datasets/signbank/signbank.py
 sign_language_datasets/datasets/signbank/signbank_test.py
 sign_language_datasets/datasets/signsuisse/__init__.py
 sign_language_datasets/datasets/signsuisse/checksums.tsv
+sign_language_datasets/datasets/signsuisse/download_holistic_gcs.py
+sign_language_datasets/datasets/signsuisse/example.py
+sign_language_datasets/datasets/signsuisse/holistic.poseheader
 sign_language_datasets/datasets/signsuisse/signsuisse.py
 sign_language_datasets/datasets/signsuisse/signsuisse_test.py
+sign_language_datasets/datasets/signsuisse/dummy_data/de.json
 sign_language_datasets/datasets/signtyp/__init__.py
 sign_language_datasets/datasets/signtyp/checksums.tsv
 sign_language_datasets/datasets/signtyp/signtyp.py
 sign_language_datasets/datasets/signtyp/signtyp_test.py
 sign_language_datasets/datasets/swojs_glossario/__init__.py
 sign_language_datasets/datasets/swojs_glossario/checksums.tsv
 sign_language_datasets/datasets/swojs_glossario/swojs_glossario.py
```

