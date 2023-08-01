# Comparing `tmp/ExpoSeq-2.0.2.tar.gz` & `tmp/ExpoSeq-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExpoSeq-2.0.2.tar", last modified: Sat Jul 29 09:26:41 2023, max compression
+gzip compressed data, was "ExpoSeq-2.0.3.tar", last modified: Tue Aug  1 10:18:33 2023, max compression
```

## Comparing `ExpoSeq-2.0.2.tar` & `ExpoSeq-2.0.3.tar`

### file list

```diff
@@ -1,90 +1,92 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 09:26:41.775496 ExpoSeq-2.0.2/
--rw-rw-rw-   0        0        0    11543 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/LICENSE
--rw-rw-rw-   0        0        0       59 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     7611 2023-07-29 09:26:41.774562 ExpoSeq-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     7230 2023-07-22 09:38:55.000000 ExpoSeq-2.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-29 09:26:41.775496 ExpoSeq-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1335 2023-07-29 09:26:17.000000 ExpoSeq-2.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 09:26:41.217673 ExpoSeq-2.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-29 09:26:41.267675 ExpoSeq-2.0.2/src/ExpoSeq/
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 09:26:41.367945 ExpoSeq-2.0.2/src/ExpoSeq/augment_data/
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/augment_data/__init__.py
--rw-rw-rw-   0        0        0     1357 2023-07-29 09:01:16.000000 ExpoSeq-2.0.2/src/ExpoSeq/augment_data/binding_data.py
--rw-rw-rw-   0        0        0      858 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/augment_data/check_reports.py
--rw-rw-rw-   0        0        0      913 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/augment_data/load_data.py
--rw-rw-rw-   0        0        0     4616 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/augment_data/loop_collect_reports.py
--rw-rw-rw-   0        0        0    10625 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/augment_data/mixcr_nils.py
--rw-rw-rw-   0        0        0     6813 2023-07-16 09:18:38.000000 ExpoSeq-2.0.2/src/ExpoSeq/augment_data/randomizer.py
--rw-rw-rw-   0        0        0      580 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/augment_data/read_raw_data.py
--rw-rw-rw-   0        0        0     3646 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/augment_data/structure_files.py
--rw-rw-rw-   0        0        0      519 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/augment_data/trimming.py
--rw-rw-rw-   0        0        0    21027 2023-07-29 07:17:35.000000 ExpoSeq-2.0.2/src/ExpoSeq/augment_data/uploader.py
--rw-rw-rw-   0        0        0    10290 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/full_pipe.py
--rw-rw-rw-   0        0        0    41988 2023-07-29 09:12:18.000000 ExpoSeq-2.0.2/src/ExpoSeq/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-07-29 09:26:41.563519 ExpoSeq-2.0.2/src/ExpoSeq/plots/
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/plots/__init__.py
--rw-rw-rw-   0        0        0     2061 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/plots/barplot.py
--rw-rw-rw-   0        0        0     1666 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/plots/cluster_embedding.py
--rw-rw-rw-   0        0        0     4363 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/plots/embedding_with_binding.py
--rw-rw-rw-   0        0        0     3292 2023-07-16 08:59:57.000000 ExpoSeq-2.0.2/src/ExpoSeq/plots/length_distribution.py
--rw-rw-rw-   0        0        0     7812 2023-07-29 09:06:08.000000 ExpoSeq-2.0.2/src/ExpoSeq/plots/levenshtein_clustering.py
--rw-rw-rw-   0        0        0     4641 2023-07-29 09:26:08.000000 ExpoSeq-2.0.2/src/ExpoSeq/plots/logo_plot.py
--rw-rw-rw-   0        0        0     3382 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/plots/plt_heatmap.py
--rw-rw-rw-   0        0        0     2524 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/plots/protvec.py
--rw-rw-rw-   0        0        0     1470 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/plots/relative_sequence_abundance.py
--rw-rw-rw-   0        0        0     1724 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/plots/saveFig.py
--rw-rw-rw-   0        0        0     1171 2023-07-29 08:02:14.000000 ExpoSeq-2.0.2/src/ExpoSeq/plots/stacked_aa_distribution.py
--rw-rw-rw-   0        0        0     2540 2023-07-16 09:10:35.000000 ExpoSeq-2.0.2/src/ExpoSeq/plots/usq_plot.py
--rw-rw-rw-   0        0        0     3019 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/reset.py
--rw-rw-rw-   0        0        0      288 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/run.py
-drwxrwxrwx   0        0        0        0 2023-07-29 09:26:41.588216 ExpoSeq-2.0.2/src/ExpoSeq/settings/
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/settings/__init__.py
--rw-rw-rw-   0        0        0     2086 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/settings/blosum_62.txt
--rw-rw-rw-   0        0        0     1883 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/settings/change_save_settings.py
--rw-rw-rw-   0        0        0       94 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/settings/colorbar.txt
--rw-rw-rw-   0        0        0       86 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/settings/font_settings.txt
--rw-rw-rw-   0        0        0       57 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/settings/global_vars.txt
--rw-rw-rw-   0        0        0      173 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/settings/legend_settings.txt
--rw-rw-rw-   0        0        0     8133 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/settings/plot_styler.py
--rw-rw-rw-   0        0        0       42 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/settings/save_settings.txt
-drwxrwxrwx   0        0        0        0 2023-07-29 09:26:41.594219 ExpoSeq-2.0.2/src/ExpoSeq/test_data/
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/test_data/__init__.py
--rw-rw-rw-   0        0        0    20748 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/test_data/all_alignment_reports.pickle
-drwxrwxrwx   0        0        0        0 2023-07-29 09:26:41.640618 ExpoSeq-2.0.2/src/ExpoSeq/test_data/test_files/
--rw-rw-rw-   0        0        0     3578 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/test_data/test_files/Chris_main_df.csv
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/test_data/test_files/__init__.py
--rw-rw-rw-   0        0        0    11375 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/test_data/test_files/binding_data.csv
--rw-rw-rw-   0        0        0      566 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/test_data/test_files/experiment_names.pickle
--rw-rw-rw-   0        0        0 17354490 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/test_data/test_files/sequencing_report.csv
--rw-rw-rw-   0        0        0    88335 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/test_data/test_files/test1.fastq
--rw-rw-rw-   0        0        0   213105 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/test_data/test_files/test2.fastq
--rw-rw-rw-   0        0        0    95440 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/test_data/test_files/test3.fastq
--rw-rw-rw-   0        0        0     2632 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/test_uploader.py
-drwxrwxrwx   0        0        0        0 2023-07-29 09:26:41.740570 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/__init__.py
--rw-rw-rw-   0        0        0     2176 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/aminoacid_distribution.py
--rw-rw-rw-   0        0        0     2228 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/barplot.py
--rw-rw-rw-   0        0        0     1142 2023-07-29 07:45:22.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/clustering.py
-drwxrwxrwx   0        0        0        0 2023-07-29 09:26:41.769477 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/heatmaps/
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/heatmaps/__init__.py
--rw-rw-rw-   0        0        0     1509 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py
--rw-rw-rw-   0        0        0     1818 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py
--rw-rw-rw-   0        0        0     1673 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py
--rw-rw-rw-   0        0        0     5139 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py
--rw-rw-rw-   0        0        0     1597 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py
--rw-rw-rw-   0        0        0      678 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/interpret_data.py
--rw-rw-rw-   0        0        0     3907 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/read_extract_data.py
--rw-rw-rw-   0        0        0      440 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/tidy_USQ_plot_.py
--rw-rw-rw-   0        0        0     1217 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/tidy_alignment_reports.py
--rw-rw-rw-   0        0        0     1461 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py
--rw-rw-rw-   0        0        0      391 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/tidy_library.py
--rw-rw-rw-   0        0        0     1992 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py
--rw-rw-rw-   0        0        0     1599 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py
--rw-rw-rw-   0        0        0     1299 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py
-drwxrwxrwx   0        0        0        0 2023-07-29 09:26:41.279684 ExpoSeq-2.0.2/src/ExpoSeq.egg-info/
--rw-rw-rw-   0        0        0     7611 2023-07-29 09:26:41.000000 ExpoSeq-2.0.2/src/ExpoSeq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2934 2023-07-29 09:26:41.000000 ExpoSeq-2.0.2/src/ExpoSeq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 09:26:41.000000 ExpoSeq-2.0.2/src/ExpoSeq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      188 2023-07-29 09:26:41.000000 ExpoSeq-2.0.2/src/ExpoSeq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-29 09:26:41.000000 ExpoSeq-2.0.2/src/ExpoSeq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 10:18:33.455007 ExpoSeq-2.0.3/
+-rw-rw-rw-   0        0        0    11543 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/LICENSE
+-rw-rw-rw-   0        0        0       59 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     7611 2023-08-01 10:18:33.455007 ExpoSeq-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7230 2023-07-22 09:38:55.000000 ExpoSeq-2.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 10:18:33.455007 ExpoSeq-2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1335 2023-08-01 10:18:10.000000 ExpoSeq-2.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 10:18:31.591985 ExpoSeq-2.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-08-01 10:18:31.746842 ExpoSeq-2.0.3/src/ExpoSeq/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 10:18:32.153311 ExpoSeq-2.0.3/src/ExpoSeq/augment_data/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/augment_data/__init__.py
+-rw-rw-rw-   0        0        0     1357 2023-07-29 09:01:16.000000 ExpoSeq-2.0.3/src/ExpoSeq/augment_data/binding_data.py
+-rw-rw-rw-   0        0        0      858 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/augment_data/check_reports.py
+-rw-rw-rw-   0        0        0      913 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/augment_data/load_data.py
+-rw-rw-rw-   0        0        0     4616 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/augment_data/loop_collect_reports.py
+-rw-rw-rw-   0        0        0    10625 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/augment_data/mixcr_nils.py
+-rw-rw-rw-   0        0        0     6813 2023-07-16 09:18:38.000000 ExpoSeq-2.0.3/src/ExpoSeq/augment_data/randomizer.py
+-rw-rw-rw-   0        0        0      580 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/augment_data/read_raw_data.py
+-rw-rw-rw-   0        0        0     3646 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/augment_data/structure_files.py
+-rw-rw-rw-   0        0        0      519 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/augment_data/trimming.py
+-rw-rw-rw-   0        0        0    21063 2023-08-01 08:47:50.000000 ExpoSeq-2.0.3/src/ExpoSeq/augment_data/uploader.py
+-rw-rw-rw-   0        0        0    10290 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/full_pipe.py
+-rw-rw-rw-   0        0        0    45632 2023-08-01 10:17:43.000000 ExpoSeq-2.0.3/src/ExpoSeq/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-08-01 10:18:32.277256 ExpoSeq-2.0.3/src/ExpoSeq/plots/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/plots/__init__.py
+-rw-rw-rw-   0        0        0     2061 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/plots/barplot.py
+-rw-rw-rw-   0        0        0     1666 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/plots/cluster_embedding.py
+-rw-rw-rw-   0        0        0     4363 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/plots/embedding_with_binding.py
+-rw-rw-rw-   0        0        0     5815 2023-07-30 16:37:34.000000 ExpoSeq-2.0.3/src/ExpoSeq/plots/hist_lvst_dist.py
+-rw-rw-rw-   0        0        0     3292 2023-07-30 09:23:50.000000 ExpoSeq-2.0.3/src/ExpoSeq/plots/length_distribution.py
+-rw-rw-rw-   0        0        0     7812 2023-07-29 09:06:08.000000 ExpoSeq-2.0.3/src/ExpoSeq/plots/levenshtein_clustering.py
+-rw-rw-rw-   0        0        0     4641 2023-07-29 09:26:08.000000 ExpoSeq-2.0.3/src/ExpoSeq/plots/logo_plot.py
+-rw-rw-rw-   0        0        0     3382 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/plots/plt_heatmap.py
+-rw-rw-rw-   0        0        0     2524 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/plots/protvec.py
+-rw-rw-rw-   0        0        0     1470 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/plots/relative_sequence_abundance.py
+-rw-rw-rw-   0        0        0     1724 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/plots/saveFig.py
+-rw-rw-rw-   0        0        0     1910 2023-07-30 09:44:33.000000 ExpoSeq-2.0.3/src/ExpoSeq/plots/stacked_aa_distribution.py
+-rw-rw-rw-   0        0        0     2540 2023-07-16 09:10:35.000000 ExpoSeq-2.0.3/src/ExpoSeq/plots/usq_plot.py
+-rw-rw-rw-   0        0        0     3019 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/reset.py
+-rw-rw-rw-   0        0        0      288 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/run.py
+drwxrwxrwx   0        0        0        0 2023-08-01 10:18:32.310262 ExpoSeq-2.0.3/src/ExpoSeq/settings/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/settings/__init__.py
+-rw-rw-rw-   0        0        0     2086 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/settings/blosum_62.txt
+-rw-rw-rw-   0        0        0     1883 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/settings/change_save_settings.py
+-rw-rw-rw-   0        0        0       94 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/settings/colorbar.txt
+-rw-rw-rw-   0        0        0       86 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/settings/font_settings.txt
+-rw-rw-rw-   0        0        0       57 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/settings/global_vars.txt
+-rw-rw-rw-   0        0        0      173 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/settings/legend_settings.txt
+-rw-rw-rw-   0        0        0     8133 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/settings/plot_styler.py
+-rw-rw-rw-   0        0        0       42 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/settings/save_settings.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 10:18:32.318536 ExpoSeq-2.0.3/src/ExpoSeq/test_data/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/test_data/__init__.py
+-rw-rw-rw-   0        0        0    20748 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/test_data/all_alignment_reports.pickle
+drwxrwxrwx   0        0        0        0 2023-08-01 10:18:32.394154 ExpoSeq-2.0.3/src/ExpoSeq/test_data/test_files/
+-rw-rw-rw-   0        0        0     3578 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/test_data/test_files/Chris_main_df.csv
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/test_data/test_files/__init__.py
+-rw-rw-rw-   0        0        0    11375 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/test_data/test_files/binding_data.csv
+-rw-rw-rw-   0        0        0      566 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/test_data/test_files/experiment_names.pickle
+-rw-rw-rw-   0        0        0 17354490 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/test_data/test_files/sequencing_report.csv
+-rw-rw-rw-   0        0        0    88335 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/test_data/test_files/test1.fastq
+-rw-rw-rw-   0        0        0   213105 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/test_data/test_files/test2.fastq
+-rw-rw-rw-   0        0        0    95440 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/test_data/test_files/test3.fastq
+-rw-rw-rw-   0        0        0     2632 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/test_uploader.py
+drwxrwxrwx   0        0        0        0 2023-08-01 10:18:33.067185 ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/__init__.py
+-rw-rw-rw-   0        0        0     2176 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/aminoacid_distribution.py
+-rw-rw-rw-   0        0        0     2228 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/barplot.py
+-rw-rw-rw-   0        0        0     1142 2023-07-29 07:45:22.000000 ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/clustering.py
+drwxrwxrwx   0        0        0        0 2023-08-01 10:18:33.390234 ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/heatmaps/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/heatmaps/__init__.py
+-rw-rw-rw-   0        0        0     1509 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py
+-rw-rw-rw-   0        0        0     1818 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py
+-rw-rw-rw-   0        0        0     1673 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py
+-rw-rw-rw-   0        0        0     5139 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py
+-rw-rw-rw-   0        0        0     1597 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py
+-rw-rw-rw-   0        0        0      678 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/interpret_data.py
+-rw-rw-rw-   0        0        0     3907 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/read_extract_data.py
+-rw-rw-rw-   0        0        0      440 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/tidy_USQ_plot_.py
+-rw-rw-rw-   0        0        0     1217 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/tidy_alignment_reports.py
+-rw-rw-rw-   0        0        0     1461 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py
+-rw-rw-rw-   0        0        0      947 2023-07-30 11:05:37.000000 ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/tidy_hist_lvst_dist.py
+-rw-rw-rw-   0        0        0      391 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/tidy_library.py
+-rw-rw-rw-   0        0        0     1992 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py
+-rw-rw-rw-   0        0        0     1599 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py
+-rw-rw-rw-   0        0        0     1299 2023-07-15 16:28:47.000000 ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py
+drwxrwxrwx   0        0        0        0 2023-08-01 10:18:31.762824 ExpoSeq-2.0.3/src/ExpoSeq.egg-info/
+-rw-rw-rw-   0        0        0     7611 2023-08-01 10:18:31.000000 ExpoSeq-2.0.3/src/ExpoSeq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3015 2023-08-01 10:18:31.000000 ExpoSeq-2.0.3/src/ExpoSeq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 10:18:31.000000 ExpoSeq-2.0.3/src/ExpoSeq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      188 2023-08-01 10:18:31.000000 ExpoSeq-2.0.3/src/ExpoSeq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-01 10:18:31.000000 ExpoSeq-2.0.3/src/ExpoSeq.egg-info/top_level.txt
```

### Comparing `ExpoSeq-2.0.2/LICENSE` & `ExpoSeq-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/PKG-INFO` & `ExpoSeq-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ExpoSeq
-Version: 2.0.2
+Version: 2.0.3
 Summary: A pacakge which provides various ways to analyze NGS data from phage display campaigns
 Home-page: https://github.com/nilshof01/ExpoSeq
 Author: Nils Hofmann
 Author-email: n.hofmann.99@web.de
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `ExpoSeq-2.0.2/README.md` & `ExpoSeq-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/setup.py` & `ExpoSeq-2.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name = "ExpoSeq",
-    version = "2.0.2",
+    version = "2.0.3",
     description = "A pacakge which provides various ways to analyze NGS data from phage display campaigns",
     long_description=long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/nilshof01/ExpoSeq",
     author = "Nils Hofmann",
     author_email = "n.hofmann.99@web.de",
     license = "Apache License 2.0",
```

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/augment_data/binding_data.py` & `ExpoSeq-2.0.3/src/ExpoSeq/augment_data/binding_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/augment_data/check_reports.py` & `ExpoSeq-2.0.3/src/ExpoSeq/augment_data/check_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/augment_data/load_data.py` & `ExpoSeq-2.0.3/src/ExpoSeq/augment_data/load_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/augment_data/loop_collect_reports.py` & `ExpoSeq-2.0.3/src/ExpoSeq/augment_data/loop_collect_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/augment_data/mixcr_nils.py` & `ExpoSeq-2.0.3/src/ExpoSeq/augment_data/mixcr_nils.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/augment_data/randomizer.py` & `ExpoSeq-2.0.3/src/ExpoSeq/augment_data/randomizer.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/augment_data/read_raw_data.py` & `ExpoSeq-2.0.3/src/ExpoSeq/augment_data/read_raw_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/augment_data/structure_files.py` & `ExpoSeq-2.0.3/src/ExpoSeq/augment_data/structure_files.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/augment_data/trimming.py` & `ExpoSeq-2.0.3/src/ExpoSeq/augment_data/trimming.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/augment_data/uploader.py` & `ExpoSeq-2.0.3/src/ExpoSeq/augment_data/uploader.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,14 +268,15 @@
                 subdirectory = find_file_in_subdirectories(os.path.join(module_dir, "my_experiments"), "sequencing_report.csv")
                 if subdirectory is not None:
                     repo_path = subdirectory
                     dirpath = os.path.dirname(subdirectory)
                     last_experiment = os.path.basename(dirpath)
                 else:
                     print("The experiments in my experiment do not contain the sequencing report. You need to upload a new experiment.")
+                    repo_path = ""
             
         else:
             repo_path = os.path.join(module_dir,
                                    "my_experiments",
                                     last_experiment,
                                     "sequencing_report.csv")
     else:
```

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/full_pipe.py` & `ExpoSeq-2.0.3/src/ExpoSeq/full_pipe.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/pipeline.py` & `ExpoSeq-2.0.3/src/ExpoSeq/pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 from .plots.length_distribution import length_distribution_single, length_distribution_multi
 from .plots.levenshtein_clustering import clusterSeq, cluster_single_AG
 from .plots.embedding_with_binding import cluster_toxins_tsne
 from .plots.relative_sequence_abundance import relative_sequence_abundance
 from .plots.cluster_embedding import show_difference
 from .plots.stacked_aa_distribution import stacked_aa_distr
 from .plots.barplot import barplot
+from .plots.hist_lvst_dist import levenshtein_dend, dendo_binding
 from .plots.saveFig import saveFig
 import matplotlib.pyplot as plt
 from .augment_data.binding_data import collect_binding_data
 from .augment_data.uploader import upload
 from ast import literal_eval
 from .settings.plot_styler import PlotStyle
 import pandas as pd
 import pickle
 import pkg_resources
 import os
 from ExpoSeq.settings.change_save_settings import Change_save_settings
 from ExpoSeq.augment_data.randomizer import create_sequencing_report, create_binding_report
+
 from ExpoSeq.reset import original_settings
 import shutil
 
 class PlotManager:
     def __init__(self, test_version = False, test_exp_num = 3, test_panrou_num = 1):
         self.is_test = test_version
         self.module_dir = os.path.abspath("")
@@ -247,15 +249,15 @@
                          self.font_settings,
                          self.legend_settings)
         self.plot_type = "single"
         self.ax = self.fig.gca()
         self.style = PlotStyle(self.ax, self.plot_type)
         figManager = plt.get_current_fig_manager()
         figManager.window.showMaximized()
-    def usqPlot(self, samples):
+    def rarefraction_curves(self, samples):
         """
         :param samples: you insert a list which contains the sample names
         :return: USQ stands for unique sequences quality and the plot shows you the depth of unique sequences which can be used for evaluating your sequencing quality.
         """
         if not plt.fignum_exists(1):
             self.fig = plt.figure(1)
             print("Please do not close the window for the figure while the plot is loading")
@@ -551,15 +553,15 @@
         self.ax = self.fig.gca()
         self.style = PlotStyle(self.ax, self.plot_type)
         figManager = plt.get_current_fig_manager()
         figManager.window.showMaximized()
         save_embedding = input("Do you want to save the corresponding data as csv? (Y/n)?")
         if save_embedding.lower() in ["Y", "y"]:
             name_csv = input("How do you want to call the file")
-            path_save_embedding = os.path.join(save_embedding, name_csv + ".csv" )
+            path_save_embedding = os.path.join(name_csv + ".csv")
             tsne_results.to_csv(path_save_embedding, index=False)
 
     def embedding_tsne(self,
                        samples,
                        strands = True,
                        pca_components = 80,
                        perplexity = 30,
@@ -714,19 +716,77 @@
         self.ax = self.fig.gca()
         self.style = PlotStyle(self.ax, self.plot_type)
         figManager = plt.get_current_fig_manager()
         figManager.window.showMaximized()
         
 
 
+    def levenshtein_demdogram(self,sample, max_cluster_dist = 2, batch_size = 1000):
+        """
+        :params sample: the sample you would like to analyze
+        :max_cluster_dist: Default is 2. Maximum levenshtein distance between sequences within a cluster.
+        :params batch_size: Default is 1000. The size of the sample which is chosen. 
+        """
+        if not plt.fignum_exists(1):
+            self.fig = plt.figure(1)
+            print("Please do not close the window for the figure while the plot is loading")
+            
+        self.fig.clear()
+        self.ax = self.fig.gca()
+        levenshtein_dend(self.ax,
+                         self.sequencing_report,
+                         sample,
+                         batch_size,
+                         max_cluster_dist, 
+                         self.font_settings,
+                         )
+        self.plot_type = "single"
+        self.ax = self.fig.gca()
+        self.style = PlotStyle(self.ax, self.plot_type)
+        figManager = plt.get_current_fig_manager()
 
-
-
-
-
+        figManager.window.showMaximized()
+        
+        
+    def levenshtein_binding_dendogram(self,sample, antigens, batch_size = 1000, max_cluster_dist = 2, scale_factor_lines = 1.0):
+        """
+        :param sample: the sample you would like to analyze
+        :params antigens: the antigens you would like to analyze. input format is a list and you find the names in the binding_data
+        :params batch_size: Default is 1000. The size of the sample which is chosen. 
+        :max_cluster_dist: Default is 2. Maximum levenshtein distance between sequences within a cluster.
+        :scale_factor_lines: Default is 1.5. You can change the scale factor of the lines in the dendogram which indicates the value of your binding data. if you increase the scale factor high values become very clear.
+        """
+        assert sample in self.experiments_list, "The provided sample name is not in your sequencing report. Please check the spelling or use the print_samples function to see the names of your samples"
+        assert type(sample) == str, "You have to give a string as input for the sample"
+        assert type(antigens) == list, "You have to give a list with the antigens you want to analyze"
+        assert type(batch_size) == int, "You have to give an integer as input for the batch size"
+        assert type(max_cluster_dist) == int, "You have to give an integer as input for the maximum levenshtein distance"
+        assert type(scale_factor_lines) == float, "You have to give a float as input for the scale factor of the lines"
+        assert self.binding_data is not None, "You have not given binding data. You can add it with the add_binding_data function"
+        if not plt.fignum_exists(1):
+            self.fig = plt.figure(1)
+            print("Please do not close the window for the figure while the plot is loading")
+            
+        self.fig.clear()
+        self.ax = self.fig.gca()
+        dendo_binding(self.ax,
+                    self.sequencing_report,
+                    self.binding_data,
+                    sample,
+                    antigens,
+                    batch_size,
+                    max_cluster_dist,
+                    scale_factor_lines,
+                    self.font_settings)
+        self.plot_type = "single"
+        self.ax = self.fig.gca()
+        self.style = PlotStyle(self.ax, self.plot_type)
+        figManager = plt.get_current_fig_manager()
+        figManager.window.showMaximized()
+        plt.tight_layout()
```

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/plots/barplot.py` & `ExpoSeq-2.0.3/src/ExpoSeq/plots/barplot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/plots/cluster_embedding.py` & `ExpoSeq-2.0.3/src/ExpoSeq/plots/cluster_embedding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/plots/embedding_with_binding.py` & `ExpoSeq-2.0.3/src/ExpoSeq/plots/embedding_with_binding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/plots/length_distribution.py` & `ExpoSeq-2.0.3/src/ExpoSeq/plots/length_distribution.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     batch = sequencing_report[sequencing_report["Experiment"] == sample]
     length = batch["aaSeqCDR3"].str.len()
     unique_length, counts_length = np.unique(np.array(length)
                                                 , return_counts = True)
     ax.bar(unique_length, counts_length)  # Or whatever you want in the subplot
     #ax.set_xticks(range(0, max_length + 1, 1), range(0, max_length + 1, 1))
     ax.title.set_text(sample)
-    ax.title.set_size(10)
+    ax.title.set_size(18)
     ax.set_ylabel("Read Count",
                     **font_settings)  # Y label
     ax.set_xlabel('Read Length',
                 **font_settings)  # X label
 
     original_fontsize = font_settings["fontsize"]
     font_settings["fontsize"] = 20
```

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/plots/levenshtein_clustering.py` & `ExpoSeq-2.0.3/src/ExpoSeq/plots/levenshtein_clustering.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/plots/logo_plot.py` & `ExpoSeq-2.0.3/src/ExpoSeq/plots/logo_plot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/plots/plt_heatmap.py` & `ExpoSeq-2.0.3/src/ExpoSeq/plots/plt_heatmap.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/plots/protvec.py` & `ExpoSeq-2.0.3/src/ExpoSeq/plots/protvec.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/plots/relative_sequence_abundance.py` & `ExpoSeq-2.0.3/src/ExpoSeq/plots/relative_sequence_abundance.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/plots/saveFig.py` & `ExpoSeq-2.0.3/src/ExpoSeq/plots/saveFig.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/plots/stacked_aa_distribution.py` & `ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,27 @@
-from ExpoSeq.tidy_data.tidy_stacked_aa_distr import cleaning
-import matplotlib.pyplot as plt
+import pandas as pd
 
-def stacked_aa_distr(ax, sequencing_report, sample, region, protein, font_settings, legend_settings):
-    aa_distribution = cleaning(sequencing_report, sample, region, protein)
-    aa_distribution.plot(kind='bar', stacked=True, ax = ax)
-    ax.set_xlabel('Position on amino acid sequence', **font_settings)
+def cleaning(sequencing_report, sample, region, protein):
     if protein == True:
-        ax.set_ylabel('Relatvie Proportion of Amino Acid', **font_settings)
+        sequence_type = "aaSeqCDR3"
     else:
-        ax.set_ylabel('Relatvie Proportion of Nucleotide', **font_settings)
+        sequence_type = "nSeqCDR3"
+    sample = sequencing_report[sequencing_report["Experiment"] == sample]
+    local_report = sample[["Experiment", "clonesFraction", sequence_type]]
+    aminoacids = "ACDEFGHIKLMNPQRSTVWY"
 
-#    ax.set_xticks(rotation = 360)
-    ax.legend(bbox_to_anchor=(1.05, 1), loc='upper left')
-    original_fontsize = font_settings["fontsize"]
-    font_settings["fontsize"] = 22
-    if protein == True:
-        ax.set_title("Distribution of Aminoacids per Position for your sequences",pad = 12, **font_settings)
-    else:
-        ax.set_title("Distribution of Nucleotides per Position for your sequences",pad = 12, **font_settings)
-    ax.set_xticklabels([*range(region[0], region[1]+1)], rotation=0, ha='center')
-    font_settings["fontsize"] = original_fontsize
+    sequences = local_report[local_report[sequence_type].astype(str).str.len() >= region[1]][sequence_type]
+    max_length = local_report[sequence_type].str.len().max()
+    if not region[1] <= max_length:
+        raise ValueError("you upper region limit is above the longest sequence. That is not possible. Please reduce it.")
+    compDict = {aa: max_length*[0] for aa in aminoacids}
+    for seq in sequences:
+        for aa_position in range(len(seq)):
+            aminoacid = seq[aa_position]
+            if aminoacid == '*':
+                pass
+            else:
+                compDict[aminoacid][aa_position] += 1
+    aa_distribution = pd.DataFrame.from_dict(compDict)
+    aa_distribution = aa_distribution.divide(aa_distribution.sum(axis=1), axis=0)
+    aa_distribution = aa_distribution[(aa_distribution.index >= region[0]) & (aa_distribution.index <= region[1])]
+    return aa_distribution
```

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/plots/usq_plot.py` & `ExpoSeq-2.0.3/src/ExpoSeq/plots/usq_plot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/reset.py` & `ExpoSeq-2.0.3/src/ExpoSeq/reset.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/settings/blosum_62.txt` & `ExpoSeq-2.0.3/src/ExpoSeq/settings/blosum_62.txt`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/settings/change_save_settings.py` & `ExpoSeq-2.0.3/src/ExpoSeq/settings/change_save_settings.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/settings/plot_styler.py` & `ExpoSeq-2.0.3/src/ExpoSeq/settings/plot_styler.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/test_data/all_alignment_reports.pickle` & `ExpoSeq-2.0.3/src/ExpoSeq/test_data/all_alignment_reports.pickle`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/test_data/test_files/Chris_main_df.csv` & `ExpoSeq-2.0.3/src/ExpoSeq/test_data/test_files/Chris_main_df.csv`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/test_data/test_files/binding_data.csv` & `ExpoSeq-2.0.3/src/ExpoSeq/test_data/test_files/binding_data.csv`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/test_data/test_files/experiment_names.pickle` & `ExpoSeq-2.0.3/src/ExpoSeq/test_data/test_files/experiment_names.pickle`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/test_data/test_files/sequencing_report.csv` & `ExpoSeq-2.0.3/src/ExpoSeq/test_data/test_files/sequencing_report.csv`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/test_data/test_files/test1.fastq` & `ExpoSeq-2.0.3/src/ExpoSeq/test_data/test_files/test1.fastq`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/test_data/test_files/test2.fastq` & `ExpoSeq-2.0.3/src/ExpoSeq/test_data/test_files/test2.fastq`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/test_data/test_files/test3.fastq` & `ExpoSeq-2.0.3/src/ExpoSeq/test_data/test_files/test3.fastq`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/test_uploader.py` & `ExpoSeq-2.0.3/src/ExpoSeq/test_uploader.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/aminoacid_distribution.py` & `ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/aminoacid_distribution.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/barplot.py` & `ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/barplot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/clustering.py` & `ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/clustering.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py` & `ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py` & `ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py` & `ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py` & `ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py` & `ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/interpret_data.py` & `ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/interpret_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/read_extract_data.py` & `ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/read_extract_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/tidy_alignment_reports.py` & `ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/tidy_alignment_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py` & `ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py` & `ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py` & `ExpoSeq-2.0.3/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq.egg-info/PKG-INFO` & `ExpoSeq-2.0.3/src/ExpoSeq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ExpoSeq
-Version: 2.0.2
+Version: 2.0.3
 Summary: A pacakge which provides various ways to analyze NGS data from phage display campaigns
 Home-page: https://github.com/nilshof01/ExpoSeq
 Author: Nils Hofmann
 Author-email: n.hofmann.99@web.de
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `ExpoSeq-2.0.2/src/ExpoSeq.egg-info/SOURCES.txt` & `ExpoSeq-2.0.3/src/ExpoSeq.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 src/ExpoSeq/augment_data/structure_files.py
 src/ExpoSeq/augment_data/trimming.py
 src/ExpoSeq/augment_data/uploader.py
 src/ExpoSeq/plots/__init__.py
 src/ExpoSeq/plots/barplot.py
 src/ExpoSeq/plots/cluster_embedding.py
 src/ExpoSeq/plots/embedding_with_binding.py
+src/ExpoSeq/plots/hist_lvst_dist.py
 src/ExpoSeq/plots/length_distribution.py
 src/ExpoSeq/plots/levenshtein_clustering.py
 src/ExpoSeq/plots/logo_plot.py
 src/ExpoSeq/plots/plt_heatmap.py
 src/ExpoSeq/plots/protvec.py
 src/ExpoSeq/plots/relative_sequence_abundance.py
 src/ExpoSeq/plots/saveFig.py
@@ -61,14 +62,15 @@
 src/ExpoSeq/tidy_data/barplot.py
 src/ExpoSeq/tidy_data/clustering.py
 src/ExpoSeq/tidy_data/interpret_data.py
 src/ExpoSeq/tidy_data/read_extract_data.py
 src/ExpoSeq/tidy_data/tidy_USQ_plot_.py
 src/ExpoSeq/tidy_data/tidy_alignment_reports.py
 src/ExpoSeq/tidy_data/tidy_cluster_embedding.py
+src/ExpoSeq/tidy_data/tidy_hist_lvst_dist.py
 src/ExpoSeq/tidy_data/tidy_library.py
 src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py
 src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py
 src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py
 src/ExpoSeq/tidy_data/heatmaps/__init__.py
 src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py
 src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py
```

