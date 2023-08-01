# Comparing `tmp/immunopipe-0.5.0.tar.gz` & `tmp/immunopipe-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "immunopipe-0.5.0.tar", max compression
+gzip compressed data, was "immunopipe-0.5.1.tar", max compression
```

## Comparing `immunopipe-0.5.0.tar` & `immunopipe-0.5.1.tar`

### file list

```diff
@@ -1,22 +1,20 @@
--rw-r--r--   0        0        0    35128 2023-07-05 16:52:10.608739 immunopipe-0.5.0/LICENSE
--rw-r--r--   0        0        0     3185 2023-07-05 16:52:10.608739 immunopipe-0.5.0/README.md
--rw-r--r--   0        0        0      143 2023-07-05 16:52:10.612739 immunopipe-0.5.0/immunopipe/__init__.py
--rw-r--r--   0        0        0      109 2023-07-05 16:52:10.612739 immunopipe-0.5.0/immunopipe/__main__.py
--rw-r--r--   0        0        0     4551 2023-07-05 16:52:10.612739 immunopipe-0.5.0/immunopipe/inhouse.py
--rw-r--r--   0        0        0      432 2023-07-05 16:52:10.612739 immunopipe-0.5.0/immunopipe/pipeline.py
--rw-r--r--   0        0        0     7596 2023-07-05 16:52:10.612739 immunopipe-0.5.0/immunopipe/processes.py
--rw-r--r--   0        0        0     1581 2023-07-05 16:52:10.612739 immunopipe-0.5.0/immunopipe/reports/CloneHeterogeneity.svelte
--rw-r--r--   0        0        0      683 2023-07-05 16:52:10.612739 immunopipe-0.5.0/immunopipe/reports/MarkersOverlapping.svelte
--rw-r--r--   0        0        0      679 2023-07-05 16:52:10.612739 immunopipe-0.5.0/immunopipe/reports/MetaMarkersForClones.svelte
--rw-r--r--   0        0        0      181 2023-07-05 16:52:10.612739 immunopipe-0.5.0/immunopipe/reports/RadarPlots.svelte
--rw-r--r--   0        0        0      214 2023-07-05 16:52:10.612739 immunopipe-0.5.0/immunopipe/reports/SampleInfo.svelte
--rw-r--r--   0        0        0     1012 2023-07-05 16:52:10.612739 immunopipe-0.5.0/immunopipe/reports/SelectTCells.svelte
--rw-r--r--   0        0        0     4769 2023-07-05 16:52:10.612739 immunopipe-0.5.0/immunopipe/scripts/CloneHeterogeneity.R
--rw-r--r--   0        0        0     2029 2023-07-05 16:52:10.612739 immunopipe-0.5.0/immunopipe/scripts/MarkersOverlapping.R
--rw-r--r--   0        0        0     3289 2023-07-05 16:52:10.612739 immunopipe-0.5.0/immunopipe/scripts/MetaMarkersForClones.R
--rw-r--r--   0        0        0     3699 2023-07-05 16:52:10.612739 immunopipe-0.5.0/immunopipe/scripts/RadarPlots.R
--rw-r--r--   0        0        0     4029 2023-07-05 16:52:10.612739 immunopipe-0.5.0/immunopipe/scripts/SelectTCells.R
--rw-r--r--   0        0        0       22 2023-07-05 16:52:10.612739 immunopipe-0.5.0/immunopipe/version.py
--rw-r--r--   0        0        0      855 2023-07-05 16:52:10.612739 immunopipe-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     4128 1970-01-01 00:00:00.000000 immunopipe-0.5.0/setup.py
--rw-r--r--   0        0        0     3920 1970-01-01 00:00:00.000000 immunopipe-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    35128 2023-08-01 02:31:56.601427 immunopipe-0.5.1/LICENSE
+-rw-r--r--   0        0        0     3185 2023-08-01 02:31:56.601427 immunopipe-0.5.1/README.md
+-rw-r--r--   0        0        0      143 2023-08-01 02:31:56.605428 immunopipe-0.5.1/immunopipe/__init__.py
+-rw-r--r--   0        0        0      109 2023-08-01 02:31:56.605428 immunopipe-0.5.1/immunopipe/__main__.py
+-rw-r--r--   0        0        0     3469 2023-08-01 02:31:56.605428 immunopipe-0.5.1/immunopipe/inhouse.py
+-rw-r--r--   0        0        0      432 2023-08-01 02:31:56.605428 immunopipe-0.5.1/immunopipe/pipeline.py
+-rw-r--r--   0        0        0     8373 2023-08-01 02:31:56.605428 immunopipe-0.5.1/immunopipe/processes.py
+-rw-r--r--   0        0        0     1581 2023-08-01 02:31:56.605428 immunopipe-0.5.1/immunopipe/reports/CloneHeterogeneity.svelte
+-rw-r--r--   0        0        0      683 2023-08-01 02:31:56.605428 immunopipe-0.5.1/immunopipe/reports/MarkersOverlapping.svelte
+-rw-r--r--   0        0        0      679 2023-08-01 02:31:56.605428 immunopipe-0.5.1/immunopipe/reports/MetaMarkersForClones.svelte
+-rw-r--r--   0        0        0      214 2023-08-01 02:31:56.605428 immunopipe-0.5.1/immunopipe/reports/SampleInfo.svelte
+-rw-r--r--   0        0        0     1012 2023-08-01 02:31:56.605428 immunopipe-0.5.1/immunopipe/reports/SelectTCells.svelte
+-rw-r--r--   0        0        0     4769 2023-08-01 02:31:56.605428 immunopipe-0.5.1/immunopipe/scripts/CloneHeterogeneity.R
+-rw-r--r--   0        0        0     2029 2023-08-01 02:31:56.605428 immunopipe-0.5.1/immunopipe/scripts/MarkersOverlapping.R
+-rw-r--r--   0        0        0     3289 2023-08-01 02:31:56.605428 immunopipe-0.5.1/immunopipe/scripts/MetaMarkersForClones.R
+-rw-r--r--   0        0        0     4029 2023-08-01 02:31:56.605428 immunopipe-0.5.1/immunopipe/scripts/SelectTCells.R
+-rw-r--r--   0        0        0       22 2023-08-01 02:31:56.605428 immunopipe-0.5.1/immunopipe/version.py
+-rw-r--r--   0        0        0      857 2023-08-01 02:31:56.609428 immunopipe-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4132 1970-01-01 00:00:00.000000 immunopipe-0.5.1/setup.py
+-rw-r--r--   0        0        0     3924 1970-01-01 00:00:00.000000 immunopipe-0.5.1/PKG-INFO
```

### Comparing `immunopipe-0.5.0/LICENSE` & `immunopipe-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `immunopipe-0.5.0/README.md` & `immunopipe-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `immunopipe-0.5.0/immunopipe/inhouse.py` & `immunopipe-0.5.1/immunopipe/inhouse.py`

 * *Files 15% similar despite different names*

```diff
@@ -40,41 +40,14 @@
         "report": "file://reports/SelectTCells.svelte",
         # "report_toc": False,
         "report_order": 2,
     }
     order = 5
 
 
-class RadarPlots(Proc):
-    """Radar plots for cell proportion in different clusters
-
-    Envs:
-        cases (type=json): Cases with keys as case names
-            each case has arguments with keys:
-            * mutaters: Add new columns to the meta.data.
-            * by: Which column to use to separate the cells in different groups.
-            * order: The order of the values in `by`.
-            * breaks: breaks of the radar plots.
-            * direction: Direction to calculate the percentages.
-                inter-cluster: the percentage of the cells in all groups.
-                intra-cluster: the percentage of the cells in all clusters.
-            * prec_with_na: Whether the percentages are
-                calculated before or after filtering out the NAs.
-    """
-    input = "srtobj:file"
-    output = "outdir:dir:{{in.srtobj | stem}}.radar_plots"
-    lang = config.lang.rscript
-    script = "file://scripts/RadarPlots.R"
-    envs = {"cases": {}}
-    plugin_opts = {
-        "report": "file://reports/RadarPlots.svelte",
-        "report_toc": False,
-    }
-
-
 class CloneHeterogeneity(Proc):
     """Clone heterogeneity in each cluster
 
     Envs:
         cases (type=json): Cases with keys as case names.
             Each case has arguments with keys:
             * cut: How to cut the clones by sizes
```

### Comparing `immunopipe-0.5.0/immunopipe/processes.py` & `immunopipe-0.5.1/immunopipe/processes.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,21 +23,22 @@
     SeuratClustering,
     SeuratClusterStats,
     SeuratMetadataMutater as SeuratMetadataMutater_,
     MarkersFinder,
     CellTypeAnnotate as CellTypeAnnotate_,
     CellsDistribution,
     ScFGSEA,
+    TopExpressingGenes,
+    RadarPlots,
 )
 from biopipen.ns.scrna_metabolic_landscape import ScrnaMetabolicLandscape
 
 # inhouse processes
 from .inhouse import (
     SelectTCells,
-    RadarPlots,
     CloneHeterogeneity,
     MetaMarkersForClones,
     MarkersOverlapping,
 )
 
 toml_dumps = FILTERS["toml_dumps"]
 from_board = from_pipen_board()
@@ -97,14 +98,28 @@
     {{*Summary.long}}
     """
     requires = SeuratClusteringOfAllCells
     plugin_opts = {"report_order": 1}
     order = 4
 
 
+@annotate.format_doc(indent=1)
+class TopExpressingGenesOfAllCells(TopExpressingGenes):
+    """Top expressing genes for clusters of all cells.
+
+    If all your cells are T cells, the clustering will be performed on all
+    T cells. `TopExpressingGenesOfTCells` will be skipped.
+
+    {{*Summary.long}}
+    """
+    requires = SeuratClusteringOfAllCells
+    plugin_opts = {"report_order": 1}
+    order = 4
+
+
 class Immunarch(Immunarch):
     requires = ImmunarchLoading
 
 
 @mark(board_config_hidden=True)
 class Immunarch2VDJtools(Immunarch2VDJtools):
     requires = ImmunarchLoading
@@ -141,14 +156,26 @@
         """Find markers for clusters of T cells
 
         This process will be skipped if all cells are T cells.
 
         {{*Summary.long}}
         """
         requires = SeuratClusteringOfTCells
+        plugin_opts = {"report_order": 3}
+        order = 6
+
+    @annotate.format_doc(indent=2)
+    class TopExpressingGenesOfTCells(TopExpressingGenes):
+        """Find markers for clusters of T cells
+
+        This process will be skipped if all cells are T cells.
+
+        {{*Summary.long}}
+        """
+        requires = SeuratClusteringOfTCells
         plugin_opts = {"report_order": 3}
         order = 6
 
 else:
     SeuratClusteringOfTCells = SeuratClusteringOfAllCells
```

### Comparing `immunopipe-0.5.0/immunopipe/reports/CloneHeterogeneity.svelte` & `immunopipe-0.5.1/immunopipe/reports/CloneHeterogeneity.svelte`

 * *Files identical despite different names*

### Comparing `immunopipe-0.5.0/immunopipe/reports/MarkersOverlapping.svelte` & `immunopipe-0.5.1/immunopipe/reports/MarkersOverlapping.svelte`

 * *Files identical despite different names*

### Comparing `immunopipe-0.5.0/immunopipe/reports/MetaMarkersForClones.svelte` & `immunopipe-0.5.1/immunopipe/reports/MetaMarkersForClones.svelte`

 * *Files identical despite different names*

### Comparing `immunopipe-0.5.0/immunopipe/reports/SelectTCells.svelte` & `immunopipe-0.5.1/immunopipe/reports/SelectTCells.svelte`

 * *Files identical despite different names*

### Comparing `immunopipe-0.5.0/immunopipe/scripts/CloneHeterogeneity.R` & `immunopipe-0.5.1/immunopipe/scripts/CloneHeterogeneity.R`

 * *Files identical despite different names*

### Comparing `immunopipe-0.5.0/immunopipe/scripts/MarkersOverlapping.R` & `immunopipe-0.5.1/immunopipe/scripts/MarkersOverlapping.R`

 * *Files identical despite different names*

### Comparing `immunopipe-0.5.0/immunopipe/scripts/MetaMarkersForClones.R` & `immunopipe-0.5.1/immunopipe/scripts/MetaMarkersForClones.R`

 * *Files identical despite different names*

### Comparing `immunopipe-0.5.0/immunopipe/scripts/SelectTCells.R` & `immunopipe-0.5.1/immunopipe/scripts/SelectTCells.R`

 * *Files identical despite different names*

### Comparing `immunopipe-0.5.0/pyproject.toml` & `immunopipe-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "immunopipe"
 description = "A pipeline for integrative analysis for scTCR- and scRNA-seq data"
 authors = [ "pwwang <pwwang@pwwang.com>",]
-version = "0.5.0"
+version = "0.5.1"
 license = "GNU General Public License v3.0"
 readme = "README.md"
 homepage = "https://github.com/pwwang/immunopipe"
 repository = "https://github.com/pwwang/immunopipe"
 
 [tool.poetry.build]
 generate-setup-file = true
 
 [tool.poetry.dependencies]
 python = "^3.8"
 # pipen-report and pipen-board are required by biopipen
-biopipen = "^0.15"
+biopipen = "^0.15.2"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.scripts]
 immunopipe = "immunopipe.pipeline:main"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `immunopipe-0.5.0/setup.py` & `immunopipe-0.5.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 packages = \
 ['immunopipe']
 
 package_data = \
 {'': ['*'], 'immunopipe': ['reports/*', 'scripts/*']}
 
 install_requires = \
-['biopipen>=0.15,<0.16']
+['biopipen>=0.15.2,<0.16.0']
 
 entry_points = \
 {'console_scripts': ['immunopipe = immunopipe.pipeline:main']}
 
 setup_kwargs = {
     'name': 'immunopipe',
-    'version': '0.5.0',
+    'version': '0.5.1',
     'description': 'A pipeline for integrative analysis for scTCR- and scRNA-seq data',
     'long_description': '# immunopipe\n\nIntegrative analysis for scTCR- and scRNA-seq data\n\n## Requirements & Installation\n\n- `python`: `3.7+`\n    - Other python depedencies should be installed via `pip install -U immunopipe`\n\n- `R`\n    - A bunch of R packages\n\n- Other\n  - VDJtools: https://vdjtools-doc.readthedocs.io/en/master/install.html\n\n- Checking requirements\n\n  ```shell\n  pip install -U pipen-cli-require\n  pipen require immunopipe.pipeline:pipeline <pipeline arguments>\n  ```\n\n- Quick way to install the dependencies using conda\n  ```shell\n  conda env install --name <env_name> --file docker/environment.yml\n  # then\n  conda activate <env_name>\n  ```\n\n## Running as a container\n\n### Using docker:\n\n```bash\ndocker run \\\n    -w /immunopipe/workdir \\\n    -v $(pwd)/:/immunopipe/workdir \\\n    -v /tmp \\\n    -v $(pwd)/prepared-data:/mnt \\\n    justold/immunopipe:<tag>  # or :dev to use the development version\n```\n\n### Using singularity:\n\n```bash\nsingularity run -w \\  # need it to be writable\n  --pwd /immunopipe/workdir -B .:/immunopipe/workdir \\  # Could use other directory instead of "."\n  # --contain: don\'t map host filesystem\n  # --cleanenv: recommended, to avoid other host\'s environment variables to be used\n  #   For example, $CONDA_PREFIX to affect host\'s conda environment\n  --contain --cleanenv \\\n  docker://justold/immunopipe:<tag>  # or :dev to use the development version\n\n# The mount your data directory to /mnt, which will make startup faster\n# For example\n#   -B .:/immunopipe/workdir,/path/to/data:/mnt\n# Where /path/to/data is the data directory containing the data files\n# You may also want to bind other directories (i.e. /tmp)\n#   -B <other bindings>,/tmp\n\n# Or you can pull the image first by:\nsingularity pull --force --dir images/ docker://justold/immunopipe:<tag>\n# Then you can replace "docker://justold/immunopipe:<tag>" with "images/immunopipe.sif"\n```\n\n## Modules\n\n![immunopipe](./immunopipe.png)\n\n- Basic TCR data analysis using `immunarch`\n- Clone Residency analysis if you have paired samples (i.e. Tumor vs Normal)\n- V-J usage, the frequency of various V-J junctions in circos-style plots\n- Clustering cells and configurale arguments to separate T and non-T cells\n- Clustering T cell, markers for each cluster and enrichment analysis for the markers\n- Radar plots to show the composition of cells for clusters\n- (Meta-)Markers finder for selected groups/clones of cells\n- Psedo-bulk GSEA analysis of two groups of cells\n- Seurat cluster statistics, including:\n  - Basic statistics of the clusters (e.g. number of cells in each cluster)\n  - Gene expressions (e.g. ridge, violin, feature, dot and heatmap plots)\n  - Dimensional reduction plots\n- TCR clustering using CDR3 sequences and the statistics of the clusters\n- Cell group distribution (TCR clones/clusters) in Seurat clusters\n- Clone heterogeneity (TCR clone distribution) in Seurat clusters\n- Metabolic landscape analysis (Ref: Xiao, Zhengtao, Ziwei Dai, and Jason W. Locasale. "Metabolic landscape of the tumor microenvironment at single cell resolution." Nature communications 10.1 (2019): 1-12.)\n\n## Documentaion\n\nhttps://pwwang.github.io/immunopipe\n\n## Example\n\nhttps://github.com/pwwang/immunopipe-example\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pwwang/immunopipe',
```

### Comparing `immunopipe-0.5.0/PKG-INFO` & `immunopipe-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: immunopipe
-Version: 0.5.0
+Version: 0.5.1
 Summary: A pipeline for integrative analysis for scTCR- and scRNA-seq data
 Home-page: https://github.com/pwwang/immunopipe
 License: GNU General Public License v3.0
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: biopipen (>=0.15,<0.16)
+Requires-Dist: biopipen (>=0.15.2,<0.16.0)
 Project-URL: Repository, https://github.com/pwwang/immunopipe
 Description-Content-Type: text/markdown
 
 # immunopipe
 
 Integrative analysis for scTCR- and scRNA-seq data
```

