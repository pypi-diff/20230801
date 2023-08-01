# Comparing `tmp/pgscatalog_utils-0.3.1.tar.gz` & `tmp/pgscatalog_utils-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgscatalog_utils-0.3.1.tar", max compression
+gzip compressed data, was "pgscatalog_utils-0.4.0.tar", max compression
```

## Comparing `pgscatalog_utils-0.3.1.tar` & `pgscatalog_utils-0.4.0.tar`

### file list

```diff
@@ -1,46 +1,56 @@
--rw-r--r--   0        0        0    11357 2023-01-27 10:25:08.048632 pgscatalog_utils-0.3.1/LICENSE
--rw-r--r--   0        0        0     3182 2023-01-27 10:25:08.048826 pgscatalog_utils-0.3.1/README.md
--rw-r--r--   0        0        0       22 2023-01-27 10:25:19.302556 pgscatalog_utils-0.3.1/pgscatalog_utils/__init__.py
--rw-r--r--   0        0        0        0 2023-01-27 10:25:08.049199 pgscatalog_utils-0.3.1/pgscatalog_utils/aggregate/__init__.py
--rw-r--r--   0        0        0     3245 2023-01-27 10:25:08.049333 pgscatalog_utils-0.3.1/pgscatalog_utils/aggregate/aggregate_scores.py
--rw-r--r--   0        0        0     2127 2023-01-27 10:25:08.049438 pgscatalog_utils-0.3.1/pgscatalog_utils/config.py
--rw-r--r--   0        0        0        0 2023-01-27 10:25:08.049518 pgscatalog_utils-0.3.1/pgscatalog_utils/download/__init__.py
--rw-r--r--   0        0        0     6276 2023-01-27 10:25:08.049666 pgscatalog_utils-0.3.1/pgscatalog_utils/download/download_scorefile.py
--rw-r--r--   0        0        0      726 2023-01-27 10:25:08.049772 pgscatalog_utils-0.3.1/pgscatalog_utils/download/publication.py
--rw-r--r--   0        0        0     3284 2023-01-27 10:25:08.049881 pgscatalog_utils-0.3.1/pgscatalog_utils/download/score.py
--rw-r--r--   0        0        0      896 2023-01-27 10:25:08.049984 pgscatalog_utils-0.3.1/pgscatalog_utils/download/trait.py
--rw-r--r--   0        0        0        0 2023-01-27 10:25:08.050076 pgscatalog_utils-0.3.1/pgscatalog_utils/match/__init__.py
--rw-r--r--   0        0        0     3385 2023-01-27 10:25:19.302896 pgscatalog_utils-0.3.1/pgscatalog_utils/match/combine_matches.py
--rw-r--r--   0        0        0     2822 2023-01-27 10:25:19.303105 pgscatalog_utils-0.3.1/pgscatalog_utils/match/filter.py
--rw-r--r--   0        0        0    13968 2023-01-27 10:25:19.303361 pgscatalog_utils-0.3.1/pgscatalog_utils/match/label.py
--rw-r--r--   0        0        0     3888 2023-01-27 10:25:19.303581 pgscatalog_utils-0.3.1/pgscatalog_utils/match/log.py
--rw-r--r--   0        0        0     4404 2023-01-27 10:25:08.050719 pgscatalog_utils-0.3.1/pgscatalog_utils/match/match.py
--rw-r--r--   0        0        0    14171 2023-01-27 10:25:19.303767 pgscatalog_utils-0.3.1/pgscatalog_utils/match/match_variants.py
--rw-r--r--   0        0        0     2087 2023-01-27 10:25:08.050890 pgscatalog_utils-0.3.1/pgscatalog_utils/match/preprocess.py
--rw-r--r--   0        0        0     2188 2023-01-27 10:25:19.303946 pgscatalog_utils-0.3.1/pgscatalog_utils/match/read.py
--rw-r--r--   0        0        0     1746 2023-01-27 10:25:08.051076 pgscatalog_utils-0.3.1/pgscatalog_utils/match/tempdir.py
--rw-r--r--   0        0        0     7523 2023-01-27 10:25:19.304167 pgscatalog_utils-0.3.1/pgscatalog_utils/match/write.py
--rw-r--r--   0        0        0        0 2023-01-27 10:25:08.051309 pgscatalog_utils-0.3.1/pgscatalog_utils/scorefile/__init__.py
--rw-r--r--   0        0        0     8586 2023-01-27 10:25:08.051446 pgscatalog_utils-0.3.1/pgscatalog_utils/scorefile/combine_scorefiles.py
--rw-r--r--   0        0        0     1222 2023-01-27 10:25:08.051534 pgscatalog_utils-0.3.1/pgscatalog_utils/scorefile/effect_type.py
--rw-r--r--   0        0        0     1753 2023-01-27 10:25:08.051617 pgscatalog_utils-0.3.1/pgscatalog_utils/scorefile/effect_weight.py
--rw-r--r--   0        0        0      883 2023-01-27 10:25:08.051703 pgscatalog_utils-0.3.1/pgscatalog_utils/scorefile/genome_build.py
--rw-r--r--   0        0        0     1435 2023-01-27 10:25:08.051784 pgscatalog_utils-0.3.1/pgscatalog_utils/scorefile/harmonised.py
--rw-r--r--   0        0        0     4952 2023-01-27 10:25:08.051887 pgscatalog_utils-0.3.1/pgscatalog_utils/scorefile/liftover.py
--rw-r--r--   0        0        0     3662 2023-01-27 10:25:08.051976 pgscatalog_utils-0.3.1/pgscatalog_utils/scorefile/qc.py
--rw-r--r--   0        0        0     2652 2023-01-27 10:25:08.052070 pgscatalog_utils-0.3.1/pgscatalog_utils/scorefile/read.py
--rw-r--r--   0        0        0     1582 2023-01-27 10:25:08.052169 pgscatalog_utils-0.3.1/pgscatalog_utils/scorefile/write.py
--rw-r--r--   0        0        0    10321 2023-01-27 10:25:08.052294 pgscatalog_utils-0.3.1/pgscatalog_utils/target.py
--rw-r--r--   0        0        0        0 2023-01-27 10:25:08.052379 pgscatalog_utils-0.3.1/pgscatalog_utils/validate/__init__.py
--rw-r--r--   0        0        0     1893 2023-01-27 10:25:08.052485 pgscatalog_utils-0.3.1/pgscatalog_utils/validate/common_constants.py
--rw-r--r--   0        0        0        0 2023-01-27 10:25:08.052568 pgscatalog_utils-0.3.1/pgscatalog_utils/validate/formatted/__init__.py
--rw-r--r--   0        0        0     8928 2023-01-27 10:25:08.052716 pgscatalog_utils-0.3.1/pgscatalog_utils/validate/formatted/validator.py
--rw-r--r--   0        0        0        0 2023-01-27 10:25:08.052798 pgscatalog_utils-0.3.1/pgscatalog_utils/validate/harmonized_position/__init__.py
--rw-r--r--   0        0        0     4584 2023-01-27 10:25:08.052921 pgscatalog_utils-0.3.1/pgscatalog_utils/validate/harmonized_position/validator.py
--rw-r--r--   0        0        0      916 2023-01-27 10:25:08.053015 pgscatalog_utils-0.3.1/pgscatalog_utils/validate/helpers.py
--rw-r--r--   0        0        0     8856 2023-01-27 10:25:08.053135 pgscatalog_utils-0.3.1/pgscatalog_utils/validate/schemas.py
--rw-r--r--   0        0        0     7034 2023-01-27 10:25:08.053280 pgscatalog_utils-0.3.1/pgscatalog_utils/validate/validate_scorefile.py
--rw-r--r--   0        0        0    17087 2023-01-27 10:25:08.053454 pgscatalog_utils-0.3.1/pgscatalog_utils/validate/validator_base.py
--rw-r--r--   0        0        0     1343 2023-01-27 10:25:19.305884 pgscatalog_utils-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     5240 1970-01-01 00:00:00.000000 pgscatalog_utils-0.3.1/setup.py
--rw-r--r--   0        0        0     4099 1970-01-01 00:00:00.000000 pgscatalog_utils-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-01 16:14:09.227816 pgscatalog_utils-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3558 2023-08-01 16:14:09.227816 pgscatalog_utils-0.4.0/README.md
+-rw-r--r--   0        0        0       22 2023-08-01 16:14:09.227816 pgscatalog_utils-0.4.0/pgscatalog_utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 16:14:09.227816 pgscatalog_utils-0.4.0/pgscatalog_utils/aggregate/__init__.py
+-rw-r--r--   0        0        0     3811 2023-08-01 16:14:09.227816 pgscatalog_utils-0.4.0/pgscatalog_utils/aggregate/aggregate_scores.py
+-rw-r--r--   0        0        0        0 2023-08-01 16:14:09.227816 pgscatalog_utils-0.4.0/pgscatalog_utils/ancestry/__init__.py
+-rw-r--r--   0        0        0     8643 2023-08-01 16:14:09.227816 pgscatalog_utils-0.4.0/pgscatalog_utils/ancestry/ancestry_analysis.py
+-rw-r--r--   0        0        0     2954 2023-08-01 16:14:09.227816 pgscatalog_utils-0.4.0/pgscatalog_utils/ancestry/read.py
+-rw-r--r--   0        0        0    24147 2023-08-01 16:14:09.227816 pgscatalog_utils-0.4.0/pgscatalog_utils/ancestry/tools.py
+-rw-r--r--   0        0        0     2246 2023-08-01 16:14:09.227816 pgscatalog_utils-0.4.0/pgscatalog_utils/config.py
+-rw-r--r--   0        0        0     7222 2023-08-01 16:14:09.227816 pgscatalog_utils-0.4.0/pgscatalog_utils/download/Catalog.py
+-rw-r--r--   0        0        0      122 2023-08-01 16:14:09.227816 pgscatalog_utils-0.4.0/pgscatalog_utils/download/CatalogCategory.py
+-rw-r--r--   0        0        0       95 2023-08-01 16:14:09.227816 pgscatalog_utils-0.4.0/pgscatalog_utils/download/GenomeBuild.py
+-rw-r--r--   0        0        0     1385 2023-08-01 16:14:09.227816 pgscatalog_utils-0.4.0/pgscatalog_utils/download/ScoringFile.py
+-rw-r--r--   0        0        0     2000 2023-08-01 16:14:09.227816 pgscatalog_utils-0.4.0/pgscatalog_utils/download/ScoringFileChecksum.py
+-rw-r--r--   0        0        0     2359 2023-08-01 16:14:09.227816 pgscatalog_utils-0.4.0/pgscatalog_utils/download/ScoringFileDownloader.py
+-rw-r--r--   0        0        0        0 2023-08-01 16:14:09.227816 pgscatalog_utils-0.4.0/pgscatalog_utils/download/__init__.py
+-rw-r--r--   0        0        0     2515 2023-08-01 16:14:09.227816 pgscatalog_utils-0.4.0/pgscatalog_utils/download/download_file.py
+-rw-r--r--   0        0        0     6939 2023-08-01 16:14:09.227816 pgscatalog_utils-0.4.0/pgscatalog_utils/download/download_scorefile.py
+-rw-r--r--   0        0        0        0 2023-08-01 16:14:09.227816 pgscatalog_utils-0.4.0/pgscatalog_utils/match/__init__.py
+-rw-r--r--   0        0        0     4042 2023-08-01 16:14:09.227816 pgscatalog_utils-0.4.0/pgscatalog_utils/match/combine_matches.py
+-rw-r--r--   0        0        0     2823 2023-08-01 16:14:09.227816 pgscatalog_utils-0.4.0/pgscatalog_utils/match/filter.py
+-rw-r--r--   0        0        0    14883 2023-08-01 16:14:09.227816 pgscatalog_utils-0.4.0/pgscatalog_utils/match/label.py
+-rw-r--r--   0        0        0     3944 2023-08-01 16:14:09.227816 pgscatalog_utils-0.4.0/pgscatalog_utils/match/log.py
+-rw-r--r--   0        0        0     4404 2023-08-01 16:14:09.227816 pgscatalog_utils-0.4.0/pgscatalog_utils/match/match.py
+-rw-r--r--   0        0        0    14867 2023-08-01 16:14:09.227816 pgscatalog_utils-0.4.0/pgscatalog_utils/match/match_variants.py
+-rw-r--r--   0        0        0     2087 2023-08-01 16:14:09.227816 pgscatalog_utils-0.4.0/pgscatalog_utils/match/preprocess.py
+-rw-r--r--   0        0        0     2188 2023-08-01 16:14:09.227816 pgscatalog_utils-0.4.0/pgscatalog_utils/match/read.py
+-rw-r--r--   0        0        0     1746 2023-08-01 16:14:09.231816 pgscatalog_utils-0.4.0/pgscatalog_utils/match/tempdir.py
+-rw-r--r--   0        0        0     7547 2023-08-01 16:14:09.231816 pgscatalog_utils-0.4.0/pgscatalog_utils/match/write.py
+-rw-r--r--   0        0        0     6615 2023-08-01 16:14:09.231816 pgscatalog_utils-0.4.0/pgscatalog_utils/relabel/relabel_ids.py
+-rwxr-xr-x   0        0        0    10768 2023-08-01 16:14:09.231816 pgscatalog_utils-0.4.0/pgscatalog_utils/samplesheet/check.py
+-rw-r--r--   0        0        0        0 2023-08-01 16:14:09.231816 pgscatalog_utils-0.4.0/pgscatalog_utils/scorefile/__init__.py
+-rw-r--r--   0        0        0     8586 2023-08-01 16:14:09.231816 pgscatalog_utils-0.4.0/pgscatalog_utils/scorefile/combine_scorefiles.py
+-rw-r--r--   0        0        0     1222 2023-08-01 16:14:09.231816 pgscatalog_utils-0.4.0/pgscatalog_utils/scorefile/effect_type.py
+-rw-r--r--   0        0        0     1753 2023-08-01 16:14:09.231816 pgscatalog_utils-0.4.0/pgscatalog_utils/scorefile/effect_weight.py
+-rw-r--r--   0        0        0      883 2023-08-01 16:14:09.231816 pgscatalog_utils-0.4.0/pgscatalog_utils/scorefile/genome_build.py
+-rw-r--r--   0        0        0     1435 2023-08-01 16:14:09.231816 pgscatalog_utils-0.4.0/pgscatalog_utils/scorefile/harmonised.py
+-rw-r--r--   0        0        0     4952 2023-08-01 16:14:09.231816 pgscatalog_utils-0.4.0/pgscatalog_utils/scorefile/liftover.py
+-rw-r--r--   0        0        0     3662 2023-08-01 16:14:09.231816 pgscatalog_utils-0.4.0/pgscatalog_utils/scorefile/qc.py
+-rw-r--r--   0        0        0     2652 2023-08-01 16:14:09.231816 pgscatalog_utils-0.4.0/pgscatalog_utils/scorefile/read.py
+-rw-r--r--   0        0        0     1582 2023-08-01 16:14:09.231816 pgscatalog_utils-0.4.0/pgscatalog_utils/scorefile/write.py
+-rw-r--r--   0        0        0    10321 2023-08-01 16:14:09.231816 pgscatalog_utils-0.4.0/pgscatalog_utils/target.py
+-rw-r--r--   0        0        0        0 2023-08-01 16:14:09.231816 pgscatalog_utils-0.4.0/pgscatalog_utils/validate/__init__.py
+-rw-r--r--   0        0        0     1893 2023-08-01 16:14:09.231816 pgscatalog_utils-0.4.0/pgscatalog_utils/validate/common_constants.py
+-rw-r--r--   0        0        0        0 2023-08-01 16:14:09.231816 pgscatalog_utils-0.4.0/pgscatalog_utils/validate/formatted/__init__.py
+-rw-r--r--   0        0        0     8928 2023-08-01 16:14:09.231816 pgscatalog_utils-0.4.0/pgscatalog_utils/validate/formatted/validator.py
+-rw-r--r--   0        0        0        0 2023-08-01 16:14:09.231816 pgscatalog_utils-0.4.0/pgscatalog_utils/validate/harmonized_position/__init__.py
+-rw-r--r--   0        0        0     4584 2023-08-01 16:14:09.231816 pgscatalog_utils-0.4.0/pgscatalog_utils/validate/harmonized_position/validator.py
+-rw-r--r--   0        0        0      916 2023-08-01 16:14:09.231816 pgscatalog_utils-0.4.0/pgscatalog_utils/validate/helpers.py
+-rw-r--r--   0        0        0     8869 2023-08-01 16:14:09.231816 pgscatalog_utils-0.4.0/pgscatalog_utils/validate/schemas.py
+-rw-r--r--   0        0        0     7034 2023-08-01 16:14:09.231816 pgscatalog_utils-0.4.0/pgscatalog_utils/validate/validate_scorefile.py
+-rw-r--r--   0        0        0    17087 2023-08-01 16:14:09.231816 pgscatalog_utils-0.4.0/pgscatalog_utils/validate/validator_base.py
+-rw-r--r--   0        0        0     1619 2023-08-01 16:14:09.231816 pgscatalog_utils-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6105 1970-01-01 00:00:00.000000 pgscatalog_utils-0.4.0/setup.py
+-rw-r--r--   0        0        0     4520 1970-01-01 00:00:00.000000 pgscatalog_utils-0.4.0/PKG-INFO
```

### Comparing `pgscatalog_utils-0.3.1/LICENSE` & `pgscatalog_utils-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pgscatalog_utils-0.3.1/README.md` & `pgscatalog_utils-0.4.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # PGS Catalog utilities
 
 [![CI](https://github.com/PGScatalog/pgscatalog_utils/actions/workflows/main.yml/badge.svg)](https://github.com/PGScatalog/pgscatalog_utils/actions/workflows/main.yml)
+[![DOI](https://zenodo.org/badge/513521373.svg)](https://zenodo.org/badge/latestdoi/513521373)
 
 This repository is a collection of useful tools for downloading and working with scoring files from the
 PGS Catalog. This is mostly used internally by the PGS Catalog Calculator ([`PGScatalog/pgsc_calc`](https://github.com/PGScatalog/pgsc_calc)); however, other users may find some of these tools helpful.
 
 ## Overview
 
 * `download_scorefiles`: Download scoring files by PGS ID (accession) in genome builds GRCh37 or GRCh38
 * `combine_scorefile`: Combine multiple scoring files into a single scoring file
 in 'long' format
 * `match_variants`: Match target variants (bim or pvar files) against the output
 of `combine_scorefile` to produce scoring files for plink 2
+* `ancestry_analysis` : use genetic PCA loadings to compare samples to population reference panels, and report PGS adjusted for these axes of genetic ancestry. The PCs will likely have been generated with [FRAPOSA (pgs catalog version)](https://github.com/PGScatalog/fraposa_pgsc)
 * `validate_scorefiles`: Check/validate that the scoring files and harmonized scoring files match the PGS Catalog scoring file formats.
 
 ## Installation
 
 ```
 $ pip install pgscatalog-utils
 ```
```

### Comparing `pgscatalog_utils-0.3.1/pgscatalog_utils/aggregate/aggregate_scores.py` & `pgscatalog_utils-0.4.0/pgscatalog_utils/download/download_file.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,92 +1,71 @@
-import argparse
-import textwrap
+import logging
+import os
+import pathlib
+import time
+import urllib.parse
+from ftplib import FTP
+from urllib.parse import urlsplit
 
-import pandas as pd
+import requests
 
-from pgscatalog_utils.config import set_logging_level
-import glob
-import logging
+from pgscatalog_utils import config
 
 logger = logging.getLogger(__name__)
 
 
-def aggregate_scores():
-    args = _parse_args()
-    set_logging_level(args.verbose)
-    df = aggregate(list(set(args.scores)))
-    logger.debug("Compressing and writing combined scores")
-    df.to_csv('aggregated_scores.txt.gz', sep='\t', compression='gzip')
-
-
-def aggregate(scorefiles: list[str]):
-    combined = pd.DataFrame()
-    aggcols = set()
-
-    for i, path in enumerate(scorefiles):
-        logger.debug(f"Reading {path}")
-        # pandas can automatically detect zst compression, neat!
-        df = (pd.read_table(path)
-              .assign(sampleset=path.split('_')[0])
-              .set_index(['sampleset', '#IID']))
-
-        df.index.names = ['sampleset', 'IID']
-
-        # Subset to aggregatable columns
-        df = df[_select_agg_cols(df.columns)]
-        aggcols.update(set(df.columns))
-
-        # Combine DFs
-        if i == 0:
-            logger.debug('Initialising combined DF')
-            combined = df.copy()
+def download_file(url: str, local_path: str, overwrite: bool, ftp_fallback: bool) -> None:
+    if config.OUTDIR.joinpath(local_path).exists():
+        if not overwrite:
+            logger.warning(f"{config.OUTDIR.joinpath(local_path)} exists and overwrite is false, skipping download")
+            return
+        elif overwrite:
+            logger.warning(f"Overwriting {config.OUTDIR.joinpath(local_path)}")
+
+    logger.info(f"Downloading {local_path} from {url}")
+    attempt: int = 0
+
+    while attempt < config.MAX_RETRIES:
+        response: requests.Response = requests.get(url)
+        match response.status_code:
+            case 200:
+                with open(config.OUTDIR.joinpath(local_path), "wb") as f:
+                    f.write(response.content)
+                logger.info("HTTPS download complete")
+                attempt = 0
+                break
+            case _:
+                logger.warning(f"HTTP status {response.status_code} at download attempt {attempt}")
+                attempt += 1
+                time.sleep(5)
+
+    if attempt > config.MAX_RETRIES:
+        if ftp_fallback:
+            logger.warning("Attempting FTP fallback")
+            _ftp_fallback_download(url=url, local_path=local_path)
         else:
-            logger.debug('Adding to combined DF')
-            combined = combined.add(df, fill_value=0)
-
-    assert all([x in combined.columns for x in aggcols]), "All Aggregatable Columns are present in the final DF"
-
-    return combined.pipe(_calculate_average)
-
-
-def _calculate_average(combined: pd.DataFrame):
-    logger.debug("Averaging data")
-    avgs = combined.loc[:, combined.columns.str.endswith('_SUM')].divide(combined['DENOM'], axis=0)
-    avgs.columns = avgs.columns.str.replace('_SUM', '_AVG')
-    return pd.concat([combined, avgs], axis=1)
-
-
-def _select_agg_cols(cols):
-    keep_cols = ['DENOM']
-    return [x for x in cols if (x.endswith('_SUM') and (x != 'NAMED_ALLELE_DOSAGE_SUM')) or (x in keep_cols)]
-
-
-def _description_text() -> str:
-    return textwrap.dedent('''
-    Aggregate plink .sscore files into a combined TSV table.
-    
-    This aggregation sums scores that were calculated from plink
-    .scorefiles. Scorefiles may be split to calculate scores over different
-    chromosomes or effect types. The PGS Catalog calculator automatically splits
-    scorefiles where appropriate, and uses this script to combine them.
-    
-    Input .sscore files can be optionally compressed with zstd or gzip. 
-    
-    The aggregated output scores are compressed with gzip.
-   ''')
-
-
-def _parse_args(args=None) -> argparse.Namespace:
-    parser = argparse.ArgumentParser(description=_description_text(),
-                                     formatter_class=argparse.RawDescriptionHelpFormatter)
-    parser.add_argument('-s', '--scores', dest='scores', required=True, nargs='+',
-                        help='<Required> List of scorefile paths. Use a wildcard (*) to select multiple files.')
-    parser.add_argument('-o', '--outdir', dest='outdir', required=True,
-                        default='scores/', help='<Required> Output directory to store downloaded files')
-    parser.add_argument('-v', '--verbose', dest='verbose', action='store_true',
-                        help='<Optional> Extra logging information')
-    return parser.parse_args(args)
-
+            raise Exception(f"Can't download {url} using HTTPS")
 
-if __name__ == "__main__":
-    aggregate_scores()
 
+def _ftp_fallback_download(url: str, local_path: str) -> None:
+    url = url.replace("https://", "ftp://")
+    retries = 0
+
+    while retries < config.MAX_RETRIES:
+        try:
+            spliturl: urllib.parse.SplitResult = urlsplit(url)
+            ftp = FTP(spliturl.hostname)
+            ftp.login()
+            ftp.cwd(str(pathlib.Path(urlsplit(url).path).parent))
+            with open(config.OUTDIR.joinpath(local_path), "wb") as file:
+                ftp.retrbinary("RETR " + local_path, file.write)
+                ftp.quit()
+                logger.info("FTP download completed")
+                return
+        except Exception as e:
+            if "421" in str(e):
+                retries += 1
+                logger.debug(f"FTP server is busy. Waiting and retrying. Retry {retries} of {config.MAX_RETRIES}")
+                time.sleep(config.DOWNLOAD_WAIT_TIME)
+            else:
+                logger.critical(f"Download failed: {e}")
+                raise Exception
```

### Comparing `pgscatalog_utils-0.3.1/pgscatalog_utils/config.py` & `pgscatalog_utils-0.4.0/pgscatalog_utils/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 import atexit
 import logging
 import os
+import pathlib
 import tempfile
+import typing
 
 import polars as pl
 
 from pgscatalog_utils.match import tempdir
 
 N_THREADS: int = 1  # dummy value, is reset by args.n_threads (default: 1)
-OUTDIR: str = "."  # dummy value, reset by args.outdir
+OUTDIR: pathlib.Path
 TEMPDIR: tempfile.TemporaryDirectory
+PGSC_CALC_VERSION: typing.Union[None, str] = None
+OVERWRITE: bool = False
+MAX_RETRIES: int = 3
+DOWNLOAD_WAIT_TIME: int = 30
 
 logger = logging.getLogger(__name__)
 
 
 def setup_tmpdir(outdir, combine=False):
     if combine:
         work_dir = "work_combine"
```

### Comparing `pgscatalog_utils-0.3.1/pgscatalog_utils/download/download_scorefile.py` & `pgscatalog_utils-0.4.0/pgscatalog_utils/download/download_scorefile.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,113 +1,115 @@
 import argparse
 import logging
 import os
-import shutil
+import pathlib
 import textwrap
-import time
-from contextlib import closing
-from functools import reduce
-from urllib import request as request
-from urllib.error import HTTPError, URLError
-
-from pgscatalog_utils.download.publication import query_publication
-from pgscatalog_utils.download.score import get_url
-from pgscatalog_utils.download.trait import query_trait
-from pgscatalog_utils.config import set_logging_level
+import typing
+
+from pgscatalog_utils import config
+from pgscatalog_utils.download.CatalogCategory import CatalogCategory
+from pgscatalog_utils.download.Catalog import CatalogQuery, CatalogResult
+from pgscatalog_utils.download.GenomeBuild import GenomeBuild
+from pgscatalog_utils.download.ScoringFileDownloader import ScoringFileDownloader
+
 
 logger = logging.getLogger(__name__)
 
 
 def download_scorefile() -> None:
     args = _parse_args()
-    set_logging_level(args.verbose)
+    config.set_logging_level(args.verbose)
     _check_args(args)
-    _mkdir(args.outdir)
-
-    if args.build is None:
-        logger.critical(f'Downloading scoring file(s) in the author-reported genome build')
-    elif args.build in ['GRCh37', 'GRCh38']:
-        logger.critical(f'Downloading harmonized scoring file(s) in build: {args.build}.')
-    else:
-        logger.critical(f'Invalid genome build specified: {args.build}. Only -b GRCh37 and -b GRCh38 are supported')
-        raise Exception
 
-    pgs_lst: list[list[str]] = []
+    build: typing.Union[None, GenomeBuild]
+    match args.build:
+        case None:
+            logger.info("Downloading scoring file(s) in the author-reported genome build")
+            build = None
+        case "GRCh37":
+            build = GenomeBuild.GRCh37
+        case "GRCh38":
+            build = GenomeBuild.GRCh38
+        case _:
+            logger.critical(f"Invalid genome build specified: {args.build}")
+            logger.critical("Only -b GRCh37 and -b GRCh38 are supported")
+            raise Exception
+
+    if build is not None:
+        logger.info(f"Downloading harmonised scoring file(s) in build: {build}")
+
+    if args.overwrite_existing_file:
+        logger.debug("--overwrite, overwriting new version of the Scoring file, if available")
+        logger.warning(
+            "Existing Scoring files will be overwritten if new versions of the Scoring files are available for download.")
 
-    pgsc_calc_info = None
     if args.pgsc_calc:
-        pgsc_calc_info = args.pgsc_calc
+        config.PGSC_CALC_VERSION = args.pgsc_calc
+        logger.info(f"Setting user agent to {config.PGSC_CALC_VERSION} for PGS Catalog API queries")
 
+    config.OUTDIR = pathlib.Path(args.outdir).resolve()
+    logger.info(f"Download directory: {config.OUTDIR}")
+    config.OUTDIR.mkdir(exist_ok=True)
+    config.OVERWRITE = args.overwrite_existing_file
+
+    results: list[list[CatalogResult]] = []
     if args.efo:
+        inc_child = False
         if args.efo_include_children:
             logger.debug("--trait set, querying traits (including PGS for child terms)")
+            inc_child = True
         else:
             logger.debug("--trait set, querying traits")
-        pgs_lst = pgs_lst + [query_trait(x, pgsc_calc_info, args.efo_include_children) for x in args.efo]
-
+        for term in args.efo:
+            results.append(CatalogQuery(CatalogCategory.TRAIT, term, include_children=inc_child,
+                                    pgsc_calc_version=config.PGSC_CALC_VERSION).get())
 
     if args.pgp:
         logger.debug("--pgp set, querying publications")
-        pgs_lst = pgs_lst + [query_publication(x, pgsc_calc_info) for x in args.pgp]
+        for term in args.pgp:
+            results.append(CatalogQuery(CatalogCategory.PUBLICATION, term, pgsc_calc_version=config.PGSC_CALC_VERSION).get())
 
     if args.pgs:
         logger.debug("--id set, querying scores")
-        pgs_lst.append(args.pgs)  # pgs_lst: a list containing up to three flat lists
-
-    pgs_id: list[str] = list(set(reduce(lambda x, y: x + y, pgs_lst)))
-
-    urls: dict[str, str] = get_url(pgs_id, args.build, pgsc_calc_info)
-
-    for pgsid, url in urls.items():
-        logger.debug(f"Downloading {pgsid} from {url}")
-        if args.build is None:
-            path: str = os.path.join(args.outdir, pgsid + '.txt.gz')
-        else:
-            path: str = os.path.join(args.outdir, pgsid + f'_hmPOS_{args.build}.txt.gz')
-        _download_ftp(url, path)
-
-
-def _mkdir(outdir: str) -> None:
-    if not os.path.exists(outdir):
-        logger.debug("Creating output directory")
-        os.makedirs(outdir)
+        results.append(
+            CatalogQuery(CatalogCategory.SCORE, args.pgs,
+                         pgsc_calc_version=config.PGSC_CALC_VERSION).get())  # pgs_lst: a list containing up to three flat lists
+
+    flat_results = [element for sublist in results for element in sublist]
+
+    ScoringFileDownloader(results=flat_results, genome_build=build, overwrite=config.OVERWRITE).download_files()
+
+    # warn if missing PGS IDs in downloaded files
+    requested_pgs: set[str]
+    if args.pgs is None:
+        requested_pgs = set()
+    else:
+        requested_pgs = set(args.pgs)
+    missing_pgs: set[str] = requested_pgs.difference(flat_results[-1].pgs_ids)
 
+    if missing_pgs:
+        logger.warning(f"Requested PGS scoring file not downloaded: {missing_pgs}")
+        logger.warning("Check if the accessions are valid")
 
-def _download_ftp(url: str, path: str, retry:int = 0) -> None:
-    if os.path.exists(path):
-        logger.warning(f"File already exists at {path}, skipping download")
-        return
-    else:
-        try:
-            with closing(request.urlopen(url)) as r:
-                with open(path, 'wb') as f:
-                    shutil.copyfileobj(r, f)
-        except (HTTPError, URLError) as error:
-            max_retries = 5
-            print(f'Download failed: {error.reason}')
-            # Retry to download the file if the server is busy
-            if '421' in error.reason and retry < max_retries:
-                print(f'> Retry to download the file ... attempt {retry+1} out of {max_retries}.')
-                retry += 1
-                time.sleep(10)
-                _download_ftp(url,path,retry)
-            else:
-                raise RuntimeError("Failed to download '{}'.\nError message: '{}'".format(url, error.reason))
+    logger.info("Downloads complete")
 
 
 def _check_args(args):
     if not args.efo:
         if not args.pgp:
             if not args.pgs:
-                logger.critical("One of --trait, --pgp, or --id is required to download scorefiles")
+                logger.critical(
+                    "One of --trait, --pgp, or --id is required to download scorefiles"
+                )
                 raise Exception
 
 
 def _description_text() -> str:
-    return textwrap.dedent('''\
+    return textwrap.dedent(
+        """\
     Download a set of scoring files from the PGS Catalog using PGS
     Scoring IDs, traits, or publication IDs.
     
     The PGS Catalog API is queried to get a list of scoring file
     URLs. Scoring files are downloaded via FTP to a specified
     directory. PGS Catalog scoring files are staged with the name:
 
@@ -115,43 +117,93 @@
 
     If a valid build is specified harmonized files are downloaded as:
     
         {PGS_ID}_hmPOS_{genome_build}.txt.gz
     
     These harmonised scoring files contain genomic coordinates,
     remapped from author-submitted information such as rsids.
-   ''')
+   """
+    )
 
 
 def _epilog_text() -> str:
-    return textwrap.dedent('''\
+    return textwrap.dedent(
+        """\
     download_scorefiles will skip downloading a scoring file if it
     already exists in the download directory. This can be useful if
     the download process is interrupted and needs to be restarted
     later. You can track download progress with the verbose flag.    
-   ''')
+   """
+    )
 
 
 def _parse_args(args=None) -> argparse.Namespace:
-    parser = argparse.ArgumentParser(description=_description_text(), epilog=_epilog_text(),
-                                     formatter_class=argparse.RawDescriptionHelpFormatter)
-    parser.add_argument('-i', '--pgs', nargs='+', dest='pgs', help='PGS Catalog ID(s) (e.g. PGS000001)')
-    parser.add_argument('-t', '--efo', dest='efo', nargs='+',
-                        help='Traits described by an EFO term(s) (e.g. EFO_0004611)')
-    parser.add_argument('-e', '--efo_direct', dest='efo_include_children', action='store_false',
-                        help='<Optional> Return only PGS tagged with exact EFO term '
-                             '(e.g. no PGS for child/descendant terms in the ontology)')
-    parser.add_argument('-p', '--pgp', dest='pgp', help='PGP publication ID(s) (e.g. PGP000007)', nargs='+')
-    parser.add_argument('-b', '--build', dest='build', choices=['GRCh37', 'GRCh38'],
-                        help='Download Harmonized Scores with Positions in Genome build: GRCh37 or GRCh38')
-    parser.add_argument('-o', '--outdir', dest='outdir', required=True,
-                        default='scores/',
-                        help='<Required> Output directory to store downloaded files')
-    parser.add_argument('-c', '--pgsc_calc', dest='pgsc_calc',
-                        help='<Optional> Provide information about downloading scoring files via pgsc_calc')
-    parser.add_argument('-v', '--verbose', dest='verbose', action='store_true',
-                        help='<Optional> Extra logging information')
+    parser = argparse.ArgumentParser(
+        description=_description_text(),
+        epilog=_epilog_text(),
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+    )
+    parser.add_argument(
+        "-i", "--pgs", nargs="+", dest="pgs", help="PGS Catalog ID(s) (e.g. PGS000001)"
+    )
+    parser.add_argument(
+        "-t",
+        "--efo",
+        dest="efo",
+        nargs="+",
+        help="Traits described by an EFO term(s) (e.g. EFO_0004611)",
+    )
+    parser.add_argument(
+        "-e",
+        "--efo_direct",
+        dest="efo_include_children",
+        action="store_false",
+        help="<Optional> Return only PGS tagged with exact EFO term "
+             "(e.g. no PGS for child/descendant terms in the ontology)",
+    )
+    parser.add_argument(
+        "-p",
+        "--pgp",
+        dest="pgp",
+        help="PGP publication ID(s) (e.g. PGP000007)",
+        nargs="+",
+    )
+    parser.add_argument(
+        "-b",
+        "--build",
+        dest="build",
+        choices=["GRCh37", "GRCh38"],
+        help="Download Harmonized Scores with Positions in Genome build: GRCh37 or GRCh38",
+    )
+    parser.add_argument(
+        "-o",
+        "--outdir",
+        dest="outdir",
+        required=True,
+        default="scores/",
+        help="<Required> Output directory to store downloaded files",
+    )
+    parser.add_argument(
+        "-w",
+        "--overwrite",
+        dest="overwrite_existing_file",
+        action="store_true",
+        help="<Optional> Overwrite existing Scoring File if a new version is available for download on the FTP",
+    )
+    parser.add_argument(
+        "-c",
+        "--pgsc_calc",
+        dest="pgsc_calc",
+        help="<Optional> Provide information about downloading scoring files via pgsc_calc",
+    )
+    parser.add_argument(
+        "-v",
+        "--verbose",
+        dest="verbose",
+        action="store_true",
+        help="<Optional> Extra logging information",
+    )
     return parser.parse_args(args)
 
 
 if __name__ == "__main__":
     download_scorefile()
```

### Comparing `pgscatalog_utils-0.3.1/pgscatalog_utils/match/combine_matches.py` & `pgscatalog_utils-0.4.0/pgscatalog_utils/match/combine_matches.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 from pgscatalog_utils.match.read import read_scorefile
 
 logger = logging.getLogger(__name__)
 
 
 def combine_matches():
     args = _parse_args()
+    if (args.combined is False) and (args.split is False):
+        logger.warning("No output format specified, writing to combined scoring file")
+        args.combined = True
+
     config.set_logging_level(args.verbose)
     config.setup_polars_threads(args.n_threads)
     config.setup_tmpdir(args.outdir, combine=True)
     config.OUTDIR = args.outdir
 
     with pl.StringCache():
         scorefile = read_scorefile(path=args.scorefile, chrom=None)  # chrom=None to read all variants
@@ -54,19 +58,24 @@
                         help='<Required> Label for target genomic dataset')
     parser.add_argument('-s', '--scorefile', dest='scorefile', required=True,
                         help='<Required> Path to scorefile')
     parser.add_argument('-m', '--matches', dest='matches', required=True, nargs='+',
                         help='<Required> List of match files')
     parser.add_argument('--min_overlap', dest='min_overlap', required=True,
                         type=float, help='<Required> Minimum proportion of variants to match before error')
+    parser.add_argument('-IDs', '--filter_IDs', dest='filter',
+                        help='<Optional> Path to file containing list of variant IDs that can be included in the final scorefile.'
+                             '[useful for limiting scoring files to variants present in multiple datasets]')
     parser = add_match_args(parser) # params for labelling matches
     parser.add_argument('--outdir', dest='outdir', required=True,
                         help='<Required> Output directory')
     parser.add_argument('--split', dest='split', default=False, action='store_true',
-                        help='<Optional> Split scorefile per chromosome?')
+                        help='<Optional> Write scorefiles split per chromosome?')
+    parser.add_argument('--combined', dest='combined', default=False, action='store_true',
+                        help='<Optional> Write scorefiles in combined format?')
     parser.add_argument('-n', dest='n_threads', default=1, help='<Optional> n threads for matching', type=int)
     parser.add_argument('-v', '--verbose', dest='verbose', action='store_true',
                         help='<Optional> Extra logging information')
     return parser.parse_args(args)
 
 
 if __name__ == "__main__":
```

### Comparing `pgscatalog_utils-0.3.1/pgscatalog_utils/match/filter.py` & `pgscatalog_utils-0.4.0/pgscatalog_utils/match/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     match_log: pl.LazyFrame = (_join_filtered_matches(filtered_matches, scorefile, dataset)
                                .with_columns(pl.col('best_match').fill_null(False)))
 
     fail_rates: pl.DataFrame = _calculate_match_rate(match_log).collect()  # collect for iteration
 
     scores: list[pl.DataFrame] = []
     for accession, rate in zip(fail_rates['accession'].to_list(), fail_rates['fail_rate'].to_list()):
-        if rate < (1 - min_overlap):
+        if rate <= (1 - min_overlap):
             df: pl.DataFrame = pl.DataFrame({'accession': [accession], 'score_pass': [True], 'match_rate': [1 - rate]})
             logger.debug(f"Score {accession} passes minimum matching threshold ({1 - rate:.2%}  variants match)")
             scores.append(df.with_column(pl.col('accession').cast(pl.Categorical)))
         else:
             df: pl.DataFrame = pl.DataFrame({'accession': [accession], 'score_pass': [False], 'match_rate': [1 - rate]})
             logger.error(f"Score {accession} fails minimum matching threshold ({1 - rate:.2%} variants match)")
             scores.append(df.with_column(pl.col('accession').cast(pl.Categorical)))
```

### Comparing `pgscatalog_utils-0.3.1/pgscatalog_utils/match/label.py` & `pgscatalog_utils-0.4.0/pgscatalog_utils/match/label.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,36 +5,44 @@
 from pgscatalog_utils.match.preprocess import complement_valid_alleles
 
 logger = logging.getLogger(__name__)
 
 
 def make_params_dict(args) -> dict[str, bool]:
     """ Make a dictionary with parameters that control labelling match candidates """
+    filter_IDs = []
+    if args.filter:
+        logger.debug("Reading filter file (variant IDs)")
+        with open(args.filter, 'r') as f:
+            filter_IDs = pl.Series([line.strip() for line in f], dtype=pl.Utf8)
+
     return {'keep_first_match': args.keep_first_match,
             'remove_ambiguous': args.remove_ambiguous,
             'skip_flip': args.skip_flip,
-            'remove_multiallelic': args.remove_multiallelic}
+            'remove_multiallelic': args.remove_multiallelic,
+            'filter_IDs': filter_IDs}
 
 
 def label_matches(df: pl.LazyFrame, params: dict[str, bool]) -> pl.LazyFrame:
     """ Label match candidates with additional metadata. Column definitions:
 
     - match_candidate: All input variants that were returned from match.get_all_matches() (always True in this function)
     - best_match: True if row is the best possible match type (refalt > altref > ...)
     - duplicate: True if more than one best match exists for the same accession and ID
     - ambiguous: True if ambiguous
     """
-    assert set(params.keys()) == {'keep_first_match', 'remove_ambiguous', 'remove_multiallelic', 'skip_flip'}
+    assert set(params.keys()) == {'keep_first_match', 'remove_ambiguous', 'remove_multiallelic', 'skip_flip', 'filter_IDs'}
     labelled = (df.with_column(pl.lit(False).alias('exclude'))  # set up dummy exclude column for _label_*
                 .pipe(_label_best_match)
                 .pipe(_label_duplicate_best_match)
                 .pipe(_label_duplicate_id, params['keep_first_match'])
                 .pipe(_label_biallelic_ambiguous, params['remove_ambiguous'])
                 .pipe(_label_multiallelic, params['remove_multiallelic'])
                 .pipe(_label_flips, params['skip_flip'])
+                .pipe(_label_filter, params['filter_IDs'])
                 .with_column(pl.lit(True).alias('match_candidate')))
 
     return _encode_match_priority(labelled)
 
 
 def _encode_match_priority(df: pl.LazyFrame) -> pl.LazyFrame:
     """ Encode a new column called match status containing matched, unmatched, excluded, and not_best """
@@ -211,7 +219,20 @@
         return df.with_column(pl.when(pl.col('match_flipped') == True)
                               .then(True)
                               .otherwise(pl.col('exclude'))  # don't overwrite existing exclude flags
                               .alias('exclude'))
     else:
         logger.debug("Not excluding flipped matches")
         return df
+
+
+def _label_filter(df: pl.LazyFrame, filter_IDs: list) -> pl.LazyFrame:
+    nIDs = len(filter_IDs)
+    if nIDs > 0:
+        logger.debug("Excluding variants that are not in ID list (read {} IDs)".format(nIDs))
+        df = df.with_column(pl.col('ID').is_in(filter_IDs).alias('match_IDs'))
+        return df.with_column(pl.when(pl.col('match_IDs') == False)
+                              .then(True)
+                              .otherwise(pl.col('exclude'))
+                              .alias('exclude'))
+    else:
+        return df.with_column((pl.lit('NA')).alias('match_IDs'))
```

### Comparing `pgscatalog_utils-0.3.1/pgscatalog_utils/match/log.py` & `pgscatalog_utils-0.4.0/pgscatalog_utils/match/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     """ Make an aggregated table """
     logger.debug("Aggregating best matches into a summary table")
     best_matches: pl.LazyFrame = match_candidates.filter(pl.col('best_match') == True)
     return (scorefile.join(best_matches, on=['row_nr', 'accession'], how='outer')
             .select(pl.exclude("^.*_right$"))
             .with_columns([pl.col('match_status').fill_null(value='unmatched'),
                            pl.lit(dataset).alias('dataset')])  # fill in unmatched variants
-            .groupby(['dataset', 'accession', 'match_status', 'ambiguous', 'is_multiallelic', 'match_flipped',
-                      'duplicate_best_match', 'duplicate_ID'])
+            .groupby(['dataset', 'accession', 'ambiguous', 'is_multiallelic', 'match_flipped',
+                      'duplicate_best_match', 'duplicate_ID', 'match_IDs', 'match_status'])
             .agg(pl.count())
             .join(filter_summary, how='left', on='accession')
             .pipe(_prettify_summary))
 
 
 def check_log_count(scorefile: pl.LazyFrame, summary_log: pl.LazyFrame) -> None:
     """ Check aggregated counts vs original from scoring file """
@@ -41,25 +41,25 @@
     assert (log_count.get_column('count') == log_count.get_column(
         'count_right')).all(), "Log doesn't match input scoring file"
     logger.debug("Log matches input scoring file")
 
 
 def _prettify_summary(df: pl.LazyFrame) -> pl.LazyFrame:
     keep_cols = ["dataset", "accession", "score_pass", "match_status", "ambiguous", "is_multiallelic",
-                 "duplicate_best_match", "duplicate_ID", "count", "percent"]
+                 "duplicate_best_match", "duplicate_ID", 'match_flipped', "match_IDs", "count", "percent"]
     return (df.with_column((pl.col("count") / pl.sum("count") * 100)
                            .over(["dataset", "accession"])
                            .alias("percent"))
             .select(keep_cols))
 
 
 def _prettify_log(df: pl.LazyFrame) -> pl.LazyFrame:
     keep_cols = ["row_nr", "accession", "chr_name", "chr_position", "effect_allele", "other_allele", "effect_weight",
                  "effect_type", "ID", "REF", "ALT", "matched_effect_allele", "match_type", "is_multiallelic",
-                 "ambiguous", "match_flipped", "best_match", "exclude", "duplicate_best_match", "duplicate_ID",
+                 "ambiguous", "match_flipped", "best_match", "exclude", "duplicate_best_match", "duplicate_ID", "match_IDs",
                  "match_status", "dataset"]
     pretty_df = (df.select(keep_cols)
                  .select(pl.exclude("^.*_right"))
                  .sort(["accession", "row_nr", "chr_name", "chr_position", "match_status"]))
     return pretty_df
```

### Comparing `pgscatalog_utils-0.3.1/pgscatalog_utils/match/match.py` & `pgscatalog_utils-0.4.0/pgscatalog_utils/match/match.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_utils-0.3.1/pgscatalog_utils/match/match_variants.py` & `pgscatalog_utils-0.4.0/pgscatalog_utils/match/match_variants.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,15 +85,15 @@
                                                   min_overlap=args.min_overlap)
 
     if filter_summary.filter(pl.col("score_pass") == True).collect().is_empty():
         # this can happen when args.min_overlap = 0
         logger.critical("Error: no target variants match any variants in scoring files")
         raise Exception("No valid matches found")
 
-    write_scorefiles(valid_matches, args.split, dataset)
+    write_scorefiles(matches=valid_matches, split=args.split, combined=args.combined, dataset=dataset)
 
     big_log: pl.LazyFrame = make_logs(scorefile=scorefile, match_candidates=matches, dataset=dataset)
     summary_log: pl.LazyFrame = make_summary_log(match_candidates=matches, filter_summary=filter_summary,
                                                  dataset=dataset,
                                                  scorefile=scorefile)
 
     check_log_count(summary_log=summary_log, scorefile=scorefile)
@@ -206,19 +206,24 @@
                         help='<Optional> Set which chromosome is in the target variant file to speed up matching ')
     parser.add_argument('-f', '--fast', dest='fast', action='store_true',
                         help='<Optional> Enable faster matching at the cost of increased RAM usage')
     parser.add_argument('--only_match', dest='only_match', action='store_true',
                         help="<Optional> Only match, then write intermediate files, don't make scoring files")
     parser.add_argument('--min_overlap', dest='min_overlap', required=False,
                         type=float, help='<Optional> Minimum proportion of variants to match before error')
+    parser.add_argument('-IDs', '--filter_IDs', dest='filter',
+                        help='<Optional> Path to file containing list of variant IDs that can be included in the final scorefile.'
+                             '[useful for limiting scoring files to variants present in multiple datasets]')
     parser = add_match_args(parser) # params for labelling matches
     parser.add_argument('--outdir', dest='outdir', required=True,
                         help='<Required> Output directory')
     parser.add_argument('--split', dest='split', default=False, action='store_true',
                         help='<Optional> Split scorefile per chromosome?')
+    parser.add_argument('--combined', dest='combined', default=False, action='store_true',
+                        help='<Optional> Write scorefiles in combined format?')
     parser.add_argument('-n', dest='n_threads', default=1, help='<Optional> n threads for matching', type=int)
     parser.add_argument('-v', '--verbose', dest='verbose', action='store_true',
                         help='<Optional> Extra logging information')
     return _check_args(parser.parse_args(args))
 
 
 def add_match_args(parser):
@@ -266,12 +271,16 @@
         sys.exit(1)
     if any([x in sys.argv for x in ['--keep_first_match', '--ignore_strand_flips',
                                     '--keep_multiallelic', '--keep_ambiguous']]):
         logger.warning("Invalid arguments: --only_match and --keep_first_match, --ignore_strand_flips,"
                         "keep_multiallelic, or keep_ambiguous")
         logger.warning("Pass these arguments to combine_matches instead")
 
+    if (args.combined is False) and (args.split is False):
+        logger.warning("No output format specified, writing to combined scoring file")
+        args.combined = True
+
     return args
 
 
 if __name__ == "__main__":
     match_variants()
```

### Comparing `pgscatalog_utils-0.3.1/pgscatalog_utils/match/preprocess.py` & `pgscatalog_utils-0.4.0/pgscatalog_utils/match/preprocess.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_utils-0.3.1/pgscatalog_utils/match/read.py` & `pgscatalog_utils-0.4.0/pgscatalog_utils/match/read.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_utils-0.3.1/pgscatalog_utils/match/tempdir.py` & `pgscatalog_utils-0.4.0/pgscatalog_utils/match/tempdir.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_utils-0.3.1/pgscatalog_utils/match/write.py` & `pgscatalog_utils-0.4.0/pgscatalog_utils/match/write.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     if os.path.exists(fout):
         logger.warning(f"Overwriting log that already exists: {fout}")
         os.remove(fout)
 
     _write_text_pgzip(df=df, sep = ',', fout=fout)
 
 
-def write_scorefiles(matches: pl.LazyFrame, split: bool, dataset: str):
+def write_scorefiles(matches: pl.LazyFrame, split: bool, combined: bool, dataset: str):
     _check_column_types(matches)
     additive: pl.LazyFrame
     dominant: pl.LazyFrame
     recessive: pl.LazyFrame
 
     # collect and cache minimum required columns
     min_cols: list[str] = ['accession', 'effect_type', 'chr_name', 'ID', 'matched_effect_allele', 'effect_weight']
@@ -45,15 +45,16 @@
 
             # 3. deduplicate
             effect_types = ['additive', 'dominant', 'recessive']
             deduped = dict(zip(effect_types, [_deduplicate_variants(x) for x in [additive, dominant, recessive]]))
 
             # 4. pivot and write!
             _write_split(deduped, chrom, dataset)
-    else:
+
+    if combined:
         # 1. split by effect type
         additive, dominant, recessive = _split_effect_type(matches)
 
         # 2. deduplicate
         effect_types = ['additive', 'dominant', 'recessive']
         deduped = dict(zip(effect_types, [_deduplicate_variants(x) for x in [additive, dominant, recessive]]))
```

### Comparing `pgscatalog_utils-0.3.1/pgscatalog_utils/scorefile/combine_scorefiles.py` & `pgscatalog_utils-0.4.0/pgscatalog_utils/scorefile/combine_scorefiles.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_utils-0.3.1/pgscatalog_utils/scorefile/effect_type.py` & `pgscatalog_utils-0.4.0/pgscatalog_utils/scorefile/effect_type.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_utils-0.3.1/pgscatalog_utils/scorefile/effect_weight.py` & `pgscatalog_utils-0.4.0/pgscatalog_utils/scorefile/effect_weight.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_utils-0.3.1/pgscatalog_utils/scorefile/genome_build.py` & `pgscatalog_utils-0.4.0/pgscatalog_utils/scorefile/genome_build.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_utils-0.3.1/pgscatalog_utils/scorefile/harmonised.py` & `pgscatalog_utils-0.4.0/pgscatalog_utils/scorefile/harmonised.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_utils-0.3.1/pgscatalog_utils/scorefile/liftover.py` & `pgscatalog_utils-0.4.0/pgscatalog_utils/scorefile/liftover.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_utils-0.3.1/pgscatalog_utils/scorefile/qc.py` & `pgscatalog_utils-0.4.0/pgscatalog_utils/scorefile/qc.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_utils-0.3.1/pgscatalog_utils/scorefile/read.py` & `pgscatalog_utils-0.4.0/pgscatalog_utils/scorefile/read.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_utils-0.3.1/pgscatalog_utils/scorefile/write.py` & `pgscatalog_utils-0.4.0/pgscatalog_utils/scorefile/write.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_utils-0.3.1/pgscatalog_utils/target.py` & `pgscatalog_utils-0.4.0/pgscatalog_utils/target.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_utils-0.3.1/pgscatalog_utils/validate/common_constants.py` & `pgscatalog_utils-0.4.0/pgscatalog_utils/validate/common_constants.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_utils-0.3.1/pgscatalog_utils/validate/formatted/validator.py` & `pgscatalog_utils-0.4.0/pgscatalog_utils/validate/formatted/validator.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_utils-0.3.1/pgscatalog_utils/validate/harmonized_position/validator.py` & `pgscatalog_utils-0.4.0/pgscatalog_utils/validate/harmonized_position/validator.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_utils-0.3.1/pgscatalog_utils/validate/helpers.py` & `pgscatalog_utils-0.4.0/pgscatalog_utils/validate/helpers.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_utils-0.3.1/pgscatalog_utils/validate/schemas.py` & `pgscatalog_utils-0.4.0/pgscatalog_utils/validate/schemas.py`

 * *Files 10% similar despite different names*

```diff
@@ -69,28 +69,28 @@
     EFFECT_DSET: Column(EFFECT_DSET, [MatchesPatternValidation(r'^[ACTGN\-]+$')], allow_empty=False),
     OTH_DSET: Column(OTH_DSET, [MatchesPatternValidation(r'^[ACTGN\-]+$')], allow_empty=True),
     LOCUS_DSET: Column(LOCUS_DSET, [CanConvertValidation(DSET_TYPES[LOCUS_DSET]), LeadingWhitespaceValidation(), TrailingWhitespaceValidation(), null_validation], allow_empty=True)
 }
 
 # Formatted validators
 FORMATTED_VALIDATORS = {k:v for k,v in GENERIC_VALIDATORS.items()}
-FORMATTED_VALIDATORS[SNP_DSET] = Column(SNP_DSET, [CanConvertValidation(DSET_TYPES[SNP_DSET]), MatchesPatternValidation(r'^(rs|HLA\-\w+\*)[0-9]+$')], allow_empty=True)
+FORMATTED_VALIDATORS[SNP_DSET] = Column(SNP_DSET, [CanConvertValidation(DSET_TYPES[SNP_DSET]), MatchesPatternValidation(r'^(\.|(rs|HLA\-\w+\*)[0-9]+)$')], allow_empty=True)
 FORMATTED_VALIDATORS[OR_DSET] = Column(OR_DSET, [CanConvertValidation(DSET_TYPES[OR_DSET]), null_validation], allow_empty=True)
 FORMATTED_VALIDATORS[HR_DSET] = Column(HR_DSET, [CanConvertValidation(DSET_TYPES[HR_DSET]), null_validation], allow_empty=True)
 FORMATTED_VALIDATORS[BETA_DSET] = Column(BETA_DSET, [CanConvertValidation(DSET_TYPES[BETA_DSET]), null_validation], allow_empty=True)
 FORMATTED_VALIDATORS[FREQ_DSET] = Column(FREQ_DSET, [CanConvertValidation(DSET_TYPES[FREQ_DSET]), null_validation], allow_empty=True)
 FORMATTED_VALIDATORS[DOSAGE_0_WEIGHT] = Column(DOSAGE_0_WEIGHT, [CanConvertValidation(DSET_TYPES[DOSAGE_0_WEIGHT]), null_validation], allow_empty=True)
 FORMATTED_VALIDATORS[DOSAGE_1_WEIGHT] = Column(DOSAGE_1_WEIGHT, [CanConvertValidation(DSET_TYPES[DOSAGE_1_WEIGHT]), null_validation], allow_empty=True)
 FORMATTED_VALIDATORS[DOSAGE_2_WEIGHT] = Column(DOSAGE_2_WEIGHT, [CanConvertValidation(DSET_TYPES[DOSAGE_2_WEIGHT]), null_validation], allow_empty=True)
 
 FORMATTED_VALIDATORS_SNP = {k:v for k,v in FORMATTED_VALIDATORS.items()}
-FORMATTED_VALIDATORS_SNP[SNP_DSET] = Column(SNP_DSET, [CanConvertValidation(DSET_TYPES[SNP_DSET]), MatchesPatternValidation(r'^(rs|HLA\-\w+\*)[0-9]+$')], allow_empty=False)
+FORMATTED_VALIDATORS_SNP[SNP_DSET] = Column(SNP_DSET, [CanConvertValidation(DSET_TYPES[SNP_DSET]), MatchesPatternValidation(r'^(\.|(rs|HLA\-\w+\*)[0-9]+)$')], allow_empty=False)
 
 FORMATTED_VALIDATORS_SNP_EMPTY = {k:v for k,v in FORMATTED_VALIDATORS.items()}
-FORMATTED_VALIDATORS_SNP_EMPTY[SNP_DSET] = Column(SNP_DSET, [CanConvertValidation(DSET_TYPES[SNP_DSET]), MatchesPatternValidation(r'^(rs[0-9]+|HLA\-\w+\*[0-9]+|nan)$')], allow_empty=False)
+FORMATTED_VALIDATORS_SNP_EMPTY[SNP_DSET] = Column(SNP_DSET, [CanConvertValidation(DSET_TYPES[SNP_DSET]), MatchesPatternValidation(r'^(rs[0-9]+|HLA\-\w+\*[0-9]+|nan|\.)$')], allow_empty=False)
 FORMATTED_VALIDATORS_SNP_EMPTY[CHR_DSET] = Column(CHR_DSET, [InListValidation(VALID_CHROMOSOMES)], allow_empty=False)
 FORMATTED_VALIDATORS_SNP_EMPTY[BP_DSET]  = Column(BP_DSET, [CanConvertValidation(DSET_TYPES[BP_DSET]), InInclusiveRangeValidation(1, 999999999)], allow_empty=False)
 
 FORMATTED_VALIDATORS_POS = {k:v for k,v in FORMATTED_VALIDATORS.items()}
 FORMATTED_VALIDATORS_POS[CHR_DSET] = Column(CHR_DSET, [InListValidation(VALID_CHROMOSOMES)], allow_empty=False)
 FORMATTED_VALIDATORS_POS[BP_DSET]  = Column(BP_DSET, [CanConvertValidation(DSET_TYPES[BP_DSET]), InInclusiveRangeValidation(1, 999999999)], allow_empty=False)
```

### Comparing `pgscatalog_utils-0.3.1/pgscatalog_utils/validate/validate_scorefile.py` & `pgscatalog_utils-0.4.0/pgscatalog_utils/validate/validate_scorefile.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_utils-0.3.1/pgscatalog_utils/validate/validator_base.py` & `pgscatalog_utils-0.4.0/pgscatalog_utils/validate/validator_base.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_utils-0.3.1/pyproject.toml` & `pgscatalog_utils-0.4.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 [tool.poetry]
 name = "pgscatalog_utils"
-version = "0.3.1"
+version = "0.4.0"
 description = "Utilities for working with PGS Catalog API and scoring files"
 homepage = "https://github.com/PGScatalog/pgscatalog_utils"
 authors = ["Benjamin Wingfield <bwingfield@ebi.ac.uk>", "Samuel Lambert <sl925@medschl.cam.ac.uk>", "Laurent Gil <lg10@sanger.ac.uk>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.scripts]
 combine_scorefiles = "pgscatalog_utils.scorefile.combine_scorefiles:combine_scorefiles"
 download_scorefiles = "pgscatalog_utils.download.download_scorefile:download_scorefile"
 match_variants = "pgscatalog_utils.match.match_variants:match_variants"
 combine_matches = "pgscatalog_utils.match.combine_matches:combine_matches"
 aggregate_scores = "pgscatalog_utils.aggregate.aggregate_scores:aggregate_scores"
 validate_scorefiles = "pgscatalog_utils.validate.validate_scorefile:validate_scorefile"
+relabel_ids = "pgscatalog_utils.relabel.relabel_ids:relabel_ids"
+ancestry_analysis = "pgscatalog_utils.ancestry.ancestry_analysis:ancestry_analysis"
+samplesheet_to_json = "pgscatalog_utils.samplesheet.check:check_samplesheet"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 numpy = "^1.23.3"
 pandas = "^1.4.3"
 pandas-schema = "^0.3.6"
 pyliftover = "^0.4"
 requests = "^2.28.1"
 jq = "^1.2.2"
-polars = "^0.14.9"
+polars = "^0.15.0"
 zstandard = "^0.18.0"
 pgzip = "^0.3.2"
+scikit-learn = "^1.2.1"
 
-[tool.poetry.dev-dependencies]
-pytest = "^7.1.2"
-pytest-cov = "^3.0.0"
-pysqlar = "^0.1.2"
+[tool.poetry.group.dev.dependencies]
+jupyter = "^1.0.0"
 memory-profiler = "^0.60.0"
-matplotlib = "^3.6.0"
+pytest = "^7.2.2"
+pytest-cov = "^4.0.0"
+matplotlib = "^3.7.1"
+seaborn = "^0.12.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pgscatalog_utils-0.3.1/setup.py` & `pgscatalog_utils-0.4.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,53 +1,63 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['pgscatalog_utils',
  'pgscatalog_utils.aggregate',
+ 'pgscatalog_utils.ancestry',
  'pgscatalog_utils.download',
  'pgscatalog_utils.match',
+ 'pgscatalog_utils.relabel',
+ 'pgscatalog_utils.samplesheet',
  'pgscatalog_utils.scorefile',
  'pgscatalog_utils.validate',
  'pgscatalog_utils.validate.formatted',
  'pgscatalog_utils.validate.harmonized_position']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['jq>=1.2.2,<2.0.0',
  'numpy>=1.23.3,<2.0.0',
  'pandas-schema>=0.3.6,<0.4.0',
  'pandas>=1.4.3,<2.0.0',
  'pgzip>=0.3.2,<0.4.0',
- 'polars>=0.14.9,<0.15.0',
+ 'polars>=0.15.0,<0.16.0',
  'pyliftover>=0.4,<0.5',
  'requests>=2.28.1,<3.0.0',
+ 'scikit-learn>=1.2.1,<2.0.0',
  'zstandard>=0.18.0,<0.19.0']
 
 entry_points = \
 {'console_scripts': ['aggregate_scores = '
                      'pgscatalog_utils.aggregate.aggregate_scores:aggregate_scores',
+                     'ancestry_analysis = '
+                     'pgscatalog_utils.ancestry.ancestry_analysis:ancestry_analysis',
                      'combine_matches = '
                      'pgscatalog_utils.match.combine_matches:combine_matches',
                      'combine_scorefiles = '
                      'pgscatalog_utils.scorefile.combine_scorefiles:combine_scorefiles',
                      'download_scorefiles = '
                      'pgscatalog_utils.download.download_scorefile:download_scorefile',
                      'match_variants = '
                      'pgscatalog_utils.match.match_variants:match_variants',
+                     'relabel_ids = '
+                     'pgscatalog_utils.relabel.relabel_ids:relabel_ids',
+                     'samplesheet_to_json = '
+                     'pgscatalog_utils.samplesheet.check:check_samplesheet',
                      'validate_scorefiles = '
                      'pgscatalog_utils.validate.validate_scorefile:validate_scorefile']}
 
 setup_kwargs = {
     'name': 'pgscatalog-utils',
-    'version': '0.3.1',
+    'version': '0.4.0',
     'description': 'Utilities for working with PGS Catalog API and scoring files',
-    'long_description': "# PGS Catalog utilities\n\n[![CI](https://github.com/PGScatalog/pgscatalog_utils/actions/workflows/main.yml/badge.svg)](https://github.com/PGScatalog/pgscatalog_utils/actions/workflows/main.yml)\n\nThis repository is a collection of useful tools for downloading and working with scoring files from the\nPGS Catalog. This is mostly used internally by the PGS Catalog Calculator ([`PGScatalog/pgsc_calc`](https://github.com/PGScatalog/pgsc_calc)); however, other users may find some of these tools helpful.\n\n## Overview\n\n* `download_scorefiles`: Download scoring files by PGS ID (accession) in genome builds GRCh37 or GRCh38\n* `combine_scorefile`: Combine multiple scoring files into a single scoring file\nin 'long' format\n* `match_variants`: Match target variants (bim or pvar files) against the output\nof `combine_scorefile` to produce scoring files for plink 2\n* `validate_scorefiles`: Check/validate that the scoring files and harmonized scoring files match the PGS Catalog scoring file formats.\n\n## Installation\n\n```\n$ pip install pgscatalog-utils\n```\n\n## Quickstart\n\n```\n$ download_scorefiles -i PGS000922 PGS001229 -o . -b GRCh37\n$ combine_scorefiles -s PGS*.txt.gz -o combined.txt \n$ match_variants -s combined.txt -t <example.pvar> --min_overlap 0.75 --outdir .\n$ validate_scorefiles -t formatted --dir <scoringfiles_directory> --log_dir <logs_directory>\n```\n\nMore details are available using the `--help` parameter.\n\n## Install from source\n\nRequirements:\n\n- python 3.10\n- [poetry](https://python-poetry.org)\n\n```\n$ git clone https://github.com/PGScatalog/pgscatalog_utils.git\n$ cd pgscatalog_utils\n$ poetry install\n$ poetry build\n$ pip install --user dist/*.whl \n```\n\n## Credits\n\nThe `pgscatalog_utils` package is developed as part of the **Polygenic Score (PGS) Catalog** \n([www.PGSCatalog.org](https://www.PGSCatalog.org)) project, a collaboration between the \nUniversity of Cambridge’s Department of Public Health and Primary Care (Michael Inouye, Samuel Lambert, Laurent Gil) \nand the European Bioinformatics Institute (Helen Parkinson, Aoife McMahon, Ben Wingfield, Laura Harris).\n\nA manuscript describing the tool and larger PGS Catalog Calculator pipeline \n[(`PGSCatalog/pgsc_calc`)](https://github.com/PGScatalog/pgsc_calc) is in preparation. In the meantime \nif you use these tools we ask you to cite the repo(s) and the paper describing the PGS Catalog resource:\n\n- >PGS Catalog utilities _(in development)_. PGS Catalog\n  Team. [https://github.com/PGScatalog/pgscatalog_utils](https://github.com/PGScatalog/pgscatalog_utils)\n- >PGS Catalog Calculator _(in development)_. PGS Catalog\n  Team. [https://github.com/PGScatalog/pgsc_calc](https://github.com/PGScatalog/pgsc_calc)\n- >Lambert _et al._ (2021) The Polygenic Score Catalog as an open database for\nreproducibility and systematic evaluation.  Nature Genetics. 53:420–425\ndoi:[10.1038/s41588-021-00783-5](https://doi.org/10.1038/s41588-021-00783-5).\n\nThis work has received funding from EMBL-EBI core funds, the Baker Institute, the University of Cambridge, \nHealth Data Research UK (HDRUK), and the European Union's Horizon 2020 research and innovation programme \nunder grant agreement No 101016775 INTERVENE.\n",
+    'long_description': "# PGS Catalog utilities\n\n[![CI](https://github.com/PGScatalog/pgscatalog_utils/actions/workflows/main.yml/badge.svg)](https://github.com/PGScatalog/pgscatalog_utils/actions/workflows/main.yml)\n[![DOI](https://zenodo.org/badge/513521373.svg)](https://zenodo.org/badge/latestdoi/513521373)\n\nThis repository is a collection of useful tools for downloading and working with scoring files from the\nPGS Catalog. This is mostly used internally by the PGS Catalog Calculator ([`PGScatalog/pgsc_calc`](https://github.com/PGScatalog/pgsc_calc)); however, other users may find some of these tools helpful.\n\n## Overview\n\n* `download_scorefiles`: Download scoring files by PGS ID (accession) in genome builds GRCh37 or GRCh38\n* `combine_scorefile`: Combine multiple scoring files into a single scoring file\nin 'long' format\n* `match_variants`: Match target variants (bim or pvar files) against the output\nof `combine_scorefile` to produce scoring files for plink 2\n* `ancestry_analysis` : use genetic PCA loadings to compare samples to population reference panels, and report PGS adjusted for these axes of genetic ancestry. The PCs will likely have been generated with [FRAPOSA (pgs catalog version)](https://github.com/PGScatalog/fraposa_pgsc)\n* `validate_scorefiles`: Check/validate that the scoring files and harmonized scoring files match the PGS Catalog scoring file formats.\n\n## Installation\n\n```\n$ pip install pgscatalog-utils\n```\n\n## Quickstart\n\n```\n$ download_scorefiles -i PGS000922 PGS001229 -o . -b GRCh37\n$ combine_scorefiles -s PGS*.txt.gz -o combined.txt \n$ match_variants -s combined.txt -t <example.pvar> --min_overlap 0.75 --outdir .\n$ validate_scorefiles -t formatted --dir <scoringfiles_directory> --log_dir <logs_directory>\n```\n\nMore details are available using the `--help` parameter.\n\n## Install from source\n\nRequirements:\n\n- python 3.10\n- [poetry](https://python-poetry.org)\n\n```\n$ git clone https://github.com/PGScatalog/pgscatalog_utils.git\n$ cd pgscatalog_utils\n$ poetry install\n$ poetry build\n$ pip install --user dist/*.whl \n```\n\n## Credits\n\nThe `pgscatalog_utils` package is developed as part of the **Polygenic Score (PGS) Catalog** \n([www.PGSCatalog.org](https://www.PGSCatalog.org)) project, a collaboration between the \nUniversity of Cambridge’s Department of Public Health and Primary Care (Michael Inouye, Samuel Lambert, Laurent Gil) \nand the European Bioinformatics Institute (Helen Parkinson, Aoife McMahon, Ben Wingfield, Laura Harris).\n\nA manuscript describing the tool and larger PGS Catalog Calculator pipeline \n[(`PGSCatalog/pgsc_calc`)](https://github.com/PGScatalog/pgsc_calc) is in preparation. In the meantime \nif you use these tools we ask you to cite the repo(s) and the paper describing the PGS Catalog resource:\n\n- >PGS Catalog utilities _(in development)_. PGS Catalog\n  Team. [https://github.com/PGScatalog/pgscatalog_utils](https://github.com/PGScatalog/pgscatalog_utils)\n- >PGS Catalog Calculator _(in development)_. PGS Catalog\n  Team. [https://github.com/PGScatalog/pgsc_calc](https://github.com/PGScatalog/pgsc_calc)\n- >Lambert _et al._ (2021) The Polygenic Score Catalog as an open database for\nreproducibility and systematic evaluation.  Nature Genetics. 53:420–425\ndoi:[10.1038/s41588-021-00783-5](https://doi.org/10.1038/s41588-021-00783-5).\n\nThis work has received funding from EMBL-EBI core funds, the Baker Institute, the University of Cambridge, \nHealth Data Research UK (HDRUK), and the European Union's Horizon 2020 research and innovation programme \nunder grant agreement No 101016775 INTERVENE.\n",
     'author': 'Benjamin Wingfield',
     'author_email': 'bwingfield@ebi.ac.uk',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/PGScatalog/pgscatalog_utils',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pgscatalog_utils-0.3.1/PKG-INFO` & `pgscatalog_utils-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgscatalog-utils
-Version: 0.3.1
+Version: 0.4.0
 Summary: Utilities for working with PGS Catalog API and scoring files
 Home-page: https://github.com/PGScatalog/pgscatalog_utils
 License: Apache-2.0
 Author: Benjamin Wingfield
 Author-email: bwingfield@ebi.ac.uk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,34 +12,37 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jq (>=1.2.2,<2.0.0)
 Requires-Dist: numpy (>=1.23.3,<2.0.0)
 Requires-Dist: pandas (>=1.4.3,<2.0.0)
 Requires-Dist: pandas-schema (>=0.3.6,<0.4.0)
 Requires-Dist: pgzip (>=0.3.2,<0.4.0)
-Requires-Dist: polars (>=0.14.9,<0.15.0)
+Requires-Dist: polars (>=0.15.0,<0.16.0)
 Requires-Dist: pyliftover (>=0.4,<0.5)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: scikit-learn (>=1.2.1,<2.0.0)
 Requires-Dist: zstandard (>=0.18.0,<0.19.0)
 Description-Content-Type: text/markdown
 
 # PGS Catalog utilities
 
 [![CI](https://github.com/PGScatalog/pgscatalog_utils/actions/workflows/main.yml/badge.svg)](https://github.com/PGScatalog/pgscatalog_utils/actions/workflows/main.yml)
+[![DOI](https://zenodo.org/badge/513521373.svg)](https://zenodo.org/badge/latestdoi/513521373)
 
 This repository is a collection of useful tools for downloading and working with scoring files from the
 PGS Catalog. This is mostly used internally by the PGS Catalog Calculator ([`PGScatalog/pgsc_calc`](https://github.com/PGScatalog/pgsc_calc)); however, other users may find some of these tools helpful.
 
 ## Overview
 
 * `download_scorefiles`: Download scoring files by PGS ID (accession) in genome builds GRCh37 or GRCh38
 * `combine_scorefile`: Combine multiple scoring files into a single scoring file
 in 'long' format
 * `match_variants`: Match target variants (bim or pvar files) against the output
 of `combine_scorefile` to produce scoring files for plink 2
+* `ancestry_analysis` : use genetic PCA loadings to compare samples to population reference panels, and report PGS adjusted for these axes of genetic ancestry. The PCs will likely have been generated with [FRAPOSA (pgs catalog version)](https://github.com/PGScatalog/fraposa_pgsc)
 * `validate_scorefiles`: Check/validate that the scoring files and harmonized scoring files match the PGS Catalog scoring file formats.
 
 ## Installation
 
 ```
 $ pip install pgscatalog-utils
 ```
```

