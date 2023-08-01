# Comparing `tmp/cognite_neat-0.18.2.tar.gz` & `tmp/cognite_neat-0.18.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_neat-0.18.2.tar", max compression
+gzip compressed data, was "cognite_neat-0.18.3.tar", max compression
```

## Comparing `cognite_neat-0.18.2.tar` & `cognite_neat-0.18.3.tar`

### file list

```diff
@@ -1,117 +1,127 @@
--rw-r--r--   0        0        0    11351 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/LICENSE
--rw-r--r--   0        0        0     8667 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/README.md
--rw-r--r--   0        0        0       61 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/__init__.py
--rw-r--r--   0        0        0       23 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/_version.py
--rw-r--r--   0        0        0        0 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/api/__init__.py
--rw-r--r--   0        0        0     2778 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/api/app.py
--rw-r--r--   0        0        0     5611 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/api/configuration.py
--rw-r--r--   0        0        0        0 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/api/data_classes/__init__.py
--rw-r--r--   0        0        0     1390 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/api/data_classes/rest.py
--rw-r--r--   0        0        0    24080 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/api/explorer.py
--rw-r--r--   0        0        0        0 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/api/utils/__init__.py
--rw-r--r--   0        0        0      412 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/api/utils/data_mapping.py
--rw-r--r--   0        0        0     4622 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/api/utils/query_templates.py
--rw-r--r--   0        0        0      357 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/main.py
--rw-r--r--   0        0        0       16 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/ui/index.html
--rw-r--r--   0        0        0      312 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/.gitignore
--rw-r--r--   0        0        0     3359 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/README.md
--rw-r--r--   0        0        0      464 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/asset-manifest.json
--rw-r--r--   0        0        0     3870 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/favicon.ico
--rw-r--r--   0        0        0      630 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/index.html
--rw-r--r--   0        0        0     5347 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/logo192.png
--rw-r--r--   0        0        0      492 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/manifest.json
--rw-r--r--   0        0        0       67 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/robots.txt
--rw-r--r--   0        0        0     8524 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
--rw-r--r--   0        0        0    13319 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
--rw-r--r--   0        0        0  1370405 2023-07-26 15:57:51.286903 cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/static/js/main.694f3f8e.js
--rw-r--r--   0        0        0     2667 2023-07-26 15:57:51.286903 cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/static/js/main.694f3f8e.js.LICENSE.txt
--rw-r--r--   0        0        0  5883860 2023-07-26 15:57:51.322903 cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/static/js/main.694f3f8e.js.map
--rw-r--r--   0        0        0     2633 2023-07-26 15:57:51.322903 cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
--rw-r--r--   0        0        0      979 2023-07-26 15:57:51.326903 cognite_neat-0.18.2/cognite/neat/config.py
--rw-r--r--   0        0        0      347 2023-07-26 15:57:51.326903 cognite_neat-0.18.2/cognite/neat/constants.py
--rw-r--r--   0        0        0     1276 2023-07-26 15:57:51.326903 cognite_neat-0.18.2/cognite/neat/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-26 15:57:51.326903 cognite_neat-0.18.2/cognite/neat/graph/__init__.py
--rw-r--r--   0        0        0  1437938 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0      368 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/examples/__init__.py
--rw-r--r--   0        0        0      442 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/extractors/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/extractors/data_stores/__init__.py
--rw-r--r--   0        0        0     1520 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/extractors/data_stores/metrics.py
--rw-r--r--   0        0        0     9436 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/extractors/data_stores/oxrdflib.py
--rw-r--r--   0        0        0     7255 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/extractors/graph_sheet_to_graph.py
--rw-r--r--   0        0        0    11434 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/extractors/graph_store.py
--rw-r--r--   0        0        0       68 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/extractors/mocks/__init__.py
--rw-r--r--   0        0        0    12883 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/extractors/mocks/graph.py
--rw-r--r--   0        0        0     1213 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/extractors/rdf_to_graph.py
--rw-r--r--   0        0        0      432 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/loaders/__init__.py
--rw-r--r--   0        0        0     2837 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/loaders/_exceptions.py
--rw-r--r--   0        0        0        0 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/loaders/core/__init__.py
--rw-r--r--   0        0        0     2279 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/loaders/core/labels.py
--rw-r--r--   0        0        0     5043 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/loaders/core/models.py
--rw-r--r--   0        0        0    39898 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/loaders/core/rdf_to_assets.py
--rw-r--r--   0        0        0    20925 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/loaders/core/rdf_to_relationships.py
--rw-r--r--   0        0        0     2650 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/loaders/validator.py
--rw-r--r--   0        0        0        0 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/transformations/__init__.py
--rw-r--r--   0        0        0       73 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/transformations/query_generator/__init__.py
--rw-r--r--   0        0        0     9592 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/graph/transformations/query_generator/sparql.py
--rw-r--r--   0        0        0    11892 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/graph/transformations/transformer.py
--rw-r--r--   0        0        0      379 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/__init__.py
--rw-r--r--   0        0        0    49672 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/_exceptions.py
--rw-r--r--   0        0        0    13038 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/_parser.py
--rw-r--r--   0        0        0     3496 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/_validation.py
--rw-r--r--   0        0        0     4777 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/analysis.py
--rw-r--r--   0        0        0    80218 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/examples/Rules-Nordic44-to-TNT.xlsx
--rw-r--r--   0        0        0      449 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/examples/__init__.py
--rw-r--r--   0        0        0    77381 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/examples/power-grid-example.xlsx
--rw-r--r--   0        0        0    75865 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/examples/rules-template.xlsx
--rw-r--r--   0        0        0    52650 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/examples/sheet2cdf-transformation-rules.xlsx
--rw-r--r--   0        0        0    79964 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/examples/source-to-solution-mapping-rules.xlsx
--rw-r--r--   0        0        0        0 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/exporter/__init__.py
--rw-r--r--   0        0        0      102 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/exporter/core/__init__.py
--rw-r--r--   0        0        0      610 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/exporter/core/rules2labels.py
--rw-r--r--   0        0        0       48 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/exporter/dm/rules2dms.py
--rw-r--r--   0        0        0     5403 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/exporter/rules2graph_sheet.py
--rw-r--r--   0        0        0     4763 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/exporter/rules2graphql.py
--rw-r--r--   0        0        0    15643 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/exporter/rules2ontology.py
--rw-r--r--   0        0        0     4019 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/exporter/rules2rules.py
--rw-r--r--   0        0        0      631 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/exporter/rules2triples.py
--rw-r--r--   0        0        0       63 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/importer/__init__.py
--rw-r--r--   0        0        0    13007 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/importer/ontology2excel.py
--rw-r--r--   0        0        0    24214 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/models.py
--rw-r--r--   0        0        0     8231 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/to_rdf_path.py
--rw-r--r--   0        0        0        0 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/utils/__init__.py
--rw-r--r--   0        0        0      309 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/utils/auxiliary.py
--rw-r--r--   0        0        0      741 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/utils/cdf.py
--rw-r--r--   0        0        0    10682 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/utils/utils.py
--rw-r--r--   0        0        0      352 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/workflows/__init__.py
--rw-r--r--   0        0        0    23386 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/workflows/base.py
--rw-r--r--   0        0        0     9986 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/workflows/base_workflows/graph2assets_relationships.py
--rw-r--r--   0        0        0     7066 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/workflows/base_workflows/graphs_and_rules.py
--rw-r--r--   0        0        0    14390 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/workflows/base_workflows/sheet2cdf.py
--rw-r--r--   0        0        0    11774 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/workflows/base_workflows/sme_graph_capture.py
--rw-r--r--   0        0        0    17837 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/workflows/cdf_store.py
--rw-r--r--   0        0        0     1442 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/workflows/examples/basic/workflow.py
--rw-r--r--   0        0        0     1782 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/examples/basic/workflow.yaml
--rw-r--r--   0        0        0    15718 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/examples/default/workflow.py
--rw-r--r--   0        0        0     6774 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/examples/default/workflow.yaml
--rw-r--r--   0        0        0     3536 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/examples/fdm_schema_generation/workflow.py
--rw-r--r--   0        0        0     2573 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/examples/fdm_schema_generation/workflow.yaml
--rw-r--r--   0        0        0    11435 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/examples/graph_db_import/workflow.py
--rw-r--r--   0        0        0     4792 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/examples/graph_db_import/workflow.yaml
--rw-r--r--   0        0        0      324 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/examples/graph_to_asset_hierarchy/workflow.py
--rw-r--r--   0        0        0     8063 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/examples/graph_to_asset_hierarchy/workflow.yaml
--rw-r--r--   0        0        0      274 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/examples/sheet2cdf/workflow.py
--rw-r--r--   0        0        0     6668 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/examples/sheet2cdf/workflow.yaml
--rw-r--r--   0        0        0      301 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/examples/sme_graph_capture/workflow.py
--rw-r--r--   0        0        0     6837 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/examples/sme_graph_capture/workflow.yaml
--rw-r--r--   0        0        0    11648 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/manager.py
--rw-r--r--   0        0        0        0 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/migration/__init__.py
--rw-r--r--   0        0        0     1581 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/migration/wf_manifests.py
--rw-r--r--   0        0        0     4907 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/model.py
--rw-r--r--   0        0        0     1008 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/step_model.py
--rw-r--r--   0        0        0      651 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/steps/data_contracts.py
--rw-r--r--   0        0        0     1978 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/steps/steps.py
--rw-r--r--   0        0        0      771 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/tasks.py
--rw-r--r--   0        0        0     6969 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/triggers.py
--rw-r--r--   0        0        0      453 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/utils.py
--rw-r--r--   0        0        0     2740 2023-07-26 15:57:51.846905 cognite_neat-0.18.2/pyproject.toml
--rw-r--r--   0        0        0    10617 1970-01-01 00:00:00.000000 cognite_neat-0.18.2/PKG-INFO
+-rw-r--r--   0        0        0    11351 2023-08-01 09:39:47.775102 cognite_neat-0.18.3/LICENSE
+-rw-r--r--   0        0        0     8667 2023-08-01 09:39:47.775102 cognite_neat-0.18.3/README.md
+-rw-r--r--   0        0        0       61 2023-08-01 09:39:47.775102 cognite_neat-0.18.3/cognite/neat/__init__.py
+-rw-r--r--   0        0        0       23 2023-08-01 09:39:47.775102 cognite_neat-0.18.3/cognite/neat/_version.py
+-rw-r--r--   0        0        0        0 2023-08-01 09:39:47.775102 cognite_neat-0.18.3/cognite/neat/app/api/__init__.py
+-rw-r--r--   0        0        0      153 2023-08-01 09:39:47.775102 cognite_neat-0.18.3/cognite/neat/app/api/asgi/metrics.py
+-rw-r--r--   0        0        0     4137 2023-08-01 09:39:47.775102 cognite_neat-0.18.3/cognite/neat/app/api/configuration.py
+-rw-r--r--   0        0        0       90 2023-08-01 09:39:47.775102 cognite_neat-0.18.3/cognite/neat/app/api/context_manager/__init__.py
+-rw-r--r--   0        0        0      380 2023-08-01 09:39:47.775102 cognite_neat-0.18.3/cognite/neat/app/api/context_manager/manager.py
+-rw-r--r--   0        0        0        0 2023-08-01 09:39:47.775102 cognite_neat-0.18.3/cognite/neat/app/api/data_classes/__init__.py
+-rw-r--r--   0        0        0     3826 2023-08-01 09:39:47.775102 cognite_neat-0.18.3/cognite/neat/app/api/data_classes/configuration.py
+-rw-r--r--   0        0        0     1390 2023-08-01 09:39:47.775102 cognite_neat-0.18.3/cognite/neat/app/api/data_classes/rest.py
+-rw-r--r--   0        0        0     1595 2023-08-01 09:39:47.779103 cognite_neat-0.18.3/cognite/neat/app/api/explorer.py
+-rw-r--r--   0        0        0      635 2023-08-01 09:39:47.779103 cognite_neat-0.18.3/cognite/neat/app/api/routers/configuration.py
+-rw-r--r--   0        0        0     3196 2023-08-01 09:39:47.779103 cognite_neat-0.18.3/cognite/neat/app/api/routers/crud.py
+-rw-r--r--   0        0        0    11484 2023-08-01 09:39:47.779103 cognite_neat-0.18.3/cognite/neat/app/api/routers/data_exploration.py
+-rw-r--r--   0        0        0      210 2023-08-01 09:39:47.779103 cognite_neat-0.18.3/cognite/neat/app/api/routers/metrics.py
+-rw-r--r--   0        0        0     2503 2023-08-01 09:39:47.779103 cognite_neat-0.18.3/cognite/neat/app/api/routers/rules.py
+-rw-r--r--   0        0        0     4573 2023-08-01 09:39:47.779103 cognite_neat-0.18.3/cognite/neat/app/api/routers/workflows.py
+-rw-r--r--   0        0        0        0 2023-08-01 09:39:47.779103 cognite_neat-0.18.3/cognite/neat/app/api/utils/__init__.py
+-rw-r--r--   0        0        0      412 2023-08-01 09:39:47.779103 cognite_neat-0.18.3/cognite/neat/app/api/utils/data_mapping.py
+-rw-r--r--   0        0        0     4622 2023-08-01 09:39:47.779103 cognite_neat-0.18.3/cognite/neat/app/api/utils/query_templates.py
+-rw-r--r--   0        0        0      357 2023-08-01 09:39:47.779103 cognite_neat-0.18.3/cognite/neat/app/main.py
+-rw-r--r--   0        0        0       16 2023-08-01 09:39:47.779103 cognite_neat-0.18.3/cognite/neat/app/ui/index.html
+-rw-r--r--   0        0        0      312 2023-08-01 09:39:47.779103 cognite_neat-0.18.3/cognite/neat/app/ui/neat-app/.gitignore
+-rw-r--r--   0        0        0     3359 2023-08-01 09:39:47.779103 cognite_neat-0.18.3/cognite/neat/app/ui/neat-app/README.md
+-rw-r--r--   0        0        0      464 2023-08-01 09:39:47.779103 cognite_neat-0.18.3/cognite/neat/app/ui/neat-app/build/asset-manifest.json
+-rw-r--r--   0        0        0     3870 2023-08-01 09:39:47.779103 cognite_neat-0.18.3/cognite/neat/app/ui/neat-app/build/favicon.ico
+-rw-r--r--   0        0        0      630 2023-08-01 09:39:47.779103 cognite_neat-0.18.3/cognite/neat/app/ui/neat-app/build/index.html
+-rw-r--r--   0        0        0     5347 2023-08-01 09:39:47.779103 cognite_neat-0.18.3/cognite/neat/app/ui/neat-app/build/logo192.png
+-rw-r--r--   0        0        0      492 2023-08-01 09:39:47.779103 cognite_neat-0.18.3/cognite/neat/app/ui/neat-app/build/manifest.json
+-rw-r--r--   0        0        0       67 2023-08-01 09:39:47.779103 cognite_neat-0.18.3/cognite/neat/app/ui/neat-app/build/robots.txt
+-rw-r--r--   0        0        0     8524 2023-08-01 09:39:47.779103 cognite_neat-0.18.3/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
+-rw-r--r--   0        0        0    13319 2023-08-01 09:39:47.779103 cognite_neat-0.18.3/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
+-rw-r--r--   0        0        0  1370405 2023-08-01 09:39:47.787103 cognite_neat-0.18.3/cognite/neat/app/ui/neat-app/build/static/js/main.694f3f8e.js
+-rw-r--r--   0        0        0     2667 2023-08-01 09:39:47.787103 cognite_neat-0.18.3/cognite/neat/app/ui/neat-app/build/static/js/main.694f3f8e.js.LICENSE.txt
+-rw-r--r--   0        0        0  5883860 2023-08-01 09:39:47.819104 cognite_neat-0.18.3/cognite/neat/app/ui/neat-app/build/static/js/main.694f3f8e.js.map
+-rw-r--r--   0        0        0     2633 2023-08-01 09:39:47.819104 cognite_neat-0.18.3/cognite/neat/app/ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
+-rw-r--r--   0        0        0      979 2023-08-01 09:39:47.823104 cognite_neat-0.18.3/cognite/neat/config.py
+-rw-r--r--   0        0        0     1368 2023-08-01 09:39:47.823104 cognite_neat-0.18.3/cognite/neat/constants.py
+-rw-r--r--   0        0        0     1276 2023-08-01 09:39:47.823104 cognite_neat-0.18.3/cognite/neat/exceptions.py
+-rw-r--r--   0        0        0        0 2023-08-01 09:39:47.823104 cognite_neat-0.18.3/cognite/neat/graph/__init__.py
+-rw-r--r--   0        0        0  1437938 2023-08-01 09:39:47.827104 cognite_neat-0.18.3/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0      368 2023-08-01 09:39:47.827104 cognite_neat-0.18.3/cognite/neat/graph/examples/__init__.py
+-rw-r--r--   0        0        0      442 2023-08-01 09:39:47.827104 cognite_neat-0.18.3/cognite/neat/graph/extractors/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 09:39:47.827104 cognite_neat-0.18.3/cognite/neat/graph/extractors/data_stores/__init__.py
+-rw-r--r--   0        0        0      456 2023-08-01 09:39:47.827104 cognite_neat-0.18.3/cognite/neat/graph/extractors/data_stores/configuration.py
+-rw-r--r--   0        0        0     1520 2023-08-01 09:39:47.827104 cognite_neat-0.18.3/cognite/neat/graph/extractors/data_stores/metrics.py
+-rw-r--r--   0        0        0     9436 2023-08-01 09:39:47.827104 cognite_neat-0.18.3/cognite/neat/graph/extractors/data_stores/oxrdflib.py
+-rw-r--r--   0        0        0     7255 2023-08-01 09:39:47.827104 cognite_neat-0.18.3/cognite/neat/graph/extractors/graph_sheet_to_graph.py
+-rw-r--r--   0        0        0    11489 2023-08-01 09:39:47.827104 cognite_neat-0.18.3/cognite/neat/graph/extractors/graph_store.py
+-rw-r--r--   0        0        0       68 2023-08-01 09:39:47.827104 cognite_neat-0.18.3/cognite/neat/graph/extractors/mocks/__init__.py
+-rw-r--r--   0        0        0    12883 2023-08-01 09:39:47.827104 cognite_neat-0.18.3/cognite/neat/graph/extractors/mocks/graph.py
+-rw-r--r--   0        0        0     1201 2023-08-01 09:39:47.827104 cognite_neat-0.18.3/cognite/neat/graph/extractors/rdf_to_graph.py
+-rw-r--r--   0        0        0      432 2023-08-01 09:39:47.827104 cognite_neat-0.18.3/cognite/neat/graph/loaders/__init__.py
+-rw-r--r--   0        0        0     2837 2023-08-01 09:39:47.827104 cognite_neat-0.18.3/cognite/neat/graph/loaders/_exceptions.py
+-rw-r--r--   0        0        0        0 2023-08-01 09:39:47.827104 cognite_neat-0.18.3/cognite/neat/graph/loaders/core/__init__.py
+-rw-r--r--   0        0        0     2279 2023-08-01 09:39:47.827104 cognite_neat-0.18.3/cognite/neat/graph/loaders/core/labels.py
+-rw-r--r--   0        0        0     5043 2023-08-01 09:39:47.827104 cognite_neat-0.18.3/cognite/neat/graph/loaders/core/models.py
+-rw-r--r--   0        0        0    40137 2023-08-01 09:39:47.827104 cognite_neat-0.18.3/cognite/neat/graph/loaders/core/rdf_to_assets.py
+-rw-r--r--   0        0        0    20925 2023-08-01 09:39:47.827104 cognite_neat-0.18.3/cognite/neat/graph/loaders/core/rdf_to_relationships.py
+-rw-r--r--   0        0        0     2650 2023-08-01 09:39:47.827104 cognite_neat-0.18.3/cognite/neat/graph/loaders/validator.py
+-rw-r--r--   0        0        0        0 2023-08-01 09:39:47.827104 cognite_neat-0.18.3/cognite/neat/graph/transformations/__init__.py
+-rw-r--r--   0        0        0       73 2023-08-01 09:39:47.827104 cognite_neat-0.18.3/cognite/neat/graph/transformations/query_generator/__init__.py
+-rw-r--r--   0        0        0     9580 2023-08-01 09:39:47.827104 cognite_neat-0.18.3/cognite/neat/graph/transformations/query_generator/sparql.py
+-rw-r--r--   0        0        0    11892 2023-08-01 09:39:47.827104 cognite_neat-0.18.3/cognite/neat/graph/transformations/transformer.py
+-rw-r--r--   0        0        0      378 2023-08-01 09:39:47.827104 cognite_neat-0.18.3/cognite/neat/rules/__init__.py
+-rw-r--r--   0        0        0    49672 2023-08-01 09:39:47.827104 cognite_neat-0.18.3/cognite/neat/rules/_exceptions.py
+-rw-r--r--   0        0        0     3496 2023-08-01 09:39:47.827104 cognite_neat-0.18.3/cognite/neat/rules/_validation.py
+-rw-r--r--   0        0        0     4777 2023-08-01 09:39:47.827104 cognite_neat-0.18.3/cognite/neat/rules/analysis.py
+-rw-r--r--   0        0        0    80218 2023-08-01 09:39:47.831104 cognite_neat-0.18.3/cognite/neat/rules/examples/Rules-Nordic44-to-TNT.xlsx
+-rw-r--r--   0        0        0      449 2023-08-01 09:39:47.831104 cognite_neat-0.18.3/cognite/neat/rules/examples/__init__.py
+-rw-r--r--   0        0        0    77381 2023-08-01 09:39:47.831104 cognite_neat-0.18.3/cognite/neat/rules/examples/power-grid-example.xlsx
+-rw-r--r--   0        0        0    75865 2023-08-01 09:39:47.831104 cognite_neat-0.18.3/cognite/neat/rules/examples/rules-template.xlsx
+-rw-r--r--   0        0        0    52650 2023-08-01 09:39:47.831104 cognite_neat-0.18.3/cognite/neat/rules/examples/sheet2cdf-transformation-rules.xlsx
+-rw-r--r--   0        0        0    79964 2023-08-01 09:39:47.831104 cognite_neat-0.18.3/cognite/neat/rules/examples/source-to-solution-mapping-rules.xlsx
+-rw-r--r--   0        0        0        0 2023-08-01 09:39:47.831104 cognite_neat-0.18.3/cognite/neat/rules/exporter/__init__.py
+-rw-r--r--   0        0        0      102 2023-08-01 09:39:47.831104 cognite_neat-0.18.3/cognite/neat/rules/exporter/core/__init__.py
+-rw-r--r--   0        0        0      610 2023-08-01 09:39:47.831104 cognite_neat-0.18.3/cognite/neat/rules/exporter/core/rules2labels.py
+-rw-r--r--   0        0        0       48 2023-08-01 09:39:47.831104 cognite_neat-0.18.3/cognite/neat/rules/exporter/dm/rules2dms.py
+-rw-r--r--   0        0        0     5403 2023-08-01 09:39:47.831104 cognite_neat-0.18.3/cognite/neat/rules/exporter/rules2graph_sheet.py
+-rw-r--r--   0        0        0     4763 2023-08-01 09:39:47.831104 cognite_neat-0.18.3/cognite/neat/rules/exporter/rules2graphql.py
+-rw-r--r--   0        0        0    15643 2023-08-01 09:39:47.831104 cognite_neat-0.18.3/cognite/neat/rules/exporter/rules2ontology.py
+-rw-r--r--   0        0        0     4019 2023-08-01 09:39:47.831104 cognite_neat-0.18.3/cognite/neat/rules/exporter/rules2rules.py
+-rw-r--r--   0        0        0      631 2023-08-01 09:39:47.831104 cognite_neat-0.18.3/cognite/neat/rules/exporter/rules2triples.py
+-rw-r--r--   0        0        0       63 2023-08-01 09:39:47.831104 cognite_neat-0.18.3/cognite/neat/rules/importer/__init__.py
+-rw-r--r--   0        0        0    13007 2023-08-01 09:39:47.831104 cognite_neat-0.18.3/cognite/neat/rules/importer/ontology2excel.py
+-rw-r--r--   0        0        0    24202 2023-08-01 09:39:47.831104 cognite_neat-0.18.3/cognite/neat/rules/models.py
+-rw-r--r--   0        0        0    13026 2023-08-01 09:39:47.831104 cognite_neat-0.18.3/cognite/neat/rules/parser.py
+-rw-r--r--   0        0        0     8231 2023-08-01 09:39:47.831104 cognite_neat-0.18.3/cognite/neat/rules/to_rdf_path.py
+-rw-r--r--   0        0        0        0 2023-08-01 09:39:47.831104 cognite_neat-0.18.3/cognite/neat/utils/__init__.py
+-rw-r--r--   0        0        0      309 2023-08-01 09:39:47.831104 cognite_neat-0.18.3/cognite/neat/utils/auxiliary.py
+-rw-r--r--   0        0        0      741 2023-08-01 09:39:47.831104 cognite_neat-0.18.3/cognite/neat/utils/cdf.py
+-rw-r--r--   0        0        0    10682 2023-08-01 09:39:47.831104 cognite_neat-0.18.3/cognite/neat/utils/utils.py
+-rw-r--r--   0        0        0      352 2023-08-01 09:39:47.831104 cognite_neat-0.18.3/cognite/neat/workflows/__init__.py
+-rw-r--r--   0        0        0    23792 2023-08-01 09:39:47.831104 cognite_neat-0.18.3/cognite/neat/workflows/base.py
+-rw-r--r--   0        0        0    17837 2023-08-01 09:39:47.831104 cognite_neat-0.18.3/cognite/neat/workflows/cdf_store.py
+-rw-r--r--   0        0        0      669 2023-08-01 09:39:47.831104 cognite_neat-0.18.3/cognite/neat/workflows/composition_based/data_contracts.py
+-rw-r--r--   0        0        0     1418 2023-08-01 09:39:47.831104 cognite_neat-0.18.3/cognite/neat/workflows/composition_based/step_model.py
+-rw-r--r--   0        0        0     2006 2023-08-01 09:39:47.831104 cognite_neat-0.18.3/cognite/neat/workflows/composition_based/steps.py
+-rw-r--r--   0        0        0     1442 2023-08-01 09:39:47.831104 cognite_neat-0.18.3/cognite/neat/workflows/examples/basic/workflow.py
+-rw-r--r--   0        0        0     1782 2023-08-01 09:39:47.831104 cognite_neat-0.18.3/cognite/neat/workflows/examples/basic/workflow.yaml
+-rw-r--r--   0        0        0    15758 2023-08-01 09:39:47.835104 cognite_neat-0.18.3/cognite/neat/workflows/examples/default/workflow.py
+-rw-r--r--   0        0        0     6774 2023-08-01 09:39:47.835104 cognite_neat-0.18.3/cognite/neat/workflows/examples/default/workflow.yaml
+-rw-r--r--   0        0        0     3681 2023-08-01 09:39:47.835104 cognite_neat-0.18.3/cognite/neat/workflows/examples/fdm_schema_generation/workflow.py
+-rw-r--r--   0        0        0     2573 2023-08-01 09:39:47.835104 cognite_neat-0.18.3/cognite/neat/workflows/examples/fdm_schema_generation/workflow.yaml
+-rw-r--r--   0        0        0    11480 2023-08-01 09:39:47.835104 cognite_neat-0.18.3/cognite/neat/workflows/examples/graph_db_import/workflow.py
+-rw-r--r--   0        0        0     4792 2023-08-01 09:39:47.835104 cognite_neat-0.18.3/cognite/neat/workflows/examples/graph_db_import/workflow.yaml
+-rw-r--r--   0        0        0      327 2023-08-01 09:39:47.835104 cognite_neat-0.18.3/cognite/neat/workflows/examples/graph_to_asset_hierarchy/workflow.py
+-rw-r--r--   0        0        0     8063 2023-08-01 09:39:47.835104 cognite_neat-0.18.3/cognite/neat/workflows/examples/graph_to_asset_hierarchy/workflow.yaml
+-rw-r--r--   0        0        0      277 2023-08-01 09:39:47.835104 cognite_neat-0.18.3/cognite/neat/workflows/examples/sheet2cdf/workflow.py
+-rw-r--r--   0        0        0     6668 2023-08-01 09:39:47.835104 cognite_neat-0.18.3/cognite/neat/workflows/examples/sheet2cdf/workflow.yaml
+-rw-r--r--   0        0        0      304 2023-08-01 09:39:47.835104 cognite_neat-0.18.3/cognite/neat/workflows/examples/sme_graph_capture/workflow.py
+-rw-r--r--   0        0        0     6837 2023-08-01 09:39:47.835104 cognite_neat-0.18.3/cognite/neat/workflows/examples/sme_graph_capture/workflow.yaml
+-rw-r--r--   0        0        0    16844 2023-08-01 09:39:47.835104 cognite_neat-0.18.3/cognite/neat/workflows/inheritance_based/graph2assets_relationships.py
+-rw-r--r--   0        0        0     7094 2023-08-01 09:39:47.835104 cognite_neat-0.18.3/cognite/neat/workflows/inheritance_based/remove_graphs_and_rules.py
+-rw-r--r--   0        0        0    14430 2023-08-01 09:39:47.835104 cognite_neat-0.18.3/cognite/neat/workflows/inheritance_based/sheet2cdf.py
+-rw-r--r--   0        0        0    11814 2023-08-01 09:39:47.835104 cognite_neat-0.18.3/cognite/neat/workflows/inheritance_based/sme_graph_capture.py
+-rw-r--r--   0        0        0    13125 2023-08-01 09:39:47.835104 cognite_neat-0.18.3/cognite/neat/workflows/manager.py
+-rw-r--r--   0        0        0        0 2023-08-01 09:39:47.835104 cognite_neat-0.18.3/cognite/neat/workflows/migration/__init__.py
+-rw-r--r--   0        0        0     1581 2023-08-01 09:39:47.835104 cognite_neat-0.18.3/cognite/neat/workflows/migration/wf_manifests.py
+-rw-r--r--   0        0        0     4907 2023-08-01 09:39:47.835104 cognite_neat-0.18.3/cognite/neat/workflows/model.py
+-rw-r--r--   0        0        0      774 2023-08-01 09:39:47.835104 cognite_neat-0.18.3/cognite/neat/workflows/tasks.py
+-rw-r--r--   0        0        0     6969 2023-08-01 09:39:47.835104 cognite_neat-0.18.3/cognite/neat/workflows/triggers.py
+-rw-r--r--   0        0        0      453 2023-08-01 09:39:47.835104 cognite_neat-0.18.3/cognite/neat/workflows/utils.py
+-rw-r--r--   0        0        0     2740 2023-08-01 09:39:48.315117 cognite_neat-0.18.3/pyproject.toml
+-rw-r--r--   0        0        0    10617 1970-01-01 00:00:00.000000 cognite_neat-0.18.3/PKG-INFO
```

### Comparing `cognite_neat-0.18.2/LICENSE` & `cognite_neat-0.18.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/README.md` & `cognite_neat-0.18.3/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/app/api/data_classes/rest.py` & `cognite_neat-0.18.3/cognite/neat/app/api/data_classes/rest.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/app/api/utils/query_templates.py` & `cognite_neat-0.18.3/cognite/neat/app/api/utils/query_templates.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/README.md` & `cognite_neat-0.18.3/cognite/neat/app/ui/neat-app/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/favicon.ico` & `cognite_neat-0.18.3/cognite/neat/app/ui/neat-app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/index.html` & `cognite_neat-0.18.3/cognite/neat/app/ui/neat-app/build/index.html`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/logo192.png` & `cognite_neat-0.18.3/cognite/neat/app/ui/neat-app/build/logo192.png`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css` & `cognite_neat-0.18.3/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map` & `cognite_neat-0.18.3/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/static/js/main.694f3f8e.js` & `cognite_neat-0.18.3/cognite/neat/app/ui/neat-app/build/static/js/main.694f3f8e.js`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/static/js/main.694f3f8e.js.LICENSE.txt` & `cognite_neat-0.18.3/cognite/neat/app/ui/neat-app/build/static/js/main.694f3f8e.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/static/js/main.694f3f8e.js.map` & `cognite_neat-0.18.3/cognite/neat/app/ui/neat-app/build/static/js/main.694f3f8e.js.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg` & `cognite_neat-0.18.3/cognite/neat/app/ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/config.py` & `cognite_neat-0.18.3/cognite/neat/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/exceptions.py` & `cognite_neat-0.18.3/cognite/neat/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.18.3/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/graph/extractors/data_stores/metrics.py` & `cognite_neat-0.18.3/cognite/neat/graph/extractors/data_stores/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/graph/extractors/data_stores/oxrdflib.py` & `cognite_neat-0.18.3/cognite/neat/graph/extractors/data_stores/oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/graph/extractors/graph_sheet_to_graph.py` & `cognite_neat-0.18.3/cognite/neat/graph/extractors/graph_sheet_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/graph/extractors/graph_store.py` & `cognite_neat-0.18.3/cognite/neat/graph/extractors/graph_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 import pyoxigraph
 import requests
 from prometheus_client import Gauge, Summary
 from rdflib import Graph, Namespace
 from rdflib.plugins.stores.sparqlstore import SPARQLUpdateStore
 from rdflib.query import Result
 
-from cognite.neat.app.api.configuration import DEFAULT_NAMESPACE, PREFIXES, RdfStoreType
+from cognite.neat.constants import PREFIXES, DEFAULT_NAMESPACE
 from cognite.neat.graph.extractors.data_stores import oxrdflib
+from cognite.neat.graph.extractors.data_stores.configuration import RdfStoreType
 from cognite.neat.graph.extractors.rdf_to_graph import rdf_file_to_graph
 
 prom_qsm = Summary("store_query_time_summary", "Time spent processing queries", ["query"])
 prom_sq = Gauge("store_single_query_time", "Time spent processing a single query", ["query"])
 
 
 class NeatGraphStore:
```

### Comparing `cognite_neat-0.18.2/cognite/neat/graph/extractors/mocks/graph.py` & `cognite_neat-0.18.3/cognite/neat/graph/extractors/mocks/graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/graph/extractors/rdf_to_graph.py` & `cognite_neat-0.18.3/cognite/neat/graph/extractors/rdf_to_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 
 from rdflib import Graph, Namespace
 
-from cognite.neat.app.api.configuration import DEFAULT_NAMESPACE, DEFAULT_URI, PREFIXES
+from cognite.neat.constants import DEFAULT_NAMESPACE, DEFAULT_URI, PREFIXES
 
 __all__ = ["rdf_file_to_graph"]
 
 
 def rdf_file_to_graph(
     filepath: Path,
     base_prefix: str = DEFAULT_URI,
```

### Comparing `cognite_neat-0.18.2/cognite/neat/graph/loaders/_exceptions.py` & `cognite_neat-0.18.3/cognite/neat/graph/loaders/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/graph/loaders/core/labels.py` & `cognite_neat-0.18.3/cognite/neat/graph/loaders/core/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/graph/loaders/core/models.py` & `cognite_neat-0.18.3/cognite/neat/graph/loaders/core/models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/graph/loaders/core/rdf_to_assets.py` & `cognite_neat-0.18.3/cognite/neat/graph/loaders/core/rdf_to_assets.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,28 @@
 from cognite.client import CogniteClient
 from cognite.client.data_classes import Asset, AssetHierarchy, AssetList
 from cognite.client.exceptions import CogniteDuplicatedError
 from deepdiff import DeepDiff
 from rdflib import Graph, Namespace
 from rdflib.term import URIRef
 
-from cognite.neat.app.api.configuration import EXCLUDE_PATHS
 from cognite.neat.graph.loaders.core.models import AssetTemplate
 from cognite.neat.graph.extractors.graph_store import NeatGraphStore
 from cognite.neat.rules.models import Property, TransformationRules
 from cognite.neat.utils.utils import chunker, datetime_utc_now, remove_namespace, retry_decorator
 
+EXCLUDE_PATHS = [
+    "root['labels']",
+    "root['metadata']['create_time']",
+    "root['metadata']['start_time']",
+    "root['metadata']['update_time']",
+    "root['metadata']['end_time']",
+    "root['metadata']['resurrection_time']",  # need to account for assets that are brought back to life
+]
+
 
 @dataclass
 class NeatMetadataKeys:
     start_time: str = "start_time"
     end_time: str = "end_time"
     update_time: str = "update_time"
     resurrection_time: str = "resurrection_time"
```

### Comparing `cognite_neat-0.18.2/cognite/neat/graph/loaders/core/rdf_to_relationships.py` & `cognite_neat-0.18.3/cognite/neat/graph/loaders/core/rdf_to_relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/graph/loaders/validator.py` & `cognite_neat-0.18.3/cognite/neat/graph/loaders/validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/graph/transformations/query_generator/sparql.py` & `cognite_neat-0.18.3/cognite/neat/graph/transformations/query_generator/sparql.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from rdflib import Graph, Namespace
 from rdflib.term import URIRef
 
-from cognite.neat.app.api.configuration import PREFIXES
+from cognite.neat.constants import PREFIXES
 from cognite.neat.rules.to_rdf_path import (
     AllProperties,
     AllReferences,
     Hop,
     SingleProperty,
     Traversal,
     Triple,
```

### Comparing `cognite_neat-0.18.2/cognite/neat/graph/transformations/transformer.py` & `cognite_neat-0.18.3/cognite/neat/graph/transformations/transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/rules/_exceptions.py` & `cognite_neat-0.18.3/cognite/neat/rules/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/rules/_parser.py` & `cognite_neat-0.18.3/cognite/neat/rules/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import pandas as pd
 import requests
 
 from rdflib import Namespace
 
 
 from cognite.neat.utils.auxiliary import local_import
-from cognite.neat.app.api.configuration import PREFIXES
+from cognite.neat.constants import PREFIXES
 from cognite.neat.rules import _exceptions
 from cognite.neat.rules.models import Class, Metadata, Property, RuleModel, TransformationRules
 
 
 @overload
 def parse_rules_from_excel_file(filepath: Path, return_report: Literal[False] = False) -> TransformationRules:
     ...
```

### Comparing `cognite_neat-0.18.2/cognite/neat/rules/_validation.py` & `cognite_neat-0.18.3/cognite/neat/rules/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/rules/analysis.py` & `cognite_neat-0.18.3/cognite/neat/rules/analysis.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/rules/examples/Rules-Nordic44-to-TNT.xlsx` & `cognite_neat-0.18.3/cognite/neat/rules/examples/Rules-Nordic44-to-TNT.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/rules/examples/power-grid-example.xlsx` & `cognite_neat-0.18.3/cognite/neat/rules/examples/power-grid-example.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/rules/examples/rules-template.xlsx` & `cognite_neat-0.18.3/cognite/neat/rules/examples/rules-template.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/rules/examples/sheet2cdf-transformation-rules.xlsx` & `cognite_neat-0.18.3/cognite/neat/rules/examples/sheet2cdf-transformation-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/rules/examples/source-to-solution-mapping-rules.xlsx` & `cognite_neat-0.18.3/cognite/neat/rules/examples/source-to-solution-mapping-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/rules/exporter/core/rules2labels.py` & `cognite_neat-0.18.3/cognite/neat/rules/exporter/core/rules2labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/rules/exporter/rules2graph_sheet.py` & `cognite_neat-0.18.3/cognite/neat/rules/exporter/rules2graph_sheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/rules/exporter/rules2graphql.py` & `cognite_neat-0.18.3/cognite/neat/rules/exporter/rules2graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/rules/exporter/rules2ontology.py` & `cognite_neat-0.18.3/cognite/neat/rules/exporter/rules2ontology.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/rules/exporter/rules2rules.py` & `cognite_neat-0.18.3/cognite/neat/rules/exporter/rules2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/rules/exporter/rules2triples.py` & `cognite_neat-0.18.3/cognite/neat/rules/exporter/rules2triples.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/rules/importer/ontology2excel.py` & `cognite_neat-0.18.3/cognite/neat/rules/importer/ontology2excel.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/rules/models.py` & `cognite_neat-0.18.3/cognite/neat/rules/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     model_validator,
     parse_obj_as,
     validator,
 )
 from pydantic.fields import FieldInfo
 from rdflib import XSD, Literal, Namespace, URIRef
 
-from cognite.neat.app.api.configuration import PREFIXES
+from cognite.neat.constants import PREFIXES
 
 # from . import _exceptions
 from cognite.neat.rules import _exceptions
 from cognite.neat.rules.to_rdf_path import Entity, RuleType, parse_rule
 
 __all__ = ["Class", "Instance", "Metadata", "Prefixes", "Property", "Resource", "TransformationRules"]
```

### Comparing `cognite_neat-0.18.2/cognite/neat/rules/to_rdf_path.py` & `cognite_neat-0.18.3/cognite/neat/rules/to_rdf_path.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/utils/cdf.py` & `cognite_neat-0.18.3/cognite/neat/utils/cdf.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/utils/utils.py` & `cognite_neat-0.18.3/cognite/neat/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/workflows/base.py` & `cognite_neat-0.18.3/cognite/neat/workflows/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,17 @@
     WorkflowStepEvent,
     WorkflowSystemComponent,
 )
 from cognite.neat.workflows.tasks import WorkflowTaskBuilder
 
 from cognite.neat.app.api.configuration import Config
 from cognite.neat.utils.cdf import CogniteClientConfig
-from . import utils, cdf_store
-from .step_model import DataContract
-import cognite.neat.workflows.steps.steps
+from cognite.neat.workflows import utils, cdf_store
+from cognite.neat.workflows.composition_based.step_model import DataContract
+import cognite.neat.workflows.composition_based.steps
 
 summary_metrics = Gauge("neat_workflow_summary_metrics", "Workflow execution summary metrics", ["wf_name", "name"])
 steps_metrics = Gauge("neat_workflow_steps_metrics", "Workflow step level metrics", ["wf_name", "step_name", "name"])
 timing_metrics = Gauge("neat_workflow_timing_metrics", "Workflow timing metrics", ["wf_name", "component", "name"])
 
 
 class BaseWorkflow:
@@ -254,29 +254,32 @@
                     component_name=f"wf step runner , step.id = {step.id}",
                 )
                 def method_runner():
                     return method(flow_message)
 
                 new_flow_message = method_runner()
             elif step.stype == StepType.STD_STEP:
-                for name, step_cls in inspect.getmembers(cognite.neat.workflows.steps.steps):
+                for name, step_cls in inspect.getmembers(cognite.neat.workflows.composition_based.steps):
                     if inspect.isclass(step_cls):
                         if name == step.method:
                             step_obj = step_cls(self.metrics)
                             step_obj.set_global_configs(self.cdf_client, self.data_store_path, self.rules_storage_path)
                             signature = inspect.signature(step_obj.run)
                             parameters = signature.parameters
                             is_valid = True
                             input_data = []
                             missing_data = []
                             for parameter in parameters.values():
                                 try:
                                     if parameter.annotation.__name__ == "FlowMessage":
                                         input_data.append(self.flow_message)
                                     else:
+                                        # Comment: self.data is suppose to be a dict of data contracts
+                                        # but it's not set anywhere. It is unclear where and how this
+                                        # this is suppose to be set
                                         input_data.append(self.data[parameter.annotation.__name__])
                                 except KeyError:
                                     is_valid = False
                                     logging.error(f"Missing data for step {step.id} parameter {parameter.name}")
                                     missing_data.append(parameter.annotation.__name__)
                                     continue
                             if not is_valid:
@@ -443,27 +446,27 @@
         )
         if output_format == "json":
             return json.dumps(workflow_definitions.model_dump(), indent=4)
         elif output_format == "yaml":
             return yaml.dump(workflow_definitions.model_dump(), indent=4)
 
     @classmethod
-    def deserialize_metadata(cls, json_string: str, output_format: str = "json") -> WorkflowDefinition:
+    def deserialize_definition(cls, json_string: str, output_format: str = "json") -> WorkflowDefinition:
         if output_format == "json":
             workflow_definitions = WorkflowDefinition.model_validate(json.loads(json_string))
         elif output_format == "yaml":
             workflow_definitions = WorkflowDefinition.model_validate(yaml.load(json_string, Loader=yaml.Loader))
         else:
             raise NotImplementedError(f"Output format {output_format} is not supported.")
         return workflow_definitions
 
-    def set_metadata(self, metadata: WorkflowDefinition):
-        self.workflow_steps = metadata.steps
-        self.workflow_system_components = metadata.system_components
-        self.configs = metadata.configs
+    def set_definition(self, workflow_definition: WorkflowDefinition):
+        self.workflow_steps = workflow_definition.steps
+        self.workflow_system_components = workflow_definition.system_components
+        self.configs = workflow_definition.configs
 
     def set_storage_path(self, storage_type: str, storage_path: str):
         if storage_type == "transformation_rules":
             self.rules_storage_path = storage_path
         elif storage_type == "data_store":
             self.data_store_path = storage_path
```

### Comparing `cognite_neat-0.18.2/cognite/neat/workflows/base_workflows/graphs_and_rules.py` & `cognite_neat-0.18.3/cognite/neat/workflows/inheritance_based/remove_graphs_and_rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import logging
 from pathlib import Path
 
 from cognite.client import CogniteClient
 
 from cognite.neat import rules
 from cognite.neat.graph import extractors
-from cognite.neat.app.api.configuration import PREFIXES
+from cognite.neat.constants import PREFIXES
 from cognite.neat.graph.extractors import NeatGraphStore, drop_graph_store
 from cognite.neat.rules.exporter.rules2triples import get_instances_as_triples
 from cognite.neat.rules.models import TransformationRules
 from cognite.neat.graph.transformations.transformer import RuleProcessingReport, domain2app_knowledge_graph
 from cognite.neat.workflows import utils
-from cognite.neat.workflows.base import BaseWorkflow, FlowMessage
+from cognite.neat.workflows.base import BaseWorkflow
+from cognite.neat.workflows.model import FlowMessage
 from cognite.neat.workflows.cdf_store import CdfStore
 
 
 class GraphsAndRulesBaseWorkflow(BaseWorkflow):
     def __init__(self, name: str, client: CogniteClient):
         super().__init__(name, client, [])
         self.dataset_id: int = 0
```

### Comparing `cognite_neat-0.18.2/cognite/neat/workflows/base_workflows/sheet2cdf.py` & `cognite_neat-0.18.3/cognite/neat/workflows/inheritance_based/sheet2cdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,16 @@
     upload_relationships,
 )
 from cognite.neat.graph.extractors import NeatGraphStore
 from cognite.neat.rules.exporter.rules2triples import get_instances_as_triples
 from cognite.neat.rules.models import TransformationRules
 from cognite.neat.graph.loaders.validator import validate_asset_hierarchy
 from cognite.neat.workflows import utils
-from cognite.neat.workflows.base import BaseWorkflow, FlowMessage
+from cognite.neat.workflows.base import BaseWorkflow
+from cognite.neat.workflows.model import FlowMessage
 from cognite.neat.workflows.cdf_store import CdfStore
 
 with contextlib.suppress(ValueError):
     prom_cdf_resource_stats = Gauge(
         "neat_sheet2cdf_cdf_resource_stats",
         "CDF resource stats before and after running sheet2cdf workflow",
         ["resource_type", "state"],
```

### Comparing `cognite_neat-0.18.2/cognite/neat/workflows/base_workflows/sme_graph_capture.py` & `cognite_neat-0.18.3/cognite/neat/workflows/inheritance_based/sme_graph_capture.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,16 @@
     upload_relationships,
 )
 from cognite.neat.graph.extractors import NeatGraphStore
 from cognite.neat.rules.models import TransformationRules
 from cognite.neat.utils.utils import add_triples
 from cognite.neat.graph.loaders.validator import validate_asset_hierarchy
 from cognite.neat.workflows import utils
-from cognite.neat.workflows.base import BaseWorkflow, FlowMessage
+from cognite.neat.workflows.base import BaseWorkflow
+from cognite.neat.workflows.model import FlowMessage
 from cognite.neat.workflows.cdf_store import CdfStore
 
 
 class SmeGraphCaptureBaseWorkflow(BaseWorkflow):
     def __init__(self, name: str, client: CogniteClient):
         super().__init__(name, client, [])
         self.counter = 0
```

### Comparing `cognite_neat-0.18.2/cognite/neat/workflows/cdf_store.py` & `cognite_neat-0.18.3/cognite/neat/workflows/cdf_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/workflows/examples/basic/workflow.py` & `cognite_neat-0.18.3/cognite/neat/workflows/examples/basic/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/workflows/examples/basic/workflow.yaml` & `cognite_neat-0.18.3/cognite/neat/workflows/examples/basic/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/workflows/examples/default/workflow.py` & `cognite_neat-0.18.3/cognite/neat/workflows/examples/default/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 )
 from cognite.neat.graph.extractors import NeatGraphStore, drop_graph_store
 from cognite.neat.rules.exporter.rules2triples import get_instances_as_triples
 from cognite.neat.rules.models import TransformationRules
 from cognite.neat.graph.transformations.transformer import RuleProcessingReport, domain2app_knowledge_graph
 from cognite.neat.graph.loaders.validator import validate_asset_hierarchy
 from cognite.neat.workflows import utils
-from cognite.neat.workflows.base import BaseWorkflow, FlowMessage
+from cognite.neat.workflows.base import BaseWorkflow
+from cognite.neat.workflows.model import FlowMessage
 from cognite.neat.workflows.cdf_store import CdfStore
 
 with contextlib.suppress(ValueError):
     prom_cdf_resource_stats = Gauge(
         "neat_default_wf_cdf_resource_stats",
         "CDF resource stats before and after running default workflow",
         ["resource_type", "state"],
@@ -115,15 +116,15 @@
                 logging.error(f"Failed to query most likely remote DB is not running {e}")
                 raise Exception("Failed to query graph , most likely remote DB is not running") from e
             else:
                 logging.info(f"Loaded {len(result.bindings)} classes")
         elif self.graph_source_type.lower() in ("memory", "oxigraph"):
             if source_file := self.get_config_item_value("source_rdf_store.file"):
                 # Todo avoid hard-coding adjacent path
-                graphs = Path(self.data_store_path) / "source_graphs"
+                graphs = Path(self.data_store_path) / "source-graphs"
                 self.source_graph.import_from_file(graphs / source_file)
                 logging.info(f"Loaded {source_file} into source graph.")
             else:
                 raise ValueError("You need a source_rdf_store.file specified for source_rdf_store.type=memory")
         else:
             raise NotImplementedError(f"Graph type {self.graph_source_type} is not supported.")
```

### Comparing `cognite_neat-0.18.2/cognite/neat/workflows/examples/default/workflow.yaml` & `cognite_neat-0.18.3/cognite/neat/workflows/examples/default/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/workflows/examples/fdm_schema_generation/workflow.py` & `cognite_neat-0.18.3/cognite/neat/workflows/examples/fdm_schema_generation/workflow.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import logging
+import os
 import time
 from pathlib import Path
 
 from cognite.client import CogniteClient
 
 from cognite.neat import rules
 from cognite.neat.rules.exporter.rules2graphql import GraphQLSchema
 from cognite.neat.graph.extractors import NeatGraphStore
 from cognite.neat.rules.models import TransformationRules
 from cognite.neat.workflows import utils
-from cognite.neat.workflows.base import BaseWorkflow, FlowMessage
+from cognite.neat.workflows.base import BaseWorkflow
+from cognite.neat.workflows.model import FlowMessage
 from cognite.neat.workflows.cdf_store import CdfStore
 
 
 class FDMSchemaGenerationNeatWorkflow(BaseWorkflow):
     def __init__(self, name: str, client: CogniteClient):
         super().__init__(name, client, [])
         self.counter = 0
@@ -54,22 +56,24 @@
         logging.info(f"Loaded prefixes {str(self.transformation_rules.prefixes)} rules")
         output_text = f"Loaded {len(self.transformation_rules.properties)} rules"
         logging.info(output_text)
         return FlowMessage(output_text=output_text)
 
     def step_generate_fdm_schema(self, flow_msg: FlowMessage = None):
         logging.info("Generating FDM schema")
-        self.data_model_gql = GraphQLSchema(self.transformation_rules, verbose=True).schema
+        self.data_model_gql = GraphQLSchema.from_rules(self.transformation_rules, verbose=True).schema
 
         default_name = (
             f"{self.transformation_rules.metadata.prefix}-"
             f"v{self.transformation_rules.metadata.version.strip().replace('.', '_')}"
             ".graphql"
         )
         schema_name = self.get_config_item_value("fdm_schema.file", default_name)
+
+        os.makedirs(self.rules_storage_path.parent / "data-models", exist_ok=True)
         fdm_path = self.rules_storage_path.parent / "data-models" / schema_name
 
         with open(fdm_path, "w") as fdm_file:
             fdm_file.write(self.data_model_gql)
 
         output_text = (
             "FDM Schema generated and can be downloaded here : "
```

### Comparing `cognite_neat-0.18.2/cognite/neat/workflows/examples/fdm_schema_generation/workflow.yaml` & `cognite_neat-0.18.3/cognite/neat/workflows/examples/fdm_schema_generation/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/workflows/examples/graph_db_import/workflow.py` & `cognite_neat-0.18.3/cognite/neat/workflows/examples/graph_db_import/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from pathlib import Path
 
 import requests
 from cognite.client import CogniteClient
 
 from cognite.neat.graph.extractors import NeatGraphStore
 from cognite.neat.rules.models import TransformationRules
-from cognite.neat.workflows import BaseWorkflow, FlowMessage
+from cognite.neat.workflows.base import BaseWorkflow
+from cognite.neat.workflows.model import FlowMessage
 
 
 class GraphDbImportNeatWorkflow(BaseWorkflow):
     def __init__(self, name: str, client: CogniteClient):
         super().__init__(name, client, [])
         self.dataset_id: int = 0
         self.current_step: str = None
```

### Comparing `cognite_neat-0.18.2/cognite/neat/workflows/examples/graph_db_import/workflow.yaml` & `cognite_neat-0.18.3/cognite/neat/workflows/examples/graph_db_import/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/workflows/examples/graph_to_asset_hierarchy/workflow.yaml` & `cognite_neat-0.18.3/cognite/neat/workflows/examples/graph_to_asset_hierarchy/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/workflows/examples/sheet2cdf/workflow.yaml` & `cognite_neat-0.18.3/cognite/neat/workflows/examples/sheet2cdf/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/workflows/examples/sme_graph_capture/workflow.yaml` & `cognite_neat-0.18.3/cognite/neat/workflows/examples/sme_graph_capture/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/workflows/manager.py` & `cognite_neat-0.18.3/cognite/neat/workflows/manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -57,102 +57,129 @@
         self.rules_storage_path = rules_storage_path if rules_storage_path else Path("rules")
         self.task_builder = WorkflowTaskBuilder(client, self)
 
     def update_cdf_client(self, client: CogniteClient):
         self.client = client
         self.task_builder = WorkflowTaskBuilder(client, self)
         self.workflow_registry = {}
-        self.load_workflows_from_storage_v2()
+        self.load_workflows_from_storage()
 
     def get_list_of_workflows(self):
         return list(self.workflow_registry.keys())
 
     def get_workflow(self, name: str) -> BaseWorkflow:
         return self.workflow_registry[name]
 
     def start_workflow(self, name: str, sync=False, **kwargs):
         workflow = self.get_workflow(name)
         workflow.start(sync, kwargs=kwargs)
         return workflow
 
     def delete_workflow(self, name: str):
         del self.workflow_registry[name]
-        return
 
     def update_workflow(self, name: str, workflow: WorkflowDefinition):
         self.workflow_registry[name].workflow_steps = workflow.steps
         self.workflow_registry[name].configs = workflow.configs
         self.workflow_registry[name].workflow_system_components = workflow.system_components
-        return
 
     def save_workflow_to_storage(self, name: str, custom_implementation_module: str = None):
         """Save workflow from memory to storage"""
         if self.workflows_storage_type == "file":
             full_path = self.workflows_storage_path / name / "workflow.yaml"
             wf = self.workflow_registry[name]
             with open(full_path, "w") as f:
                 f.write(
                     wf.serialize_workflow(
                         output_format="yaml", custom_implementation_module=custom_implementation_module
                     )
                 )
 
-    def load_workflows_from_storage_v2(self, dir_path: str = None):
+    def load_workflows_from_storage(self, workflows_storage_path: str | Path = None):
         """Loads workflows from disk/storage into memory, initializes and register them in the workflow registry"""
-        if dir_path:
-            dir_path = Path(dir_path)
-        else:
-            dir_path = self.workflows_storage_path
-        sys.path.append(str(dir_path))
-        for wf_module_name in os.listdir(dir_path):
-            wf_module_full_path = dir_path / wf_module_name
-            if wf_module_full_path.is_dir():
+
+        # set workflow storage path
+        workflows_storage_path = Path(workflows_storage_path) if workflows_storage_path else self.workflows_storage_path
+
+        # set system path to be used when importing individual workflows as python modules
+        # via importlib.import_module(...)
+        sys.path.append(str(workflows_storage_path))
+
+        for workflow_name in os.listdir(workflows_storage_path):
+            workflow_path = workflows_storage_path / workflow_name
+            # THIS IS WHERE WE LOAD THE WORKFLOW MODULES
+            if workflow_path.is_dir():
+                logging.info(f"Loading workflow {workflow_name} from {workflow_path}")
                 try:
-                    logging.info(f"Loading workflow {wf_module_name} from {wf_module_full_path}")
-                    # metadata_file = f"{dir_path}//{module_name}.yaml"
-                    metadata_file = dir_path / wf_module_name / "workflow.yaml"
-                    logging.info(f"Loading workflow {wf_module_name} metadata from {metadata_file}")
-                    if os.path.exists(metadata_file):
-                        with open(metadata_file, "r") as f:
-                            wf_str = f.read()
-                            metadata = BaseWorkflow.deserialize_metadata(wf_str, output_format="yaml")
+                    workflow_definition_path = workflow_path / "workflow.yaml"
+                    logging.info(f"Loading workflow {workflow_name} definition from {workflow_definition_path}")
+                    if os.path.exists(workflow_definition_path):
+                        with open(workflow_definition_path, "r") as workflow_definition_file:
+                            workflow_definition: WorkflowDefinition = BaseWorkflow.deserialize_definition(
+                                workflow_definition_file.read(), output_format="yaml"
+                            )
                     else:
-                        logging.info(f"Metadata file {metadata_file} not found, skipping")
+                        logging.info(f"Definition file {workflow_definition_path} not found, skipping")
                         continue
 
-                    if metadata.implementation_module:
-                        wf_module_name = metadata.implementation_module
-                        logging.info(f"Loading CUSTOM workflow module {wf_module_name}")
+                    # Comment: All our workflows implementation_module is None
+                    # what is this meant for ?, just to have different name?
+                    if workflow_definition.implementation_module:
+                        workflow_name = workflow_definition.implementation_module
+                        logging.info(f"Loading CUSTOM workflow module {workflow_name}")
                     else:
-                        logging.info(f"Loading workflow module {wf_module_name}")
+                        logging.info(f"Loading workflow module {workflow_name}")
 
-                    full_module_name = f"{wf_module_name}.workflow"
+                    full_module_name = f"{workflow_name}.workflow"
                     if full_module_name in sys.modules:
-                        logging.info(f"Reloading existing workflow module {wf_module_name}")
+                        logging.info(f"Reloading existing workflow module {workflow_name}")
                         module = importlib.reload(sys.modules[full_module_name])
                     else:
-                        logging.info(f"Loading NEW workflow module {wf_module_name}")
+                        logging.info(f"Loading NEW workflow module {workflow_name}")
+                        logging.info(f"Loading NEW workflow module {full_module_name}")
                         module = importlib.import_module(full_module_name)
-                    # dynamically load all classes in the module
+
+                    # Dynamically load workflow classes which contain "NeatWorkflow" in their name
+                    # from workflow.py module in the workflow directory and
+                    # Instantiate them using the workflow definition loaded
+                    # from workflow.yaml file
                     for name, obj in inspect.getmembers(module):
-                        if "NeatWorkflow" not in name:
-                            continue
-                        logging.info(f"Found class {name} in module {wf_module_name}")
-                        if inspect.isclass(obj):
-                            self.workflow_registry[wf_module_name] = obj(wf_module_name, self.client)
-                            self.workflow_registry[wf_module_name].set_metadata(metadata)
-                            self.workflow_registry[wf_module_name].set_task_builder(self.task_builder)
-                            self.workflow_registry[wf_module_name].set_default_dataset_id(self.data_set_id)
-                            self.workflow_registry[wf_module_name].set_storage_path(
-                                "transformation_rules", self.rules_storage_path
+                        if "NeatWorkflow" in name and inspect.isclass(obj):
+                            logging.info(
+                                (
+                                    f"Found class {name} in module {workflow_name},"
+                                    f" registering it as '{workflow_name}' in the workflow registry"
+                                )
                             )
-                            self.workflow_registry[wf_module_name].set_storage_path("data_store", self.data_store_path)
+                            self.register_workflow(obj, workflow_name, workflow_definition)
+
                 except Exception as e:
                     trace = traceback.format_exc()
-                    logging.error(f"Error loading workflow {wf_module_name}: error: {e} trace : {trace}")
+                    logging.error(f"Error loading workflow {workflow_name}: error: {e} trace : {trace}")
+
+    def register_workflow(self, obj, workflow_name, workflow_definition):
+        """Register workflow in the workflow registry
+
+        Parameters
+        ----------
+        obj : BaseWorkflow
+            Class of the workflow to be registered
+        workflow_name : _type_
+            Name of the workflow to be registered
+        workflow_definition : _type_
+            Definition of the workflow to be registered originating from workflow.yaml
+        """
+        self.workflow_registry[workflow_name] = obj(workflow_name, self.client)
+        self.workflow_registry[workflow_name].set_definition(workflow_definition)
+        # Comment: Not entirely sure what is task_builder meant for
+        # as at first glance it looks like circular import ???
+        self.workflow_registry[workflow_name].set_task_builder(self.task_builder)
+        self.workflow_registry[workflow_name].set_default_dataset_id(self.data_set_id)
+        self.workflow_registry[workflow_name].set_storage_path("transformation_rules", self.rules_storage_path)
+        self.workflow_registry[workflow_name].set_storage_path("data_store", self.data_store_path)
 
     def create_workflow_instance(self, template_name: str, add_to_registry: bool = True) -> BaseWorkflow:
         new_instance = self.workflow_registry[template_name].copy()
         if add_to_registry:
             self.ephemeral_instance_registry[new_instance.instance_id] = new_instance
         live_workflow_instances.labels(itype="ephemeral").set(len(self.ephemeral_instance_registry))
         return new_instance
```

### Comparing `cognite_neat-0.18.2/cognite/neat/workflows/migration/wf_manifests.py` & `cognite_neat-0.18.3/cognite/neat/workflows/migration/wf_manifests.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/workflows/model.py` & `cognite_neat-0.18.3/cognite/neat/workflows/model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/cognite/neat/workflows/steps/data_contracts.py` & `cognite_neat-0.18.3/cognite/neat/workflows/composition_based/data_contracts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 
 from cognite.client import CogniteClient
 
 from cognite.neat.graph.extractors import NeatGraphStore
 from cognite.neat.rules.models import TransformationRules
-from cognite.neat.workflows.step_model import DataContract
+from cognite.neat.workflows.composition_based.step_model import DataContract
 
 
 class RulesData(DataContract):
     rules: TransformationRules
 
     @property
     def dataset_id(self) -> int:
```

### Comparing `cognite_neat-0.18.2/cognite/neat/workflows/steps/steps.py` & `cognite_neat-0.18.3/cognite/neat/workflows/composition_based/steps.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 from pathlib import Path
 from typing import Optional, Tuple
 
-from ...graph import extractors
+from cognite.neat.graph import extractors
 from cognite.neat.graph.loaders import upload_labels
 from cognite.neat.rules import parse_rules_from_excel_file
 from cognite.neat.workflows.model import FlowMessage
-from cognite.neat.workflows.step_model import Step
+from cognite.neat.workflows.composition_based.step_model import Step
 from .data_contracts import ClientData, PathData, RulesData, SourceGraphData
 
 __all__ = [
     "LoadTransformationRules",
     "ConfiguringStores",
     "LoadInstancesToGraph",
     "CreateCDFLabels",
```

### Comparing `cognite_neat-0.18.2/cognite/neat/workflows/tasks.py` & `cognite_neat-0.18.3/cognite/neat/workflows/tasks.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 from cognite.neat.workflows.model import FlowMessage
 
 
 class WorkflowTaskBuilder:
     """Collection of all base tasks for workflows.All tasks must run in the context of a workflow including threads."""
 
-    def __init__(self, cdf_client: CogniteClient, worflow_manager):
-        # TODO : figure out ciclura import and set type to WorkflowManager
+    def __init__(self, cdf_client: CogniteClient, workflow_manager):
+        # TODO : figure out circular import and set type to WorkflowManager
         self.cdf_client = cdf_client
-        self.workflow_manager = worflow_manager
+        self.workflow_manager = workflow_manager
 
     def start_workflow_task(self, workflow_name: str, sync: bool, flow_message: FlowMessage):
         """Call a workflow task from another workflow"""
         return self.workflow_manager.start_workflow_instance(
             workflow_name=workflow_name, flow_msg=flow_message, sync=sync
         )
```

### Comparing `cognite_neat-0.18.2/cognite/neat/workflows/triggers.py` & `cognite_neat-0.18.3/cognite/neat/workflows/triggers.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.2/pyproject.toml` & `cognite_neat-0.18.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-neat"
-version = "0.18.2"
+version = "0.18.3"
 readme = "README.md"
 description = "Knowledge graph transformation"
 authors = ["Nikola Vasiljevic <nikola.vasiljevic@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>",
     "Aleksandrs Livincovs <aleksandrs.livincovs@cognite.com>"]
 license = "Apache-2.0"
 documentation = "https://cognite-neat.readthedocs-hosted.com/"
```

### Comparing `cognite_neat-0.18.2/PKG-INFO` & `cognite_neat-0.18.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-neat
-Version: 0.18.2
+Version: 0.18.3
 Summary: Knowledge graph transformation
 Home-page: https://cognite-neat.readthedocs-hosted.com/
 License: Apache-2.0
 Author: Nikola Vasiljevic
 Author-email: nikola.vasiljevic@cognite.com
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
```

