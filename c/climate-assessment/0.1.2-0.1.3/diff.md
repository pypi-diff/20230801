# Comparing `tmp/climate-assessment-0.1.2.tar.gz` & `tmp/climate-assessment-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climate-assessment-0.1.2.tar", last modified: Tue Jun 13 15:42:38 2023, max compression
+gzip compressed data, was "climate-assessment-0.1.3.tar", last modified: Tue Aug  1 14:13:07 2023, max compression
```

## Comparing `climate-assessment-0.1.2.tar` & `climate-assessment-0.1.3.tar`

### file list

```diff
@@ -1,91 +1,92 @@
-drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2023-06-13 15:42:38.560252 climate-assessment-0.1.2/
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      226 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/.dockerignore
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      965 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/.env.sample
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     2035 2023-05-11 09:56:20.000000 climate-assessment-0.1.2/.gitignore
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      107 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/.readthedocs.yml
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     1074 2023-06-13 15:33:48.000000 climate-assessment-0.1.2/CHANGELOG.rst
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     1393 2023-06-13 15:33:54.000000 climate-assessment-0.1.2/CITATION.cff
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      588 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/Dockerfile
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     1073 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/LICENSE
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)       44 2023-05-11 09:56:20.000000 climate-assessment-0.1.2/MANIFEST.in
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     3650 2023-05-11 09:56:20.000000 climate-assessment-0.1.2/Makefile
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     4289 2023-06-13 15:42:38.560252 climate-assessment-0.1.2/PKG-INFO
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     3034 2023-05-11 09:56:20.000000 climate-assessment-0.1.2/README.rst
-drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2023-06-13 15:42:38.528253 climate-assessment-0.1.2/data/
-drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2023-06-13 15:42:38.528253 climate-assessment-0.1.2/data/cicero/
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)   295394 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/data/cicero/subset_cscm_configfile.json
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     9175 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/data/emissions_variable_list_climateruns.xlsx
-drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2023-06-13 15:42:38.536253 climate-assessment-0.1.2/doc/
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      634 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/doc/Makefile
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     3583 2023-06-13 15:33:54.000000 climate-assessment-0.1.2/doc/NOTICE.rst
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      867 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/doc/README.rst
-drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2023-06-13 15:42:38.540253 climate-assessment-0.1.2/doc/_static/
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)        0 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/doc/_static/.gitkeep
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)   305539 2022-06-08 09:35:56.000000 climate-assessment-0.1.2/doc/_static/category_flowchart.jpg
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    86790 2022-06-08 09:35:56.000000 climate-assessment-0.1.2/doc/_static/overview_workflow.png
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     2558 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/doc/code.rst
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     2500 2022-06-21 15:23:17.000000 climate-assessment-0.1.2/doc/conf.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     1272 2022-06-08 09:35:56.000000 climate-assessment-0.1.2/doc/dev.rst
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    10916 2023-06-13 15:33:54.000000 climate-assessment-0.1.2/doc/emulator.rst
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    61922 2023-06-13 15:33:54.000000 climate-assessment-0.1.2/doc/general.rst
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     5071 2023-06-13 15:33:54.000000 climate-assessment-0.1.2/doc/index.rst
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     3219 2023-05-11 09:56:20.000000 climate-assessment-0.1.2/doc/install.rst
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      760 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/doc/make.bat
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     1584 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/doc/prereqs.rst
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     1540 2022-06-08 09:35:56.000000 climate-assessment-0.1.2/doc/user_guide.rst
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      714 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/doc/utility.rst
-drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2023-06-13 15:42:38.540253 climate-assessment-0.1.2/notebooks/
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)        0 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/notebooks/.gitkeep
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     9853 2023-05-11 09:56:20.000000 climate-assessment-0.1.2/notebooks/run-example-ciceroscm.ipynb
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    13107 2023-05-11 09:56:20.000000 climate-assessment-0.1.2/notebooks/run-example-custom.ipynb
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    11556 2023-05-11 09:56:20.000000 climate-assessment-0.1.2/notebooks/run-example-fair.ipynb
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    13020 2023-05-11 09:56:20.000000 climate-assessment-0.1.2/notebooks/run-example-magicc.ipynb
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      109 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/run_docker.sh
-drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2023-06-13 15:42:38.544252 climate-assessment-0.1.2/scripts/
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     2125 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/scripts/generate-magicc-sr15-input-files.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      161 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/scripts/run_clim.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      177 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/scripts/run_create_infillerdatabase.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      100 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/scripts/run_extract_ips.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      162 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/scripts/run_harm.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      173 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/scripts/run_harm_inf.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      159 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/scripts/run_infilling.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      164 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/scripts/run_postprocess.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      117 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/scripts/run_split_scenarios.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      161 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/scripts/run_workflow.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     2262 2023-06-13 15:42:38.560252 climate-assessment-0.1.2/setup.cfg
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)       58 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/setup.py
-drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2023-06-13 15:42:38.524253 climate-assessment-0.1.2/src/
-drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2023-06-13 15:42:38.548252 climate-assessment-0.1.2/src/climate_assessment/
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      853 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/__init__.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    38775 2023-06-13 15:33:48.000000 climate-assessment-0.1.2/src/climate_assessment/checks.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    33528 2022-06-21 15:23:17.000000 climate-assessment-0.1.2/src/climate_assessment/cli.py
-drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2023-06-13 15:42:38.556252 climate-assessment-0.1.2/src/climate_assessment/climate/
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    16426 2023-05-17 09:02:43.000000 climate-assessment-0.1.2/src/climate_assessment/climate/__init__.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      830 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/climate/ciceroscm.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     3505 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/climate/fair.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     4713 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/climate/magicc7.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    17320 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/climate/post_process.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    12231 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/climate/variable_definitions.csv
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     2385 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/climate/wg3.py
-drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2023-06-13 15:42:38.556252 climate-assessment-0.1.2/src/climate_assessment/harmonization/
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    13035 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/harmonization/__init__.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      174 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/harmonization/aneris_ar6.yaml
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      173 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/harmonization/aneris_ar6_co2.yaml
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      175 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/harmonization/aneris_sr15.yaml
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      174 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/harmonization/aneris_sr15_co2.yaml
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    68340 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/harmonization/history_ar6.csv
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    68367 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/harmonization/history_sr15.csv
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)       69 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/harmonization/regions_ar6.csv
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     4469 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/harmonization_and_infilling.py
-drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2023-06-13 15:42:38.560252 climate-assessment-0.1.2/src/climate_assessment/infilling/
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    19254 2023-05-17 09:02:43.000000 climate-assessment-0.1.2/src/climate_assessment/infilling/__init__.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)   799351 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/infilling/cmip6-ssps-workflow-emissions.csv
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     2627 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/postprocess.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     1878 2023-05-17 09:02:43.000000 climate-assessment-0.1.2/src/climate_assessment/testing.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    16431 2023-05-17 09:02:43.000000 climate-assessment-0.1.2/src/climate_assessment/utils.py
-drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2023-06-13 15:42:38.552252 climate-assessment-0.1.2/src/climate_assessment.egg-info/
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     4289 2023-06-13 15:42:37.000000 climate-assessment-0.1.2/src/climate_assessment.egg-info/PKG-INFO
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     2325 2023-06-13 15:42:38.000000 climate-assessment-0.1.2/src/climate_assessment.egg-info/SOURCES.txt
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)        1 2023-06-13 15:42:37.000000 climate-assessment-0.1.2/src/climate_assessment.egg-info/dependency_links.txt
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      662 2023-06-13 15:42:37.000000 climate-assessment-0.1.2/src/climate_assessment.egg-info/requires.txt
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)       19 2023-06-13 15:42:37.000000 climate-assessment-0.1.2/src/climate_assessment.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:13:07.025075 climate-assessment-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/.env.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-08-01 14:13:07.025075 climate-assessment-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/RELEASING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:13:07.013075 climate-assessment-0.1.3/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:13:07.013075 climate-assessment-0.1.3/data/cicero/
+-rw-r--r--   0 runner    (1001) docker     (123)   295394 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/data/cicero/subset_cscm_configfile.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9175 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/data/emissions_variable_list_climateruns.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:13:07.013075 climate-assessment-0.1.3/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/doc/NOTICE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/doc/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:13:07.017075 climate-assessment-0.1.3/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/doc/_static/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)   305539 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/doc/_static/category_flowchart.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    86790 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/doc/_static/overview_workflow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/doc/code.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/doc/dev.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10916 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/doc/emulator.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    61922 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/doc/general.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/doc/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/doc/prereqs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/doc/user_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/doc/utility.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:13:07.017075 climate-assessment-0.1.3/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/notebooks/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     9853 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/notebooks/run-example-ciceroscm.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13107 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/notebooks/run-example-custom.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11556 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/notebooks/run-example-fair.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13020 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/notebooks/run-example-magicc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/run_docker.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:13:07.017075 climate-assessment-0.1.3/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/scripts/generate-magicc-sr15-input-files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/scripts/run_clim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/scripts/run_create_infillerdatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/scripts/run_extract_ips.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/scripts/run_harm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/scripts/run_harm_inf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/scripts/run_infilling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/scripts/run_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/scripts/run_split_scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/scripts/run_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-08-01 14:13:07.025075 climate-assessment-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:13:07.009074 climate-assessment-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:13:07.021075 climate-assessment-0.1.3/src/climate_assessment/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/src/climate_assessment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38775 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/src/climate_assessment/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33528 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/src/climate_assessment/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:13:07.021075 climate-assessment-0.1.3/src/climate_assessment/climate/
+-rw-r--r--   0 runner    (1001) docker     (123)    16426 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/src/climate_assessment/climate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/src/climate_assessment/climate/ciceroscm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/src/climate_assessment/climate/fair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/src/climate_assessment/climate/magicc7.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17320 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/src/climate_assessment/climate/post_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12231 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/src/climate_assessment/climate/variable_definitions.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/src/climate_assessment/climate/wg3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:13:07.021075 climate-assessment-0.1.3/src/climate_assessment/harmonization/
+-rw-r--r--   0 runner    (1001) docker     (123)    13035 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/src/climate_assessment/harmonization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/src/climate_assessment/harmonization/aneris_ar6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/src/climate_assessment/harmonization/aneris_ar6_co2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/src/climate_assessment/harmonization/aneris_sr15.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/src/climate_assessment/harmonization/aneris_sr15_co2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    68340 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/src/climate_assessment/harmonization/history_ar6.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    68367 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/src/climate_assessment/harmonization/history_sr15.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/src/climate_assessment/harmonization/regions_ar6.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/src/climate_assessment/harmonization_and_infilling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:13:07.025075 climate-assessment-0.1.3/src/climate_assessment/infilling/
+-rw-r--r--   0 runner    (1001) docker     (123)    19254 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/src/climate_assessment/infilling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   799351 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/src/climate_assessment/infilling/cmip6-ssps-workflow-emissions.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/src/climate_assessment/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/src/climate_assessment/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16431 2023-08-01 14:12:44.000000 climate-assessment-0.1.3/src/climate_assessment/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:13:07.021075 climate-assessment-0.1.3/src/climate_assessment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-08-01 14:13:05.000000 climate-assessment-0.1.3/src/climate_assessment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-08-01 14:13:07.000000 climate-assessment-0.1.3/src/climate_assessment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:13:05.000000 climate-assessment-0.1.3/src/climate_assessment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-01 14:13:05.000000 climate-assessment-0.1.3/src/climate_assessment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-01 14:13:05.000000 climate-assessment-0.1.3/src/climate_assessment.egg-info/top_level.txt
```

### Comparing `climate-assessment-0.1.2/.env.sample` & `climate-assessment-0.1.3/.env.sample`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/.gitignore` & `climate-assessment-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/CHANGELOG.rst` & `climate-assessment-0.1.3/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     - Security: in case of vulnerabilities.
 
 master
 ------
 
 Added
 ~~~~~
+- (`#40 https://github.com/iiasa/climate-assessment/pull/40`_) Update awscli to >= 1.29.4
 - (`#31 https://github.com/iiasa/climate-assessment/pull/31`_) Update pyam-iamc to >=1.7.0
 - (`#15 <https://github.com/iiasa/climate-assessment/pull/15>`_) Fix packaging issues and add installation instructions
 - (`#6 <https://github.com/iiasa/climate-assessment/pull/6>`_) Added example run notebooks and tests thereof
 - (`#1 <https://github.com/iiasa/climate-assessment/pull/1>`_) Added :func:`climate_assessment.cli.run_workflow`
 
 
 v0.1.0 - 2022-06-08
```

### Comparing `climate-assessment-0.1.2/CITATION.cff` & `climate-assessment-0.1.3/CITATION.cff`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/Dockerfile` & `climate-assessment-0.1.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/LICENSE` & `climate-assessment-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/Makefile` & `climate-assessment-0.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/PKG-INFO` & `climate-assessment-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climate-assessment
-Version: 0.1.2
+Version: 0.1.3
 Summary: Climate assessment of long-term emissions pathways: IPCC AR6 WGIII version
 Home-page: https://github.com/iiasa/climate-assessment
 Author: Jarmo S. Kikstra, Zebedee R.J. Nicholls, Jared Lewis, Christopher J. Smith, Robin D. Lamboll, Edward Byers, Marit Sandstad, Laura Wienpahl, Philip Hackstock
 Author-email: kikstra@iiasa.ac.at
 License: MIT License
 Project-URL: Source, http://github.com/iiasa/climate-assessment
 Project-URL: Documentation, https://climate-assessment.readthedocs.io/
```

### Comparing `climate-assessment-0.1.2/README.rst` & `climate-assessment-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/data/cicero/subset_cscm_configfile.json` & `climate-assessment-0.1.3/data/cicero/subset_cscm_configfile.json`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/data/emissions_variable_list_climateruns.xlsx` & `climate-assessment-0.1.3/data/emissions_variable_list_climateruns.xlsx`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/doc/Makefile` & `climate-assessment-0.1.3/doc/Makefile`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/doc/NOTICE.rst` & `climate-assessment-0.1.3/doc/NOTICE.rst`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/doc/README.rst` & `climate-assessment-0.1.3/doc/README.rst`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/doc/_static/category_flowchart.jpg` & `climate-assessment-0.1.3/doc/_static/category_flowchart.jpg`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/doc/_static/overview_workflow.png` & `climate-assessment-0.1.3/doc/_static/overview_workflow.png`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/doc/code.rst` & `climate-assessment-0.1.3/doc/code.rst`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/doc/conf.py` & `climate-assessment-0.1.3/doc/conf.py`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/doc/dev.rst` & `climate-assessment-0.1.3/doc/dev.rst`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/doc/emulator.rst` & `climate-assessment-0.1.3/doc/emulator.rst`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/doc/general.rst` & `climate-assessment-0.1.3/doc/general.rst`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/doc/index.rst` & `climate-assessment-0.1.3/doc/index.rst`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/doc/install.rst` & `climate-assessment-0.1.3/doc/install.rst`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/doc/make.bat` & `climate-assessment-0.1.3/doc/make.bat`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/doc/prereqs.rst` & `climate-assessment-0.1.3/doc/prereqs.rst`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/doc/user_guide.rst` & `climate-assessment-0.1.3/doc/user_guide.rst`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/doc/utility.rst` & `climate-assessment-0.1.3/doc/utility.rst`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/notebooks/run-example-ciceroscm.ipynb` & `climate-assessment-0.1.3/notebooks/run-example-ciceroscm.ipynb`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/notebooks/run-example-custom.ipynb` & `climate-assessment-0.1.3/notebooks/run-example-custom.ipynb`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/notebooks/run-example-fair.ipynb` & `climate-assessment-0.1.3/notebooks/run-example-fair.ipynb`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/notebooks/run-example-magicc.ipynb` & `climate-assessment-0.1.3/notebooks/run-example-magicc.ipynb`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/scripts/generate-magicc-sr15-input-files.py` & `climate-assessment-0.1.3/scripts/generate-magicc-sr15-input-files.py`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/setup.cfg` & `climate-assessment-0.1.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 [options]
 packages = find:
 package_dir = 
 	=src
 include_package_data = True
 install_requires = 
 	aneris-iamc==0.3.1
-	awscli==1.27.134
+	awscli>=1.29.4
 	click
 	fair==1.6.2
 	importlib-metadata
 	joblib
 	matplotlib
 	numpy
 	openscm-units==0.5.0
```

### Comparing `climate-assessment-0.1.2/src/climate_assessment/__init__.py` & `climate-assessment-0.1.3/src/climate_assessment/__init__.py`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/src/climate_assessment/checks.py` & `climate-assessment-0.1.3/src/climate_assessment/checks.py`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/src/climate_assessment/cli.py` & `climate-assessment-0.1.3/src/climate_assessment/cli.py`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/src/climate_assessment/climate/__init__.py` & `climate-assessment-0.1.3/src/climate_assessment/climate/__init__.py`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/src/climate_assessment/climate/ciceroscm.py` & `climate-assessment-0.1.3/src/climate_assessment/climate/ciceroscm.py`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/src/climate_assessment/climate/fair.py` & `climate-assessment-0.1.3/src/climate_assessment/climate/fair.py`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/src/climate_assessment/climate/magicc7.py` & `climate-assessment-0.1.3/src/climate_assessment/climate/magicc7.py`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/src/climate_assessment/climate/post_process.py` & `climate-assessment-0.1.3/src/climate_assessment/climate/post_process.py`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/src/climate_assessment/climate/variable_definitions.csv` & `climate-assessment-0.1.3/src/climate_assessment/climate/variable_definitions.csv`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/src/climate_assessment/climate/wg3.py` & `climate-assessment-0.1.3/src/climate_assessment/climate/wg3.py`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/src/climate_assessment/harmonization/__init__.py` & `climate-assessment-0.1.3/src/climate_assessment/harmonization/__init__.py`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/src/climate_assessment/harmonization/history_ar6.csv` & `climate-assessment-0.1.3/src/climate_assessment/harmonization/history_ar6.csv`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/src/climate_assessment/harmonization/history_sr15.csv` & `climate-assessment-0.1.3/src/climate_assessment/harmonization/history_sr15.csv`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/src/climate_assessment/harmonization_and_infilling.py` & `climate-assessment-0.1.3/src/climate_assessment/harmonization_and_infilling.py`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/src/climate_assessment/infilling/__init__.py` & `climate-assessment-0.1.3/src/climate_assessment/infilling/__init__.py`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/src/climate_assessment/infilling/cmip6-ssps-workflow-emissions.csv` & `climate-assessment-0.1.3/src/climate_assessment/infilling/cmip6-ssps-workflow-emissions.csv`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/src/climate_assessment/postprocess.py` & `climate-assessment-0.1.3/src/climate_assessment/postprocess.py`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/src/climate_assessment/testing.py` & `climate-assessment-0.1.3/src/climate_assessment/testing.py`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/src/climate_assessment/utils.py` & `climate-assessment-0.1.3/src/climate_assessment/utils.py`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.2/src/climate_assessment.egg-info/PKG-INFO` & `climate-assessment-0.1.3/src/climate_assessment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climate-assessment
-Version: 0.1.2
+Version: 0.1.3
 Summary: Climate assessment of long-term emissions pathways: IPCC AR6 WGIII version
 Home-page: https://github.com/iiasa/climate-assessment
 Author: Jarmo S. Kikstra, Zebedee R.J. Nicholls, Jared Lewis, Christopher J. Smith, Robin D. Lamboll, Edward Byers, Marit Sandstad, Laura Wienpahl, Philip Hackstock
 Author-email: kikstra@iiasa.ac.at
 License: MIT License
 Project-URL: Source, http://github.com/iiasa/climate-assessment
 Project-URL: Documentation, https://climate-assessment.readthedocs.io/
```

### Comparing `climate-assessment-0.1.2/src/climate_assessment.egg-info/SOURCES.txt` & `climate-assessment-0.1.3/src/climate_assessment.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 CHANGELOG.rst
 CITATION.cff
 Dockerfile
 LICENSE
 MANIFEST.in
 Makefile
 README.rst
+RELEASING.rst
 run_docker.sh
 setup.cfg
 setup.py
 data/emissions_variable_list_climateruns.xlsx
 data/cicero/subset_cscm_configfile.json
 doc/Makefile
 doc/NOTICE.rst
```

### Comparing `climate-assessment-0.1.2/src/climate_assessment.egg-info/requires.txt` & `climate-assessment-0.1.3/src/climate_assessment.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 aneris-iamc==0.3.1
-awscli==1.27.134
+awscli>=1.29.4
 click
 fair==1.6.2
 importlib-metadata
 joblib
 matplotlib
 numpy
 openscm-units==0.5.0
```

