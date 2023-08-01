# Comparing `tmp/isovar-1.1.1.tar.gz` & `tmp/isovar-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/isovar-1.1.1.tar", last modified: Wed Aug 19 18:59:04 2020, max compression
+gzip compressed data, was "isovar-1.3.0.tar", last modified: Tue Aug  1 17:55:43 2023, max compression
```

## Comparing `isovar-1.1.1.tar` & `isovar-1.3.0.tar`

### file list

```diff
@@ -1,102 +1,103 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-19 18:59:04.000000 isovar-1.1.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)    21917 2020-08-19 18:59:04.000000 isovar-1.1.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    18032 2020-08-19 18:49:19.000000 isovar-1.1.1/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-19 18:59:04.000000 isovar-1.1.1/isovar/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3998 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/read_evidence.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1770 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/translation_key.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6449 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/filtering.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3318 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/alignment_score.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4388 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/translation_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5319 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/phasing.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37719 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/isovar_result.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5310 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/default_parameters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4090 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/allele_read.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11831 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/variant_orf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1889 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/protein_sequence_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      909 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/logging.conf
--rw-rw-r--   0 travis    (2000) travis    (2000)     5848 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/effect_prediction.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22490 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/read_collector.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3288 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/value_object.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5017 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/variant_orf_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3711 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/allele_read_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9572 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/reference_coding_sequence_key.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2461 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10005 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/variant_sequence.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1476 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/dna.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      827 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/logging.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5842 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/variant_sequence_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1823 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/string_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7369 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/dataframe_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7356 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/dataframe_builder.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8454 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/genetic_code.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5798 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/assembly.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-19 18:59:04.000000 isovar-1.1.1/isovar/cli/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2582 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/cli/variant_sequences_args.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1359 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/cli/isovar_allele_counts.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1272 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/cli/isovar_reference_contexts.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2322 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/cli/isovar_variant_sequences.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2959 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/cli/filter_args.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1220 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/cli/isovar_allele_reads.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2669 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/cli/isovar_translations.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4593 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/cli/rna_args.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1437 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/cli/isovar_protein_sequences.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2337 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/cli/reference_context_args.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1347 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/cli/isovar_variant_reads.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3454 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/cli/protein_sequence_args.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1723 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/cli/output_args.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1012 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/cli/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1480 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/cli/isovar_main.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1990 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/cli/main_args.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2912 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/cli/translation_args.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15146 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/protein_sequence.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3404 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/reference_context_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6696 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/variant_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6725 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/main.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7813 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/variant_sequence_creator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1454 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16686 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/protein_sequence_creator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4439 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/reference_sequence_key.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4067 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/reference_context.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5389 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/translation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6248 2020-08-19 18:49:19.000000 isovar-1.1.1/isovar/locus_read.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-08-19 18:59:04.000000 isovar-1.1.1/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-19 18:59:04.000000 isovar-1.1.1/isovar.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    21917 2020-08-19 18:59:04.000000 isovar-1.1.1/isovar.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-08-19 18:59:04.000000 isovar-1.1.1/isovar.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        7 2020-08-19 18:59:04.000000 isovar-1.1.1/isovar.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2704 2020-08-19 18:59:04.000000 isovar-1.1.1/isovar.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       87 2020-08-19 18:59:04.000000 isovar-1.1.1/isovar.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      490 2020-08-19 18:59:04.000000 isovar-1.1.1/isovar.egg-info/entry_points.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-19 18:59:04.000000 isovar-1.1.1/test/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1113 2020-08-19 18:49:19.000000 isovar-1.1.1/test/test_value_object.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2864 2020-08-19 18:49:19.000000 isovar-1.1.1/test/test_mutant_amino_acids_in_protein_sequence.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1658 2020-08-19 18:49:19.000000 isovar-1.1.1/test/testing_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1100 2020-08-19 18:49:19.000000 isovar-1.1.1/test/test_alignment_score.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1426 2020-08-19 18:49:19.000000 isovar-1.1.1/test/test_somatic_variant_with_0_supporting_rna_reads.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      773 2020-08-19 18:49:19.000000 isovar-1.1.1/test/test_translation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1802 2020-08-19 18:49:19.000000 isovar-1.1.1/test/test_somatic_variant_with_2_supporting_rna_reads.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3349 2020-08-19 18:49:19.000000 isovar-1.1.1/test/test_dataframe_builder.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1984 2020-08-19 18:49:19.000000 isovar-1.1.1/test/test_filtering.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12632 2020-08-19 18:49:19.000000 isovar-1.1.1/test/test_variant_orf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      554 2020-08-19 18:49:19.000000 isovar-1.1.1/test/test_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8361 2020-08-19 18:49:19.000000 isovar-1.1.1/test/test_reference_sequence_key.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8512 2020-08-19 18:49:19.000000 isovar-1.1.1/test/test_assembly.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4692 2020-08-19 18:49:19.000000 isovar-1.1.1/test/test_isovar_result.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      860 2020-08-19 18:49:19.000000 isovar-1.1.1/test/test_argparser_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6002 2020-08-19 18:49:19.000000 isovar-1.1.1/test/test_reference_contexts.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1851 2020-08-19 18:49:19.000000 isovar-1.1.1/test/test_cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1092 2020-08-19 18:49:19.000000 isovar-1.1.1/test/test_allele_reads.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7684 2020-08-19 18:49:19.000000 isovar-1.1.1/test/test_locus_reads.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1334 2020-08-19 18:49:19.000000 isovar-1.1.1/test/test_genetic_code.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11461 2020-08-19 18:49:19.000000 isovar-1.1.1/test/test_protein_sequences.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1188 2020-08-19 18:49:19.000000 isovar-1.1.1/test/test_read_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      533 2020-08-19 18:49:19.000000 isovar-1.1.1/test/test_main.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3113 2020-08-19 18:49:19.000000 isovar-1.1.1/test/test_variant_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13725 2020-08-19 18:49:19.000000 isovar-1.1.1/test/test_reference_coding_sequence_key.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1634 2020-08-19 18:49:19.000000 isovar-1.1.1/test/test_gather_variant_reads_wgs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1072 2020-08-19 18:49:19.000000 isovar-1.1.1/test/test_allele_counts.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      259 2020-08-19 18:49:19.000000 isovar-1.1.1/test/test_dna_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3398 2020-08-19 18:49:19.000000 isovar-1.1.1/test/test_variant_reads_with_dummy_samfile.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7734 2020-08-19 18:49:19.000000 isovar-1.1.1/test/test_variant_sequences.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      695 2020-08-19 18:49:19.000000 isovar-1.1.1/test/test_effect_prediction.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3085 2020-08-19 18:49:19.000000 isovar-1.1.1/setup.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-08-01 17:55:43.424268 isovar-1.3.0/
+-rw-r--r--   0 iskander   (501) staff       (20)    11357 2021-12-21 21:56:52.000000 isovar-1.3.0/LICENSE
+-rw-r--r--   0 iskander   (501) staff       (20)    18764 2023-08-01 17:55:43.424115 isovar-1.3.0/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)    18032 2021-12-21 21:56:52.000000 isovar-1.3.0/README.md
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-08-01 17:55:43.417176 isovar-1.3.0/isovar/
+-rw-r--r--   0 iskander   (501) staff       (20)     1454 2023-08-01 17:49:36.000000 isovar-1.3.0/isovar/__init__.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3318 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/alignment_score.py
+-rw-r--r--   0 iskander   (501) staff       (20)     4090 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/allele_read.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3711 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/allele_read_helpers.py
+-rw-r--r--   0 iskander   (501) staff       (20)     5798 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/assembly.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-08-01 17:55:43.419508 isovar-1.3.0/isovar/cli/
+-rw-r--r--   0 iskander   (501) staff       (20)     1012 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/cli/__init__.py
+-rw-r--r--   0 iskander   (501) staff       (20)     2959 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/cli/filter_args.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1359 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/cli/isovar_allele_counts.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1220 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/cli/isovar_allele_reads.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1480 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/cli/isovar_main.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1437 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/cli/isovar_protein_sequences.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1272 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/cli/isovar_reference_contexts.py
+-rw-r--r--   0 iskander   (501) staff       (20)     2669 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/cli/isovar_translations.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1347 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/cli/isovar_variant_reads.py
+-rw-r--r--   0 iskander   (501) staff       (20)     2322 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/cli/isovar_variant_sequences.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1990 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/cli/main_args.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1723 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/cli/output_args.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3454 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/cli/protein_sequence_args.py
+-rw-r--r--   0 iskander   (501) staff       (20)     2337 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/cli/reference_context_args.py
+-rw-r--r--   0 iskander   (501) staff       (20)     4593 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/cli/rna_args.py
+-rw-r--r--   0 iskander   (501) staff       (20)     2912 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/cli/translation_args.py
+-rw-r--r--   0 iskander   (501) staff       (20)     2582 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/cli/variant_sequences_args.py
+-rw-r--r--   0 iskander   (501) staff       (20)     2461 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/common.py
+-rw-r--r--   0 iskander   (501) staff       (20)     7356 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/dataframe_builder.py
+-rw-r--r--   0 iskander   (501) staff       (20)     7369 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/dataframe_helpers.py
+-rw-r--r--   0 iskander   (501) staff       (20)     5310 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/default_parameters.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1476 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/dna.py
+-rw-r--r--   0 iskander   (501) staff       (20)     5848 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/effect_prediction.py
+-rw-r--r--   0 iskander   (501) staff       (20)     6449 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/filtering.py
+-rw-r--r--   0 iskander   (501) staff       (20)     8454 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/genetic_code.py
+-rw-r--r--   0 iskander   (501) staff       (20)    37719 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/isovar_result.py
+-rw-r--r--   0 iskander   (501) staff       (20)     6248 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/locus_read.py
+-rw-r--r--   0 iskander   (501) staff       (20)      909 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/logging.conf
+-rw-r--r--   0 iskander   (501) staff       (20)      827 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/logging.py
+-rw-r--r--   0 iskander   (501) staff       (20)     6725 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/main.py
+-rw-r--r--   0 iskander   (501) staff       (20)     5319 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/phasing.py
+-rw-r--r--   0 iskander   (501) staff       (20)    15146 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/protein_sequence.py
+-rw-r--r--   0 iskander   (501) staff       (20)    16686 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/protein_sequence_creator.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1889 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/protein_sequence_helpers.py
+-rw-r--r--   0 iskander   (501) staff       (20)    22442 2023-08-01 17:47:28.000000 isovar-1.3.0/isovar/read_collector.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3998 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/read_evidence.py
+-rw-r--r--   0 iskander   (501) staff       (20)     9572 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/reference_coding_sequence_key.py
+-rw-r--r--   0 iskander   (501) staff       (20)     4067 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/reference_context.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3404 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/reference_context_helpers.py
+-rw-r--r--   0 iskander   (501) staff       (20)     4439 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/reference_sequence_key.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1823 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/string_helpers.py
+-rw-r--r--   0 iskander   (501) staff       (20)     5389 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/translation.py
+-rw-r--r--   0 iskander   (501) staff       (20)     4388 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/translation_helpers.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1770 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/translation_key.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3288 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/value_object.py
+-rw-r--r--   0 iskander   (501) staff       (20)     6696 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/variant_helpers.py
+-rw-r--r--   0 iskander   (501) staff       (20)    11831 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/variant_orf.py
+-rw-r--r--   0 iskander   (501) staff       (20)     5017 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/variant_orf_helpers.py
+-rw-r--r--   0 iskander   (501) staff       (20)    10005 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/variant_sequence.py
+-rw-r--r--   0 iskander   (501) staff       (20)     7813 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/variant_sequence_creator.py
+-rw-r--r--   0 iskander   (501) staff       (20)     5842 2021-12-21 21:56:52.000000 isovar-1.3.0/isovar/variant_sequence_helpers.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-08-01 17:55:43.417779 isovar-1.3.0/isovar.egg-info/
+-rw-r--r--   0 iskander   (501) staff       (20)    18764 2023-08-01 17:55:43.000000 isovar-1.3.0/isovar.egg-info/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)     2712 2023-08-01 17:55:43.000000 isovar-1.3.0/isovar.egg-info/SOURCES.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        1 2023-08-01 17:55:43.000000 isovar-1.3.0/isovar.egg-info/dependency_links.txt
+-rw-r--r--   0 iskander   (501) staff       (20)      489 2023-08-01 17:55:43.000000 isovar-1.3.0/isovar.egg-info/entry_points.txt
+-rw-r--r--   0 iskander   (501) staff       (20)       87 2023-08-01 17:55:43.000000 isovar-1.3.0/isovar.egg-info/requires.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        7 2023-08-01 17:55:43.000000 isovar-1.3.0/isovar.egg-info/top_level.txt
+-rw-r--r--   0 iskander   (501) staff       (20)       38 2023-08-01 17:55:43.424299 isovar-1.3.0/setup.cfg
+-rw-r--r--   0 iskander   (501) staff       (20)     3085 2021-12-21 21:56:52.000000 isovar-1.3.0/setup.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-08-01 17:55:43.423946 isovar-1.3.0/test/
+-rw-r--r--   0 iskander   (501) staff       (20)     1100 2021-12-21 21:56:53.000000 isovar-1.3.0/test/test_alignment_score.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1072 2021-12-21 21:56:53.000000 isovar-1.3.0/test/test_allele_counts.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3466 2023-08-01 17:30:24.000000 isovar-1.3.0/test/test_allele_reads.py
+-rw-r--r--   0 iskander   (501) staff       (20)      860 2021-12-21 21:56:53.000000 isovar-1.3.0/test/test_argparser_helpers.py
+-rw-r--r--   0 iskander   (501) staff       (20)     8512 2021-12-21 21:56:53.000000 isovar-1.3.0/test/test_assembly.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1851 2021-12-21 21:56:53.000000 isovar-1.3.0/test/test_cli.py
+-rw-r--r--   0 iskander   (501) staff       (20)      554 2021-12-21 21:56:53.000000 isovar-1.3.0/test/test_common.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3349 2021-12-21 21:56:53.000000 isovar-1.3.0/test/test_dataframe_builder.py
+-rw-r--r--   0 iskander   (501) staff       (20)      259 2021-12-21 21:56:53.000000 isovar-1.3.0/test/test_dna_helpers.py
+-rw-r--r--   0 iskander   (501) staff       (20)      695 2021-12-21 21:56:53.000000 isovar-1.3.0/test/test_effect_prediction.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1984 2021-12-21 21:56:53.000000 isovar-1.3.0/test/test_filtering.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1634 2021-12-21 21:56:53.000000 isovar-1.3.0/test/test_gather_variant_reads_wgs.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1334 2021-12-21 21:56:53.000000 isovar-1.3.0/test/test_genetic_code.py
+-rw-r--r--   0 iskander   (501) staff       (20)     4692 2021-12-21 21:56:53.000000 isovar-1.3.0/test/test_isovar_result.py
+-rw-r--r--   0 iskander   (501) staff       (20)     7684 2021-12-21 21:56:53.000000 isovar-1.3.0/test/test_locus_reads.py
+-rw-r--r--   0 iskander   (501) staff       (20)      533 2021-12-21 21:56:53.000000 isovar-1.3.0/test/test_main.py
+-rw-r--r--   0 iskander   (501) staff       (20)     2864 2021-12-21 21:56:53.000000 isovar-1.3.0/test/test_mutant_amino_acids_in_protein_sequence.py
+-rw-r--r--   0 iskander   (501) staff       (20)    11461 2021-12-21 21:56:53.000000 isovar-1.3.0/test/test_protein_sequences.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1188 2021-12-21 21:56:53.000000 isovar-1.3.0/test/test_read_helpers.py
+-rw-r--r--   0 iskander   (501) staff       (20)    13725 2021-12-21 21:56:53.000000 isovar-1.3.0/test/test_reference_coding_sequence_key.py
+-rw-r--r--   0 iskander   (501) staff       (20)     6002 2021-12-21 21:56:53.000000 isovar-1.3.0/test/test_reference_contexts.py
+-rw-r--r--   0 iskander   (501) staff       (20)     8361 2021-12-21 21:56:53.000000 isovar-1.3.0/test/test_reference_sequence_key.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1426 2021-12-21 21:56:53.000000 isovar-1.3.0/test/test_somatic_variant_with_0_supporting_rna_reads.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1802 2021-12-21 21:56:53.000000 isovar-1.3.0/test/test_somatic_variant_with_2_supporting_rna_reads.py
+-rw-r--r--   0 iskander   (501) staff       (20)      773 2021-12-21 21:56:53.000000 isovar-1.3.0/test/test_translation.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1113 2021-12-21 21:56:53.000000 isovar-1.3.0/test/test_value_object.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3113 2021-12-21 21:56:53.000000 isovar-1.3.0/test/test_variant_helpers.py
+-rw-r--r--   0 iskander   (501) staff       (20)    12632 2021-12-21 21:56:53.000000 isovar-1.3.0/test/test_variant_orf.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3398 2021-12-21 21:56:53.000000 isovar-1.3.0/test/test_variant_reads_with_dummy_samfile.py
+-rw-r--r--   0 iskander   (501) staff       (20)     7734 2021-12-21 21:56:53.000000 isovar-1.3.0/test/test_variant_sequences.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1658 2021-12-21 21:56:53.000000 isovar-1.3.0/test/testing_helpers.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `isovar-1.1.1/PKG-INFO` & `isovar-1.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,411 +1,411 @@
 Metadata-Version: 2.1
 Name: isovar
-Version: 1.1.1
+Version: 1.3.0
 Summary: Determine mutant protein sequences from RN using assembly around variants
 Home-page: https://github.com/openvax/isovar
 Author: Alex Rubinsteyn, Arman Aksoy, Julia Kodysh
 Author-email: alex.rubinsteyn@mssm.edu
 License: http://www.apache.org/licenses/LICENSE-2.0.html
-Description: <a href="https://travis-ci.org/openvax/isovar">
-            <img src="https://travis-ci.org/openvax/isovar.svg?branch=master" alt="Build Status" />
-        </a>
-        <a href="https://coveralls.io/github/openvax/isovar?branch=master">
-            <img src="https://coveralls.io/repos/openvax/isovar/badge.svg?branch=master&service=github" alt="Coverage Status" />
-        </a>
-        <a href="https://pypi.python.org/pypi/isovar/">
-            <img src="https://img.shields.io/pypi/v/isovar.svg?maxAge=1000" alt="PyPI" />
-        </a>
-        
-        # Isovar
-        
-        * [Overview](#overview)
-        * [Python API](#python-api)
-        * [Commandline](#commandline)
-        * [Internal Design](#internal-design)
-        * [Other Isovar Commandline Tools](#other-isovar-commandline-tools)
-        * [Sequencing Recommendations](#sequencing-recommendations)
-        
-        ## Overview
-        Isovar determines mutant protein subsequences around mutations from cancer RNAseq data.
-        
-        Isovar works by:
-        
-         1) collecting RNA reads which spanning the location of a variant,
-        
-         2) filtering the RNA reads to those which support the mutation,
-        
-         3) assembling mutant reads into longer coding sequences,  
-        
-         4) matching mutant coding sequences against reference annotated reading
-        frames, and
-        
-         5) translating coding sequences determined directly from RNA into mutant protein sequences.
-        
-        The assembled coding sequences may incorporate proximal 
-        (germline and somatic) variants, along with any splicing alterations 
-        which occur due to modified splice signals.
-        
-        ## Python API
-        
-        In the example below, `isovar.run_isovar` returns a list of `isovar.IsovarResult` objects. 
-        Each of these objects corresponds to a single input variant and contains all of the information about the RNA evidence at that variant's location and any mutant protein sequences which were assembled for the variant.
-        
-        ```python
-        
-        from isovar import run_isovar
-        
-        isovar_results = run_isovar(
-            variants="cancer-mutations.vcf",
-            alignment_file="tumor-rna.bam")
-            
-        # this code traverses every variant and prints the number
-        # of RNA reads which support the alt allele for variants
-        # which had a successfully assembled/translated protein sequence
-        for isovar_result in isovar_results:
-            # if any protein sequences were assembled from RNA
-            # then the one with most supporting reads can be
-            # accessed from a property called `top_protein_sequence`.
-            if isovar_result.top_protein_sequence is not None:
-                # print number of distinct fragments supporting the
-                # the variant allele for this mutation
-                print(isovar_result.variant, isovar_result.num_alt_fragments)
-            
-        ```
-        
-        A collection of `IsovarResult` objects can also be flattened into a Pandas DataFrame:
-        
-        ```python
-        
-        from isovar import run_isovar, isovar_results_to_dataframe
-        
-        df =  isovar_results_to_dataframe(
-                run_isovar(
-                    variants="cancer-mutations.vcf",
-                    alignment_file="tumor-rna.bam"))
-        ```
-        
-        
-        ### Python API options for collecting RNA reads
-        
-        To change how Isovar collects and filters RNA reads you can create
-        your own instance of the `isovar.ReadCollector` class and pass it to `run_isovar`.
-        ```python
-        from isovar import run_isovar, ReadCollector
-        
-        # create a custom ReadCollector to change options for how RNA reads are processed
-        read_collector = ReadCollector(
-            use_duplicate_reads=True,
-            use_secondary_alignments=True, 
-            use_soft_clipped_bases=True)
-        
-        isovar_results = run_isovar(
-            variants="cancer-mutations.vcf",
-            alignment_file="tumor-rna.bam",
-            read_collector=read_collector)
-        
-        ````
-        
-        
-        ### Python API options for coding sequence assembly and translation
-        
-        To change how Isovar assembles RNA reads into coding sequences, determines their
-        reading frames, and groups translated amino acid sequences you can create your
-        own instance of the `isovar.ProteinSequenceCreator` class and pass it to `run_isovar`.
-        
-        
-        ```python
-        from isovar import run_isovar, ProteinSequenceCreator
-        
-        # create a custom ProteinSequenceCreator to change options for how
-        # protein sequences are assembled from RNA reads
-        protein_sequence_creator = ProteinSequenceCreator(
-            # number of amino acids we're aiming for, coding sequences
-            # might still give us a shorter sequence due to an early stop 
-            # codon or poor coverage
-            protein_sequence_length=30,
-            # minimum number of reads covering each base of the coding sequence
-            min_variant_sequence_coverage=2,
-            # how much of a reference transcript should a coding sequence match before
-            # we use it to establish a reading frame
-            min_transcript_prefix_length=20,
-            # how many mismatches allowed between coding sequence (before the variant)
-            # and transcript (before the variant location)
-            max_transcript_mismatches=2,
-            # also count mismatches after the variant location toward
-            # max_transcript_mismatches
-            count_mismatches_after_variant=False,
-            # if more than one protein sequence can be assembled for a variant
-            # then drop any beyond this number 
-            max_protein_sequences_per_variant=1,
-            # if set to False then coding sequence will be derived from
-            # a single RNA read with the variant closest to its center
-            variant_sequence_assembly=True,
-            # how many nucleotides must two reads overlap before they are combined
-            # into a single coding sequence
-            min_assembly_overlap_size=30)
-        
-        isovar_results = run_isovar(
-            variants="cancer-mutations.vcf",
-            alignment_file="tumor-rna.bam",
-            protein_sequence_creator=protein_sequence_creator)
-        ```
-        
-        ### Python API for filtering results
-        
-        You can filter a collection of `IsovarResult` objects by any of their numerical properties using the `filter_thresholds` option
-        of the `run_isovar` function. The value expected for this argument is a dictionary whose keys have named like `'min_fraction_ref_reads'` or `'max_num_alt_fragments'`  and whose values are numerical thresholds.
-        Everything after the `'min_'` or `'max_'` at the start of a key is expected to be the name of a property of `IsovarResult`. 
-        Many of the commonly accessed properties regarding RNA read evidence follow the pattern: 
-        ```
-        {num|fraction}_{ref|alt|other}_{reads|fragments} 
-        ```
-        
-        For example, in the following code the results are filtered to have 10 or more alt reads supporting a variant and no more than 25% of the fragments supporting an allele other than the ref or alt.
-        ```python
-        from isovar import run_isovar
-        
-        isovar_results = run_isovar(
-            variants="cancer-mutations.vcf",
-            alignment_file="tumor-rna.bam",
-            filter_thresholds={"min_num_alt_reads": 10, "max_fraction_other_fragments": 0.25})    
-        
-        for isovar_result in isovar_results:
-            # print each variant and whether it passed both filters
-            print(isovar_result.variant, isovar_result.passes_all_filters)
-        ```
-        
-        A variant which fails one or more filters is not excluded from the result collection but it has `False` values in its corresponding 
-        `filter_values` dictionary property and will have a `False` value for the `passes_all_filters` property. 
-        
-        If a result collection is flattened into a DataFrame then each filter is included as a column. 
-        
-        It's also possible to filter on boolean properties (without numerical thresholds) by passing `filter_flags` to `run_isovar`. These boolean
-        properties can be further negated by prepending 'not_' to the property name, so that both `'protein_sequence_matches_predicted_effect'` and `'not_protein_sequence_matches_predicted_effect'` are valid names for `filter_flags`.
-        
-        ## Commandline 
-        
-        Basic example:
-        
-        ```sh
-        $ isovar  \
-            --vcf somatic-variants.vcf  \
-            --bam rnaseq.bam \
-            --protein-sequence-length 30 \
-            --output isovar-results.csv
-        ```
-        
-        ### Commandline options for loading variants
-        
-        ###
-        ```
-          --vcf VCF             Genomic variants in VCF format
-          
-          --maf MAF             Genomic variants in TCGA's MAF format
-          
-          --variant CHR POS REF ALT
-                                Individual variant as 4 arguments giving chromsome,
-                                position, ref, and alt. Example: chr1 3848 C G. Use
-                                '.' to indicate empty alleles for insertions or
-                                deletions.
-          
-          --genome GENOME       What reference assembly your variant coordinates are
-                                using. Examples: 'hg19', 'GRCh38', or 'mm9'. This
-                                argument is ignored for MAF files, since each row
-                                includes the reference. For VCF files, this is used if
-                                specified, and otherwise is guessed from the header.
-                                For variants specfied on the commandline with
-                                --variant, this option is required.
-          
-          --download-reference-genome-data
-                                Automatically download genome reference data required
-                                for annotation using PyEnsembl. Otherwise you must
-                                first run 'pyensembl install' for the release/species
-                                corresponding to the genome used in your VCF.
-          
-          --json-variants JSON_VARIANTS
-                                Path to Varcode.VariantCollection object serialized as
-                                a JSON file.
-        
-        ```
-        
-        ### Commandline options for loading aligned tumor RNA-seq reads
-        
-        ```
-          --bam BAM             BAM file containing RNAseq reads
-          
-          --min-mapping-quality MIN_MAPPING_QUALITY
-                                Minimum MAPQ value to allow for a read (default 1)
-          
-          --use-duplicate-reads
-                                By default, reads which have been marked as duplicates
-                                are excluded.Use this option to include duplicate
-                                reads.
-                                
-          --drop-secondary-alignments
-                                By default, secondary alignments are included in
-                                reads, use this option to instead only use primary
-                                alignments.
-        ```
-        
-        ### Commandline options for coding sequence assembly
-        ```
-          --min-variant-sequence-coverage MIN_VARIANT_SEQUENCE_COVERAGE
-                                Minimum number of reads supporting a variant sequence
-                                (default 2)
-                                
-          --disable-variant-sequence-assembly
-                                Disable assemble variant cDNA sequence from
-                                overlapping reads
-        ```
-        
-        ### Commandline options for translating cDNA to protein sequence
-        ```
-          --protein-sequence-length PROTEIN_SEQUENCE_LENGTH
-          
-          --max-reference-transcript-mismatches MAX_REFERENCE_TRANSCRIPT_MISMATCHES
-                                Maximum number of mismatches between variant sequence
-                                reference sequence before a candidate reading frame is
-                                ignored.
-                                
-          --count-mismatches-after-variant
-                                If true, mismatches after the variant locus will count
-                                toward the --max-reference-transcript-mismatches
-                                filter.
-                                
-          --min-transcript-prefix-length MIN_TRANSCRIPT_PREFIX_LENGTH
-                                Number of nucleotides before the variant we try to
-                                match against a reference transcript. Values greater
-                                than zero exclude variants near the start codon of
-                                transcripts without 5' UTRs.
-                                
-          --max-protein-sequences-per-variant MAX_PROTEIN_SEQUENCES_PER_VARIANT
-        
-        ```
-        
-        ### Commandline options for filtering 
-        
-        ```
-          --min-alt-rna-reads MIN_ALT_RNA_READS
-                                Minimum number of reads supporting variant allele
-                                (default 3)
-        
-          --min-alt-rna-fragments MIN_ALT_RNA_FRAGMENTS
-                                Minimum number of fragments supporting variant allele
-                                (default 2). Note that this option is the same as
-                                --min-alt-rna-reads for single-end sequencing.
-        
-          --min-alt-rna-fraction MIN_ALT_RNA_FRACTION
-                                Minimum ratio of fragments supporting variant allele
-                                to total RNA fragments (default 0.005).
-        
-          --min-ratio-alt-to-other-fragments MIN_RATIO_ALT_TO_OTHER_FRAGMENTS
-                                At loci where alleles other than the ref and a single
-                                alt are supported, this parameter controls how many
-                                more times fragments supporting the variant allele are
-                                required relative to other non-reference alleles
-                                (default 3.0).
-        ```
-        
-        ### Commandline options for writing an output CSV
-        
-        ```
-          --output OUTPUT       Output CSV file
-          
-          --output-columns OUTPUT_COLUMNS [OUTPUT_COLUMNS ...]
-                                Subset of columns to write
-        
-        ```
-        
-        
-        
-        ## Internal Design
-        
-        ![](isovar_design.png)
-        
-        The inputs to Isovar are one or more somatic variant call (VCF) files, along with a BAM file 
-        containing aligned tumor RNA reads. The following objects are used to aggregate information within Isovar:
-        
-        * [LocusRead](https://github.com/openvax/isovar/blob/master/isovar/locus_read.py): Isovar examines each variant locus and extracts reads overlapping that locus, 
-        represented by `LocusRead`. The `LocusRead` representation allows filtering  based
-        on quality and alignment criteria (e.g. MAPQ > 0) which are thrown away in later stages
-        of Isovar. 
-        
-        * [AlleleRead](https://github.com/openvax/isovar/blob/master/isovar/allele_read.py): Once `LocusRead` objects have been filtered, they are converted into a simplified 
-        representation called `AlleleRead`. Each `AlleleRead` contains only the cDNA sequences 
-        *before*, *at*, and *after* the variant locus. 
-        
-        * [ReadEvidence](https://github.com/openvax/isovar/blob/master/isovar/read_evidence.py): 
-        The set of `AlleleRead` objects overlapping a mutation's location may support many different
-        distinct allele. The `ReadEvidence` type represents the grouping of these reads into
-        *ref*, *alt* and *other* `AlleleRead` sets, where *ref* reads agree with the reference
-         sequence, *alt* reads agree with the given mutation, and *other* reads contain all
-         non-ref/non-alt alleles. The *alt* reads will be used later to determine
-        a mutant coding sequence, but the *ref* and *other* groups are also kept in case they are
-        useful for filtering. 
-        
-        * [VariantSequence](https://github.com/openvax/isovar/blob/master/isovar/variant_sequence.py):
-        Overlapping `AlleleRead`s containing the same mutation are assembled into a longer
-        sequence. The `VariantSequence` object represents this candidate coding sequence, as well
-        as all the `AlleleRead` objects which were used to create it.
-        
-        * [ReferenceContext](https://github.com/openvax/isovar/blob/master/isovar/reference_context.py): To determine the reading frame in which to translate a `VariantSequence`, Isovar
-        looks at all Ensembl annotated transcripts overlapping the locus and collapses them
-         into one or more `ReferenceContext` object. Each `ReferenceContext` represents the 
-         cDNA sequence upstream of the variant locus and in which of the {0, +1, +2} reading frames
-          it is translated. 
-        
-        * [Translation](https://github.com/openvax/isovar/blob/master/isovar/translation.py): Use the reading frame from a `ReferenceContext` to translate a `VariantSequence` 
-        into a protein fragment, represented by `Translation`.
-        
-        * [ProteinSequence](https://github.com/openvax/isovar/blob/master/isovar/protein_sequence.py):
-        Multiple distinct variant sequences and reference contexts can generate the same translations, so we aggregate those equivalent `Translation` objects into a `ProteinSequence`.
-        
-        * [IsovarResult](https://github.com/openvax/isovar/blob/master/isovar/isovar_result.py): Since a single variant locus might have reads which assemble into multiple incompatible coding sequences, an `IsovarResult` represents a variant and one or more `ProteinSequence` objects which are associated with it. We typically don't want to deal with *every* possible translation of *every* distinct sequence detected around a variant, so the protein sequences are sorted by their number of supporting fragments and the best protein sequence is made easy to access. The `IsovarResult` object also has many informative properties such `num_alt_fragments`, `fraction_ref_reads`, &c.  
-        
-        
-        ## Other Isovar Commandline Tools
-        
-        <dl>
-        <dt>isovar-protein-sequences --vcf variants.vcf --bam rna.bam</dt>
-        <dd>All protein sequences which can be assembled from RNA reads for any of the given variants.</dd>
-        
-        <dt>isovar-allele-counts --vcf variants.vcf --bam rna.bam</dt>
-        <dd>Counts of reads and fragments supporting the ref, alt, and other alleles at all given variant locations.</dd>
-        
-        <dt>isovar-allele-reads --vcf variants.vcf --bam rna.bam</dt>
-        <dd>Sequences of all reads overlapping any of the given variants.</dd>
-         
-        <dt>isovar-translations --vcf variants.vcf --bam rna.bam</dt>
-        <dd>All possible translations of any assembled cDNA sequence containing any of the given variants in the reference frame of any matching transcript.</dd>
-        
-        <dt>isovar-reference-contexts --vcf variants.vcf</dt>
-        <dd>Shows all candidate reference contexts (sequence and reading frame) before each variant, derived from overlapping reference coding transcripts.</dd>
-        
-        <dt>isovar-variant-reads --vcf variants.vcf --bam rna.bam</dt>
-        <dd>Like the isovar-allele-reads command but limited only to reads which support the alt allele.</dd>
-        
-        <dt>isovar-variant-sequences --vcf variants.vcf --bam rna.bam</dt>
-        <dd>Shows all assembled cDNA coding sequences supporting any of the given variants.</dd>
-        </dl>
-        
-        ## Sequencing Recommendations
-        
-        Isovar works best with high quality / high coverage mRNA sequence data. 
-        This means that you will get best results from >100M paired-end reads sequenced on an 
-        Illumina HiSeq from a library enriched with poly-A capture. The number of reads varies 
-        depending on degree of RNA degradation and tumor purity. The read length will determine 
-        the longest protein sequence you can recover, since Isovar's cDNA assembly only 
-        considers reads that overlap a variant. With 100bp reads you will be able to assemble
-        at most 199bp of sequence around a somatic single nucleotide variant, and consequently 
-        only be to determine 66 amino acids from the protein sequence. If you disable the cDNA 
-        assembly algorithm then a 100bp read will only be able to determine 33 amino acids.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<a href="https://travis-ci.org/openvax/isovar">
+    <img src="https://travis-ci.org/openvax/isovar.svg?branch=master" alt="Build Status" />
+</a>
+<a href="https://coveralls.io/github/openvax/isovar?branch=master">
+    <img src="https://coveralls.io/repos/openvax/isovar/badge.svg?branch=master&service=github" alt="Coverage Status" />
+</a>
+<a href="https://pypi.python.org/pypi/isovar/">
+    <img src="https://img.shields.io/pypi/v/isovar.svg?maxAge=1000" alt="PyPI" />
+</a>
+
+# Isovar
+
+* [Overview](#overview)
+* [Python API](#python-api)
+* [Commandline](#commandline)
+* [Internal Design](#internal-design)
+* [Other Isovar Commandline Tools](#other-isovar-commandline-tools)
+* [Sequencing Recommendations](#sequencing-recommendations)
+
+## Overview
+Isovar determines mutant protein subsequences around mutations from cancer RNAseq data.
+
+Isovar works by:
+
+ 1) collecting RNA reads which spanning the location of a variant,
+
+ 2) filtering the RNA reads to those which support the mutation,
+
+ 3) assembling mutant reads into longer coding sequences,  
+
+ 4) matching mutant coding sequences against reference annotated reading
+frames, and
+
+ 5) translating coding sequences determined directly from RNA into mutant protein sequences.
+
+The assembled coding sequences may incorporate proximal 
+(germline and somatic) variants, along with any splicing alterations 
+which occur due to modified splice signals.
+
+## Python API
+
+In the example below, `isovar.run_isovar` returns a list of `isovar.IsovarResult` objects. 
+Each of these objects corresponds to a single input variant and contains all of the information about the RNA evidence at that variant's location and any mutant protein sequences which were assembled for the variant.
+
+```python
+
+from isovar import run_isovar
+
+isovar_results = run_isovar(
+    variants="cancer-mutations.vcf",
+    alignment_file="tumor-rna.bam")
+    
+# this code traverses every variant and prints the number
+# of RNA reads which support the alt allele for variants
+# which had a successfully assembled/translated protein sequence
+for isovar_result in isovar_results:
+    # if any protein sequences were assembled from RNA
+    # then the one with most supporting reads can be
+    # accessed from a property called `top_protein_sequence`.
+    if isovar_result.top_protein_sequence is not None:
+        # print number of distinct fragments supporting the
+        # the variant allele for this mutation
+        print(isovar_result.variant, isovar_result.num_alt_fragments)
+    
+```
+
+A collection of `IsovarResult` objects can also be flattened into a Pandas DataFrame:
+
+```python
+
+from isovar import run_isovar, isovar_results_to_dataframe
+
+df =  isovar_results_to_dataframe(
+        run_isovar(
+            variants="cancer-mutations.vcf",
+            alignment_file="tumor-rna.bam"))
+```
+
+
+### Python API options for collecting RNA reads
+
+To change how Isovar collects and filters RNA reads you can create
+your own instance of the `isovar.ReadCollector` class and pass it to `run_isovar`.
+```python
+from isovar import run_isovar, ReadCollector
+
+# create a custom ReadCollector to change options for how RNA reads are processed
+read_collector = ReadCollector(
+    use_duplicate_reads=True,
+    use_secondary_alignments=True, 
+    use_soft_clipped_bases=True)
+
+isovar_results = run_isovar(
+    variants="cancer-mutations.vcf",
+    alignment_file="tumor-rna.bam",
+    read_collector=read_collector)
+
+````
+
+
+### Python API options for coding sequence assembly and translation
+
+To change how Isovar assembles RNA reads into coding sequences, determines their
+reading frames, and groups translated amino acid sequences you can create your
+own instance of the `isovar.ProteinSequenceCreator` class and pass it to `run_isovar`.
+
+
+```python
+from isovar import run_isovar, ProteinSequenceCreator
+
+# create a custom ProteinSequenceCreator to change options for how
+# protein sequences are assembled from RNA reads
+protein_sequence_creator = ProteinSequenceCreator(
+    # number of amino acids we're aiming for, coding sequences
+    # might still give us a shorter sequence due to an early stop 
+    # codon or poor coverage
+    protein_sequence_length=30,
+    # minimum number of reads covering each base of the coding sequence
+    min_variant_sequence_coverage=2,
+    # how much of a reference transcript should a coding sequence match before
+    # we use it to establish a reading frame
+    min_transcript_prefix_length=20,
+    # how many mismatches allowed between coding sequence (before the variant)
+    # and transcript (before the variant location)
+    max_transcript_mismatches=2,
+    # also count mismatches after the variant location toward
+    # max_transcript_mismatches
+    count_mismatches_after_variant=False,
+    # if more than one protein sequence can be assembled for a variant
+    # then drop any beyond this number 
+    max_protein_sequences_per_variant=1,
+    # if set to False then coding sequence will be derived from
+    # a single RNA read with the variant closest to its center
+    variant_sequence_assembly=True,
+    # how many nucleotides must two reads overlap before they are combined
+    # into a single coding sequence
+    min_assembly_overlap_size=30)
+
+isovar_results = run_isovar(
+    variants="cancer-mutations.vcf",
+    alignment_file="tumor-rna.bam",
+    protein_sequence_creator=protein_sequence_creator)
+```
+
+### Python API for filtering results
+
+You can filter a collection of `IsovarResult` objects by any of their numerical properties using the `filter_thresholds` option
+of the `run_isovar` function. The value expected for this argument is a dictionary whose keys have named like `'min_fraction_ref_reads'` or `'max_num_alt_fragments'`  and whose values are numerical thresholds.
+Everything after the `'min_'` or `'max_'` at the start of a key is expected to be the name of a property of `IsovarResult`. 
+Many of the commonly accessed properties regarding RNA read evidence follow the pattern: 
+```
+{num|fraction}_{ref|alt|other}_{reads|fragments} 
+```
+
+For example, in the following code the results are filtered to have 10 or more alt reads supporting a variant and no more than 25% of the fragments supporting an allele other than the ref or alt.
+```python
+from isovar import run_isovar
+
+isovar_results = run_isovar(
+    variants="cancer-mutations.vcf",
+    alignment_file="tumor-rna.bam",
+    filter_thresholds={"min_num_alt_reads": 10, "max_fraction_other_fragments": 0.25})    
+
+for isovar_result in isovar_results:
+    # print each variant and whether it passed both filters
+    print(isovar_result.variant, isovar_result.passes_all_filters)
+```
+
+A variant which fails one or more filters is not excluded from the result collection but it has `False` values in its corresponding 
+`filter_values` dictionary property and will have a `False` value for the `passes_all_filters` property. 
+
+If a result collection is flattened into a DataFrame then each filter is included as a column. 
+
+It's also possible to filter on boolean properties (without numerical thresholds) by passing `filter_flags` to `run_isovar`. These boolean
+properties can be further negated by prepending 'not_' to the property name, so that both `'protein_sequence_matches_predicted_effect'` and `'not_protein_sequence_matches_predicted_effect'` are valid names for `filter_flags`.
+
+## Commandline 
+
+Basic example:
+
+```sh
+$ isovar  \
+    --vcf somatic-variants.vcf  \
+    --bam rnaseq.bam \
+    --protein-sequence-length 30 \
+    --output isovar-results.csv
+```
+
+### Commandline options for loading variants
+
+###
+```
+  --vcf VCF             Genomic variants in VCF format
+  
+  --maf MAF             Genomic variants in TCGA's MAF format
+  
+  --variant CHR POS REF ALT
+                        Individual variant as 4 arguments giving chromsome,
+                        position, ref, and alt. Example: chr1 3848 C G. Use
+                        '.' to indicate empty alleles for insertions or
+                        deletions.
+  
+  --genome GENOME       What reference assembly your variant coordinates are
+                        using. Examples: 'hg19', 'GRCh38', or 'mm9'. This
+                        argument is ignored for MAF files, since each row
+                        includes the reference. For VCF files, this is used if
+                        specified, and otherwise is guessed from the header.
+                        For variants specfied on the commandline with
+                        --variant, this option is required.
+  
+  --download-reference-genome-data
+                        Automatically download genome reference data required
+                        for annotation using PyEnsembl. Otherwise you must
+                        first run 'pyensembl install' for the release/species
+                        corresponding to the genome used in your VCF.
+  
+  --json-variants JSON_VARIANTS
+                        Path to Varcode.VariantCollection object serialized as
+                        a JSON file.
+
+```
+
+### Commandline options for loading aligned tumor RNA-seq reads
+
+```
+  --bam BAM             BAM file containing RNAseq reads
+  
+  --min-mapping-quality MIN_MAPPING_QUALITY
+                        Minimum MAPQ value to allow for a read (default 1)
+  
+  --use-duplicate-reads
+                        By default, reads which have been marked as duplicates
+                        are excluded.Use this option to include duplicate
+                        reads.
+                        
+  --drop-secondary-alignments
+                        By default, secondary alignments are included in
+                        reads, use this option to instead only use primary
+                        alignments.
+```
+
+### Commandline options for coding sequence assembly
+```
+  --min-variant-sequence-coverage MIN_VARIANT_SEQUENCE_COVERAGE
+                        Minimum number of reads supporting a variant sequence
+                        (default 2)
+                        
+  --disable-variant-sequence-assembly
+                        Disable assemble variant cDNA sequence from
+                        overlapping reads
+```
+
+### Commandline options for translating cDNA to protein sequence
+```
+  --protein-sequence-length PROTEIN_SEQUENCE_LENGTH
+  
+  --max-reference-transcript-mismatches MAX_REFERENCE_TRANSCRIPT_MISMATCHES
+                        Maximum number of mismatches between variant sequence
+                        reference sequence before a candidate reading frame is
+                        ignored.
+                        
+  --count-mismatches-after-variant
+                        If true, mismatches after the variant locus will count
+                        toward the --max-reference-transcript-mismatches
+                        filter.
+                        
+  --min-transcript-prefix-length MIN_TRANSCRIPT_PREFIX_LENGTH
+                        Number of nucleotides before the variant we try to
+                        match against a reference transcript. Values greater
+                        than zero exclude variants near the start codon of
+                        transcripts without 5' UTRs.
+                        
+  --max-protein-sequences-per-variant MAX_PROTEIN_SEQUENCES_PER_VARIANT
+
+```
+
+### Commandline options for filtering 
+
+```
+  --min-alt-rna-reads MIN_ALT_RNA_READS
+                        Minimum number of reads supporting variant allele
+                        (default 3)
+
+  --min-alt-rna-fragments MIN_ALT_RNA_FRAGMENTS
+                        Minimum number of fragments supporting variant allele
+                        (default 2). Note that this option is the same as
+                        --min-alt-rna-reads for single-end sequencing.
+
+  --min-alt-rna-fraction MIN_ALT_RNA_FRACTION
+                        Minimum ratio of fragments supporting variant allele
+                        to total RNA fragments (default 0.005).
+
+  --min-ratio-alt-to-other-fragments MIN_RATIO_ALT_TO_OTHER_FRAGMENTS
+                        At loci where alleles other than the ref and a single
+                        alt are supported, this parameter controls how many
+                        more times fragments supporting the variant allele are
+                        required relative to other non-reference alleles
+                        (default 3.0).
+```
+
+### Commandline options for writing an output CSV
+
+```
+  --output OUTPUT       Output CSV file
+  
+  --output-columns OUTPUT_COLUMNS [OUTPUT_COLUMNS ...]
+                        Subset of columns to write
+
+```
+
+
+
+## Internal Design
+
+![](isovar_design.png)
+
+The inputs to Isovar are one or more somatic variant call (VCF) files, along with a BAM file 
+containing aligned tumor RNA reads. The following objects are used to aggregate information within Isovar:
+
+* [LocusRead](https://github.com/openvax/isovar/blob/master/isovar/locus_read.py): Isovar examines each variant locus and extracts reads overlapping that locus, 
+represented by `LocusRead`. The `LocusRead` representation allows filtering  based
+on quality and alignment criteria (e.g. MAPQ > 0) which are thrown away in later stages
+of Isovar. 
+
+* [AlleleRead](https://github.com/openvax/isovar/blob/master/isovar/allele_read.py): Once `LocusRead` objects have been filtered, they are converted into a simplified 
+representation called `AlleleRead`. Each `AlleleRead` contains only the cDNA sequences 
+*before*, *at*, and *after* the variant locus. 
+
+* [ReadEvidence](https://github.com/openvax/isovar/blob/master/isovar/read_evidence.py): 
+The set of `AlleleRead` objects overlapping a mutation's location may support many different
+distinct allele. The `ReadEvidence` type represents the grouping of these reads into
+*ref*, *alt* and *other* `AlleleRead` sets, where *ref* reads agree with the reference
+ sequence, *alt* reads agree with the given mutation, and *other* reads contain all
+ non-ref/non-alt alleles. The *alt* reads will be used later to determine
+a mutant coding sequence, but the *ref* and *other* groups are also kept in case they are
+useful for filtering. 
+
+* [VariantSequence](https://github.com/openvax/isovar/blob/master/isovar/variant_sequence.py):
+Overlapping `AlleleRead`s containing the same mutation are assembled into a longer
+sequence. The `VariantSequence` object represents this candidate coding sequence, as well
+as all the `AlleleRead` objects which were used to create it.
+
+* [ReferenceContext](https://github.com/openvax/isovar/blob/master/isovar/reference_context.py): To determine the reading frame in which to translate a `VariantSequence`, Isovar
+looks at all Ensembl annotated transcripts overlapping the locus and collapses them
+ into one or more `ReferenceContext` object. Each `ReferenceContext` represents the 
+ cDNA sequence upstream of the variant locus and in which of the {0, +1, +2} reading frames
+  it is translated. 
+
+* [Translation](https://github.com/openvax/isovar/blob/master/isovar/translation.py): Use the reading frame from a `ReferenceContext` to translate a `VariantSequence` 
+into a protein fragment, represented by `Translation`.
+
+* [ProteinSequence](https://github.com/openvax/isovar/blob/master/isovar/protein_sequence.py):
+Multiple distinct variant sequences and reference contexts can generate the same translations, so we aggregate those equivalent `Translation` objects into a `ProteinSequence`.
+
+* [IsovarResult](https://github.com/openvax/isovar/blob/master/isovar/isovar_result.py): Since a single variant locus might have reads which assemble into multiple incompatible coding sequences, an `IsovarResult` represents a variant and one or more `ProteinSequence` objects which are associated with it. We typically don't want to deal with *every* possible translation of *every* distinct sequence detected around a variant, so the protein sequences are sorted by their number of supporting fragments and the best protein sequence is made easy to access. The `IsovarResult` object also has many informative properties such `num_alt_fragments`, `fraction_ref_reads`, &c.  
+
+
+## Other Isovar Commandline Tools
+
+<dl>
+<dt>isovar-protein-sequences --vcf variants.vcf --bam rna.bam</dt>
+<dd>All protein sequences which can be assembled from RNA reads for any of the given variants.</dd>
+
+<dt>isovar-allele-counts --vcf variants.vcf --bam rna.bam</dt>
+<dd>Counts of reads and fragments supporting the ref, alt, and other alleles at all given variant locations.</dd>
+
+<dt>isovar-allele-reads --vcf variants.vcf --bam rna.bam</dt>
+<dd>Sequences of all reads overlapping any of the given variants.</dd>
+ 
+<dt>isovar-translations --vcf variants.vcf --bam rna.bam</dt>
+<dd>All possible translations of any assembled cDNA sequence containing any of the given variants in the reference frame of any matching transcript.</dd>
+
+<dt>isovar-reference-contexts --vcf variants.vcf</dt>
+<dd>Shows all candidate reference contexts (sequence and reading frame) before each variant, derived from overlapping reference coding transcripts.</dd>
+
+<dt>isovar-variant-reads --vcf variants.vcf --bam rna.bam</dt>
+<dd>Like the isovar-allele-reads command but limited only to reads which support the alt allele.</dd>
+
+<dt>isovar-variant-sequences --vcf variants.vcf --bam rna.bam</dt>
+<dd>Shows all assembled cDNA coding sequences supporting any of the given variants.</dd>
+</dl>
+
+## Sequencing Recommendations
+
+Isovar works best with high quality / high coverage mRNA sequence data. 
+This means that you will get best results from >100M paired-end reads sequenced on an 
+Illumina HiSeq from a library enriched with poly-A capture. The number of reads varies 
+depending on degree of RNA degradation and tumor purity. The read length will determine 
+the longest protein sequence you can recover, since Isovar's cDNA assembly only 
+considers reads that overlap a variant. With 100bp reads you will be able to assemble
+at most 199bp of sequence around a somatic single nucleotide variant, and consequently 
+only be to determine 66 amino acids from the protein sequence. If you disable the cDNA 
+assembly algorithm then a 100bp read will only be able to determine 33 amino acids.
```

#### html2text {}

```diff
@@ -1,15 +1,20 @@
-Metadata-Version: 2.1 Name: isovar Version: 1.1.1 Summary: Determine mutant
+Metadata-Version: 2.1 Name: isovar Version: 1.3.0 Summary: Determine mutant
 protein sequences from RN using assembly around variants Home-page: https://
 github.com/openvax/isovar Author: Alex Rubinsteyn, Arman Aksoy, Julia Kodysh
 Author-email: alex.rubinsteyn@mssm.edu License: http://www.apache.org/licenses/
-LICENSE-2.0.html Description: [Build_Status] [Coverage_Status] [PyPI] # Isovar
-* [Overview](#overview) * [Python API](#python-api) * [Commandline]
-(#commandline) * [Internal Design](#internal-design) * [Other Isovar
-Commandline Tools](#other-isovar-commandline-tools) * [Sequencing
+LICENSE-2.0.html Classifier: Development Status :: 4 - Beta Classifier:
+Environment :: Console Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
+Approved :: Apache Software License Classifier: Programming Language :: Python
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics Description-
+Content-Type: text/markdown License-File: LICENSE [Build_Status] [Coverage
+Status] [PyPI] # Isovar * [Overview](#overview) * [Python API](#python-api) *
+[Commandline](#commandline) * [Internal Design](#internal-design) * [Other
+Isovar Commandline Tools](#other-isovar-commandline-tools) * [Sequencing
 Recommendations](#sequencing-recommendations) ## Overview Isovar determines
 mutant protein subsequences around mutations from cancer RNAseq data. Isovar
 works by: 1) collecting RNA reads which spanning the location of a variant, 2)
 filtering the RNA reads to those which support the mutation, 3) assembling
 mutant reads into longer coding sequences, 4) matching mutant coding sequences
 against reference annotated reading frames, and 5) translating coding sequences
 determined directly from RNA into mutant protein sequences. The assembled
@@ -214,13 +219,8 @@
 with poly-A capture. The number of reads varies depending on degree of RNA
 degradation and tumor purity. The read length will determine the longest
 protein sequence you can recover, since Isovar's cDNA assembly only considers
 reads that overlap a variant. With 100bp reads you will be able to assemble at
 most 199bp of sequence around a somatic single nucleotide variant, and
 consequently only be to determine 66 amino acids from the protein sequence. If
 you disable the cDNA assembly algorithm then a 100bp read will only be able to
-determine 33 amino acids. Platform: UNKNOWN Classifier: Development Status :: 4
-- Beta Classifier: Environment :: Console Classifier: Operating System :: OS
-Independent Classifier: Intended Audience :: Science/Research Classifier:
-License :: OSI Approved :: Apache Software License Classifier: Programming
-Language :: Python Classifier: Topic :: Scientific/Engineering :: Bio-
-Informatics Description-Content-Type: text/markdown
+determine 33 amino acids.
```

### Comparing `isovar-1.1.1/README.md` & `isovar-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/read_evidence.py` & `isovar-1.3.0/isovar/read_evidence.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/translation_key.py` & `isovar-1.3.0/isovar/translation_key.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/filtering.py` & `isovar-1.3.0/isovar/filtering.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/alignment_score.py` & `isovar-1.3.0/isovar/alignment_score.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/translation_helpers.py` & `isovar-1.3.0/isovar/translation_helpers.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/phasing.py` & `isovar-1.3.0/isovar/phasing.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/isovar_result.py` & `isovar-1.3.0/isovar/isovar_result.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/default_parameters.py` & `isovar-1.3.0/isovar/default_parameters.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/allele_read.py` & `isovar-1.3.0/isovar/allele_read.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/variant_orf.py` & `isovar-1.3.0/isovar/variant_orf.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/protein_sequence_helpers.py` & `isovar-1.3.0/isovar/protein_sequence_helpers.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/logging.conf` & `isovar-1.3.0/isovar/logging.conf`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/effect_prediction.py` & `isovar-1.3.0/isovar/effect_prediction.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/read_collector.py` & `isovar-1.3.0/isovar/read_collector.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,20 +30,22 @@
 
 
 class ReadCollector(object):
     """
     ReadCollector holds options related to extracting reads from SAM/BAM alignment files
     and provides methods for different ways to create LocusRead objects.
     """
+
     def __init__(
-            self,
-            use_secondary_alignments=USE_SECONDARY_ALIGNMENTS,
-            use_duplicate_reads=USE_DUPLICATE_READS,
-            min_mapping_quality=MIN_READ_MAPPING_QUALITY,
-            use_soft_clipped_bases=USE_SOFT_CLIPPED_BASES):
+        self,
+        use_secondary_alignments=USE_SECONDARY_ALIGNMENTS,
+        use_duplicate_reads=USE_DUPLICATE_READS,
+        min_mapping_quality=MIN_READ_MAPPING_QUALITY,
+        use_soft_clipped_bases=USE_SOFT_CLIPPED_BASES,
+    ):
         """
         Parameters
         ----------
         use_secondary_alignments : bool
             Use a read even when it's not the primary alignment at a locus
 
         use_duplicate_reads : bool
@@ -57,18 +59,16 @@
         """
         self.use_secondary_alignments = use_secondary_alignments
         self.use_duplicate_reads = use_duplicate_reads
         self.min_mapping_quality = min_mapping_quality
         self.use_soft_clipped_bases = use_soft_clipped_bases
 
     def locus_read_from_pysam_aligned_segment(
-            self,
-            pysam_aligned_segment,
-            base0_start_inclusive,
-            base0_end_exclusive):
+        self, pysam_aligned_segment, base0_start_inclusive, base0_end_exclusive
+    ):
         """
         Create LocusRead from pysam.AlignedSegment object and the start/end indices
         of the locus of interest. If any essential fields of the aligned segment
         are missing then None is returned instead.
 
         Parameters
         ----------
@@ -88,36 +88,33 @@
 
         if pysam_aligned_segment.is_duplicate and not self.use_duplicate_reads:
             return None
 
         name = pysam_aligned_segment.query_name
 
         if name is None:
-            logger.warn(
-                "Read missing name at position %d",
-                base0_start_inclusive + 1)
+            logger.warn("Read missing name at position %d", base0_start_inclusive + 1)
             return None
 
         if pysam_aligned_segment.is_unmapped:
-            logger.warn(
-                "How did we get unmapped read '%s' in a pileup?", name)
+            logger.warn("How did we get unmapped read '%s' in a pileup?", name)
             return None
 
-
         mapping_quality = pysam_aligned_segment.mapping_quality
 
         if self.min_mapping_quality > 0 and (mapping_quality is None):
             logger.debug("Skipping read '%s' due to missing MAPQ" % name)
             return None
         elif mapping_quality < self.min_mapping_quality:
             logger.debug(
                 "Skipping read '%s' due to low MAPQ: %d < %d",
                 name,
                 mapping_quality,
-                self.min_mapping_quality)
+                self.min_mapping_quality,
+            )
             return None
 
         sequence = pysam_aligned_segment.query_sequence
 
         if sequence is None:
             logger.warn("Skipping read '%s' due to missing sequence" % name)
             return None
@@ -125,34 +122,33 @@
         base_qualities = pysam_aligned_segment.query_qualities
 
         if base_qualities is None:
             logger.warn("Skipping read '%s' due to missing base qualities" % name)
             return None
         elif len(base_qualities) != len(sequence):
             logger.warn(
-                "Skipping read '%s' due to mismatch in length of sequence (%d) and qualities (%d)" % (
-                    name,
-                    len(sequence),
-                    len(base_qualities)))
+                "Skipping read '%s' due to mismatch in length of sequence (%d) and qualities (%d)"
+                % (name, len(sequence), len(base_qualities))
+            )
             return None
 
         # By default, AlignedSegment.get_reference_positions only returns base-1 positions
         # from the reference that are within the alignment. If full_length is set,
         # None values will be included for any soft-clipped or unaligned positions
         # within the read. The returned list will thus be of the same
         # length as the read.
-        base0_reference_positions = \
-            pysam_aligned_segment.get_reference_positions(full_length=True)
+        base0_reference_positions = pysam_aligned_segment.get_reference_positions(
+            full_length=True
+        )
 
         if len(base0_reference_positions) != len(base_qualities):
             logger.warn(
-                "Skipping read '%s' due to mismatch in length of positions (%d) and qualities (%d)" % (
-                    name,
-                    len(base0_reference_positions),
-                    len(base_qualities)))
+                "Skipping read '%s' due to mismatch in length of positions (%d) and qualities (%d)"
+                % (name, len(base0_reference_positions), len(base_qualities))
+            )
             return None
 
         reference_interval_size = base0_end_exclusive - base0_start_inclusive
         if reference_interval_size < 0:
             raise ValueError("Unexpected interval start after interval end")
 
         # TODO:
@@ -187,28 +183,31 @@
             # interval of [start, start).
             #
             # To deal with insertions at the beginning and end of a read we're
             # going to allow the start/end to be None.
             reference_position_before_insertion = base0_start_inclusive - 1
             reference_position_after_insertion = base0_start_inclusive
             if reference_position_before_insertion in base0_reference_positions:
-                read_base0_before_insertion = \
-                    base0_reference_positions.index(
-                        reference_position_before_insertion)
+                read_base0_before_insertion = base0_reference_positions.index(
+                    reference_position_before_insertion
+                )
             else:
                 return None
 
             if reference_position_after_insertion in base0_reference_positions:
                 read_base0_after_insertion = base0_reference_positions.index(
-                    reference_position_after_insertion)
+                    reference_position_after_insertion
+                )
             else:
                 return None
 
             if read_base0_after_insertion - read_base0_after_insertion == 1:
-                read_base0_start_inclusive = read_base0_end_exclusive = read_base0_before_insertion + 1
+                read_base0_start_inclusive = read_base0_end_exclusive = (
+                    read_base0_before_insertion + 1
+                )
             else:
                 read_base0_start_inclusive = read_base0_before_insertion + 1
                 read_base0_end_exclusive = read_base0_after_insertion
         else:
             # Reference bases are selected for match or deletion.
             #
             # What happens if the reference bases are interspersed with insertions?
@@ -226,72 +225,78 @@
             # In this case we need to figure out the first and last positions
             # which match the inclusive interval and then convert it to a half-open
             # interval. One possibly more obvious alternative is just to
             # figure out which read indices correspond to base0_start_inclusive and
             # base0_end_exclusive but this would fail if base0_end_exclusive is
             # after the end the end of the read.
             if base0_start_inclusive in base0_reference_positions:
-                read_base0_start_inclusive = base0_reference_positions.index(base0_start_inclusive)
+                read_base0_start_inclusive = base0_reference_positions.index(
+                    base0_start_inclusive
+                )
             elif base0_start_inclusive - 1 in base0_reference_positions:
                 # if first base of reference locus isn't mapped, try getting the base
                 # before it and then adding one to its corresponding base index
-                read_base0_position_before_locus = \
-                    base0_reference_positions.index(base0_start_inclusive - 1)
+                read_base0_position_before_locus = base0_reference_positions.index(
+                    base0_start_inclusive - 1
+                )
                 read_base0_start_inclusive = read_base0_position_before_locus + 1
             else:
                 return None
 
             if base0_end_exclusive in base0_reference_positions:
-                read_base0_end_exclusive = \
-                    base0_reference_positions.index(base0_end_exclusive)
+                read_base0_end_exclusive = base0_reference_positions.index(
+                    base0_end_exclusive
+                )
             elif (base0_end_exclusive - 1) in base0_reference_positions:
                 # if exclusive last index of reference interval doesn't have a corresponding
                 # base position then try getting the base position of the reference
                 # position before it and then adding one
-                read_base0_end_inclusive = \
-                    base0_reference_positions.index(base0_end_exclusive - 1)
+                read_base0_end_inclusive = base0_reference_positions.index(
+                    base0_end_exclusive - 1
+                )
                 read_base0_end_exclusive = read_base0_end_inclusive + 1
             else:
                 return None
 
         if isinstance(sequence, bytes):
-            sequence = sequence.decode('ascii')
+            sequence = sequence.decode("ascii")
 
         if not self.use_soft_clipped_bases:
             # if we're not allowing soft clipped based then
             # the fraction of the read which is usable may be smaller
             # than the sequence, qualities, and alignment positions
             # we've extracted, so slice through those to get rid of
             # soft-clipped ends of the read
             aligned_subsequence_start = pysam_aligned_segment.query_alignment_start
             aligned_subsequence_end = pysam_aligned_segment.query_alignment_end
             sequence = sequence[aligned_subsequence_start:aligned_subsequence_end]
             base0_reference_positions = base0_reference_positions[
-                aligned_subsequence_start:aligned_subsequence_end]
-            base_qualities = base_qualities[aligned_subsequence_start:aligned_subsequence_end]
+                aligned_subsequence_start:aligned_subsequence_end
+            ]
+            base_qualities = base_qualities[
+                aligned_subsequence_start:aligned_subsequence_end
+            ]
             if read_base0_start_inclusive is not None:
                 read_base0_start_inclusive -= aligned_subsequence_start
             if read_base0_end_exclusive is not None:
                 read_base0_end_exclusive -= aligned_subsequence_start
         return LocusRead(
             name=name,
             sequence=sequence,
             reference_positions=base0_reference_positions,
             quality_scores=base_qualities,
             reference_base0_start_inclusive=base0_start_inclusive,
             reference_base0_end_exclusive=base0_end_exclusive,
             read_base0_start_inclusive=read_base0_start_inclusive,
-            read_base0_end_exclusive=read_base0_end_exclusive)
+            read_base0_end_exclusive=read_base0_end_exclusive,
+        )
 
     def get_locus_reads(
-            self,
-            alignment_file,
-            chromosome,
-            base0_start_inclusive,
-            base0_end_exclusive):
+        self, alignment_file, chromosome, base0_start_inclusive, base0_end_exclusive
+    ):
         """
         Create LocusRead objects for reads which overlap the given chromosome,
         start, and end positions. The actual work to figure out if what's between
         those positions matches a variant happens later when LocusRead objects are
         converted to AlleleRead objects.
 
         Parameters
@@ -308,47 +313,52 @@
 
         Returns a sequence of ReadAtLocus objects
         """
         logger.debug(
             "Gathering reads at locus %s:%d-%d",
             chromosome,
             base0_start_inclusive,
-            base0_end_exclusive)
+            base0_end_exclusive,
+        )
         reads = []
         total_count = 0
         # check overlap against wider overlap to make sure we don't miss
         # any reads
         base0_pos_before_start = base0_start_inclusive - 1
         base0_pos_after_end = base0_end_exclusive + 1
         for aligned_segment in alignment_file.fetch(
-                chromosome,
-                base0_start_inclusive,
-                base0_end_exclusive):
+            chromosome, base0_pos_before_start, base0_pos_after_end
+        ):
             total_count += 1
             # we get a significant speed up if we skip reads that have spliced
             # out the entire interval of interest. this is redundant with the
             # attempt to find mapping positions in
             #   self.locus_read_from_pysam_aligned_segment
             # but we do it here to skip the function call overhead for loci
             # where ~1M reads are mapped
-            if aligned_segment.get_overlap(base0_pos_before_start, base0_pos_after_end) == 0:
+            if (
+                aligned_segment.get_overlap(base0_pos_before_start, base0_pos_after_end)
+                == 0
+            ):
                 continue
             read = self.locus_read_from_pysam_aligned_segment(
                 aligned_segment,
                 base0_start_inclusive=base0_start_inclusive,
-                base0_end_exclusive=base0_end_exclusive)
+                base0_end_exclusive=base0_end_exclusive,
+            )
             if read is not None:
                 reads.append(read)
         logger.info(
             "Kept %d/%d reads overlapping locus %s:%d-%d",
             len(reads),
             total_count,
             chromosome,
             base0_start_inclusive,
-            base0_end_exclusive)
+            base0_end_exclusive,
+        )
         return reads
 
     @staticmethod
     def _infer_chromosome_name(variant_chromosome_name, valid_chromosome_names):
         """
         In case the variant is using an hg19 reference name and the alignment
         was against b37 (or vice versa) we have to check whether adding or removing
@@ -379,19 +389,15 @@
             candidate_names.add(candidate.lower())
             candidate_names.add(candidate.upper())
         for candidate in candidate_names:
             if candidate in valid_chromosome_names:
                 return candidate
         return None
 
-    def locus_reads_overlapping_variant(
-            self,
-            alignment_file,
-            variant,
-            chromosome=None):
+    def locus_reads_overlapping_variant(self, alignment_file, variant, chromosome=None):
         """
         Find reads in the given SAM/BAM file which overlap the given variant and
         return them as a list of LocusRead objects.
 
         Parameters
         ----------
         alignment_file : pysam.AlignmentFile
@@ -405,30 +411,33 @@
         if chromosome is None:
             # if a chromosome name isn't manually specified then try
             # to figure out whether adding or removing "chr" is necessary
             # match chromosome names used for variant calling and those
             # found in read alignments
             chromosome = self._infer_chromosome_name(
                 variant_chromosome_name=variant.contig,
-                valid_chromosome_names=set(alignment_file.references))
+                valid_chromosome_names=set(alignment_file.references),
+            )
 
         if chromosome is None:
             # failed to infer a chromsome name for this variant which
             # matches names used in SAM/BAM file
             logger.warning(
                 "Chromosome '%s' from variant %s not in alignment file %s",
                 variant.contig,
                 variant,
-                alignment_file.filename)
+                alignment_file.filename,
+            )
             return []
 
         logger.info(
             "Gathering reads for variant %s (with gene names %s)",
             variant,
-            variant.gene_names)
+            variant.gene_names,
+        )
 
         base1_position, ref, alt = trim_variant(variant)
 
         if len(ref) == 0:
             # If there is no reference sequence in the variant
             # then it's an insertion and the base 0 coordinates
             # will select the space between two bases.
@@ -455,20 +464,18 @@
             base0_start_inclusive = base1_position - 1
             base0_end_exclusive = base0_start_inclusive + len(ref)
 
         return self.get_locus_reads(
             alignment_file=alignment_file,
             chromosome=chromosome,
             base0_start_inclusive=base0_start_inclusive,
-            base0_end_exclusive=base0_end_exclusive)
+            base0_end_exclusive=base0_end_exclusive,
+        )
 
-    def allele_reads_overlapping_variant(
-            self,
-            variant,
-            alignment_file):
+    def allele_reads_overlapping_variant(self, variant, alignment_file):
         """
         Find reads in the given SAM/BAM file which overlap the given variant and
         return them as a list of AlleleRead objects.
 
         Parameters
         ----------
         variant : varcode.Variant
@@ -476,21 +483,19 @@
         alignment_file : pysam.AlignmentFile
             Aligned RNA reads
 
         Returns sequence of AlleleRead objects.
         """
         return allele_reads_from_locus_reads(
             self.locus_reads_overlapping_variant(
-                alignment_file=alignment_file,
-                variant=variant))
+                alignment_file=alignment_file, variant=variant
+            )
+        )
 
-    def read_evidence_for_variant(
-            self,
-            variant,
-            alignment_file):
+    def read_evidence_for_variant(self, variant, alignment_file):
         """
         Find reads in the given SAM/BAM file which overlap the given variant and
         return them as a ReadEvidence object, which splits the reads into
         ref/alt/other groups.
 
         Parameters
         ----------
@@ -498,19 +503,17 @@
 
         alignment_file : pysam.AlignmentFile
             Aligned RNA reads
 
         Returns ReadEvidence
         """
         allele_reads = self.allele_reads_overlapping_variant(
-            variant=variant,
-            alignment_file=alignment_file)
-        return ReadEvidence.from_variant_and_allele_reads(
-            variant,
-            allele_reads)
+            variant=variant, alignment_file=alignment_file
+        )
+        return ReadEvidence.from_variant_and_allele_reads(variant, allele_reads)
 
     def allele_reads_supporting_variant(self, variant, alignment_file):
         """
         Gather AlleleRead objects which contain the same allele as the variant.
 
         Parameters
         ----------
@@ -519,16 +522,16 @@
 
         alignment_file : pysam.AlignmentFile
             Aligned RNA reads
 
         Returns list of AlleleRead
         """
         read_evidence = self.read_evidence_for_variant(
-            variant=variant,
-            alignment_file=alignment_file)
+            variant=variant, alignment_file=alignment_file
+        )
         return read_evidence.alt_reads
 
     def read_evidence_generator(self, variants, alignment_file):
         """
         Consumes a generator of varcode.Variant objects, collects read evidence
         for each variant from the alignment_file, and generates a sequence
         of (Variant, ReadEvidence) pairs.
@@ -541,10 +544,10 @@
         alignment_file : pysam.AlignmentFile
             Aligned RNA reads
 
         Generates sequence of (varcode.Variant, ReadEvidence) pairs
         """
         for variant in variants:
             read_evidence = self.read_evidence_for_variant(
-                variant=variant,
-                alignment_file=alignment_file)
+                variant=variant, alignment_file=alignment_file
+            )
             yield variant, read_evidence
```

### Comparing `isovar-1.1.1/isovar/value_object.py` & `isovar-1.3.0/isovar/value_object.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/variant_orf_helpers.py` & `isovar-1.3.0/isovar/variant_orf_helpers.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/allele_read_helpers.py` & `isovar-1.3.0/isovar/allele_read_helpers.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/reference_coding_sequence_key.py` & `isovar-1.3.0/isovar/reference_coding_sequence_key.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/common.py` & `isovar-1.3.0/isovar/common.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/variant_sequence.py` & `isovar-1.3.0/isovar/variant_sequence.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/dna.py` & `isovar-1.3.0/isovar/dna.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/logging.py` & `isovar-1.3.0/isovar/logging.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/variant_sequence_helpers.py` & `isovar-1.3.0/isovar/variant_sequence_helpers.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/string_helpers.py` & `isovar-1.3.0/isovar/string_helpers.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/dataframe_helpers.py` & `isovar-1.3.0/isovar/dataframe_helpers.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/dataframe_builder.py` & `isovar-1.3.0/isovar/dataframe_builder.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/genetic_code.py` & `isovar-1.3.0/isovar/genetic_code.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/assembly.py` & `isovar-1.3.0/isovar/assembly.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/cli/variant_sequences_args.py` & `isovar-1.3.0/isovar/cli/variant_sequences_args.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/cli/isovar_allele_counts.py` & `isovar-1.3.0/isovar/cli/isovar_allele_counts.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/cli/isovar_reference_contexts.py` & `isovar-1.3.0/isovar/cli/isovar_reference_contexts.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/cli/isovar_variant_sequences.py` & `isovar-1.3.0/isovar/cli/isovar_variant_sequences.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/cli/filter_args.py` & `isovar-1.3.0/isovar/cli/filter_args.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/cli/isovar_allele_reads.py` & `isovar-1.3.0/isovar/cli/isovar_allele_reads.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/cli/isovar_translations.py` & `isovar-1.3.0/isovar/cli/isovar_translations.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/cli/rna_args.py` & `isovar-1.3.0/isovar/cli/rna_args.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/cli/isovar_protein_sequences.py` & `isovar-1.3.0/isovar/cli/isovar_protein_sequences.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/cli/reference_context_args.py` & `isovar-1.3.0/isovar/cli/reference_context_args.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/cli/isovar_variant_reads.py` & `isovar-1.3.0/isovar/cli/isovar_variant_reads.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/cli/protein_sequence_args.py` & `isovar-1.3.0/isovar/cli/protein_sequence_args.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/cli/output_args.py` & `isovar-1.3.0/isovar/cli/output_args.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/cli/__init__.py` & `isovar-1.3.0/isovar/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/cli/isovar_main.py` & `isovar-1.3.0/isovar/cli/isovar_main.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/cli/main_args.py` & `isovar-1.3.0/isovar/cli/main_args.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/cli/translation_args.py` & `isovar-1.3.0/isovar/cli/translation_args.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/protein_sequence.py` & `isovar-1.3.0/isovar/protein_sequence.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/reference_context_helpers.py` & `isovar-1.3.0/isovar/reference_context_helpers.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/variant_helpers.py` & `isovar-1.3.0/isovar/variant_helpers.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/main.py` & `isovar-1.3.0/isovar/main.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/variant_sequence_creator.py` & `isovar-1.3.0/isovar/variant_sequence_creator.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/__init__.py` & `isovar-1.3.0/isovar/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import print_function, division, absolute_import
 
-__version__ = "1.1.1"
+__version__ = "1.3.0"
 
 
 from .allele_read import AlleleRead
 from .dataframe_helpers import isovar_results_to_dataframe
 from .isovar_result import IsovarResult
 from .locus_read import LocusRead
 from .main import run_isovar
```

### Comparing `isovar-1.1.1/isovar/protein_sequence_creator.py` & `isovar-1.3.0/isovar/protein_sequence_creator.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/reference_sequence_key.py` & `isovar-1.3.0/isovar/reference_sequence_key.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/reference_context.py` & `isovar-1.3.0/isovar/reference_context.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/translation.py` & `isovar-1.3.0/isovar/translation.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar/locus_read.py` & `isovar-1.3.0/isovar/locus_read.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/isovar.egg-info/PKG-INFO` & `isovar-1.3.0/isovar.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,411 +1,411 @@
 Metadata-Version: 2.1
 Name: isovar
-Version: 1.1.1
+Version: 1.3.0
 Summary: Determine mutant protein sequences from RN using assembly around variants
 Home-page: https://github.com/openvax/isovar
 Author: Alex Rubinsteyn, Arman Aksoy, Julia Kodysh
 Author-email: alex.rubinsteyn@mssm.edu
 License: http://www.apache.org/licenses/LICENSE-2.0.html
-Description: <a href="https://travis-ci.org/openvax/isovar">
-            <img src="https://travis-ci.org/openvax/isovar.svg?branch=master" alt="Build Status" />
-        </a>
-        <a href="https://coveralls.io/github/openvax/isovar?branch=master">
-            <img src="https://coveralls.io/repos/openvax/isovar/badge.svg?branch=master&service=github" alt="Coverage Status" />
-        </a>
-        <a href="https://pypi.python.org/pypi/isovar/">
-            <img src="https://img.shields.io/pypi/v/isovar.svg?maxAge=1000" alt="PyPI" />
-        </a>
-        
-        # Isovar
-        
-        * [Overview](#overview)
-        * [Python API](#python-api)
-        * [Commandline](#commandline)
-        * [Internal Design](#internal-design)
-        * [Other Isovar Commandline Tools](#other-isovar-commandline-tools)
-        * [Sequencing Recommendations](#sequencing-recommendations)
-        
-        ## Overview
-        Isovar determines mutant protein subsequences around mutations from cancer RNAseq data.
-        
-        Isovar works by:
-        
-         1) collecting RNA reads which spanning the location of a variant,
-        
-         2) filtering the RNA reads to those which support the mutation,
-        
-         3) assembling mutant reads into longer coding sequences,  
-        
-         4) matching mutant coding sequences against reference annotated reading
-        frames, and
-        
-         5) translating coding sequences determined directly from RNA into mutant protein sequences.
-        
-        The assembled coding sequences may incorporate proximal 
-        (germline and somatic) variants, along with any splicing alterations 
-        which occur due to modified splice signals.
-        
-        ## Python API
-        
-        In the example below, `isovar.run_isovar` returns a list of `isovar.IsovarResult` objects. 
-        Each of these objects corresponds to a single input variant and contains all of the information about the RNA evidence at that variant's location and any mutant protein sequences which were assembled for the variant.
-        
-        ```python
-        
-        from isovar import run_isovar
-        
-        isovar_results = run_isovar(
-            variants="cancer-mutations.vcf",
-            alignment_file="tumor-rna.bam")
-            
-        # this code traverses every variant and prints the number
-        # of RNA reads which support the alt allele for variants
-        # which had a successfully assembled/translated protein sequence
-        for isovar_result in isovar_results:
-            # if any protein sequences were assembled from RNA
-            # then the one with most supporting reads can be
-            # accessed from a property called `top_protein_sequence`.
-            if isovar_result.top_protein_sequence is not None:
-                # print number of distinct fragments supporting the
-                # the variant allele for this mutation
-                print(isovar_result.variant, isovar_result.num_alt_fragments)
-            
-        ```
-        
-        A collection of `IsovarResult` objects can also be flattened into a Pandas DataFrame:
-        
-        ```python
-        
-        from isovar import run_isovar, isovar_results_to_dataframe
-        
-        df =  isovar_results_to_dataframe(
-                run_isovar(
-                    variants="cancer-mutations.vcf",
-                    alignment_file="tumor-rna.bam"))
-        ```
-        
-        
-        ### Python API options for collecting RNA reads
-        
-        To change how Isovar collects and filters RNA reads you can create
-        your own instance of the `isovar.ReadCollector` class and pass it to `run_isovar`.
-        ```python
-        from isovar import run_isovar, ReadCollector
-        
-        # create a custom ReadCollector to change options for how RNA reads are processed
-        read_collector = ReadCollector(
-            use_duplicate_reads=True,
-            use_secondary_alignments=True, 
-            use_soft_clipped_bases=True)
-        
-        isovar_results = run_isovar(
-            variants="cancer-mutations.vcf",
-            alignment_file="tumor-rna.bam",
-            read_collector=read_collector)
-        
-        ````
-        
-        
-        ### Python API options for coding sequence assembly and translation
-        
-        To change how Isovar assembles RNA reads into coding sequences, determines their
-        reading frames, and groups translated amino acid sequences you can create your
-        own instance of the `isovar.ProteinSequenceCreator` class and pass it to `run_isovar`.
-        
-        
-        ```python
-        from isovar import run_isovar, ProteinSequenceCreator
-        
-        # create a custom ProteinSequenceCreator to change options for how
-        # protein sequences are assembled from RNA reads
-        protein_sequence_creator = ProteinSequenceCreator(
-            # number of amino acids we're aiming for, coding sequences
-            # might still give us a shorter sequence due to an early stop 
-            # codon or poor coverage
-            protein_sequence_length=30,
-            # minimum number of reads covering each base of the coding sequence
-            min_variant_sequence_coverage=2,
-            # how much of a reference transcript should a coding sequence match before
-            # we use it to establish a reading frame
-            min_transcript_prefix_length=20,
-            # how many mismatches allowed between coding sequence (before the variant)
-            # and transcript (before the variant location)
-            max_transcript_mismatches=2,
-            # also count mismatches after the variant location toward
-            # max_transcript_mismatches
-            count_mismatches_after_variant=False,
-            # if more than one protein sequence can be assembled for a variant
-            # then drop any beyond this number 
-            max_protein_sequences_per_variant=1,
-            # if set to False then coding sequence will be derived from
-            # a single RNA read with the variant closest to its center
-            variant_sequence_assembly=True,
-            # how many nucleotides must two reads overlap before they are combined
-            # into a single coding sequence
-            min_assembly_overlap_size=30)
-        
-        isovar_results = run_isovar(
-            variants="cancer-mutations.vcf",
-            alignment_file="tumor-rna.bam",
-            protein_sequence_creator=protein_sequence_creator)
-        ```
-        
-        ### Python API for filtering results
-        
-        You can filter a collection of `IsovarResult` objects by any of their numerical properties using the `filter_thresholds` option
-        of the `run_isovar` function. The value expected for this argument is a dictionary whose keys have named like `'min_fraction_ref_reads'` or `'max_num_alt_fragments'`  and whose values are numerical thresholds.
-        Everything after the `'min_'` or `'max_'` at the start of a key is expected to be the name of a property of `IsovarResult`. 
-        Many of the commonly accessed properties regarding RNA read evidence follow the pattern: 
-        ```
-        {num|fraction}_{ref|alt|other}_{reads|fragments} 
-        ```
-        
-        For example, in the following code the results are filtered to have 10 or more alt reads supporting a variant and no more than 25% of the fragments supporting an allele other than the ref or alt.
-        ```python
-        from isovar import run_isovar
-        
-        isovar_results = run_isovar(
-            variants="cancer-mutations.vcf",
-            alignment_file="tumor-rna.bam",
-            filter_thresholds={"min_num_alt_reads": 10, "max_fraction_other_fragments": 0.25})    
-        
-        for isovar_result in isovar_results:
-            # print each variant and whether it passed both filters
-            print(isovar_result.variant, isovar_result.passes_all_filters)
-        ```
-        
-        A variant which fails one or more filters is not excluded from the result collection but it has `False` values in its corresponding 
-        `filter_values` dictionary property and will have a `False` value for the `passes_all_filters` property. 
-        
-        If a result collection is flattened into a DataFrame then each filter is included as a column. 
-        
-        It's also possible to filter on boolean properties (without numerical thresholds) by passing `filter_flags` to `run_isovar`. These boolean
-        properties can be further negated by prepending 'not_' to the property name, so that both `'protein_sequence_matches_predicted_effect'` and `'not_protein_sequence_matches_predicted_effect'` are valid names for `filter_flags`.
-        
-        ## Commandline 
-        
-        Basic example:
-        
-        ```sh
-        $ isovar  \
-            --vcf somatic-variants.vcf  \
-            --bam rnaseq.bam \
-            --protein-sequence-length 30 \
-            --output isovar-results.csv
-        ```
-        
-        ### Commandline options for loading variants
-        
-        ###
-        ```
-          --vcf VCF             Genomic variants in VCF format
-          
-          --maf MAF             Genomic variants in TCGA's MAF format
-          
-          --variant CHR POS REF ALT
-                                Individual variant as 4 arguments giving chromsome,
-                                position, ref, and alt. Example: chr1 3848 C G. Use
-                                '.' to indicate empty alleles for insertions or
-                                deletions.
-          
-          --genome GENOME       What reference assembly your variant coordinates are
-                                using. Examples: 'hg19', 'GRCh38', or 'mm9'. This
-                                argument is ignored for MAF files, since each row
-                                includes the reference. For VCF files, this is used if
-                                specified, and otherwise is guessed from the header.
-                                For variants specfied on the commandline with
-                                --variant, this option is required.
-          
-          --download-reference-genome-data
-                                Automatically download genome reference data required
-                                for annotation using PyEnsembl. Otherwise you must
-                                first run 'pyensembl install' for the release/species
-                                corresponding to the genome used in your VCF.
-          
-          --json-variants JSON_VARIANTS
-                                Path to Varcode.VariantCollection object serialized as
-                                a JSON file.
-        
-        ```
-        
-        ### Commandline options for loading aligned tumor RNA-seq reads
-        
-        ```
-          --bam BAM             BAM file containing RNAseq reads
-          
-          --min-mapping-quality MIN_MAPPING_QUALITY
-                                Minimum MAPQ value to allow for a read (default 1)
-          
-          --use-duplicate-reads
-                                By default, reads which have been marked as duplicates
-                                are excluded.Use this option to include duplicate
-                                reads.
-                                
-          --drop-secondary-alignments
-                                By default, secondary alignments are included in
-                                reads, use this option to instead only use primary
-                                alignments.
-        ```
-        
-        ### Commandline options for coding sequence assembly
-        ```
-          --min-variant-sequence-coverage MIN_VARIANT_SEQUENCE_COVERAGE
-                                Minimum number of reads supporting a variant sequence
-                                (default 2)
-                                
-          --disable-variant-sequence-assembly
-                                Disable assemble variant cDNA sequence from
-                                overlapping reads
-        ```
-        
-        ### Commandline options for translating cDNA to protein sequence
-        ```
-          --protein-sequence-length PROTEIN_SEQUENCE_LENGTH
-          
-          --max-reference-transcript-mismatches MAX_REFERENCE_TRANSCRIPT_MISMATCHES
-                                Maximum number of mismatches between variant sequence
-                                reference sequence before a candidate reading frame is
-                                ignored.
-                                
-          --count-mismatches-after-variant
-                                If true, mismatches after the variant locus will count
-                                toward the --max-reference-transcript-mismatches
-                                filter.
-                                
-          --min-transcript-prefix-length MIN_TRANSCRIPT_PREFIX_LENGTH
-                                Number of nucleotides before the variant we try to
-                                match against a reference transcript. Values greater
-                                than zero exclude variants near the start codon of
-                                transcripts without 5' UTRs.
-                                
-          --max-protein-sequences-per-variant MAX_PROTEIN_SEQUENCES_PER_VARIANT
-        
-        ```
-        
-        ### Commandline options for filtering 
-        
-        ```
-          --min-alt-rna-reads MIN_ALT_RNA_READS
-                                Minimum number of reads supporting variant allele
-                                (default 3)
-        
-          --min-alt-rna-fragments MIN_ALT_RNA_FRAGMENTS
-                                Minimum number of fragments supporting variant allele
-                                (default 2). Note that this option is the same as
-                                --min-alt-rna-reads for single-end sequencing.
-        
-          --min-alt-rna-fraction MIN_ALT_RNA_FRACTION
-                                Minimum ratio of fragments supporting variant allele
-                                to total RNA fragments (default 0.005).
-        
-          --min-ratio-alt-to-other-fragments MIN_RATIO_ALT_TO_OTHER_FRAGMENTS
-                                At loci where alleles other than the ref and a single
-                                alt are supported, this parameter controls how many
-                                more times fragments supporting the variant allele are
-                                required relative to other non-reference alleles
-                                (default 3.0).
-        ```
-        
-        ### Commandline options for writing an output CSV
-        
-        ```
-          --output OUTPUT       Output CSV file
-          
-          --output-columns OUTPUT_COLUMNS [OUTPUT_COLUMNS ...]
-                                Subset of columns to write
-        
-        ```
-        
-        
-        
-        ## Internal Design
-        
-        ![](isovar_design.png)
-        
-        The inputs to Isovar are one or more somatic variant call (VCF) files, along with a BAM file 
-        containing aligned tumor RNA reads. The following objects are used to aggregate information within Isovar:
-        
-        * [LocusRead](https://github.com/openvax/isovar/blob/master/isovar/locus_read.py): Isovar examines each variant locus and extracts reads overlapping that locus, 
-        represented by `LocusRead`. The `LocusRead` representation allows filtering  based
-        on quality and alignment criteria (e.g. MAPQ > 0) which are thrown away in later stages
-        of Isovar. 
-        
-        * [AlleleRead](https://github.com/openvax/isovar/blob/master/isovar/allele_read.py): Once `LocusRead` objects have been filtered, they are converted into a simplified 
-        representation called `AlleleRead`. Each `AlleleRead` contains only the cDNA sequences 
-        *before*, *at*, and *after* the variant locus. 
-        
-        * [ReadEvidence](https://github.com/openvax/isovar/blob/master/isovar/read_evidence.py): 
-        The set of `AlleleRead` objects overlapping a mutation's location may support many different
-        distinct allele. The `ReadEvidence` type represents the grouping of these reads into
-        *ref*, *alt* and *other* `AlleleRead` sets, where *ref* reads agree with the reference
-         sequence, *alt* reads agree with the given mutation, and *other* reads contain all
-         non-ref/non-alt alleles. The *alt* reads will be used later to determine
-        a mutant coding sequence, but the *ref* and *other* groups are also kept in case they are
-        useful for filtering. 
-        
-        * [VariantSequence](https://github.com/openvax/isovar/blob/master/isovar/variant_sequence.py):
-        Overlapping `AlleleRead`s containing the same mutation are assembled into a longer
-        sequence. The `VariantSequence` object represents this candidate coding sequence, as well
-        as all the `AlleleRead` objects which were used to create it.
-        
-        * [ReferenceContext](https://github.com/openvax/isovar/blob/master/isovar/reference_context.py): To determine the reading frame in which to translate a `VariantSequence`, Isovar
-        looks at all Ensembl annotated transcripts overlapping the locus and collapses them
-         into one or more `ReferenceContext` object. Each `ReferenceContext` represents the 
-         cDNA sequence upstream of the variant locus and in which of the {0, +1, +2} reading frames
-          it is translated. 
-        
-        * [Translation](https://github.com/openvax/isovar/blob/master/isovar/translation.py): Use the reading frame from a `ReferenceContext` to translate a `VariantSequence` 
-        into a protein fragment, represented by `Translation`.
-        
-        * [ProteinSequence](https://github.com/openvax/isovar/blob/master/isovar/protein_sequence.py):
-        Multiple distinct variant sequences and reference contexts can generate the same translations, so we aggregate those equivalent `Translation` objects into a `ProteinSequence`.
-        
-        * [IsovarResult](https://github.com/openvax/isovar/blob/master/isovar/isovar_result.py): Since a single variant locus might have reads which assemble into multiple incompatible coding sequences, an `IsovarResult` represents a variant and one or more `ProteinSequence` objects which are associated with it. We typically don't want to deal with *every* possible translation of *every* distinct sequence detected around a variant, so the protein sequences are sorted by their number of supporting fragments and the best protein sequence is made easy to access. The `IsovarResult` object also has many informative properties such `num_alt_fragments`, `fraction_ref_reads`, &c.  
-        
-        
-        ## Other Isovar Commandline Tools
-        
-        <dl>
-        <dt>isovar-protein-sequences --vcf variants.vcf --bam rna.bam</dt>
-        <dd>All protein sequences which can be assembled from RNA reads for any of the given variants.</dd>
-        
-        <dt>isovar-allele-counts --vcf variants.vcf --bam rna.bam</dt>
-        <dd>Counts of reads and fragments supporting the ref, alt, and other alleles at all given variant locations.</dd>
-        
-        <dt>isovar-allele-reads --vcf variants.vcf --bam rna.bam</dt>
-        <dd>Sequences of all reads overlapping any of the given variants.</dd>
-         
-        <dt>isovar-translations --vcf variants.vcf --bam rna.bam</dt>
-        <dd>All possible translations of any assembled cDNA sequence containing any of the given variants in the reference frame of any matching transcript.</dd>
-        
-        <dt>isovar-reference-contexts --vcf variants.vcf</dt>
-        <dd>Shows all candidate reference contexts (sequence and reading frame) before each variant, derived from overlapping reference coding transcripts.</dd>
-        
-        <dt>isovar-variant-reads --vcf variants.vcf --bam rna.bam</dt>
-        <dd>Like the isovar-allele-reads command but limited only to reads which support the alt allele.</dd>
-        
-        <dt>isovar-variant-sequences --vcf variants.vcf --bam rna.bam</dt>
-        <dd>Shows all assembled cDNA coding sequences supporting any of the given variants.</dd>
-        </dl>
-        
-        ## Sequencing Recommendations
-        
-        Isovar works best with high quality / high coverage mRNA sequence data. 
-        This means that you will get best results from >100M paired-end reads sequenced on an 
-        Illumina HiSeq from a library enriched with poly-A capture. The number of reads varies 
-        depending on degree of RNA degradation and tumor purity. The read length will determine 
-        the longest protein sequence you can recover, since Isovar's cDNA assembly only 
-        considers reads that overlap a variant. With 100bp reads you will be able to assemble
-        at most 199bp of sequence around a somatic single nucleotide variant, and consequently 
-        only be to determine 66 amino acids from the protein sequence. If you disable the cDNA 
-        assembly algorithm then a 100bp read will only be able to determine 33 amino acids.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<a href="https://travis-ci.org/openvax/isovar">
+    <img src="https://travis-ci.org/openvax/isovar.svg?branch=master" alt="Build Status" />
+</a>
+<a href="https://coveralls.io/github/openvax/isovar?branch=master">
+    <img src="https://coveralls.io/repos/openvax/isovar/badge.svg?branch=master&service=github" alt="Coverage Status" />
+</a>
+<a href="https://pypi.python.org/pypi/isovar/">
+    <img src="https://img.shields.io/pypi/v/isovar.svg?maxAge=1000" alt="PyPI" />
+</a>
+
+# Isovar
+
+* [Overview](#overview)
+* [Python API](#python-api)
+* [Commandline](#commandline)
+* [Internal Design](#internal-design)
+* [Other Isovar Commandline Tools](#other-isovar-commandline-tools)
+* [Sequencing Recommendations](#sequencing-recommendations)
+
+## Overview
+Isovar determines mutant protein subsequences around mutations from cancer RNAseq data.
+
+Isovar works by:
+
+ 1) collecting RNA reads which spanning the location of a variant,
+
+ 2) filtering the RNA reads to those which support the mutation,
+
+ 3) assembling mutant reads into longer coding sequences,  
+
+ 4) matching mutant coding sequences against reference annotated reading
+frames, and
+
+ 5) translating coding sequences determined directly from RNA into mutant protein sequences.
+
+The assembled coding sequences may incorporate proximal 
+(germline and somatic) variants, along with any splicing alterations 
+which occur due to modified splice signals.
+
+## Python API
+
+In the example below, `isovar.run_isovar` returns a list of `isovar.IsovarResult` objects. 
+Each of these objects corresponds to a single input variant and contains all of the information about the RNA evidence at that variant's location and any mutant protein sequences which were assembled for the variant.
+
+```python
+
+from isovar import run_isovar
+
+isovar_results = run_isovar(
+    variants="cancer-mutations.vcf",
+    alignment_file="tumor-rna.bam")
+    
+# this code traverses every variant and prints the number
+# of RNA reads which support the alt allele for variants
+# which had a successfully assembled/translated protein sequence
+for isovar_result in isovar_results:
+    # if any protein sequences were assembled from RNA
+    # then the one with most supporting reads can be
+    # accessed from a property called `top_protein_sequence`.
+    if isovar_result.top_protein_sequence is not None:
+        # print number of distinct fragments supporting the
+        # the variant allele for this mutation
+        print(isovar_result.variant, isovar_result.num_alt_fragments)
+    
+```
+
+A collection of `IsovarResult` objects can also be flattened into a Pandas DataFrame:
+
+```python
+
+from isovar import run_isovar, isovar_results_to_dataframe
+
+df =  isovar_results_to_dataframe(
+        run_isovar(
+            variants="cancer-mutations.vcf",
+            alignment_file="tumor-rna.bam"))
+```
+
+
+### Python API options for collecting RNA reads
+
+To change how Isovar collects and filters RNA reads you can create
+your own instance of the `isovar.ReadCollector` class and pass it to `run_isovar`.
+```python
+from isovar import run_isovar, ReadCollector
+
+# create a custom ReadCollector to change options for how RNA reads are processed
+read_collector = ReadCollector(
+    use_duplicate_reads=True,
+    use_secondary_alignments=True, 
+    use_soft_clipped_bases=True)
+
+isovar_results = run_isovar(
+    variants="cancer-mutations.vcf",
+    alignment_file="tumor-rna.bam",
+    read_collector=read_collector)
+
+````
+
+
+### Python API options for coding sequence assembly and translation
+
+To change how Isovar assembles RNA reads into coding sequences, determines their
+reading frames, and groups translated amino acid sequences you can create your
+own instance of the `isovar.ProteinSequenceCreator` class and pass it to `run_isovar`.
+
+
+```python
+from isovar import run_isovar, ProteinSequenceCreator
+
+# create a custom ProteinSequenceCreator to change options for how
+# protein sequences are assembled from RNA reads
+protein_sequence_creator = ProteinSequenceCreator(
+    # number of amino acids we're aiming for, coding sequences
+    # might still give us a shorter sequence due to an early stop 
+    # codon or poor coverage
+    protein_sequence_length=30,
+    # minimum number of reads covering each base of the coding sequence
+    min_variant_sequence_coverage=2,
+    # how much of a reference transcript should a coding sequence match before
+    # we use it to establish a reading frame
+    min_transcript_prefix_length=20,
+    # how many mismatches allowed between coding sequence (before the variant)
+    # and transcript (before the variant location)
+    max_transcript_mismatches=2,
+    # also count mismatches after the variant location toward
+    # max_transcript_mismatches
+    count_mismatches_after_variant=False,
+    # if more than one protein sequence can be assembled for a variant
+    # then drop any beyond this number 
+    max_protein_sequences_per_variant=1,
+    # if set to False then coding sequence will be derived from
+    # a single RNA read with the variant closest to its center
+    variant_sequence_assembly=True,
+    # how many nucleotides must two reads overlap before they are combined
+    # into a single coding sequence
+    min_assembly_overlap_size=30)
+
+isovar_results = run_isovar(
+    variants="cancer-mutations.vcf",
+    alignment_file="tumor-rna.bam",
+    protein_sequence_creator=protein_sequence_creator)
+```
+
+### Python API for filtering results
+
+You can filter a collection of `IsovarResult` objects by any of their numerical properties using the `filter_thresholds` option
+of the `run_isovar` function. The value expected for this argument is a dictionary whose keys have named like `'min_fraction_ref_reads'` or `'max_num_alt_fragments'`  and whose values are numerical thresholds.
+Everything after the `'min_'` or `'max_'` at the start of a key is expected to be the name of a property of `IsovarResult`. 
+Many of the commonly accessed properties regarding RNA read evidence follow the pattern: 
+```
+{num|fraction}_{ref|alt|other}_{reads|fragments} 
+```
+
+For example, in the following code the results are filtered to have 10 or more alt reads supporting a variant and no more than 25% of the fragments supporting an allele other than the ref or alt.
+```python
+from isovar import run_isovar
+
+isovar_results = run_isovar(
+    variants="cancer-mutations.vcf",
+    alignment_file="tumor-rna.bam",
+    filter_thresholds={"min_num_alt_reads": 10, "max_fraction_other_fragments": 0.25})    
+
+for isovar_result in isovar_results:
+    # print each variant and whether it passed both filters
+    print(isovar_result.variant, isovar_result.passes_all_filters)
+```
+
+A variant which fails one or more filters is not excluded from the result collection but it has `False` values in its corresponding 
+`filter_values` dictionary property and will have a `False` value for the `passes_all_filters` property. 
+
+If a result collection is flattened into a DataFrame then each filter is included as a column. 
+
+It's also possible to filter on boolean properties (without numerical thresholds) by passing `filter_flags` to `run_isovar`. These boolean
+properties can be further negated by prepending 'not_' to the property name, so that both `'protein_sequence_matches_predicted_effect'` and `'not_protein_sequence_matches_predicted_effect'` are valid names for `filter_flags`.
+
+## Commandline 
+
+Basic example:
+
+```sh
+$ isovar  \
+    --vcf somatic-variants.vcf  \
+    --bam rnaseq.bam \
+    --protein-sequence-length 30 \
+    --output isovar-results.csv
+```
+
+### Commandline options for loading variants
+
+###
+```
+  --vcf VCF             Genomic variants in VCF format
+  
+  --maf MAF             Genomic variants in TCGA's MAF format
+  
+  --variant CHR POS REF ALT
+                        Individual variant as 4 arguments giving chromsome,
+                        position, ref, and alt. Example: chr1 3848 C G. Use
+                        '.' to indicate empty alleles for insertions or
+                        deletions.
+  
+  --genome GENOME       What reference assembly your variant coordinates are
+                        using. Examples: 'hg19', 'GRCh38', or 'mm9'. This
+                        argument is ignored for MAF files, since each row
+                        includes the reference. For VCF files, this is used if
+                        specified, and otherwise is guessed from the header.
+                        For variants specfied on the commandline with
+                        --variant, this option is required.
+  
+  --download-reference-genome-data
+                        Automatically download genome reference data required
+                        for annotation using PyEnsembl. Otherwise you must
+                        first run 'pyensembl install' for the release/species
+                        corresponding to the genome used in your VCF.
+  
+  --json-variants JSON_VARIANTS
+                        Path to Varcode.VariantCollection object serialized as
+                        a JSON file.
+
+```
+
+### Commandline options for loading aligned tumor RNA-seq reads
+
+```
+  --bam BAM             BAM file containing RNAseq reads
+  
+  --min-mapping-quality MIN_MAPPING_QUALITY
+                        Minimum MAPQ value to allow for a read (default 1)
+  
+  --use-duplicate-reads
+                        By default, reads which have been marked as duplicates
+                        are excluded.Use this option to include duplicate
+                        reads.
+                        
+  --drop-secondary-alignments
+                        By default, secondary alignments are included in
+                        reads, use this option to instead only use primary
+                        alignments.
+```
+
+### Commandline options for coding sequence assembly
+```
+  --min-variant-sequence-coverage MIN_VARIANT_SEQUENCE_COVERAGE
+                        Minimum number of reads supporting a variant sequence
+                        (default 2)
+                        
+  --disable-variant-sequence-assembly
+                        Disable assemble variant cDNA sequence from
+                        overlapping reads
+```
+
+### Commandline options for translating cDNA to protein sequence
+```
+  --protein-sequence-length PROTEIN_SEQUENCE_LENGTH
+  
+  --max-reference-transcript-mismatches MAX_REFERENCE_TRANSCRIPT_MISMATCHES
+                        Maximum number of mismatches between variant sequence
+                        reference sequence before a candidate reading frame is
+                        ignored.
+                        
+  --count-mismatches-after-variant
+                        If true, mismatches after the variant locus will count
+                        toward the --max-reference-transcript-mismatches
+                        filter.
+                        
+  --min-transcript-prefix-length MIN_TRANSCRIPT_PREFIX_LENGTH
+                        Number of nucleotides before the variant we try to
+                        match against a reference transcript. Values greater
+                        than zero exclude variants near the start codon of
+                        transcripts without 5' UTRs.
+                        
+  --max-protein-sequences-per-variant MAX_PROTEIN_SEQUENCES_PER_VARIANT
+
+```
+
+### Commandline options for filtering 
+
+```
+  --min-alt-rna-reads MIN_ALT_RNA_READS
+                        Minimum number of reads supporting variant allele
+                        (default 3)
+
+  --min-alt-rna-fragments MIN_ALT_RNA_FRAGMENTS
+                        Minimum number of fragments supporting variant allele
+                        (default 2). Note that this option is the same as
+                        --min-alt-rna-reads for single-end sequencing.
+
+  --min-alt-rna-fraction MIN_ALT_RNA_FRACTION
+                        Minimum ratio of fragments supporting variant allele
+                        to total RNA fragments (default 0.005).
+
+  --min-ratio-alt-to-other-fragments MIN_RATIO_ALT_TO_OTHER_FRAGMENTS
+                        At loci where alleles other than the ref and a single
+                        alt are supported, this parameter controls how many
+                        more times fragments supporting the variant allele are
+                        required relative to other non-reference alleles
+                        (default 3.0).
+```
+
+### Commandline options for writing an output CSV
+
+```
+  --output OUTPUT       Output CSV file
+  
+  --output-columns OUTPUT_COLUMNS [OUTPUT_COLUMNS ...]
+                        Subset of columns to write
+
+```
+
+
+
+## Internal Design
+
+![](isovar_design.png)
+
+The inputs to Isovar are one or more somatic variant call (VCF) files, along with a BAM file 
+containing aligned tumor RNA reads. The following objects are used to aggregate information within Isovar:
+
+* [LocusRead](https://github.com/openvax/isovar/blob/master/isovar/locus_read.py): Isovar examines each variant locus and extracts reads overlapping that locus, 
+represented by `LocusRead`. The `LocusRead` representation allows filtering  based
+on quality and alignment criteria (e.g. MAPQ > 0) which are thrown away in later stages
+of Isovar. 
+
+* [AlleleRead](https://github.com/openvax/isovar/blob/master/isovar/allele_read.py): Once `LocusRead` objects have been filtered, they are converted into a simplified 
+representation called `AlleleRead`. Each `AlleleRead` contains only the cDNA sequences 
+*before*, *at*, and *after* the variant locus. 
+
+* [ReadEvidence](https://github.com/openvax/isovar/blob/master/isovar/read_evidence.py): 
+The set of `AlleleRead` objects overlapping a mutation's location may support many different
+distinct allele. The `ReadEvidence` type represents the grouping of these reads into
+*ref*, *alt* and *other* `AlleleRead` sets, where *ref* reads agree with the reference
+ sequence, *alt* reads agree with the given mutation, and *other* reads contain all
+ non-ref/non-alt alleles. The *alt* reads will be used later to determine
+a mutant coding sequence, but the *ref* and *other* groups are also kept in case they are
+useful for filtering. 
+
+* [VariantSequence](https://github.com/openvax/isovar/blob/master/isovar/variant_sequence.py):
+Overlapping `AlleleRead`s containing the same mutation are assembled into a longer
+sequence. The `VariantSequence` object represents this candidate coding sequence, as well
+as all the `AlleleRead` objects which were used to create it.
+
+* [ReferenceContext](https://github.com/openvax/isovar/blob/master/isovar/reference_context.py): To determine the reading frame in which to translate a `VariantSequence`, Isovar
+looks at all Ensembl annotated transcripts overlapping the locus and collapses them
+ into one or more `ReferenceContext` object. Each `ReferenceContext` represents the 
+ cDNA sequence upstream of the variant locus and in which of the {0, +1, +2} reading frames
+  it is translated. 
+
+* [Translation](https://github.com/openvax/isovar/blob/master/isovar/translation.py): Use the reading frame from a `ReferenceContext` to translate a `VariantSequence` 
+into a protein fragment, represented by `Translation`.
+
+* [ProteinSequence](https://github.com/openvax/isovar/blob/master/isovar/protein_sequence.py):
+Multiple distinct variant sequences and reference contexts can generate the same translations, so we aggregate those equivalent `Translation` objects into a `ProteinSequence`.
+
+* [IsovarResult](https://github.com/openvax/isovar/blob/master/isovar/isovar_result.py): Since a single variant locus might have reads which assemble into multiple incompatible coding sequences, an `IsovarResult` represents a variant and one or more `ProteinSequence` objects which are associated with it. We typically don't want to deal with *every* possible translation of *every* distinct sequence detected around a variant, so the protein sequences are sorted by their number of supporting fragments and the best protein sequence is made easy to access. The `IsovarResult` object also has many informative properties such `num_alt_fragments`, `fraction_ref_reads`, &c.  
+
+
+## Other Isovar Commandline Tools
+
+<dl>
+<dt>isovar-protein-sequences --vcf variants.vcf --bam rna.bam</dt>
+<dd>All protein sequences which can be assembled from RNA reads for any of the given variants.</dd>
+
+<dt>isovar-allele-counts --vcf variants.vcf --bam rna.bam</dt>
+<dd>Counts of reads and fragments supporting the ref, alt, and other alleles at all given variant locations.</dd>
+
+<dt>isovar-allele-reads --vcf variants.vcf --bam rna.bam</dt>
+<dd>Sequences of all reads overlapping any of the given variants.</dd>
+ 
+<dt>isovar-translations --vcf variants.vcf --bam rna.bam</dt>
+<dd>All possible translations of any assembled cDNA sequence containing any of the given variants in the reference frame of any matching transcript.</dd>
+
+<dt>isovar-reference-contexts --vcf variants.vcf</dt>
+<dd>Shows all candidate reference contexts (sequence and reading frame) before each variant, derived from overlapping reference coding transcripts.</dd>
+
+<dt>isovar-variant-reads --vcf variants.vcf --bam rna.bam</dt>
+<dd>Like the isovar-allele-reads command but limited only to reads which support the alt allele.</dd>
+
+<dt>isovar-variant-sequences --vcf variants.vcf --bam rna.bam</dt>
+<dd>Shows all assembled cDNA coding sequences supporting any of the given variants.</dd>
+</dl>
+
+## Sequencing Recommendations
+
+Isovar works best with high quality / high coverage mRNA sequence data. 
+This means that you will get best results from >100M paired-end reads sequenced on an 
+Illumina HiSeq from a library enriched with poly-A capture. The number of reads varies 
+depending on degree of RNA degradation and tumor purity. The read length will determine 
+the longest protein sequence you can recover, since Isovar's cDNA assembly only 
+considers reads that overlap a variant. With 100bp reads you will be able to assemble
+at most 199bp of sequence around a somatic single nucleotide variant, and consequently 
+only be to determine 66 amino acids from the protein sequence. If you disable the cDNA 
+assembly algorithm then a 100bp read will only be able to determine 33 amino acids.
```

#### html2text {}

```diff
@@ -1,15 +1,20 @@
-Metadata-Version: 2.1 Name: isovar Version: 1.1.1 Summary: Determine mutant
+Metadata-Version: 2.1 Name: isovar Version: 1.3.0 Summary: Determine mutant
 protein sequences from RN using assembly around variants Home-page: https://
 github.com/openvax/isovar Author: Alex Rubinsteyn, Arman Aksoy, Julia Kodysh
 Author-email: alex.rubinsteyn@mssm.edu License: http://www.apache.org/licenses/
-LICENSE-2.0.html Description: [Build_Status] [Coverage_Status] [PyPI] # Isovar
-* [Overview](#overview) * [Python API](#python-api) * [Commandline]
-(#commandline) * [Internal Design](#internal-design) * [Other Isovar
-Commandline Tools](#other-isovar-commandline-tools) * [Sequencing
+LICENSE-2.0.html Classifier: Development Status :: 4 - Beta Classifier:
+Environment :: Console Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
+Approved :: Apache Software License Classifier: Programming Language :: Python
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics Description-
+Content-Type: text/markdown License-File: LICENSE [Build_Status] [Coverage
+Status] [PyPI] # Isovar * [Overview](#overview) * [Python API](#python-api) *
+[Commandline](#commandline) * [Internal Design](#internal-design) * [Other
+Isovar Commandline Tools](#other-isovar-commandline-tools) * [Sequencing
 Recommendations](#sequencing-recommendations) ## Overview Isovar determines
 mutant protein subsequences around mutations from cancer RNAseq data. Isovar
 works by: 1) collecting RNA reads which spanning the location of a variant, 2)
 filtering the RNA reads to those which support the mutation, 3) assembling
 mutant reads into longer coding sequences, 4) matching mutant coding sequences
 against reference annotated reading frames, and 5) translating coding sequences
 determined directly from RNA into mutant protein sequences. The assembled
@@ -214,13 +219,8 @@
 with poly-A capture. The number of reads varies depending on degree of RNA
 degradation and tumor purity. The read length will determine the longest
 protein sequence you can recover, since Isovar's cDNA assembly only considers
 reads that overlap a variant. With 100bp reads you will be able to assemble at
 most 199bp of sequence around a somatic single nucleotide variant, and
 consequently only be to determine 66 amino acids from the protein sequence. If
 you disable the cDNA assembly algorithm then a 100bp read will only be able to
-determine 33 amino acids. Platform: UNKNOWN Classifier: Development Status :: 4
-- Beta Classifier: Environment :: Console Classifier: Operating System :: OS
-Independent Classifier: Intended Audience :: Science/Research Classifier:
-License :: OSI Approved :: Apache Software License Classifier: Programming
-Language :: Python Classifier: Topic :: Scientific/Engineering :: Bio-
-Informatics Description-Content-Type: text/markdown
+determine 33 amino acids.
```

### Comparing `isovar-1.1.1/isovar.egg-info/SOURCES.txt` & `isovar-1.3.0/isovar.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 isovar/__init__.py
 isovar/alignment_score.py
 isovar/allele_read.py
 isovar/allele_read_helpers.py
 isovar/assembly.py
```

### Comparing `isovar-1.1.1/test/test_value_object.py` & `isovar-1.3.0/test/test_value_object.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/test/test_mutant_amino_acids_in_protein_sequence.py` & `isovar-1.3.0/test/test_mutant_amino_acids_in_protein_sequence.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/test/testing_helpers.py` & `isovar-1.3.0/test/testing_helpers.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/test/test_alignment_score.py` & `isovar-1.3.0/test/test_alignment_score.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/test/test_somatic_variant_with_0_supporting_rna_reads.py` & `isovar-1.3.0/test/test_somatic_variant_with_0_supporting_rna_reads.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/test/test_translation.py` & `isovar-1.3.0/test/test_translation.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/test/test_somatic_variant_with_2_supporting_rna_reads.py` & `isovar-1.3.0/test/test_somatic_variant_with_2_supporting_rna_reads.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/test/test_dataframe_builder.py` & `isovar-1.3.0/test/test_dataframe_builder.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/test/test_filtering.py` & `isovar-1.3.0/test/test_filtering.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/test/test_variant_orf.py` & `isovar-1.3.0/test/test_variant_orf.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/test/test_common.py` & `isovar-1.3.0/test/test_common.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/test/test_reference_sequence_key.py` & `isovar-1.3.0/test/test_reference_sequence_key.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/test/test_assembly.py` & `isovar-1.3.0/test/test_assembly.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/test/test_isovar_result.py` & `isovar-1.3.0/test/test_isovar_result.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/test/test_argparser_helpers.py` & `isovar-1.3.0/test/test_argparser_helpers.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/test/test_reference_contexts.py` & `isovar-1.3.0/test/test_reference_contexts.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/test/test_cli.py` & `isovar-1.3.0/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/test/test_locus_reads.py` & `isovar-1.3.0/test/test_locus_reads.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/test/test_genetic_code.py` & `isovar-1.3.0/test/test_genetic_code.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/test/test_protein_sequences.py` & `isovar-1.3.0/test/test_protein_sequences.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/test/test_read_helpers.py` & `isovar-1.3.0/test/test_read_helpers.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/test/test_main.py` & `isovar-1.3.0/test/test_main.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/test/test_variant_helpers.py` & `isovar-1.3.0/test/test_variant_helpers.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/test/test_reference_coding_sequence_key.py` & `isovar-1.3.0/test/test_reference_coding_sequence_key.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/test/test_gather_variant_reads_wgs.py` & `isovar-1.3.0/test/test_gather_variant_reads_wgs.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/test/test_allele_counts.py` & `isovar-1.3.0/test/test_allele_counts.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/test/test_variant_reads_with_dummy_samfile.py` & `isovar-1.3.0/test/test_variant_reads_with_dummy_samfile.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/test/test_variant_sequences.py` & `isovar-1.3.0/test/test_variant_sequences.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/test/test_effect_prediction.py` & `isovar-1.3.0/test/test_effect_prediction.py`

 * *Files identical despite different names*

### Comparing `isovar-1.1.1/setup.py` & `isovar-1.3.0/setup.py`

 * *Files identical despite different names*

