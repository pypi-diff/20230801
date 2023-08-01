# Comparing `tmp/hoppr-1.9.1.tar.gz` & `tmp/hoppr-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoppr-1.9.1.tar", max compression
+gzip compressed data, was "hoppr-1.9.2.tar", max compression
```

## Comparing `hoppr-1.9.1.tar` & `hoppr-1.9.2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0     1084 2023-07-26 21:05:34.000000 hoppr-1.9.1/LICENSE
--rw-r--r--   0        0        0     1215 2023-07-26 21:05:34.000000 hoppr-1.9.1/README.md
--rw-r--r--   0        0        0      994 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/__init__.py
--rw-r--r--   0        0        0      154 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/__main__.py
--rw-r--r--   0        0        0        0 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/base_plugins/__init__.py
--rw-r--r--   0        0        0    11546 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/base_plugins/collector.py
--rw-r--r--   0        0        0    10563 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/base_plugins/hoppr.py
--rw-r--r--   0        0        0        0 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/base_plugins/py.typed
--rw-r--r--   0        0        0     2843 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/cli/__init__.py
--rw-r--r--   0        0        0     2875 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/cli/bundle.py
--rw-r--r--   0        0        0     2252 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/cli/generate.py
--rw-r--r--   0        0        0     4025 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/cli/layout.py
--rw-r--r--   0        0        0     7383 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/cli/merge.py
--rw-r--r--   0        0        0        0 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/cli/py.typed
--rw-r--r--   0        0        0      563 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/constants.py
--rw-r--r--   0        0        0        0 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/__init__.py
--rw-r--r--   0        0        0     3046 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/bundle_tar.py
--rw-r--r--   0        0        0    12806 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/collect_apt_plugin.py
--rw-r--r--   0        0        0     2330 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/collect_cargo_plugin.py
--rw-r--r--   0        0        0    10738 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/collect_dnf_plugin.py
--rw-r--r--   0        0        0     4327 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/collect_docker_plugin.py
--rw-r--r--   0        0        0     4647 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/collect_git_plugin.py
--rw-r--r--   0        0        0     2330 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/collect_golang_plugin.py
--rw-r--r--   0        0        0     4109 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/collect_helm_plugin.py
--rw-r--r--   0        0        0     6284 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/collect_maven_plugin.py
--rw-r--r--   0        0        0     7946 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/collect_nexus_search.py
--rw-r--r--   0        0        0     2390 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/collect_npm_plugin.py
--rw-r--r--   0        0        0     2788 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/collect_nuget_plugin.py
--rw-r--r--   0        0        0     6799 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/collect_pypi_plugin.py
--rw-r--r--   0        0        0     3033 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/collect_raw_plugin.py
--rw-r--r--   0        0        0     3608 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/collect_yum_plugin.py
--rw-r--r--   0        0        0     4278 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/composite_collector.py
--rw-r--r--   0        0        0     5506 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/delta_sbom.py
--rw-r--r--   0        0        0     6885 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/oras_bundle.py
--rw-r--r--   0        0        0     5252 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/oras_registry.py
--rw-r--r--   0        0        0        0 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/py.typed
--rw-r--r--   0        0        0      202 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/report_generator/__init__.py
--rw-r--r--   0        0        0   126749 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png
--rw-r--r--   0        0        0     4635 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/report_generator/report_generator.py
--rw-r--r--   0        0        0    60554 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js
--rw-r--r--   0        0        0      518 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/report_generator/scripts/custom.js
--rw-r--r--   0        0        0   220780 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/report_generator/styles/bootstrap.min.css
--rw-r--r--   0        0        0     3562 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/report_generator/styles/custom.css
--rw-r--r--   0        0        0     5052 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/report_generator/templates/component_card.jinja2
--rw-r--r--   0        0        0     1230 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/report_generator/templates/general_summary.jinja2
--rw-r--r--   0        0        0     7246 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/report_generator/templates/index.jinja2
--rw-r--r--   0        0        0      458 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/exceptions.py
--rw-r--r--   0        0        0     6827 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/in_toto.py
--rw-r--r--   0        0        0     2908 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/main.py
--rw-r--r--   0        0        0     4106 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/mem_logger.py
--rw-r--r--   0        0        0     1627 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/models/__init__.py
--rw-r--r--   0        0        0     1602 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/models/__main__.py
--rw-r--r--   0        0        0     1546 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/models/base.py
--rw-r--r--   0        0        0     4001 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/models/credentials.py
--rw-r--r--   0        0        0    12711 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/models/manifest.py
--rw-r--r--   0        0        0        0 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/models/py.typed
--rw-r--r--   0        0        0    20814 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/models/sbom.py
--rw-r--r--   0        0        0     4730 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/models/transfer.py
--rw-r--r--   0        0        0     5677 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/models/types.py
--rw-r--r--   0        0        0     2335 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/net.py
--rw-r--r--   0        0        0     4251 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/oci_artifacts.py
--rw-r--r--   0        0        0     1332 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/plugin_utils.py
--rw-r--r--   0        0        0    28786 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/processor.py
--rw-r--r--   0        0        0        0 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/py.typed
--rw-r--r--   0        0        0    22579 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/resources/hoppr-hippo.ansi
--rw-r--r--   0        0        0    19725 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/resources/hoppr-hippo.ascii
--rw-r--r--   0        0        0     4036 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/result.py
--rw-r--r--   0        0        0     7785 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/utils.py
--rw-r--r--   0        0        0     5052 2023-07-26 21:05:34.000000 hoppr-1.9.1/pyproject.toml
--rw-r--r--   0        0        0     2648 1970-01-01 00:00:00.000000 hoppr-1.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-08-01 20:05:46.000000 hoppr-1.9.2/LICENSE
+-rw-r--r--   0        0        0     1215 2023-08-01 20:05:46.000000 hoppr-1.9.2/README.md
+-rw-r--r--   0        0        0      994 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/__init__.py
+-rw-r--r--   0        0        0      154 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/base_plugins/__init__.py
+-rw-r--r--   0        0        0    11546 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/base_plugins/collector.py
+-rw-r--r--   0        0        0    10563 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/base_plugins/hoppr.py
+-rw-r--r--   0        0        0        0 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/base_plugins/py.typed
+-rw-r--r--   0        0        0     2843 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/cli/__init__.py
+-rw-r--r--   0        0        0     2875 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/cli/bundle.py
+-rw-r--r--   0        0        0     2252 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/cli/generate.py
+-rw-r--r--   0        0        0     4025 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/cli/layout.py
+-rw-r--r--   0        0        0     7383 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/cli/merge.py
+-rw-r--r--   0        0        0        0 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/cli/py.typed
+-rw-r--r--   0        0        0      563 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/constants.py
+-rw-r--r--   0        0        0        0 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/core_plugins/__init__.py
+-rw-r--r--   0        0        0     3046 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/core_plugins/bundle_tar.py
+-rw-r--r--   0        0        0    12806 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/core_plugins/collect_apt_plugin.py
+-rw-r--r--   0        0        0     2330 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/core_plugins/collect_cargo_plugin.py
+-rw-r--r--   0        0        0    10738 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/core_plugins/collect_dnf_plugin.py
+-rw-r--r--   0        0        0     4327 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/core_plugins/collect_docker_plugin.py
+-rw-r--r--   0        0        0     4647 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/core_plugins/collect_git_plugin.py
+-rw-r--r--   0        0        0     2330 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/core_plugins/collect_golang_plugin.py
+-rw-r--r--   0        0        0     4109 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/core_plugins/collect_helm_plugin.py
+-rw-r--r--   0        0        0     6284 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/core_plugins/collect_maven_plugin.py
+-rw-r--r--   0        0        0     7946 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/core_plugins/collect_nexus_search.py
+-rw-r--r--   0        0        0     2390 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/core_plugins/collect_npm_plugin.py
+-rw-r--r--   0        0        0     2788 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/core_plugins/collect_nuget_plugin.py
+-rw-r--r--   0        0        0     6799 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/core_plugins/collect_pypi_plugin.py
+-rw-r--r--   0        0        0     3033 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/core_plugins/collect_raw_plugin.py
+-rw-r--r--   0        0        0     3608 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/core_plugins/collect_yum_plugin.py
+-rw-r--r--   0        0        0     4278 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/core_plugins/composite_collector.py
+-rw-r--r--   0        0        0     5506 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/core_plugins/delta_sbom.py
+-rw-r--r--   0        0        0     6885 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/core_plugins/oras_bundle.py
+-rw-r--r--   0        0        0     5252 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/core_plugins/oras_registry.py
+-rw-r--r--   0        0        0        0 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/core_plugins/py.typed
+-rw-r--r--   0        0        0      202 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/core_plugins/report_generator/__init__.py
+-rw-r--r--   0        0        0   126749 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png
+-rw-r--r--   0        0        0     4635 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/core_plugins/report_generator/report_generator.py
+-rw-r--r--   0        0        0    60554 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js
+-rw-r--r--   0        0        0      518 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/core_plugins/report_generator/scripts/custom.js
+-rw-r--r--   0        0        0   220780 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/core_plugins/report_generator/styles/bootstrap.min.css
+-rw-r--r--   0        0        0     3562 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/core_plugins/report_generator/styles/custom.css
+-rw-r--r--   0        0        0     5052 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/core_plugins/report_generator/templates/component_card.jinja2
+-rw-r--r--   0        0        0     1230 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/core_plugins/report_generator/templates/general_summary.jinja2
+-rw-r--r--   0        0        0     7246 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/core_plugins/report_generator/templates/index.jinja2
+-rw-r--r--   0        0        0      458 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/exceptions.py
+-rw-r--r--   0        0        0     6827 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/in_toto.py
+-rw-r--r--   0        0        0     2908 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/main.py
+-rw-r--r--   0        0        0     4106 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/mem_logger.py
+-rw-r--r--   0        0        0     1627 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/models/__init__.py
+-rw-r--r--   0        0        0     1602 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/models/__main__.py
+-rw-r--r--   0        0        0     1546 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/models/base.py
+-rw-r--r--   0        0        0     4001 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/models/credentials.py
+-rw-r--r--   0        0        0    12711 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/models/manifest.py
+-rw-r--r--   0        0        0        0 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/models/py.typed
+-rw-r--r--   0        0        0    20799 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/models/sbom.py
+-rw-r--r--   0        0        0     4730 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/models/transfer.py
+-rw-r--r--   0        0        0     5677 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/models/types.py
+-rw-r--r--   0        0        0     2335 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/net.py
+-rw-r--r--   0        0        0     4251 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/oci_artifacts.py
+-rw-r--r--   0        0        0     1332 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/plugin_utils.py
+-rw-r--r--   0        0        0    28786 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/processor.py
+-rw-r--r--   0        0        0        0 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/py.typed
+-rw-r--r--   0        0        0    22579 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/resources/hoppr-hippo.ansi
+-rw-r--r--   0        0        0    19725 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/resources/hoppr-hippo.ascii
+-rw-r--r--   0        0        0     4036 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/result.py
+-rw-r--r--   0        0        0     7785 2023-08-01 20:05:46.000000 hoppr-1.9.2/hoppr/utils.py
+-rw-r--r--   0        0        0     5052 2023-08-01 20:05:46.000000 hoppr-1.9.2/pyproject.toml
+-rw-r--r--   0        0        0     2648 1970-01-01 00:00:00.000000 hoppr-1.9.2/PKG-INFO
```

### Comparing `hoppr-1.9.1/LICENSE` & `hoppr-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/README.md` & `hoppr-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/__init__.py` & `hoppr-1.9.2/hoppr/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,8 +28,8 @@
     "Manifest",
     "PurlType",
     "Result",
     "Sbom",
     "Transfer",
 ]
 
-__version__ = "1.9.1"
+__version__ = "1.9.2"
```

### Comparing `hoppr-1.9.1/hoppr/base_plugins/collector.py` & `hoppr-1.9.2/hoppr/base_plugins/collector.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/base_plugins/hoppr.py` & `hoppr-1.9.2/hoppr/base_plugins/hoppr.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/cli/__init__.py` & `hoppr-1.9.2/hoppr/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/cli/bundle.py` & `hoppr-1.9.2/hoppr/cli/bundle.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/cli/generate.py` & `hoppr-1.9.2/hoppr/cli/generate.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/cli/layout.py` & `hoppr-1.9.2/hoppr/cli/layout.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/cli/merge.py` & `hoppr-1.9.2/hoppr/cli/merge.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/constants.py` & `hoppr-1.9.2/hoppr/constants.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/core_plugins/bundle_tar.py` & `hoppr-1.9.2/hoppr/core_plugins/bundle_tar.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/core_plugins/collect_apt_plugin.py` & `hoppr-1.9.2/hoppr/core_plugins/collect_apt_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/core_plugins/collect_cargo_plugin.py` & `hoppr-1.9.2/hoppr/core_plugins/collect_cargo_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/core_plugins/collect_dnf_plugin.py` & `hoppr-1.9.2/hoppr/core_plugins/collect_dnf_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/core_plugins/collect_docker_plugin.py` & `hoppr-1.9.2/hoppr/core_plugins/collect_docker_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/core_plugins/collect_git_plugin.py` & `hoppr-1.9.2/hoppr/core_plugins/collect_git_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/core_plugins/collect_golang_plugin.py` & `hoppr-1.9.2/hoppr/core_plugins/collect_golang_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/core_plugins/collect_helm_plugin.py` & `hoppr-1.9.2/hoppr/core_plugins/collect_helm_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/core_plugins/collect_maven_plugin.py` & `hoppr-1.9.2/hoppr/core_plugins/collect_maven_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/core_plugins/collect_nexus_search.py` & `hoppr-1.9.2/hoppr/core_plugins/collect_nexus_search.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/core_plugins/collect_npm_plugin.py` & `hoppr-1.9.2/hoppr/core_plugins/collect_npm_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/core_plugins/collect_nuget_plugin.py` & `hoppr-1.9.2/hoppr/core_plugins/collect_nuget_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/core_plugins/collect_pypi_plugin.py` & `hoppr-1.9.2/hoppr/core_plugins/collect_pypi_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/core_plugins/collect_raw_plugin.py` & `hoppr-1.9.2/hoppr/core_plugins/collect_raw_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/core_plugins/collect_yum_plugin.py` & `hoppr-1.9.2/hoppr/core_plugins/collect_yum_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/core_plugins/composite_collector.py` & `hoppr-1.9.2/hoppr/core_plugins/composite_collector.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/core_plugins/delta_sbom.py` & `hoppr-1.9.2/hoppr/core_plugins/delta_sbom.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/core_plugins/oras_bundle.py` & `hoppr-1.9.2/hoppr/core_plugins/oras_bundle.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/core_plugins/oras_registry.py` & `hoppr-1.9.2/hoppr/core_plugins/oras_registry.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png` & `hoppr-1.9.2/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/core_plugins/report_generator/report_generator.py` & `hoppr-1.9.2/hoppr/core_plugins/report_generator/report_generator.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js` & `hoppr-1.9.2/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/core_plugins/report_generator/scripts/custom.js` & `hoppr-1.9.2/hoppr/core_plugins/report_generator/scripts/custom.js`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/core_plugins/report_generator/styles/bootstrap.min.css` & `hoppr-1.9.2/hoppr/core_plugins/report_generator/styles/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/core_plugins/report_generator/styles/custom.css` & `hoppr-1.9.2/hoppr/core_plugins/report_generator/styles/custom.css`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/core_plugins/report_generator/templates/component_card.jinja2` & `hoppr-1.9.2/hoppr/core_plugins/report_generator/templates/component_card.jinja2`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/core_plugins/report_generator/templates/general_summary.jinja2` & `hoppr-1.9.2/hoppr/core_plugins/report_generator/templates/general_summary.jinja2`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/core_plugins/report_generator/templates/index.jinja2` & `hoppr-1.9.2/hoppr/core_plugins/report_generator/templates/index.jinja2`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/in_toto.py` & `hoppr-1.9.2/hoppr/in_toto.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/main.py` & `hoppr-1.9.2/hoppr/main.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/mem_logger.py` & `hoppr-1.9.2/hoppr/mem_logger.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/models/__init__.py` & `hoppr-1.9.2/hoppr/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/models/__main__.py` & `hoppr-1.9.2/hoppr/models/__main__.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/models/base.py` & `hoppr-1.9.2/hoppr/models/base.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/models/credentials.py` & `hoppr-1.9.2/hoppr/models/credentials.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/models/manifest.py` & `hoppr-1.9.2/hoppr/models/manifest.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/models/sbom.py` & `hoppr-1.9.2/hoppr/models/sbom.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         """
         merged_field = getattr(self, target_field_name)
         field_type = type(merged_field)
 
         if isinstance(field_type, type(BaseModel)):
             merged_field = CycloneDXBaseModel.create(model=merged_field)
             source_field = CycloneDXBaseModel.create(model=source_field)
-            merged_field = merged_field.merge(source_field)
+            merged_field.merge(source_field)
         elif self._is_list_of(BaseModel, merged_field):
             merged_field = hoppr.utils.dedup_list([CycloneDXBaseModel.create(model=_field) for _field in merged_field])
             source_field = [CycloneDXBaseModel.create(model=_field) for _field in source_field or []]
             self._merge_field_items(merged_field, source_field)
 
         setattr(self, target_field_name, merged_field)
```

### Comparing `hoppr-1.9.1/hoppr/models/transfer.py` & `hoppr-1.9.2/hoppr/models/transfer.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/models/types.py` & `hoppr-1.9.2/hoppr/models/types.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/net.py` & `hoppr-1.9.2/hoppr/net.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/oci_artifacts.py` & `hoppr-1.9.2/hoppr/oci_artifacts.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/plugin_utils.py` & `hoppr-1.9.2/hoppr/plugin_utils.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/processor.py` & `hoppr-1.9.2/hoppr/processor.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/resources/hoppr-hippo.ansi` & `hoppr-1.9.2/hoppr/resources/hoppr-hippo.ansi`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/resources/hoppr-hippo.ascii` & `hoppr-1.9.2/hoppr/resources/hoppr-hippo.ascii`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/result.py` & `hoppr-1.9.2/hoppr/result.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/hoppr/utils.py` & `hoppr-1.9.2/hoppr/utils.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.1/pyproject.toml` & `hoppr-1.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hoppr"
-version = "1.9.1"
+version = "1.9.2"
 description = "A tool for defining, verifying, and transferring software dependencies between environments."
 authors = ["LMCO Open Source <open.source@lmco.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://hoppr.dev"
 repository = "https://gitlab.com/hoppr/hoppr"
```

### Comparing `hoppr-1.9.1/PKG-INFO` & `hoppr-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoppr
-Version: 1.9.1
+Version: 1.9.2
 Summary: A tool for defining, verifying, and transferring software dependencies between environments.
 Home-page: https://hoppr.dev
 License: MIT
 Keywords: packaging,reports,build dependencies,software bill of materials
 Author: LMCO Open Source
 Author-email: open.source@lmco.com
 Requires-Python: >=3.10,<4.0
```

