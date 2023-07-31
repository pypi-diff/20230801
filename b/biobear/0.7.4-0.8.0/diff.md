# Comparing `tmp/biobear-0.7.4.tar.gz` & `tmp/biobear-0.8.0.tar.gz`

## Comparing `biobear-0.7.4.tar` & `biobear-0.8.0.tar`

### file list

```diff
@@ -1,61 +1,68 @@
--rw-r--r--   0        0        0      297 1970-01-01 00:00:00.000000 biobear-0.7.4/Cargo.toml
--rw-r--r--   0     1001      123     3295 2023-07-13 15:47:50.000000 biobear-0.7.4/.github/biobear.svg
--rw-r--r--   0     1001      123      100 2023-07-13 15:47:50.000000 biobear-0.7.4/.github/dependabot.yml
--rw-r--r--   0     1001      123     2650 2023-07-13 15:47:50.000000 biobear-0.7.4/.github/workflows/release.yml
--rw-r--r--   0     1001      123      704 2023-07-13 15:47:50.000000 biobear-0.7.4/.github/workflows/smoke-test.yml
--rw-r--r--   0     1001      123      143 2023-07-13 15:47:50.000000 biobear-0.7.4/.github/workflows/smoketest.py
--rw-r--r--   0     1001      123      940 2023-07-13 15:47:50.000000 biobear-0.7.4/.github/workflows/test.yml
--rw-r--r--   0     1001      123     4135 2023-07-13 15:47:50.000000 biobear-0.7.4/.gitignore
--rw-r--r--   0     1001      123     1725 2023-07-13 15:47:50.000000 biobear-0.7.4/CHANGELOG.md
--rw-r--r--   0     1001      123     1055 2023-07-13 15:47:50.000000 biobear-0.7.4/LICENSE
--rw-r--r--   0     1001      123       68 2023-07-13 15:47:50.000000 biobear-0.7.4/Makefile
--rw-r--r--   0     1001      123     2899 2023-07-13 15:47:50.000000 biobear-0.7.4/README.md
--rw-r--r--   0     1001      123      224 2023-07-13 15:47:50.000000 biobear-0.7.4/cz.json
--rw-r--r--   0     1001      123      252 2023-07-13 15:47:50.000000 biobear-0.7.4/docs.bash
--rw-r--r--   0     1001      123      604 2023-07-13 15:47:50.000000 biobear-0.7.4/pyproject.toml
--rw-r--r--   0     1001      123     1299 2023-07-13 15:47:50.000000 biobear-0.7.4/python/biobear/__init__.py
--rw-r--r--   0     1001      123     1829 2023-07-13 15:47:50.000000 biobear-0.7.4/python/biobear/bam_reader.py
--rw-r--r--   0     1001      123     1883 2023-07-13 15:47:50.000000 biobear-0.7.4/python/biobear/bcf_reader.py
--rw-r--r--   0     1001      123     1309 2023-07-13 15:47:50.000000 biobear-0.7.4/python/biobear/compression.py
--rw-r--r--   0     1001      123     1520 2023-07-13 15:47:50.000000 biobear-0.7.4/python/biobear/fasta_reader.py
--rw-r--r--   0     1001      123     1516 2023-07-13 15:47:50.000000 biobear-0.7.4/python/biobear/fastq_reader.py
--rw-r--r--   0     1001      123      858 2023-07-13 15:47:50.000000 biobear-0.7.4/python/biobear/genbank_reader.py
--rw-r--r--   0     1001      123     1565 2023-07-13 15:47:50.000000 biobear-0.7.4/python/biobear/gff_reader.py
--rw-r--r--   0     1001      123     1566 2023-07-13 15:47:50.000000 biobear-0.7.4/python/biobear/gtf_reader.py
--rw-r--r--   0     1001      123     2338 2023-07-13 15:47:50.000000 biobear-0.7.4/python/biobear/reader.py
--rw-r--r--   0     1001      123     1887 2023-07-13 15:47:50.000000 biobear-0.7.4/python/biobear/vcf_reader.py
--rw-r--r--   0     1001      123   124562 2023-07-13 15:47:50.000000 biobear-0.7.4/python/tests/data/BGC0000404.gbk
--rw-r--r--   0     1001      123     6152 2023-07-13 15:47:50.000000 biobear-0.7.4/python/tests/data/bedcov.bam
--rw-r--r--   0     1001      123     7608 2023-07-13 15:47:50.000000 biobear-0.7.4/python/tests/data/bedcov.bam.bai
--rw-r--r--   0     1001      123     1749 2023-07-13 15:47:50.000000 biobear-0.7.4/python/tests/data/file.vcf
--rw-r--r--   0     1001      123     9521 2023-07-13 15:47:50.000000 biobear-0.7.4/python/tests/data/index.bcf
--rw-r--r--   0     1001      123      143 2023-07-13 15:47:50.000000 biobear-0.7.4/python/tests/data/index.bcf.csi
--rw-r--r--   0     1001      123     8638 2023-07-13 15:47:50.000000 biobear-0.7.4/python/tests/data/index.vcf.gz
--rw-r--r--   0     1001      123      213 2023-07-13 15:47:50.000000 biobear-0.7.4/python/tests/data/index.vcf.gz.tbi
--rw-r--r--   0     1001      123       41 2023-07-13 15:47:50.000000 biobear-0.7.4/python/tests/data/test.fasta
--rw-r--r--   0     1001      123       58 2023-07-13 15:47:50.000000 biobear-0.7.4/python/tests/data/test.fasta.gz
--rw-r--r--   0     1001      123      286 2023-07-13 15:47:50.000000 biobear-0.7.4/python/tests/data/test.fastq
--rw-r--r--   0     1001      123      134 2023-07-13 15:47:50.000000 biobear-0.7.4/python/tests/data/test.fastq.gz
--rw-r--r--   0     1001      123      112 2023-07-13 15:47:50.000000 biobear-0.7.4/python/tests/data/test.gff
--rw-r--r--   0     1001      123       91 2023-07-13 15:47:50.000000 biobear-0.7.4/python/tests/data/test.gff.gz
--rw-r--r--   0     1001      123    17994 2023-07-13 15:47:50.000000 biobear-0.7.4/python/tests/data/test.gtf
--rw-r--r--   0     1001      123     1478 2023-07-13 15:47:50.000000 biobear-0.7.4/python/tests/data/test.gtf.gz
--rw-r--r--   0     1001      123     4302 2023-07-13 15:47:50.000000 biobear-0.7.4/python/tests/data/vcf_file.vcf
--rw-r--r--   0     1001      123     1669 2023-07-13 15:47:50.000000 biobear-0.7.4/python/tests/data/vcf_file.vcf.gz
--rw-r--r--   0     1001      123      254 2023-07-13 15:47:50.000000 biobear-0.7.4/python/tests/data/vcf_file.vcf.gz.tbi
--rw-r--r--   0     1001      123      816 2023-07-13 15:47:50.000000 biobear-0.7.4/python/tests/test_bam_reader.py
--rw-r--r--   0     1001      123     1615 2023-07-13 15:47:50.000000 biobear-0.7.4/python/tests/test_bcf_reader.py
--rw-r--r--   0     1001      123     1729 2023-07-13 15:47:50.000000 biobear-0.7.4/python/tests/test_fasta_reader.py
--rw-r--r--   0     1001      123     1380 2023-07-13 15:47:50.000000 biobear-0.7.4/python/tests/test_fastq_reader.py
--rw-r--r--   0     1001      123      544 2023-07-13 15:47:50.000000 biobear-0.7.4/python/tests/test_genbank_reader.py
--rw-r--r--   0     1001      123     1575 2023-07-13 15:47:50.000000 biobear-0.7.4/python/tests/test_gff_reader.py
--rw-r--r--   0     1001      123     1583 2023-07-13 15:47:50.000000 biobear-0.7.4/python/tests/test_gtf_reader.py
--rw-r--r--   0     1001      123     1052 2023-07-13 15:47:50.000000 biobear-0.7.4/python/tests/test_vcf_reader.py
--rw-r--r--   0     1001      123       20 2023-07-13 15:47:50.000000 biobear-0.7.4/requirements-dev.txt
--rw-r--r--   0     1001      123     3389 2023-07-13 15:47:50.000000 biobear-0.7.4/src/bam_reader.rs
--rw-r--r--   0     1001      123     3226 2023-07-13 15:47:50.000000 biobear-0.7.4/src/bcf_reader.rs
--rw-r--r--   0     1001      123     4488 2023-07-13 15:47:50.000000 biobear-0.7.4/src/exon_reader.rs
--rw-r--r--   0     1001      123      977 2023-07-13 15:47:50.000000 biobear-0.7.4/src/lib.rs
--rw-r--r--   0     1001      123     3226 2023-07-13 15:47:50.000000 biobear-0.7.4/src/vcf_reader.rs
--rw-r--r--   0     1001      123    92936 2023-07-13 15:47:59.000000 biobear-0.7.4/Cargo.lock
--rw-r--r--   0        0        0     3336 1970-01-01 00:00:00.000000 biobear-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0      297 1970-01-01 00:00:00.000000 biobear-0.8.0/Cargo.toml
+-rw-r--r--   0     1001      123     3295 2023-07-31 21:16:18.000000 biobear-0.8.0/.github/biobear.svg
+-rw-r--r--   0     1001      123      100 2023-07-31 21:16:18.000000 biobear-0.8.0/.github/dependabot.yml
+-rw-r--r--   0     1001      123     2650 2023-07-31 21:16:18.000000 biobear-0.8.0/.github/workflows/release.yml
+-rw-r--r--   0     1001      123     1385 2023-07-31 21:16:18.000000 biobear-0.8.0/.github/workflows/smoke-test.yml
+-rw-r--r--   0     1001      123      143 2023-07-31 21:16:18.000000 biobear-0.8.0/.github/workflows/smoketest.py
+-rw-r--r--   0     1001      123      940 2023-07-31 21:16:18.000000 biobear-0.8.0/.github/workflows/test.yml
+-rw-r--r--   0     1001      123     4135 2023-07-31 21:16:18.000000 biobear-0.8.0/.gitignore
+-rw-r--r--   0     1001      123     1863 2023-07-31 21:16:18.000000 biobear-0.8.0/CHANGELOG.md
+-rw-r--r--   0     1001      123     1055 2023-07-31 21:16:18.000000 biobear-0.8.0/LICENSE
+-rw-r--r--   0     1001      123      211 2023-07-31 21:16:18.000000 biobear-0.8.0/Makefile
+-rw-r--r--   0     1001      123     3691 2023-07-31 21:16:18.000000 biobear-0.8.0/README.md
+-rw-r--r--   0     1001      123      393 2023-07-31 21:16:18.000000 biobear-0.8.0/benchmarks/biobear-scan.py
+-rw-r--r--   0     1001      123      467 2023-07-31 21:16:18.000000 biobear-0.8.0/benchmarks/biopython-scan.py
+-rw-r--r--   0     1001      123      979 2023-07-31 21:16:18.000000 biobear-0.8.0/benchmarks/results.json
+-rw-r--r--   0     1001      123      224 2023-07-31 21:16:18.000000 biobear-0.8.0/cz.json
+-rw-r--r--   0     1001      123      252 2023-07-31 21:16:18.000000 biobear-0.8.0/docs.bash
+-rw-r--r--   0     1001      123      548 2023-07-31 21:16:18.000000 biobear-0.8.0/pyproject.toml
+-rw-r--r--   0     1001      123     1402 2023-07-31 21:16:18.000000 biobear-0.8.0/python/biobear/__init__.py
+-rw-r--r--   0     1001      123     1829 2023-07-31 21:16:18.000000 biobear-0.8.0/python/biobear/bam_reader.py
+-rw-r--r--   0     1001      123     1883 2023-07-31 21:16:18.000000 biobear-0.8.0/python/biobear/bcf_reader.py
+-rw-r--r--   0     1001      123     1309 2023-07-31 21:16:18.000000 biobear-0.8.0/python/biobear/compression.py
+-rw-r--r--   0     1001      123     1520 2023-07-31 21:16:18.000000 biobear-0.8.0/python/biobear/fasta_reader.py
+-rw-r--r--   0     1001      123     1516 2023-07-31 21:16:18.000000 biobear-0.8.0/python/biobear/fastq_reader.py
+-rw-r--r--   0     1001      123      858 2023-07-31 21:16:18.000000 biobear-0.8.0/python/biobear/genbank_reader.py
+-rw-r--r--   0     1001      123     1565 2023-07-31 21:16:18.000000 biobear-0.8.0/python/biobear/gff_reader.py
+-rw-r--r--   0     1001      123     1566 2023-07-31 21:16:18.000000 biobear-0.8.0/python/biobear/gtf_reader.py
+-rw-r--r--   0     1001      123      779 2023-07-31 21:16:18.000000 biobear-0.8.0/python/biobear/mzml_reader.py
+-rw-r--r--   0     1001      123     2338 2023-07-31 21:16:18.000000 biobear-0.8.0/python/biobear/reader.py
+-rw-r--r--   0     1001      123     1887 2023-07-31 21:16:18.000000 biobear-0.8.0/python/biobear/vcf_reader.py
+-rw-r--r--   0     1001      123   124562 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/BGC0000404.gbk
+-rw-r--r--   0     1001      123     6152 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/bedcov.bam
+-rw-r--r--   0     1001      123     7608 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/bedcov.bam.bai
+-rw-r--r--   0     1001      123     1749 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/file.vcf
+-rw-r--r--   0     1001      123     9521 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/index.bcf
+-rw-r--r--   0     1001      123      143 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/index.bcf.csi
+-rw-r--r--   0     1001      123     8638 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/index.vcf.gz
+-rw-r--r--   0     1001      123      213 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/index.vcf.gz.tbi
+-rw-r--r--   0     1001      123       41 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/test.fasta
+-rw-r--r--   0     1001      123       58 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/test.fasta.gz
+-rw-r--r--   0     1001      123      286 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/test.fastq
+-rw-r--r--   0     1001      123      134 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/test.fastq.gz
+-rw-r--r--   0     1001      123      112 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/test.gff
+-rw-r--r--   0     1001      123       91 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/test.gff.gz
+-rw-r--r--   0     1001      123    17994 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/test.gtf
+-rw-r--r--   0     1001      123     1478 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/test.gtf.gz
+-rw-r--r--   0     1001      123    17171 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/test.mzML
+-rw-r--r--   0     1001      123     2845 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/test.mzML.gz
+-rw-r--r--   0     1001      123     4302 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/vcf_file.vcf
+-rw-r--r--   0     1001      123     1669 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/vcf_file.vcf.gz
+-rw-r--r--   0     1001      123      254 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/vcf_file.vcf.gz.tbi
+-rw-r--r--   0     1001      123      816 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/test_bam_reader.py
+-rw-r--r--   0     1001      123     1615 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/test_bcf_reader.py
+-rw-r--r--   0     1001      123     1729 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/test_fasta_reader.py
+-rw-r--r--   0     1001      123     1380 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/test_fastq_reader.py
+-rw-r--r--   0     1001      123      544 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/test_genbank_reader.py
+-rw-r--r--   0     1001      123     1576 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/test_gff_reader.py
+-rw-r--r--   0     1001      123     1583 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/test_gtf_reader.py
+-rw-r--r--   0     1001      123     1166 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/test_mzml_reader.py
+-rw-r--r--   0     1001      123     1052 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/test_vcf_reader.py
+-rw-r--r--   0     1001      123       20 2023-07-31 21:16:18.000000 biobear-0.8.0/requirements-dev.txt
+-rw-r--r--   0     1001      123     3369 2023-07-31 21:16:18.000000 biobear-0.8.0/src/bam_reader.rs
+-rw-r--r--   0     1001      123     3217 2023-07-31 21:16:18.000000 biobear-0.8.0/src/bcf_reader.rs
+-rw-r--r--   0     1001      123     4463 2023-07-31 21:16:18.000000 biobear-0.8.0/src/exon_reader.rs
+-rw-r--r--   0     1001      123      977 2023-07-31 21:16:18.000000 biobear-0.8.0/src/lib.rs
+-rw-r--r--   0     1001      123     3222 2023-07-31 21:16:18.000000 biobear-0.8.0/src/vcf_reader.rs
+-rw-r--r--   0     1001      123    92835 2023-07-31 21:16:25.000000 biobear-0.8.0/Cargo.lock
+-rw-r--r--   0        0        0     4128 1970-01-01 00:00:00.000000 biobear-0.8.0/PKG-INFO
```

### Comparing `biobear-0.7.4/.github/biobear.svg` & `biobear-0.8.0/.github/biobear.svg`

 * *Files identical despite different names*

### Comparing `biobear-0.7.4/.github/workflows/release.yml` & `biobear-0.8.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `biobear-0.7.4/.github/workflows/test.yml` & `biobear-0.8.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `biobear-0.7.4/.gitignore` & `biobear-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `biobear-0.7.4/CHANGELOG.md` & `biobear-0.8.0/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+## v0.8.0 (2023-07-31)
+
+### Feat
+
+- update exon for faster scans (#50)
+- add conda forge to bb test (#48)
+- IC for mzml in biobear (#46)
+
 ## v0.7.4 (2023-07-13)
 
 ## v0.7.3 (2023-07-13)
 
 ## v0.7.2 (2023-07-13)
 
 ## v0.7.1 (2023-07-11)
```

### Comparing `biobear-0.7.4/LICENSE` & `biobear-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biobear-0.7.4/pyproject.toml` & `biobear-0.8.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -14,15 +14,10 @@
 dependencies = ["pyarrow>=12"]
 
 license = {file = "LICENSE"}
 name = "biobear"
 readme = "README.md"
 requires-python = ">=3.8"
 
-[tool.poetry.extras]
-polars = [
-  "polars>=0.18,<1",
-]
-
 [tool.maturin]
 features = ["pyo3/extension-module"]
 python-source = "python"
```

### Comparing `biobear-0.7.4/python/biobear/__init__.py` & `biobear-0.8.0/python/biobear/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,26 +16,31 @@
 
 from biobear.fasta_reader import FastaReader
 from biobear.fastq_reader import FastqReader
 from biobear.vcf_reader import VCFReader, VCFIndexedReader
 from biobear.bam_reader import BamReader, BamIndexedReader
 from biobear.gtf_reader import GTFReader
 from biobear.gff_reader import GFFReader
+from biobear.mzml_reader import MzMLReader
 from biobear.genbank_reader import GenbankReader
 from biobear.bcf_reader import BCFReader, BCFIndexedReader
 
 from biobear import compression
 
+__version__ = "0.7.4"
+
 __all__ = [
     "FastaReader",
     "FastqReader",
     "VCFReader",
     "VCFIndexedReader",
     "BamReader",
     "BamIndexedReader",
     "BCFReader",
     "BCFIndexedReader",
     "GFFReader",
     "GTFReader",
     "GenbankReader",
+    "MzMLReader",
     "compression",
+    "__version__",
 ]
```

### Comparing `biobear-0.7.4/python/biobear/bam_reader.py` & `biobear-0.8.0/python/biobear/bam_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.4/python/biobear/bcf_reader.py` & `biobear-0.8.0/python/biobear/bcf_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.4/python/biobear/compression.py` & `biobear-0.8.0/python/biobear/compression.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.4/python/biobear/fasta_reader.py` & `biobear-0.8.0/python/biobear/fasta_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.4/python/biobear/fastq_reader.py` & `biobear-0.8.0/python/biobear/fastq_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.4/python/biobear/genbank_reader.py` & `biobear-0.8.0/python/biobear/genbank_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.4/python/biobear/gff_reader.py` & `biobear-0.8.0/python/biobear/gff_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.4/python/biobear/gtf_reader.py` & `biobear-0.8.0/python/biobear/gtf_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.4/python/biobear/reader.py` & `biobear-0.8.0/python/biobear/reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.4/python/biobear/vcf_reader.py` & `biobear-0.8.0/python/biobear/vcf_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.4/python/tests/data/BGC0000404.gbk` & `biobear-0.8.0/python/tests/data/BGC0000404.gbk`

 * *Files identical despite different names*

### Comparing `biobear-0.7.4/python/tests/data/bedcov.bam` & `biobear-0.8.0/python/tests/data/bedcov.bam`

 * *Files identical despite different names*

### Comparing `biobear-0.7.4/python/tests/data/bedcov.bam.bai` & `biobear-0.8.0/python/tests/data/bedcov.bam.bai`

 * *Files identical despite different names*

### Comparing `biobear-0.7.4/python/tests/data/file.vcf` & `biobear-0.8.0/python/tests/data/file.vcf`

 * *Files identical despite different names*

### Comparing `biobear-0.7.4/python/tests/data/index.bcf` & `biobear-0.8.0/python/tests/data/index.bcf`

 * *Files identical despite different names*

### Comparing `biobear-0.7.4/python/tests/data/index.vcf.gz` & `biobear-0.8.0/python/tests/data/index.vcf.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.7.4/python/tests/data/test.gtf` & `biobear-0.8.0/python/tests/data/test.gtf`

 * *Files identical despite different names*

### Comparing `biobear-0.7.4/python/tests/data/test.gtf.gz` & `biobear-0.8.0/python/tests/data/test.gtf.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.7.4/python/tests/data/vcf_file.vcf` & `biobear-0.8.0/python/tests/data/vcf_file.vcf`

 * *Files identical despite different names*

### Comparing `biobear-0.7.4/python/tests/data/vcf_file.vcf.gz` & `biobear-0.8.0/python/tests/data/vcf_file.vcf.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.7.4/python/tests/test_bam_reader.py` & `biobear-0.8.0/python/tests/test_bam_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.4/python/tests/test_bcf_reader.py` & `biobear-0.8.0/python/tests/test_bcf_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.4/python/tests/test_fasta_reader.py` & `biobear-0.8.0/python/tests/test_fasta_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.4/python/tests/test_fastq_reader.py` & `biobear-0.8.0/python/tests/test_fastq_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.4/python/tests/test_genbank_reader.py` & `biobear-0.8.0/python/tests/test_genbank_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.4/python/tests/test_gff_reader.py` & `biobear-0.8.0/python/tests/test_gff_reader.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,28 +27,28 @@
     import polars as pl
 
     reader = GFFReader(DATA / "test.gff")
     df = reader.to_polars()
     dtype = df.select(pl.col("attributes")).dtypes[0]
 
     key_field = pl.Field("key", pl.Utf8)
-    value_field = pl.Field("value", pl.Utf8)
+    value_field = pl.Field("value", pl.List(pl.Utf8))
     assert dtype == pl.List(pl.Struct([key_field, value_field]))
 
 
 def test_gff_reader_to_scanner():
     reader = GFFReader(DATA / "test.gff")
     scanner = reader.to_arrow_scanner()
 
     assert scanner.count_rows() == 2
 
 
 def test_gff_reader_no_file():
     with pytest.raises(OSError):
-        GFFReader("test.gff")
+        GFFReader("")
 
 
 @pytest.mark.skipif(
     not importlib.util.find_spec("polars"), reason="polars not installed"
 )
 def test_gff_reader_gz():
     reader = GFFReader(DATA / "test.gff.gz")
```

### Comparing `biobear-0.7.4/python/tests/test_gtf_reader.py` & `biobear-0.8.0/python/tests/test_gtf_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.4/python/tests/test_vcf_reader.py` & `biobear-0.8.0/python/tests/test_vcf_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.7.4/src/bam_reader.rs` & `biobear-0.8.0/src/bam_reader.rs`

 * *Files 7% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 use arrow::ffi_stream::ArrowArrayStreamReader;
 use arrow::ffi_stream::FFI_ArrowArrayStream;
 use arrow::pyarrow::IntoPyArrow;
-use datafusion::prelude::SessionConfig;
 use datafusion::prelude::SessionContext;
-use exon::context::ExonSessionExt;
 use exon::ffi::create_dataset_stream_from_table_provider;
+use exon::new_exon_config;
+use exon::ExonSessionExt;
 use pyo3::prelude::*;
 
 use tokio::runtime::Runtime;
 
 use std::io;
 use std::sync::Arc;
 
@@ -61,20 +61,20 @@
             PyErr::new::<pyo3::exceptions::PyIOError, _>(format!(
                 "Failed to open file: {path} with error: {e}"
             ))
         })
     }
 
     fn query(&mut self, region: &str) -> PyResult<PyObject> {
-        let mut config = SessionConfig::new();
+        let mut config = new_exon_config();
         if let Some(batch_size) = self.batch_size {
             config = config.with_batch_size(batch_size);
         }
 
-        let ctx = SessionContext::with_config(config);
+        let ctx = SessionContext::with_config_exon(config);
 
         let df = self._runtime.block_on(async {
             match ctx.query_bam_file(self.path.as_str(), region).await {
                 Ok(df) => Ok(df),
                 Err(e) => Err(io::Error::new(
                     io::ErrorKind::Other,
                     format!("Error reading GFF file: {e}"),
```

### Comparing `biobear-0.7.4/src/bcf_reader.rs` & `biobear-0.8.0/src/bcf_reader.rs`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 use arrow::ffi_stream::{ArrowArrayStreamReader, FFI_ArrowArrayStream};
 use arrow::pyarrow::IntoPyArrow;
 use datafusion::prelude::{SessionConfig, SessionContext};
 use pyo3::prelude::*;
 use tokio::runtime::Runtime;
 
-use exon::{context::ExonSessionExt, ffi::create_dataset_stream_from_table_provider};
+use exon::{ffi::create_dataset_stream_from_table_provider, ExonSessionExt};
 
 use std::io;
 use std::sync::Arc;
 
 #[pyclass(name = "_BCFIndexedReader")]
 pub struct BCFIndexedReader {
     path: String,
```

### Comparing `biobear-0.7.4/src/exon_reader.rs` & `biobear-0.8.0/src/exon_reader.rs`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,17 @@
 use std::str::FromStr;
 use std::sync::Arc;
 
 use arrow::ffi_stream::{ArrowArrayStreamReader, FFI_ArrowArrayStream};
 use arrow::pyarrow::IntoPyArrow;
 use datafusion::datasource::file_format::file_type::FileCompressionType;
 use datafusion::prelude::{SessionConfig, SessionContext};
-use exon::context::ExonSessionExt;
 use exon::datasources::ExonFileType;
 use exon::ffi::create_dataset_stream_from_table_provider;
-use exon::runtime_env::ExonRuntimeEnvExt;
+use exon::{ExonRuntimeEnvExt, ExonSessionExt};
 use pyo3::prelude::*;
 use tokio::runtime::Runtime;
 
 #[pyclass(name = "_ExonReader")]
 pub struct ExonReader {
     df: datafusion::dataframe::DataFrame,
     exhausted: bool,
@@ -44,15 +43,15 @@
         let rt = Arc::new(Runtime::new().unwrap());
 
         let mut config = SessionConfig::new();
         if let Some(batch_size) = batch_size {
             config = config.with_batch_size(batch_size);
         }
 
-        let ctx = SessionContext::with_config(config);
+        let ctx = SessionContext::with_config_exon(config);
 
         let df = rt.block_on(async {
             ctx.runtime_env()
                 .exon_register_object_store_uri(path)
                 .await?;
 
             match ctx.read_exon_table(path, file_type, compression).await {
```

### Comparing `biobear-0.7.4/src/lib.rs` & `biobear-0.8.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.7.4/src/vcf_reader.rs` & `biobear-0.8.0/src/vcf_reader.rs`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 use arrow::ffi_stream::{ArrowArrayStreamReader, FFI_ArrowArrayStream};
 use arrow::pyarrow::IntoPyArrow;
 use datafusion::prelude::{SessionConfig, SessionContext};
 use pyo3::prelude::*;
 use tokio::runtime::Runtime;
 
-use exon::{context::ExonSessionExt, ffi::create_dataset_stream_from_table_provider};
+use exon::{ffi::create_dataset_stream_from_table_provider, ExonSessionExt};
 
 use std::io;
 use std::sync::Arc;
 
 #[pyclass(name = "_VCFIndexedReader")]
 pub struct VCFIndexedReader {
     path: String,
@@ -59,15 +59,15 @@
 
     fn query(&mut self, region: &str) -> PyResult<PyObject> {
         let mut config = SessionConfig::new();
         if let Some(batch_size) = self.batch_size {
             config = config.with_batch_size(batch_size);
         }
 
-        let ctx = SessionContext::with_config(config);
+        let ctx = SessionContext::with_config_exon(config);
 
         let df = self._runtime.block_on(async {
             match ctx.query_vcf_file(self.path.as_str(), region).await {
                 Ok(df) => Ok(df),
                 Err(e) => Err(io::Error::new(
                     io::ErrorKind::Other,
                     format!("Error reading VCF file: {e}"),
```

### Comparing `biobear-0.7.4/Cargo.lock` & `biobear-0.8.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -52,17 +52,17 @@
 checksum = "94fb8275041c72129eb51b7d0322c29b8387a0386127718b096429201a5d6ece"
 dependencies = [
  "alloc-no-stdlib",
 ]
 
 [[package]]
 name = "allocator-api2"
-version = "0.2.15"
+version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "56fc6cf8dc8c4158eed8649f9b8b0ea1518eb62b544fe9490d66fa0b349eafe9"
+checksum = "0942ffc6dcaadf03badf6e6a2d0228460359d5e34b57ccdc720b7382dfbd5ec5"
 
 [[package]]
 name = "android-tzdata"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
 
@@ -85,17 +85,17 @@
 name = "arrayvec"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "96d30a06541fbafbc7f82ed10c06164cfbd2c401138f6addd8404629c4b16711"
 
 [[package]]
 name = "arrow"
-version = "42.0.0"
+version = "43.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "773d18d72cd290f3f9e2149a714c8ac404b6c3fd614c684f0015449940fca899"
+checksum = "2feeebd77b34b0bc88f224e06d01c27da4733997cc4789a4e056196656cdc59a"
 dependencies = [
  "ahash",
  "arrow-arith",
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-csv",
@@ -108,59 +108,59 @@
  "arrow-select",
  "arrow-string",
  "pyo3",
 ]
 
 [[package]]
 name = "arrow-arith"
-version = "42.0.0"
+version = "43.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93bc0da4b22ba63807fa2a74998e21209179c93c67856ae65d9218b81f3ef918"
+checksum = "7173f5dc49c0ecb5135f52565af33afd3fdc9a12d13bd6f9973e8b96305e4b2e"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "chrono",
  "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-array"
-version = "42.0.0"
+version = "43.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ea9a0fd21121304cad96f307c938d861cb1e7f0c151b93047462cd9817d760fb"
+checksum = "63d7ea725f7d1f8bb2cffc53ef538557e95fc802e217d5be25122d402e22f3d0"
 dependencies = [
  "ahash",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "chrono",
  "chrono-tz",
  "half",
  "hashbrown 0.14.0",
  "num",
 ]
 
 [[package]]
 name = "arrow-buffer"
-version = "42.0.0"
+version = "43.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "30ce342ecf5971004e23cef8b5fb3bacd2bbc48a381464144925074e1472e9eb"
+checksum = "bdbe439e077f484e5000b9e1d47b5e4c0d15f2b311a8f5bcc682553d5d67a722"
 dependencies = [
  "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-cast"
-version = "42.0.0"
+version = "43.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4b94a0ce7d27abbb02e2ee4db770f593127610f57b32625b0bc6a1a90d65f085"
+checksum = "93913cc14875770aa1eef5e310765e855effa352c094cb1c7c00607d0f37b4e1"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "arrow-select",
  "chrono",
@@ -168,17 +168,17 @@
  "half",
  "lexical-core",
  "num",
 ]
 
 [[package]]
 name = "arrow-csv"
-version = "42.0.0"
+version = "43.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f3be10a00a43c4bf0d243c070754ebdde17c5d576b4928d9c3efbe3005a3853"
+checksum = "ef55b67c55ed877e6fe7b923121c19dae5e31ca70249ea2779a17b58fb0fbd9a"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-data",
  "arrow-schema",
  "chrono",
@@ -187,121 +187,122 @@
  "lazy_static",
  "lexical-core",
  "regex",
 ]
 
 [[package]]
 name = "arrow-data"
-version = "42.0.0"
+version = "43.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d9a83dad6a53d6907765106d3bc61d6d9d313cfe1751701b3ef0948e7283dc2"
+checksum = "d4f4f4a3c54614126a71ab91f6631c9743eb4643d6e9318b74191da9dc6e028b"
 dependencies = [
  "arrow-buffer",
  "arrow-schema",
  "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-ipc"
-version = "42.0.0"
+version = "43.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a46da5e438a854e0386b38774da88a98782c0973c6dbc5c949ca4e02faf9b016"
+checksum = "d41a3659f984a524ef1c2981d43747b24d8eec78e2425267fcd0ef34ce71cd18"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-data",
  "arrow-schema",
  "flatbuffers",
 ]
 
 [[package]]
 name = "arrow-json"
-version = "42.0.0"
+version = "43.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d5f27a1fbc76553ad92dc1a9583e56b7058d8c418c4089b0b689f5b87e2da5e1"
+checksum = "10b95faa95a378f56ef32d84cc0104ea998c39ef7cd1faaa6b4cebf8ea92846d"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-data",
  "arrow-schema",
  "chrono",
  "half",
- "indexmap 1.9.3",
+ "indexmap 2.0.0",
  "lexical-core",
  "num",
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "arrow-ord"
-version = "42.0.0"
+version = "43.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f2373661f6c2233e18f6fa69c40999a9440231d1e8899be8bbbe73c7e24aa3b4"
+checksum = "c68549a4284d9f8b39586afb8d5ff8158b8f0286353a4844deb1d11cf1ba1f26"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "arrow-select",
  "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-row"
-version = "42.0.0"
+version = "43.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "377cd5158b7de4034a175e296726c40c3236e65d71d90a5dab2fb4fab526a8f4"
+checksum = "0a75a4a757afc301ce010adadff54d79d66140c4282ed3de565f6ccb716a5cf3"
 dependencies = [
  "ahash",
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "half",
  "hashbrown 0.14.0",
 ]
 
 [[package]]
 name = "arrow-schema"
-version = "42.0.0"
+version = "43.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba9ed245bd2d7d97ad1457cb281d4296e8b593588758b8fec6d67b2b2b0f2265"
+checksum = "2bebcb57eef570b15afbcf2d07d813eb476fde9f6dd69c81004d6476c197e87e"
 dependencies = [
  "bitflags 2.3.3",
 ]
 
 [[package]]
 name = "arrow-select"
-version = "42.0.0"
+version = "43.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0dc9bd6aebc565b1d04bae64a0f4dda3abc677190eb7d960471b1b20e1cebed0"
+checksum = "f6e2943fa433a48921e914417173816af64eef61c0a3d448280e6c40a62df221"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "num",
 ]
 
 [[package]]
 name = "arrow-string"
-version = "42.0.0"
+version = "43.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23cf2baea2ef53787332050decf7d71aca836a352e188c8ad062892405955d2b"
+checksum = "bbc92ed638851774f6d7af1ad900b92bc1486746497511868b4298fcbcfa35af"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "arrow-select",
+ "num",
  "regex",
  "regex-syntax",
 ]
 
 [[package]]
 name = "async-compression"
 version = "0.4.1"
@@ -318,21 +319,21 @@
  "xz2",
  "zstd",
  "zstd-safe",
 ]
 
 [[package]]
 name = "async-trait"
-version = "0.1.71"
+version = "0.1.72"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a564d521dd56509c4c47480d00b80ee55f7e385ae48db5744c67ad50c92d2ebf"
+checksum = "cc6dde6e4ed435a4c1ee4e73592f5ba9da2151af10076cc04858746af9352d09"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.25",
+ "syn 2.0.28",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
@@ -351,15 +352,15 @@
  "aws-smithy-client",
  "aws-smithy-http",
  "aws-smithy-http-tower",
  "aws-smithy-json",
  "aws-smithy-types",
  "aws-types",
  "bytes",
- "fastrand",
+ "fastrand 1.9.0",
  "hex",
  "http",
  "hyper",
  "ring",
  "time",
  "tokio",
  "tower",
@@ -371,15 +372,15 @@
 name = "aws-credential-types"
 version = "0.55.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fcdb2f7acbc076ff5ad05e7864bdb191ca70a6fd07668dc3a1a8bcd051de5ae"
 dependencies = [
  "aws-smithy-async",
  "aws-smithy-types",
- "fastrand",
+ "fastrand 1.9.0",
  "tokio",
  "tracing",
  "zeroize",
 ]
 
 [[package]]
 name = "aws-endpoint"
@@ -517,15 +518,15 @@
 checksum = "0a86aa6e21e86c4252ad6a0e3e74da9617295d8d6e374d552be7d3059c41cedd"
 dependencies = [
  "aws-smithy-async",
  "aws-smithy-http",
  "aws-smithy-http-tower",
  "aws-smithy-types",
  "bytes",
- "fastrand",
+ "fastrand 1.9.0",
  "http",
  "http-body",
  "hyper",
  "hyper-rustls 0.23.2",
  "lazy_static",
  "pin-project-lite",
  "rustls 0.20.8",
@@ -656,15 +657,15 @@
 dependencies = [
  "outref",
  "vsimd",
 ]
 
 [[package]]
 name = "biobear"
-version = "0.7.4"
+version = "0.8.0"
 dependencies = [
  "arrow",
  "datafusion",
  "exon",
  "pyo3",
  "tokio",
 ]
@@ -985,17 +986,17 @@
  "lock_api",
  "once_cell",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "datafusion"
-version = "27.0.0"
+version = "28.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e96f6e4eb10bd3e6b709686858246466983e8c5354a928ff77ee34919aa60d00"
+checksum = "5ddbcb2dda5b5033537457992ebde78938014390b2b19f9f4282e3be0e18b0c3"
 dependencies = [
  "ahash",
  "arrow",
  "arrow-array",
  "arrow-schema",
  "async-compression",
  "async-trait",
@@ -1004,21 +1005,21 @@
  "chrono",
  "dashmap",
  "datafusion-common",
  "datafusion-execution",
  "datafusion-expr",
  "datafusion-optimizer",
  "datafusion-physical-expr",
- "datafusion-row",
  "datafusion-sql",
  "flate2",
  "futures",
  "glob",
+ "half",
  "hashbrown 0.14.0",
- "indexmap 1.9.3",
+ "indexmap 2.0.0",
  "itertools 0.11.0",
  "lazy_static",
  "log",
  "num_cpus",
  "object_store",
  "parking_lot",
  "parquet",
@@ -1034,32 +1035,32 @@
  "uuid",
  "xz2",
  "zstd",
 ]
 
 [[package]]
 name = "datafusion-common"
-version = "27.0.0"
+version = "28.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "00e5fddcc0dd49bbe199e43aa406f39c46c790bb2a43c7b36a478e5f3f971235"
+checksum = "85fbb7b4da925031311743ab96662d55f0f7342d3692744f184f99b2257ef435"
 dependencies = [
  "arrow",
  "arrow-array",
  "chrono",
  "num_cpus",
  "object_store",
  "parquet",
  "sqlparser",
 ]
 
 [[package]]
 name = "datafusion-execution"
-version = "27.0.0"
+version = "28.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cfd50b6cb17acc78d2473c0d28014b8fd4e2e0a2c067c07645d6547b33b0aeeb"
+checksum = "5bb3617466d894eb0ad11d06bab1e6e89c571c0a27d660685d327d0c6e1e1ccd"
 dependencies = [
  "dashmap",
  "datafusion-common",
  "datafusion-expr",
  "hashbrown 0.14.0",
  "log",
  "object_store",
@@ -1067,32 +1068,32 @@
  "rand",
  "tempfile",
  "url",
 ]
 
 [[package]]
 name = "datafusion-expr"
-version = "27.0.0"
+version = "28.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1a35dc2cd9eac18063d636f7ddf4f090fe1f34284d80192ac7ade38cc3c6991"
+checksum = "3bd8220a0dfcdfddcc785cd7e71770ef1ce54fbe1e08984e5adf537027ecb6de"
 dependencies = [
  "ahash",
  "arrow",
  "datafusion-common",
  "lazy_static",
  "sqlparser",
  "strum 0.25.0",
  "strum_macros 0.25.1",
 ]
 
 [[package]]
 name = "datafusion-optimizer"
-version = "27.0.0"
+version = "28.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5f5043afeb45ec1c0f45519e1eed6a477f2d30732e8f975d9cf9a75fba0ca716"
+checksum = "1d685a100c66952aaadd0cbe766df46d1887d58fc8bcf3589e6387787f18492b"
 dependencies = [
  "arrow",
  "async-trait",
  "chrono",
  "datafusion-common",
  "datafusion-expr",
  "datafusion-physical-expr",
@@ -1100,72 +1101,68 @@
  "itertools 0.11.0",
  "log",
  "regex-syntax",
 ]
 
 [[package]]
 name = "datafusion-physical-expr"
-version = "27.0.0"
+version = "28.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6cc892a24f4b829ee7718ad3950884c0346dbdf1517f3df153af4bcf54d8ca4d"
+checksum = "0f2c635da9b05b4b4c6c8d935f46fd99f9b6225f834091cf4e3c8a045b68beab"
 dependencies = [
  "ahash",
  "arrow",
  "arrow-array",
  "arrow-buffer",
  "arrow-schema",
+ "base64",
  "blake2",
  "blake3",
  "chrono",
  "datafusion-common",
  "datafusion-expr",
- "datafusion-row",
  "half",
  "hashbrown 0.14.0",
- "indexmap 1.9.3",
+ "hex",
+ "indexmap 2.0.0",
  "itertools 0.11.0",
  "lazy_static",
  "libc",
+ "log",
  "md-5",
  "paste",
  "petgraph",
  "rand",
  "regex",
  "sha2",
  "unicode-segmentation",
  "uuid",
 ]
 
 [[package]]
-name = "datafusion-row"
-version = "27.0.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ce75c660bbddfdd254109e668e5b5bd69df31ea26e3768e15cef0c68015e650e"
-dependencies = [
- "arrow",
- "datafusion-common",
- "paste",
- "rand",
-]
-
-[[package]]
 name = "datafusion-sql"
-version = "27.0.0"
+version = "28.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "49cab87e4933a452e0b7b3f0cbd0e760daf7d33fb54d09d70d3ffba229eaa652"
+checksum = "b3ef8abf4dd84d3f20c910822b52779c035ab7f4f2d5e7125ede3bae618e9de8"
 dependencies = [
  "arrow",
  "arrow-schema",
  "datafusion-common",
  "datafusion-expr",
  "log",
  "sqlparser",
 ]
 
 [[package]]
+name = "deranged"
+version = "0.3.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8810e7e2cf385b1e9b50d68264908ec367ba642c96d02edfe61c39e88e2a3c01"
+
+[[package]]
 name = "digest"
 version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
 dependencies = [
  "block-buffer",
  "crypto-common",
@@ -1176,17 +1173,17 @@
 name = "doc-comment"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fea41bba32d969b513997752735605054bc0dfa92b4c56bf1189f2e174be7a10"
 
 [[package]]
 name = "either"
-version = "1.8.1"
+version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
+checksum = "a26ae43d7bcc3b814de94796a5e736d4029efb0ee900c12e2d54c993ad1a1e07"
 
 [[package]]
 name = "encoding_rs"
 version = "0.8.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "071a31f4ee85403370b58aca746f01041ede6f0da2730960ad001edc2b71b394"
 dependencies = [
@@ -1211,17 +1208,17 @@
  "rustversion",
  "syn 1.0.109",
  "synstructure",
 ]
 
 [[package]]
 name = "errno"
-version = "0.3.1"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
+checksum = "6b30f669a7961ef1631673d2766cc92f52d64f7ef354d4fe0ddfd30ed52f0f4f"
 dependencies = [
  "errno-dragonfly",
  "libc",
  "windows-sys",
 ]
 
 [[package]]
@@ -1232,33 +1229,35 @@
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
 name = "exon"
-version = "0.2.5"
+version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e4de1173112b783f139d84209b8b0d92be65365bda4e2d52941d81b133de96d"
+checksum = "b1bb7a7f30bdac3a5c4a9731315ba8de047316c2db70eb87f98adfb3ae45d1b5"
 dependencies = [
  "arrow",
  "async-trait",
  "aws-config",
  "aws-credential-types",
  "base64",
  "byteorder",
  "bytes",
  "datafusion",
  "flate2",
  "futures",
  "gb-io",
  "noodles",
+ "num_cpus",
  "object_store",
+ "parking_lot",
  "pin-project",
- "quick-xml 0.29.0",
+ "quick-xml 0.30.0",
  "serde",
  "tokio",
  "tokio-util",
  "url",
 ]
 
 [[package]]
@@ -1267,14 +1266,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e51093e27b0797c359783294ca4f0a911c270184cb10f85783b118614a1501be"
 dependencies = [
  "instant",
 ]
 
 [[package]]
+name = "fastrand"
+version = "2.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6999dc1837253364c2ebb0704ba97994bd874e8f195d665c50b7548f6ea92764"
+
+[[package]]
 name = "fixedbitset"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ce7134b9999ecaf8bcd65542e436736ef32ddca1b3e06094cb6ec5755203b80"
 
 [[package]]
 name = "flatbuffers"
@@ -1363,15 +1368,15 @@
 name = "futures-macro"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.25",
+ "syn 2.0.28",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
@@ -1687,25 +1692,14 @@
 [[package]]
 name = "integer-encoding"
 version = "3.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8bb03732005da905c88227371639bf1ad885cc712789c011c31c5fb3ab3ccf02"
 
 [[package]]
-name = "io-lifetimes"
-version = "1.0.11"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
-dependencies = [
- "hermit-abi",
- "libc",
- "windows-sys",
-]
-
-[[package]]
 name = "ipnet"
 version = "2.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "28b29a3cd74f0f4598934efe3aeba42bae0eb4680554128851ebbecb02af14e6"
 
 [[package]]
 name = "itertools"
@@ -1723,17 +1717,17 @@
 checksum = "b1c173a5686ce8bfa551b3563d0c2170bf24ca44da99c7ca4bfdab5418c3fe57"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b02a5381cc465bd3041d84623d0fa3b66738b52b8e2fc3bab8ad63ab032f4a"
+checksum = "af150ab688ff2122fcef229be89cb50dd66af9e01a4ff320cc137eecc9bacc38"
 
 [[package]]
 name = "jobserver"
 version = "0.1.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "936cfd212a0155903bcbc060e316fb6cc7cbf2e1907329391ebadc1fe0ce77c2"
 dependencies = [
@@ -1829,17 +1823,17 @@
 name = "libm"
 version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f7012b1bbb0719e1097c47611d3898568c546d597c2e74d66f6087edd5233ff4"
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.3.8"
+version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
+checksum = "09fc20d2ca12cb9f044c93e3bd6d32d523e6e2ec3db4f7b2939cd99026ecd3f0"
 
 [[package]]
 name = "lock_api"
 version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
@@ -1964,17 +1958,17 @@
 dependencies = [
  "memchr",
  "minimal-lexical",
 ]
 
 [[package]]
 name = "noodles"
-version = "0.44.0"
+version = "0.46.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "57213e65425cd2be8923d39ad3cd13c0847949dc9ed3e1bef73f2733d84c0570"
+checksum = "b7375dbfcd8a0f37bc8f9ac105614bc821860ed1bc085d2b2b0b4025fd8375c6"
 dependencies = [
  "noodles-bam",
  "noodles-bcf",
  "noodles-bed",
  "noodles-bgzf",
  "noodles-core",
  "noodles-cram",
@@ -1986,17 +1980,17 @@
  "noodles-sam",
  "noodles-tabix",
  "noodles-vcf",
 ]
 
 [[package]]
 name = "noodles-bam"
-version = "0.38.0"
+version = "0.40.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7fe7adec46a8667c07fa94df7e85994a41b1c03f04e03302629d9024691b2505"
+checksum = "719973d977642a2e7ff85770e14a9d0b3d53810caad12589369da23dc713e76d"
 dependencies = [
  "bit-vec",
  "byteorder",
  "bytes",
  "futures",
  "noodles-bgzf",
  "noodles-core",
@@ -2050,17 +2044,17 @@
 name = "noodles-core"
 version = "0.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94fbe3192fe33acacabaedd387657f39b0fc606f1996d546db0dfe14703b843a"
 
 [[package]]
 name = "noodles-cram"
-version = "0.35.0"
+version = "0.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6fd08805b7505def607baea746f79ed4138f796cc9de8d665c7c34c8c011ae05"
+checksum = "c1758a42f8b3063267f09d56116209028f2a542509dacd4da3332d20374ca9eb"
 dependencies = [
  "async-compression",
  "bitflags 2.3.3",
  "byteorder",
  "bytes",
  "bzip2",
  "flate2",
@@ -2087,17 +2081,17 @@
  "noodles-bgzf",
  "noodles-core",
  "tokio",
 ]
 
 [[package]]
 name = "noodles-fasta"
-version = "0.25.0"
+version = "0.27.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e096096e1c04ab76fe034ea499c692d8a4401a321155b542cd8ea3b1f7d08d12"
+checksum = "a8af3e2fd41a831ab9fbbbd33ce00ab2c1299d6548c13ffc30152ede4d10f6ea"
 dependencies = [
  "bytes",
  "memchr",
  "noodles-bgzf",
  "noodles-core",
  "tokio",
 ]
@@ -2111,18 +2105,19 @@
  "futures",
  "memchr",
  "tokio",
 ]
 
 [[package]]
 name = "noodles-gff"
-version = "0.16.0"
+version = "0.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "112d886335b986e5716de8c02291565813fd3be65053e3f5774b95399434af4f"
+checksum = "29cd6131bf39317a7b222eab0e99f3a14559e02a2a8c22e6160f66d17a513b74"
 dependencies = [
+ "indexmap 2.0.0",
  "noodles-bgzf",
  "noodles-core",
  "noodles-csi",
  "percent-encoding",
 ]
 
 [[package]]
@@ -2134,17 +2129,17 @@
  "noodles-bgzf",
  "noodles-core",
  "noodles-csi",
 ]
 
 [[package]]
 name = "noodles-sam"
-version = "0.35.0"
+version = "0.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "40acd01b9fa3935af0c2623ff6c8709c19fe45c0d63bd32931d2cf9939dc690c"
+checksum = "174066f6273cca871327768b20b2ce9b44bca09b020b240852b16789b324199e"
 dependencies = [
  "bitflags 2.3.3",
  "futures",
  "indexmap 2.0.0",
  "lexical-core",
  "memchr",
  "noodles-bgzf",
@@ -2250,17 +2245,17 @@
  "num-bigint",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.15"
+version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
+checksum = "f30b0abd723be7e2ffca1272140fac1a2f084c77ec3e123c192b66af1ee9e6c2"
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
 name = "num_cpus"
@@ -2359,17 +2354,17 @@
  "redox_syscall",
  "smallvec",
  "windows-targets",
 ]
 
 [[package]]
 name = "parquet"
-version = "42.0.0"
+version = "43.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "baab9c36b1c8300b81b4d577d306a0a733f9d34021363098d3548e37757ed6c8"
+checksum = "ec7267a9607c3f955d4d0ac41b88a67cecc0d8d009173ad3da390699a6cb3750"
 dependencies = [
  "ahash",
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-data",
  "arrow-ipc",
@@ -2402,17 +2397,17 @@
 checksum = "c705f256449c60da65e11ff6626e0c16a0a0b96aaa348de61376b249bc340f41"
 dependencies = [
  "regex",
 ]
 
 [[package]]
 name = "paste"
-version = "1.0.13"
+version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b4b27ab7be369122c218afc2079489cdcb4b517c0a3fc386ff11e1fedfcc2b35"
+checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
 
 [[package]]
 name = "percent-encoding"
 version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
 
@@ -2496,15 +2491,15 @@
 name = "pin-project-internal"
 version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec2e072ecce94ec471b13398d5402c188e76ac03cf74dd1a975161b23a3f6d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.25",
+ "syn 2.0.28",
 ]
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4c40d25201921e5ff0c862a505c6557ea88568a4e3ace775ab55e93f2f4f9d57"
@@ -2561,17 +2556,17 @@
 name = "proc-macro-hack"
 version = "0.5.20+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.64"
+version = "1.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "78803b62cbf1f46fde80d7c0e803111524b9877184cfe7c3033659490ac7a7da"
+checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.19.1"
@@ -2640,28 +2635,28 @@
 dependencies = [
  "memchr",
  "serde",
 ]
 
 [[package]]
 name = "quick-xml"
-version = "0.29.0"
+version = "0.30.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "81b9228215d82c7b61490fec1de287136b5de6f5700f6e58ea9ad61a7964ca51"
+checksum = "eff6510e86862b57b210fd8cbe8ed3f0d7d600b9c2863cd4549a2e033c66e956"
 dependencies = [
  "memchr",
  "serde",
  "tokio",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.29"
+version = "1.0.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "573015e8ab27661678357f27dc26460738fd2b6c86e46f386fde94cb5d913105"
+checksum = "50f3b39ccfb720540debaa0164757101c08ecb8d326b15358ce76a62c7e85965"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -2711,17 +2706,17 @@
  "memchr",
  "regex-automata",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-automata"
-version = "0.3.3"
+version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "39354c10dd07468c2e73926b23bb9c2caca74c5501e38a35da70406f1d923310"
+checksum = "b7b6d6190b7594385f61bd3911cd1be99dfddcfc365a4160cc2ab5bff4aed294"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
@@ -2799,21 +2794,20 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.37.23"
+version = "0.38.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4d69718bf81c6127a49dc64e44a742e8bb9213c0ff8869a22c308f84c1d4ab06"
+checksum = "0a962918ea88d644592894bc6dc55acc6c0956488adcebbfb6e273506b7fd6e5"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags 2.3.3",
  "errno",
- "io-lifetimes",
  "libc",
  "linux-raw-sys",
  "windows-sys",
 ]
 
 [[package]]
 name = "rustls"
@@ -2858,33 +2852,33 @@
 checksum = "2d3987094b1d07b653b7dfdc3f70ce9a1da9c51ac18c1b06b662e4f9a0e9f4b2"
 dependencies = [
  "base64",
 ]
 
 [[package]]
 name = "rustls-webpki"
-version = "0.101.1"
+version = "0.101.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "15f36a6828982f422756984e47912a7a51dcbc2a197aa791158f8ca61cd8204e"
+checksum = "513722fd73ad80a71f72b61009ea1b584bcfa1483ca93949c8f290298837fa59"
 dependencies = [
  "ring",
  "untrusted",
 ]
 
 [[package]]
 name = "rustversion"
-version = "1.0.13"
+version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc31bd9b61a32c31f9650d18add92aa83a49ba979c143eefd27fe7177b05bd5f"
+checksum = "7ffc183a10b4478d04cbbbfc96d0873219d962dd5accaff2ffbd4ceb7df837f4"
 
 [[package]]
 name = "ryu"
-version = "1.0.14"
+version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fe232bdf6be8c8de797b22184ee71118d63780ea42ac85b61d1baa6d3b782ae9"
+checksum = "1ad4cc8da4ef723ed60bced201181d83791ad433213d8c24efffda1eec85d741"
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
@@ -2898,97 +2892,97 @@
 checksum = "0c3733bf4cf7ea0880754e19cb5a462007c4a8c1914bff372ccc95b464f1df88"
 dependencies = [
  "windows-sys",
 ]
 
 [[package]]
 name = "scopeguard"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "sct"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d53dcdb7c9f8158937a7981b48accfd39a43af418591a5d008c7b22b5e1b7ca4"
 dependencies = [
  "ring",
  "untrusted",
 ]
 
 [[package]]
 name = "security-framework"
-version = "2.9.1"
+version = "2.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1fc758eb7bffce5b308734e9b0c1468893cae9ff70ebf13e7090be8dcbcc83a8"
+checksum = "05b64fb303737d99b81884b2c63433e9ae28abebe5eb5045dcdd175dc2ecf4de"
 dependencies = [
  "bitflags 1.3.2",
  "core-foundation",
  "core-foundation-sys",
  "libc",
  "security-framework-sys",
 ]
 
 [[package]]
 name = "security-framework-sys"
-version = "2.9.0"
+version = "2.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f51d0c0d83bec45f16480d0ce0058397a69e48fcdc52d1dc8855fb68acbd31a7"
+checksum = "e932934257d3b408ed8f30db49d85ea163bfe74961f017f405b025af298f0c7a"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "semver"
-version = "1.0.17"
+version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
+checksum = "b0293b4b29daaf487284529cc2f5675b8e57c61f70167ba415a463651fd6a918"
 
 [[package]]
 name = "seq-macro"
-version = "0.3.4"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "63134939175b3131fe4d2c131b103fd42f25ccca89423d43b5e4f267920ccf03"
+checksum = "a3f0bf26fd526d2a95683cd0f87bf103b8539e2ca1ef48ce002d67aad59aa0b4"
 
 [[package]]
 name = "serde"
-version = "1.0.171"
+version = "1.0.180"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "30e27d1e4fd7659406c492fd6cfaf2066ba8773de45ca75e855590f856dc34a9"
+checksum = "0ea67f183f058fe88a4e3ec6e2788e003840893b91bac4559cabedd00863b3ed"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_bytes"
-version = "0.11.11"
+version = "0.11.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a16be4fe5320ade08736447e3198294a5ea9a6d44dde6f35f0a5e06859c427a"
+checksum = "ab33ec92f677585af6d88c65593ae2375adde54efdbf16d597f2cbc7a6d368ff"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.171"
+version = "1.0.180"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "389894603bd18c46fa56231694f8d827779c0951a667087194cf9de94ed24682"
+checksum = "24e744d7782b686ab3b73267ef05697159cc0e5abbed3f47f9933165e5219036"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.25",
+ "syn 2.0.28",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.102"
+version = "1.0.104"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5062a995d481b2308b6064e9af76011f2921c35f97b0468811ed9f6cd91dfed"
+checksum = "076066c5f1078eac5b722a31827a8832fe108bed65dfa75e233c89f8206e976c"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -3166,15 +3160,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6069ca09d878a33f883cc06aaa9718ede171841d3832450354410b718b097232"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "rustversion",
- "syn 2.0.25",
+ "syn 2.0.28",
 ]
 
 [[package]]
 name = "subtle"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
@@ -3188,17 +3182,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.25"
+version = "2.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "15e3fc8c0c74267e2df136e5e5fb656a464158aa57624053375eb9c8c6e25ae2"
+checksum = "04361975b3f5e348b2189d8dc55bc942f278b2d482a6a0365de5bdd62d351567"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -3211,27 +3205,26 @@
  "quote",
  "syn 1.0.109",
  "unicode-xid",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.9"
+version = "0.12.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "df8e77cb757a61f51b947ec4a7e3646efd825b73561db1c232a8ccb639e611a0"
+checksum = "9d0e916b1148c8e263850e1ebcbd046f333e0683c724876bb0da63ea4373dc8a"
 
 [[package]]
 name = "tempfile"
-version = "3.6.0"
+version = "3.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "31c0432476357e58790aaa47a8efb0c5138f137343f3b5f23bd36a27e3b0a6d6"
+checksum = "5486094ee78b2e5038a6382ed7645bc084dc2ec433426ca4c3cb61e2007b8998"
 dependencies = [
- "autocfg",
  "cfg-if",
- "fastrand",
+ "fastrand 2.0.0",
  "redox_syscall",
  "rustix",
  "windows-sys",
 ]
 
 [[package]]
 name = "thrift"
@@ -3242,34 +3235,35 @@
  "byteorder",
  "integer-encoding",
  "ordered-float",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.23"
+version = "0.3.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "59e399c068f43a5d116fedaf73b203fa4f9c519f17e2b34f63221d3792f81446"
+checksum = "b79eabcd964882a646b3584543ccabeae7869e9ac32a46f6f22b7a5bd405308b"
 dependencies = [
+ "deranged",
  "serde",
  "time-core",
  "time-macros",
 ]
 
 [[package]]
 name = "time-core"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7300fbefb4dadc1af235a9cef3737cea692a9d97e1b9cbcd4ebdae6f8868e6fb"
 
 [[package]]
 name = "time-macros"
-version = "0.2.10"
+version = "0.2.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "96ba15a897f3c86766b757e5ac7221554c6750054d74d5b28844fce5fb36a6c4"
+checksum = "eb71511c991639bb078fd5bf97757e03914361c48100d52878b8e52b46fb92cd"
 dependencies = [
  "time-core",
 ]
 
 [[package]]
 name = "tiny-keccak"
 version = "2.0.2"
@@ -3317,15 +3311,15 @@
 name = "tokio-macros"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.25",
+ "syn 2.0.28",
 ]
 
 [[package]]
 name = "tokio-rustls"
 version = "0.23.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c43ee83903113e03984cb9e5cebe6c04a5116269e900e3ddba8f068a62adda59"
@@ -3416,15 +3410,15 @@
 name = "tracing-attributes"
 version = "0.1.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5f4f31f56159e98206da9efd823404b79b6ef3143b4a7ab76e67b1751b25a4ab"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.25",
+ "syn 2.0.28",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
@@ -3458,17 +3452,17 @@
 name = "unicode-bidi"
 version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "22049a19f4a68748a168c0fc439f9516686aa045927ff767eca0a85101fb6e73"
+checksum = "301abaae475aa91687eb82514b328ab47a211a533026cb25fc3e519b86adfc3c"
 
 [[package]]
 name = "unicode-normalization"
 version = "0.1.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
 dependencies = [
@@ -3514,23 +3508,23 @@
  "form_urlencoded",
  "idna",
  "percent-encoding",
 ]
 
 [[package]]
 name = "urlencoding"
-version = "2.1.2"
+version = "2.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e8db7427f936968176eaa7cdf81b7f98b980b18495ec28f1b5791ac3bfe3eea9"
+checksum = "daf8dba3b7eb870caf1ddeed7bc9d2a049f3cfdfae7cb521b087cc33ae4c49da"
 
 [[package]]
 name = "uuid"
-version = "1.4.0"
+version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d023da39d1fde5a8a3fe1f3e01ca9632ada0a63e9797de55a879d6e2236277be"
+checksum = "79daa5ed5740825c40b389c5e50312b9c86df53fccd33f281df655642b43869d"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "version_check"
 version = "0.1.5"
@@ -3591,15 +3585,15 @@
 checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.25",
+ "syn 2.0.28",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
 version = "0.4.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -3625,15 +3619,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.25",
+ "syn 2.0.28",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.87"
@@ -3816,26 +3810,26 @@
 name = "zeroize"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2a0956f1ba7c7909bfb66c2e9e4124ab6f6482560f6628b5aaeba39207c9aad9"
 
 [[package]]
 name = "zstd"
-version = "0.12.3+zstd.1.5.2"
+version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "76eea132fb024e0e13fd9c2f5d5d595d8a967aa72382ac2f9d39fcc95afd0806"
+checksum = "1a27595e173641171fc74a1232b7b1c7a7cb6e18222c11e9dfb9888fa424c53c"
 dependencies = [
  "zstd-safe",
 ]
 
 [[package]]
 name = "zstd-safe"
-version = "6.0.5+zstd.1.5.4"
+version = "6.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d56d9e60b4b1758206c238a10165fbcae3ca37b01744e394c463463f6529d23b"
+checksum = "ee98ffd0b48ee95e6c5168188e44a54550b1564d9d530ee21d5f0eaed1069581"
 dependencies = [
  "libc",
  "zstd-sys",
 ]
 
 [[package]]
 name = "zstd-sys"
```

### Comparing `biobear-0.7.4/PKG-INFO` & `biobear-0.8.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: biobear
-Version: 0.7.4
-Classifier: Programming Language :: Rust
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Dist: pyarrow >=12
-License-File: LICENSE
-Author-email: WHERE TRUE devs <thauck+biobear@wheretrue.com>
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-
 <h1 align="center">
     <img src=".github/biobear.svg" width="400px" alt="biobear" />
 </h1>
 
 biobear is a Python library designed for reading and searching bioinformatic file formats, using Rust as its backend and producing Arrow Batch Readers and other downstream formats (like polars or duckdb).
 
 The python package has minimal dependencies and only requires Polars. Biobear can be used to read various bioinformatic file formats, including FASTA, FASTQ, VCF, BAM, and GFF locally or from an object store like S3. It can also query some indexed file formats locally like VCF and BAM.
@@ -58,7 +46,21 @@
 │ str     ┆ str    ┆ str  ┆ i64   ┆   ┆ f32   ┆ str    ┆ str   ┆ list[struct[2]]                   │
 ╞═════════╪════════╪══════╪═══════╪═══╪═══════╪════════╪═══════╪═══════════════════════════════════╡
 │ chr1    ┆ .      ┆ gene ┆ 1     ┆ … ┆ null  ┆ +      ┆ null  ┆ [{"gene_id","1"}, {"gene_name","… │
 │ chr1    ┆ .      ┆ gene ┆ 200   ┆ … ┆ null  ┆ +      ┆ null  ┆ [{"gene_id","2"}, {"gene_name","… │
 └─────────┴────────┴──────┴───────┴───┴───────┴────────┴───────┴───────────────────────────────────┘
 ```
 
+## Performance
+
+Please see the [exon][]'s performance metrics for thorough benchmarks, but in short, biobear is generally faster than other Python libraries for reading bioinformatic file formats.
+
+For example, here's quick benchmarks for reading one FASTA file with 1 million records and reading 5 FASTA files each with 1 million records for the local file system on an M1 MacBook Pro:
+
+| Library   | 1 file (s)         | 5 files (s)         |
+|-----------|--------------------|---------------------|
+| BioBear   | 4.605 s ±  0.166 s | 6.420 s ±  0.113 s  |
+| BioPython | 6.654 s ±  0.003 s | 34.254 s ±  0.053 s |
+
+The larger difference multiple files is due to biobear's ability to read multiple files in parallel.
+
+[exon]: https://github.com/wheretrue/exon/tree/main/exon-benchmarks
```

