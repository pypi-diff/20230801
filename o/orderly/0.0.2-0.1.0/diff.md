# Comparing `tmp/orderly-0.0.2.tar.gz` & `tmp/orderly-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orderly-0.0.2.tar", last modified: Mon Jul 10 13:54:11 2023, max compression
+gzip compressed data, was "orderly-0.1.0.tar", last modified: Tue Aug  1 12:38:57 2023, max compression
```

## Comparing `orderly-0.0.2.tar` & `orderly-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 dsw46      (502) staff       (20)        0 2023-07-10 13:54:11.112041 orderly-0.0.2/
--rw-r--r--   0 dsw46      (502) staff       (20)      390 2023-07-05 16:07:31.000000 orderly-0.0.2/AUTHORS
--rw-r--r--   0 dsw46      (502) staff       (20)     1060 2023-07-05 16:07:31.000000 orderly-0.0.2/LICENSE
--rw-r--r--   0 dsw46      (502) staff       (20)     8715 2023-07-10 13:54:11.111495 orderly-0.0.2/PKG-INFO
--rw-r--r--   0 dsw46      (502) staff       (20)     8275 2023-07-10 11:52:23.000000 orderly-0.0.2/README.md
-drwxr-xr-x   0 dsw46      (502) staff       (20)        0 2023-07-10 13:54:11.106632 orderly-0.0.2/orderly/
--rw-r--r--   0 dsw46      (502) staff       (20)      294 2023-07-05 16:07:31.000000 orderly-0.0.2/orderly/__init__.py
--rw-r--r--   0 dsw46      (502) staff       (20)     1934 2023-07-05 16:07:31.000000 orderly-0.0.2/orderly/types.py
-drwxr-xr-x   0 dsw46      (502) staff       (20)        0 2023-07-10 13:54:11.108218 orderly-0.0.2/orderly.egg-info/
--rw-r--r--   0 dsw46      (502) staff       (20)     8715 2023-07-10 13:54:11.000000 orderly-0.0.2/orderly.egg-info/PKG-INFO
--rw-r--r--   0 dsw46      (502) staff       (20)      271 2023-07-10 13:54:11.000000 orderly-0.0.2/orderly.egg-info/SOURCES.txt
--rw-r--r--   0 dsw46      (502) staff       (20)        1 2023-07-10 13:54:11.000000 orderly-0.0.2/orderly.egg-info/dependency_links.txt
--rw-r--r--   0 dsw46      (502) staff       (20)        8 2023-07-10 13:54:11.000000 orderly-0.0.2/orderly.egg-info/top_level.txt
--rw-r--r--   0 dsw46      (502) staff       (20)     1096 2023-07-05 16:07:31.000000 orderly-0.0.2/pyproject.toml
--rw-r--r--   0 dsw46      (502) staff       (20)       38 2023-07-10 13:54:11.112177 orderly-0.0.2/setup.cfg
--rw-r--r--   0 dsw46      (502) staff       (20)      634 2023-07-10 13:51:54.000000 orderly-0.0.2/setup.py
-drwxr-xr-x   0 dsw46      (502) staff       (20)        0 2023-07-10 13:54:11.110160 orderly-0.0.2/tests/
--rw-r--r--   0 dsw46      (502) staff       (20)    42944 2023-07-05 16:07:31.000000 orderly-0.0.2/tests/test_clean.py
--rw-r--r--   0 dsw46      (502) staff       (20)     1548 2023-07-05 16:07:31.000000 orderly-0.0.2/tests/test_data.py
--rw-r--r--   0 dsw46      (502) staff       (20)    59324 2023-07-05 16:07:31.000000 orderly-0.0.2/tests/test_extract.py
+drwxr-xr-x   0 dsw46      (502) staff       (20)        0 2023-08-01 12:38:57.450646 orderly-0.1.0/
+-rw-r--r--   0 dsw46      (502) staff       (20)      390 2023-04-14 18:37:02.000000 orderly-0.1.0/AUTHORS
+-rw-r--r--   0 dsw46      (502) staff       (20)     1079 2023-07-03 14:56:10.000000 orderly-0.1.0/LICENSE
+-rw-r--r--   0 dsw46      (502) staff       (20)     8971 2023-08-01 12:38:57.450365 orderly-0.1.0/PKG-INFO
+-rw-r--r--   0 dsw46      (502) staff       (20)     8718 2023-08-01 12:20:44.000000 orderly-0.1.0/README.md
+drwxr-xr-x   0 dsw46      (502) staff       (20)        0 2023-08-01 12:38:57.447829 orderly-0.1.0/orderly/
+-rw-r--r--   0 dsw46      (502) staff       (20)      315 2023-07-31 10:25:49.000000 orderly-0.1.0/orderly/__init__.py
+-rw-r--r--   0 dsw46      (502) staff       (20)     1934 2023-05-02 14:22:54.000000 orderly-0.1.0/orderly/types.py
+drwxr-xr-x   0 dsw46      (502) staff       (20)        0 2023-08-01 12:38:57.448798 orderly-0.1.0/orderly.egg-info/
+-rw-r--r--   0 dsw46      (502) staff       (20)     8971 2023-08-01 12:38:57.000000 orderly-0.1.0/orderly.egg-info/PKG-INFO
+-rw-r--r--   0 dsw46      (502) staff       (20)      271 2023-08-01 12:38:57.000000 orderly-0.1.0/orderly.egg-info/SOURCES.txt
+-rw-r--r--   0 dsw46      (502) staff       (20)        1 2023-08-01 12:38:57.000000 orderly-0.1.0/orderly.egg-info/dependency_links.txt
+-rw-r--r--   0 dsw46      (502) staff       (20)        8 2023-08-01 12:38:57.000000 orderly-0.1.0/orderly.egg-info/top_level.txt
+-rw-r--r--   0 dsw46      (502) staff       (20)     1140 2023-07-03 14:56:10.000000 orderly-0.1.0/pyproject.toml
+-rw-r--r--   0 dsw46      (502) staff       (20)       38 2023-08-01 12:38:57.450690 orderly-0.1.0/setup.cfg
+-rw-r--r--   0 dsw46      (502) staff       (20)      655 2023-08-01 12:38:05.000000 orderly-0.1.0/setup.py
+drwxr-xr-x   0 dsw46      (502) staff       (20)        0 2023-08-01 12:38:57.449899 orderly-0.1.0/tests/
+-rw-r--r--   0 dsw46      (502) staff       (20)    44246 2023-07-03 14:56:10.000000 orderly-0.1.0/tests/test_clean.py
+-rw-r--r--   0 dsw46      (502) staff       (20)     1548 2023-04-14 18:37:02.000000 orderly-0.1.0/tests/test_data.py
+-rw-r--r--   0 dsw46      (502) staff       (20)    60769 2023-07-03 14:56:10.000000 orderly-0.1.0/tests/test_extract.py
```

### Comparing `orderly-0.0.2/LICENSE` & `orderly-0.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Copyright (c) Daniel Wigh and others
-
-Permission is hereby granted, free of charge, to any person obtaining
-a copy of this software and associated documentation files (the
-"Software"), to deal in the Software without restriction, including
-without limitation the rights to use, copy, modify, merge, publish,
-distribute, sublicense, and/or sell copies of the Software, and to
-permit persons to whom the Software is furnished to do so, subject to
-the following conditions:
-
-The above copyright notice and this permission notice shall be
-included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
-NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
-LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
+Copyright (c) Daniel Wigh and others
+
+Permission is hereby granted, free of charge, to any person obtaining
+a copy of this software and associated documentation files (the
+"Software"), to deal in the Software without restriction, including
+without limitation the rights to use, copy, modify, merge, publish,
+distribute, sublicense, and/or sell copies of the Software, and to
+permit persons to whom the Software is furnished to do so, subject to
+the following conditions:
+
+The above copyright notice and this permission notice shall be
+included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
+LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
 WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `orderly-0.0.2/PKG-INFO` & `orderly-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orderly
-Version: 0.0.2
+Version: 0.1.0
 Summary: A wrapper for downloading ORD-schema data, extracting and cleaning the data
 Author: ['Daniel S. Wigh <dsw46@cam.ac.uk>', 'Joe Arrowsmith <joearrowsmith0@gmail.com>', 'Alexander Pomberger <ap2153@cam.ac.uk>', 'Kobi C. Felton <kcmf2@cam.ac.uk>', 'Alexei A. Lapkin <aal35@cam.ac.uk>']
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
@@ -12,14 +12,16 @@
 
 🧪 Cleaning chemical reaction data 🧪
 
 🎯 [Condition Prediction Benchmark](https://figshare.com/articles/dataset/ORDerly_chemical_reactions_condition_benchmarks/23298467) 🎯
 
 ## Quick Install
 
+Requires Python 3.10 (Tested on MacOS and Linux)
+
 ```pip install orderly```
 
 🤔 What is this?
 -----------------
 
 Machine learning has the potential to provide tremendous value to chemistry. However, large amounts of clean high-quality data are needed to train models
 
@@ -36,19 +38,21 @@
 <!-- Section on extracting and cleaning a dataset-->
 
 📖 Extract and clean a dataset
 ------------------------------
  
 ### Download data from ORD
 
-```python -m orderly.download.ord```
+<!-- ```python -m orderly.download.ord```
+
+This will create a folder called ```/data/ord/``` in your current directory, and download the data into ```ord/``` -->
 
-This will create a folder called ```/data/ord/``` in your current directory, and download the data into ```ord/```
+Data in ORD format should be placed in a folder called ```/data/ord/```. You can either use your own data, or the open-source ORD data.
 
-Alternatively, you can also follow the instructions on the [official website](https://github.com/open-reaction-database/ord-data) to download the data in ```ord-data/data/```.
+To download the ORD data follow the instructions on the [official website](https://github.com/open-reaction-database/ord-data) (i.e. download GitLFS and clone their repository) and then place it within a folder called ```/data/ord/```.
 
 ### Extract data from the ORD files
 
 ```python -m orderly.extract```
 
 If you want to run ORDerly on your own data, and want to specify the input and output path:
```

### Comparing `orderly-0.0.2/README.md` & `orderly-0.1.0/orderly.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,27 @@
+Metadata-Version: 2.1
+Name: orderly
+Version: 0.1.0
+Summary: A wrapper for downloading ORD-schema data, extracting and cleaning the data
+Author: ['Daniel S. Wigh <dsw46@cam.ac.uk>', 'Joe Arrowsmith <joearrowsmith0@gmail.com>', 'Alexander Pomberger <ap2153@cam.ac.uk>', 'Kobi C. Felton <kcmf2@cam.ac.uk>', 'Alexei A. Lapkin <aal35@cam.ac.uk>']
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS
+
 # ORDerly
 
 🧪 Cleaning chemical reaction data 🧪
 
 🎯 [Condition Prediction Benchmark](https://figshare.com/articles/dataset/ORDerly_chemical_reactions_condition_benchmarks/23298467) 🎯
 
 ## Quick Install
 
+Requires Python 3.10 (Tested on MacOS and Linux)
+
 ```pip install orderly```
 
 🤔 What is this?
 -----------------
 
 Machine learning has the potential to provide tremendous value to chemistry. However, large amounts of clean high-quality data are needed to train models
 
@@ -26,19 +38,21 @@
 <!-- Section on extracting and cleaning a dataset-->
 
 📖 Extract and clean a dataset
 ------------------------------
  
 ### Download data from ORD
 
-```python -m orderly.download.ord```
+<!-- ```python -m orderly.download.ord```
+
+This will create a folder called ```/data/ord/``` in your current directory, and download the data into ```ord/``` -->
 
-This will create a folder called ```/data/ord/``` in your current directory, and download the data into ```ord/```
+Data in ORD format should be placed in a folder called ```/data/ord/```. You can either use your own data, or the open-source ORD data.
 
-Alternatively, you can also follow the instructions on the [official website](https://github.com/open-reaction-database/ord-data) to download the data in ```ord-data/data/```.
+To download the ORD data follow the instructions on the [official website](https://github.com/open-reaction-database/ord-data) (i.e. download GitLFS and clone their repository) and then place it within a folder called ```/data/ord/```.
 
 ### Extract data from the ORD files
 
 ```python -m orderly.extract```
 
 If you want to run ORDerly on your own data, and want to specify the input and output path:
```

### Comparing `orderly-0.0.2/orderly/types.py` & `orderly-0.1.0/orderly/types.py`

 * *Files identical despite different names*

### Comparing `orderly-0.0.2/orderly.egg-info/PKG-INFO` & `orderly-0.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,193 +1,187 @@
-Metadata-Version: 2.1
-Name: orderly
-Version: 0.0.2
-Summary: A wrapper for downloading ORD-schema data, extracting and cleaning the data
-Author: ['Daniel S. Wigh <dsw46@cam.ac.uk>', 'Joe Arrowsmith <joearrowsmith0@gmail.com>', 'Alexander Pomberger <ap2153@cam.ac.uk>', 'Kobi C. Felton <kcmf2@cam.ac.uk>', 'Alexei A. Lapkin <aal35@cam.ac.uk>']
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS
-
-# ORDerly
-
-🧪 Cleaning chemical reaction data 🧪
-
-🎯 [Condition Prediction Benchmark](https://figshare.com/articles/dataset/ORDerly_chemical_reactions_condition_benchmarks/23298467) 🎯
-
-## Quick Install
-
-```pip install orderly```
-
-🤔 What is this?
------------------
-
-Machine learning has the potential to provide tremendous value to chemistry. However, large amounts of clean high-quality data are needed to train models
-
-ORDerly cleans chemical reaction data from the growing [Open Reaction Database (ORD)](https://docs.open-reaction-database.org/en/latest/).
-
-Use ORDerly to:
-- Extract and clean your own dataset from ORD
-- Access the [ORDerly condition prediction benchmark dataset](https://figshare.com/articles/dataset/ORDerly_chemical_reactions_condition_benchmarks/23298467) for reaction condition prediction.
-- Reproduce results from our paper including training a ML model to predict reaction conditions
-
-<img src="images/abstract_fig.png" alt="Abstract Figure" width="300">
-
-
-<!-- Section on extracting and cleaning a dataset-->
-
-📖 Extract and clean a dataset
-------------------------------
- 
-### Download data from ORD
-
-```python -m orderly.download.ord```
-
-This will create a folder called ```/data/ord/``` in your current directory, and download the data into ```ord/```
-
-Alternatively, you can also follow the instructions on the [official website](https://github.com/open-reaction-database/ord-data) to download the data in ```ord-data/data/```.
-
-### Extract data from the ORD files
-
-```python -m orderly.extract```
-
-If you want to run ORDerly on your own data, and want to specify the input and output path:
-
-```python -m orderly.extract --input_path="/data/ord/" --output_path="/data/orderly/"```
-
-This will generate a parquet file for each ORD file.
-
-### Clean the data
-
-This will produce train and test parquet files, along with a .json file showing the arguments used and a .log file showing the operations run.
-
-```python -m orderly.clean```
-
-<!-- Section on downloading the benchmark -->
-🚀 Download the condition prediction benchmark dataset
---------------------------------------------------------
-
-Reaction condition prediction is the problem of predicting the things "above the arrow" in chemical reactions.
-
-<!-- Include image of a reactions -->
-
-There are three options for donwloading the benchmark.
-
-1) If you have orderly installed you can download the benchmark using this command:
-
-```python -m orderly.download.benchmark```
-
-2) Or you can either download the [ORDerly condition prediction benchmark dataset](https://figshare.com/articles/dataset/ORDerly_chemical_reactions_condition_benchmarks/23298467) directly
-
-3) Or use the following code to download it (without installing ORDerly). Make sure to install needed dependencies first (shown below).
-
-
-<details>
-<summary>Toggle to see code to download benchmark</summary>
-
-```pip install requests fastparquet pandas```
-
-```python
-import pathlib
-import zipfile
-
-import pandas as pd
-import requests
-
-
-def download_benchmark(
-    benchmark_zip_file="orderly_benchmark.zip",
-    benchmark_directory="orderly_benchmark/",
-    version=2,
-):
-    figshare_url = (
-        f"https://figshare.com/ndownloader/articles/23298467/versions/{version}"
-    )
-    print(f"Downloading benchmark from {figshare_url} to {benchmark_zip_file}")
-    r = requests.get(figshare_url, allow_redirects=True)
-    with open(benchmark_zip_file, "wb") as f:
-        f.write(r.content)
-
-    print("Unzipping benchmark")
-    benchmark_directory = pathlib.Path(benchmark_directory)
-    benchmark_directory.mkdir(parents=True, exist_ok=True)
-    with zipfile.ZipFile(benchmark_zip_file, "r") as zip_ref:
-        zip_ref.extractall(benchmark_directory)
-
-
-download_benchmark()
-train_df = pd.read_parquet("orderly_benchmark/orderly_benchmark_train.parquet")
-test_df = pd.read_parquet("orderly_benchmark/orderly_benchmark_test.parquet")
-```
-</details>
-
-
-
-📋 Reproducing results from paper
-------------------------------
-
-To reproduce the results from the paper, please clone the repository, and use poetry to install the requirements (see above). Towards the bottom of the makefile, you will find a comprehensive 8 step list of steps to generate all the datasets and reproduce all results presented in the paper. 
-
-### Results
-
-We run the condition prediction model on four different datasets, and find that trusting the labelling of the ORD data leads to overly confident test accuracy. We conclude that applying chemical logic to the reaction string is necessary to get a high-quality dataset, and that the best strategy for dealing with rare molecules is to delete reactions where they appear.
-
-Top-3 exact match combination accuracy (\%): frequency informed guess  // model prediction  //  AIB\%:
-
-| Dataset            | A (labeling; rare->"other")   | B (labeling; rare->delete rxn) | C (reaction string; rare->"other") | D (reaction string; rare->delete rxn) |
-|--------------------|--------------------------------|---------------------------------|------------------------------------|--------------------------------------|
-| Solvents           | 47 // 58 // 21%                | 50 // 61 // 22%                 | 23 // 42 // 26%                    | 24 // 45 // 28%                      |
-| Agents             | 54 // 70 // 35%                | 58 // 72 // 32%                 | 19 // 39 // 25%                    | 21 // 42 // 27%                      |
-| Solvents & Agents  | 31 // 44 // 19%                | 33 // 47 // 21%                 | 4 // 21 // 18%                     | 5 // 24 // 21%                       |
-
-Where AIB\% is the Average Improvement of the model over the Baseline (i.e. a frequency informed guess), where $A_m$ is the accuracy of the model, and $A_B$ is the accuracy of the baseline: 
-$`AIB = (A_m - A_b) / (1 - A_b)`$
-
-
-
-Full API documentation
-------------------------
-
-## Extraction
-There are two different ways to extract data from ORD files, trusting the labelling, or using the reaction string (as specified in the ```trust_labelling``` boolean). Below you see all the arguments that can be passed to the extraction script, change as appropriate:
-
-```python -m orderly.extract --name_contains_substring="uspto" --trust_labelling=False --output_path="data/orderly/uspto_no_trust" --consider_molecule_names=False```
-
-## Cleaning
-There are also a number of customisable steps for the cleaning:
-
-```python -m orderly.clean --output_path="data/orderly/datasets_$(dataset_version)/orderly_no_trust_no_map.parquet" --ord_extraction_path="data/orderly/uspto_no_trust/extracted_ords" --molecules_to_remove_path="data/orderly/uspto_no_trust/all_molecule_names.csv" --min_frequency_of_occurrence=100 --map_rare_molecules_to_other=False --set_unresolved_names_to_none_if_mapped_rxn_str_exists_else_del_rxn=True --remove_rxn_with_unresolved_names=False --set_unresolved_names_to_none=False --num_product=1 --num_reactant=2 --num_solv=2 --num_agent=3 --num_cat=0 --num_reag=0 --consistent_yield=True --scramble=True --train_test_split_fraction=0.9```
-
-A list of solvents (names and SMILES) commonly used in pharmaceutical chemistry can be found at orderly/data/solvents.csv
-
-
-## Issues?
-Submit an [issue](https://github.com/sustainable-processes/ORDerly/issues) or send an email to dsw46@cam.ac.uk.
-
-## Citing
-
-If you find this project useful, we encourage you to
-
-* Star this repository :star: 
-<!-- * Cite our [paper](https://chemistry-europe.onlinelibrary.wiley.com/doi/full/10.1002/cmtd.202000051).
-```
-@article{Felton2021,
-author = "Kobi Felton and Jan Rittig and Alexei Lapkin",
-title = "{Summit: Benchmarking Machine Learning Methods for Reaction Optimisation}",
-year = "2021",
-month = "2",
-url = "https://chemistry-europe.onlinelibrary.wiley.com/doi/full/10.1002/cmtd.202000051",
-journal = "Chemistry Methods"
-} 
-```-->
-
-
-
-
-<!-- ### 2. Run extraction
-
-We can run extraction using: ```poetry run python -m orderly.extract```. Using ```poetry run python -m orderly.extract --help``` will explain the arguments. Certain args must be set such as data paths.
-
-### 3. Run cleaning
-
-We can run cleaning using: ```poetry run python -m orderly.clean```. Using ```poetry run python -m orderly.clean --help``` will explain the arguments. Certain args must be set such as data paths. -->
-
+# ORDerly
+
+🧪 Cleaning chemical reaction data 🧪
+
+🎯 [Condition Prediction Benchmark](https://figshare.com/articles/dataset/ORDerly_chemical_reactions_condition_benchmarks/23298467) 🎯
+
+## Quick Install
+
+Requires Python 3.10 (Tested on MacOS and Linux)
+
+```pip install orderly```
+
+🤔 What is this?
+-----------------
+
+Machine learning has the potential to provide tremendous value to chemistry. However, large amounts of clean high-quality data are needed to train models
+
+ORDerly cleans chemical reaction data from the growing [Open Reaction Database (ORD)](https://docs.open-reaction-database.org/en/latest/).
+
+Use ORDerly to:
+- Extract and clean your own dataset from ORD
+- Access the [ORDerly condition prediction benchmark dataset](https://figshare.com/articles/dataset/ORDerly_chemical_reactions_condition_benchmarks/23298467) for reaction condition prediction.
+- Reproduce results from our paper including training a ML model to predict reaction conditions
+
+<img src="images/abstract_fig.png" alt="Abstract Figure" width="300">
+
+
+<!-- Section on extracting and cleaning a dataset-->
+
+📖 Extract and clean a dataset
+------------------------------
+ 
+### Download data from ORD
+
+<!-- ```python -m orderly.download.ord```
+
+This will create a folder called ```/data/ord/``` in your current directory, and download the data into ```ord/``` -->
+
+Data in ORD format should be placed in a folder called ```/data/ord/```. You can either use your own data, or the open-source ORD data.
+
+To download the ORD data follow the instructions on the [official website](https://github.com/open-reaction-database/ord-data) (i.e. download GitLFS and clone their repository) and then place it within a folder called ```/data/ord/```.
+
+### Extract data from the ORD files
+
+```python -m orderly.extract```
+
+If you want to run ORDerly on your own data, and want to specify the input and output path:
+
+```python -m orderly.extract --input_path="/data/ord/" --output_path="/data/orderly/"```
+
+This will generate a parquet file for each ORD file.
+
+### Clean the data
+
+This will produce train and test parquet files, along with a .json file showing the arguments used and a .log file showing the operations run.
+
+```python -m orderly.clean```
+
+<!-- Section on downloading the benchmark -->
+🚀 Download the condition prediction benchmark dataset
+--------------------------------------------------------
+
+Reaction condition prediction is the problem of predicting the things "above the arrow" in chemical reactions.
+
+<!-- Include image of a reactions -->
+
+There are three options for donwloading the benchmark.
+
+1) If you have orderly installed you can download the benchmark using this command:
+
+```python -m orderly.download.benchmark```
+
+2) Or you can either download the [ORDerly condition prediction benchmark dataset](https://figshare.com/articles/dataset/ORDerly_chemical_reactions_condition_benchmarks/23298467) directly
+
+3) Or use the following code to download it (without installing ORDerly). Make sure to install needed dependencies first (shown below).
+
+
+<details>
+<summary>Toggle to see code to download benchmark</summary>
+
+```pip install requests fastparquet pandas```
+
+```python
+import pathlib
+import zipfile
+
+import pandas as pd
+import requests
+
+
+def download_benchmark(
+    benchmark_zip_file="orderly_benchmark.zip",
+    benchmark_directory="orderly_benchmark/",
+    version=2,
+):
+    figshare_url = (
+        f"https://figshare.com/ndownloader/articles/23298467/versions/{version}"
+    )
+    print(f"Downloading benchmark from {figshare_url} to {benchmark_zip_file}")
+    r = requests.get(figshare_url, allow_redirects=True)
+    with open(benchmark_zip_file, "wb") as f:
+        f.write(r.content)
+
+    print("Unzipping benchmark")
+    benchmark_directory = pathlib.Path(benchmark_directory)
+    benchmark_directory.mkdir(parents=True, exist_ok=True)
+    with zipfile.ZipFile(benchmark_zip_file, "r") as zip_ref:
+        zip_ref.extractall(benchmark_directory)
+
+
+download_benchmark()
+train_df = pd.read_parquet("orderly_benchmark/orderly_benchmark_train.parquet")
+test_df = pd.read_parquet("orderly_benchmark/orderly_benchmark_test.parquet")
+```
+</details>
+
+
+
+📋 Reproducing results from paper
+------------------------------
+
+To reproduce the results from the paper, please clone the repository, and use poetry to install the requirements (see above). Towards the bottom of the makefile, you will find a comprehensive 8 step list of steps to generate all the datasets and reproduce all results presented in the paper. 
+
+### Results
+
+We run the condition prediction model on four different datasets, and find that trusting the labelling of the ORD data leads to overly confident test accuracy. We conclude that applying chemical logic to the reaction string is necessary to get a high-quality dataset, and that the best strategy for dealing with rare molecules is to delete reactions where they appear.
+
+Top-3 exact match combination accuracy (\%): frequency informed guess  // model prediction  //  AIB\%:
+
+| Dataset            | A (labeling; rare->"other")   | B (labeling; rare->delete rxn) | C (reaction string; rare->"other") | D (reaction string; rare->delete rxn) |
+|--------------------|--------------------------------|---------------------------------|------------------------------------|--------------------------------------|
+| Solvents           | 47 // 58 // 21%                | 50 // 61 // 22%                 | 23 // 42 // 26%                    | 24 // 45 // 28%                      |
+| Agents             | 54 // 70 // 35%                | 58 // 72 // 32%                 | 19 // 39 // 25%                    | 21 // 42 // 27%                      |
+| Solvents & Agents  | 31 // 44 // 19%                | 33 // 47 // 21%                 | 4 // 21 // 18%                     | 5 // 24 // 21%                       |
+
+Where AIB\% is the Average Improvement of the model over the Baseline (i.e. a frequency informed guess), where $A_m$ is the accuracy of the model, and $A_B$ is the accuracy of the baseline: 
+$`AIB = (A_m - A_b) / (1 - A_b)`$
+
+
+
+Full API documentation
+------------------------
+
+## Extraction
+There are two different ways to extract data from ORD files, trusting the labelling, or using the reaction string (as specified in the ```trust_labelling``` boolean). Below you see all the arguments that can be passed to the extraction script, change as appropriate:
+
+```python -m orderly.extract --name_contains_substring="uspto" --trust_labelling=False --output_path="data/orderly/uspto_no_trust" --consider_molecule_names=False```
+
+## Cleaning
+There are also a number of customisable steps for the cleaning:
+
+```python -m orderly.clean --output_path="data/orderly/datasets_$(dataset_version)/orderly_no_trust_no_map.parquet" --ord_extraction_path="data/orderly/uspto_no_trust/extracted_ords" --molecules_to_remove_path="data/orderly/uspto_no_trust/all_molecule_names.csv" --min_frequency_of_occurrence=100 --map_rare_molecules_to_other=False --set_unresolved_names_to_none_if_mapped_rxn_str_exists_else_del_rxn=True --remove_rxn_with_unresolved_names=False --set_unresolved_names_to_none=False --num_product=1 --num_reactant=2 --num_solv=2 --num_agent=3 --num_cat=0 --num_reag=0 --consistent_yield=True --scramble=True --train_test_split_fraction=0.9```
+
+A list of solvents (names and SMILES) commonly used in pharmaceutical chemistry can be found at orderly/data/solvents.csv
+
+
+## Issues?
+Submit an [issue](https://github.com/sustainable-processes/ORDerly/issues) or send an email to dsw46@cam.ac.uk.
+
+## Citing
+
+If you find this project useful, we encourage you to
+
+* Star this repository :star: 
+<!-- * Cite our [paper](https://chemistry-europe.onlinelibrary.wiley.com/doi/full/10.1002/cmtd.202000051).
+```
+@article{Felton2021,
+author = "Kobi Felton and Jan Rittig and Alexei Lapkin",
+title = "{Summit: Benchmarking Machine Learning Methods for Reaction Optimisation}",
+year = "2021",
+month = "2",
+url = "https://chemistry-europe.onlinelibrary.wiley.com/doi/full/10.1002/cmtd.202000051",
+journal = "Chemistry Methods"
+} 
+```-->
+
+
+
+
+<!-- ### 2. Run extraction
+
+We can run extraction using: ```poetry run python -m orderly.extract```. Using ```poetry run python -m orderly.extract --help``` will explain the arguments. Certain args must be set such as data paths.
+
+### 3. Run cleaning
+
+We can run cleaning using: ```poetry run python -m orderly.clean```. Using ```poetry run python -m orderly.clean --help``` will explain the arguments. Certain args must be set such as data paths. -->
+
```

### Comparing `orderly-0.0.2/tests/test_clean.py` & `orderly-0.1.0/tests/test_clean.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,1302 +1,1302 @@
-import pathlib
-from typing import Any, Dict, List, Optional, Tuple
-
-import pandas as pd
-import pytest
-
-
-def test_hello_world() -> None:
-    assert True
-
-
-@pytest.fixture
-def toy_dict() -> Dict[str, List[str]]:
-    toy_dict = {
-        "reactant_000": ["B", "A", "F", "A"],
-        "reactant_001": ["D", "A", pd.NA, "B"],
-        "product_000": ["C", "A", "E", "A"],
-        "product_001": ["E", "G", "C", "H"],
-        "agent_000": ["D", "F", "D", "B"],
-        "agent_001": ["C", "E", "G", "A"],
-        "solvent_000": ["E", "B", "G", "C"],
-        "solvent_001": ["C", "D", "B", "G"],
-        "solvent_002": ["D", "B", "F", "G"],
-    }
-
-    return toy_dict
-
-
-def get_cleaned_df(
-    output_path: pathlib.Path,
-    trust_labelling: bool,
-    consistent_yield: bool,
-    num_reactant: int,
-    num_product: int,
-    num_solv: int,
-    num_agent: int,
-    num_cat: int,
-    num_reag: int,
-    min_frequency_of_occurrence: int,
-    map_rare_molecules_to_other: bool,
-    set_unresolved_names_to_none_if_mapped_rxn_str_exists_else_del_rxn: bool,
-    set_unresolved_names_to_none: bool,
-    remove_rxn_with_unresolved_names: bool,
-    remove_reactions_with_no_reactants: bool,
-    remove_reactions_with_no_products: bool,
-    remove_reactions_with_no_solvents: bool,
-    remove_reactions_with_no_agents: bool,
-    remove_reactions_with_no_conditions: bool,
-    drop_duplicates: bool,
-) -> pd.DataFrame:
-    import orderly.clean.cleaner
-    import orderly.data.test_data
-
-    ord_extraction_path = (
-        orderly.data.test_data.get_path_of_test_extracted_ords(
-            trust_labelling=trust_labelling
-        )
-        / "extracted_ords"
-    )
-    molecules_to_remove_path = (
-        orderly.data.test_data.get_path_of_test_extracted_ords(
-            trust_labelling=trust_labelling
-        )
-        / "all_molecule_names.csv"
-    )
-
-    orderly.clean.cleaner.main(
-        output_path=output_path,
-        ord_extraction_path=ord_extraction_path,
-        molecules_to_remove_path=molecules_to_remove_path,
-        consistent_yield=consistent_yield,
-        num_reactant=num_reactant,
-        num_product=num_product,
-        num_solv=num_solv,
-        num_agent=num_agent,
-        num_cat=num_cat,
-        num_reag=num_reag,
-        min_frequency_of_occurrence=min_frequency_of_occurrence,
-        map_rare_molecules_to_other=map_rare_molecules_to_other,
-        set_unresolved_names_to_none_if_mapped_rxn_str_exists_else_del_rxn=set_unresolved_names_to_none_if_mapped_rxn_str_exists_else_del_rxn,
-        set_unresolved_names_to_none=set_unresolved_names_to_none,
-        remove_rxn_with_unresolved_names=remove_rxn_with_unresolved_names,
-        remove_reactions_with_no_reactants=remove_reactions_with_no_reactants,
-        remove_reactions_with_no_products=remove_reactions_with_no_products,
-        remove_reactions_with_no_solvents=remove_reactions_with_no_solvents,
-        remove_reactions_with_no_agents=remove_reactions_with_no_agents,
-        remove_reactions_with_no_conditions=remove_reactions_with_no_conditions,
-        scramble=False,
-        train_test_split_fraction=0,
-        drop_duplicates=drop_duplicates,
-        disable_tqdm=False,
-        overwrite=False,
-    )
-
-    import pandas as pd
-
-    return pd.read_parquet(output_path)
-
-
-@pytest.fixture
-def cleaned_df_params_default(
-    tmp_path: pathlib.Path, request: pytest.FixtureRequest
-) -> Tuple[pd.DataFrame, List[Any]]:
-    assert len(request.param) == 10
-    updated_args = request.param + [
-        True,
-        False,
-        False,
-        True,
-        True,
-        True,
-        True,
-        False,
-        True,
-    ]
-    # set_unresolved_names_to_none_if_mapped_rxn_str_exists_else_del_rxn: bool,
-    # set_unresolved_names_to_none: bool,
-    # remove_rxn_with_unresolved_names: bool,
-    # remove_reactions_with_no_reactants: bool,
-    # remove_reactions_with_no_products: bool,
-    # remove_reactions_with_no_solvents: bool,
-    # remove_reactions_with_no_agents: bool,
-    # remove_reactions_with_no_conditions: bool,
-    # drop_duplicates: bool
-    return (
-        get_cleaned_df(
-            tmp_path / "cleaned_df" / "orderly_ord.parquet",
-            *updated_args,
-        ),
-        request.param,
-    )
-
-
-@pytest.fixture
-def cleaned_df_params_default_without_min_freq(
-    tmp_path: pathlib.Path, request: pytest.FixtureRequest
-) -> Tuple[pd.DataFrame, List[Any]]:
-    import copy
-
-    args = copy.copy(request.param)
-    args[-2] = 0
-    assert len(request.param) == 10
-    updated_args = args + [
-        True,
-        False,
-        False,
-        True,
-        True,
-        True,
-        True,
-        False,
-        True,
-    ]
-    # set_unresolved_names_to_none_if_mapped_rxn_str_exists_else_del_rxn: bool,
-    # set_unresolved_names_to_none: bool,
-    # remove_rxn_with_unresolved_names: bool,
-    # remove_reactions_with_no_reactants: bool,
-    # remove_reactions_with_no_products: bool,
-    # remove_reactions_with_no_solvents: bool,
-    # remove_reactions_with_no_agents: bool,
-    # remove_reactions_with_no_conditions: bool,
-    # drop_duplicates: bool
-    return (
-        get_cleaned_df(
-            tmp_path
-            / "cleaned_df_params_default_without_min_freq"
-            / "orderly_ord.parquet",
-            *updated_args,
-        ),
-        args,
-    )
-
-
-@pytest.fixture
-def cleaned_df_params_retaining_unresolved_names_and_duplicates(
-    tmp_path: pathlib.Path, request: pytest.FixtureRequest
-) -> Tuple[pd.DataFrame, List[Any]]:
-    assert len(request.param) == 10
-    updated_args = request.param + [
-        False,
-        False,
-        False,
-        True,
-        True,
-        True,
-        True,
-        False,
-        False,
-    ]
-    # set_unresolved_names_to_none_if_mapped_rxn_str_exists_else_del_rxn: bool,
-    # set_unresolved_names_to_none: bool,
-    # remove_rxn_with_unresolved_names: bool,
-    # remove_reactions_with_no_reactants: bool,
-    # remove_reactions_with_no_products: bool,
-    # remove_reactions_with_no_solvents: bool,
-    # remove_reactions_with_no_agents: bool,
-    # remove_reactions_with_no_conditions: bool,
-    # drop_duplicates: bool
-
-    return (
-        get_cleaned_df(
-            tmp_path
-            / "cleaned_df_params_retaining_unresolved_names_and_duplicates"
-            / "orderly_ord.parquet",
-            *updated_args,
-        ),
-        request.param,
-    )
-
-
-@pytest.fixture
-def cleaned_df_params_retaining_unresolved_names_and_duplicates_without_min_freq(
-    tmp_path: pathlib.Path, request: pytest.FixtureRequest
-) -> Tuple[pd.DataFrame, List[Any]]:
-    import copy
-
-    args = copy.copy(request.param)
-    args[-2] = 0
-    assert len(request.param) == 10
-    updated_args = args + [
-        False,
-        False,
-        False,
-        True,
-        True,
-        True,
-        True,
-        False,
-        False,
-    ]
-    # set_unresolved_names_to_none_if_mapped_rxn_str_exists_else_del_rxn: bool,
-    # set_unresolved_names_to_none: bool,
-    # remove_rxn_with_unresolved_names: bool,
-    # remove_reactions_with_no_reactants: bool,
-    # remove_reactions_with_no_products: bool,
-    # remove_reactions_with_no_solvents: bool,
-    # remove_reactions_with_no_agents: bool,
-    # remove_reactions_with_no_conditions: bool,
-    # drop_duplicates: bool
-    return (
-        get_cleaned_df(
-            tmp_path
-            / "cleaned_df_params_retaining_unresolved_names_and_duplicates_without_min_freq"
-            / "orderly_ord.parquet",
-            *updated_args,
-        ),
-        args,
-    )
-
-
-def test_molecule_names_not_empty() -> None:
-    import os
-    import pathlib
-
-    import pandas as pd
-
-    import orderly.data.util
-    from orderly.data.test_data import get_path_of_molecule_names
-
-    all_empty = True
-
-    molecule_names_folder_path = get_path_of_molecule_names()
-
-    files = os.listdir(molecule_names_folder_path)
-    for file in files:
-        if file.endswith(".csv"):  # or file.endswith(".parquet")
-            file_path = pathlib.Path(os.path.join(molecule_names_folder_path, file))
-            molecule_names_list = orderly.data.util.load_list(path=file_path)
-            if len(molecule_names_list) > 0:
-                all_empty = False
-    assert not all_empty
-
-
-@pytest.mark.parametrize(
-    "columns_to_count_from, expected_total_value_counts",
-    (
-        pytest.param(
-            [
-                "reactant_000",
-                "reactant_001",
-                "product_000",
-                "product_001",
-                "agent_000",
-                "agent_001",
-                "solvent_000",
-                "solvent_001",
-                "solvent_002",
-            ],
-            {"A": 6, "B": 6, "C": 5, "D": 5, "E": 4, "F": 3, "G": 5, "H": 1},
-            id="all_columns",
-        ),
-        pytest.param(
-            ["agent_000", "agent_001", "solvent_000", "solvent_001", "solvent_002"],
-            {"A": 1, "B": 4, "C": 3, "D": 4, "E": 2, "F": 2, "G": 4},
-            id="agent_and_solvent_columns",
-        ),
-    ),
-)
-def test_get_value_counts(
-    toy_dict: Dict[str, List[str]],
-    columns_to_count_from: List[str],
-    expected_total_value_counts: Dict[str, int],
-) -> None:
-    import copy
-
-    import pandas as pd
-
-    import orderly.clean.cleaner
-
-    toy_dict = copy.copy(toy_dict)
-
-    df = pd.DataFrame(toy_dict)
-
-    total_value_counts = orderly.clean.cleaner.Cleaner._get_value_counts(
-        df, columns_to_count_from
-    )
-
-    expected_total_value_counts = pd.Series(expected_total_value_counts).sort_values(
-        ascending=False
-    )
-
-    assert total_value_counts.equals(
-        pd.Series(expected_total_value_counts)
-    ), f"Got: {total_value_counts}, expected: {expected_total_value_counts},"
-
-
-def test_scramble(
-    toy_dict: Dict[str, List[str]],
-) -> None:
-    import copy
-
-    import pandas as pd
-
-    import orderly.clean.cleaner
-
-    toy_dict = copy.copy(toy_dict)
-
-    df = pd.DataFrame(toy_dict)
-    components = ("reactant", "agent", "solvent", "catalyst", "reagent")
-
-    scrambled_df = orderly.clean.cleaner.Cleaner._scramble(df, components)
-
-    assert not scrambled_df.equals(
-        df
-    ), f"Got: {scrambled_df}, expected to be different from: {df},"
-
-    # check that molecules have only been moved around within the same reaction (i.e. the same row)
-    rows_to_check = min(10, len(df))
-    for i in range(rows_to_check):
-        sorted_row_components = set(df.iloc[i])
-        scrambled_row_components = set(scrambled_df.iloc[i])
-        assert (
-            sorted_row_components == scrambled_row_components
-        ), f"Got: {sorted_row_components}, expected: {scrambled_row_components},"
-
-
-@pytest.mark.parametrize(
-    "component_name, number_of_columns_to_keep, expected_dict",
-    (
-        # Del reactions with too many reactants
-        pytest.param(
-            "reactant",
-            1,
-            {
-                "reactant_000": ["F"],
-                "product_000": ["E"],
-                "product_001": ["C"],
-                "agent_000": ["D"],
-                "agent_001": ["G"],
-                "solvent_000": ["G"],
-                "solvent_001": ["B"],
-                "solvent_002": ["F"],
-            },
-        ),
-        # Add a component
-        pytest.param(
-            "reactant",
-            3,
-            {
-                "reactant_000": ["B", "A", "F", "A"],
-                "reactant_001": ["D", "A", pd.NA, "B"],
-                "reactant_002": [pd.NA, pd.NA, pd.NA, pd.NA],
-                "product_000": ["C", "A", "E", "A"],
-                "product_001": ["E", "G", "C", "H"],
-                "agent_000": ["D", "F", "D", "B"],
-                "agent_001": ["C", "E", "G", "A"],
-                "solvent_000": ["E", "B", "G", "C"],
-                "solvent_001": ["C", "D", "B", "G"],
-                "solvent_002": ["D", "B", "F", "G"],
-            },
-        ),
-        # Add two component
-        pytest.param(
-            "reactant",
-            4,
-            {
-                "reactant_000": ["B", "A", "F", "A"],
-                "reactant_001": ["D", "A", pd.NA, "B"],
-                "reactant_002": [pd.NA, pd.NA, pd.NA, pd.NA],
-                "reactant_003": [pd.NA, pd.NA, pd.NA, pd.NA],
-                "product_000": ["C", "A", "E", "A"],
-                "product_001": ["E", "G", "C", "H"],
-                "agent_000": ["D", "F", "D", "B"],
-                "agent_001": ["C", "E", "G", "A"],
-                "solvent_000": ["E", "B", "G", "C"],
-                "solvent_001": ["C", "D", "B", "G"],
-                "solvent_002": ["D", "B", "F", "G"],
-            },
-        ),
-        # Do nothing
-        pytest.param(
-            "reactant",
-            2,
-            {
-                "reactant_000": ["B", "A", "F", "A"],
-                "reactant_001": ["D", "A", pd.NA, "B"],
-                "product_000": ["C", "A", "E", "A"],
-                "product_001": ["E", "G", "C", "H"],
-                "agent_000": ["D", "F", "D", "B"],
-                "agent_001": ["C", "E", "G", "A"],
-                "solvent_000": ["E", "B", "G", "C"],
-                "solvent_001": ["C", "D", "B", "G"],
-                "solvent_002": ["D", "B", "F", "G"],
-            },
-        ),
-        # Do nothing
-        pytest.param(
-            "reactant",
-            -1,
-            {
-                "reactant_000": ["B", "A", "F", "A"],
-                "reactant_001": ["D", "A", pd.NA, "B"],
-                "product_000": ["C", "A", "E", "A"],
-                "product_001": ["E", "G", "C", "H"],
-                "agent_000": ["D", "F", "D", "B"],
-                "agent_001": ["C", "E", "G", "A"],
-                "solvent_000": ["E", "B", "G", "C"],
-                "solvent_001": ["C", "D", "B", "G"],
-                "solvent_002": ["D", "B", "F", "G"],
-            },
-        ),
-    ),
-)
-def test_remove_reactions_with_too_many_of_component(
-    toy_dict: Dict[str, List[str]],
-    component_name: str,
-    number_of_columns_to_keep: int,
-    expected_dict: Dict[str, int],
-) -> None:
-    import copy
-
-    import pandas as pd
-
-    import orderly.clean.cleaner
-
-    toy_dict = copy.copy(toy_dict)
-
-    df = pd.DataFrame(toy_dict)
-
-    filtered_df = (
-        orderly.clean.cleaner.Cleaner._remove_reactions_with_too_many_of_component(
-            df=df,
-            component_name=component_name,
-            number_of_columns_to_keep=number_of_columns_to_keep,
-        )
-    )
-
-    expected_filtered_df = pd.DataFrame(expected_dict).sort_index(axis=1)
-    if filtered_df.empty:
-        assert filtered_df.empty == expected_filtered_df.empty
-    else:
-        assert filtered_df.equals(
-            expected_filtered_df
-        ), f"Got: {filtered_df}, expected: {expected_filtered_df},"
-
-
-@pytest.mark.parametrize(
-    "columns_to_transform, value_counts_dict, min_frequency_of_occurrence, expected_dict,",
-    (
-        pytest.param(
-            [
-                "reactant_000",
-                "reactant_001",
-                "product_000",
-                "product_001",
-                "agent_000",
-                "agent_001",
-                "solvent_000",
-                "solvent_001",
-                "solvent_002",
-            ],
-            {"A": 6, "B": 6, "C": 5, "D": 5, "E": 4, "F": 3, "G": 5, "H": 1},
-            4,
-            {
-                "reactant_000": ["B", "A", "other", "A"],
-                "reactant_001": ["D", "A", pd.NA, "B"],
-                "product_000": ["C", "A", "E", "A"],
-                "product_001": ["E", "G", "C", "other"],
-                "agent_000": ["D", "other", "D", "B"],
-                "agent_001": ["C", "E", "G", "A"],
-                "solvent_000": ["E", "B", "G", "C"],
-                "solvent_001": ["C", "D", "B", "G"],
-                "solvent_002": ["D", "B", "other", "G"],
-            },
-            id="all_columns",
-        ),
-        pytest.param(
-            ["agent_000", "agent_001", "solvent_000", "solvent_001", "solvent_002"],
-            {"A": 1, "B": 4, "C": 3, "D": 4, "E": 2, "F": 2, "G": 3},
-            3,
-            {
-                "reactant_000": ["B", "A", "F", "A"],
-                "reactant_001": ["D", "A", pd.NA, "B"],
-                "product_000": ["C", "A", "E", "A"],
-                "product_001": ["E", "G", "C", "H"],
-                "agent_000": ["D", "other", "D", "B"],
-                "agent_001": ["C", "other", "G", "other"],
-                "solvent_000": ["other", "B", "G", "C"],
-                "solvent_001": ["C", "D", "B", "G"],
-                "solvent_002": ["D", "B", "other", "G"],
-            },
-            id="agent_and_solvent_columns",
-        ),
-    ),
-)
-def test_map_rare_molecules_to_other(
-    toy_dict: Dict[str, List[str]],
-    columns_to_transform: List[str],
-    value_counts_dict: Dict[str, int],
-    min_frequency_of_occurrence: int,
-    expected_dict: Dict[str, List[str]],
-) -> None:
-    import copy
-
-    import pandas as pd
-
-    import orderly.clean.cleaner
-
-    toy_dict = copy.copy(toy_dict)
-
-    df = pd.DataFrame(toy_dict)
-    value_counts_series = pd.Series(value_counts_dict)
-
-    df = orderly.clean.cleaner.Cleaner._map_rare_molecules_to_other(
-        df, columns_to_transform, value_counts_series, min_frequency_of_occurrence
-    )
-
-    expected_df = pd.DataFrame(expected_dict)
-
-    assert df.equals(expected_df), f"Got: {df}, expected: {expected_df},"
-
-
-@pytest.mark.parametrize(
-    "toy_dict, target_strings, expected_dict,",
-    (
-        pytest.param(
-            {
-                "reactant_000": [
-                    "a",
-                    None,
-                    None,
-                    "a",
-                ],
-                "reactant_001": [
-                    None,
-                    "a",
-                    None,
-                    "b",
-                ],
-                "reactant_002": [
-                    "b",
-                    "b",
-                    "a",
-                    "c",
-                ],
-                "agent_000": [
-                    "a",
-                    "a",
-                    None,
-                    None,
-                ],
-                "agent_001": [
-                    None,
-                    "b",
-                    "a",
-                    None,
-                ],
-                "agent_002": [
-                    "b",
-                    "c",
-                    "b",
-                    None,
-                ],
-            },
-            ("reactant", "product", "agent", "solvent"),
-            {
-                "reactant_000": [
-                    "a",
-                    "a",
-                    "a",
-                    "a",
-                ],
-                "reactant_001": [
-                    "b",
-                    "b",
-                    None,
-                    "b",
-                ],
-                "reactant_002": [
-                    None,
-                    None,
-                    None,
-                    "c",
-                ],
-                "agent_000": [
-                    "a",
-                    "a",
-                    "a",
-                    None,
-                ],
-                "agent_001": [
-                    "b",
-                    "b",
-                    "b",
-                    None,
-                ],
-                "agent_002": [
-                    None,
-                    "c",
-                    None,
-                    None,
-                ],
-            },
-        ),
-        pytest.param(
-            {
-                "product_000": [
-                    "a",
-                    "a",
-                    None,
-                    None,
-                ],
-                "product_001": [
-                    None,
-                    "b",
-                    "a",
-                    None,
-                ],
-                "product_002": [
-                    "b",
-                    "c",
-                    "b",
-                    None,
-                ],
-                "yield_000": [
-                    "a",
-                    "a",
-                    "c",
-                    None,
-                ],
-                "yield_001": [
-                    None,
-                    "b",
-                    "a",
-                    None,
-                ],
-                "yield_002": [
-                    "b",
-                    "c",
-                    "b",
-                    None,
-                ],
-            },
-            ("product",),
-            {
-                "product_000": [
-                    "a",
-                    "a",
-                    "a",
-                    None,
-                ],
-                "product_001": [
-                    "b",
-                    "b",
-                    "b",
-                    None,
-                ],
-                "product_002": [
-                    None,
-                    "c",
-                    None,
-                    None,
-                ],
-                "yield_000": [
-                    "a",
-                    "a",
-                    "a",
-                    None,
-                ],
-                "yield_001": [
-                    "b",
-                    "b",
-                    "b",
-                    None,
-                ],
-                "yield_002": [
-                    None,
-                    "c",
-                    "c",
-                    None,
-                ],
-            },
-        ),
-    ),
-)
-def test_move_none_to_after_data(
-    toy_dict: Dict[str, List[str]],
-    target_strings: Tuple[str, ...],
-    expected_dict: Dict[str, List[str]],
-) -> None:
-    import copy
-
-    import pandas as pd
-
-    import orderly.clean.cleaner
-
-    toy_dict = copy.copy(toy_dict)
-
-    df = pd.DataFrame(toy_dict)
-
-    df = orderly.clean.cleaner.Cleaner._move_none_to_after_data(df, target_strings)
-
-    expected_df = pd.DataFrame(expected_dict)
-
-    assert df.equals(expected_df), f"Got: \n{df}, expected: \n{expected_df},"
-
-
-@pytest.mark.parametrize(
-    "columns_to_transform, value_counts_dict, min_frequency_of_occurrence, expected_dict,",
-    (
-        pytest.param(
-            [
-                "reactant_000",
-                "reactant_001",
-                "product_000",
-                "product_001",
-                "agent_000",
-                "agent_001",
-                "solvent_000",
-                "solvent_001",
-                "solvent_002",
-            ],
-            {"A": 6, "B": 6, "C": 5, "D": 5, "E": 4, "F": 3, "G": 6, "H": 1},
-            4,
-            {
-                "reactant_000": ["B"],
-                "reactant_001": ["D"],
-                "product_000": ["C"],
-                "product_001": ["E"],
-                "agent_000": ["D"],
-                "agent_001": ["C"],
-                "solvent_000": ["E"],
-                "solvent_001": ["C"],
-                "solvent_002": ["D"],
-            },
-            id="all_columns",
-        ),
-        pytest.param(
-            ["agent_000", "agent_001", "solvent_000", "solvent_001", "solvent_002"],
-            {"A": 1, "B": 4, "C": 3, "D": 4, "E": 2, "F": 2, "G": 4},
-            2,
-            {
-                "reactant_000": ["B", "A", "F"],
-                "reactant_001": ["D", "A", pd.NA],
-                "product_000": ["C", "A", "E"],
-                "product_001": ["E", "G", "C"],
-                "agent_000": ["D", "F", "D"],
-                "agent_001": ["C", "E", "G"],
-                "solvent_000": ["E", "B", "G"],
-                "solvent_001": ["C", "D", "B"],
-                "solvent_002": ["D", "B", "F"],
-            },
-            id="agent_and_solvent_columns",
-        ),
-    ),
-)
-def test_remove_rare_molecules(
-    toy_dict: Dict[str, List[str]],
-    columns_to_transform: List[str],
-    value_counts_dict: Dict[str, int],
-    min_frequency_of_occurrence: int,
-    expected_dict: Dict[str, List[str]],
-) -> None:
-    import copy
-
-    import pandas as pd
-
-    import orderly.clean.cleaner
-
-    toy_dict = copy.copy(toy_dict)
-
-    df = pd.DataFrame(toy_dict)
-    value_counts_series = pd.Series(value_counts_dict)
-
-    df = orderly.clean.cleaner.Cleaner._remove_rare_molecules(
-        df, columns_to_transform, value_counts_series, min_frequency_of_occurrence
-    )
-
-    expected_df = pd.DataFrame(expected_dict)
-
-    assert df.equals(expected_df), f"Got: {df}, expected: {expected_df},"
-
-
-@pytest.mark.parametrize(
-    "cleaned_df_params_default",
-    (
-        pytest.param(
-            [False, False, 5, 5, 2, 3, 0, 0, 55, False],
-            id="trust_labelling:F|consistent_yield:F|map_rare_molecules_to_other:F",
-        ),
-        pytest.param(
-            [True, False, 5, 5, 2, 0, 2, 1, 15, False],
-            id="trust_labelling:T|consistent_yield:F|map_rare_molecules_to_other:F",
-        ),
-        pytest.param(
-            [False, True, 5, 5, 2, 3, 0, 0, 15, False],
-            id="trust_labelling:F|consistent_yield:T|map_rare_molecules_to_other:F",
-        ),
-        pytest.param(
-            [False, False, 5, 5, 2, 3, 0, 0, 15, True],
-            id="trust_labelling:F|consistent_yield:F|map_rare_molecules_to_other:T",
-        ),
-        pytest.param(
-            [True, True, 5, 5, 2, 0, 2, 1, 15, False],
-            id="trust_labelling:T|consistent_yield:T|map_rare_molecules_to_other:F",
-        ),
-        pytest.param(
-            [True, False, 5, 5, 2, 0, 2, 1, 15, True],
-            id="trust_labelling:T|consistent_yield:F|map_rare_molecules_to_other:T",
-        ),
-        pytest.param(
-            [False, True, 5, 5, 2, 3, 0, 0, 15, True],
-            id="trust_labelling:F|consistent_yield:T|map_rare_molecules_to_other:T",
-        ),
-        pytest.param(
-            [True, True, 5, 5, 2, 0, 2, 1, 15, True],
-            id="trust_labelling:T|consistent_yield:T|map_rare_molecules_to_other:T",
-        ),
-    ),
-    indirect=True,
-)
-def test_get_cleaned_df(
-    cleaned_df_params_default: Tuple[pd.DataFrame, List[Any]]
-) -> None:
-    import copy
-
-    cleaned_df, _ = copy.copy(cleaned_df_params_default)
-    assert not cleaned_df.empty
-    # TODO: check that there's only NaN or NaT, but no None
-
-
-@pytest.mark.parametrize(
-    "cleaned_df_params_default",
-    (
-        pytest.param(
-            [False, False, 5, 5, 2, 3, 0, 0, 15, False],
-            id="trust_labelling:F|consistent_yield:F|map_rare_molecules_to_other:F",
-        ),
-        pytest.param(
-            [True, False, 5, 5, 2, 0, 2, 1, 15, False],
-            id="trust_labelling:T|consistent_yield:F|map_rare_molecules_to_other:F",
-        ),
-        pytest.param(
-            [False, True, 5, 5, 2, 3, 0, 0, 15, False],
-            id="trust_labelling:F|consistent_yield:T|map_rare_molecules_to_other:F",
-        ),
-        pytest.param(
-            [False, False, 5, 5, 2, 3, 0, 0, 15, True],
-            id="trust_labelling:F|consistent_yield:F|map_rare_molecules_to_other:T",
-        ),
-        pytest.param(
-            [True, True, 5, 5, 2, 0, 2, 1, 15, False],
-            id="trust_labelling:T|consistent_yield:T|map_rare_molecules_to_other:F",
-        ),
-        pytest.param(
-            [True, False, 5, 5, 2, 0, 2, 1, 15, True],
-            id="trust_labelling:T|consistent_yield:F|map_rare_molecules_to_other:T",
-        ),
-        pytest.param(
-            [False, True, 5, 5, 2, 3, 0, 0, 15, True],
-            id="trust_labelling:F|consistent_yield:T|map_rare_molecules_to_other:T",
-        ),
-        pytest.param(
-            [True, True, 5, 5, 2, 0, 2, 1, 15, True],
-            id="trust_labelling:T|consistent_yield:T|map_rare_molecules_to_other:T",
-        ),
-        # XFAILS
-        pytest.param(
-            [False, True, 5, 5, 5, 5, 5, 5, 5, True],
-            marks=pytest.mark.xfail(
-                reason="AssertionError: Invalid input: If trust_labelling=True in orderly.extract, then num_cat and num_reag must be 0. If trust_labelling=False, then num_agent must be 0."
-            ),
-            id="trust_labelling:F|consistent_yield:T|map_rare_molecules_to_other:F|fives",
-        ),
-    ),
-    indirect=True,
-)
-def test_number_of_columns_and_order_of_None(
-    cleaned_df_params_default: Tuple[pd.DataFrame, List[Any]]
-) -> None:
-    import copy
-
-    import numpy as np
-
-    cleaned_df, params = copy.copy(cleaned_df_params_default)
-
-    (
-        _,
-        _,
-        num_reactant,
-        num_product,
-        num_solv,
-        num_agent,
-        num_cat,
-        num_reag,
-        _,
-        _,
-    ) = params
-
-    # check that the number of columns is correct
-    num_reactant_cols = 0
-    num_product_cols = 0
-    num_agent_cols = 0
-    num_cat_cols = 0
-    num_reag_cols = 0
-    num_solv_cols = 0
-
-    cols = cleaned_df.columns
-    for col in cols:
-        if col.startswith("react"):
-            num_reactant_cols += 1
-        elif col.startswith("prod"):
-            num_product_cols += 1
-        elif col.startswith("agent"):
-            num_agent_cols += 1
-        elif col.startswith("cat"):
-            num_cat_cols += 1
-        elif col.startswith("reag"):
-            num_reag_cols += 1
-        elif col.startswith("solv"):
-            num_solv_cols += 1
-
-    # if num_reactant == -1 we just include all reactant columns (and same for the others)
-    assert (num_reactant_cols == num_reactant) or num_reactant == -1
-    assert (num_product_cols == num_product) or num_product == -1
-    assert (num_agent_cols == num_agent) or num_agent == -1
-    assert (num_cat_cols == num_cat) or num_cat == -1
-    assert (num_reag_cols == num_reag) or num_reag == -1
-    assert (num_solv_cols == num_solv) or num_solv == -1
-
-    assert "grant_date" in cols
-    assert "date_of_experiment" in cols
-
-    import numpy as np
-
-    grant_date = cleaned_df["grant_date"].replace({None: np.nan})
-    date_of_experiment = cleaned_df["date_of_experiment"].replace({None: np.nan})
-    if not grant_date.dropna().empty:
-        assert pd.api.types.is_datetime64_ns_dtype(
-            grant_date
-        ), f"failure for grant_date: {cleaned_df['grant_date'].dtype}"
-    if not date_of_experiment.dropna().empty:
-        assert pd.api.types.is_datetime64_ns_dtype(
-            date_of_experiment
-        ), f"failure for date_of_experiment: {cleaned_df['date_of_experiment'].dtype}"
-
-    # Check that grant_date and date_of_experiment columns are either dtype = datetime64 or full of None
-    datetime_coumns = cleaned_df.select_dtypes(include=[np.datetime64])
-    assert ("grant_date" in datetime_coumns.columns) or (
-        len(cleaned_df["grant_date"].dropna()) == 0
-    )
-    assert ("date_of_experiment" in datetime_coumns.columns) or (
-        len(cleaned_df["date_of_experiment"].dropna()) == 0
-    )
-
-    # Also check that there are no instances of None before data in the cleaned df
-
-    def _get_columns_beginning_with_str(
-        columns: List[str], target_strings: Optional[Tuple[str, ...]] = None
-    ) -> List[str]:
-        """goes through the column in a dataframe and adds columns that start with a string in the target strings"""
-        if target_strings is None:
-            target_strings = (
-                "agent",
-                "solvent",
-                "reagent",
-                "catalyst",
-                "product",
-                "reactant",
-            )
-
-        return sorted([col for col in columns if col.startswith(target_strings)])
-
-    target_strings = (
-        "agent",
-        "solvent",
-        "reagent",
-        "catalyst",
-        "product",
-        "reactant",
-    )
-
-    def check_valid_order(row: pd.Series) -> pd.Series:
-        seen_none = False
-        for idx, a in enumerate(row):
-            current_isna = pd.isna(a) or (a == "")
-            if seen_none:
-                if not current_isna:
-                    raise ValueError(f"Unexpected order at {idx=} for {row.tolist()=}")
-            if current_isna:
-                seen_none = True
-        return row
-
-    for target_string in target_strings:
-        target_columns = _get_columns_beginning_with_str(
-            columns=cleaned_df.columns,
-            target_strings=(target_string,),
-        )
-        # check that there are no instances of None before data in the cleaned df
-        for idx, row in cleaned_df.loc[:, target_columns].iterrows():
-            check_valid_order(row)
-        # cleaned_df.loc[:, target_columns].apply(check_valid_order, axis=1)
-
-
-def double_list(
-    x: List[Any],
-) -> Tuple[List[Any], List[Any]]:
-    return (x, x)
-
-
-@pytest.mark.parametrize(
-    "cleaned_df_params_default,cleaned_df_params_default_without_min_freq",
-    (
-        pytest.param(
-            *double_list([False, False, 5, 5, 2, 3, 0, 0, 15, False]),
-            id="trust_labelling:F|consistent_yield:F|map_rare_molecules_to_other:F|15",
-        ),
-        pytest.param(
-            *double_list([False, False, 5, 5, 2, 3, 0, 0, 100, False]),
-            id="trust_labelling:F|consistent_yield:F|map_rare_molecules_to_other:F|100",
-        ),
-        pytest.param(
-            *double_list([True, False, 5, 5, 2, 0, 2, 1, 15, False]),
-            id="trust_labelling:T|consistent_yield:F|map_rare_molecules_to_other:F",
-        ),
-        pytest.param(
-            *double_list([False, True, 5, 5, 2, 3, 0, 0, 15, False]),
-            id="trust_labelling:F|consistent_yield:T|map_rare_molecules_to_other:F",
-        ),
-        pytest.param(
-            *double_list([False, False, 5, 5, 2, 3, 0, 0, 15, True]),
-            id="trust_labelling:F|consistent_yield:F|map_rare_molecules_to_other:T",
-        ),
-        pytest.param(
-            *double_list([True, True, 5, 5, 2, 0, 2, 1, 15, False]),
-            id="trust_labelling:T|consistent_yield:T|map_rare_molecules_to_other:F",
-        ),
-        pytest.param(
-            *double_list([True, False, 5, 5, 2, 0, 2, 1, 15, True]),
-            id="trust_labelling:T|consistent_yield:F|map_rare_molecules_to_other:T",
-        ),
-        pytest.param(
-            *double_list([False, True, 5, 5, 2, 3, 0, 0, 15, True]),
-            id="trust_labelling:F|consistent_yield:T|map_rare_molecules_to_other:T",
-        ),
-        pytest.param(
-            *double_list([True, True, 5, 5, 2, 0, 2, 1, 15, True]),
-            id="trust_labelling:T|consistent_yield:T|map_rare_molecules_to_other:T",
-        ),
-        # XFAILS
-        pytest.param(
-            *double_list([False, True, 5, 5, 5, 5, 5, 5, 5, True]),
-            marks=pytest.mark.xfail(
-                reason="AssertionError: Invalid input: If trust_labelling=True in orderly.extract, then num_cat and num_reag must be 0. If trust_labelling=False, then num_agent must be 0."
-            ),
-            id="trust_labelling:F|consistent_yield:T|map_rare_molecules_to_other:F|fives",
-        ),
-    ),
-    indirect=True,
-)
-def test_frequency_params_default(
-    cleaned_df_params_default: Tuple[pd.DataFrame, List[Any]],
-    cleaned_df_params_default_without_min_freq: Tuple[pd.DataFrame, List[Any]],
-) -> None:
-    """
-    Test that there are no rare molecules left in the dataset after the cleaning process. There may be molecules appearing less often than the minimum frequency of occurrence, even after the cleaning, but this is because when deleting rows with rare values we may cause new molecules to become rare; this is why we check for the intersection of the two dfs at the very end of the test.
-    """
-
-    import copy
-
-    cleaned_df, params = copy.copy(cleaned_df_params_default)
-    uncleaned_df, unclean_params = copy.copy(cleaned_df_params_default_without_min_freq)
-
-    assert len(params) == len(unclean_params)
-    assert unclean_params[-2] == 0
-    assert len(params) == 10
-    min_frequency_of_occurrence = params[-2]
-
-    import pandas as pd
-
-    def get_value_counts(df: pd.DataFrame) -> pd.Series:
-        # Define the list of columns to check
-        columns_to_check = [
-            col
-            for col in df.columns
-            if col.startswith(("agent", "solvent", "reagent", "catalyst"))
-        ]
-
-        # Initialize a list to store the results
-        results = []
-
-        # Loop through the columns
-        for col in columns_to_check:
-            # Get the value counts for the column
-            results += [df[col].value_counts()]
-
-        total_value_counts = (
-            pd.concat(results, axis=0, sort=True).groupby(level=0).sum()
-        )
-        if "other" in total_value_counts.index:
-            total_value_counts = total_value_counts.drop("other")
-        total_value_counts = total_value_counts.sort_values(ascending=True)
-        return total_value_counts
-
-    cleaned_value_counts = get_value_counts(df=cleaned_df.copy())
-    uncleaned_value_counts = get_value_counts(df=uncleaned_df.copy())
-
-    assert min_frequency_of_occurrence > 0  # sanity check the copying worked
-    assert "" not in cleaned_value_counts.keys()  # check there are no empty strings
-    assert "" not in uncleaned_value_counts.keys()  # check there are no empty strings
-
-    cleaned_rare = cleaned_value_counts[
-        cleaned_value_counts < min_frequency_of_occurrence
-    ]
-    uncleaned_rare = uncleaned_value_counts[
-        uncleaned_value_counts < min_frequency_of_occurrence
-    ]
-
-    if not cleaned_rare.empty:
-        assert uncleaned_rare.index.intersection(cleaned_value_counts.index).empty
-
-
-@pytest.mark.parametrize(
-    "cleaned_df_params_retaining_unresolved_names_and_duplicates,cleaned_df_params_retaining_unresolved_names_and_duplicates_without_min_freq",
-    (
-        pytest.param(
-            *double_list([False, False, 5, 5, 2, 3, 0, 0, 15, False]),
-            id="trust_labelling:F|consistent_yield:F|map_rare_molecules_to_other:F|15",
-        ),
-        pytest.param(
-            *double_list([False, False, 5, 5, 2, 3, 0, 0, 100, False]),
-            id="trust_labelling:F|consistent_yield:F|map_rare_molecules_to_other:F|100",
-        ),
-        pytest.param(
-            *double_list([True, False, 5, 5, 2, 0, 2, 1, 15, False]),
-            id="trust_labelling:T|consistent_yield:F|map_rare_molecules_to_other:F",
-        ),
-        pytest.param(
-            *double_list([False, True, 5, 5, 2, 3, 0, 0, 15, False]),
-            id="trust_labelling:F|consistent_yield:T|map_rare_molecules_to_other:F",
-        ),
-        pytest.param(
-            *double_list([True, True, 5, 5, 2, 0, 2, 1, 15, False]),
-            id="trust_labelling:T|consistent_yield:T|map_rare_molecules_to_other:F",
-        ),
-        pytest.param(
-            *double_list([False, False, 5, 5, 2, 3, 0, 0, 15, True]),
-            id="trust_labelling:F|consistent_yield:F|map_rare_molecules_to_other:T",
-        ),
-        pytest.param(
-            *double_list([True, False, 5, 5, 2, 0, 2, 1, 15, True]),
-            id="trust_labelling:T|consistent_yield:F|map_rare_molecules_to_other:T",
-        ),
-        pytest.param(
-            *double_list([False, True, 5, 5, 2, 3, 0, 0, 15, True]),
-            id="trust_labelling:F|consistent_yield:T|map_rare_molecules_to_other:T",
-        ),
-        pytest.param(
-            *double_list([True, True, 5, 5, 2, 0, 2, 1, 15, True]),
-            id="trust_labelling:T|consistent_yield:T|map_rare_molecules_to_other:T",
-        ),
-    ),
-    indirect=True,
-)
-def test_frequency_retaining_unresolved_names_and_duplicates(
-    cleaned_df_params_retaining_unresolved_names_and_duplicates: Tuple[
-        pd.DataFrame, List[Any]
-    ],
-    cleaned_df_params_retaining_unresolved_names_and_duplicates_without_min_freq: Tuple[
-        pd.DataFrame, List[Any]
-    ],
-) -> None:
-    """
-    Test that there are no rare molecules left in the dataset after the cleaning process. There may be molecules appearing less often than the minimum frequency of occurrence, even after the cleaning, but this is because when deleting rows with rare values we may cause new molecules to become rare; this is why we check for the intersection of the two dfs at the very end of the test.
-
-    In this test we retain duplicate reactions and unresolved names (e.g. english names for molecules that aren't in our manual mapping).
-    """
-    import copy
-
-    cleaned_df, params = copy.copy(
-        cleaned_df_params_retaining_unresolved_names_and_duplicates
-    )
-    uncleaned_df, unclean_params = copy.copy(
-        cleaned_df_params_retaining_unresolved_names_and_duplicates_without_min_freq
-    )
-
-    assert len(params) == len(unclean_params)
-    assert unclean_params[-2] == 0
-    assert len(params) == 10
-    min_frequency_of_occurrence = params[-2]
-
-    import pandas as pd
-
-    def get_value_counts(df: pd.DataFrame) -> pd.Series:
-        # Define the list of columns to check
-        columns_to_check = [
-            col
-            for col in df.columns
-            if col.startswith(("agent", "solvent", "reagent", "catalyst"))
-        ]
-
-        # Initialize a list to store the results
-        results = []
-
-        # Loop through the columns
-        for col in columns_to_check:
-            # Get the value counts for the column
-            results += [df[col].value_counts()]
-
-        total_value_counts = (
-            pd.concat(results, axis=0, sort=True).groupby(level=0).sum()
-        )
-        if "other" in total_value_counts.index:
-            total_value_counts = total_value_counts.drop("other")
-        total_value_counts = total_value_counts.sort_values(ascending=True)
-        return total_value_counts
-
-    cleaned_value_counts = get_value_counts(df=cleaned_df.copy())
-    uncleaned_value_counts = get_value_counts(df=uncleaned_df.copy())
-
-    assert min_frequency_of_occurrence > 0  # sanity check the copying worked
-    assert "" not in cleaned_value_counts.keys()  # check there are no empty strings
-    assert "" not in uncleaned_value_counts.keys()  # check there are no empty strings
-
-    cleaned_rare = cleaned_value_counts[
-        cleaned_value_counts < min_frequency_of_occurrence
-    ]
-    uncleaned_rare = uncleaned_value_counts[
-        uncleaned_value_counts < min_frequency_of_occurrence
-    ]
-
-    if not cleaned_rare.empty:
-        # if there is stuff that is rare now, we want to make sure it wasnt rare previously
-        assert uncleaned_rare.index.intersection(cleaned_value_counts.index).empty
-
-
-def test_move_rows_from_test_to_train_set() -> None:
-    """
-    Test that the function that moves rows from the test set to the train set works as expected.
-    """
-    import numpy as np
-    import pandas as pd
-
-    import orderly.clean.cleaner
-
-    reactant_columns = ["reactant_000", "reactant_001"]
-    product_columns = ["product_000"]
-
-    train_indices = np.array([0, 1, 2])
-    test_indices = np.array([3, 4, 5])
-
-    train_dict = {
-        "reactant_000": ["a", "b", "c"],
-        "reactant_001": ["b", "e", "f"],
-        "product_000": ["c", "h", "i"],
-    }
-    test_dict = {
-        "reactant_000": ["a", "b", "c"],
-        "reactant_001": ["b", "a", "a"],
-        "product_000": ["c", "c", "b"],
-    }
-    train_df = pd.DataFrame(train_dict)
-    test_df = pd.DataFrame(test_dict)
-    df = pd.concat([train_df, test_df], axis=0, sort=False)
-
-    df = df.reset_index(drop=True)
-
-    matching_indices = orderly.clean.cleaner.get_matching_indices(
-        df, train_indices, test_indices, reactant_columns, product_columns
-    )
-
-    assert np.equal(matching_indices, np.array([3, 4])).all()
+import pathlib
+from typing import Any, Dict, List, Optional, Tuple
+
+import pandas as pd
+import pytest
+
+
+def test_hello_world() -> None:
+    assert True
+
+
+@pytest.fixture
+def toy_dict() -> Dict[str, List[str]]:
+    toy_dict = {
+        "reactant_000": ["B", "A", "F", "A"],
+        "reactant_001": ["D", "A", pd.NA, "B"],
+        "product_000": ["C", "A", "E", "A"],
+        "product_001": ["E", "G", "C", "H"],
+        "agent_000": ["D", "F", "D", "B"],
+        "agent_001": ["C", "E", "G", "A"],
+        "solvent_000": ["E", "B", "G", "C"],
+        "solvent_001": ["C", "D", "B", "G"],
+        "solvent_002": ["D", "B", "F", "G"],
+    }
+
+    return toy_dict
+
+
+def get_cleaned_df(
+    output_path: pathlib.Path,
+    trust_labelling: bool,
+    consistent_yield: bool,
+    num_reactant: int,
+    num_product: int,
+    num_solv: int,
+    num_agent: int,
+    num_cat: int,
+    num_reag: int,
+    min_frequency_of_occurrence: int,
+    map_rare_molecules_to_other: bool,
+    set_unresolved_names_to_none_if_mapped_rxn_str_exists_else_del_rxn: bool,
+    set_unresolved_names_to_none: bool,
+    remove_rxn_with_unresolved_names: bool,
+    remove_reactions_with_no_reactants: bool,
+    remove_reactions_with_no_products: bool,
+    remove_reactions_with_no_solvents: bool,
+    remove_reactions_with_no_agents: bool,
+    remove_reactions_with_no_conditions: bool,
+    drop_duplicates: bool,
+) -> pd.DataFrame:
+    import orderly.clean.cleaner
+    import orderly.data.test_data
+
+    ord_extraction_path = (
+        orderly.data.test_data.get_path_of_test_extracted_ords(
+            trust_labelling=trust_labelling
+        )
+        / "extracted_ords"
+    )
+    molecules_to_remove_path = (
+        orderly.data.test_data.get_path_of_test_extracted_ords(
+            trust_labelling=trust_labelling
+        )
+        / "all_molecule_names.csv"
+    )
+
+    orderly.clean.cleaner.main(
+        output_path=output_path,
+        ord_extraction_path=ord_extraction_path,
+        molecules_to_remove_path=molecules_to_remove_path,
+        consistent_yield=consistent_yield,
+        num_reactant=num_reactant,
+        num_product=num_product,
+        num_solv=num_solv,
+        num_agent=num_agent,
+        num_cat=num_cat,
+        num_reag=num_reag,
+        min_frequency_of_occurrence=min_frequency_of_occurrence,
+        map_rare_molecules_to_other=map_rare_molecules_to_other,
+        set_unresolved_names_to_none_if_mapped_rxn_str_exists_else_del_rxn=set_unresolved_names_to_none_if_mapped_rxn_str_exists_else_del_rxn,
+        set_unresolved_names_to_none=set_unresolved_names_to_none,
+        remove_rxn_with_unresolved_names=remove_rxn_with_unresolved_names,
+        remove_reactions_with_no_reactants=remove_reactions_with_no_reactants,
+        remove_reactions_with_no_products=remove_reactions_with_no_products,
+        remove_reactions_with_no_solvents=remove_reactions_with_no_solvents,
+        remove_reactions_with_no_agents=remove_reactions_with_no_agents,
+        remove_reactions_with_no_conditions=remove_reactions_with_no_conditions,
+        scramble=False,
+        train_test_split_fraction=0,
+        drop_duplicates=drop_duplicates,
+        disable_tqdm=False,
+        overwrite=False,
+    )
+
+    import pandas as pd
+
+    return pd.read_parquet(output_path)
+
+
+@pytest.fixture
+def cleaned_df_params_default(
+    tmp_path: pathlib.Path, request: pytest.FixtureRequest
+) -> Tuple[pd.DataFrame, List[Any]]:
+    assert len(request.param) == 10
+    updated_args = request.param + [
+        True,
+        False,
+        False,
+        True,
+        True,
+        True,
+        True,
+        False,
+        True,
+    ]
+    # set_unresolved_names_to_none_if_mapped_rxn_str_exists_else_del_rxn: bool,
+    # set_unresolved_names_to_none: bool,
+    # remove_rxn_with_unresolved_names: bool,
+    # remove_reactions_with_no_reactants: bool,
+    # remove_reactions_with_no_products: bool,
+    # remove_reactions_with_no_solvents: bool,
+    # remove_reactions_with_no_agents: bool,
+    # remove_reactions_with_no_conditions: bool,
+    # drop_duplicates: bool
+    return (
+        get_cleaned_df(
+            tmp_path / "cleaned_df" / "orderly_ord.parquet",
+            *updated_args,
+        ),
+        request.param,
+    )
+
+
+@pytest.fixture
+def cleaned_df_params_default_without_min_freq(
+    tmp_path: pathlib.Path, request: pytest.FixtureRequest
+) -> Tuple[pd.DataFrame, List[Any]]:
+    import copy
+
+    args = copy.copy(request.param)
+    args[-2] = 0
+    assert len(request.param) == 10
+    updated_args = args + [
+        True,
+        False,
+        False,
+        True,
+        True,
+        True,
+        True,
+        False,
+        True,
+    ]
+    # set_unresolved_names_to_none_if_mapped_rxn_str_exists_else_del_rxn: bool,
+    # set_unresolved_names_to_none: bool,
+    # remove_rxn_with_unresolved_names: bool,
+    # remove_reactions_with_no_reactants: bool,
+    # remove_reactions_with_no_products: bool,
+    # remove_reactions_with_no_solvents: bool,
+    # remove_reactions_with_no_agents: bool,
+    # remove_reactions_with_no_conditions: bool,
+    # drop_duplicates: bool
+    return (
+        get_cleaned_df(
+            tmp_path
+            / "cleaned_df_params_default_without_min_freq"
+            / "orderly_ord.parquet",
+            *updated_args,
+        ),
+        args,
+    )
+
+
+@pytest.fixture
+def cleaned_df_params_retaining_unresolved_names_and_duplicates(
+    tmp_path: pathlib.Path, request: pytest.FixtureRequest
+) -> Tuple[pd.DataFrame, List[Any]]:
+    assert len(request.param) == 10
+    updated_args = request.param + [
+        False,
+        False,
+        False,
+        True,
+        True,
+        True,
+        True,
+        False,
+        False,
+    ]
+    # set_unresolved_names_to_none_if_mapped_rxn_str_exists_else_del_rxn: bool,
+    # set_unresolved_names_to_none: bool,
+    # remove_rxn_with_unresolved_names: bool,
+    # remove_reactions_with_no_reactants: bool,
+    # remove_reactions_with_no_products: bool,
+    # remove_reactions_with_no_solvents: bool,
+    # remove_reactions_with_no_agents: bool,
+    # remove_reactions_with_no_conditions: bool,
+    # drop_duplicates: bool
+
+    return (
+        get_cleaned_df(
+            tmp_path
+            / "cleaned_df_params_retaining_unresolved_names_and_duplicates"
+            / "orderly_ord.parquet",
+            *updated_args,
+        ),
+        request.param,
+    )
+
+
+@pytest.fixture
+def cleaned_df_params_retaining_unresolved_names_and_duplicates_without_min_freq(
+    tmp_path: pathlib.Path, request: pytest.FixtureRequest
+) -> Tuple[pd.DataFrame, List[Any]]:
+    import copy
+
+    args = copy.copy(request.param)
+    args[-2] = 0
+    assert len(request.param) == 10
+    updated_args = args + [
+        False,
+        False,
+        False,
+        True,
+        True,
+        True,
+        True,
+        False,
+        False,
+    ]
+    # set_unresolved_names_to_none_if_mapped_rxn_str_exists_else_del_rxn: bool,
+    # set_unresolved_names_to_none: bool,
+    # remove_rxn_with_unresolved_names: bool,
+    # remove_reactions_with_no_reactants: bool,
+    # remove_reactions_with_no_products: bool,
+    # remove_reactions_with_no_solvents: bool,
+    # remove_reactions_with_no_agents: bool,
+    # remove_reactions_with_no_conditions: bool,
+    # drop_duplicates: bool
+    return (
+        get_cleaned_df(
+            tmp_path
+            / "cleaned_df_params_retaining_unresolved_names_and_duplicates_without_min_freq"
+            / "orderly_ord.parquet",
+            *updated_args,
+        ),
+        args,
+    )
+
+
+def test_molecule_names_not_empty() -> None:
+    import os
+    import pathlib
+
+    import pandas as pd
+
+    import orderly.data.util
+    from orderly.data.test_data import get_path_of_molecule_names
+
+    all_empty = True
+
+    molecule_names_folder_path = get_path_of_molecule_names()
+
+    files = os.listdir(molecule_names_folder_path)
+    for file in files:
+        if file.endswith(".csv"):  # or file.endswith(".parquet")
+            file_path = pathlib.Path(os.path.join(molecule_names_folder_path, file))
+            molecule_names_list = orderly.data.util.load_list(path=file_path)
+            if len(molecule_names_list) > 0:
+                all_empty = False
+    assert not all_empty
+
+
+@pytest.mark.parametrize(
+    "columns_to_count_from, expected_total_value_counts",
+    (
+        pytest.param(
+            [
+                "reactant_000",
+                "reactant_001",
+                "product_000",
+                "product_001",
+                "agent_000",
+                "agent_001",
+                "solvent_000",
+                "solvent_001",
+                "solvent_002",
+            ],
+            {"A": 6, "B": 6, "C": 5, "D": 5, "E": 4, "F": 3, "G": 5, "H": 1},
+            id="all_columns",
+        ),
+        pytest.param(
+            ["agent_000", "agent_001", "solvent_000", "solvent_001", "solvent_002"],
+            {"A": 1, "B": 4, "C": 3, "D": 4, "E": 2, "F": 2, "G": 4},
+            id="agent_and_solvent_columns",
+        ),
+    ),
+)
+def test_get_value_counts(
+    toy_dict: Dict[str, List[str]],
+    columns_to_count_from: List[str],
+    expected_total_value_counts: Dict[str, int],
+) -> None:
+    import copy
+
+    import pandas as pd
+
+    import orderly.clean.cleaner
+
+    toy_dict = copy.copy(toy_dict)
+
+    df = pd.DataFrame(toy_dict)
+
+    total_value_counts = orderly.clean.cleaner.Cleaner._get_value_counts(
+        df, columns_to_count_from
+    )
+
+    expected_total_value_counts = pd.Series(expected_total_value_counts).sort_values(
+        ascending=False
+    )
+
+    assert total_value_counts.equals(
+        pd.Series(expected_total_value_counts)
+    ), f"Got: {total_value_counts}, expected: {expected_total_value_counts},"
+
+
+def test_scramble(
+    toy_dict: Dict[str, List[str]],
+) -> None:
+    import copy
+
+    import pandas as pd
+
+    import orderly.clean.cleaner
+
+    toy_dict = copy.copy(toy_dict)
+
+    df = pd.DataFrame(toy_dict)
+    components = ("reactant", "agent", "solvent", "catalyst", "reagent")
+
+    scrambled_df = orderly.clean.cleaner.Cleaner._scramble(df, components)
+
+    assert not scrambled_df.equals(
+        df
+    ), f"Got: {scrambled_df}, expected to be different from: {df},"
+
+    # check that molecules have only been moved around within the same reaction (i.e. the same row)
+    rows_to_check = min(10, len(df))
+    for i in range(rows_to_check):
+        sorted_row_components = set(df.iloc[i])
+        scrambled_row_components = set(scrambled_df.iloc[i])
+        assert (
+            sorted_row_components == scrambled_row_components
+        ), f"Got: {sorted_row_components}, expected: {scrambled_row_components},"
+
+
+@pytest.mark.parametrize(
+    "component_name, number_of_columns_to_keep, expected_dict",
+    (
+        # Del reactions with too many reactants
+        pytest.param(
+            "reactant",
+            1,
+            {
+                "reactant_000": ["F"],
+                "product_000": ["E"],
+                "product_001": ["C"],
+                "agent_000": ["D"],
+                "agent_001": ["G"],
+                "solvent_000": ["G"],
+                "solvent_001": ["B"],
+                "solvent_002": ["F"],
+            },
+        ),
+        # Add a component
+        pytest.param(
+            "reactant",
+            3,
+            {
+                "reactant_000": ["B", "A", "F", "A"],
+                "reactant_001": ["D", "A", pd.NA, "B"],
+                "reactant_002": [pd.NA, pd.NA, pd.NA, pd.NA],
+                "product_000": ["C", "A", "E", "A"],
+                "product_001": ["E", "G", "C", "H"],
+                "agent_000": ["D", "F", "D", "B"],
+                "agent_001": ["C", "E", "G", "A"],
+                "solvent_000": ["E", "B", "G", "C"],
+                "solvent_001": ["C", "D", "B", "G"],
+                "solvent_002": ["D", "B", "F", "G"],
+            },
+        ),
+        # Add two component
+        pytest.param(
+            "reactant",
+            4,
+            {
+                "reactant_000": ["B", "A", "F", "A"],
+                "reactant_001": ["D", "A", pd.NA, "B"],
+                "reactant_002": [pd.NA, pd.NA, pd.NA, pd.NA],
+                "reactant_003": [pd.NA, pd.NA, pd.NA, pd.NA],
+                "product_000": ["C", "A", "E", "A"],
+                "product_001": ["E", "G", "C", "H"],
+                "agent_000": ["D", "F", "D", "B"],
+                "agent_001": ["C", "E", "G", "A"],
+                "solvent_000": ["E", "B", "G", "C"],
+                "solvent_001": ["C", "D", "B", "G"],
+                "solvent_002": ["D", "B", "F", "G"],
+            },
+        ),
+        # Do nothing
+        pytest.param(
+            "reactant",
+            2,
+            {
+                "reactant_000": ["B", "A", "F", "A"],
+                "reactant_001": ["D", "A", pd.NA, "B"],
+                "product_000": ["C", "A", "E", "A"],
+                "product_001": ["E", "G", "C", "H"],
+                "agent_000": ["D", "F", "D", "B"],
+                "agent_001": ["C", "E", "G", "A"],
+                "solvent_000": ["E", "B", "G", "C"],
+                "solvent_001": ["C", "D", "B", "G"],
+                "solvent_002": ["D", "B", "F", "G"],
+            },
+        ),
+        # Do nothing
+        pytest.param(
+            "reactant",
+            -1,
+            {
+                "reactant_000": ["B", "A", "F", "A"],
+                "reactant_001": ["D", "A", pd.NA, "B"],
+                "product_000": ["C", "A", "E", "A"],
+                "product_001": ["E", "G", "C", "H"],
+                "agent_000": ["D", "F", "D", "B"],
+                "agent_001": ["C", "E", "G", "A"],
+                "solvent_000": ["E", "B", "G", "C"],
+                "solvent_001": ["C", "D", "B", "G"],
+                "solvent_002": ["D", "B", "F", "G"],
+            },
+        ),
+    ),
+)
+def test_remove_reactions_with_too_many_of_component(
+    toy_dict: Dict[str, List[str]],
+    component_name: str,
+    number_of_columns_to_keep: int,
+    expected_dict: Dict[str, int],
+) -> None:
+    import copy
+
+    import pandas as pd
+
+    import orderly.clean.cleaner
+
+    toy_dict = copy.copy(toy_dict)
+
+    df = pd.DataFrame(toy_dict)
+
+    filtered_df = (
+        orderly.clean.cleaner.Cleaner._remove_reactions_with_too_many_of_component(
+            df=df,
+            component_name=component_name,
+            number_of_columns_to_keep=number_of_columns_to_keep,
+        )
+    )
+
+    expected_filtered_df = pd.DataFrame(expected_dict).sort_index(axis=1)
+    if filtered_df.empty:
+        assert filtered_df.empty == expected_filtered_df.empty
+    else:
+        assert filtered_df.equals(
+            expected_filtered_df
+        ), f"Got: {filtered_df}, expected: {expected_filtered_df},"
+
+
+@pytest.mark.parametrize(
+    "columns_to_transform, value_counts_dict, min_frequency_of_occurrence, expected_dict,",
+    (
+        pytest.param(
+            [
+                "reactant_000",
+                "reactant_001",
+                "product_000",
+                "product_001",
+                "agent_000",
+                "agent_001",
+                "solvent_000",
+                "solvent_001",
+                "solvent_002",
+            ],
+            {"A": 6, "B": 6, "C": 5, "D": 5, "E": 4, "F": 3, "G": 5, "H": 1},
+            4,
+            {
+                "reactant_000": ["B", "A", "other", "A"],
+                "reactant_001": ["D", "A", pd.NA, "B"],
+                "product_000": ["C", "A", "E", "A"],
+                "product_001": ["E", "G", "C", "other"],
+                "agent_000": ["D", "other", "D", "B"],
+                "agent_001": ["C", "E", "G", "A"],
+                "solvent_000": ["E", "B", "G", "C"],
+                "solvent_001": ["C", "D", "B", "G"],
+                "solvent_002": ["D", "B", "other", "G"],
+            },
+            id="all_columns",
+        ),
+        pytest.param(
+            ["agent_000", "agent_001", "solvent_000", "solvent_001", "solvent_002"],
+            {"A": 1, "B": 4, "C": 3, "D": 4, "E": 2, "F": 2, "G": 3},
+            3,
+            {
+                "reactant_000": ["B", "A", "F", "A"],
+                "reactant_001": ["D", "A", pd.NA, "B"],
+                "product_000": ["C", "A", "E", "A"],
+                "product_001": ["E", "G", "C", "H"],
+                "agent_000": ["D", "other", "D", "B"],
+                "agent_001": ["C", "other", "G", "other"],
+                "solvent_000": ["other", "B", "G", "C"],
+                "solvent_001": ["C", "D", "B", "G"],
+                "solvent_002": ["D", "B", "other", "G"],
+            },
+            id="agent_and_solvent_columns",
+        ),
+    ),
+)
+def test_map_rare_molecules_to_other(
+    toy_dict: Dict[str, List[str]],
+    columns_to_transform: List[str],
+    value_counts_dict: Dict[str, int],
+    min_frequency_of_occurrence: int,
+    expected_dict: Dict[str, List[str]],
+) -> None:
+    import copy
+
+    import pandas as pd
+
+    import orderly.clean.cleaner
+
+    toy_dict = copy.copy(toy_dict)
+
+    df = pd.DataFrame(toy_dict)
+    value_counts_series = pd.Series(value_counts_dict)
+
+    df = orderly.clean.cleaner.Cleaner._map_rare_molecules_to_other(
+        df, columns_to_transform, value_counts_series, min_frequency_of_occurrence
+    )
+
+    expected_df = pd.DataFrame(expected_dict)
+
+    assert df.equals(expected_df), f"Got: {df}, expected: {expected_df},"
+
+
+@pytest.mark.parametrize(
+    "toy_dict, target_strings, expected_dict,",
+    (
+        pytest.param(
+            {
+                "reactant_000": [
+                    "a",
+                    None,
+                    None,
+                    "a",
+                ],
+                "reactant_001": [
+                    None,
+                    "a",
+                    None,
+                    "b",
+                ],
+                "reactant_002": [
+                    "b",
+                    "b",
+                    "a",
+                    "c",
+                ],
+                "agent_000": [
+                    "a",
+                    "a",
+                    None,
+                    None,
+                ],
+                "agent_001": [
+                    None,
+                    "b",
+                    "a",
+                    None,
+                ],
+                "agent_002": [
+                    "b",
+                    "c",
+                    "b",
+                    None,
+                ],
+            },
+            ("reactant", "product", "agent", "solvent"),
+            {
+                "reactant_000": [
+                    "a",
+                    "a",
+                    "a",
+                    "a",
+                ],
+                "reactant_001": [
+                    "b",
+                    "b",
+                    None,
+                    "b",
+                ],
+                "reactant_002": [
+                    None,
+                    None,
+                    None,
+                    "c",
+                ],
+                "agent_000": [
+                    "a",
+                    "a",
+                    "a",
+                    None,
+                ],
+                "agent_001": [
+                    "b",
+                    "b",
+                    "b",
+                    None,
+                ],
+                "agent_002": [
+                    None,
+                    "c",
+                    None,
+                    None,
+                ],
+            },
+        ),
+        pytest.param(
+            {
+                "product_000": [
+                    "a",
+                    "a",
+                    None,
+                    None,
+                ],
+                "product_001": [
+                    None,
+                    "b",
+                    "a",
+                    None,
+                ],
+                "product_002": [
+                    "b",
+                    "c",
+                    "b",
+                    None,
+                ],
+                "yield_000": [
+                    "a",
+                    "a",
+                    "c",
+                    None,
+                ],
+                "yield_001": [
+                    None,
+                    "b",
+                    "a",
+                    None,
+                ],
+                "yield_002": [
+                    "b",
+                    "c",
+                    "b",
+                    None,
+                ],
+            },
+            ("product",),
+            {
+                "product_000": [
+                    "a",
+                    "a",
+                    "a",
+                    None,
+                ],
+                "product_001": [
+                    "b",
+                    "b",
+                    "b",
+                    None,
+                ],
+                "product_002": [
+                    None,
+                    "c",
+                    None,
+                    None,
+                ],
+                "yield_000": [
+                    "a",
+                    "a",
+                    "a",
+                    None,
+                ],
+                "yield_001": [
+                    "b",
+                    "b",
+                    "b",
+                    None,
+                ],
+                "yield_002": [
+                    None,
+                    "c",
+                    "c",
+                    None,
+                ],
+            },
+        ),
+    ),
+)
+def test_move_none_to_after_data(
+    toy_dict: Dict[str, List[str]],
+    target_strings: Tuple[str, ...],
+    expected_dict: Dict[str, List[str]],
+) -> None:
+    import copy
+
+    import pandas as pd
+
+    import orderly.clean.cleaner
+
+    toy_dict = copy.copy(toy_dict)
+
+    df = pd.DataFrame(toy_dict)
+
+    df = orderly.clean.cleaner.Cleaner._move_none_to_after_data(df, target_strings)
+
+    expected_df = pd.DataFrame(expected_dict)
+
+    assert df.equals(expected_df), f"Got: \n{df}, expected: \n{expected_df},"
+
+
+@pytest.mark.parametrize(
+    "columns_to_transform, value_counts_dict, min_frequency_of_occurrence, expected_dict,",
+    (
+        pytest.param(
+            [
+                "reactant_000",
+                "reactant_001",
+                "product_000",
+                "product_001",
+                "agent_000",
+                "agent_001",
+                "solvent_000",
+                "solvent_001",
+                "solvent_002",
+            ],
+            {"A": 6, "B": 6, "C": 5, "D": 5, "E": 4, "F": 3, "G": 6, "H": 1},
+            4,
+            {
+                "reactant_000": ["B"],
+                "reactant_001": ["D"],
+                "product_000": ["C"],
+                "product_001": ["E"],
+                "agent_000": ["D"],
+                "agent_001": ["C"],
+                "solvent_000": ["E"],
+                "solvent_001": ["C"],
+                "solvent_002": ["D"],
+            },
+            id="all_columns",
+        ),
+        pytest.param(
+            ["agent_000", "agent_001", "solvent_000", "solvent_001", "solvent_002"],
+            {"A": 1, "B": 4, "C": 3, "D": 4, "E": 2, "F": 2, "G": 4},
+            2,
+            {
+                "reactant_000": ["B", "A", "F"],
+                "reactant_001": ["D", "A", pd.NA],
+                "product_000": ["C", "A", "E"],
+                "product_001": ["E", "G", "C"],
+                "agent_000": ["D", "F", "D"],
+                "agent_001": ["C", "E", "G"],
+                "solvent_000": ["E", "B", "G"],
+                "solvent_001": ["C", "D", "B"],
+                "solvent_002": ["D", "B", "F"],
+            },
+            id="agent_and_solvent_columns",
+        ),
+    ),
+)
+def test_remove_rare_molecules(
+    toy_dict: Dict[str, List[str]],
+    columns_to_transform: List[str],
+    value_counts_dict: Dict[str, int],
+    min_frequency_of_occurrence: int,
+    expected_dict: Dict[str, List[str]],
+) -> None:
+    import copy
+
+    import pandas as pd
+
+    import orderly.clean.cleaner
+
+    toy_dict = copy.copy(toy_dict)
+
+    df = pd.DataFrame(toy_dict)
+    value_counts_series = pd.Series(value_counts_dict)
+
+    df = orderly.clean.cleaner.Cleaner._remove_rare_molecules(
+        df, columns_to_transform, value_counts_series, min_frequency_of_occurrence
+    )
+
+    expected_df = pd.DataFrame(expected_dict)
+
+    assert df.equals(expected_df), f"Got: {df}, expected: {expected_df},"
+
+
+@pytest.mark.parametrize(
+    "cleaned_df_params_default",
+    (
+        pytest.param(
+            [False, False, 5, 5, 2, 3, 0, 0, 55, False],
+            id="trust_labelling:F|consistent_yield:F|map_rare_molecules_to_other:F",
+        ),
+        pytest.param(
+            [True, False, 5, 5, 2, 0, 2, 1, 15, False],
+            id="trust_labelling:T|consistent_yield:F|map_rare_molecules_to_other:F",
+        ),
+        pytest.param(
+            [False, True, 5, 5, 2, 3, 0, 0, 15, False],
+            id="trust_labelling:F|consistent_yield:T|map_rare_molecules_to_other:F",
+        ),
+        pytest.param(
+            [False, False, 5, 5, 2, 3, 0, 0, 15, True],
+            id="trust_labelling:F|consistent_yield:F|map_rare_molecules_to_other:T",
+        ),
+        pytest.param(
+            [True, True, 5, 5, 2, 0, 2, 1, 15, False],
+            id="trust_labelling:T|consistent_yield:T|map_rare_molecules_to_other:F",
+        ),
+        pytest.param(
+            [True, False, 5, 5, 2, 0, 2, 1, 15, True],
+            id="trust_labelling:T|consistent_yield:F|map_rare_molecules_to_other:T",
+        ),
+        pytest.param(
+            [False, True, 5, 5, 2, 3, 0, 0, 15, True],
+            id="trust_labelling:F|consistent_yield:T|map_rare_molecules_to_other:T",
+        ),
+        pytest.param(
+            [True, True, 5, 5, 2, 0, 2, 1, 15, True],
+            id="trust_labelling:T|consistent_yield:T|map_rare_molecules_to_other:T",
+        ),
+    ),
+    indirect=True,
+)
+def test_get_cleaned_df(
+    cleaned_df_params_default: Tuple[pd.DataFrame, List[Any]]
+) -> None:
+    import copy
+
+    cleaned_df, _ = copy.copy(cleaned_df_params_default)
+    assert not cleaned_df.empty
+    # TODO: check that there's only NaN or NaT, but no None
+
+
+@pytest.mark.parametrize(
+    "cleaned_df_params_default",
+    (
+        pytest.param(
+            [False, False, 5, 5, 2, 3, 0, 0, 15, False],
+            id="trust_labelling:F|consistent_yield:F|map_rare_molecules_to_other:F",
+        ),
+        pytest.param(
+            [True, False, 5, 5, 2, 0, 2, 1, 15, False],
+            id="trust_labelling:T|consistent_yield:F|map_rare_molecules_to_other:F",
+        ),
+        pytest.param(
+            [False, True, 5, 5, 2, 3, 0, 0, 15, False],
+            id="trust_labelling:F|consistent_yield:T|map_rare_molecules_to_other:F",
+        ),
+        pytest.param(
+            [False, False, 5, 5, 2, 3, 0, 0, 15, True],
+            id="trust_labelling:F|consistent_yield:F|map_rare_molecules_to_other:T",
+        ),
+        pytest.param(
+            [True, True, 5, 5, 2, 0, 2, 1, 15, False],
+            id="trust_labelling:T|consistent_yield:T|map_rare_molecules_to_other:F",
+        ),
+        pytest.param(
+            [True, False, 5, 5, 2, 0, 2, 1, 15, True],
+            id="trust_labelling:T|consistent_yield:F|map_rare_molecules_to_other:T",
+        ),
+        pytest.param(
+            [False, True, 5, 5, 2, 3, 0, 0, 15, True],
+            id="trust_labelling:F|consistent_yield:T|map_rare_molecules_to_other:T",
+        ),
+        pytest.param(
+            [True, True, 5, 5, 2, 0, 2, 1, 15, True],
+            id="trust_labelling:T|consistent_yield:T|map_rare_molecules_to_other:T",
+        ),
+        # XFAILS
+        pytest.param(
+            [False, True, 5, 5, 5, 5, 5, 5, 5, True],
+            marks=pytest.mark.xfail(
+                reason="AssertionError: Invalid input: If trust_labelling=True in orderly.extract, then num_cat and num_reag must be 0. If trust_labelling=False, then num_agent must be 0."
+            ),
+            id="trust_labelling:F|consistent_yield:T|map_rare_molecules_to_other:F|fives",
+        ),
+    ),
+    indirect=True,
+)
+def test_number_of_columns_and_order_of_None(
+    cleaned_df_params_default: Tuple[pd.DataFrame, List[Any]]
+) -> None:
+    import copy
+
+    import numpy as np
+
+    cleaned_df, params = copy.copy(cleaned_df_params_default)
+
+    (
+        _,
+        _,
+        num_reactant,
+        num_product,
+        num_solv,
+        num_agent,
+        num_cat,
+        num_reag,
+        _,
+        _,
+    ) = params
+
+    # check that the number of columns is correct
+    num_reactant_cols = 0
+    num_product_cols = 0
+    num_agent_cols = 0
+    num_cat_cols = 0
+    num_reag_cols = 0
+    num_solv_cols = 0
+
+    cols = cleaned_df.columns
+    for col in cols:
+        if col.startswith("react"):
+            num_reactant_cols += 1
+        elif col.startswith("prod"):
+            num_product_cols += 1
+        elif col.startswith("agent"):
+            num_agent_cols += 1
+        elif col.startswith("cat"):
+            num_cat_cols += 1
+        elif col.startswith("reag"):
+            num_reag_cols += 1
+        elif col.startswith("solv"):
+            num_solv_cols += 1
+
+    # if num_reactant == -1 we just include all reactant columns (and same for the others)
+    assert (num_reactant_cols == num_reactant) or num_reactant == -1
+    assert (num_product_cols == num_product) or num_product == -1
+    assert (num_agent_cols == num_agent) or num_agent == -1
+    assert (num_cat_cols == num_cat) or num_cat == -1
+    assert (num_reag_cols == num_reag) or num_reag == -1
+    assert (num_solv_cols == num_solv) or num_solv == -1
+
+    assert "grant_date" in cols
+    assert "date_of_experiment" in cols
+
+    import numpy as np
+
+    grant_date = cleaned_df["grant_date"].replace({None: np.nan})
+    date_of_experiment = cleaned_df["date_of_experiment"].replace({None: np.nan})
+    if not grant_date.dropna().empty:
+        assert pd.api.types.is_datetime64_ns_dtype(
+            grant_date
+        ), f"failure for grant_date: {cleaned_df['grant_date'].dtype}"
+    if not date_of_experiment.dropna().empty:
+        assert pd.api.types.is_datetime64_ns_dtype(
+            date_of_experiment
+        ), f"failure for date_of_experiment: {cleaned_df['date_of_experiment'].dtype}"
+
+    # Check that grant_date and date_of_experiment columns are either dtype = datetime64 or full of None
+    datetime_coumns = cleaned_df.select_dtypes(include=[np.datetime64])
+    assert ("grant_date" in datetime_coumns.columns) or (
+        len(cleaned_df["grant_date"].dropna()) == 0
+    )
+    assert ("date_of_experiment" in datetime_coumns.columns) or (
+        len(cleaned_df["date_of_experiment"].dropna()) == 0
+    )
+
+    # Also check that there are no instances of None before data in the cleaned df
+
+    def _get_columns_beginning_with_str(
+        columns: List[str], target_strings: Optional[Tuple[str, ...]] = None
+    ) -> List[str]:
+        """goes through the column in a dataframe and adds columns that start with a string in the target strings"""
+        if target_strings is None:
+            target_strings = (
+                "agent",
+                "solvent",
+                "reagent",
+                "catalyst",
+                "product",
+                "reactant",
+            )
+
+        return sorted([col for col in columns if col.startswith(target_strings)])
+
+    target_strings = (
+        "agent",
+        "solvent",
+        "reagent",
+        "catalyst",
+        "product",
+        "reactant",
+    )
+
+    def check_valid_order(row: pd.Series) -> pd.Series:
+        seen_none = False
+        for idx, a in enumerate(row):
+            current_isna = pd.isna(a) or (a == "")
+            if seen_none:
+                if not current_isna:
+                    raise ValueError(f"Unexpected order at {idx=} for {row.tolist()=}")
+            if current_isna:
+                seen_none = True
+        return row
+
+    for target_string in target_strings:
+        target_columns = _get_columns_beginning_with_str(
+            columns=cleaned_df.columns,
+            target_strings=(target_string,),
+        )
+        # check that there are no instances of None before data in the cleaned df
+        for idx, row in cleaned_df.loc[:, target_columns].iterrows():
+            check_valid_order(row)
+        # cleaned_df.loc[:, target_columns].apply(check_valid_order, axis=1)
+
+
+def double_list(
+    x: List[Any],
+) -> Tuple[List[Any], List[Any]]:
+    return (x, x)
+
+
+@pytest.mark.parametrize(
+    "cleaned_df_params_default,cleaned_df_params_default_without_min_freq",
+    (
+        pytest.param(
+            *double_list([False, False, 5, 5, 2, 3, 0, 0, 15, False]),
+            id="trust_labelling:F|consistent_yield:F|map_rare_molecules_to_other:F|15",
+        ),
+        pytest.param(
+            *double_list([False, False, 5, 5, 2, 3, 0, 0, 100, False]),
+            id="trust_labelling:F|consistent_yield:F|map_rare_molecules_to_other:F|100",
+        ),
+        pytest.param(
+            *double_list([True, False, 5, 5, 2, 0, 2, 1, 15, False]),
+            id="trust_labelling:T|consistent_yield:F|map_rare_molecules_to_other:F",
+        ),
+        pytest.param(
+            *double_list([False, True, 5, 5, 2, 3, 0, 0, 15, False]),
+            id="trust_labelling:F|consistent_yield:T|map_rare_molecules_to_other:F",
+        ),
+        pytest.param(
+            *double_list([False, False, 5, 5, 2, 3, 0, 0, 15, True]),
+            id="trust_labelling:F|consistent_yield:F|map_rare_molecules_to_other:T",
+        ),
+        pytest.param(
+            *double_list([True, True, 5, 5, 2, 0, 2, 1, 15, False]),
+            id="trust_labelling:T|consistent_yield:T|map_rare_molecules_to_other:F",
+        ),
+        pytest.param(
+            *double_list([True, False, 5, 5, 2, 0, 2, 1, 15, True]),
+            id="trust_labelling:T|consistent_yield:F|map_rare_molecules_to_other:T",
+        ),
+        pytest.param(
+            *double_list([False, True, 5, 5, 2, 3, 0, 0, 15, True]),
+            id="trust_labelling:F|consistent_yield:T|map_rare_molecules_to_other:T",
+        ),
+        pytest.param(
+            *double_list([True, True, 5, 5, 2, 0, 2, 1, 15, True]),
+            id="trust_labelling:T|consistent_yield:T|map_rare_molecules_to_other:T",
+        ),
+        # XFAILS
+        pytest.param(
+            *double_list([False, True, 5, 5, 5, 5, 5, 5, 5, True]),
+            marks=pytest.mark.xfail(
+                reason="AssertionError: Invalid input: If trust_labelling=True in orderly.extract, then num_cat and num_reag must be 0. If trust_labelling=False, then num_agent must be 0."
+            ),
+            id="trust_labelling:F|consistent_yield:T|map_rare_molecules_to_other:F|fives",
+        ),
+    ),
+    indirect=True,
+)
+def test_frequency_params_default(
+    cleaned_df_params_default: Tuple[pd.DataFrame, List[Any]],
+    cleaned_df_params_default_without_min_freq: Tuple[pd.DataFrame, List[Any]],
+) -> None:
+    """
+    Test that there are no rare molecules left in the dataset after the cleaning process. There may be molecules appearing less often than the minimum frequency of occurrence, even after the cleaning, but this is because when deleting rows with rare values we may cause new molecules to become rare; this is why we check for the intersection of the two dfs at the very end of the test.
+    """
+
+    import copy
+
+    cleaned_df, params = copy.copy(cleaned_df_params_default)
+    uncleaned_df, unclean_params = copy.copy(cleaned_df_params_default_without_min_freq)
+
+    assert len(params) == len(unclean_params)
+    assert unclean_params[-2] == 0
+    assert len(params) == 10
+    min_frequency_of_occurrence = params[-2]
+
+    import pandas as pd
+
+    def get_value_counts(df: pd.DataFrame) -> pd.Series:
+        # Define the list of columns to check
+        columns_to_check = [
+            col
+            for col in df.columns
+            if col.startswith(("agent", "solvent", "reagent", "catalyst"))
+        ]
+
+        # Initialize a list to store the results
+        results = []
+
+        # Loop through the columns
+        for col in columns_to_check:
+            # Get the value counts for the column
+            results += [df[col].value_counts()]
+
+        total_value_counts = (
+            pd.concat(results, axis=0, sort=True).groupby(level=0).sum()
+        )
+        if "other" in total_value_counts.index:
+            total_value_counts = total_value_counts.drop("other")
+        total_value_counts = total_value_counts.sort_values(ascending=True)
+        return total_value_counts
+
+    cleaned_value_counts = get_value_counts(df=cleaned_df.copy())
+    uncleaned_value_counts = get_value_counts(df=uncleaned_df.copy())
+
+    assert min_frequency_of_occurrence > 0  # sanity check the copying worked
+    assert "" not in cleaned_value_counts.keys()  # check there are no empty strings
+    assert "" not in uncleaned_value_counts.keys()  # check there are no empty strings
+
+    cleaned_rare = cleaned_value_counts[
+        cleaned_value_counts < min_frequency_of_occurrence
+    ]
+    uncleaned_rare = uncleaned_value_counts[
+        uncleaned_value_counts < min_frequency_of_occurrence
+    ]
+
+    if not cleaned_rare.empty:
+        assert uncleaned_rare.index.intersection(cleaned_value_counts.index).empty
+
+
+@pytest.mark.parametrize(
+    "cleaned_df_params_retaining_unresolved_names_and_duplicates,cleaned_df_params_retaining_unresolved_names_and_duplicates_without_min_freq",
+    (
+        pytest.param(
+            *double_list([False, False, 5, 5, 2, 3, 0, 0, 15, False]),
+            id="trust_labelling:F|consistent_yield:F|map_rare_molecules_to_other:F|15",
+        ),
+        pytest.param(
+            *double_list([False, False, 5, 5, 2, 3, 0, 0, 100, False]),
+            id="trust_labelling:F|consistent_yield:F|map_rare_molecules_to_other:F|100",
+        ),
+        pytest.param(
+            *double_list([True, False, 5, 5, 2, 0, 2, 1, 15, False]),
+            id="trust_labelling:T|consistent_yield:F|map_rare_molecules_to_other:F",
+        ),
+        pytest.param(
+            *double_list([False, True, 5, 5, 2, 3, 0, 0, 15, False]),
+            id="trust_labelling:F|consistent_yield:T|map_rare_molecules_to_other:F",
+        ),
+        pytest.param(
+            *double_list([True, True, 5, 5, 2, 0, 2, 1, 15, False]),
+            id="trust_labelling:T|consistent_yield:T|map_rare_molecules_to_other:F",
+        ),
+        pytest.param(
+            *double_list([False, False, 5, 5, 2, 3, 0, 0, 15, True]),
+            id="trust_labelling:F|consistent_yield:F|map_rare_molecules_to_other:T",
+        ),
+        pytest.param(
+            *double_list([True, False, 5, 5, 2, 0, 2, 1, 15, True]),
+            id="trust_labelling:T|consistent_yield:F|map_rare_molecules_to_other:T",
+        ),
+        pytest.param(
+            *double_list([False, True, 5, 5, 2, 3, 0, 0, 15, True]),
+            id="trust_labelling:F|consistent_yield:T|map_rare_molecules_to_other:T",
+        ),
+        pytest.param(
+            *double_list([True, True, 5, 5, 2, 0, 2, 1, 15, True]),
+            id="trust_labelling:T|consistent_yield:T|map_rare_molecules_to_other:T",
+        ),
+    ),
+    indirect=True,
+)
+def test_frequency_retaining_unresolved_names_and_duplicates(
+    cleaned_df_params_retaining_unresolved_names_and_duplicates: Tuple[
+        pd.DataFrame, List[Any]
+    ],
+    cleaned_df_params_retaining_unresolved_names_and_duplicates_without_min_freq: Tuple[
+        pd.DataFrame, List[Any]
+    ],
+) -> None:
+    """
+    Test that there are no rare molecules left in the dataset after the cleaning process. There may be molecules appearing less often than the minimum frequency of occurrence, even after the cleaning, but this is because when deleting rows with rare values we may cause new molecules to become rare; this is why we check for the intersection of the two dfs at the very end of the test.
+
+    In this test we retain duplicate reactions and unresolved names (e.g. english names for molecules that aren't in our manual mapping).
+    """
+    import copy
+
+    cleaned_df, params = copy.copy(
+        cleaned_df_params_retaining_unresolved_names_and_duplicates
+    )
+    uncleaned_df, unclean_params = copy.copy(
+        cleaned_df_params_retaining_unresolved_names_and_duplicates_without_min_freq
+    )
+
+    assert len(params) == len(unclean_params)
+    assert unclean_params[-2] == 0
+    assert len(params) == 10
+    min_frequency_of_occurrence = params[-2]
+
+    import pandas as pd
+
+    def get_value_counts(df: pd.DataFrame) -> pd.Series:
+        # Define the list of columns to check
+        columns_to_check = [
+            col
+            for col in df.columns
+            if col.startswith(("agent", "solvent", "reagent", "catalyst"))
+        ]
+
+        # Initialize a list to store the results
+        results = []
+
+        # Loop through the columns
+        for col in columns_to_check:
+            # Get the value counts for the column
+            results += [df[col].value_counts()]
+
+        total_value_counts = (
+            pd.concat(results, axis=0, sort=True).groupby(level=0).sum()
+        )
+        if "other" in total_value_counts.index:
+            total_value_counts = total_value_counts.drop("other")
+        total_value_counts = total_value_counts.sort_values(ascending=True)
+        return total_value_counts
+
+    cleaned_value_counts = get_value_counts(df=cleaned_df.copy())
+    uncleaned_value_counts = get_value_counts(df=uncleaned_df.copy())
+
+    assert min_frequency_of_occurrence > 0  # sanity check the copying worked
+    assert "" not in cleaned_value_counts.keys()  # check there are no empty strings
+    assert "" not in uncleaned_value_counts.keys()  # check there are no empty strings
+
+    cleaned_rare = cleaned_value_counts[
+        cleaned_value_counts < min_frequency_of_occurrence
+    ]
+    uncleaned_rare = uncleaned_value_counts[
+        uncleaned_value_counts < min_frequency_of_occurrence
+    ]
+
+    if not cleaned_rare.empty:
+        # if there is stuff that is rare now, we want to make sure it wasnt rare previously
+        assert uncleaned_rare.index.intersection(cleaned_value_counts.index).empty
+
+
+def test_move_rows_from_test_to_train_set() -> None:
+    """
+    Test that the function that moves rows from the test set to the train set works as expected.
+    """
+    import numpy as np
+    import pandas as pd
+
+    import orderly.clean.cleaner
+
+    reactant_columns = ["reactant_000", "reactant_001"]
+    product_columns = ["product_000"]
+
+    train_indices = np.array([0, 1, 2])
+    test_indices = np.array([3, 4, 5])
+
+    train_dict = {
+        "reactant_000": ["a", "b", "c"],
+        "reactant_001": ["b", "e", "f"],
+        "product_000": ["c", "h", "i"],
+    }
+    test_dict = {
+        "reactant_000": ["a", "b", "c"],
+        "reactant_001": ["b", "a", "a"],
+        "product_000": ["c", "c", "b"],
+    }
+    train_df = pd.DataFrame(train_dict)
+    test_df = pd.DataFrame(test_dict)
+    df = pd.concat([train_df, test_df], axis=0, sort=False)
+
+    df = df.reset_index(drop=True)
+
+    matching_indices = orderly.clean.cleaner.get_matching_indices(
+        df, train_indices, test_indices, reactant_columns, product_columns
+    )
+
+    assert np.equal(matching_indices, np.array([3, 4])).all()
```

### Comparing `orderly-0.0.2/tests/test_data.py` & `orderly-0.1.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `orderly-0.0.2/tests/test_extract.py` & `orderly-0.1.0/tests/test_extract.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,1445 +1,1445 @@
-from typing import List, Dict, Callable, Set, Optional
-import pytest
-import pathlib
-
-from ord_schema.proto import reaction_pb2 as ord_reaction_pb2
-
-from orderly.types import YIELD, MANUAL_REPLACEMENTS_DICT
-
-REPETITIONS = 1
-SLOW_REPETITIONS = 1
-
-
-def test_hello_world() -> None:
-    assert True
-
-
-def get_rxn_func() -> Callable[[str, int], ord_reaction_pb2.Reaction]:
-    from ord_schema.proto import reaction_pb2 as ord_reaction_pb2
-
-    def get_rxn(
-        file_name: str,
-        rxn_idx: int,
-    ) -> ord_reaction_pb2.Reaction:
-        import orderly.extract.extractor
-        import orderly.data.test_data
-        import orderly.extract.main
-
-        _file = orderly.extract.main.get_file_names(
-            directory=orderly.data.test_data.get_path_of_test_ords(),
-            file_ending=f"{file_name}.pb.gz",
-        )
-        assert len(_file) == 1
-        file = pathlib.Path(_file[0])
-
-        dataset = orderly.extract.extractor.OrdExtractor.load_data(file)
-        rxn = dataset.reactions[rxn_idx]
-        return rxn
-
-    return get_rxn
-
-
-@pytest.mark.parametrize(
-    "file_name,rxn_idx,expected_labelled_reactants,expected_labelled_reagents,expected_labelled_solvents,expected_labelled_catalysts,expected_labelled_products_from_input,expected_ice_present,expected_non_smiles_names_list_additions",
-    (
-        [
-            "ord_dataset-00005539a1e04c809a9a78647bea649c",
-            0,
-            ["CC(C)N1CCNCC1", "CCOC(=O)c1cnc2cc(OCC)c(Br)cc2c1Nc1ccc(F)cc1F"],
-            ["O=C([O-])[O-]", "[Cs+]", "[Cs+]"],
-            [],
-            [
-                "c1ccc(P(c2ccccc2)c2ccc3ccccc3c2-c2c(P(c3ccccc3)c3ccccc3)ccc3ccccc23)cc1",
-                "O=C(/C=C/c1ccccc1)/C=C/c1ccccc1",
-                "O=C(/C=C/c1ccccc1)/C=C/c1ccccc1",
-                "O=C(/C=C/c1ccccc1)/C=C/c1ccccc1",
-                "[Pd]",
-                "[Pd]",
-            ],
-            [],
-            False,
-            [],
-        ],
-        [
-            "ord_dataset-0b70410902ae4139bd5d334881938f69",
-            0,
-            [
-                "SCc1ccccc1",
-                "[H-]",
-                "[Na+]",
-                "O=[N+]([O-])c1ccc(Oc2ccc(C(F)(F)F)cc2Cl)cc1[N+](=O)[O-]",
-            ],
-            [],
-            ["C1CCOC1", "C1CCOC1"],
-            [],
-            [],
-            False,
-            [],
-        ],
-        [
-            "ord_dataset-0bb2e99daa66408fb8dbd6a0781d241c",
-            0,
-            [
-                "[Na+]",
-                "[Na+]",
-                "[Na+]",
-                "[Na+]",
-                "[Na+]",
-                "[Na+]",
-                "[Na+]",
-                "[Na+]",
-                "[Na+]",
-                "[Na+]",
-                "[Na+]",
-                "[Na+]",
-                "[O-]B([O-])[O-]",
-                "[O-]B([O-])[O-]",
-                "[O-]B([O-])[O-]",
-                "[O-]B([O-])[O-]",
-                "35(Na2O)",
-            ],
-            [],
-            ["O"],
-            [],
-            [],
-            False,
-            ["35(Na2O)"],
-        ],
-        [
-            "ord_dataset-0bf72e95d80743729fdbb8b57a4bc0c6",
-            0,
-            ["CC1(C)C2CCC(=O)C1C2", "C1CCNC1", "Cc1ccc(S(=O)(=O)O)cc1", "O"],
-            [],
-            ["c1ccccc1"],
-            [],
-            [],
-            False,
-            [],
-        ],
-        [
-            "ord_dataset-a0eff6fe4b4143f284f0fc5ac503acad",
-            38,
-            [
-                "BrBr",
-                "CC1CC(C)(C)CC(C#N)(NNC(C)(C)C)C1",
-                "4-t-butylhydrazo-4-cyano-2,6-dimethylheptane",
-            ],
-            [],
-            [],
-            [],
-            [],
-            False,
-            ["4-t-butylhydrazo-4-cyano-2,6-dimethylheptane"],
-        ],
-    ),
-)
-@pytest.mark.parametrize("execution_number", range(REPETITIONS))
-def test_rxn_input_extractor(
-    execution_number: int,
-    file_name: str,
-    rxn_idx: int,
-    expected_labelled_reactants: List[str],
-    expected_labelled_reagents: List[str],
-    expected_labelled_solvents: List[str],
-    expected_labelled_catalysts: List[str],
-    expected_labelled_products_from_input: List[str],
-    expected_ice_present: bool,
-    expected_non_smiles_names_list_additions: List[str],
-) -> None:
-    rxn = get_rxn_func()(file_name, rxn_idx)
-
-    expected_labelled_reactants = sorted(expected_labelled_reactants)
-    expected_labelled_reagents = sorted(expected_labelled_reagents)
-    expected_labelled_solvents = sorted(expected_labelled_solvents)
-    expected_labelled_catalysts = sorted(expected_labelled_catalysts)
-    expected_labelled_products_from_input = sorted(
-        expected_labelled_products_from_input
-    )
-
-    import orderly.extract.extractor
-
-    (
-        labelled_reactants,
-        labelled_reagents,
-        labelled_solvents,
-        labelled_catalysts,
-        labelled_products_from_input,  # Daniel: I'm not sure what to do with this, it doesn't make sense for people to have put a product as an input, so this list should be empty anyway
-        ice_present,
-        non_smiles_names_list_additions,
-    ) = orderly.extract.extractor.OrdExtractor.rxn_input_extractor(
-        rxn, consider_molecule_names=True
-    )  # TODO: Add tests for when consider_molecule_names=False
-
-    assert (
-        expected_labelled_reactants == labelled_reactants
-    ), f"failure for {sorted(expected_labelled_reactants)=}, got {labelled_reactants}"  # TODO unsure why we have random ordering on ubuntu
-    assert (
-        expected_labelled_reagents == labelled_reagents
-    ), f"failure for {expected_labelled_reagents=}, got {labelled_reagents}"
-    assert (
-        expected_labelled_solvents == labelled_solvents
-    ), f"failure for {expected_labelled_solvents=}, got {labelled_solvents}"
-    assert (
-        expected_labelled_catalysts == labelled_catalysts
-    ), f"failure for {expected_labelled_catalysts=}, got {labelled_catalysts}"
-    assert (
-        expected_labelled_products_from_input == labelled_products_from_input
-    ), f"failure for {expected_labelled_products_from_input=}, got {labelled_products_from_input}"
-    assert (
-        expected_ice_present == ice_present
-    ), f"failure for {expected_ice_present=}, got {ice_present}"
-    assert (
-        expected_non_smiles_names_list_additions == non_smiles_names_list_additions
-    ), f"failure for {expected_non_smiles_names_list_additions=}, got {non_smiles_names_list_additions}"
-
-
-@pytest.mark.parametrize(
-    "file_name,rxn_idx,expected_labelled_products,expected_yields,expected_non_smiles_names_list_additions",
-    (
-        [
-            "ord_dataset-00005539a1e04c809a9a78647bea649c",
-            0,
-            ["CCOC(=O)c1cnc2cc(OCC)c(N3CCN(C(C)C)CC3)cc2c1Nc1ccc(F)cc1F"],
-            [65.39],
-            [],
-        ],
-        [
-            "ord_dataset-0b70410902ae4139bd5d334881938f69",
-            0,
-            ["O=[N+]([O-])c1ccc(Oc2ccc(C(F)(F)F)cc2Cl)cc1SCc1ccccc1"],
-            [None],
-            [],
-        ],
-        [
-            "ord_dataset-0bb2e99daa66408fb8dbd6a0781d241c",
-            0,
-            ["[O-]B1OB2OB([O-])OB(O1)O2", "[Na+]", "[Na+]"],
-            [None, None, None],
-            [],
-        ],
-        [
-            "ord_dataset-0bf72e95d80743729fdbb8b57a4bc0c6",
-            0,
-            ["CC1(C)C2CC=C(N3CCCC3)C1C2"],
-            [95.0],
-            [],
-        ],
-    ),
-)
-@pytest.mark.parametrize("execution_number", range(REPETITIONS))
-def test_rxn_outcomes_extractor(
-    execution_number: int,
-    file_name: str,
-    rxn_idx: int,
-    expected_labelled_products: List[str],
-    expected_yields: List[Optional[float]],
-    expected_non_smiles_names_list_additions: List[str],
-) -> None:
-    rxn = get_rxn_func()(file_name, rxn_idx)
-
-    import orderly.extract.extractor
-
-    (
-        labelled_products,
-        yields,
-        non_smiles_names_list_additions,
-    ) = orderly.extract.extractor.OrdExtractor.rxn_outcomes_extractor(
-        rxn, consider_molecule_names=True
-    )  # TODO: Add tests for when consider_molecule_names=False
-
-    assert expected_yields == yields, f"failure for {expected_yields=} got {yields}"
-    assert (
-        expected_labelled_products == labelled_products
-    ), f"failure for {expected_labelled_products=} got {labelled_products}"
-    assert (
-        expected_non_smiles_names_list_additions == non_smiles_names_list_additions
-    ), f"failure for {expected_non_smiles_names_list_additions=} got {non_smiles_names_list_additions}"
-
-
-@pytest.mark.parametrize(
-    "file_name,rxn_idx,expected_rxn_str,expected_is_mapped",
-    (
-        ["ord_dataset-00005539a1e04c809a9a78647bea649c", 0, None, None],
-        [
-            "ord_dataset-0b70410902ae4139bd5d334881938f69",
-            0,
-            "[CH2:1]([SH:8])[C:2]1[CH:7]=[CH:6][CH:5]=[CH:4][CH:3]=1.[H-].[Na+].[Cl:11][C:12]1[CH:30]=[C:29]([C:31]([F:34])([F:33])[F:32])[CH:28]=[CH:27][C:13]=1[O:14][C:15]1[CH:20]=[CH:19][C:18]([N+:21]([O-:23])=[O:22])=[C:17]([N+]([O-])=O)[CH:16]=1>O1CCCC1>[CH2:1]([S:8][C:17]1[CH:16]=[C:15]([O:14][C:13]2[CH:27]=[CH:28][C:29]([C:31]([F:34])([F:32])[F:33])=[CH:30][C:12]=2[Cl:11])[CH:20]=[CH:19][C:18]=1[N+:21]([O-:23])=[O:22])[C:2]1[CH:7]=[CH:6][CH:5]=[CH:4][CH:3]=1",
-            True,
-        ],
-        [
-            "ord_dataset-0bb2e99daa66408fb8dbd6a0781d241c",
-            0,
-            "[B:1]([O-:4])([O-:3])[O-:2].[B:5]([O-:8])([O-:7])[O-:6].[B:9]([O-:12])([O-])[O-].[B:13]([O-])([O-])[O-].[Na+:17].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+]>O>[B:1]1([O-:4])[O:3][B:13]2[O:12][B:9]([O:6][B:5]([O-:8])[O:7]2)[O:2]1.[Na+:17].[Na+:17]",
-            True,
-        ],
-        [
-            "ord_dataset-0bf72e95d80743729fdbb8b57a4bc0c6",
-            0,
-            "[CH3:1][C:2]1([CH3:10])[CH:8]2[CH2:9][CH:3]1[CH2:4][CH2:5][C:6]2=O.[NH:11]1[CH2:15][CH2:14][CH2:13][CH2:12]1.C1(C)C=CC(S(O)(=O)=O)=CC=1.O>C1C=CC=CC=1>[CH3:1][C:2]1([CH3:10])[CH:8]2[CH2:9][CH:3]1[CH2:4][CH:5]=[C:6]2[N:11]1[CH2:15][CH2:14][CH2:13][CH2:12]1",
-            True,
-        ],
-    ),
-)
-@pytest.mark.parametrize("execution_number", range(REPETITIONS))
-def test_rxn_string_and_is_mapped(
-    execution_number: int,
-    file_name: str,
-    rxn_idx: int,
-    expected_rxn_str: Optional[str],
-    expected_is_mapped: Optional[bool],
-) -> None:
-    rxn = get_rxn_func()(file_name, rxn_idx)
-
-    import orderly.extract.extractor
-
-    rxn_str_output = (
-        orderly.extract.extractor.OrdExtractor.get_rxn_string_and_is_mapped(rxn)
-    )
-    if rxn_str_output is None:
-        rxn_str, is_mapped = None, None
-    else:
-        rxn_str, is_mapped = rxn_str_output
-
-    assert expected_rxn_str == rxn_str, f"failure for {expected_rxn_str=} got {rxn_str}"
-    assert (
-        expected_is_mapped == is_mapped
-    ), f"failure for {expected_is_mapped=} got {is_mapped}"
-
-
-@pytest.mark.parametrize(
-    "file_name,rxn_idx,rxn_overwrite,expected_rxn_str_reactants,expected_rxn_str_agents,expected_rxn_str_products,expected_rxn_str,expected_non_smiles_names_list_additions,expected_none",
-    (
-        [
-            "ord_dataset-00005539a1e04c809a9a78647bea649c",
-            0,
-            None,
-            None,
-            None,
-            None,
-            None,
-            None,
-            True,
-        ],
-        [
-            "ord_dataset-0b70410902ae4139bd5d334881938f69",
-            0,
-            None,
-            [
-                "O=[N+]([O-])c1ccc(Oc2ccc(C(F)(F)F)cc2Cl)cc1[N+](=O)[O-]",
-                "SCc1ccccc1",
-            ],
-            [
-                "C1CCOC1",
-                "[H-]",
-                "[Na+]",
-            ],
-            ["O=[N+]([O-])c1ccc(Oc2ccc(C(F)(F)F)cc2Cl)cc1SCc1ccccc1"],
-            "[CH2:1]([SH:8])[C:2]1[CH:7]=[CH:6][CH:5]=[CH:4][CH:3]=1.[H-].[Na+].[Cl:11][C:12]1[CH:30]=[C:29]([C:31]([F:34])([F:33])[F:32])[CH:28]=[CH:27][C:13]=1[O:14][C:15]1[CH:20]=[CH:19][C:18]([N+:21]([O-:23])=[O:22])=[C:17]([N+]([O-])=O)[CH:16]=1>O1CCCC1>[CH2:1]([S:8][C:17]1[CH:16]=[C:15]([O:14][C:13]2[CH:27]=[CH:28][C:29]([C:31]([F:34])([F:32])[F:33])=[CH:30][C:12]=2[Cl:11])[CH:20]=[CH:19][C:18]=1[N+:21]([O-:23])=[O:22])[C:2]1[CH:7]=[CH:6][CH:5]=[CH:4][CH:3]=1",
-            [],
-            False,
-        ],
-        [
-            "ord_dataset-0bb2e99daa66408fb8dbd6a0781d241c",
-            0,
-            None,
-            [
-                "[O-]B([O-])[O-]",
-            ],
-            [
-                "O",
-                "[Na+]",
-            ],
-            [
-                "[O-]B1OB2OB([O-])OB(O1)O2",
-            ],
-            "[B:1]([O-:4])([O-:3])[O-:2].[B:5]([O-:8])([O-:7])[O-:6].[B:9]([O-:12])([O-])[O-].[B:13]([O-])([O-])[O-].[Na+:17].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+]>O>[B:1]1([O-:4])[O:3][B:13]2[O:12][B:9]([O:6][B:5]([O-:8])[O:7]2)[O:2]1.[Na+:17].[Na+:17]",
-            [],
-            False,
-        ],
-        [
-            "ord_dataset-0bf72e95d80743729fdbb8b57a4bc0c6",
-            0,
-            None,
-            [
-                "C1CCNC1",
-                "CC1(C)C2CCC(=O)C1C2",
-            ],
-            ["Cc1ccc(S(=O)(=O)O)cc1", "O", "c1ccccc1"],
-            ["CC1(C)C2CC=C(N3CCCC3)C1C2"],
-            "[CH3:1][C:2]1([CH3:10])[CH:8]2[CH2:9][CH:3]1[CH2:4][CH2:5][C:6]2=O.[NH:11]1[CH2:15][CH2:14][CH2:13][CH2:12]1.C1(C)C=CC(S(O)(=O)=O)=CC=1.O>C1C=CC=CC=1>[CH3:1][C:2]1([CH3:10])[CH:8]2[CH2:9][CH:3]1[CH2:4][CH:5]=[C:6]2[N:11]1[CH2:15][CH2:14][CH2:13][CH2:12]1",
-            [],
-            False,
-        ],
-        # test case where the products list starts non-empty but ends empty
-        # I think this is a crystalisation/protonation/stabilisation reaction
-        [
-            "ord_dataset-a0eff6fe4b4143f284f0fc5ac503acad",
-            10,
-            None,
-            [],
-            [
-                "Cc1cc2c([N+](=O)[O-])cccc2cn1",
-                "Cl",
-                "I",
-                "O=[N+]([O-])c1ccc(Cl)c2ccncc12",
-            ],
-            [],
-            "CC1N=CC2C(C=1)=C([N+]([O-])=O)C=CC=2.[Cl:15][C:16]1[CH:25]=[CH:24][C:23]([N+:26]([O-:28])=[O:27])=[C:22]2[C:17]=1[CH:18]=[CH:19][N:20]=[CH:21]2.Cl.CC1N=CC2C(C=1)=C([N+]([O-])=O)C=CC=2.[IH:44]>>[IH:44].[Cl:15][C:16]1[CH:25]=[CH:24][C:23]([N+:26]([O-:28])=[O:27])=[C:22]2[C:17]=1[CH:18]=[CH:19][N:20]=[CH:21]2",
-            [],
-            False,
-        ],
-        [
-            "ord_dataset-a0eff6fe4b4143f284f0fc5ac503acad",
-            1932,
-            None,
-            ["C=C(C)Br", "C=C1CC(=O)CCC2=C(C)CCC12"],
-            [
-                "C1CCOC1",
-                "II",
-                "[Mg]",
-            ],
-            ["C=C1CC(O)(C(=C)C)CCC2=C(C)CCC12"],
-            "[Mg].II.Br[C:5]([CH3:7])=[CH2:6].[CH3:8][C:9]1[CH2:10][CH2:11][CH:12]2[C:18]=1[CH2:17][CH2:16][C:15](=[O:19])[CH2:14][C:13]2=[CH2:20]>O1CCCC1>[OH:19][C:15]1([C:5]([CH3:7])=[CH2:6])[CH2:16][CH2:17][C:18]2[CH:12]([CH2:11][CH2:10][C:9]=2[CH3:8])[C:13](=[CH2:20])[CH2:14]1",
-            [],
-            False,
-        ],
-        [
-            "ord_dataset-85c00026681b46f89ef8634d2b8618c3",
-            3948,
-            None,
-            [
-                "O=S(=O)(O)O",
-                "[Co]",
-            ],
-            [
-                "CCCCCC=N",
-                "O=S(=O)([O-])[O-]",
-                "[Co+3]",
-                "[NH4+]",
-            ],
-            [],
-            "[Co:1].[S:2]([OH:6])([OH:5])(=[O:4])=[O:3].[CH:7](=[NH:13])[CH2:8][CH2:9][CH2:10][CH2:11][CH3:12].[S:14]([O-:18])([O-:17])(=[O:16])=[O:15].[NH4+].[NH4+].[Co+3]>>[S:2]([O-:6])([O-:5])(=[O:4])=[O:3].[CH:7](=[NH:13])[CH2:8][CH2:9][CH2:10][CH2:11][CH3:12].[Co+3:1].[S:14]([O-:18])([O-:17])(=[O:16])=[O:15].[S:2]([O-:6])([O-:5])(=[O:4])=[O:3].[Co+3:1]",
-            [],
-            False,
-        ],
-        # Test case where reaction with only 1 >
-        pytest.param(
-            "ord_dataset-0bf72e95d80743729fdbb8b57a4bc0c6",
-            0,
-            "CC.C>CCC",
-            ["CC", "C"],
-            [],
-            ["CCC"],
-            "CC.C>CCC",
-            [],
-            True,
-        ),
-        # There's no point in trying to test whether the the rxn.identifiers[0].value = None because the schema doesn't allow that overwrite to happen!
-    ),
-)
-@pytest.mark.parametrize("execution_number", range(REPETITIONS))
-def test_extract_info_from_rxn_str(
-    execution_number: int,
-    file_name: str,
-    rxn_idx: int,
-    rxn_overwrite: Optional[bool],
-    expected_rxn_str_reactants: Optional[List[str]],
-    expected_rxn_str_agents: Optional[List[str]],
-    expected_rxn_str_products: Optional[List[str]],
-    expected_rxn_str: Optional[str],
-    expected_non_smiles_names_list_additions: Optional[List[str]],
-    expected_none: bool,
-) -> None:
-    rxn = get_rxn_func()(file_name, rxn_idx)
-
-    if rxn_overwrite is not None:
-        rxn.identifiers[0].value = rxn_overwrite
-
-    import orderly.extract.extractor
-
-    _rxn_info = orderly.extract.extractor.OrdExtractor.get_rxn_string_and_is_mapped(rxn)
-    if _rxn_info is None:
-        return None
-    rxn_str, is_mapped = _rxn_info
-
-    rxn_info = orderly.extract.extractor.OrdExtractor.extract_info_from_rxn_str(
-        rxn_str, is_mapped
-    )
-    if expected_none:
-        assert rxn_info is None, f"expected a none but got {rxn_info=}"
-        return
-    else:
-        assert rxn_info is not None, f"did not expect a none but got one {rxn_info=}"
-    (
-        rxn_str_reactants,
-        rxn_str_agents,
-        rxn_str_products,
-        rxn_str,
-        non_smiles_names_list_additions,
-    ) = rxn_info
-
-    assert expected_rxn_str_reactants is not None
-    assert expected_rxn_str_agents is not None
-    assert expected_rxn_str_products is not None
-    assert expected_rxn_str is not None
-    assert expected_non_smiles_names_list_additions is not None
-
-    assert expected_rxn_str_reactants == rxn_str_reactants
-    assert expected_rxn_str_agents == rxn_str_agents
-    assert expected_rxn_str_products == rxn_str_products
-    assert expected_rxn_str == rxn_str
-    assert expected_non_smiles_names_list_additions == non_smiles_names_list_additions
-
-
-@pytest.mark.parametrize(
-    "file_name,rxn_idx,expected_temperature",
-    (
-        [
-            "ord_dataset-00005539a1e04c809a9a78647bea649c",
-            0,
-            110.0,
-        ],
-        ["ord_dataset-0b70410902ae4139bd5d334881938f69", 0, None],
-        ["ord_dataset-0bb2e99daa66408fb8dbd6a0781d241c", 0, 1100.0],
-        ["ord_dataset-0bf72e95d80743729fdbb8b57a4bc0c6", 0, None],
-    ),
-)
-@pytest.mark.parametrize("execution_number", range(REPETITIONS))
-def test_temperature_extractor(
-    execution_number: int,
-    file_name: str,
-    rxn_idx: int,
-    expected_temperature: Optional[float],
-) -> None:
-    rxn = get_rxn_func()(file_name, rxn_idx)
-
-    import orderly.extract.extractor
-
-    temperature = orderly.extract.extractor.OrdExtractor.temperature_extractor(rxn)
-
-    assert (
-        expected_temperature == temperature
-    ), f"failure for {expected_temperature=} got {temperature}"
-    if temperature is not None:
-        assert isinstance(
-            temperature, float
-        ), f"expected a float but got {temperature=}"
-
-
-@pytest.mark.parametrize(
-    "file_name,rxn_idx,expected_rxn_time",
-    (
-        ["ord_dataset-00005539a1e04c809a9a78647bea649c", 0, None],
-        ["ord_dataset-0b70410902ae4139bd5d334881938f69", 0, None],
-        ["ord_dataset-0bb2e99daa66408fb8dbd6a0781d241c", 0, 0.17],
-        ["ord_dataset-0bf72e95d80743729fdbb8b57a4bc0c6", 0, None],
-    ),
-)
-@pytest.mark.parametrize("execution_number", range(REPETITIONS))
-def test_time_extractor(
-    execution_number: int,
-    file_name: str,
-    rxn_idx: int,
-    expected_rxn_time: Optional[float],
-) -> None:
-    rxn = get_rxn_func()(file_name, rxn_idx)
-
-    import orderly.extract.extractor
-
-    rxn_time = orderly.extract.extractor.OrdExtractor.rxn_time_extractor(rxn)
-
-    assert (
-        expected_rxn_time == rxn_time
-    ), f"failure for {expected_rxn_time=} got {rxn_time=}"
-
-    if rxn_time is not None:
-        assert isinstance(rxn_time, float), f"expected a float but got {rxn_time=}"
-
-
-@pytest.mark.parametrize(
-    "rxn_str_agents,labelled_catalysts,labelled_solvents,labelled_reagents,solvents_set,expected_agents,expected_solvents",
-    (
-        [
-            None,
-            [
-                "c1ccc(P(c2ccccc2)c2ccc3ccccc3c2-c2c(P(c3ccccc3)c3ccccc3)ccc3ccccc23)cc1",
-                "O=C(/C=C/c1ccccc1)/C=C/c1ccccc1",
-                "[Pd]",
-            ],
-            [],
-            ["O=C([O-])[O-]", "[Cs+]"],
-            None,
-            [
-                "[Pd]",
-                "O=C(/C=C/c1ccccc1)/C=C/c1ccccc1",
-                "O=C([O-])[O-]",
-                "[Cs+]",
-                "c1ccc(P(c2ccccc2)c2ccc3ccccc3c2-c2c(P(c3ccccc3)c3ccccc3)ccc3ccccc23)cc1",
-            ],
-            [],
-        ],
-        [["C1CCOC1"], None, ["C1CCOC1", "C1CCOC1"], None, None, [], ["C1CCOC1"]],
-        [["O"], [], ["O"], [], None, [], ["O"]],
-        [
-            ["c1ccccc1", "Cc1ccc(S(=O)(=O)O)cc1", "O"],
-            [],
-            ["c1ccccc1"],
-            [],
-            None,
-            ["Cc1ccc(S(=O)(=O)O)cc1"],
-            ["O", "c1ccccc1"],
-        ],
-        # Made up test cases:
-        [
-            [
-                "c1ccccc1",
-                "Cc1ccc(S(=O)(=O)O)cc1",
-                "O",
-                None,
-            ],
-            ["[Pd]"],
-            ["O", "CCO"],
-            ["O=C([O-])[O-]"],
-            None,
-            ["[Pd]", "Cc1ccc(S(=O)(=O)O)cc1", "O=C([O-])[O-]"],
-            ["CCO", "O", "c1ccccc1"],
-        ],
-        pytest.param(
-            ["c1ccccc1", "Cc1ccc(S(=O)(=O)O)cc1", "O"],
-            ["[Pd]"],
-            ["O", "CCO"],
-            ["O=C([O-])[O-]"],
-            None,
-            ["c1ccccc1", "Cc1ccc(S(=O)(=O)O)cc1", "O"],
-            ["O", "CCO"],
-            marks=pytest.mark.xfail,
-        ),
-        pytest.param(
-            ["c1ccccc1", "Cc1ccc(S(=O)(=O)O)cc1", "O"],
-            ["[Pd]"],
-            ["O", "CCO"],
-            ["O=C([O-])[O-]"],
-            None,
-            ["[Pd]", "Cc1ccc(S(=O)(=O)O)cc1", "O=C([O-])[O-]", "O", "CCO", "c1ccccc1"],
-            [],
-            marks=pytest.mark.xfail,
-        ),
-        pytest.param(
-            ["c1ccccc1", "Cc1ccc(S(=O)(=O)O)cc1", "O"],
-            ["[Pd]"],
-            ["O", "CCO"],
-            ["O=C([O-])[O-]"],
-            None,
-            ["[Pd]", "Cc1ccc(S(=O)(=O)O)cc1", "O=C([O-])[O-]"],
-            ["O", "O", "CCO", "c1ccccc1"],
-            marks=pytest.mark.xfail,
-        ),
-    ),
-)
-@pytest.mark.parametrize("execution_number", range(REPETITIONS))
-def test_merge_to_agents(
-    execution_number: int,
-    rxn_str_agents: Optional[List[str]],
-    labelled_catalysts: Optional[List[str]],
-    labelled_solvents: Optional[List[str]],
-    labelled_reagents: Optional[List[str]],
-    solvents_set: Set[str],
-    expected_agents: Optional[List[str]],
-    expected_solvents: Optional[List[str]],
-) -> None:
-    import orderly.extract.extractor
-    import orderly.extract.defaults
-
-    if solvents_set is None:
-        solvents_set = orderly.extract.defaults.get_solvents_set()
-
-    agents, solvents = orderly.extract.extractor.OrdExtractor.merge_to_agents(
-        rxn_str_agents,
-        labelled_catalysts,
-        labelled_solvents,
-        labelled_reagents,
-        solvents_set,
-    )
-
-    assert expected_agents == agents, f"failure for {expected_agents=} got {agents}"
-    assert (
-        expected_solvents == solvents
-    ), f"failure for {expected_solvents=} got {solvents}"
-
-
-@pytest.mark.parametrize(
-    "rxn_str_products,labelled_products,input_yields,expected_products,expected_yields",
-    (
-        [
-            [],
-            ["CCOC(=O)c1cnc2cc(OCC)c(N3CCN(C(C)C)CC3)cc2c1Nc1ccc(F)cc1F"],
-            [65.39],
-            [],
-            [],
-        ],
-        [
-            ["O=[N+]([O-])c1ccc(Oc2ccc(C(F)(F)F)cc2Cl)cc1SCc1ccccc1"],
-            ["O=[N+]([O-])c1ccc(Oc2ccc(C(F)(F)F)cc2Cl)cc1SCc1ccccc1"],
-            [None],
-            ["O=[N+]([O-])c1ccc(Oc2ccc(C(F)(F)F)cc2Cl)cc1SCc1ccccc1"],
-            [None],
-        ],
-        [
-            ["[Na+]", "[Na+]", "[O-]B1OB2OB([O-])OB(O1)O2"],
-            ["[Na+]", "[Na+]", "[O-]B1OB2OB([O-])OB(O1)O2"],
-            [None, None, None],
-            ["[Na+]", "[Na+]", "[O-]B1OB2OB([O-])OB(O1)O2"],
-            [None, None, None],
-        ],
-        pytest.param(
-            ["[Na+]", "[Na+]", "[O-]B1OB2OB([O-])OB(O1)O2"],
-            ["[Na+]", "[Na+]", "[O-]B1OB2OB([O-])OB(O1)O2"],
-            [None],
-            ["[Na+]", "[Na+]", "[O-]B1OB2OB([O-])OB(O1)O2"],
-            [None],
-            marks=pytest.mark.xfail(reason="IndexError: list index out of range"),
-        ),
-        [
-            ["O=[N+]([O-])c1ccc(Oc2ccc(C(F)(F)F)cc2Cl)cc1SCc1ccccc1"],
-            ["[Na+]", "[Na+]", "[O-]B1OB2OB([O-])OB(O1)O2"],
-            [None, None, None],
-            ["O=[N+]([O-])c1ccc(Oc2ccc(C(F)(F)F)cc2Cl)cc1SCc1ccccc1"],
-            [None],
-        ],
-        [
-            ["CC1(C)C2CC=C(N3CCCC3)C1C2"],
-            ["CC1(C)C2CC=C(N3CCCC3)C1C2"],
-            [95.0],
-            ["CC1(C)C2CC=C(N3CCCC3)C1C2"],
-            [95.0],
-        ],
-    ),
-)
-@pytest.mark.parametrize("execution_number", range(REPETITIONS))
-def test_match_yield_with_product(
-    execution_number: int,
-    rxn_str_products: List[str],
-    labelled_products: List[str],
-    input_yields: List[Optional[YIELD]],
-    expected_products: List[str],
-    expected_yields: List[Optional[YIELD]],
-) -> None:
-    import orderly.extract.extractor
-
-    products, yields = orderly.extract.extractor.OrdExtractor.match_yield_with_product(
-        rxn_str_products, labelled_products, input_yields
-    )
-
-    assert (
-        expected_products == products
-    ), f"failure for {expected_products=} got {products=}"
-    assert expected_yields == yields, f"failure for {expected_yields=} got {yields=}"
-
-
-@pytest.mark.parametrize(
-    "file_name,rxn_idx,manual_replacements_dict,trust_labelling,expected_reactants, expected_agents, expected_reagents,expected_solvents,expected_catalysts,expected_products,expected_yields,expected_temperature,expected_rxn_time,expected_rxn_str, expected_procedure_details, expected_date_of_experiment, expected_names_list, expected_is_mapped",
-    (
-        [
-            "ord_dataset-00005539a1e04c809a9a78647bea649c",
-            0,
-            {},
-            False,
-            ["CC(C)N1CCNCC1", "CCOC(=O)c1cnc2cc(OCC)c(Br)cc2c1Nc1ccc(F)cc1F"],
-            [
-                "[Pd]",
-                "O=C(/C=C/c1ccccc1)/C=C/c1ccccc1",
-                "O=C([O-])[O-]",
-                "[Cs+]",
-                "c1ccc(P(c2ccccc2)c2ccc3ccccc3c2-c2c(P(c3ccccc3)c3ccccc3)ccc3ccccc23)cc1",
-            ],
-            [],
-            [],
-            [],
-            ["CCOC(=O)c1cnc2cc(OCC)c(N3CCN(C(C)C)CC3)cc2c1Nc1ccc(F)cc1F"],
-            [65.39],
-            110.0,
-            None,
-            None,
-            "To a solution of ethyl 6-bromo-4-(2,4-difluorophenylamino)-7-ethoxyquinoline-3-carboxylate (400 mg, 0.89 mmol) and 1-(Isopropyl)piperazine (254 µl, 1.77 mmol) in dioxane was added cesium carbonate (722 mg, 2.22 mmol), tris(dibenzylideneacetone)dipalladium(0) (40.6 mg, 0.04 mmol) and rac-2,2'-Bis(diphenylphosphino)-1,1'-binaphthyl (55.2 mg, 0.09 mmol). Reaction vessel in oil bath set to 110 °C. 11am  After 5 hours, MS shows product (major peak 499), and SM (minor peak 453).  o/n, MS shows product peak. Reaction cooled, concentrated onto silica, and purified on ISCO. 40g column, 1:1 EA:Hex, then 100% EA.  289mg yellow solid. NMR (EN00180-62-1) supports product, but some oxidised BINAP impurity (LCMS 655).  ",
-            "07/01/2008",
-            [],
-            False,
-        ],
-        [
-            "ord_dataset-0b70410902ae4139bd5d334881938f69",
-            0,
-            {},
-            False,
-            [
-                "SCc1ccccc1",
-                "O=[N+]([O-])c1ccc(Oc2ccc(C(F)(F)F)cc2Cl)cc1[N+](=O)[O-]",
-            ],
-            ["[H-]", "[Na+]"],
-            [],
-            ["C1CCOC1"],
-            [],
-            ["O=[N+]([O-])c1ccc(Oc2ccc(C(F)(F)F)cc2Cl)cc1SCc1ccccc1"],
-            [None],
-            None,
-            None,
-            "[CH2:1]([SH:8])[C:2]1[CH:7]=[CH:6][CH:5]=[CH:4][CH:3]=1.[H-].[Na+].[Cl:11][C:12]1[CH:30]=[C:29]([C:31]([F:34])([F:33])[F:32])[CH:28]=[CH:27][C:13]=1[O:14][C:15]1[CH:20]=[CH:19][C:18]([N+:21]([O-:23])=[O:22])=[C:17]([N+]([O-])=O)[CH:16]=1>O1CCCC1>[CH2:1]([S:8][C:17]1[CH:16]=[C:15]([O:14][C:13]2[CH:27]=[CH:28][C:29]([C:31]([F:34])([F:32])[F:33])=[CH:30][C:12]=2[Cl:11])[CH:20]=[CH:19][C:18]=1[N+:21]([O-:23])=[O:22])[C:2]1[CH:7]=[CH:6][CH:5]=[CH:4][CH:3]=1",
-            "1.7 g of benzyl mercaptan was dissolved in dry tetrahydrofuran and 0.5 g of sodium hydride added with stirring under dry nitrogen. The reaction mixture was stirred under reflux for 30 minutes, and a solution of 5 g of 1A dissolved in 25 ml of dry tetrahydrofuran was added dropwise. Reaction occurred rapidly, and the product was chromatographically purified to give 2-benzylthio-4-(2-chloro-4-trifluoromethylphenoxy)nitrobenzene (1B) as a yellow oil.",
-            None,
-            [],
-            True,
-        ],
-        [
-            "ord_dataset-0bb2e99daa66408fb8dbd6a0781d241c",
-            0,
-            {},
-            False,
-            ["[O-]B([O-])[O-]"],
-            [
-                "[Na+]",
-                "35(Na2O)",
-            ],
-            [],
-            ["O"],
-            [],
-            ["[O-]B1OB2OB([O-])OB(O1)O2"],
-            [None],
-            1100.0,
-            0.17,
-            "[B:1]([O-:4])([O-:3])[O-:2].[B:5]([O-:8])([O-:7])[O-:6].[B:9]([O-:12])([O-])[O-].[B:13]([O-])([O-])[O-].[Na+:17].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+]>O>[B:1]1([O-:4])[O:3][B:13]2[O:12][B:9]([O:6][B:5]([O-:8])[O:7]2)[O:2]1.[Na+:17].[Na+:17]",
-            "Sodium tetraborate (Na2B4O7.10H2O), analyzed reagent was dried overnight at 150° C, mixed with the appropriate quantity of dopant ions and homogenized in an electric homogenizer (vibrator) during 10 minutes. The material was then transferred to a platinum crucible and heated at 1100° C for at least 30 minutes, until a clear transparent solution was obtained. The glass matrix loses water and the composition of the matrix is after the heating 35(Na2O).65(B2O3). A drop of the hot melt was allowed to fall directly onto a clean white glazed ceramic surface, into the center of a space ring of 1 mm thickness, and pressed with a second ceramic tile to produce a glass disk of 1 mm thickness and an approximate diameter of 12 mm. The glass is transparent in the ultraviolet and in the visible part of the spectrum.",
-            None,
-            ["35(Na2O)"],
-            True,
-        ],
-        [
-            "ord_dataset-0bb2e99daa66408fb8dbd6a0781d241c",
-            0,
-            {},
-            True,
-            [
-                "[Na+]",
-                "[Na+]",
-                "[Na+]",
-                "[Na+]",
-                "[Na+]",
-                "[Na+]",
-                "[Na+]",
-                "[Na+]",
-                "[Na+]",
-                "[Na+]",
-                "[Na+]",
-                "[Na+]",
-                "[O-]B([O-])[O-]",
-                "[O-]B([O-])[O-]",
-                "[O-]B([O-])[O-]",
-                "[O-]B([O-])[O-]",
-                "35(Na2O)",
-            ],
-            [],
-            [],
-            ["O"],
-            [],
-            [
-                "[O-]B1OB2OB([O-])OB(O1)O2",
-                "[Na+]",
-                "[Na+]",
-            ],
-            [None, None, None],
-            1100.0,
-            0.17,
-            "[B:1]([O-:4])([O-:3])[O-:2].[B:5]([O-:8])([O-:7])[O-:6].[B:9]([O-:12])([O-])[O-].[B:13]([O-])([O-])[O-].[Na+:17].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+]>O>[B:1]1([O-:4])[O:3][B:13]2[O:12][B:9]([O:6][B:5]([O-:8])[O:7]2)[O:2]1.[Na+:17].[Na+:17]",
-            "Sodium tetraborate (Na2B4O7.10H2O), analyzed reagent was dried overnight at 150° C, mixed with the appropriate quantity of dopant ions and homogenized in an electric homogenizer (vibrator) during 10 minutes. The material was then transferred to a platinum crucible and heated at 1100° C for at least 30 minutes, until a clear transparent solution was obtained. The glass matrix loses water and the composition of the matrix is after the heating 35(Na2O).65(B2O3). A drop of the hot melt was allowed to fall directly onto a clean white glazed ceramic surface, into the center of a space ring of 1 mm thickness, and pressed with a second ceramic tile to produce a glass disk of 1 mm thickness and an approximate diameter of 12 mm. The glass is transparent in the ultraviolet and in the visible part of the spectrum.",
-            None,
-            ["35(Na2O)"],
-            True,
-        ],
-        [
-            "ord_dataset-0bf72e95d80743729fdbb8b57a4bc0c6",
-            0,
-            {},
-            False,
-            [
-                "CC1(C)C2CCC(=O)C1C2",
-                "C1CCNC1",
-            ],
-            [
-                "Cc1ccc(S(=O)(=O)O)cc1",
-            ],
-            [],
-            [
-                "O",
-                "c1ccccc1",
-            ],
-            [],
-            ["CC1(C)C2CC=C(N3CCCC3)C1C2"],
-            [95.0],
-            None,
-            None,
-            "[CH3:1][C:2]1([CH3:10])[CH:8]2[CH2:9][CH:3]1[CH2:4][CH2:5][C:6]2=O.[NH:11]1[CH2:15][CH2:14][CH2:13][CH2:12]1.C1(C)C=CC(S(O)(=O)=O)=CC=1.O>C1C=CC=CC=1>[CH3:1][C:2]1([CH3:10])[CH:8]2[CH2:9][CH:3]1[CH2:4][CH:5]=[C:6]2[N:11]1[CH2:15][CH2:14][CH2:13][CH2:12]1",
-            "A solution of 30 g of nopinone ([α]D20 =+39.90; c=8 in ethanol), 29 of pyrrolidine and 0.4 g of p-toluenesulfonic acid in 150 ml anhydrous benzene was heated at reflux for 40 h under nitrogen atmosphere in a vessel fitted with a water separator. After evaporation of the solvent and distillation of the residue, there were obtained 39.5 g (95% yield) of 1-(6,6-dimethylnorpin-2-en-2-yl)-pyrrolidine having b.p. 117°-118° C./10 Torr.",
-            None,
-            [],
-            True,
-        ],
-        [
-            "ord_dataset-0bf72e95d80743729fdbb8b57a4bc0c6",
-            0,
-            {},
-            True,
-            [
-                "C1CCNC1",
-                "CC1(C)C2CCC(=O)C1C2",
-                "O",
-                "Cc1ccc(S(=O)(=O)O)cc1",
-            ],
-            [],
-            [],
-            ["c1ccccc1"],
-            [],
-            ["CC1(C)C2CC=C(N3CCCC3)C1C2"],
-            [95.0],
-            None,
-            None,
-            "[CH3:1][C:2]1([CH3:10])[CH:8]2[CH2:9][CH:3]1[CH2:4][CH2:5][C:6]2=O.[NH:11]1[CH2:15][CH2:14][CH2:13][CH2:12]1.C1(C)C=CC(S(O)(=O)=O)=CC=1.O>C1C=CC=CC=1>[CH3:1][C:2]1([CH3:10])[CH:8]2[CH2:9][CH:3]1[CH2:4][CH:5]=[C:6]2[N:11]1[CH2:15][CH2:14][CH2:13][CH2:12]1",
-            "A solution of 30 g of nopinone ([α]D20 =+39.90; c=8 in ethanol), 29 of pyrrolidine and 0.4 g of p-toluenesulfonic acid in 150 ml anhydrous benzene was heated at reflux for 40 h under nitrogen atmosphere in a vessel fitted with a water separator. After evaporation of the solvent and distillation of the residue, there were obtained 39.5 g (95% yield) of 1-(6,6-dimethylnorpin-2-en-2-yl)-pyrrolidine having b.p. 117°-118° C./10 Torr.",
-            None,
-            [],
-            True,
-        ],
-        # Test: one of the input reactants = 'liquid'; trust_labelling = True
-        [
-            "ord_dataset-0b70410902ae4139bd5d334881938f69",
-            3,
-            {},
-            True,
-            ["Clc1nc(Cl)nc(Cl)n1", "N"],
-            [],
-            [],
-            ["C1CCOC1", "COCCOCCOC"],
-            [],
-            ["Nc1nc(Cl)nc(Cl)n1"],
-            [None],
-            25,
-            1.0,
-            "[N:1]1[C:8]([Cl:9])=[N:7][C:5]([Cl:6])=[N:4][C:2]=1Cl.[NH3:10]>C1COCC1.COCCOCCOC>[NH2:10][C:2]1[N:1]=[C:8]([Cl:9])[N:7]=[C:5]([Cl:6])[N:4]=1",
-            "A solution of 300 g (1.63 mol) of cyanuric chloride in 1 liter THF and 0.24 liter diglyme was cooled to 0\302\260 C. and 81.6 mL (3.36 mol) of liquid ammonia added dropwise over 90 min. keeping the temperature between 10\302\260-15\302\260. The mixture was stirred for one hour at -10\302\260 to 0\302\260 and then allowed to warm to ambient temperature over one hour. The resulting suspension was filtered, the solid washed with THF, the filtrate reduced to 1/2 its original volume, and poured over 1 liter of ice water to give a white solid which was collected, washed with water, and dried in vacuo to give 244.3 g of 2-amino-4,6-dichloro-1,3,5-triazine with m.p. 221\302\260-223.5\302\260 (dec).",
-            None,
-            ["liquid"],
-            True,
-        ],
-        # Test: one of the input reactants = 'liquid'; trust_labelling = False
-        [
-            "ord_dataset-0b70410902ae4139bd5d334881938f69",
-            3,
-            {},
-            False,
-            ["Clc1nc(Cl)nc(Cl)n1", "N"],
-            [],
-            [],
-            ["C1CCOC1", "COCCOCCOC"],
-            [],
-            ["Nc1nc(Cl)nc(Cl)n1"],
-            [None],
-            25,
-            1.0,
-            "[N:1]1[C:8]([Cl:9])=[N:7][C:5]([Cl:6])=[N:4][C:2]=1Cl.[NH3:10]>C1COCC1.COCCOCCOC>[NH2:10][C:2]1[N:1]=[C:8]([Cl:9])[N:7]=[C:5]([Cl:6])[N:4]=1",
-            "A solution of 300 g (1.63 mol) of cyanuric chloride in 1 liter THF and 0.24 liter diglyme was cooled to 0\302\260 C. and 81.6 mL (3.36 mol) of liquid ammonia added dropwise over 90 min. keeping the temperature between 10\302\260-15\302\260. The mixture was stirred for one hour at -10\302\260 to 0\302\260 and then allowed to warm to ambient temperature over one hour. The resulting suspension was filtered, the solid washed with THF, the filtrate reduced to 1/2 its original volume, and poured over 1 liter of ice water to give a white solid which was collected, washed with water, and dried in vacuo to give 244.3 g of 2-amino-4,6-dichloro-1,3,5-triazine with m.p. 221\302\260-223.5\302\260 (dec).",
-            None,
-            ["liquid"],
-            True,
-        ],
-        # synthesis of islatravir by biocatalytic cascade
-        # We put trust_labelling = False to test that the inputs are extracted instead, since I know that there's no rxn string
-        [
-            "ord_dataset-6a0bfcdf53a64c07987822162ae591e2",
-            0,
-            {},
-            False,
-            ["C#CC(O)(CO)CO"],
-            [
-                "[Cu+2]",
-                "O=S(=O)([O-])CCN1CCN(CCS(=O)(=O)[O-])CC1",
-                "O=S(=O)([O-])[O-]",
-                "[K+]",
-                "Antifoam 204",
-                "bovine catalase",
-                "evolved galactose oxidase GOase-Rd13BB",
-                "horseradish peroxidase",
-            ],
-            [],
-            ["O"],
-            [],
-            ["C#C[C@](O)(C=O)CO"],
-            [68.0],
-            25.0,
-            22.0,
-            None,
-            "",
-            None,
-            [
-                "Antifoam 204",
-                "bovine catalase",
-                "evolved galactose oxidase GOase-Rd13BB",
-                "horseradish peroxidase",
-            ],
-            False,
-        ],
-        # An example where we need the manual_replacements_dict
-        [
-            "ord_dataset-0b70410902ae4139bd5d334881938f69",
-            982,
-            {},
-            True,
-            [
-                "CCO",
-                "O",
-                "COc1ccccc1C(O)c1cccc(Br)n1",
-                "O=[Cr](=O)=O",
-            ],
-            [],
-            [],
-            ["CC(=O)O"],
-            [],
-            ["COc1ccccc1C(=O)c1cccc(Br)n1"],
-            [66.2],
-            None,
-            None,
-            "[Br:1][C:2]1[N:7]=[C:6]([CH:8]([C:10]2[CH:15]=[CH:14][CH:13]=[CH:12][C:11]=2[O:16][CH3:17])[OH:9])[CH:5]=[CH:4][CH:3]=1.C(O)C.O>C(O)(=O)C>[Br:1][C:2]1[N:7]=[C:6]([C:8](=[O:9])[C:10]2[CH:15]=[CH:14][CH:13]=[CH:12][C:11]=2[O:16][CH3:17])[CH:5]=[CH:4][CH:3]=1",
-            "By the same procedure of Ex. 22, and reacting 3.3 g 6-bromo-\316\261-(2-methoxyphenyl)-2-pyridinemethanol (obtained as in Ex. 19) in 20 ml glacial acetic acid with CrO3 (1 g in 5 ml water), there is obtained 2.17 g title product, m.p. 97\302\260-8\302\260 C. (ethanol:water); UV (ethanol):\316\273max. 278 nm, \316\265: 12,480; Br 27.67 (27.36).",
-            None,
-            ["CrO3"],
-            True,
-        ],
-        [
-            "ord_dataset-0b70410902ae4139bd5d334881938f69",
-            982,
-            {},
-            False,
-            [
-                "COc1ccccc1C(O)c1cccc(Br)n1",
-            ],
-            [
-                "O=[Cr](=O)=O",
-            ],
-            [],
-            ["CC(=O)O", "CCO", "O"],
-            [],
-            ["COc1ccccc1C(=O)c1cccc(Br)n1"],
-            [66.2],
-            None,
-            None,
-            "[Br:1][C:2]1[N:7]=[C:6]([CH:8]([C:10]2[CH:15]=[CH:14][CH:13]=[CH:12][C:11]=2[O:16][CH3:17])[OH:9])[CH:5]=[CH:4][CH:3]=1.C(O)C.O>C(O)(=O)C>[Br:1][C:2]1[N:7]=[C:6]([C:8](=[O:9])[C:10]2[CH:15]=[CH:14][CH:13]=[CH:12][C:11]=2[O:16][CH3:17])[CH:5]=[CH:4][CH:3]=1",
-            "By the same procedure of Ex. 22, and reacting 3.3 g 6-bromo-\316\261-(2-methoxyphenyl)-2-pyridinemethanol (obtained as in Ex. 19) in 20 ml glacial acetic acid with CrO3 (1 g in 5 ml water), there is obtained 2.17 g title product, m.p. 97\302\260-8\302\260 C. (ethanol:water); UV (ethanol):\316\273max. 278 nm, \316\265: 12,480; Br 27.67 (27.36).",
-            None,
-            ["CrO3"],
-            True,
-        ],
-        [
-            "ord_dataset-a0eff6fe4b4143f284f0fc5ac503acad",
-            1932,
-            {},
-            False,
-            ["C=C(C)Br", "C=C1CC(=O)CCC2=C(C)CCC12"],
-            [
-                "II",
-                "[Mg]",
-            ],
-            [],
-            [
-                "C1CCOC1",
-            ],
-            [],
-            ["C=C1CC(O)(C(=C)C)CCC2=C(C)CCC12"],
-            [76.0],
-            None,
-            0.5,
-            "[Mg].II.Br[C:5]([CH3:7])=[CH2:6].[CH3:8][C:9]1[CH2:10][CH2:11][CH:12]2[C:18]=1[CH2:17][CH2:16][C:15](=[O:19])[CH2:14][C:13]2=[CH2:20]>O1CCCC1>[OH:19][C:15]1([C:5]([CH3:7])=[CH2:6])[CH2:16][CH2:17][C:18]2[CH:12]([CH2:11][CH2:10][C:9]=2[CH3:8])[C:13](=[CH2:20])[CH2:14]1",
-            "To a Grignard solution, prepared from 1 g of magnesium chips activated with 1 g of iodine, 5 ml of 2-bromopropene and about 100 ml of tetrahydrofuran, were added over 10 minutes 1.76 g of 1-methyl-4-methylen-6-oxo-2,3,3a,4,5,6,7,8-octahydroazulene. The mixture was stirred vigorously for 30 minutes, cooled to 0\302\260 and treated with excess ice-cold ammonium chloride solution. The mixture was then extracted with ether, the organic extract washed with carbonate solution and water, dried over magnesium sulphate and concentrated under reduced pressure. The crude product (2.6 g), which was obtained in the form of a yellow oil, was distilled under high vacuum and yielded 1.6 g (yield 76%) of pure 6-hydroxy-6-isopropenyl-1-methyl-4-methylen-2,3,3a,4,5,6,7,8-octahydroazulene; b.p.0.1 ca 100\302\260 IR(film):\316\275max = 3550, 3090, 1640, 1450/40, 1378, 1330, 1220, 1165, 1105, 1065, 1038, 900/895, 780 cm-1. The compound has a woody, slightly camphorous, somewhat spicy odour.",
-            None,
-            [],
-            True,
-        ],
-        [
-            "ord_dataset-a0eff6fe4b4143f284f0fc5ac503acad",
-            1932,
-            {},
-            True,
-            [
-                "C=C(C)Br",
-                "C=C1CC(=O)CCC2=C(C)CCC12",
-                "II",
-                "[Mg]",
-            ],
-            [],
-            [],
-            [
-                "C1CCOC1",
-            ],
-            [],
-            ["C=C1CC(O)(C(=C)C)CCC2=C(C)CCC12"],
-            [76.0],
-            None,
-            0.5,
-            "[Mg].II.Br[C:5]([CH3:7])=[CH2:6].[CH3:8][C:9]1[CH2:10][CH2:11][CH:12]2[C:18]=1[CH2:17][CH2:16][C:15](=[O:19])[CH2:14][C:13]2=[CH2:20]>O1CCCC1>[OH:19][C:15]1([C:5]([CH3:7])=[CH2:6])[CH2:16][CH2:17][C:18]2[CH:12]([CH2:11][CH2:10][C:9]=2[CH3:8])[C:13](=[CH2:20])[CH2:14]1",
-            "To a Grignard solution, prepared from 1 g of magnesium chips activated with 1 g of iodine, 5 ml of 2-bromopropene and about 100 ml of tetrahydrofuran, were added over 10 minutes 1.76 g of 1-methyl-4-methylen-6-oxo-2,3,3a,4,5,6,7,8-octahydroazulene. The mixture was stirred vigorously for 30 minutes, cooled to 0\302\260 and treated with excess ice-cold ammonium chloride solution. The mixture was then extracted with ether, the organic extract washed with carbonate solution and water, dried over magnesium sulphate and concentrated under reduced pressure. The crude product (2.6 g), which was obtained in the form of a yellow oil, was distilled under high vacuum and yielded 1.6 g (yield 76%) of pure 6-hydroxy-6-isopropenyl-1-methyl-4-methylen-2,3,3a,4,5,6,7,8-octahydroazulene; b.p.0.1 ca 100\302\260 IR(film):\316\275max = 3550, 3090, 1640, 1450/40, 1378, 1330, 1220, 1165, 1105, 1065, 1038, 900/895, 780 cm-1. The compound has a woody, slightly camphorous, somewhat spicy odour.",
-            None,
-            [],
-            True,
-        ],
-        [
-            "ord_dataset-85c00026681b46f89ef8634d2b8618c3",
-            3948,
-            {},
-            False,
-            [
-                "[Co]",
-                "O=S(=O)(O)O",
-            ],
-            ["[Co+3]", "CCCCCC=N", "O=S(=O)([O-])[O-]", "[NH4+]"],
-            [],
-            [],
-            [],
-            [],
-            [],
-            None,
-            None,
-            "[Co:1].[S:2]([OH:6])([OH:5])(=[O:4])=[O:3].[CH:7](=[NH:13])[CH2:8][CH2:9][CH2:10][CH2:11][CH3:12].[S:14]([O-:18])([O-:17])(=[O:16])=[O:15].[NH4+].[NH4+].[Co+3]>>[S:2]([O-:6])([O-:5])(=[O:4])=[O:3].[CH:7](=[NH:13])[CH2:8][CH2:9][CH2:10][CH2:11][CH3:12].[Co+3:1].[S:14]([O-:18])([O-:17])(=[O:16])=[O:15].[S:2]([O-:6])([O-:5])(=[O:4])=[O:3].[Co+3:1]",
-            "In a process for producing cobalt metal powder from nickel-cobalt sulphides comprising leaching said nickel-cobalt sulphides in an ammoniacal ammonium sulphate solution under an elevated pressure of an oxygen bearing gas, at a temperature of at least 80\302\260 C., with an effective ammonia to metals mole ratio in the range of 5:1 to 6.5:1 to oxidize the nickel and cobalt sulphides to sulphates, and to produce an ammoniacal ammonium sulphate leach liquor in which dissolved cobalt is predominantly in the (III) oxidation state, and an ammoniacal ammonium sulphate leach residue containing a cobalt (III) hexannmine sulphate-calcium sulphate double salt, separating the ammoniacal ammonium sulphate leach liquor from the ammoniacal ammonium sulphate leach residue, saturating the ammoniacal ammonium sulphate leach liquor with an effective amount of anydrous ammonia and cooling the ammoniated leach liquor to below 50\302\260 C. to precipitate the triple salt of cobalt (III) hexammine supbate, nickel (II) hexammine sulphate and ammonium sulphate, recovering the precipitated triple salt from the leach liquor, repulping the triple salt with an effective amount of water to selectively leach nickel(II) hexammine sulphate and to produce a crystalline cobalt (III) hexammine sulphate with a Co:Ni ratio of at least 100:1 and a nickel enriched leach liquor, dissolving the cobalt (III) hexammine sulphate in hot ammonium sulphate solution, and cooling the solution to precipitate recrystallized cobalt (III) hexammine sulphate having a Co:Ni ratio of at least about 1000:1 and treating the recrystallized cobalt (III) hexammine sulphate to produce cobalt metal therefrom, the improvement comprising:",
-            None,
-            [],
-            True,
-        ],
-    ),
-)
-@pytest.mark.parametrize("execution_number", range(REPETITIONS))
-def test_handle_reaction_object(
-    execution_number: int,
-    file_name: str,
-    rxn_idx: int,
-    manual_replacements_dict: MANUAL_REPLACEMENTS_DICT,
-    trust_labelling: bool,
-    expected_reactants: List[str],
-    expected_agents: List[str],
-    expected_reagents: List[str],
-    expected_solvents: List[str],
-    expected_catalysts: List[str],
-    expected_products: List[str],
-    expected_yields: List[Optional[float]],
-    expected_temperature: Optional[float],
-    expected_rxn_time: Optional[float],
-    expected_rxn_str: Optional[str],
-    expected_procedure_details: str,
-    expected_date_of_experiment: Optional[str],
-    expected_names_list: List[str],
-    expected_is_mapped: bool,
-) -> None:
-    import orderly.extract.extractor
-    import orderly.extract.main
-    import orderly.extract.defaults
-    import pandas as pd
-
-    rxn = get_rxn_func()(file_name, rxn_idx)
-    if manual_replacements_dict == {}:
-        manual_replacements_dict = orderly.extract.main.get_manual_replacements_dict(
-            solvents_path=None
-        )
-
-    assert manual_replacements_dict is not None
-
-    solvents_set = orderly.extract.defaults.get_solvents_set()
-
-    rnx_object = orderly.extract.extractor.OrdExtractor.handle_reaction_object(
-        rxn,
-        manual_replacements_dict,
-        solvents_set,
-        trust_labelling,
-        consider_molecule_names=True,
-    )
-
-    assert rnx_object is not None
-
-    (
-        reactants,
-        agents,
-        reagents,
-        solvents,
-        catalysts,
-        products,
-        yields,
-        temperature,
-        rxn_time,
-        rxn_str,
-        procedure_details,
-        date_of_experiment,
-        is_mapped,
-        names_list,
-    ) = rnx_object
-
-    def clean_string(s: str) -> str:
-        import string
-
-        printable = set(string.printable)
-        return "".join(filter(lambda x: x in printable, s))
-
-    clean_procedure_details = clean_string(procedure_details)
-    clean_expected_procedure_details = clean_string(expected_procedure_details)
-
-    assert sorted(reactants) == sorted(
-        expected_reactants
-    ), f"failure for {sorted(expected_reactants)=} got {sorted(reactants)}"  # TODO unsure why we have random ordering on ubuntu
-    assert agents == expected_agents, f"failure for {expected_agents=} got {agents}"
-    assert (
-        reagents == expected_reagents
-    ), f"failure for {expected_reagents=} got {reagents}"
-    assert (
-        solvents == expected_solvents
-    ), f"failure for {expected_solvents=} got {solvents}"
-    assert (
-        catalysts == expected_catalysts
-    ), f"failure for {expected_catalysts=} got {catalysts}"
-    assert (
-        products == expected_products
-    ), f"failure for {expected_products=} got {products}"
-    assert yields == expected_yields, f"failure for {expected_yields=} got {yields}"
-    assert (
-        temperature == expected_temperature
-    ), f"failure for {expected_temperature=} got {temperature}"
-    assert (
-        rxn_time == expected_rxn_time
-    ), f"failure for {expected_rxn_time=} got {rxn_time}"
-    assert rxn_str == expected_rxn_str, f"failure for {expected_rxn_str=} got {rxn_str}"
-    assert (
-        names_list == expected_names_list
-    ), f"failure for {expected_names_list=} got {names_list}"
-    assert (
-        clean_procedure_details == clean_expected_procedure_details
-    ), f"failure for {clean_expected_procedure_details=} got {clean_procedure_details}"
-    assert date_of_experiment == pd.to_datetime(
-        expected_date_of_experiment, format="%m/%d/%Y"
-    ), f"failure for {expected_date_of_experiment=} got {date_of_experiment}"
-    assert (
-        is_mapped == expected_is_mapped
-    ), f"failure for {expected_is_mapped=} got {is_mapped}"
-
-
-@pytest.mark.parametrize(
-    "smiles,is_mapped,expected_canonical_smiles",
-    (
-        ["teststring", True, None],
-        ["teststring", False, None],
-        ["c1ccccc1", False, "c1ccccc1"],
-        [
-            "[CH2:1]([S:8][C:9]1[CH:14]=[C:13]([O:15][C:16]2[CH:21]=[CH:20][C:19]([C:22]([F:25])([F:24])[F:23])=[CH:18][C:17]=2[Cl:26])[CH:12]=[CH:11][C:10]=1[N+:27]([O-])=O)[C:2]1[CH:7]=[CH:6][CH:5]=[CH:4][CH:3]=1",
-            True,
-            "O=[N+]([O-])c1ccc(Oc2ccc(C(F)(F)F)cc2Cl)cc1SCc1ccccc1",
-        ],
-        ["P([O-])(O)O", False, "[O-]P(O)O"],
-        [
-            "[CC(C)(C)[P]([Pd][P](C(C)(C)C)(C(C)(C)C)C(C)(C)C)(C(C)(C)C)C(C)(C)C]",
-            False,
-            "CC(C)(C)[P]([Pd][P](C(C)(C)C)(C(C)(C)C)C(C)(C)C)(C(C)(C)C)C(C)(C)C",
-        ],
-        [
-            "[CC(C)(C)[P]([Pd][P](C(C)(C)C)(C(C)(C)C)C(C)(C)C)(C(C)(C)C)C(C)(C)C]",
-            True,
-            "CC(C)(C)[P]([Pd][P](C(C)(C)C)(C(C)(C)C)C(C)(C)C)(C(C)(C)C)C(C)(C)C",
-        ],
-    ),
-)
-@pytest.mark.parametrize("execution_number", range(REPETITIONS))
-def test_canonicalisation(
-    execution_number: int,
-    smiles: str,
-    is_mapped: bool,
-    expected_canonical_smiles: Optional[str],
-) -> None:
-    from orderly.extract.canonicalise import get_canonicalised_smiles
-
-    canonical_smiles = get_canonicalised_smiles(smiles, is_mapped)
-
-    assert (
-        expected_canonical_smiles == canonical_smiles
-    ), f"failure for {expected_canonical_smiles=} got {canonical_smiles}"
-
-
-@pytest.mark.parametrize(
-    "trust_labelling,use_multiprocessing,name_contains_substring,inverse_substring",
-    (
-        [True, False, "uspto", True],
-        [False, True, "uspto", True],
-        [
-            False,
-            True,
-            "uspto",
-            False,
-        ],
-        [True, True, None, True],
-    ),
-)
-@pytest.mark.parametrize("execution_number", range(SLOW_REPETITIONS))
-def test_extraction_pipeline(
-    execution_number: int,
-    tmp_path: pathlib.Path,
-    trust_labelling: bool,
-    use_multiprocessing: bool,
-    name_contains_substring: Optional[str],
-    inverse_substring: bool,
-) -> None:
-    extracted_ord_data_folder = "extracted_ord_data"
-    (tmp_path / extracted_ord_data_folder).mkdir()
-    molecule_names_folder = "molecule_names"
-    (tmp_path / molecule_names_folder).mkdir()
-
-    import orderly.extract.main
-    import orderly.data.test_data
-
-    orderly.extract.main.main(
-        data_path=orderly.data.test_data.get_path_of_test_ords(),
-        ord_file_ending=".pb.gz",
-        trust_labelling=trust_labelling,
-        consider_molecule_names=True,  # TODO: add test for consider_molecule_names=False
-        output_path=tmp_path,
-        extracted_ord_data_folder=extracted_ord_data_folder,
-        solvents_path=None,
-        molecule_names_folder=molecule_names_folder,
-        merged_molecules_file="all_molecule_names.csv",
-        use_multiprocessing=use_multiprocessing,
-        name_contains_substring=name_contains_substring,
-        inverse_substring=inverse_substring,
-        overwrite=False,
-    )
-
-    import pandas as pd
-    import numpy as np
-
-    for extraction in (tmp_path / extracted_ord_data_folder).glob("*"):
-        df = pd.read_parquet(extraction)
-
-        df = df.sort_index(axis=1)
-
-        assert df is not None
-
-        check_none_order_cols = [
-            "reactant",
-            "agent",
-            "reagent",
-            "solvent",
-            "catalyst",
-            "product",  # note, if this is reordered it will be out of sync with yield
-            # "yield",  we are ok with this having nones in bad order
-        ]
-        for check_col in check_none_order_cols:
-            valid_cols = sorted(
-                [col for col in df.columns if col.startswith(check_col)]
-            )
-            tmp_df = df[valid_cols]
-
-            def check_valid_order(row: pd.Series) -> pd.Series:
-                seen_none = False
-                for idx, a in enumerate(row):
-                    current_isna = pd.isna(a) or (a == "")
-                    if seen_none:
-                        if not current_isna:
-                            raise ValueError(
-                                f"Unexpected order at {idx=} for {row.tolist()=}"
-                            )
-                    if current_isna:
-                        seen_none = True
-                return row
-
-            tmp_df.apply(check_valid_order, axis=1)
-
-        # Columns: ['rxn_str', 'reactant_000', 'reactant_001', 'reactant_002', 'reactant_003', 'agent_000', 'agent_001', 'agent_002', 'agent_003', 'agent_004', 'agent_005', 'solvent_000', 'solvent_001', 'solvent_002', 'temperature', 'rxn_time', 'product_000', 'yield_000', 'grant_date'],
-        # They're allowed to be strings or floats (depending on the col) or None
-        for col in df.columns:
-            series = df[col].replace({None: np.nan})
-            if len(series.dropna()) == 0:
-                continue
-            elif col in ["grant_date", "date_of_experiment"]:
-                assert pd.api.types.is_datetime64_ns_dtype(
-                    series
-                ), f"failure for {col=}: {series.dtype=}"
-            elif ("temperature" in col) or ("rxn_time" in col) or ("yield" in col):
-                assert pd.api.types.is_float_dtype(
-                    series
-                ), f"failure for {col=} {series.dtype=}"
-            elif "is_mapped" in col:
-                assert pd.api.types.is_bool_dtype(
-                    series
-                ), f"failure for {col=} {series.dtype=}"
-            else:
-                assert pd.api.types.is_object_dtype(
-                    series
-                ), f"failure for {col=} {series.dtype=}"
-
-
-@pytest.mark.parametrize(
-    "use_multiprocessing,name_contains_substring,inverse_substring,file_to_extract,file_to_compare_against",
-    (
-        [
-            True,
-            "uspto",
-            False,
-            "0c61835e3a0b4986aabf2b61b708e322.pb.gz",
-            "uspto-grants-1995_11.parquet",
-        ],
-        [
-            True,
-            "uspto",
-            False,
-            "0c61835e3a0b4986aabf2b61b708e322.pb.gz",
-            "uspto-grants-1995_11.parquet",
-        ],
-    ),
-)
-@pytest.mark.parametrize("execution_number", range(SLOW_REPETITIONS))
-@pytest.mark.parametrize("trust_labelling", [False, True])
-def test_extraction_pipeline_exact_output(
-    execution_number: int,
-    tmp_path: pathlib.Path,
-    trust_labelling: bool,
-    use_multiprocessing: bool,
-    name_contains_substring: Optional[str],
-    inverse_substring: bool,
-    file_to_extract: str,
-    file_to_compare_against: str,
-) -> None:
-    extracted_ord_data_folder = "extracted_ord_data"
-    (tmp_path / extracted_ord_data_folder).mkdir()
-    molecule_names_folder = "molecule_names"
-    (tmp_path / molecule_names_folder).mkdir()
-
-    import orderly.extract.main
-    import orderly.data.test_data
-
-    orderly.extract.main.main(
-        data_path=orderly.data.test_data.get_path_of_test_ords(),
-        ord_file_ending=file_to_extract,
-        trust_labelling=trust_labelling,
-        consider_molecule_names=False,  # TODO: add test for consider_molecule_names=False
-        output_path=tmp_path,
-        extracted_ord_data_folder=extracted_ord_data_folder,
-        solvents_path=None,
-        molecule_names_folder=molecule_names_folder,
-        merged_molecules_file="all_molecule_names.csv",
-        use_multiprocessing=use_multiprocessing,
-        name_contains_substring=name_contains_substring,
-        inverse_substring=inverse_substring,
-        overwrite=False,
-    )
-
-    import pandas as pd
-    import numpy as np
-
-    compare_against_df = pd.read_parquet(
-        orderly.data.test_data.get_path_of_test_extracted_ords(
-            trust_labelling=trust_labelling
-        )
-        / "extracted_ords"
-        / file_to_compare_against
-    )
-    created_df = pd.read_parquet(
-        tmp_path / extracted_ord_data_folder / file_to_compare_against
-    )
-
-    pd.testing.assert_frame_equal(created_df, compare_against_df)
+from typing import List, Dict, Callable, Set, Optional
+import pytest
+import pathlib
+
+from ord_schema.proto import reaction_pb2 as ord_reaction_pb2
+
+from orderly.types import YIELD, MANUAL_REPLACEMENTS_DICT
+
+REPETITIONS = 1
+SLOW_REPETITIONS = 1
+
+
+def test_hello_world() -> None:
+    assert True
+
+
+def get_rxn_func() -> Callable[[str, int], ord_reaction_pb2.Reaction]:
+    from ord_schema.proto import reaction_pb2 as ord_reaction_pb2
+
+    def get_rxn(
+        file_name: str,
+        rxn_idx: int,
+    ) -> ord_reaction_pb2.Reaction:
+        import orderly.extract.extractor
+        import orderly.data.test_data
+        import orderly.extract.main
+
+        _file = orderly.extract.main.get_file_names(
+            directory=orderly.data.test_data.get_path_of_test_ords(),
+            file_ending=f"{file_name}.pb.gz",
+        )
+        assert len(_file) == 1
+        file = pathlib.Path(_file[0])
+
+        dataset = orderly.extract.extractor.OrdExtractor.load_data(file)
+        rxn = dataset.reactions[rxn_idx]
+        return rxn
+
+    return get_rxn
+
+
+@pytest.mark.parametrize(
+    "file_name,rxn_idx,expected_labelled_reactants,expected_labelled_reagents,expected_labelled_solvents,expected_labelled_catalysts,expected_labelled_products_from_input,expected_ice_present,expected_non_smiles_names_list_additions",
+    (
+        [
+            "ord_dataset-00005539a1e04c809a9a78647bea649c",
+            0,
+            ["CC(C)N1CCNCC1", "CCOC(=O)c1cnc2cc(OCC)c(Br)cc2c1Nc1ccc(F)cc1F"],
+            ["O=C([O-])[O-]", "[Cs+]", "[Cs+]"],
+            [],
+            [
+                "c1ccc(P(c2ccccc2)c2ccc3ccccc3c2-c2c(P(c3ccccc3)c3ccccc3)ccc3ccccc23)cc1",
+                "O=C(/C=C/c1ccccc1)/C=C/c1ccccc1",
+                "O=C(/C=C/c1ccccc1)/C=C/c1ccccc1",
+                "O=C(/C=C/c1ccccc1)/C=C/c1ccccc1",
+                "[Pd]",
+                "[Pd]",
+            ],
+            [],
+            False,
+            [],
+        ],
+        [
+            "ord_dataset-0b70410902ae4139bd5d334881938f69",
+            0,
+            [
+                "SCc1ccccc1",
+                "[H-]",
+                "[Na+]",
+                "O=[N+]([O-])c1ccc(Oc2ccc(C(F)(F)F)cc2Cl)cc1[N+](=O)[O-]",
+            ],
+            [],
+            ["C1CCOC1", "C1CCOC1"],
+            [],
+            [],
+            False,
+            [],
+        ],
+        [
+            "ord_dataset-0bb2e99daa66408fb8dbd6a0781d241c",
+            0,
+            [
+                "[Na+]",
+                "[Na+]",
+                "[Na+]",
+                "[Na+]",
+                "[Na+]",
+                "[Na+]",
+                "[Na+]",
+                "[Na+]",
+                "[Na+]",
+                "[Na+]",
+                "[Na+]",
+                "[Na+]",
+                "[O-]B([O-])[O-]",
+                "[O-]B([O-])[O-]",
+                "[O-]B([O-])[O-]",
+                "[O-]B([O-])[O-]",
+                "35(Na2O)",
+            ],
+            [],
+            ["O"],
+            [],
+            [],
+            False,
+            ["35(Na2O)"],
+        ],
+        [
+            "ord_dataset-0bf72e95d80743729fdbb8b57a4bc0c6",
+            0,
+            ["CC1(C)C2CCC(=O)C1C2", "C1CCNC1", "Cc1ccc(S(=O)(=O)O)cc1", "O"],
+            [],
+            ["c1ccccc1"],
+            [],
+            [],
+            False,
+            [],
+        ],
+        [
+            "ord_dataset-a0eff6fe4b4143f284f0fc5ac503acad",
+            38,
+            [
+                "BrBr",
+                "CC1CC(C)(C)CC(C#N)(NNC(C)(C)C)C1",
+                "4-t-butylhydrazo-4-cyano-2,6-dimethylheptane",
+            ],
+            [],
+            [],
+            [],
+            [],
+            False,
+            ["4-t-butylhydrazo-4-cyano-2,6-dimethylheptane"],
+        ],
+    ),
+)
+@pytest.mark.parametrize("execution_number", range(REPETITIONS))
+def test_rxn_input_extractor(
+    execution_number: int,
+    file_name: str,
+    rxn_idx: int,
+    expected_labelled_reactants: List[str],
+    expected_labelled_reagents: List[str],
+    expected_labelled_solvents: List[str],
+    expected_labelled_catalysts: List[str],
+    expected_labelled_products_from_input: List[str],
+    expected_ice_present: bool,
+    expected_non_smiles_names_list_additions: List[str],
+) -> None:
+    rxn = get_rxn_func()(file_name, rxn_idx)
+
+    expected_labelled_reactants = sorted(expected_labelled_reactants)
+    expected_labelled_reagents = sorted(expected_labelled_reagents)
+    expected_labelled_solvents = sorted(expected_labelled_solvents)
+    expected_labelled_catalysts = sorted(expected_labelled_catalysts)
+    expected_labelled_products_from_input = sorted(
+        expected_labelled_products_from_input
+    )
+
+    import orderly.extract.extractor
+
+    (
+        labelled_reactants,
+        labelled_reagents,
+        labelled_solvents,
+        labelled_catalysts,
+        labelled_products_from_input,  # Daniel: I'm not sure what to do with this, it doesn't make sense for people to have put a product as an input, so this list should be empty anyway
+        ice_present,
+        non_smiles_names_list_additions,
+    ) = orderly.extract.extractor.OrdExtractor.rxn_input_extractor(
+        rxn, consider_molecule_names=True
+    )  # TODO: Add tests for when consider_molecule_names=False
+
+    assert (
+        expected_labelled_reactants == labelled_reactants
+    ), f"failure for {sorted(expected_labelled_reactants)=}, got {labelled_reactants}"  # TODO unsure why we have random ordering on ubuntu
+    assert (
+        expected_labelled_reagents == labelled_reagents
+    ), f"failure for {expected_labelled_reagents=}, got {labelled_reagents}"
+    assert (
+        expected_labelled_solvents == labelled_solvents
+    ), f"failure for {expected_labelled_solvents=}, got {labelled_solvents}"
+    assert (
+        expected_labelled_catalysts == labelled_catalysts
+    ), f"failure for {expected_labelled_catalysts=}, got {labelled_catalysts}"
+    assert (
+        expected_labelled_products_from_input == labelled_products_from_input
+    ), f"failure for {expected_labelled_products_from_input=}, got {labelled_products_from_input}"
+    assert (
+        expected_ice_present == ice_present
+    ), f"failure for {expected_ice_present=}, got {ice_present}"
+    assert (
+        expected_non_smiles_names_list_additions == non_smiles_names_list_additions
+    ), f"failure for {expected_non_smiles_names_list_additions=}, got {non_smiles_names_list_additions}"
+
+
+@pytest.mark.parametrize(
+    "file_name,rxn_idx,expected_labelled_products,expected_yields,expected_non_smiles_names_list_additions",
+    (
+        [
+            "ord_dataset-00005539a1e04c809a9a78647bea649c",
+            0,
+            ["CCOC(=O)c1cnc2cc(OCC)c(N3CCN(C(C)C)CC3)cc2c1Nc1ccc(F)cc1F"],
+            [65.39],
+            [],
+        ],
+        [
+            "ord_dataset-0b70410902ae4139bd5d334881938f69",
+            0,
+            ["O=[N+]([O-])c1ccc(Oc2ccc(C(F)(F)F)cc2Cl)cc1SCc1ccccc1"],
+            [None],
+            [],
+        ],
+        [
+            "ord_dataset-0bb2e99daa66408fb8dbd6a0781d241c",
+            0,
+            ["[O-]B1OB2OB([O-])OB(O1)O2", "[Na+]", "[Na+]"],
+            [None, None, None],
+            [],
+        ],
+        [
+            "ord_dataset-0bf72e95d80743729fdbb8b57a4bc0c6",
+            0,
+            ["CC1(C)C2CC=C(N3CCCC3)C1C2"],
+            [95.0],
+            [],
+        ],
+    ),
+)
+@pytest.mark.parametrize("execution_number", range(REPETITIONS))
+def test_rxn_outcomes_extractor(
+    execution_number: int,
+    file_name: str,
+    rxn_idx: int,
+    expected_labelled_products: List[str],
+    expected_yields: List[Optional[float]],
+    expected_non_smiles_names_list_additions: List[str],
+) -> None:
+    rxn = get_rxn_func()(file_name, rxn_idx)
+
+    import orderly.extract.extractor
+
+    (
+        labelled_products,
+        yields,
+        non_smiles_names_list_additions,
+    ) = orderly.extract.extractor.OrdExtractor.rxn_outcomes_extractor(
+        rxn, consider_molecule_names=True
+    )  # TODO: Add tests for when consider_molecule_names=False
+
+    assert expected_yields == yields, f"failure for {expected_yields=} got {yields}"
+    assert (
+        expected_labelled_products == labelled_products
+    ), f"failure for {expected_labelled_products=} got {labelled_products}"
+    assert (
+        expected_non_smiles_names_list_additions == non_smiles_names_list_additions
+    ), f"failure for {expected_non_smiles_names_list_additions=} got {non_smiles_names_list_additions}"
+
+
+@pytest.mark.parametrize(
+    "file_name,rxn_idx,expected_rxn_str,expected_is_mapped",
+    (
+        ["ord_dataset-00005539a1e04c809a9a78647bea649c", 0, None, None],
+        [
+            "ord_dataset-0b70410902ae4139bd5d334881938f69",
+            0,
+            "[CH2:1]([SH:8])[C:2]1[CH:7]=[CH:6][CH:5]=[CH:4][CH:3]=1.[H-].[Na+].[Cl:11][C:12]1[CH:30]=[C:29]([C:31]([F:34])([F:33])[F:32])[CH:28]=[CH:27][C:13]=1[O:14][C:15]1[CH:20]=[CH:19][C:18]([N+:21]([O-:23])=[O:22])=[C:17]([N+]([O-])=O)[CH:16]=1>O1CCCC1>[CH2:1]([S:8][C:17]1[CH:16]=[C:15]([O:14][C:13]2[CH:27]=[CH:28][C:29]([C:31]([F:34])([F:32])[F:33])=[CH:30][C:12]=2[Cl:11])[CH:20]=[CH:19][C:18]=1[N+:21]([O-:23])=[O:22])[C:2]1[CH:7]=[CH:6][CH:5]=[CH:4][CH:3]=1",
+            True,
+        ],
+        [
+            "ord_dataset-0bb2e99daa66408fb8dbd6a0781d241c",
+            0,
+            "[B:1]([O-:4])([O-:3])[O-:2].[B:5]([O-:8])([O-:7])[O-:6].[B:9]([O-:12])([O-])[O-].[B:13]([O-])([O-])[O-].[Na+:17].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+]>O>[B:1]1([O-:4])[O:3][B:13]2[O:12][B:9]([O:6][B:5]([O-:8])[O:7]2)[O:2]1.[Na+:17].[Na+:17]",
+            True,
+        ],
+        [
+            "ord_dataset-0bf72e95d80743729fdbb8b57a4bc0c6",
+            0,
+            "[CH3:1][C:2]1([CH3:10])[CH:8]2[CH2:9][CH:3]1[CH2:4][CH2:5][C:6]2=O.[NH:11]1[CH2:15][CH2:14][CH2:13][CH2:12]1.C1(C)C=CC(S(O)(=O)=O)=CC=1.O>C1C=CC=CC=1>[CH3:1][C:2]1([CH3:10])[CH:8]2[CH2:9][CH:3]1[CH2:4][CH:5]=[C:6]2[N:11]1[CH2:15][CH2:14][CH2:13][CH2:12]1",
+            True,
+        ],
+    ),
+)
+@pytest.mark.parametrize("execution_number", range(REPETITIONS))
+def test_rxn_string_and_is_mapped(
+    execution_number: int,
+    file_name: str,
+    rxn_idx: int,
+    expected_rxn_str: Optional[str],
+    expected_is_mapped: Optional[bool],
+) -> None:
+    rxn = get_rxn_func()(file_name, rxn_idx)
+
+    import orderly.extract.extractor
+
+    rxn_str_output = (
+        orderly.extract.extractor.OrdExtractor.get_rxn_string_and_is_mapped(rxn)
+    )
+    if rxn_str_output is None:
+        rxn_str, is_mapped = None, None
+    else:
+        rxn_str, is_mapped = rxn_str_output
+
+    assert expected_rxn_str == rxn_str, f"failure for {expected_rxn_str=} got {rxn_str}"
+    assert (
+        expected_is_mapped == is_mapped
+    ), f"failure for {expected_is_mapped=} got {is_mapped}"
+
+
+@pytest.mark.parametrize(
+    "file_name,rxn_idx,rxn_overwrite,expected_rxn_str_reactants,expected_rxn_str_agents,expected_rxn_str_products,expected_rxn_str,expected_non_smiles_names_list_additions,expected_none",
+    (
+        [
+            "ord_dataset-00005539a1e04c809a9a78647bea649c",
+            0,
+            None,
+            None,
+            None,
+            None,
+            None,
+            None,
+            True,
+        ],
+        [
+            "ord_dataset-0b70410902ae4139bd5d334881938f69",
+            0,
+            None,
+            [
+                "O=[N+]([O-])c1ccc(Oc2ccc(C(F)(F)F)cc2Cl)cc1[N+](=O)[O-]",
+                "SCc1ccccc1",
+            ],
+            [
+                "C1CCOC1",
+                "[H-]",
+                "[Na+]",
+            ],
+            ["O=[N+]([O-])c1ccc(Oc2ccc(C(F)(F)F)cc2Cl)cc1SCc1ccccc1"],
+            "[CH2:1]([SH:8])[C:2]1[CH:7]=[CH:6][CH:5]=[CH:4][CH:3]=1.[H-].[Na+].[Cl:11][C:12]1[CH:30]=[C:29]([C:31]([F:34])([F:33])[F:32])[CH:28]=[CH:27][C:13]=1[O:14][C:15]1[CH:20]=[CH:19][C:18]([N+:21]([O-:23])=[O:22])=[C:17]([N+]([O-])=O)[CH:16]=1>O1CCCC1>[CH2:1]([S:8][C:17]1[CH:16]=[C:15]([O:14][C:13]2[CH:27]=[CH:28][C:29]([C:31]([F:34])([F:32])[F:33])=[CH:30][C:12]=2[Cl:11])[CH:20]=[CH:19][C:18]=1[N+:21]([O-:23])=[O:22])[C:2]1[CH:7]=[CH:6][CH:5]=[CH:4][CH:3]=1",
+            [],
+            False,
+        ],
+        [
+            "ord_dataset-0bb2e99daa66408fb8dbd6a0781d241c",
+            0,
+            None,
+            [
+                "[O-]B([O-])[O-]",
+            ],
+            [
+                "O",
+                "[Na+]",
+            ],
+            [
+                "[O-]B1OB2OB([O-])OB(O1)O2",
+            ],
+            "[B:1]([O-:4])([O-:3])[O-:2].[B:5]([O-:8])([O-:7])[O-:6].[B:9]([O-:12])([O-])[O-].[B:13]([O-])([O-])[O-].[Na+:17].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+]>O>[B:1]1([O-:4])[O:3][B:13]2[O:12][B:9]([O:6][B:5]([O-:8])[O:7]2)[O:2]1.[Na+:17].[Na+:17]",
+            [],
+            False,
+        ],
+        [
+            "ord_dataset-0bf72e95d80743729fdbb8b57a4bc0c6",
+            0,
+            None,
+            [
+                "C1CCNC1",
+                "CC1(C)C2CCC(=O)C1C2",
+            ],
+            ["Cc1ccc(S(=O)(=O)O)cc1", "O", "c1ccccc1"],
+            ["CC1(C)C2CC=C(N3CCCC3)C1C2"],
+            "[CH3:1][C:2]1([CH3:10])[CH:8]2[CH2:9][CH:3]1[CH2:4][CH2:5][C:6]2=O.[NH:11]1[CH2:15][CH2:14][CH2:13][CH2:12]1.C1(C)C=CC(S(O)(=O)=O)=CC=1.O>C1C=CC=CC=1>[CH3:1][C:2]1([CH3:10])[CH:8]2[CH2:9][CH:3]1[CH2:4][CH:5]=[C:6]2[N:11]1[CH2:15][CH2:14][CH2:13][CH2:12]1",
+            [],
+            False,
+        ],
+        # test case where the products list starts non-empty but ends empty
+        # I think this is a crystalisation/protonation/stabilisation reaction
+        [
+            "ord_dataset-a0eff6fe4b4143f284f0fc5ac503acad",
+            10,
+            None,
+            [],
+            [
+                "Cc1cc2c([N+](=O)[O-])cccc2cn1",
+                "Cl",
+                "I",
+                "O=[N+]([O-])c1ccc(Cl)c2ccncc12",
+            ],
+            [],
+            "CC1N=CC2C(C=1)=C([N+]([O-])=O)C=CC=2.[Cl:15][C:16]1[CH:25]=[CH:24][C:23]([N+:26]([O-:28])=[O:27])=[C:22]2[C:17]=1[CH:18]=[CH:19][N:20]=[CH:21]2.Cl.CC1N=CC2C(C=1)=C([N+]([O-])=O)C=CC=2.[IH:44]>>[IH:44].[Cl:15][C:16]1[CH:25]=[CH:24][C:23]([N+:26]([O-:28])=[O:27])=[C:22]2[C:17]=1[CH:18]=[CH:19][N:20]=[CH:21]2",
+            [],
+            False,
+        ],
+        [
+            "ord_dataset-a0eff6fe4b4143f284f0fc5ac503acad",
+            1932,
+            None,
+            ["C=C(C)Br", "C=C1CC(=O)CCC2=C(C)CCC12"],
+            [
+                "C1CCOC1",
+                "II",
+                "[Mg]",
+            ],
+            ["C=C1CC(O)(C(=C)C)CCC2=C(C)CCC12"],
+            "[Mg].II.Br[C:5]([CH3:7])=[CH2:6].[CH3:8][C:9]1[CH2:10][CH2:11][CH:12]2[C:18]=1[CH2:17][CH2:16][C:15](=[O:19])[CH2:14][C:13]2=[CH2:20]>O1CCCC1>[OH:19][C:15]1([C:5]([CH3:7])=[CH2:6])[CH2:16][CH2:17][C:18]2[CH:12]([CH2:11][CH2:10][C:9]=2[CH3:8])[C:13](=[CH2:20])[CH2:14]1",
+            [],
+            False,
+        ],
+        [
+            "ord_dataset-85c00026681b46f89ef8634d2b8618c3",
+            3948,
+            None,
+            [
+                "O=S(=O)(O)O",
+                "[Co]",
+            ],
+            [
+                "CCCCCC=N",
+                "O=S(=O)([O-])[O-]",
+                "[Co+3]",
+                "[NH4+]",
+            ],
+            [],
+            "[Co:1].[S:2]([OH:6])([OH:5])(=[O:4])=[O:3].[CH:7](=[NH:13])[CH2:8][CH2:9][CH2:10][CH2:11][CH3:12].[S:14]([O-:18])([O-:17])(=[O:16])=[O:15].[NH4+].[NH4+].[Co+3]>>[S:2]([O-:6])([O-:5])(=[O:4])=[O:3].[CH:7](=[NH:13])[CH2:8][CH2:9][CH2:10][CH2:11][CH3:12].[Co+3:1].[S:14]([O-:18])([O-:17])(=[O:16])=[O:15].[S:2]([O-:6])([O-:5])(=[O:4])=[O:3].[Co+3:1]",
+            [],
+            False,
+        ],
+        # Test case where reaction with only 1 >
+        pytest.param(
+            "ord_dataset-0bf72e95d80743729fdbb8b57a4bc0c6",
+            0,
+            "CC.C>CCC",
+            ["CC", "C"],
+            [],
+            ["CCC"],
+            "CC.C>CCC",
+            [],
+            True,
+        ),
+        # There's no point in trying to test whether the the rxn.identifiers[0].value = None because the schema doesn't allow that overwrite to happen!
+    ),
+)
+@pytest.mark.parametrize("execution_number", range(REPETITIONS))
+def test_extract_info_from_rxn_str(
+    execution_number: int,
+    file_name: str,
+    rxn_idx: int,
+    rxn_overwrite: Optional[bool],
+    expected_rxn_str_reactants: Optional[List[str]],
+    expected_rxn_str_agents: Optional[List[str]],
+    expected_rxn_str_products: Optional[List[str]],
+    expected_rxn_str: Optional[str],
+    expected_non_smiles_names_list_additions: Optional[List[str]],
+    expected_none: bool,
+) -> None:
+    rxn = get_rxn_func()(file_name, rxn_idx)
+
+    if rxn_overwrite is not None:
+        rxn.identifiers[0].value = rxn_overwrite
+
+    import orderly.extract.extractor
+
+    _rxn_info = orderly.extract.extractor.OrdExtractor.get_rxn_string_and_is_mapped(rxn)
+    if _rxn_info is None:
+        return None
+    rxn_str, is_mapped = _rxn_info
+
+    rxn_info = orderly.extract.extractor.OrdExtractor.extract_info_from_rxn_str(
+        rxn_str, is_mapped
+    )
+    if expected_none:
+        assert rxn_info is None, f"expected a none but got {rxn_info=}"
+        return
+    else:
+        assert rxn_info is not None, f"did not expect a none but got one {rxn_info=}"
+    (
+        rxn_str_reactants,
+        rxn_str_agents,
+        rxn_str_products,
+        rxn_str,
+        non_smiles_names_list_additions,
+    ) = rxn_info
+
+    assert expected_rxn_str_reactants is not None
+    assert expected_rxn_str_agents is not None
+    assert expected_rxn_str_products is not None
+    assert expected_rxn_str is not None
+    assert expected_non_smiles_names_list_additions is not None
+
+    assert expected_rxn_str_reactants == rxn_str_reactants
+    assert expected_rxn_str_agents == rxn_str_agents
+    assert expected_rxn_str_products == rxn_str_products
+    assert expected_rxn_str == rxn_str
+    assert expected_non_smiles_names_list_additions == non_smiles_names_list_additions
+
+
+@pytest.mark.parametrize(
+    "file_name,rxn_idx,expected_temperature",
+    (
+        [
+            "ord_dataset-00005539a1e04c809a9a78647bea649c",
+            0,
+            110.0,
+        ],
+        ["ord_dataset-0b70410902ae4139bd5d334881938f69", 0, None],
+        ["ord_dataset-0bb2e99daa66408fb8dbd6a0781d241c", 0, 1100.0],
+        ["ord_dataset-0bf72e95d80743729fdbb8b57a4bc0c6", 0, None],
+    ),
+)
+@pytest.mark.parametrize("execution_number", range(REPETITIONS))
+def test_temperature_extractor(
+    execution_number: int,
+    file_name: str,
+    rxn_idx: int,
+    expected_temperature: Optional[float],
+) -> None:
+    rxn = get_rxn_func()(file_name, rxn_idx)
+
+    import orderly.extract.extractor
+
+    temperature = orderly.extract.extractor.OrdExtractor.temperature_extractor(rxn)
+
+    assert (
+        expected_temperature == temperature
+    ), f"failure for {expected_temperature=} got {temperature}"
+    if temperature is not None:
+        assert isinstance(
+            temperature, float
+        ), f"expected a float but got {temperature=}"
+
+
+@pytest.mark.parametrize(
+    "file_name,rxn_idx,expected_rxn_time",
+    (
+        ["ord_dataset-00005539a1e04c809a9a78647bea649c", 0, None],
+        ["ord_dataset-0b70410902ae4139bd5d334881938f69", 0, None],
+        ["ord_dataset-0bb2e99daa66408fb8dbd6a0781d241c", 0, 0.17],
+        ["ord_dataset-0bf72e95d80743729fdbb8b57a4bc0c6", 0, None],
+    ),
+)
+@pytest.mark.parametrize("execution_number", range(REPETITIONS))
+def test_time_extractor(
+    execution_number: int,
+    file_name: str,
+    rxn_idx: int,
+    expected_rxn_time: Optional[float],
+) -> None:
+    rxn = get_rxn_func()(file_name, rxn_idx)
+
+    import orderly.extract.extractor
+
+    rxn_time = orderly.extract.extractor.OrdExtractor.rxn_time_extractor(rxn)
+
+    assert (
+        expected_rxn_time == rxn_time
+    ), f"failure for {expected_rxn_time=} got {rxn_time=}"
+
+    if rxn_time is not None:
+        assert isinstance(rxn_time, float), f"expected a float but got {rxn_time=}"
+
+
+@pytest.mark.parametrize(
+    "rxn_str_agents,labelled_catalysts,labelled_solvents,labelled_reagents,solvents_set,expected_agents,expected_solvents",
+    (
+        [
+            None,
+            [
+                "c1ccc(P(c2ccccc2)c2ccc3ccccc3c2-c2c(P(c3ccccc3)c3ccccc3)ccc3ccccc23)cc1",
+                "O=C(/C=C/c1ccccc1)/C=C/c1ccccc1",
+                "[Pd]",
+            ],
+            [],
+            ["O=C([O-])[O-]", "[Cs+]"],
+            None,
+            [
+                "[Pd]",
+                "O=C(/C=C/c1ccccc1)/C=C/c1ccccc1",
+                "O=C([O-])[O-]",
+                "[Cs+]",
+                "c1ccc(P(c2ccccc2)c2ccc3ccccc3c2-c2c(P(c3ccccc3)c3ccccc3)ccc3ccccc23)cc1",
+            ],
+            [],
+        ],
+        [["C1CCOC1"], None, ["C1CCOC1", "C1CCOC1"], None, None, [], ["C1CCOC1"]],
+        [["O"], [], ["O"], [], None, [], ["O"]],
+        [
+            ["c1ccccc1", "Cc1ccc(S(=O)(=O)O)cc1", "O"],
+            [],
+            ["c1ccccc1"],
+            [],
+            None,
+            ["Cc1ccc(S(=O)(=O)O)cc1"],
+            ["O", "c1ccccc1"],
+        ],
+        # Made up test cases:
+        [
+            [
+                "c1ccccc1",
+                "Cc1ccc(S(=O)(=O)O)cc1",
+                "O",
+                None,
+            ],
+            ["[Pd]"],
+            ["O", "CCO"],
+            ["O=C([O-])[O-]"],
+            None,
+            ["[Pd]", "Cc1ccc(S(=O)(=O)O)cc1", "O=C([O-])[O-]"],
+            ["CCO", "O", "c1ccccc1"],
+        ],
+        pytest.param(
+            ["c1ccccc1", "Cc1ccc(S(=O)(=O)O)cc1", "O"],
+            ["[Pd]"],
+            ["O", "CCO"],
+            ["O=C([O-])[O-]"],
+            None,
+            ["c1ccccc1", "Cc1ccc(S(=O)(=O)O)cc1", "O"],
+            ["O", "CCO"],
+            marks=pytest.mark.xfail,
+        ),
+        pytest.param(
+            ["c1ccccc1", "Cc1ccc(S(=O)(=O)O)cc1", "O"],
+            ["[Pd]"],
+            ["O", "CCO"],
+            ["O=C([O-])[O-]"],
+            None,
+            ["[Pd]", "Cc1ccc(S(=O)(=O)O)cc1", "O=C([O-])[O-]", "O", "CCO", "c1ccccc1"],
+            [],
+            marks=pytest.mark.xfail,
+        ),
+        pytest.param(
+            ["c1ccccc1", "Cc1ccc(S(=O)(=O)O)cc1", "O"],
+            ["[Pd]"],
+            ["O", "CCO"],
+            ["O=C([O-])[O-]"],
+            None,
+            ["[Pd]", "Cc1ccc(S(=O)(=O)O)cc1", "O=C([O-])[O-]"],
+            ["O", "O", "CCO", "c1ccccc1"],
+            marks=pytest.mark.xfail,
+        ),
+    ),
+)
+@pytest.mark.parametrize("execution_number", range(REPETITIONS))
+def test_merge_to_agents(
+    execution_number: int,
+    rxn_str_agents: Optional[List[str]],
+    labelled_catalysts: Optional[List[str]],
+    labelled_solvents: Optional[List[str]],
+    labelled_reagents: Optional[List[str]],
+    solvents_set: Set[str],
+    expected_agents: Optional[List[str]],
+    expected_solvents: Optional[List[str]],
+) -> None:
+    import orderly.extract.extractor
+    import orderly.extract.defaults
+
+    if solvents_set is None:
+        solvents_set = orderly.extract.defaults.get_solvents_set()
+
+    agents, solvents = orderly.extract.extractor.OrdExtractor.merge_to_agents(
+        rxn_str_agents,
+        labelled_catalysts,
+        labelled_solvents,
+        labelled_reagents,
+        solvents_set,
+    )
+
+    assert expected_agents == agents, f"failure for {expected_agents=} got {agents}"
+    assert (
+        expected_solvents == solvents
+    ), f"failure for {expected_solvents=} got {solvents}"
+
+
+@pytest.mark.parametrize(
+    "rxn_str_products,labelled_products,input_yields,expected_products,expected_yields",
+    (
+        [
+            [],
+            ["CCOC(=O)c1cnc2cc(OCC)c(N3CCN(C(C)C)CC3)cc2c1Nc1ccc(F)cc1F"],
+            [65.39],
+            [],
+            [],
+        ],
+        [
+            ["O=[N+]([O-])c1ccc(Oc2ccc(C(F)(F)F)cc2Cl)cc1SCc1ccccc1"],
+            ["O=[N+]([O-])c1ccc(Oc2ccc(C(F)(F)F)cc2Cl)cc1SCc1ccccc1"],
+            [None],
+            ["O=[N+]([O-])c1ccc(Oc2ccc(C(F)(F)F)cc2Cl)cc1SCc1ccccc1"],
+            [None],
+        ],
+        [
+            ["[Na+]", "[Na+]", "[O-]B1OB2OB([O-])OB(O1)O2"],
+            ["[Na+]", "[Na+]", "[O-]B1OB2OB([O-])OB(O1)O2"],
+            [None, None, None],
+            ["[Na+]", "[Na+]", "[O-]B1OB2OB([O-])OB(O1)O2"],
+            [None, None, None],
+        ],
+        pytest.param(
+            ["[Na+]", "[Na+]", "[O-]B1OB2OB([O-])OB(O1)O2"],
+            ["[Na+]", "[Na+]", "[O-]B1OB2OB([O-])OB(O1)O2"],
+            [None],
+            ["[Na+]", "[Na+]", "[O-]B1OB2OB([O-])OB(O1)O2"],
+            [None],
+            marks=pytest.mark.xfail(reason="IndexError: list index out of range"),
+        ),
+        [
+            ["O=[N+]([O-])c1ccc(Oc2ccc(C(F)(F)F)cc2Cl)cc1SCc1ccccc1"],
+            ["[Na+]", "[Na+]", "[O-]B1OB2OB([O-])OB(O1)O2"],
+            [None, None, None],
+            ["O=[N+]([O-])c1ccc(Oc2ccc(C(F)(F)F)cc2Cl)cc1SCc1ccccc1"],
+            [None],
+        ],
+        [
+            ["CC1(C)C2CC=C(N3CCCC3)C1C2"],
+            ["CC1(C)C2CC=C(N3CCCC3)C1C2"],
+            [95.0],
+            ["CC1(C)C2CC=C(N3CCCC3)C1C2"],
+            [95.0],
+        ],
+    ),
+)
+@pytest.mark.parametrize("execution_number", range(REPETITIONS))
+def test_match_yield_with_product(
+    execution_number: int,
+    rxn_str_products: List[str],
+    labelled_products: List[str],
+    input_yields: List[Optional[YIELD]],
+    expected_products: List[str],
+    expected_yields: List[Optional[YIELD]],
+) -> None:
+    import orderly.extract.extractor
+
+    products, yields = orderly.extract.extractor.OrdExtractor.match_yield_with_product(
+        rxn_str_products, labelled_products, input_yields
+    )
+
+    assert (
+        expected_products == products
+    ), f"failure for {expected_products=} got {products=}"
+    assert expected_yields == yields, f"failure for {expected_yields=} got {yields=}"
+
+
+@pytest.mark.parametrize(
+    "file_name,rxn_idx,manual_replacements_dict,trust_labelling,expected_reactants, expected_agents, expected_reagents,expected_solvents,expected_catalysts,expected_products,expected_yields,expected_temperature,expected_rxn_time,expected_rxn_str, expected_procedure_details, expected_date_of_experiment, expected_names_list, expected_is_mapped",
+    (
+        [
+            "ord_dataset-00005539a1e04c809a9a78647bea649c",
+            0,
+            {},
+            False,
+            ["CC(C)N1CCNCC1", "CCOC(=O)c1cnc2cc(OCC)c(Br)cc2c1Nc1ccc(F)cc1F"],
+            [
+                "[Pd]",
+                "O=C(/C=C/c1ccccc1)/C=C/c1ccccc1",
+                "O=C([O-])[O-]",
+                "[Cs+]",
+                "c1ccc(P(c2ccccc2)c2ccc3ccccc3c2-c2c(P(c3ccccc3)c3ccccc3)ccc3ccccc23)cc1",
+            ],
+            [],
+            [],
+            [],
+            ["CCOC(=O)c1cnc2cc(OCC)c(N3CCN(C(C)C)CC3)cc2c1Nc1ccc(F)cc1F"],
+            [65.39],
+            110.0,
+            None,
+            None,
+            "To a solution of ethyl 6-bromo-4-(2,4-difluorophenylamino)-7-ethoxyquinoline-3-carboxylate (400 mg, 0.89 mmol) and 1-(Isopropyl)piperazine (254 µl, 1.77 mmol) in dioxane was added cesium carbonate (722 mg, 2.22 mmol), tris(dibenzylideneacetone)dipalladium(0) (40.6 mg, 0.04 mmol) and rac-2,2'-Bis(diphenylphosphino)-1,1'-binaphthyl (55.2 mg, 0.09 mmol). Reaction vessel in oil bath set to 110 °C. 11am  After 5 hours, MS shows product (major peak 499), and SM (minor peak 453).  o/n, MS shows product peak. Reaction cooled, concentrated onto silica, and purified on ISCO. 40g column, 1:1 EA:Hex, then 100% EA.  289mg yellow solid. NMR (EN00180-62-1) supports product, but some oxidised BINAP impurity (LCMS 655).  ",
+            "07/01/2008",
+            [],
+            False,
+        ],
+        [
+            "ord_dataset-0b70410902ae4139bd5d334881938f69",
+            0,
+            {},
+            False,
+            [
+                "SCc1ccccc1",
+                "O=[N+]([O-])c1ccc(Oc2ccc(C(F)(F)F)cc2Cl)cc1[N+](=O)[O-]",
+            ],
+            ["[H-]", "[Na+]"],
+            [],
+            ["C1CCOC1"],
+            [],
+            ["O=[N+]([O-])c1ccc(Oc2ccc(C(F)(F)F)cc2Cl)cc1SCc1ccccc1"],
+            [None],
+            None,
+            None,
+            "[CH2:1]([SH:8])[C:2]1[CH:7]=[CH:6][CH:5]=[CH:4][CH:3]=1.[H-].[Na+].[Cl:11][C:12]1[CH:30]=[C:29]([C:31]([F:34])([F:33])[F:32])[CH:28]=[CH:27][C:13]=1[O:14][C:15]1[CH:20]=[CH:19][C:18]([N+:21]([O-:23])=[O:22])=[C:17]([N+]([O-])=O)[CH:16]=1>O1CCCC1>[CH2:1]([S:8][C:17]1[CH:16]=[C:15]([O:14][C:13]2[CH:27]=[CH:28][C:29]([C:31]([F:34])([F:32])[F:33])=[CH:30][C:12]=2[Cl:11])[CH:20]=[CH:19][C:18]=1[N+:21]([O-:23])=[O:22])[C:2]1[CH:7]=[CH:6][CH:5]=[CH:4][CH:3]=1",
+            "1.7 g of benzyl mercaptan was dissolved in dry tetrahydrofuran and 0.5 g of sodium hydride added with stirring under dry nitrogen. The reaction mixture was stirred under reflux for 30 minutes, and a solution of 5 g of 1A dissolved in 25 ml of dry tetrahydrofuran was added dropwise. Reaction occurred rapidly, and the product was chromatographically purified to give 2-benzylthio-4-(2-chloro-4-trifluoromethylphenoxy)nitrobenzene (1B) as a yellow oil.",
+            None,
+            [],
+            True,
+        ],
+        [
+            "ord_dataset-0bb2e99daa66408fb8dbd6a0781d241c",
+            0,
+            {},
+            False,
+            ["[O-]B([O-])[O-]"],
+            [
+                "[Na+]",
+                "35(Na2O)",
+            ],
+            [],
+            ["O"],
+            [],
+            ["[O-]B1OB2OB([O-])OB(O1)O2"],
+            [None],
+            1100.0,
+            0.17,
+            "[B:1]([O-:4])([O-:3])[O-:2].[B:5]([O-:8])([O-:7])[O-:6].[B:9]([O-:12])([O-])[O-].[B:13]([O-])([O-])[O-].[Na+:17].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+]>O>[B:1]1([O-:4])[O:3][B:13]2[O:12][B:9]([O:6][B:5]([O-:8])[O:7]2)[O:2]1.[Na+:17].[Na+:17]",
+            "Sodium tetraborate (Na2B4O7.10H2O), analyzed reagent was dried overnight at 150° C, mixed with the appropriate quantity of dopant ions and homogenized in an electric homogenizer (vibrator) during 10 minutes. The material was then transferred to a platinum crucible and heated at 1100° C for at least 30 minutes, until a clear transparent solution was obtained. The glass matrix loses water and the composition of the matrix is after the heating 35(Na2O).65(B2O3). A drop of the hot melt was allowed to fall directly onto a clean white glazed ceramic surface, into the center of a space ring of 1 mm thickness, and pressed with a second ceramic tile to produce a glass disk of 1 mm thickness and an approximate diameter of 12 mm. The glass is transparent in the ultraviolet and in the visible part of the spectrum.",
+            None,
+            ["35(Na2O)"],
+            True,
+        ],
+        [
+            "ord_dataset-0bb2e99daa66408fb8dbd6a0781d241c",
+            0,
+            {},
+            True,
+            [
+                "[Na+]",
+                "[Na+]",
+                "[Na+]",
+                "[Na+]",
+                "[Na+]",
+                "[Na+]",
+                "[Na+]",
+                "[Na+]",
+                "[Na+]",
+                "[Na+]",
+                "[Na+]",
+                "[Na+]",
+                "[O-]B([O-])[O-]",
+                "[O-]B([O-])[O-]",
+                "[O-]B([O-])[O-]",
+                "[O-]B([O-])[O-]",
+                "35(Na2O)",
+            ],
+            [],
+            [],
+            ["O"],
+            [],
+            [
+                "[O-]B1OB2OB([O-])OB(O1)O2",
+                "[Na+]",
+                "[Na+]",
+            ],
+            [None, None, None],
+            1100.0,
+            0.17,
+            "[B:1]([O-:4])([O-:3])[O-:2].[B:5]([O-:8])([O-:7])[O-:6].[B:9]([O-:12])([O-])[O-].[B:13]([O-])([O-])[O-].[Na+:17].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+].[Na+]>O>[B:1]1([O-:4])[O:3][B:13]2[O:12][B:9]([O:6][B:5]([O-:8])[O:7]2)[O:2]1.[Na+:17].[Na+:17]",
+            "Sodium tetraborate (Na2B4O7.10H2O), analyzed reagent was dried overnight at 150° C, mixed with the appropriate quantity of dopant ions and homogenized in an electric homogenizer (vibrator) during 10 minutes. The material was then transferred to a platinum crucible and heated at 1100° C for at least 30 minutes, until a clear transparent solution was obtained. The glass matrix loses water and the composition of the matrix is after the heating 35(Na2O).65(B2O3). A drop of the hot melt was allowed to fall directly onto a clean white glazed ceramic surface, into the center of a space ring of 1 mm thickness, and pressed with a second ceramic tile to produce a glass disk of 1 mm thickness and an approximate diameter of 12 mm. The glass is transparent in the ultraviolet and in the visible part of the spectrum.",
+            None,
+            ["35(Na2O)"],
+            True,
+        ],
+        [
+            "ord_dataset-0bf72e95d80743729fdbb8b57a4bc0c6",
+            0,
+            {},
+            False,
+            [
+                "CC1(C)C2CCC(=O)C1C2",
+                "C1CCNC1",
+            ],
+            [
+                "Cc1ccc(S(=O)(=O)O)cc1",
+            ],
+            [],
+            [
+                "O",
+                "c1ccccc1",
+            ],
+            [],
+            ["CC1(C)C2CC=C(N3CCCC3)C1C2"],
+            [95.0],
+            None,
+            None,
+            "[CH3:1][C:2]1([CH3:10])[CH:8]2[CH2:9][CH:3]1[CH2:4][CH2:5][C:6]2=O.[NH:11]1[CH2:15][CH2:14][CH2:13][CH2:12]1.C1(C)C=CC(S(O)(=O)=O)=CC=1.O>C1C=CC=CC=1>[CH3:1][C:2]1([CH3:10])[CH:8]2[CH2:9][CH:3]1[CH2:4][CH:5]=[C:6]2[N:11]1[CH2:15][CH2:14][CH2:13][CH2:12]1",
+            "A solution of 30 g of nopinone ([α]D20 =+39.90; c=8 in ethanol), 29 of pyrrolidine and 0.4 g of p-toluenesulfonic acid in 150 ml anhydrous benzene was heated at reflux for 40 h under nitrogen atmosphere in a vessel fitted with a water separator. After evaporation of the solvent and distillation of the residue, there were obtained 39.5 g (95% yield) of 1-(6,6-dimethylnorpin-2-en-2-yl)-pyrrolidine having b.p. 117°-118° C./10 Torr.",
+            None,
+            [],
+            True,
+        ],
+        [
+            "ord_dataset-0bf72e95d80743729fdbb8b57a4bc0c6",
+            0,
+            {},
+            True,
+            [
+                "C1CCNC1",
+                "CC1(C)C2CCC(=O)C1C2",
+                "O",
+                "Cc1ccc(S(=O)(=O)O)cc1",
+            ],
+            [],
+            [],
+            ["c1ccccc1"],
+            [],
+            ["CC1(C)C2CC=C(N3CCCC3)C1C2"],
+            [95.0],
+            None,
+            None,
+            "[CH3:1][C:2]1([CH3:10])[CH:8]2[CH2:9][CH:3]1[CH2:4][CH2:5][C:6]2=O.[NH:11]1[CH2:15][CH2:14][CH2:13][CH2:12]1.C1(C)C=CC(S(O)(=O)=O)=CC=1.O>C1C=CC=CC=1>[CH3:1][C:2]1([CH3:10])[CH:8]2[CH2:9][CH:3]1[CH2:4][CH:5]=[C:6]2[N:11]1[CH2:15][CH2:14][CH2:13][CH2:12]1",
+            "A solution of 30 g of nopinone ([α]D20 =+39.90; c=8 in ethanol), 29 of pyrrolidine and 0.4 g of p-toluenesulfonic acid in 150 ml anhydrous benzene was heated at reflux for 40 h under nitrogen atmosphere in a vessel fitted with a water separator. After evaporation of the solvent and distillation of the residue, there were obtained 39.5 g (95% yield) of 1-(6,6-dimethylnorpin-2-en-2-yl)-pyrrolidine having b.p. 117°-118° C./10 Torr.",
+            None,
+            [],
+            True,
+        ],
+        # Test: one of the input reactants = 'liquid'; trust_labelling = True
+        [
+            "ord_dataset-0b70410902ae4139bd5d334881938f69",
+            3,
+            {},
+            True,
+            ["Clc1nc(Cl)nc(Cl)n1", "N"],
+            [],
+            [],
+            ["C1CCOC1", "COCCOCCOC"],
+            [],
+            ["Nc1nc(Cl)nc(Cl)n1"],
+            [None],
+            25,
+            1.0,
+            "[N:1]1[C:8]([Cl:9])=[N:7][C:5]([Cl:6])=[N:4][C:2]=1Cl.[NH3:10]>C1COCC1.COCCOCCOC>[NH2:10][C:2]1[N:1]=[C:8]([Cl:9])[N:7]=[C:5]([Cl:6])[N:4]=1",
+            "A solution of 300 g (1.63 mol) of cyanuric chloride in 1 liter THF and 0.24 liter diglyme was cooled to 0\302\260 C. and 81.6 mL (3.36 mol) of liquid ammonia added dropwise over 90 min. keeping the temperature between 10\302\260-15\302\260. The mixture was stirred for one hour at -10\302\260 to 0\302\260 and then allowed to warm to ambient temperature over one hour. The resulting suspension was filtered, the solid washed with THF, the filtrate reduced to 1/2 its original volume, and poured over 1 liter of ice water to give a white solid which was collected, washed with water, and dried in vacuo to give 244.3 g of 2-amino-4,6-dichloro-1,3,5-triazine with m.p. 221\302\260-223.5\302\260 (dec).",
+            None,
+            ["liquid"],
+            True,
+        ],
+        # Test: one of the input reactants = 'liquid'; trust_labelling = False
+        [
+            "ord_dataset-0b70410902ae4139bd5d334881938f69",
+            3,
+            {},
+            False,
+            ["Clc1nc(Cl)nc(Cl)n1", "N"],
+            [],
+            [],
+            ["C1CCOC1", "COCCOCCOC"],
+            [],
+            ["Nc1nc(Cl)nc(Cl)n1"],
+            [None],
+            25,
+            1.0,
+            "[N:1]1[C:8]([Cl:9])=[N:7][C:5]([Cl:6])=[N:4][C:2]=1Cl.[NH3:10]>C1COCC1.COCCOCCOC>[NH2:10][C:2]1[N:1]=[C:8]([Cl:9])[N:7]=[C:5]([Cl:6])[N:4]=1",
+            "A solution of 300 g (1.63 mol) of cyanuric chloride in 1 liter THF and 0.24 liter diglyme was cooled to 0\302\260 C. and 81.6 mL (3.36 mol) of liquid ammonia added dropwise over 90 min. keeping the temperature between 10\302\260-15\302\260. The mixture was stirred for one hour at -10\302\260 to 0\302\260 and then allowed to warm to ambient temperature over one hour. The resulting suspension was filtered, the solid washed with THF, the filtrate reduced to 1/2 its original volume, and poured over 1 liter of ice water to give a white solid which was collected, washed with water, and dried in vacuo to give 244.3 g of 2-amino-4,6-dichloro-1,3,5-triazine with m.p. 221\302\260-223.5\302\260 (dec).",
+            None,
+            ["liquid"],
+            True,
+        ],
+        # synthesis of islatravir by biocatalytic cascade
+        # We put trust_labelling = False to test that the inputs are extracted instead, since I know that there's no rxn string
+        [
+            "ord_dataset-6a0bfcdf53a64c07987822162ae591e2",
+            0,
+            {},
+            False,
+            ["C#CC(O)(CO)CO"],
+            [
+                "[Cu+2]",
+                "O=S(=O)([O-])CCN1CCN(CCS(=O)(=O)[O-])CC1",
+                "O=S(=O)([O-])[O-]",
+                "[K+]",
+                "Antifoam 204",
+                "bovine catalase",
+                "evolved galactose oxidase GOase-Rd13BB",
+                "horseradish peroxidase",
+            ],
+            [],
+            ["O"],
+            [],
+            ["C#C[C@](O)(C=O)CO"],
+            [68.0],
+            25.0,
+            22.0,
+            None,
+            "",
+            None,
+            [
+                "Antifoam 204",
+                "bovine catalase",
+                "evolved galactose oxidase GOase-Rd13BB",
+                "horseradish peroxidase",
+            ],
+            False,
+        ],
+        # An example where we need the manual_replacements_dict
+        [
+            "ord_dataset-0b70410902ae4139bd5d334881938f69",
+            982,
+            {},
+            True,
+            [
+                "CCO",
+                "O",
+                "COc1ccccc1C(O)c1cccc(Br)n1",
+                "O=[Cr](=O)=O",
+            ],
+            [],
+            [],
+            ["CC(=O)O"],
+            [],
+            ["COc1ccccc1C(=O)c1cccc(Br)n1"],
+            [66.2],
+            None,
+            None,
+            "[Br:1][C:2]1[N:7]=[C:6]([CH:8]([C:10]2[CH:15]=[CH:14][CH:13]=[CH:12][C:11]=2[O:16][CH3:17])[OH:9])[CH:5]=[CH:4][CH:3]=1.C(O)C.O>C(O)(=O)C>[Br:1][C:2]1[N:7]=[C:6]([C:8](=[O:9])[C:10]2[CH:15]=[CH:14][CH:13]=[CH:12][C:11]=2[O:16][CH3:17])[CH:5]=[CH:4][CH:3]=1",
+            "By the same procedure of Ex. 22, and reacting 3.3 g 6-bromo-\316\261-(2-methoxyphenyl)-2-pyridinemethanol (obtained as in Ex. 19) in 20 ml glacial acetic acid with CrO3 (1 g in 5 ml water), there is obtained 2.17 g title product, m.p. 97\302\260-8\302\260 C. (ethanol:water); UV (ethanol):\316\273max. 278 nm, \316\265: 12,480; Br 27.67 (27.36).",
+            None,
+            ["CrO3"],
+            True,
+        ],
+        [
+            "ord_dataset-0b70410902ae4139bd5d334881938f69",
+            982,
+            {},
+            False,
+            [
+                "COc1ccccc1C(O)c1cccc(Br)n1",
+            ],
+            [
+                "O=[Cr](=O)=O",
+            ],
+            [],
+            ["CC(=O)O", "CCO", "O"],
+            [],
+            ["COc1ccccc1C(=O)c1cccc(Br)n1"],
+            [66.2],
+            None,
+            None,
+            "[Br:1][C:2]1[N:7]=[C:6]([CH:8]([C:10]2[CH:15]=[CH:14][CH:13]=[CH:12][C:11]=2[O:16][CH3:17])[OH:9])[CH:5]=[CH:4][CH:3]=1.C(O)C.O>C(O)(=O)C>[Br:1][C:2]1[N:7]=[C:6]([C:8](=[O:9])[C:10]2[CH:15]=[CH:14][CH:13]=[CH:12][C:11]=2[O:16][CH3:17])[CH:5]=[CH:4][CH:3]=1",
+            "By the same procedure of Ex. 22, and reacting 3.3 g 6-bromo-\316\261-(2-methoxyphenyl)-2-pyridinemethanol (obtained as in Ex. 19) in 20 ml glacial acetic acid with CrO3 (1 g in 5 ml water), there is obtained 2.17 g title product, m.p. 97\302\260-8\302\260 C. (ethanol:water); UV (ethanol):\316\273max. 278 nm, \316\265: 12,480; Br 27.67 (27.36).",
+            None,
+            ["CrO3"],
+            True,
+        ],
+        [
+            "ord_dataset-a0eff6fe4b4143f284f0fc5ac503acad",
+            1932,
+            {},
+            False,
+            ["C=C(C)Br", "C=C1CC(=O)CCC2=C(C)CCC12"],
+            [
+                "II",
+                "[Mg]",
+            ],
+            [],
+            [
+                "C1CCOC1",
+            ],
+            [],
+            ["C=C1CC(O)(C(=C)C)CCC2=C(C)CCC12"],
+            [76.0],
+            None,
+            0.5,
+            "[Mg].II.Br[C:5]([CH3:7])=[CH2:6].[CH3:8][C:9]1[CH2:10][CH2:11][CH:12]2[C:18]=1[CH2:17][CH2:16][C:15](=[O:19])[CH2:14][C:13]2=[CH2:20]>O1CCCC1>[OH:19][C:15]1([C:5]([CH3:7])=[CH2:6])[CH2:16][CH2:17][C:18]2[CH:12]([CH2:11][CH2:10][C:9]=2[CH3:8])[C:13](=[CH2:20])[CH2:14]1",
+            "To a Grignard solution, prepared from 1 g of magnesium chips activated with 1 g of iodine, 5 ml of 2-bromopropene and about 100 ml of tetrahydrofuran, were added over 10 minutes 1.76 g of 1-methyl-4-methylen-6-oxo-2,3,3a,4,5,6,7,8-octahydroazulene. The mixture was stirred vigorously for 30 minutes, cooled to 0\302\260 and treated with excess ice-cold ammonium chloride solution. The mixture was then extracted with ether, the organic extract washed with carbonate solution and water, dried over magnesium sulphate and concentrated under reduced pressure. The crude product (2.6 g), which was obtained in the form of a yellow oil, was distilled under high vacuum and yielded 1.6 g (yield 76%) of pure 6-hydroxy-6-isopropenyl-1-methyl-4-methylen-2,3,3a,4,5,6,7,8-octahydroazulene; b.p.0.1 ca 100\302\260 IR(film):\316\275max = 3550, 3090, 1640, 1450/40, 1378, 1330, 1220, 1165, 1105, 1065, 1038, 900/895, 780 cm-1. The compound has a woody, slightly camphorous, somewhat spicy odour.",
+            None,
+            [],
+            True,
+        ],
+        [
+            "ord_dataset-a0eff6fe4b4143f284f0fc5ac503acad",
+            1932,
+            {},
+            True,
+            [
+                "C=C(C)Br",
+                "C=C1CC(=O)CCC2=C(C)CCC12",
+                "II",
+                "[Mg]",
+            ],
+            [],
+            [],
+            [
+                "C1CCOC1",
+            ],
+            [],
+            ["C=C1CC(O)(C(=C)C)CCC2=C(C)CCC12"],
+            [76.0],
+            None,
+            0.5,
+            "[Mg].II.Br[C:5]([CH3:7])=[CH2:6].[CH3:8][C:9]1[CH2:10][CH2:11][CH:12]2[C:18]=1[CH2:17][CH2:16][C:15](=[O:19])[CH2:14][C:13]2=[CH2:20]>O1CCCC1>[OH:19][C:15]1([C:5]([CH3:7])=[CH2:6])[CH2:16][CH2:17][C:18]2[CH:12]([CH2:11][CH2:10][C:9]=2[CH3:8])[C:13](=[CH2:20])[CH2:14]1",
+            "To a Grignard solution, prepared from 1 g of magnesium chips activated with 1 g of iodine, 5 ml of 2-bromopropene and about 100 ml of tetrahydrofuran, were added over 10 minutes 1.76 g of 1-methyl-4-methylen-6-oxo-2,3,3a,4,5,6,7,8-octahydroazulene. The mixture was stirred vigorously for 30 minutes, cooled to 0\302\260 and treated with excess ice-cold ammonium chloride solution. The mixture was then extracted with ether, the organic extract washed with carbonate solution and water, dried over magnesium sulphate and concentrated under reduced pressure. The crude product (2.6 g), which was obtained in the form of a yellow oil, was distilled under high vacuum and yielded 1.6 g (yield 76%) of pure 6-hydroxy-6-isopropenyl-1-methyl-4-methylen-2,3,3a,4,5,6,7,8-octahydroazulene; b.p.0.1 ca 100\302\260 IR(film):\316\275max = 3550, 3090, 1640, 1450/40, 1378, 1330, 1220, 1165, 1105, 1065, 1038, 900/895, 780 cm-1. The compound has a woody, slightly camphorous, somewhat spicy odour.",
+            None,
+            [],
+            True,
+        ],
+        [
+            "ord_dataset-85c00026681b46f89ef8634d2b8618c3",
+            3948,
+            {},
+            False,
+            [
+                "[Co]",
+                "O=S(=O)(O)O",
+            ],
+            ["[Co+3]", "CCCCCC=N", "O=S(=O)([O-])[O-]", "[NH4+]"],
+            [],
+            [],
+            [],
+            [],
+            [],
+            None,
+            None,
+            "[Co:1].[S:2]([OH:6])([OH:5])(=[O:4])=[O:3].[CH:7](=[NH:13])[CH2:8][CH2:9][CH2:10][CH2:11][CH3:12].[S:14]([O-:18])([O-:17])(=[O:16])=[O:15].[NH4+].[NH4+].[Co+3]>>[S:2]([O-:6])([O-:5])(=[O:4])=[O:3].[CH:7](=[NH:13])[CH2:8][CH2:9][CH2:10][CH2:11][CH3:12].[Co+3:1].[S:14]([O-:18])([O-:17])(=[O:16])=[O:15].[S:2]([O-:6])([O-:5])(=[O:4])=[O:3].[Co+3:1]",
+            "In a process for producing cobalt metal powder from nickel-cobalt sulphides comprising leaching said nickel-cobalt sulphides in an ammoniacal ammonium sulphate solution under an elevated pressure of an oxygen bearing gas, at a temperature of at least 80\302\260 C., with an effective ammonia to metals mole ratio in the range of 5:1 to 6.5:1 to oxidize the nickel and cobalt sulphides to sulphates, and to produce an ammoniacal ammonium sulphate leach liquor in which dissolved cobalt is predominantly in the (III) oxidation state, and an ammoniacal ammonium sulphate leach residue containing a cobalt (III) hexannmine sulphate-calcium sulphate double salt, separating the ammoniacal ammonium sulphate leach liquor from the ammoniacal ammonium sulphate leach residue, saturating the ammoniacal ammonium sulphate leach liquor with an effective amount of anydrous ammonia and cooling the ammoniated leach liquor to below 50\302\260 C. to precipitate the triple salt of cobalt (III) hexammine supbate, nickel (II) hexammine sulphate and ammonium sulphate, recovering the precipitated triple salt from the leach liquor, repulping the triple salt with an effective amount of water to selectively leach nickel(II) hexammine sulphate and to produce a crystalline cobalt (III) hexammine sulphate with a Co:Ni ratio of at least 100:1 and a nickel enriched leach liquor, dissolving the cobalt (III) hexammine sulphate in hot ammonium sulphate solution, and cooling the solution to precipitate recrystallized cobalt (III) hexammine sulphate having a Co:Ni ratio of at least about 1000:1 and treating the recrystallized cobalt (III) hexammine sulphate to produce cobalt metal therefrom, the improvement comprising:",
+            None,
+            [],
+            True,
+        ],
+    ),
+)
+@pytest.mark.parametrize("execution_number", range(REPETITIONS))
+def test_handle_reaction_object(
+    execution_number: int,
+    file_name: str,
+    rxn_idx: int,
+    manual_replacements_dict: MANUAL_REPLACEMENTS_DICT,
+    trust_labelling: bool,
+    expected_reactants: List[str],
+    expected_agents: List[str],
+    expected_reagents: List[str],
+    expected_solvents: List[str],
+    expected_catalysts: List[str],
+    expected_products: List[str],
+    expected_yields: List[Optional[float]],
+    expected_temperature: Optional[float],
+    expected_rxn_time: Optional[float],
+    expected_rxn_str: Optional[str],
+    expected_procedure_details: str,
+    expected_date_of_experiment: Optional[str],
+    expected_names_list: List[str],
+    expected_is_mapped: bool,
+) -> None:
+    import orderly.extract.extractor
+    import orderly.extract.main
+    import orderly.extract.defaults
+    import pandas as pd
+
+    rxn = get_rxn_func()(file_name, rxn_idx)
+    if manual_replacements_dict == {}:
+        manual_replacements_dict = orderly.extract.main.get_manual_replacements_dict(
+            solvents_path=None
+        )
+
+    assert manual_replacements_dict is not None
+
+    solvents_set = orderly.extract.defaults.get_solvents_set()
+
+    rnx_object = orderly.extract.extractor.OrdExtractor.handle_reaction_object(
+        rxn,
+        manual_replacements_dict,
+        solvents_set,
+        trust_labelling,
+        consider_molecule_names=True,
+    )
+
+    assert rnx_object is not None
+
+    (
+        reactants,
+        agents,
+        reagents,
+        solvents,
+        catalysts,
+        products,
+        yields,
+        temperature,
+        rxn_time,
+        rxn_str,
+        procedure_details,
+        date_of_experiment,
+        is_mapped,
+        names_list,
+    ) = rnx_object
+
+    def clean_string(s: str) -> str:
+        import string
+
+        printable = set(string.printable)
+        return "".join(filter(lambda x: x in printable, s))
+
+    clean_procedure_details = clean_string(procedure_details)
+    clean_expected_procedure_details = clean_string(expected_procedure_details)
+
+    assert sorted(reactants) == sorted(
+        expected_reactants
+    ), f"failure for {sorted(expected_reactants)=} got {sorted(reactants)}"  # TODO unsure why we have random ordering on ubuntu
+    assert agents == expected_agents, f"failure for {expected_agents=} got {agents}"
+    assert (
+        reagents == expected_reagents
+    ), f"failure for {expected_reagents=} got {reagents}"
+    assert (
+        solvents == expected_solvents
+    ), f"failure for {expected_solvents=} got {solvents}"
+    assert (
+        catalysts == expected_catalysts
+    ), f"failure for {expected_catalysts=} got {catalysts}"
+    assert (
+        products == expected_products
+    ), f"failure for {expected_products=} got {products}"
+    assert yields == expected_yields, f"failure for {expected_yields=} got {yields}"
+    assert (
+        temperature == expected_temperature
+    ), f"failure for {expected_temperature=} got {temperature}"
+    assert (
+        rxn_time == expected_rxn_time
+    ), f"failure for {expected_rxn_time=} got {rxn_time}"
+    assert rxn_str == expected_rxn_str, f"failure for {expected_rxn_str=} got {rxn_str}"
+    assert (
+        names_list == expected_names_list
+    ), f"failure for {expected_names_list=} got {names_list}"
+    assert (
+        clean_procedure_details == clean_expected_procedure_details
+    ), f"failure for {clean_expected_procedure_details=} got {clean_procedure_details}"
+    assert date_of_experiment == pd.to_datetime(
+        expected_date_of_experiment, format="%m/%d/%Y"
+    ), f"failure for {expected_date_of_experiment=} got {date_of_experiment}"
+    assert (
+        is_mapped == expected_is_mapped
+    ), f"failure for {expected_is_mapped=} got {is_mapped}"
+
+
+@pytest.mark.parametrize(
+    "smiles,is_mapped,expected_canonical_smiles",
+    (
+        ["teststring", True, None],
+        ["teststring", False, None],
+        ["c1ccccc1", False, "c1ccccc1"],
+        [
+            "[CH2:1]([S:8][C:9]1[CH:14]=[C:13]([O:15][C:16]2[CH:21]=[CH:20][C:19]([C:22]([F:25])([F:24])[F:23])=[CH:18][C:17]=2[Cl:26])[CH:12]=[CH:11][C:10]=1[N+:27]([O-])=O)[C:2]1[CH:7]=[CH:6][CH:5]=[CH:4][CH:3]=1",
+            True,
+            "O=[N+]([O-])c1ccc(Oc2ccc(C(F)(F)F)cc2Cl)cc1SCc1ccccc1",
+        ],
+        ["P([O-])(O)O", False, "[O-]P(O)O"],
+        [
+            "[CC(C)(C)[P]([Pd][P](C(C)(C)C)(C(C)(C)C)C(C)(C)C)(C(C)(C)C)C(C)(C)C]",
+            False,
+            "CC(C)(C)[P]([Pd][P](C(C)(C)C)(C(C)(C)C)C(C)(C)C)(C(C)(C)C)C(C)(C)C",
+        ],
+        [
+            "[CC(C)(C)[P]([Pd][P](C(C)(C)C)(C(C)(C)C)C(C)(C)C)(C(C)(C)C)C(C)(C)C]",
+            True,
+            "CC(C)(C)[P]([Pd][P](C(C)(C)C)(C(C)(C)C)C(C)(C)C)(C(C)(C)C)C(C)(C)C",
+        ],
+    ),
+)
+@pytest.mark.parametrize("execution_number", range(REPETITIONS))
+def test_canonicalisation(
+    execution_number: int,
+    smiles: str,
+    is_mapped: bool,
+    expected_canonical_smiles: Optional[str],
+) -> None:
+    from orderly.extract.canonicalise import get_canonicalised_smiles
+
+    canonical_smiles = get_canonicalised_smiles(smiles, is_mapped)
+
+    assert (
+        expected_canonical_smiles == canonical_smiles
+    ), f"failure for {expected_canonical_smiles=} got {canonical_smiles}"
+
+
+@pytest.mark.parametrize(
+    "trust_labelling,use_multiprocessing,name_contains_substring,inverse_substring",
+    (
+        [True, False, "uspto", True],
+        [False, True, "uspto", True],
+        [
+            False,
+            True,
+            "uspto",
+            False,
+        ],
+        [True, True, None, True],
+    ),
+)
+@pytest.mark.parametrize("execution_number", range(SLOW_REPETITIONS))
+def test_extraction_pipeline(
+    execution_number: int,
+    tmp_path: pathlib.Path,
+    trust_labelling: bool,
+    use_multiprocessing: bool,
+    name_contains_substring: Optional[str],
+    inverse_substring: bool,
+) -> None:
+    extracted_ord_data_folder = "extracted_ord_data"
+    (tmp_path / extracted_ord_data_folder).mkdir()
+    molecule_names_folder = "molecule_names"
+    (tmp_path / molecule_names_folder).mkdir()
+
+    import orderly.extract.main
+    import orderly.data.test_data
+
+    orderly.extract.main.main(
+        data_path=orderly.data.test_data.get_path_of_test_ords(),
+        ord_file_ending=".pb.gz",
+        trust_labelling=trust_labelling,
+        consider_molecule_names=True,  # TODO: add test for consider_molecule_names=False
+        output_path=tmp_path,
+        extracted_ord_data_folder=extracted_ord_data_folder,
+        solvents_path=None,
+        molecule_names_folder=molecule_names_folder,
+        merged_molecules_file="all_molecule_names.csv",
+        use_multiprocessing=use_multiprocessing,
+        name_contains_substring=name_contains_substring,
+        inverse_substring=inverse_substring,
+        overwrite=False,
+    )
+
+    import pandas as pd
+    import numpy as np
+
+    for extraction in (tmp_path / extracted_ord_data_folder).glob("*"):
+        df = pd.read_parquet(extraction)
+
+        df = df.sort_index(axis=1)
+
+        assert df is not None
+
+        check_none_order_cols = [
+            "reactant",
+            "agent",
+            "reagent",
+            "solvent",
+            "catalyst",
+            "product",  # note, if this is reordered it will be out of sync with yield
+            # "yield",  we are ok with this having nones in bad order
+        ]
+        for check_col in check_none_order_cols:
+            valid_cols = sorted(
+                [col for col in df.columns if col.startswith(check_col)]
+            )
+            tmp_df = df[valid_cols]
+
+            def check_valid_order(row: pd.Series) -> pd.Series:
+                seen_none = False
+                for idx, a in enumerate(row):
+                    current_isna = pd.isna(a) or (a == "")
+                    if seen_none:
+                        if not current_isna:
+                            raise ValueError(
+                                f"Unexpected order at {idx=} for {row.tolist()=}"
+                            )
+                    if current_isna:
+                        seen_none = True
+                return row
+
+            tmp_df.apply(check_valid_order, axis=1)
+
+        # Columns: ['rxn_str', 'reactant_000', 'reactant_001', 'reactant_002', 'reactant_003', 'agent_000', 'agent_001', 'agent_002', 'agent_003', 'agent_004', 'agent_005', 'solvent_000', 'solvent_001', 'solvent_002', 'temperature', 'rxn_time', 'product_000', 'yield_000', 'grant_date'],
+        # They're allowed to be strings or floats (depending on the col) or None
+        for col in df.columns:
+            series = df[col].replace({None: np.nan})
+            if len(series.dropna()) == 0:
+                continue
+            elif col in ["grant_date", "date_of_experiment"]:
+                assert pd.api.types.is_datetime64_ns_dtype(
+                    series
+                ), f"failure for {col=}: {series.dtype=}"
+            elif ("temperature" in col) or ("rxn_time" in col) or ("yield" in col):
+                assert pd.api.types.is_float_dtype(
+                    series
+                ), f"failure for {col=} {series.dtype=}"
+            elif "is_mapped" in col:
+                assert pd.api.types.is_bool_dtype(
+                    series
+                ), f"failure for {col=} {series.dtype=}"
+            else:
+                assert pd.api.types.is_object_dtype(
+                    series
+                ), f"failure for {col=} {series.dtype=}"
+
+
+@pytest.mark.parametrize(
+    "use_multiprocessing,name_contains_substring,inverse_substring,file_to_extract,file_to_compare_against",
+    (
+        [
+            True,
+            "uspto",
+            False,
+            "0c61835e3a0b4986aabf2b61b708e322.pb.gz",
+            "uspto-grants-1995_11.parquet",
+        ],
+        [
+            True,
+            "uspto",
+            False,
+            "0c61835e3a0b4986aabf2b61b708e322.pb.gz",
+            "uspto-grants-1995_11.parquet",
+        ],
+    ),
+)
+@pytest.mark.parametrize("execution_number", range(SLOW_REPETITIONS))
+@pytest.mark.parametrize("trust_labelling", [False, True])
+def test_extraction_pipeline_exact_output(
+    execution_number: int,
+    tmp_path: pathlib.Path,
+    trust_labelling: bool,
+    use_multiprocessing: bool,
+    name_contains_substring: Optional[str],
+    inverse_substring: bool,
+    file_to_extract: str,
+    file_to_compare_against: str,
+) -> None:
+    extracted_ord_data_folder = "extracted_ord_data"
+    (tmp_path / extracted_ord_data_folder).mkdir()
+    molecule_names_folder = "molecule_names"
+    (tmp_path / molecule_names_folder).mkdir()
+
+    import orderly.extract.main
+    import orderly.data.test_data
+
+    orderly.extract.main.main(
+        data_path=orderly.data.test_data.get_path_of_test_ords(),
+        ord_file_ending=file_to_extract,
+        trust_labelling=trust_labelling,
+        consider_molecule_names=False,  # TODO: add test for consider_molecule_names=False
+        output_path=tmp_path,
+        extracted_ord_data_folder=extracted_ord_data_folder,
+        solvents_path=None,
+        molecule_names_folder=molecule_names_folder,
+        merged_molecules_file="all_molecule_names.csv",
+        use_multiprocessing=use_multiprocessing,
+        name_contains_substring=name_contains_substring,
+        inverse_substring=inverse_substring,
+        overwrite=False,
+    )
+
+    import pandas as pd
+    import numpy as np
+
+    compare_against_df = pd.read_parquet(
+        orderly.data.test_data.get_path_of_test_extracted_ords(
+            trust_labelling=trust_labelling
+        )
+        / "extracted_ords"
+        / file_to_compare_against
+    )
+    created_df = pd.read_parquet(
+        tmp_path / extracted_ord_data_folder / file_to_compare_against
+    )
+
+    pd.testing.assert_frame_equal(created_df, compare_against_df)
```

