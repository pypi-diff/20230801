# Comparing `tmp/jdaviz-3.6.0.tar.gz` & `tmp/jdaviz-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jdaviz-3.6.0.tar", last modified: Fri Jul 28 18:47:40 2023, max compression
+gzip compressed data, was "jdaviz-3.6.1.tar", last modified: Tue Aug  1 20:36:48 2023, max compression
```

## Comparing `jdaviz-3.6.0.tar` & `jdaviz-3.6.1.tar`

### file list

```diff
@@ -1,522 +1,522 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.301016 jdaviz-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.bandit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.241016 jdaviz-3.6.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.241016 jdaviz-3.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.github/labeler.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.245016 jdaviz-3.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.github/workflows/changelog_check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.github/workflows/ci_cron_weekly.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.github/workflows/ci_workflows.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.github/workflows/open_actions.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.github/workflows/predeps_workflows.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.github/workflows/standalone.yml
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.mailmap
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-28 18:47:24.000000 jdaviz-3.6.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    47182 2023-07-28 18:47:24.000000 jdaviz-3.6.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-28 18:47:24.000000 jdaviz-3.6.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-28 18:47:24.000000 jdaviz-3.6.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-28 18:47:24.000000 jdaviz-3.6.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-28 18:47:24.000000 jdaviz-3.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-07-28 18:47:40.301016 jdaviz-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-07-28 18:47:24.000000 jdaviz-3.6.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-28 18:47:24.000000 jdaviz-3.6.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.245016 jdaviz-3.6.0/jdaviz/
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/_astropy_init.py
--rw-r--r--   0 runner    (1001) docker     (123)   100517 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/app.vue
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.249016 jdaviz-3.6.0/jdaviz/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/docs_link.vue
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/external_link.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/glue_state_sync_wrapper.vue
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/layer_viewer_icon.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/number_uncertainty.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/play_pause_widget.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/plugin_add_results.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/plugin_auto_label.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/plugin_dataset_select.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/plugin_layer_select.vue
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/plugin_plot.vue
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/plugin_popout.vue
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/plugin_section_header.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/plugin_subset_select.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/plugin_table.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/plugin_viewer_select.vue
--rw-r--r--   0 runner    (1001) docker     (123)     8873 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/toolbar_nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/toolbar_nested.vue
--rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/tooltip.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/tray_plugin.vue
--rw-r--r--   0 runner    (1001) docker     (123)     9425 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/viewer_data_select.vue
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/components/viewer_data_select_item.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.249016 jdaviz-3.6.0/jdaviz/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.249016 jdaviz-3.6.0/jdaviz/configs/cubeviz/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/cubeviz.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/cubeviz.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.249016 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.249016 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/moment_maps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/moment_maps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.249016 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/moment_maps/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/moment_maps/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/moment_maps/tests/test_moment_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)    18788 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.249016 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/slice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/slice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/slice/slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/slice/slice.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.249016 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/slice/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/slice/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/slice/tests/test_slice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.253016 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/tests/test_cubeviz_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/tests/test_data_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/tests/test_data_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/tests/test_export_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    10258 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/tests/test_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/viewers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.253016 jdaviz-3.6.0/jdaviz/configs/default/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/default.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.253016 jdaviz-3.6.0/jdaviz/configs/default/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.253016 jdaviz-3.6.0/jdaviz/configs/default/plugins/collapse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/collapse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/collapse/collapse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/collapse/collapse.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.253016 jdaviz-3.6.0/jdaviz/configs/default/plugins/collapse/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/collapse/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/collapse/tests/test_collapse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.253016 jdaviz-3.6.0/jdaviz/configs/default/plugins/data_tools/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/data_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/data_tools/data_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/data_tools/data_tools.vue
--rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/data_tools/file_chooser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.253016 jdaviz-3.6.0/jdaviz/configs/default/plugins/export_plot/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/export_plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/export_plot/export_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/export_plot/export_plot.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.253016 jdaviz-3.6.0/jdaviz/configs/default/plugins/gaussian_smooth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/gaussian_smooth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.253016 jdaviz-3.6.0/jdaviz/configs/default/plugins/gaussian_smooth/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/gaussian_smooth/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/gaussian_smooth/tests/test_gaussian_smooth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.257016 jdaviz-3.6.0/jdaviz/configs/default/plugins/line_lists/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/line_lists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/line_lists/line_list_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    35599 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/line_lists/line_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)    15805 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/line_lists/line_lists.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.257016 jdaviz-3.6.0/jdaviz/configs/default/plugins/line_lists/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/line_lists/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/line_lists/tests/test_line_lists.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.257016 jdaviz-3.6.0/jdaviz/configs/default/plugins/markers/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/markers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/markers/markers.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/markers/markers.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.257016 jdaviz-3.6.0/jdaviz/configs/default/plugins/markers/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/markers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12863 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/markers/tests/test_markers_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.257016 jdaviz-3.6.0/jdaviz/configs/default/plugins/metadata_viewer/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/metadata_viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.257016 jdaviz-3.6.0/jdaviz/configs/default/plugins/metadata_viewer/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/metadata_viewer/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/metadata_viewer/tests/test_metadata_viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.257016 jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13952 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/fitting_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/initializers.py
--rw-r--r--   0 runner    (1001) docker     (123)    44507 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/model_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/model_fitting.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.257016 jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/tests/test_blackbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    16097 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/tests/test_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    15676 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/tests/test_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.257016 jdaviz-3.6.0/jdaviz/configs/default/plugins/plot_options/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/plot_options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35709 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/plot_options/plot_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    26019 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/plot_options/plot_options.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.257016 jdaviz-3.6.0/jdaviz/configs/default/plugins/plot_options/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/plot_options/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/plot_options/tests/test_plot_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.257016 jdaviz-3.6.0/jdaviz/configs/default/plugins/subset_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/subset_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23109 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.261016 jdaviz-3.6.0/jdaviz/configs/default/plugins/subset_plugin/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/subset_plugin/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/subset_plugin/tests/test_subset_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.261016 jdaviz-3.6.0/jdaviz/configs/default/plugins/subset_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/subset_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/subset_tools/subset_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/subset_tools/subset_tools.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.261016 jdaviz-3.6.0/jdaviz/configs/default/plugins/viewer_creator/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/viewer_creator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.vue
--rw-r--r--   0 runner    (1001) docker     (123)    10148 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/default/plugins/viewers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.261016 jdaviz-3.6.0/jdaviz/configs/imviz/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19411 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/imviz.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/imviz.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.261016 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.261016 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/aper_phot_simple/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/aper_phot_simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25491 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.261016 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/catalogs/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/catalogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10913 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/catalogs/catalogs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/catalogs/catalogs.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.261016 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/compass/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/compass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/compass/compass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/compass/compass.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.261016 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/compass/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/compass/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/compass/tests/test_compass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.261016 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/coords_info/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/coords_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23107 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/coords_info/coords_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/coords_info/coords_info.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.265016 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/image_viewer_creator/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/image_viewer_creator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/image_viewer_creator/image_viewer_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/image_viewer_creator/image_viewer_creator.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.265016 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/line_profile_xy/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/line_profile_xy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.265016 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/links_control/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/links_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/links_control/links_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/links_control/links_control.vue
--rw-r--r--   0 runner    (1001) docker     (123)    14277 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.265016 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/rotate_canvas/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/rotate_canvas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.265016 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/rotate_canvas/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/rotate_canvas/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/rotate_canvas/tests/test_rotate_canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    13559 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/plugins/viewers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.269016 jdaviz-3.6.0/jdaviz/configs/imviz/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.269016 jdaviz-3.6.0/jdaviz/configs/imviz/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/data/ds9_annulus_01.reg
--rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/data/miri_i2d_lonlat_gwcs.asdf
--rw-r--r--   0 runner    (1001) docker     (123)  8425199 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/data/roman_wfi_image_model.asdf
--rw-r--r--   0 runner    (1001) docker     (123)    15711 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_astrowidgets_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_catalogs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_line_profile_xy.py
--rw-r--r--   0 runner    (1001) docker     (123)    19474 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_linking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_links_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    25880 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_parser_roman.py
--rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16125 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_simple_aper_phot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_subset_centroid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_viewer_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_viewers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_wcs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9197 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/imviz/wcs_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.277016 jdaviz-3.6.0/jdaviz/configs/mosviz/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38346 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/mosviz.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/mosviz.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.277016 jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40180 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.277016 jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/row_lock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/row_lock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/row_lock/row_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/row_lock/row_lock.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.277016 jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/slit_overlay/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/slit_overlay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/slit_overlay/slit_overlay.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/slit_overlay/slit_overlay.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.277016 jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/slit_overlay/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/slit_overlay/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/slit_overlay/tests/test_slit_overlay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    18704 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/viewers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.277016 jdaviz-3.6.0/jdaviz/configs/mosviz/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10691 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/tests/test_data_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/tests/test_source_identifier_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/mosviz/tests/test_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.281016 jdaviz-3.6.0/jdaviz/configs/specviz/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14962 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.281016 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.281016 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/line_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/line_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29328 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.281016 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/line_analysis/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/line_analysis/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17729 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/line_analysis/tests/test_line_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/line_analysis/tests/test_lineflux.py
--rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.281016 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/unit_conversion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/unit_conversion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.281016 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/unit_conversion/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/unit_conversion/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/unit_conversion/tests/test_unit_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.vue
--rw-r--r--   0 runner    (1001) docker     (123)    22442 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/plugins/viewers.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/specviz.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/specviz.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.281016 jdaviz-3.6.0/jdaviz/configs/specviz/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19884 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz/tests/test_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.281016 jdaviz-3.6.0/jdaviz/configs/specviz2d/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz2d/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.281016 jdaviz-3.6.0/jdaviz/configs/specviz2d/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz2d/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz2d/plugins/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.281016 jdaviz-3.6.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42246 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    16527 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.281016 jdaviz-3.6.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/test_spectral_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz2d/specviz2d.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.285016 jdaviz-3.6.0/jdaviz/configs/specviz2d/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz2d/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz2d/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/configs/specviz2d/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10796 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/container.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.285016 jdaviz-3.6.0/jdaviz/core/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21374 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/astrowidgets_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/custom_traitlets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/data_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     9073 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/freezable_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    40896 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/linelists.py
--rw-r--r--   0 runner    (1001) docker     (123)    25077 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/marks.py
--rw-r--r--   0 runner    (1001) docker     (123)    14822 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/region_translators.py
--rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/registries.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/style_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)   108581 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/template_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.285016 jdaviz-3.6.0/jdaviz/core/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/tests/test_autoconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/tests/test_custom_traitlets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/tests/test_data_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/tests/test_region_translators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/tests/test_template_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    15898 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/core/validunits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.237016 jdaviz-3.6.0/jdaviz/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.293016 jdaviz-3.6.0/jdaviz/data/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/blink.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/checktoradial.svg
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/compass.svg
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/contrast.svg
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/home.svg
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/home_match.svg
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/image.svg
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/left-east.svg
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/line_select.svg
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/line_select_disabled.svg
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/pan.svg
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/pan2.svg
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/pan_x.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/pan_x_match.svg
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/pan_y.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/pan_y_match.svg
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/panzoom_match.svg
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/pixelspectra.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/radialtocheck.svg
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/right-east.svg
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/select_annulus.svg
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/select_circle.svg
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/select_ellipse.svg
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/select_lasso.svg
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/select_single_pixel.svg
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/select_x.svg
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/select_xy.svg
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/select_y.svg
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/slice.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/spectral_range.svg
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/tune.svg
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/zoom_back.svg
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/zoom_box.svg
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/zoom_box_match.svg
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/zoom_xrange.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/zoom_xrange_match.svg
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/zoom_yrange.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/icons/zoom_yrange_match.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.293016 jdaviz-3.6.0/jdaviz/data/linelists/
--rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/Atomic-ISO.csv
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/Atomic-Ionic.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/Atomic-Ionic_FineStructure.csv
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/CO-band-heads.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/CO.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/Common_Galactic_2000A-11000A.csv
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/Common_Galactic_700A-2000A.csv
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/Common_nebular.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/Common_stellar.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/DEV_NOTES.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/H-He.csv
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/H-Paschen-Brackett.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20639 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/H2-ISO.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/H2-alt.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/H2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/HeI-HeII.csv
--rw-r--r--   0 runner    (1001) docker     (123)    21334 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/JWST_line_list_original.txt
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/PAH.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/SDSS-IV.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/SDSS.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/UV_linelist_vacuum.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/data/linelists/linelist_metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/jdaviz_cli.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/jdaviz_cli_launcher.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.293016 jdaviz-3.6.0/jdaviz/models/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/models/physical_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.293016 jdaviz-3.6.0/jdaviz/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/tests/coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/tests/test_data_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    34729 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/tests/test_subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/tests/test_viewer_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)    10834 2023-07-28 18:47:24.000000 jdaviz-3.6.0/jdaviz/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-28 18:47:39.000000 jdaviz-3.6.0/jdaviz/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.245016 jdaviz-3.6.0/jdaviz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-07-28 18:47:40.000000 jdaviz-3.6.0/jdaviz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18571 2023-07-28 18:47:40.000000 jdaviz-3.6.0/jdaviz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 18:47:40.000000 jdaviz-3.6.0/jdaviz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-28 18:47:40.000000 jdaviz-3.6.0/jdaviz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 18:47:40.000000 jdaviz-3.6.0/jdaviz.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-28 18:47:40.000000 jdaviz-3.6.0/jdaviz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-28 18:47:40.000000 jdaviz-3.6.0/jdaviz.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.297016 jdaviz-3.6.0/licenses/
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-28 18:47:24.000000 jdaviz-3.6.0/licenses/GINGA_LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-28 18:47:24.000000 jdaviz-3.6.0/licenses/IMEXAM_LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-28 18:47:24.000000 jdaviz-3.6.0/licenses/IPYFILECHOOSER_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-28 18:47:24.000000 jdaviz-3.6.0/licenses/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-28 18:47:24.000000 jdaviz-3.6.0/licenses/TEMPLATE_LICENCE.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.297016 jdaviz-3.6.0/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/CubevizExample.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    17801 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/ImvizDitheredExample.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    20170 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/ImvizExample.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/MosvizExample.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/MosvizNIRISSExample.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/Specviz2dExample.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/SpecvizExample.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.301016 jdaviz-3.6.0/notebooks/concepts/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/cubeviz_contour_overlay.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9113 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/cubeviz_data_interactions.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/cubeviz_fitting.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/cubeviz_ndarray_gif.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/cubeviz_spectral_fitting.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/cubeviz_spectral_spatial_interactions.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/cubeviz_wfc3ir_ramp.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13949 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/default_programmatic_viewers_from_blank.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/imviz_color_display.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    15370 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/imviz_compass_mpl.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/imviz_custom_colormap.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/imviz_dithered_gwcs.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/imviz_edit_subset_programmatic.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/imviz_line_profiles.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/imviz_load_3d_slices.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/imviz_load_fits_hdu.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14417 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/imviz_roman_asdf.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/imviz_simple_aper_phot.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    20908 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/mosviz_concept.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    33356 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/mosviz_generate_photometry.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/mosviz_niriss_parser.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9903 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/mosviz_overplot_slit.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/pypi_metrics.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/specviz_from_list.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    82825 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/specviz_from_splot.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/specviz_glue_unit_conversion.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/specviz_line_lists.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/specviz_minimal.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-28 18:47:24.000000 jdaviz-3.6.0/notebooks/concepts/specviz_spectrum_list.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-07-28 18:47:24.000000 jdaviz-3.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-28 18:47:40.305017 jdaviz-3.6.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     5534 2023-07-28 18:47:24.000000 jdaviz-3.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.237016 jdaviz-3.6.0/share/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.237016 jdaviz-3.6.0/share/jupyter/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.237016 jdaviz-3.6.0/share/jupyter/nbconvert/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.237016 jdaviz-3.6.0/share/jupyter/nbconvert/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.301016 jdaviz-3.6.0/share/jupyter/nbconvert/templates/jdaviz-default/
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-07-28 18:47:24.000000 jdaviz-3.6.0/share/jupyter/nbconvert/templates/jdaviz-default/ansi.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     3653 2023-07-28 18:47:24.000000 jdaviz-3.6.0/share/jupyter/nbconvert/templates/jdaviz-default/app.html
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 18:47:24.000000 jdaviz-3.6.0/share/jupyter/nbconvert/templates/jdaviz-default/conf.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     3265 2023-07-28 18:47:24.000000 jdaviz-3.6.0/share/jupyter/nbconvert/templates/jdaviz-default/index.html.j2
--rwxr-xr-x   0 runner    (1001) docker     (123)     5993 2023-07-28 18:47:24.000000 jdaviz-3.6.0/share/jupyter/nbconvert/templates/jdaviz-default/util.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.241016 jdaviz-3.6.0/share/jupyter/voila/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.241016 jdaviz-3.6.0/share/jupyter/voila/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.301016 jdaviz-3.6.0/share/jupyter/voila/templates/jdaviz-default/
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-28 18:47:24.000000 jdaviz-3.6.0/share/jupyter/voila/templates/jdaviz-default/index.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.301016 jdaviz-3.6.0/standalone/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-28 18:47:24.000000 jdaviz-3.6.0/standalone/entitlements.plist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:47:40.301016 jdaviz-3.6.0/standalone/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 18:47:24.000000 jdaviz-3.6.0/standalone/hooks/hook-bqplot.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-28 18:47:24.000000 jdaviz-3.6.0/standalone/hooks/hook-debugpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-28 18:47:24.000000 jdaviz-3.6.0/standalone/hooks/hook-glue.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-28 18:47:24.000000 jdaviz-3.6.0/standalone/hooks/hook-glue_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-28 18:47:24.000000 jdaviz-3.6.0/standalone/hooks/hook-ipypopout.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-28 18:47:24.000000 jdaviz-3.6.0/standalone/hooks/hook-jdaviz.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-28 18:47:24.000000 jdaviz-3.6.0/standalone/hooks/hook-jupyter_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-28 18:47:24.000000 jdaviz-3.6.0/standalone/hooks/hook-mistune.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-28 18:47:24.000000 jdaviz-3.6.0/standalone/hooks/hook-photutils.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-28 18:47:24.000000 jdaviz-3.6.0/standalone/hooks/hook-regions.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-28 18:47:24.000000 jdaviz-3.6.0/standalone/hooks/hook-skimage.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-28 18:47:24.000000 jdaviz-3.6.0/standalone/jdaviz-cli-entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-28 18:47:24.000000 jdaviz-3.6.0/standalone/jdaviz.spec
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-28 18:47:24.000000 jdaviz-3.6.0/standalone/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-28 18:47:24.000000 jdaviz-3.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.880448 jdaviz-3.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-01 20:36:28.000000 jdaviz-3.6.1/.bandit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-08-01 20:36:28.000000 jdaviz-3.6.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.776447 jdaviz-3.6.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-01 20:36:28.000000 jdaviz-3.6.1/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.776447 jdaviz-3.6.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-08-01 20:36:28.000000 jdaviz-3.6.1/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-01 20:36:28.000000 jdaviz-3.6.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-08-01 20:36:28.000000 jdaviz-3.6.1/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-08-01 20:36:28.000000 jdaviz-3.6.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-01 20:36:28.000000 jdaviz-3.6.1/.github/labeler.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.776447 jdaviz-3.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-08-01 20:36:28.000000 jdaviz-3.6.1/.github/workflows/changelog_check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-08-01 20:36:28.000000 jdaviz-3.6.1/.github/workflows/ci_cron_weekly.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-08-01 20:36:28.000000 jdaviz-3.6.1/.github/workflows/ci_workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-08-01 20:36:28.000000 jdaviz-3.6.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-08-01 20:36:28.000000 jdaviz-3.6.1/.github/workflows/open_actions.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-08-01 20:36:28.000000 jdaviz-3.6.1/.github/workflows/predeps_workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-08-01 20:36:28.000000 jdaviz-3.6.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-08-01 20:36:28.000000 jdaviz-3.6.1/.github/workflows/standalone.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-08-01 20:36:28.000000 jdaviz-3.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-08-01 20:36:28.000000 jdaviz-3.6.1/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-01 20:36:28.000000 jdaviz-3.6.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    47453 2023-08-01 20:36:28.000000 jdaviz-3.6.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-08-01 20:36:28.000000 jdaviz-3.6.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-08-01 20:36:28.000000 jdaviz-3.6.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-08-01 20:36:28.000000 jdaviz-3.6.1/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-01 20:36:28.000000 jdaviz-3.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-08-01 20:36:48.880448 jdaviz-3.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-08-01 20:36:28.000000 jdaviz-3.6.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-08-01 20:36:28.000000 jdaviz-3.6.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.780447 jdaviz-3.6.1/jdaviz/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/_astropy_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100517 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/app.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.784447 jdaviz-3.6.1/jdaviz/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/components/docs_link.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/components/external_link.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/components/glue_state_sync_wrapper.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/components/layer_viewer_icon.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/components/number_uncertainty.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/components/play_pause_widget.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/components/plugin_add_results.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/components/plugin_auto_label.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/components/plugin_dataset_select.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/components/plugin_layer_select.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/components/plugin_plot.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/components/plugin_popout.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/components/plugin_section_header.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/components/plugin_subset_select.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/components/plugin_table.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/components/plugin_viewer_select.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     8873 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/components/toolbar_nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/components/toolbar_nested.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/components/tooltip.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/components/tray_plugin.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     9425 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/components/viewer_data_select.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/components/viewer_data_select_item.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.784447 jdaviz-3.6.1/jdaviz/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.788447 jdaviz-3.6.1/jdaviz/configs/cubeviz/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/cubeviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/cubeviz/cubeviz.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/cubeviz/cubeviz.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/cubeviz/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.788447 jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.788447 jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/moment_maps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/moment_maps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.788447 jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/moment_maps/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/moment_maps/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/moment_maps/tests/test_moment_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18788 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.788447 jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/slice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/slice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/slice/slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/slice/slice.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.792447 jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/slice/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/slice/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/slice/tests/test_slice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.792447 jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/tests/test_cubeviz_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/tests/test_data_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/tests/test_data_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/tests/test_export_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10258 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/tests/test_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/viewers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.792447 jdaviz-3.6.1/jdaviz/configs/default/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/default.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.792447 jdaviz-3.6.1/jdaviz/configs/default/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.792447 jdaviz-3.6.1/jdaviz/configs/default/plugins/collapse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/collapse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/collapse/collapse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/collapse/collapse.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.792447 jdaviz-3.6.1/jdaviz/configs/default/plugins/collapse/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/collapse/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/collapse/tests/test_collapse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.796447 jdaviz-3.6.1/jdaviz/configs/default/plugins/data_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/data_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/data_tools/data_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/data_tools/data_tools.vue
+-rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/data_tools/file_chooser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.796447 jdaviz-3.6.1/jdaviz/configs/default/plugins/export_plot/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/export_plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/export_plot/export_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/export_plot/export_plot.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.796447 jdaviz-3.6.1/jdaviz/configs/default/plugins/gaussian_smooth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/gaussian_smooth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.796447 jdaviz-3.6.1/jdaviz/configs/default/plugins/gaussian_smooth/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/gaussian_smooth/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/gaussian_smooth/tests/test_gaussian_smooth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.796447 jdaviz-3.6.1/jdaviz/configs/default/plugins/line_lists/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/line_lists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/line_lists/line_list_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35599 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/line_lists/line_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15805 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/line_lists/line_lists.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.796447 jdaviz-3.6.1/jdaviz/configs/default/plugins/line_lists/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/line_lists/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/line_lists/tests/test_line_lists.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.800447 jdaviz-3.6.1/jdaviz/configs/default/plugins/markers/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/markers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/markers/markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/markers/markers.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.800447 jdaviz-3.6.1/jdaviz/configs/default/plugins/markers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/markers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12863 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/markers/tests/test_markers_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.800447 jdaviz-3.6.1/jdaviz/configs/default/plugins/metadata_viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/metadata_viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.800447 jdaviz-3.6.1/jdaviz/configs/default/plugins/metadata_viewer/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/metadata_viewer/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/metadata_viewer/tests/test_metadata_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.800447 jdaviz-3.6.1/jdaviz/configs/default/plugins/model_fitting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/model_fitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13952 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/model_fitting/fitting_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/model_fitting/initializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44507 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/model_fitting/model_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/model_fitting/model_fitting.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.804447 jdaviz-3.6.1/jdaviz/configs/default/plugins/model_fitting/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/model_fitting/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/model_fitting/tests/test_blackbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16096 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/model_fitting/tests/test_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15676 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/model_fitting/tests/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.804447 jdaviz-3.6.1/jdaviz/configs/default/plugins/plot_options/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/plot_options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36881 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/plot_options/plot_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26118 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/plot_options/plot_options.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.804447 jdaviz-3.6.1/jdaviz/configs/default/plugins/plot_options/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/plot_options/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/plot_options/tests/test_plot_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.804447 jdaviz-3.6.1/jdaviz/configs/default/plugins/subset_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/subset_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23109 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.804447 jdaviz-3.6.1/jdaviz/configs/default/plugins/subset_plugin/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/subset_plugin/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/subset_plugin/tests/test_subset_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.804447 jdaviz-3.6.1/jdaviz/configs/default/plugins/subset_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/subset_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/subset_tools/subset_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/subset_tools/subset_tools.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.808447 jdaviz-3.6.1/jdaviz/configs/default/plugins/viewer_creator/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/viewer_creator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.vue
+-rw-r--r--   0 runner    (1001) docker     (123)    10148 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/default/plugins/viewers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.808447 jdaviz-3.6.1/jdaviz/configs/imviz/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19411 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/imviz.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/imviz.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.808447 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.808447 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/aper_phot_simple/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/aper_phot_simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25491 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.808447 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/catalogs/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/catalogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10913 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/catalogs/catalogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/catalogs/catalogs.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.812447 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/compass/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/compass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/compass/compass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/compass/compass.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.812447 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/compass/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/compass/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/compass/tests/test_compass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.812447 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/coords_info/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/coords_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23107 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/coords_info/coords_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/coords_info/coords_info.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.812447 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/image_viewer_creator/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/image_viewer_creator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/image_viewer_creator/image_viewer_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/image_viewer_creator/image_viewer_creator.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.812447 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/line_profile_xy/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/line_profile_xy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.812447 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/links_control/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/links_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/links_control/links_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/links_control/links_control.vue
+-rw-r--r--   0 runner    (1001) docker     (123)    14277 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.812447 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/rotate_canvas/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/rotate_canvas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.812447 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/rotate_canvas/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/rotate_canvas/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/rotate_canvas/tests/test_rotate_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13559 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/plugins/viewers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.816447 jdaviz-3.6.1/jdaviz/configs/imviz/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.816447 jdaviz-3.6.1/jdaviz/configs/imviz/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/tests/data/ds9_annulus_01.reg
+-rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/tests/data/miri_i2d_lonlat_gwcs.asdf
+-rw-r--r--   0 runner    (1001) docker     (123)  8425199 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/tests/data/roman_wfi_image_model.asdf
+-rw-r--r--   0 runner    (1001) docker     (123)    15711 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/tests/test_astrowidgets_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/tests/test_catalogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/tests/test_line_profile_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19474 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/tests/test_linking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/tests/test_links_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25880 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/tests/test_parser_roman.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/tests/test_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16125 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/tests/test_simple_aper_phot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/tests/test_subset_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/tests/test_viewer_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/tests/test_viewers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/tests/test_wcs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9197 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/imviz/wcs_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.836448 jdaviz-3.6.1/jdaviz/configs/mosviz/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/mosviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38346 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/mosviz/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/mosviz/mosviz.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/mosviz/mosviz.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.836448 jdaviz-3.6.1/jdaviz/configs/mosviz/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/mosviz/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40180 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/mosviz/plugins/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.836448 jdaviz-3.6.1/jdaviz/configs/mosviz/plugins/row_lock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/mosviz/plugins/row_lock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/mosviz/plugins/row_lock/row_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/mosviz/plugins/row_lock/row_lock.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.840448 jdaviz-3.6.1/jdaviz/configs/mosviz/plugins/slit_overlay/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/mosviz/plugins/slit_overlay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/mosviz/plugins/slit_overlay/slit_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/mosviz/plugins/slit_overlay/slit_overlay.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.840448 jdaviz-3.6.1/jdaviz/configs/mosviz/plugins/slit_overlay/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/mosviz/plugins/slit_overlay/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/mosviz/plugins/slit_overlay/tests/test_slit_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/mosviz/plugins/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18704 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/mosviz/plugins/viewers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.840448 jdaviz-3.6.1/jdaviz/configs/mosviz/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/mosviz/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10691 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/mosviz/tests/test_data_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/mosviz/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/mosviz/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/mosviz/tests/test_source_identifier_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/mosviz/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.840448 jdaviz-3.6.1/jdaviz/configs/specviz/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/specviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14962 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/specviz/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.840448 jdaviz-3.6.1/jdaviz/configs/specviz/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/specviz/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.844448 jdaviz-3.6.1/jdaviz/configs/specviz/plugins/line_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/specviz/plugins/line_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29328 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.844448 jdaviz-3.6.1/jdaviz/configs/specviz/plugins/line_analysis/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/specviz/plugins/line_analysis/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17729 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/specviz/plugins/line_analysis/tests/test_line_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/specviz/plugins/line_analysis/tests/test_lineflux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/specviz/plugins/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.844448 jdaviz-3.6.1/jdaviz/configs/specviz/plugins/unit_conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/specviz/plugins/unit_conversion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.844448 jdaviz-3.6.1/jdaviz/configs/specviz/plugins/unit_conversion/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/specviz/plugins/unit_conversion/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/specviz/plugins/unit_conversion/tests/test_unit_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.vue
+-rw-r--r--   0 runner    (1001) docker     (123)    22442 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/specviz/plugins/viewers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/specviz/specviz.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/specviz/specviz.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.844448 jdaviz-3.6.1/jdaviz/configs/specviz/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/specviz/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19884 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/specviz/tests/test_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.844448 jdaviz-3.6.1/jdaviz/configs/specviz2d/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/specviz2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/specviz2d/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.844448 jdaviz-3.6.1/jdaviz/configs/specviz2d/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/specviz2d/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/specviz2d/plugins/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.848448 jdaviz-3.6.1/jdaviz/configs/specviz2d/plugins/spectral_extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/specviz2d/plugins/spectral_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42246 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16527 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.848448 jdaviz-3.6.1/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/test_spectral_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/specviz2d/specviz2d.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.848448 jdaviz-3.6.1/jdaviz/configs/specviz2d/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/specviz2d/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/specviz2d/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/configs/specviz2d/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10796 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/container.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.852448 jdaviz-3.6.1/jdaviz/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21374 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/core/astrowidgets_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/core/custom_traitlets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/core/data_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9073 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/core/freezable_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40896 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/core/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/core/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/core/linelists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25077 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/core/marks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14822 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/core/region_translators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/core/registries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/core/style_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)   108581 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/core/template_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.856448 jdaviz-3.6.1/jdaviz/core/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/core/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/core/tests/test_autoconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/core/tests/test_custom_traitlets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/core/tests/test_data_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/core/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/core/tests/test_region_translators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/core/tests/test_template_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/core/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15898 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/core/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/core/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/core/validunits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.772447 jdaviz-3.6.1/jdaviz/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.860448 jdaviz-3.6.1/jdaviz/data/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/blink.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/checktoradial.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/compass.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/contrast.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/home.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/home_match.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/image.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/left-east.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/line_select.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/line_select_disabled.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/pan.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/pan2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/pan_x.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/pan_x_match.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/pan_y.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/pan_y_match.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/panzoom_match.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/pixelspectra.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/radialtocheck.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/right-east.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/select_annulus.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/select_circle.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/select_ellipse.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/select_lasso.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/select_single_pixel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/select_x.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/select_xy.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/select_y.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/slice.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/spectral_range.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/tune.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/zoom_back.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/zoom_box.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/zoom_box_match.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/zoom_xrange.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/zoom_xrange_match.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/zoom_yrange.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/icons/zoom_yrange_match.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.864448 jdaviz-3.6.1/jdaviz/data/linelists/
+-rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/linelists/Atomic-ISO.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/linelists/Atomic-Ionic.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/linelists/Atomic-Ionic_FineStructure.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/linelists/CO-band-heads.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/linelists/CO.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/linelists/Common_Galactic_2000A-11000A.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/linelists/Common_Galactic_700A-2000A.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/linelists/Common_nebular.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/linelists/Common_stellar.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/linelists/DEV_NOTES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/linelists/H-He.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/linelists/H-Paschen-Brackett.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20639 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/linelists/H2-ISO.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/linelists/H2-alt.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/linelists/H2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/linelists/HeI-HeII.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21334 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/linelists/JWST_line_list_original.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/linelists/PAH.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/linelists/SDSS-IV.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/linelists/SDSS.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/linelists/UV_linelist_vacuum.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/data/linelists/linelist_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/jdaviz_cli.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/jdaviz_cli_launcher.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.864448 jdaviz-3.6.1/jdaviz/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/models/physical_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.868448 jdaviz-3.6.1/jdaviz/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/tests/coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/tests/test_data_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34729 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/tests/test_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/tests/test_viewer_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10834 2023-08-01 20:36:28.000000 jdaviz-3.6.1/jdaviz/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-01 20:36:48.000000 jdaviz-3.6.1/jdaviz/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.780447 jdaviz-3.6.1/jdaviz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-08-01 20:36:48.000000 jdaviz-3.6.1/jdaviz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18571 2023-08-01 20:36:48.000000 jdaviz-3.6.1/jdaviz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:36:48.000000 jdaviz-3.6.1/jdaviz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-08-01 20:36:48.000000 jdaviz-3.6.1/jdaviz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:36:48.000000 jdaviz-3.6.1/jdaviz.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-08-01 20:36:48.000000 jdaviz-3.6.1/jdaviz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-01 20:36:48.000000 jdaviz-3.6.1/jdaviz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.868448 jdaviz-3.6.1/licenses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-08-01 20:36:28.000000 jdaviz-3.6.1/licenses/GINGA_LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-08-01 20:36:28.000000 jdaviz-3.6.1/licenses/IMEXAM_LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-08-01 20:36:28.000000 jdaviz-3.6.1/licenses/IPYFILECHOOSER_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-08-01 20:36:28.000000 jdaviz-3.6.1/licenses/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-08-01 20:36:28.000000 jdaviz-3.6.1/licenses/TEMPLATE_LICENCE.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.868448 jdaviz-3.6.1/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/CubevizExample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    17801 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/ImvizDitheredExample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    20170 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/ImvizExample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/MosvizExample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/MosvizNIRISSExample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/Specviz2dExample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/SpecvizExample.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.876448 jdaviz-3.6.1/notebooks/concepts/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/concepts/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/concepts/cubeviz_contour_overlay.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9113 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/concepts/cubeviz_data_interactions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/concepts/cubeviz_fitting.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/concepts/cubeviz_ndarray_gif.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/concepts/cubeviz_spectral_fitting.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/concepts/cubeviz_spectral_spatial_interactions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/concepts/cubeviz_wfc3ir_ramp.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13949 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/concepts/default_programmatic_viewers_from_blank.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/concepts/imviz_color_display.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15370 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/concepts/imviz_compass_mpl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/concepts/imviz_custom_colormap.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/concepts/imviz_dithered_gwcs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/concepts/imviz_edit_subset_programmatic.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/concepts/imviz_line_profiles.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/concepts/imviz_load_3d_slices.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/concepts/imviz_load_fits_hdu.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14417 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/concepts/imviz_roman_asdf.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/concepts/imviz_simple_aper_phot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    20908 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/concepts/mosviz_concept.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    33356 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/concepts/mosviz_generate_photometry.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/concepts/mosviz_niriss_parser.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9903 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/concepts/mosviz_overplot_slit.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/concepts/pypi_metrics.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/concepts/specviz_from_list.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    82825 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/concepts/specviz_from_splot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/concepts/specviz_glue_unit_conversion.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/concepts/specviz_line_lists.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/concepts/specviz_minimal.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-08-01 20:36:28.000000 jdaviz-3.6.1/notebooks/concepts/specviz_spectrum_list.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-08-01 20:36:28.000000 jdaviz-3.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-08-01 20:36:48.880448 jdaviz-3.6.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5534 2023-08-01 20:36:28.000000 jdaviz-3.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.772447 jdaviz-3.6.1/share/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.772447 jdaviz-3.6.1/share/jupyter/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.772447 jdaviz-3.6.1/share/jupyter/nbconvert/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.772447 jdaviz-3.6.1/share/jupyter/nbconvert/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.876448 jdaviz-3.6.1/share/jupyter/nbconvert/templates/jdaviz-default/
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-08-01 20:36:28.000000 jdaviz-3.6.1/share/jupyter/nbconvert/templates/jdaviz-default/ansi.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3653 2023-08-01 20:36:28.000000 jdaviz-3.6.1/share/jupyter/nbconvert/templates/jdaviz-default/app.html
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 20:36:28.000000 jdaviz-3.6.1/share/jupyter/nbconvert/templates/jdaviz-default/conf.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3265 2023-08-01 20:36:28.000000 jdaviz-3.6.1/share/jupyter/nbconvert/templates/jdaviz-default/index.html.j2
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5993 2023-08-01 20:36:28.000000 jdaviz-3.6.1/share/jupyter/nbconvert/templates/jdaviz-default/util.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.772447 jdaviz-3.6.1/share/jupyter/voila/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.772447 jdaviz-3.6.1/share/jupyter/voila/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.876448 jdaviz-3.6.1/share/jupyter/voila/templates/jdaviz-default/
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-08-01 20:36:28.000000 jdaviz-3.6.1/share/jupyter/voila/templates/jdaviz-default/index.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.876448 jdaviz-3.6.1/standalone/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-01 20:36:28.000000 jdaviz-3.6.1/standalone/entitlements.plist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:48.880448 jdaviz-3.6.1/standalone/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-01 20:36:28.000000 jdaviz-3.6.1/standalone/hooks/hook-bqplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-08-01 20:36:28.000000 jdaviz-3.6.1/standalone/hooks/hook-debugpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-01 20:36:28.000000 jdaviz-3.6.1/standalone/hooks/hook-glue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-08-01 20:36:28.000000 jdaviz-3.6.1/standalone/hooks/hook-glue_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-01 20:36:28.000000 jdaviz-3.6.1/standalone/hooks/hook-ipypopout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-01 20:36:28.000000 jdaviz-3.6.1/standalone/hooks/hook-jdaviz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-01 20:36:28.000000 jdaviz-3.6.1/standalone/hooks/hook-jupyter_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-01 20:36:28.000000 jdaviz-3.6.1/standalone/hooks/hook-mistune.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-01 20:36:28.000000 jdaviz-3.6.1/standalone/hooks/hook-photutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-01 20:36:28.000000 jdaviz-3.6.1/standalone/hooks/hook-regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-01 20:36:28.000000 jdaviz-3.6.1/standalone/hooks/hook-skimage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-08-01 20:36:28.000000 jdaviz-3.6.1/standalone/jdaviz-cli-entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-08-01 20:36:28.000000 jdaviz-3.6.1/standalone/jdaviz.spec
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-01 20:36:28.000000 jdaviz-3.6.1/standalone/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-08-01 20:36:28.000000 jdaviz-3.6.1/tox.ini
```

### Comparing `jdaviz-3.6.0/.github/ISSUE_TEMPLATE/bug_report.yaml` & `jdaviz-3.6.1/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/.github/ISSUE_TEMPLATE/feature_request.yaml` & `jdaviz-3.6.1/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/.github/PULL_REQUEST_TEMPLATE.md` & `jdaviz-3.6.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/.github/workflows/changelog_check.yml` & `jdaviz-3.6.1/.github/workflows/changelog_check.yml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/.github/workflows/ci_cron_weekly.yml` & `jdaviz-3.6.1/.github/workflows/ci_cron_weekly.yml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/.github/workflows/ci_workflows.yml` & `jdaviz-3.6.1/.github/workflows/ci_workflows.yml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/.github/workflows/codeql-analysis.yml` & `jdaviz-3.6.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/.github/workflows/open_actions.yml` & `jdaviz-3.6.1/.github/workflows/open_actions.yml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/.github/workflows/predeps_workflows.yml` & `jdaviz-3.6.1/.github/workflows/predeps_workflows.yml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/.github/workflows/publish.yml` & `jdaviz-3.6.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/.github/workflows/standalone.yml` & `jdaviz-3.6.1/.github/workflows/standalone.yml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/.gitignore` & `jdaviz-3.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/.mailmap` & `jdaviz-3.6.1/.mailmap`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/.readthedocs.yaml` & `jdaviz-3.6.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/CHANGES.rst` & `jdaviz-3.6.1/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+3.6.1 (2023-08-01)
+==================
+
+Bug Fixes
+---------
+
+Imviz
+^^^^^
+
+- Fixes possible extreme lag when opening the Plot Options plugin. [#2326]
+
+- Fixes minor layout issues in the Plot Options plugin. [#2326]
+
+- Fixes compass updating in popout/inline mode. [#2326]
+
 3.6 (2023-07-28)
 ================
 
 New Features
 ------------
 
 - Introduce jdaviz.open to automatically detect the appropriate config and load data [#2221]
```

### Comparing `jdaviz-3.6.0/CITATION.cff` & `jdaviz-3.6.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/CODE_OF_CONDUCT.md` & `jdaviz-3.6.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/LICENSE.rst` & `jdaviz-3.6.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/PKG-INFO` & `jdaviz-3.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jdaviz
-Version: 3.6.0
+Version: 3.6.1
 Summary: Astronomical data analysis development leveraging the Jupyter platform
 Home-page: https://jdaviz.readthedocs.io/en/latest/
 Author: JDADF Developers
 Author-email: JDADF Developers <help@stsci.edu>
 Project-URL: Homepage, https://jdaviz.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
```

### Comparing `jdaviz-3.6.0/README.rst` & `jdaviz-3.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/conftest.py` & `jdaviz-3.6.1/conftest.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/__init__.py` & `jdaviz-3.6.1/jdaviz/__init__.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/_astropy_init.py` & `jdaviz-3.6.1/jdaviz/_astropy_init.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/app.py` & `jdaviz-3.6.1/jdaviz/app.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/app.vue` & `jdaviz-3.6.1/jdaviz/app.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/cli.py` & `jdaviz-3.6.1/jdaviz/cli.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/components/docs_link.vue` & `jdaviz-3.6.1/jdaviz/components/docs_link.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/components/glue_state_sync_wrapper.vue` & `jdaviz-3.6.1/jdaviz/components/glue_state_sync_wrapper.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/components/layer_viewer_icon.vue` & `jdaviz-3.6.1/jdaviz/components/layer_viewer_icon.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/components/number_uncertainty.vue` & `jdaviz-3.6.1/jdaviz/components/number_uncertainty.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/components/play_pause_widget.vue` & `jdaviz-3.6.1/jdaviz/components/play_pause_widget.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/components/plugin_add_results.vue` & `jdaviz-3.6.1/jdaviz/components/plugin_add_results.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/components/plugin_auto_label.vue` & `jdaviz-3.6.1/jdaviz/components/plugin_auto_label.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/components/plugin_dataset_select.vue` & `jdaviz-3.6.1/jdaviz/components/plugin_dataset_select.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/components/plugin_layer_select.vue` & `jdaviz-3.6.1/jdaviz/components/plugin_layer_select.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/components/plugin_plot.vue` & `jdaviz-3.6.1/jdaviz/components/plugin_plot.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/components/plugin_section_header.vue` & `jdaviz-3.6.1/jdaviz/components/plugin_section_header.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/components/plugin_subset_select.vue` & `jdaviz-3.6.1/jdaviz/components/plugin_subset_select.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/components/plugin_table.vue` & `jdaviz-3.6.1/jdaviz/components/plugin_table.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/components/plugin_viewer_select.vue` & `jdaviz-3.6.1/jdaviz/components/plugin_viewer_select.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/components/toolbar_nested.py` & `jdaviz-3.6.1/jdaviz/components/toolbar_nested.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/components/toolbar_nested.vue` & `jdaviz-3.6.1/jdaviz/components/toolbar_nested.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/components/tooltip.vue` & `jdaviz-3.6.1/jdaviz/components/tooltip.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/components/tray_plugin.vue` & `jdaviz-3.6.1/jdaviz/components/tray_plugin.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/components/viewer_data_select.vue` & `jdaviz-3.6.1/jdaviz/components/viewer_data_select.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/components/viewer_data_select_item.vue` & `jdaviz-3.6.1/jdaviz/components/viewer_data_select_item.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/cubeviz/cubeviz.ipynb` & `jdaviz-3.6.1/jdaviz/configs/cubeviz/cubeviz.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/cubeviz/cubeviz.yaml` & `jdaviz-3.6.1/jdaviz/configs/cubeviz/cubeviz.yaml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/cubeviz/helper.py` & `jdaviz-3.6.1/jdaviz/configs/cubeviz/helper.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.py` & `jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.vue` & `jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/moment_maps/tests/test_moment_maps.py` & `jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/moment_maps/tests/test_moment_maps.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/parsers.py` & `jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/parsers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/slice/slice.py` & `jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/slice/slice.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/slice/slice.vue` & `jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/slice/slice.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/slice/tests/test_slice.py` & `jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/slice/tests/test_slice.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/tests/test_cubeviz_helper.py` & `jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/tests/test_cubeviz_helper.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/tests/test_data_retrieval.py` & `jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/tests/test_data_retrieval.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/tests/test_data_selection.py` & `jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/tests/test_data_selection.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/tests/test_export_plots.py` & `jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/tests/test_export_plots.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/tests/test_parsers.py` & `jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/tests/test_regions.py` & `jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/tests/test_regions.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/tests/test_tools.py` & `jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/tools.py` & `jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/cubeviz/plugins/viewers.py` & `jdaviz-3.6.1/jdaviz/configs/cubeviz/plugins/viewers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/default.ipynb` & `jdaviz-3.6.1/jdaviz/configs/default/default.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/__init__.py` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/collapse/collapse.py` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/collapse/collapse.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/collapse/collapse.vue` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/collapse/collapse.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/collapse/tests/test_collapse.py` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/collapse/tests/test_collapse.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/data_tools/data_tools.py` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/data_tools/data_tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/data_tools/data_tools.vue` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/data_tools/data_tools.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/data_tools/file_chooser.py` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/data_tools/file_chooser.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/export_plot/export_plot.py` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/export_plot/export_plot.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/export_plot/export_plot.vue` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/export_plot/export_plot.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.py` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.vue` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/gaussian_smooth/tests/test_gaussian_smooth.py` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/gaussian_smooth/tests/test_gaussian_smooth.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/line_lists/line_list_mixin.py` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/line_lists/line_list_mixin.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/line_lists/line_lists.py` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/line_lists/line_lists.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/line_lists/line_lists.vue` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/line_lists/line_lists.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/line_lists/tests/test_line_lists.py` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/line_lists/tests/test_line_lists.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/markers/markers.py` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/markers/markers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/markers/markers.vue` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/markers/markers.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/markers/tests/test_markers_plugin.py` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/markers/tests/test_markers_plugin.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.py` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.vue` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/metadata_viewer/tests/test_metadata_viewer.py` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/metadata_viewer/tests/test_metadata_viewer.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/fitting_backend.py` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/model_fitting/fitting_backend.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/initializers.py` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/model_fitting/initializers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/model_fitting.py` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/model_fitting/model_fitting.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/model_fitting.vue` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/model_fitting/model_fitting.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/tests/test_blackbody.py` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/model_fitting/tests/test_blackbody.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/tests/test_fitting.py` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/model_fitting/tests/test_fitting.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import warnings
 
 import numpy as np
 import pytest
 from astropy import units as u
 from astropy.io import fits
 from astropy.io.registry.base import IORegistryError
-from astropy.modeling import models, parameters as params
+from astropy.modeling import models
 from astropy.nddata import StdDevUncertainty
 from astropy.tests.helper import assert_quantity_allclose
 from astropy.wcs import WCS
 from numpy.testing import assert_allclose, assert_array_equal
 from specutils.spectra import Spectrum1D
 
 from jdaviz.configs.default.plugins.model_fitting import fitting_backend as fb
@@ -203,30 +203,30 @@
     # Fit to all spaxels.
     with warnings.catch_warnings():
         warnings.filterwarnings("ignore", message=r"The fit may be unsuccessful.*")
         fitted_parameters, fitted_spectrum = fb.fit_model_to_spectrum(
             spectrum, model_list, expression, n_cpu=n_cpu)
 
     # Check that parameter results are formatted as expected.
-    assert type(fitted_parameters) == list
+    assert isinstance(fitted_parameters, list)
     assert len(fitted_parameters) == IMAGE_SIZE_X * IMAGE_SIZE_Y
 
     for m in fitted_parameters:
         if m['x'] == 3 and m['y'] == 2:
             fitted_model = m['model']
 
-    assert type(fitted_model[0].amplitude.value) == np.float64
+    assert isinstance(fitted_model[0].amplitude.value, np.float64)
     assert fitted_model[0].amplitude.unit == u.Jy
 
-    assert type(fitted_model[0] == params.Parameter)
-    assert type(fitted_model[0].mean.value) == np.float64
+    assert isinstance(fitted_model[0], models.Gaussian1D)
+    assert isinstance(fitted_model[0].mean.value, np.float64)
     assert fitted_model[0].mean.unit == u.um
 
     # Check that spectrum result is formatted as expected.
-    assert type(fitted_spectrum) == Spectrum1D
+    assert isinstance(fitted_spectrum, Spectrum1D)
     assert len(fitted_spectrum.shape) == 3
     assert fitted_spectrum.shape == (IMAGE_SIZE_X, IMAGE_SIZE_Y, SPECTRUM_SIZE)
     assert fitted_spectrum.flux.unit == u.Jy
     assert not np.all(fitted_spectrum.flux.value == 0)
 
     # The important point here isn't to check the accuracy of the
     # fit, which was already tested elsewhere. We are mostly
```

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/model_fitting/tests/test_plugin.py` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/model_fitting/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/plot_options/plot_options.py` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/plot_options/plot_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,14 +248,20 @@
 
     icon_radialtocheck = Unicode(read_icon(os.path.join(ICON_DIR, 'radialtocheck.svg'), 'svg+xml')).tag(sync=True)  # noqa
     icon_checktoradial = Unicode(read_icon(os.path.join(ICON_DIR, 'checktoradial.svg'), 'svg+xml')).tag(sync=True)  # noqa
 
     show_viewer_labels = Bool(True).tag(sync=True)
 
     def __init__(self, *args, **kwargs):
+        # track whether the stretch histogram needs an update (some entry has changed) if is_active
+        # becomes True, to address potential lag from a backlog of calls to
+        # _update_stretch_histogram if the browser throttles pings
+        # (https://github.com/spacetelescope/jdaviz/issues/2317)
+        self._stretch_histogram_needs_update = True
+
         super().__init__(*args, **kwargs)
         self.viewer = ViewerSelect(self, 'viewer_items', 'viewer_selected', 'multiselect')
         self.layer = LayerSelect(self, 'layer_items', 'layer_selected', 'viewer_selected', 'multiselect')  # noqa
 
         def is_profile(state):
             return isinstance(state, (ProfileViewerState, ProfileLayerState))
 
@@ -484,43 +490,59 @@
         attr_name = data.get('name')
         value = data.get('value')
         setattr(self, attr_name, value)
 
     @observe('is_active', 'layer_selected', 'viewer_selected',
              'stretch_hist_zoom_limits')
     def _update_stretch_histogram(self, msg={}):
-        # Import here to prevent circular import.
-        from jdaviz.configs.imviz.plugins.viewers import ImvizImageView
-        from jdaviz.configs.cubeviz.plugins.viewers import CubevizImageView
-
-        if not self.stretch_function_sync.get('in_subscribed_states'):  # pragma: no cover
-            # no (image) viewer with stretch function options
-            return
         if not hasattr(self, 'viewer'):  # pragma: no cover
             # plugin hasn't been fully initialized yet
             return
-        if (not self.is_active
-                or not self.viewer.selected
-                or not self.layer.selected):  # pragma: no cover
-            # no need to make updates, updates will be redrawn when plugin is opened
-            # NOTE: this won't update when the plugin is shown but not open in the tray
-            return
-        if not isinstance(msg, dict) and not self.stretch_hist_zoom_limits:  # pragma: no cover
-            # then this is from the limits callbacks and we don't want to waste resources
+
+        if not isinstance(msg, dict):  # pragma: no cover
+            # then this is from the limits callbacks
             # IMPORTANT: this assumes the only non-observe callback to this method comes
             # from state callbacks from zoom limits.
+            if not self.stretch_hist_zoom_limits:
+                # there isn't anything to update, let's not waste resources
+                return
+            # override msg as an empty dict so that the rest of the logic doesn't have to check
+            # its type
+            msg = {}
+
+        if msg.get('name', None) == 'is_active' and not self._stretch_histogram_needs_update:
+            # this could be re-triggering if the browser is throttling pings on the js-side
+            # and since this is expensive, could result in laggy behavior
+            return
+        elif msg.get('name', None) != 'is_active' and not self.is_active:
+            # next time is_active becomes True, we need to update the histogram plot
+            self._stretch_histogram_needs_update = True
+            return
+
+        if not self.stretch_function_sync.get('in_subscribed_states'):  # pragma: no cover
+            # no (image) viewer with stretch function options
+            return
+
+        if (not self.viewer.selected or not self.layer.selected):  # pragma: no cover
+            # nothing to plot
+            self.stretch_histogram.clear_all_marks()
             return
 
         if self.multiselect and (len(self.viewer.selected) > 1
                                  or len(self.layer.selected) > 1):  # pragma: no cover
             # currently only support single-layer/viewer.  For now we'll just clear and return.
             # TODO: add support for multi-layer/viewer
             bqplot_clear_figure(self.stretch_histogram)
             return
 
+        # Import here to prevent circular import (and not at the top of the method so the import
+        # check is avoided, whenever possible).
+        from jdaviz.configs.imviz.plugins.viewers import ImvizImageView
+        from jdaviz.configs.cubeviz.plugins.viewers import CubevizImageView
+
         if not isinstance(self.viewer.selected_obj, (ImvizImageView, CubevizImageView)):
             # don't update histogram if selected viewer is not an image viewer:
             return
 
         viewer = self.viewer.selected_obj[0] if self.multiselect else self.viewer.selected_obj
 
         # manage viewer zoom limit callbacks
@@ -542,14 +564,15 @@
             data = self.layer.selected_obj[0].layer
         else:
             # skip further updates if no data are available:
             return
 
         comp = data.get_component(data.main_components[0])
 
+        # TODO: further optimization could be done by caching sub_data
         if self.stretch_hist_zoom_limits:
             if hasattr(viewer, '_get_zoom_limits'):
                 # Viewer limits. This takes account of Imviz linking.
                 xy_limits = viewer._get_zoom_limits(data).astype(int)
                 x_limits = xy_limits[:, 0]
                 y_limits = xy_limits[:, 1]
                 x_min = max(x_limits.min(), 0)
@@ -614,14 +637,15 @@
 
         interval = PercentileInterval(95)
         if len(sub_data) > 0:
             hist_lims = interval.get_limits(sub_data)
             hist_mark.min, hist_mark.max = hist_lims
 
         self._check_if_v_stretch_changed()
+        self._stretch_histogram_needs_update = False
 
     @observe('stretch_vmin_value', 'stretch_vmax_value')
     def _check_if_v_stretch_changed(self, msg=None):
         self._remove_histogram_marks()
         self._add_histogram_marks()
 
     def _add_histogram_marks(self):
```

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/plot_options/plot_options.vue` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/plot_options/plot_options.vue`

 * *Files 0% similar despite different names*

```diff
@@ -344,36 +344,41 @@
       <glue-float-field label="Stretch VMin" :value.sync="stretch_vmin_value" />
     </glue-state-sync-wrapper>
 
     <glue-state-sync-wrapper :sync="stretch_vmax_sync" :multiselect="multiselect" @unmix-state="unmix_state('stretch_vmax')">
       <glue-float-field label="Stretch VMax" :value.sync="stretch_vmax_value" />
     </glue-state-sync-wrapper>
 
-    <v-row v-if="stretch_function_sync.in_subscribed_states">
-      <!-- z-index to ensure on top of the jupyter widget with negative margin-top -->
-      <v-text-field
-          ref="stretch_hist_nbins"
-          type="number"
-          label="Number of Bins"
-          v-model.number="stretch_hist_nbins"
-          hint="The amount of bins used in the histogram."
-          persistent-hint
-          :rules="[() => stretch_hist_nbins !== '' || 'This field is required',
-                   () => stretch_hist_nbins > 0 || 'Number of Bins must be greater than zero']"
-      ></v-text-field>
-      <v-switch
-        v-model="stretch_hist_zoom_limits"
-        class="hide-input"
-        label="Limit histogram to current zoom limits"
-        style="z-index: 1"
-      ></v-switch>
-      <!-- NOTE: height defined here should match that in the custom CSS rules
-           below for the bqplot class -->
+    <div v-if="stretch_function_sync.in_subscribed_states">
+      <v-row>
+        <v-text-field
+            ref="stretch_hist_nbins"
+            type="number"
+            label="Number of Bins"
+            v-model.number="stretch_hist_nbins"
+            hint="The amount of bins used in the histogram."
+            persistent-hint
+            :rules="[() => stretch_hist_nbins !== '' || 'This field is required',
+                     () => stretch_hist_nbins > 0 || 'Number of Bins must be greater than zero']"
+        ></v-text-field>
+      </v-row>
+      <v-row>
+        <!-- z-index to ensure on top of the jupyter widget with negative margin-top -->
+        <v-switch
+          v-model="stretch_hist_zoom_limits"
+          class="hide-input"
+          label="Limit histogram to current zoom limits"
+          style="z-index: 1"
+        ></v-switch>
+        <!-- NOTE: height defined here should match that in the custom CSS rules
+             below for the bqplot class -->
+      </v-row>
       <jupyter-widget :widget="stretch_histogram" class="stretch-hist" style="width: 100%; height: 320px; margin-top: -60px; margin-bottom: -40px" />
-    </v-row>
+    </div>
+ 
 
     <!-- IMAGE:IMAGE -->
     <j-plugin-section-header v-if="image_visible_sync.in_subscribed_states">Image</j-plugin-section-header>
     <glue-state-sync-wrapper :sync="image_visible_sync" :multiselect="multiselect" @unmix-state="unmix_state('image_visible')">
       <span>
         <v-btn icon @click.stop="image_visible_value = !image_visible_value">
           <v-icon>mdi-eye{{ image_visible_value ? '' : '-off' }}</v-icon>
```

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/plot_options/tests/test_plot_options.py` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/plot_options/tests/test_plot_options.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.py` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.vue` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/subset_plugin/tests/test_subset_plugin.py` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/subset_plugin/tests/test_subset_plugin.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/subset_tools/subset_tools.py` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/subset_tools/subset_tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.py` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.vue` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/default/plugins/viewers.py` & `jdaviz-3.6.1/jdaviz/configs/default/plugins/viewers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/helper.py` & `jdaviz-3.6.1/jdaviz/configs/imviz/helper.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/imviz.ipynb` & `jdaviz-3.6.1/jdaviz/configs/imviz/imviz.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/imviz.yaml` & `jdaviz-3.6.1/jdaviz/configs/imviz/imviz.yaml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.py` & `jdaviz-3.6.1/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.vue` & `jdaviz-3.6.1/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/catalogs/catalogs.py` & `jdaviz-3.6.1/jdaviz/configs/imviz/plugins/catalogs/catalogs.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/catalogs/catalogs.vue` & `jdaviz-3.6.1/jdaviz/configs/imviz/plugins/catalogs/catalogs.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/compass/compass.py` & `jdaviz-3.6.1/jdaviz/configs/imviz/plugins/compass/compass.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,17 +61,20 @@
 
     @observe("viewer_selected", "is_active")
     def _compass_with_new_viewer(self, *args, **kwargs):
         if not hasattr(self, 'viewer'):
             # mixin object not yet initialized
             return
 
+        if not self.is_active:
+            return
+
         # There can be only one!
         for vid, viewer in self.app._viewer_store.items():
-            if vid == self.viewer.selected_id and self.plugin_opened:
+            if vid == self.viewer.selected_id:
                 viewer.compass = self
                 viewer.on_limits_change()  # Force redraw
 
                 self._set_compass_rotation()
             else:
                 viewer.compass = None
```

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/compass/compass.vue` & `jdaviz-3.6.1/jdaviz/configs/imviz/plugins/compass/compass.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/coords_info/coords_info.py` & `jdaviz-3.6.1/jdaviz/configs/imviz/plugins/coords_info/coords_info.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/coords_info/coords_info.vue` & `jdaviz-3.6.1/jdaviz/configs/imviz/plugins/coords_info/coords_info.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/image_viewer_creator/image_viewer_creator.py` & `jdaviz-3.6.1/jdaviz/configs/imviz/plugins/image_viewer_creator/image_viewer_creator.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.py` & `jdaviz-3.6.1/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.vue` & `jdaviz-3.6.1/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/links_control/links_control.py` & `jdaviz-3.6.1/jdaviz/configs/imviz/plugins/links_control/links_control.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/links_control/links_control.vue` & `jdaviz-3.6.1/jdaviz/configs/imviz/plugins/links_control/links_control.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/parsers.py` & `jdaviz-3.6.1/jdaviz/configs/imviz/plugins/parsers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.py` & `jdaviz-3.6.1/jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.vue` & `jdaviz-3.6.1/jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/rotate_canvas/tests/test_rotate_canvas.py` & `jdaviz-3.6.1/jdaviz/configs/imviz/plugins/rotate_canvas/tests/test_rotate_canvas.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/tools.py` & `jdaviz-3.6.1/jdaviz/configs/imviz/plugins/tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/plugins/viewers.py` & `jdaviz-3.6.1/jdaviz/configs/imviz/plugins/viewers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/tests/data/miri_i2d_lonlat_gwcs.asdf` & `jdaviz-3.6.1/jdaviz/configs/imviz/tests/data/miri_i2d_lonlat_gwcs.asdf`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/tests/data/roman_wfi_image_model.asdf` & `jdaviz-3.6.1/jdaviz/configs/imviz/tests/data/roman_wfi_image_model.asdf`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_astrowidgets_api.py` & `jdaviz-3.6.1/jdaviz/configs/imviz/tests/test_astrowidgets_api.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_catalogs.py` & `jdaviz-3.6.1/jdaviz/configs/imviz/tests/test_catalogs.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_helper.py` & `jdaviz-3.6.1/jdaviz/configs/imviz/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_line_profile_xy.py` & `jdaviz-3.6.1/jdaviz/configs/imviz/tests/test_line_profile_xy.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_linking.py` & `jdaviz-3.6.1/jdaviz/configs/imviz/tests/test_linking.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_links_control.py` & `jdaviz-3.6.1/jdaviz/configs/imviz/tests/test_links_control.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_parser.py` & `jdaviz-3.6.1/jdaviz/configs/imviz/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_parser_roman.py` & `jdaviz-3.6.1/jdaviz/configs/imviz/tests/test_parser_roman.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_regions.py` & `jdaviz-3.6.1/jdaviz/configs/imviz/tests/test_regions.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_simple_aper_phot.py` & `jdaviz-3.6.1/jdaviz/configs/imviz/tests/test_simple_aper_phot.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_subset_centroid.py` & `jdaviz-3.6.1/jdaviz/configs/imviz/tests/test_subset_centroid.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_tools.py` & `jdaviz-3.6.1/jdaviz/configs/imviz/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_viewer_tools.py` & `jdaviz-3.6.1/jdaviz/configs/imviz/tests/test_viewer_tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_viewers.py` & `jdaviz-3.6.1/jdaviz/configs/imviz/tests/test_viewers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/tests/test_wcs_utils.py` & `jdaviz-3.6.1/jdaviz/configs/imviz/tests/test_wcs_utils.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/tests/utils.py` & `jdaviz-3.6.1/jdaviz/configs/imviz/tests/utils.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/imviz/wcs_utils.py` & `jdaviz-3.6.1/jdaviz/configs/imviz/wcs_utils.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/mosviz/helper.py` & `jdaviz-3.6.1/jdaviz/configs/mosviz/helper.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/mosviz/mosviz.ipynb` & `jdaviz-3.6.1/jdaviz/configs/mosviz/mosviz.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/mosviz/mosviz.yaml` & `jdaviz-3.6.1/jdaviz/configs/mosviz/mosviz.yaml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/parsers.py` & `jdaviz-3.6.1/jdaviz/configs/mosviz/plugins/parsers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/row_lock/row_lock.py` & `jdaviz-3.6.1/jdaviz/configs/mosviz/plugins/row_lock/row_lock.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/slit_overlay/slit_overlay.py` & `jdaviz-3.6.1/jdaviz/configs/mosviz/plugins/slit_overlay/slit_overlay.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/slit_overlay/tests/test_slit_overlay.py` & `jdaviz-3.6.1/jdaviz/configs/mosviz/plugins/slit_overlay/tests/test_slit_overlay.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/tools.py` & `jdaviz-3.6.1/jdaviz/configs/mosviz/plugins/tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/mosviz/plugins/viewers.py` & `jdaviz-3.6.1/jdaviz/configs/mosviz/plugins/viewers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/mosviz/tests/test_data_loading.py` & `jdaviz-3.6.1/jdaviz/configs/mosviz/tests/test_data_loading.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/mosviz/tests/test_helper.py` & `jdaviz-3.6.1/jdaviz/configs/mosviz/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/mosviz/tests/test_parsers.py` & `jdaviz-3.6.1/jdaviz/configs/mosviz/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/mosviz/tests/test_source_identifier_extract.py` & `jdaviz-3.6.1/jdaviz/configs/mosviz/tests/test_source_identifier_extract.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/mosviz/tests/test_tools.py` & `jdaviz-3.6.1/jdaviz/configs/mosviz/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/specviz/helper.py` & `jdaviz-3.6.1/jdaviz/configs/specviz/helper.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.py` & `jdaviz-3.6.1/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.vue` & `jdaviz-3.6.1/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/specviz/plugins/line_analysis/tests/test_line_analysis.py` & `jdaviz-3.6.1/jdaviz/configs/specviz/plugins/line_analysis/tests/test_line_analysis.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/specviz/plugins/line_analysis/tests/test_lineflux.py` & `jdaviz-3.6.1/jdaviz/configs/specviz/plugins/line_analysis/tests/test_lineflux.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/specviz/plugins/parsers.py` & `jdaviz-3.6.1/jdaviz/configs/specviz/plugins/parsers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/specviz/plugins/unit_conversion/tests/test_unit_conversion.py` & `jdaviz-3.6.1/jdaviz/configs/specviz/plugins/unit_conversion/tests/test_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.py` & `jdaviz-3.6.1/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.vue` & `jdaviz-3.6.1/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/specviz/plugins/viewers.py` & `jdaviz-3.6.1/jdaviz/configs/specviz/plugins/viewers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/specviz/specviz.ipynb` & `jdaviz-3.6.1/jdaviz/configs/specviz/specviz.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/specviz/specviz.yaml` & `jdaviz-3.6.1/jdaviz/configs/specviz/specviz.yaml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/specviz/tests/test_helper.py` & `jdaviz-3.6.1/jdaviz/configs/specviz/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/specviz2d/helper.py` & `jdaviz-3.6.1/jdaviz/configs/specviz2d/helper.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/specviz2d/plugins/parsers.py` & `jdaviz-3.6.1/jdaviz/configs/specviz2d/plugins/parsers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.py` & `jdaviz-3.6.1/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.vue` & `jdaviz-3.6.1/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/test_spectral_extraction.py` & `jdaviz-3.6.1/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/test_spectral_extraction.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/specviz2d/specviz2d.yaml` & `jdaviz-3.6.1/jdaviz/configs/specviz2d/specviz2d.yaml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/specviz2d/tests/test_helper.py` & `jdaviz-3.6.1/jdaviz/configs/specviz2d/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/configs/specviz2d/tests/test_parsers.py` & `jdaviz-3.6.1/jdaviz/configs/specviz2d/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/conftest.py` & `jdaviz-3.6.1/jdaviz/conftest.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/container.vue` & `jdaviz-3.6.1/jdaviz/container.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/core/astrowidgets_api.py` & `jdaviz-3.6.1/jdaviz/core/astrowidgets_api.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/core/config.py` & `jdaviz-3.6.1/jdaviz/core/config.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/core/custom_traitlets.py` & `jdaviz-3.6.1/jdaviz/core/custom_traitlets.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/core/data_formats.py` & `jdaviz-3.6.1/jdaviz/core/data_formats.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/core/events.py` & `jdaviz-3.6.1/jdaviz/core/events.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/core/freezable_state.py` & `jdaviz-3.6.1/jdaviz/core/freezable_state.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/core/helpers.py` & `jdaviz-3.6.1/jdaviz/core/helpers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/core/launcher.py` & `jdaviz-3.6.1/jdaviz/core/launcher.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/core/linelists.py` & `jdaviz-3.6.1/jdaviz/core/linelists.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/core/marks.py` & `jdaviz-3.6.1/jdaviz/core/marks.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/core/region_translators.py` & `jdaviz-3.6.1/jdaviz/core/region_translators.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/core/registries.py` & `jdaviz-3.6.1/jdaviz/core/registries.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/core/template_mixin.py` & `jdaviz-3.6.1/jdaviz/core/template_mixin.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/core/tests/test_autoconfig.py` & `jdaviz-3.6.1/jdaviz/core/tests/test_autoconfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,9 +33,9 @@
             download_path = str(Path(tempdir) / Path(uri).name)
             Observations.download_file(uri, local_path=download_path)
         elif uri.startswith("http"):
             download_path = download_file(uri, cache=True, timeout=100)
 
         viz_helper = jdaviz_open(download_path, show=False)
 
-        assert type(viz_helper) == helper_class
+        assert isinstance(viz_helper, helper_class)
         assert len(viz_helper.app.data_collection) > 0
```

### Comparing `jdaviz-3.6.0/jdaviz/core/tests/test_custom_traitlets.py` & `jdaviz-3.6.1/jdaviz/core/tests/test_custom_traitlets.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/core/tests/test_data_menu.py` & `jdaviz-3.6.1/jdaviz/core/tests/test_data_menu.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/core/tests/test_helpers.py` & `jdaviz-3.6.1/jdaviz/core/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/core/tests/test_region_translators.py` & `jdaviz-3.6.1/jdaviz/core/tests/test_region_translators.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/core/tests/test_template_mixin.py` & `jdaviz-3.6.1/jdaviz/core/tests/test_template_mixin.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/core/tests/test_tools.py` & `jdaviz-3.6.1/jdaviz/core/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/core/tools.py` & `jdaviz-3.6.1/jdaviz/core/tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/core/user_api.py` & `jdaviz-3.6.1/jdaviz/core/user_api.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/core/validunits.py` & `jdaviz-3.6.1/jdaviz/core/validunits.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/icons/checktoradial.svg` & `jdaviz-3.6.1/jdaviz/data/icons/checktoradial.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/icons/compass.svg` & `jdaviz-3.6.1/jdaviz/data/icons/compass.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/icons/home_match.svg` & `jdaviz-3.6.1/jdaviz/data/icons/home_match.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/icons/line_select.svg` & `jdaviz-3.6.1/jdaviz/data/icons/line_select.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/icons/line_select_disabled.svg` & `jdaviz-3.6.1/jdaviz/data/icons/line_select_disabled.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/icons/pan.svg` & `jdaviz-3.6.1/jdaviz/data/icons/pan.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/icons/pan2.svg` & `jdaviz-3.6.1/jdaviz/data/icons/pan2.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/icons/pan_x_match.svg` & `jdaviz-3.6.1/jdaviz/data/icons/pan_x_match.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/icons/pan_y_match.svg` & `jdaviz-3.6.1/jdaviz/data/icons/pan_y_match.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/icons/panzoom_match.svg` & `jdaviz-3.6.1/jdaviz/data/icons/panzoom_match.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/icons/pixelspectra.svg` & `jdaviz-3.6.1/jdaviz/data/icons/pixelspectra.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/icons/radialtocheck.svg` & `jdaviz-3.6.1/jdaviz/data/icons/radialtocheck.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/icons/select_annulus.svg` & `jdaviz-3.6.1/jdaviz/data/icons/select_annulus.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/icons/select_circle.svg` & `jdaviz-3.6.1/jdaviz/data/icons/select_circle.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/icons/select_ellipse.svg` & `jdaviz-3.6.1/jdaviz/data/icons/select_ellipse.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/icons/select_lasso.svg` & `jdaviz-3.6.1/jdaviz/data/icons/select_lasso.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/icons/select_single_pixel.svg` & `jdaviz-3.6.1/jdaviz/data/icons/select_single_pixel.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/icons/select_xy.svg` & `jdaviz-3.6.1/jdaviz/data/icons/select_xy.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/icons/slice.svg` & `jdaviz-3.6.1/jdaviz/data/icons/slice.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/icons/spectral_range.svg` & `jdaviz-3.6.1/jdaviz/data/icons/spectral_range.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/icons/zoom_box_match.svg` & `jdaviz-3.6.1/jdaviz/data/icons/zoom_box_match.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/icons/zoom_xrange.svg` & `jdaviz-3.6.1/jdaviz/data/icons/zoom_xrange.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/icons/zoom_xrange_match.svg` & `jdaviz-3.6.1/jdaviz/data/icons/zoom_xrange_match.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/icons/zoom_yrange.svg` & `jdaviz-3.6.1/jdaviz/data/icons/zoom_yrange.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/icons/zoom_yrange_match.svg` & `jdaviz-3.6.1/jdaviz/data/icons/zoom_yrange_match.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/linelists/Atomic-ISO.csv` & `jdaviz-3.6.1/jdaviz/data/linelists/Atomic-ISO.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/linelists/Atomic-Ionic.csv` & `jdaviz-3.6.1/jdaviz/data/linelists/Atomic-Ionic.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/linelists/Atomic-Ionic_FineStructure.csv` & `jdaviz-3.6.1/jdaviz/data/linelists/Atomic-Ionic_FineStructure.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/linelists/CO.csv` & `jdaviz-3.6.1/jdaviz/data/linelists/CO.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/linelists/Common_Galactic_2000A-11000A.csv` & `jdaviz-3.6.1/jdaviz/data/linelists/Common_Galactic_2000A-11000A.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/linelists/Common_Galactic_700A-2000A.csv` & `jdaviz-3.6.1/jdaviz/data/linelists/Common_Galactic_700A-2000A.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/linelists/Common_nebular.csv` & `jdaviz-3.6.1/jdaviz/data/linelists/Common_nebular.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/linelists/Common_stellar.csv` & `jdaviz-3.6.1/jdaviz/data/linelists/Common_stellar.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/linelists/DEV_NOTES.txt` & `jdaviz-3.6.1/jdaviz/data/linelists/DEV_NOTES.txt`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/linelists/H-He.csv` & `jdaviz-3.6.1/jdaviz/data/linelists/H-He.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/linelists/H-Paschen-Brackett.csv` & `jdaviz-3.6.1/jdaviz/data/linelists/H-Paschen-Brackett.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/linelists/H2-ISO.csv` & `jdaviz-3.6.1/jdaviz/data/linelists/H2-ISO.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/linelists/H2-alt.csv` & `jdaviz-3.6.1/jdaviz/data/linelists/H2-alt.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/linelists/H2.csv` & `jdaviz-3.6.1/jdaviz/data/linelists/H2.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/linelists/HeI-HeII.csv` & `jdaviz-3.6.1/jdaviz/data/linelists/HeI-HeII.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/linelists/JWST_line_list_original.txt` & `jdaviz-3.6.1/jdaviz/data/linelists/JWST_line_list_original.txt`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/linelists/PAH.csv` & `jdaviz-3.6.1/jdaviz/data/linelists/PAH.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/linelists/SDSS-IV.csv` & `jdaviz-3.6.1/jdaviz/data/linelists/SDSS-IV.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/linelists/SDSS.csv` & `jdaviz-3.6.1/jdaviz/data/linelists/SDSS.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/linelists/UV_linelist_vacuum.csv` & `jdaviz-3.6.1/jdaviz/data/linelists/UV_linelist_vacuum.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/data/linelists/linelist_metadata.json` & `jdaviz-3.6.1/jdaviz/data/linelists/linelist_metadata.json`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/jdaviz_cli.ipynb` & `jdaviz-3.6.1/jdaviz/jdaviz_cli.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/jdaviz_cli_launcher.ipynb` & `jdaviz-3.6.1/jdaviz/jdaviz_cli_launcher.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/models/physical_models.py` & `jdaviz-3.6.1/jdaviz/models/physical_models.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/tests/coveragerc` & `jdaviz-3.6.1/jdaviz/tests/coveragerc`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/tests/test_app.py` & `jdaviz-3.6.1/jdaviz/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/tests/test_data_formats.py` & `jdaviz-3.6.1/jdaviz/tests/test_data_formats.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/tests/test_metadata.py` & `jdaviz-3.6.1/jdaviz/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/tests/test_subsets.py` & `jdaviz-3.6.1/jdaviz/tests/test_subsets.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/tests/test_utils.py` & `jdaviz-3.6.1/jdaviz/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/tests/test_viewer_ids.py` & `jdaviz-3.6.1/jdaviz/tests/test_viewer_ids.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz/utils.py` & `jdaviz-3.6.1/jdaviz/utils.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz.egg-info/PKG-INFO` & `jdaviz-3.6.1/jdaviz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jdaviz
-Version: 3.6.0
+Version: 3.6.1
 Summary: Astronomical data analysis development leveraging the Jupyter platform
 Home-page: https://jdaviz.readthedocs.io/en/latest/
 Author: JDADF Developers
 Author-email: JDADF Developers <help@stsci.edu>
 Project-URL: Homepage, https://jdaviz.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
```

### Comparing `jdaviz-3.6.0/jdaviz.egg-info/SOURCES.txt` & `jdaviz-3.6.1/jdaviz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/jdaviz.egg-info/requires.txt` & `jdaviz-3.6.1/jdaviz.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/licenses/GINGA_LICENSE.txt` & `jdaviz-3.6.1/licenses/GINGA_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/licenses/IMEXAM_LICENSE.txt` & `jdaviz-3.6.1/licenses/IMEXAM_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/licenses/IPYFILECHOOSER_LICENSE.rst` & `jdaviz-3.6.1/licenses/IPYFILECHOOSER_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/licenses/TEMPLATE_LICENCE.rst` & `jdaviz-3.6.1/licenses/TEMPLATE_LICENCE.rst`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/CubevizExample.ipynb` & `jdaviz-3.6.1/notebooks/CubevizExample.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/ImvizDitheredExample.ipynb` & `jdaviz-3.6.1/notebooks/ImvizDitheredExample.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/ImvizExample.ipynb` & `jdaviz-3.6.1/notebooks/ImvizExample.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/MosvizExample.ipynb` & `jdaviz-3.6.1/notebooks/MosvizExample.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/MosvizNIRISSExample.ipynb` & `jdaviz-3.6.1/notebooks/MosvizNIRISSExample.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/Specviz2dExample.ipynb` & `jdaviz-3.6.1/notebooks/Specviz2dExample.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/SpecvizExample.ipynb` & `jdaviz-3.6.1/notebooks/SpecvizExample.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/concepts/cubeviz_contour_overlay.ipynb` & `jdaviz-3.6.1/notebooks/concepts/cubeviz_contour_overlay.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/concepts/cubeviz_data_interactions.ipynb` & `jdaviz-3.6.1/notebooks/concepts/cubeviz_data_interactions.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/concepts/cubeviz_fitting.ipynb` & `jdaviz-3.6.1/notebooks/concepts/cubeviz_fitting.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/concepts/cubeviz_ndarray_gif.ipynb` & `jdaviz-3.6.1/notebooks/concepts/cubeviz_ndarray_gif.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/concepts/cubeviz_spectral_fitting.ipynb` & `jdaviz-3.6.1/notebooks/concepts/cubeviz_spectral_fitting.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/concepts/cubeviz_spectral_spatial_interactions.ipynb` & `jdaviz-3.6.1/notebooks/concepts/cubeviz_spectral_spatial_interactions.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/concepts/cubeviz_wfc3ir_ramp.ipynb` & `jdaviz-3.6.1/notebooks/concepts/cubeviz_wfc3ir_ramp.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/concepts/default_programmatic_viewers_from_blank.ipynb` & `jdaviz-3.6.1/notebooks/concepts/default_programmatic_viewers_from_blank.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/concepts/imviz_color_display.ipynb` & `jdaviz-3.6.1/notebooks/concepts/imviz_color_display.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/concepts/imviz_compass_mpl.ipynb` & `jdaviz-3.6.1/notebooks/concepts/imviz_compass_mpl.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/concepts/imviz_custom_colormap.ipynb` & `jdaviz-3.6.1/notebooks/concepts/imviz_custom_colormap.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/concepts/imviz_dithered_gwcs.ipynb` & `jdaviz-3.6.1/notebooks/concepts/imviz_dithered_gwcs.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/concepts/imviz_edit_subset_programmatic.ipynb` & `jdaviz-3.6.1/notebooks/concepts/imviz_edit_subset_programmatic.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/concepts/imviz_line_profiles.ipynb` & `jdaviz-3.6.1/notebooks/concepts/imviz_line_profiles.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/concepts/imviz_load_3d_slices.ipynb` & `jdaviz-3.6.1/notebooks/concepts/imviz_load_3d_slices.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/concepts/imviz_load_fits_hdu.ipynb` & `jdaviz-3.6.1/notebooks/concepts/imviz_load_fits_hdu.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/concepts/imviz_roman_asdf.ipynb` & `jdaviz-3.6.1/notebooks/concepts/imviz_roman_asdf.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/concepts/imviz_simple_aper_phot.ipynb` & `jdaviz-3.6.1/notebooks/concepts/imviz_simple_aper_phot.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/concepts/mosviz_concept.ipynb` & `jdaviz-3.6.1/notebooks/concepts/mosviz_concept.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/concepts/mosviz_generate_photometry.ipynb` & `jdaviz-3.6.1/notebooks/concepts/mosviz_generate_photometry.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/concepts/mosviz_niriss_parser.ipynb` & `jdaviz-3.6.1/notebooks/concepts/mosviz_niriss_parser.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/concepts/mosviz_overplot_slit.ipynb` & `jdaviz-3.6.1/notebooks/concepts/mosviz_overplot_slit.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/concepts/pypi_metrics.ipynb` & `jdaviz-3.6.1/notebooks/concepts/pypi_metrics.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/concepts/specviz_from_list.ipynb` & `jdaviz-3.6.1/notebooks/concepts/specviz_from_list.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/concepts/specviz_from_splot.ipynb` & `jdaviz-3.6.1/notebooks/concepts/specviz_from_splot.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/concepts/specviz_glue_unit_conversion.ipynb` & `jdaviz-3.6.1/notebooks/concepts/specviz_glue_unit_conversion.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/concepts/specviz_line_lists.ipynb` & `jdaviz-3.6.1/notebooks/concepts/specviz_line_lists.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/concepts/specviz_minimal.ipynb` & `jdaviz-3.6.1/notebooks/concepts/specviz_minimal.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/notebooks/concepts/specviz_spectrum_list.ipynb` & `jdaviz-3.6.1/notebooks/concepts/specviz_spectrum_list.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/pyproject.toml` & `jdaviz-3.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/setup.cfg` & `jdaviz-3.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/setup.py` & `jdaviz-3.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/share/jupyter/nbconvert/templates/jdaviz-default/ansi.js` & `jdaviz-3.6.1/share/jupyter/nbconvert/templates/jdaviz-default/ansi.js`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/share/jupyter/nbconvert/templates/jdaviz-default/app.html` & `jdaviz-3.6.1/share/jupyter/nbconvert/templates/jdaviz-default/app.html`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/share/jupyter/nbconvert/templates/jdaviz-default/index.html.j2` & `jdaviz-3.6.1/share/jupyter/nbconvert/templates/jdaviz-default/index.html.j2`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/share/jupyter/nbconvert/templates/jdaviz-default/util.js` & `jdaviz-3.6.1/share/jupyter/nbconvert/templates/jdaviz-default/util.js`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/share/jupyter/voila/templates/jdaviz-default/index.html.j2` & `jdaviz-3.6.1/share/jupyter/voila/templates/jdaviz-default/index.html.j2`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/standalone/jdaviz-cli-entrypoint.py` & `jdaviz-3.6.1/standalone/jdaviz-cli-entrypoint.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/standalone/jdaviz.spec` & `jdaviz-3.6.1/standalone/jdaviz.spec`

 * *Files identical despite different names*

### Comparing `jdaviz-3.6.0/tox.ini` & `jdaviz-3.6.1/tox.ini`

 * *Files identical despite different names*

