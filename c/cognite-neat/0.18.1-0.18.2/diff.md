# Comparing `tmp/cognite_neat-0.18.1.tar.gz` & `tmp/cognite_neat-0.18.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_neat-0.18.1.tar", max compression
+gzip compressed data, was "cognite_neat-0.18.2.tar", max compression
```

## Comparing `cognite_neat-0.18.1.tar` & `cognite_neat-0.18.2.tar`

### file list

```diff
@@ -1,122 +1,117 @@
--rw-r--r--   0        0        0    11351 2023-07-26 07:32:45.209853 cognite_neat-0.18.1/LICENSE
--rw-r--r--   0        0        0     8765 2023-07-26 07:32:45.209853 cognite_neat-0.18.1/README.md
--rw-r--r--   0        0        0       61 2023-07-26 07:32:45.209853 cognite_neat-0.18.1/cognite/neat/__init__.py
--rw-r--r--   0        0        0       23 2023-07-26 07:32:45.209853 cognite_neat-0.18.1/cognite/neat/_version.py
--rw-r--r--   0        0        0        0 2023-07-26 07:32:45.209853 cognite_neat-0.18.1/cognite/neat/app/api/__init__.py
--rw-r--r--   0        0        0     2805 2023-07-26 07:32:45.209853 cognite_neat-0.18.1/cognite/neat/app/api/app.py
--rw-r--r--   0        0        0     5611 2023-07-26 07:32:45.209853 cognite_neat-0.18.1/cognite/neat/app/api/configuration.py
--rw-r--r--   0        0        0        0 2023-07-26 07:32:45.209853 cognite_neat-0.18.1/cognite/neat/app/api/data_classes/__init__.py
--rw-r--r--   0        0        0     1390 2023-07-26 07:32:45.209853 cognite_neat-0.18.1/cognite/neat/app/api/data_classes/rest.py
--rw-r--r--   0        0        0    24133 2023-07-26 07:32:45.209853 cognite_neat-0.18.1/cognite/neat/app/api/explorer.py
--rw-r--r--   0        0        0        0 2023-07-26 07:32:45.209853 cognite_neat-0.18.1/cognite/neat/app/api/utils/__init__.py
--rw-r--r--   0        0        0      412 2023-07-26 07:32:45.209853 cognite_neat-0.18.1/cognite/neat/app/api/utils/data_mapping.py
--rw-r--r--   0        0        0     4622 2023-07-26 07:32:45.209853 cognite_neat-0.18.1/cognite/neat/app/api/utils/query_templates.py
--rw-r--r--   0        0        0      357 2023-07-26 07:32:45.209853 cognite_neat-0.18.1/cognite/neat/app/main.py
--rw-r--r--   0        0        0       16 2023-07-26 07:32:45.209853 cognite_neat-0.18.1/cognite/neat/app/ui/index.html
--rw-r--r--   0        0        0      312 2023-07-26 07:32:45.209853 cognite_neat-0.18.1/cognite/neat/app/ui/neat-app/.gitignore
--rw-r--r--   0        0        0     3359 2023-07-26 07:32:45.209853 cognite_neat-0.18.1/cognite/neat/app/ui/neat-app/README.md
--rw-r--r--   0        0        0      464 2023-07-26 07:32:45.209853 cognite_neat-0.18.1/cognite/neat/app/ui/neat-app/build/asset-manifest.json
--rw-r--r--   0        0        0     3870 2023-07-26 07:32:45.209853 cognite_neat-0.18.1/cognite/neat/app/ui/neat-app/build/favicon.ico
--rw-r--r--   0        0        0      630 2023-07-26 07:32:45.209853 cognite_neat-0.18.1/cognite/neat/app/ui/neat-app/build/index.html
--rw-r--r--   0        0        0     5347 2023-07-26 07:32:45.209853 cognite_neat-0.18.1/cognite/neat/app/ui/neat-app/build/logo192.png
--rw-r--r--   0        0        0      492 2023-07-26 07:32:45.209853 cognite_neat-0.18.1/cognite/neat/app/ui/neat-app/build/manifest.json
--rw-r--r--   0        0        0       67 2023-07-26 07:32:45.209853 cognite_neat-0.18.1/cognite/neat/app/ui/neat-app/build/robots.txt
--rw-r--r--   0        0        0     8524 2023-07-26 07:32:45.209853 cognite_neat-0.18.1/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
--rw-r--r--   0        0        0    13319 2023-07-26 07:32:45.209853 cognite_neat-0.18.1/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
--rw-r--r--   0        0        0  1370405 2023-07-26 07:32:45.217853 cognite_neat-0.18.1/cognite/neat/app/ui/neat-app/build/static/js/main.694f3f8e.js
--rw-r--r--   0        0        0     2667 2023-07-26 07:32:45.217853 cognite_neat-0.18.1/cognite/neat/app/ui/neat-app/build/static/js/main.694f3f8e.js.LICENSE.txt
--rw-r--r--   0        0        0  5883860 2023-07-26 07:32:45.245853 cognite_neat-0.18.1/cognite/neat/app/ui/neat-app/build/static/js/main.694f3f8e.js.map
--rw-r--r--   0        0        0     2633 2023-07-26 07:32:45.245853 cognite_neat-0.18.1/cognite/neat/app/ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
--rw-r--r--   0        0        0      884 2023-07-26 07:32:45.249853 cognite_neat-0.18.1/cognite/neat/constants.py
--rw-r--r--   0        0        0     1276 2023-07-26 07:32:45.249853 cognite_neat-0.18.1/cognite/neat/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-26 07:32:45.249853 cognite_neat-0.18.1/cognite/neat/graph/__init__.py
--rw-r--r--   0        0        0      442 2023-07-26 07:32:45.249853 cognite_neat-0.18.1/cognite/neat/graph/extractors/__init__.py
--rw-r--r--   0        0        0      711 2023-07-26 07:32:45.249853 cognite_neat-0.18.1/cognite/neat/graph/extractors/config.py
--rw-r--r--   0        0        0        0 2023-07-26 07:32:45.249853 cognite_neat-0.18.1/cognite/neat/graph/extractors/data_stores/__init__.py
--rw-r--r--   0        0        0     1520 2023-07-26 07:32:45.249853 cognite_neat-0.18.1/cognite/neat/graph/extractors/data_stores/metrics.py
--rw-r--r--   0        0        0     9436 2023-07-26 07:32:45.249853 cognite_neat-0.18.1/cognite/neat/graph/extractors/data_stores/oxrdflib.py
--rw-r--r--   0        0        0     7255 2023-07-26 07:32:45.249853 cognite_neat-0.18.1/cognite/neat/graph/extractors/graph_sheet_to_graph.py
--rw-r--r--   0        0        0    11434 2023-07-26 07:32:45.249853 cognite_neat-0.18.1/cognite/neat/graph/extractors/graph_store.py
--rw-r--r--   0        0        0       68 2023-07-26 07:32:45.249853 cognite_neat-0.18.1/cognite/neat/graph/extractors/mocks/__init__.py
--rw-r--r--   0        0        0    12883 2023-07-26 07:32:45.249853 cognite_neat-0.18.1/cognite/neat/graph/extractors/mocks/graph.py
--rw-r--r--   0        0        0     1213 2023-07-26 07:32:45.249853 cognite_neat-0.18.1/cognite/neat/graph/extractors/rdf_to_graph.py
--rw-r--r--   0        0        0      432 2023-07-26 07:32:45.249853 cognite_neat-0.18.1/cognite/neat/graph/loaders/__init__.py
--rw-r--r--   0        0        0     2837 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/graph/loaders/_exceptions.py
--rw-r--r--   0        0        0        0 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/graph/loaders/core/__init__.py
--rw-r--r--   0        0        0     2279 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/graph/loaders/core/labels.py
--rw-r--r--   0        0        0     5043 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/graph/loaders/core/models.py
--rw-r--r--   0        0        0    39898 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/graph/loaders/core/rdf_to_assets.py
--rw-r--r--   0        0        0    20925 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/graph/loaders/core/rdf_to_relationships.py
--rw-r--r--   0        0        0     2650 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/graph/loaders/validator.py
--rw-r--r--   0        0        0        0 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/graph/transformations/__init__.py
--rw-r--r--   0        0        0       73 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/graph/transformations/query_generator/__init__.py
--rw-r--r--   0        0        0     9592 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/graph/transformations/query_generator/sparql.py
--rw-r--r--   0        0        0    11892 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/graph/transformations/transformer.py
--rw-r--r--   0        0        0      290 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/rules/__init__.py
--rw-r--r--   0        0        0    49672 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/rules/_exceptions.py
--rw-r--r--   0        0        0    13038 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/rules/_parser.py
--rw-r--r--   0        0        0     3496 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/rules/_validation.py
--rw-r--r--   0        0        0     4777 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/rules/analysis.py
--rw-r--r--   0        0        0        0 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/rules/exporter/__init__.py
--rw-r--r--   0        0        0      102 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/rules/exporter/core/__init__.py
--rw-r--r--   0        0        0      610 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/rules/exporter/core/rules2labels.py
--rw-r--r--   0        0        0       48 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/rules/exporter/dm/rules2dms.py
--rw-r--r--   0        0        0     5403 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/rules/exporter/rules2graph_sheet.py
--rw-r--r--   0        0        0     4763 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/rules/exporter/rules2graphql.py
--rw-r--r--   0        0        0    15643 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/rules/exporter/rules2ontology.py
--rw-r--r--   0        0        0     4019 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/rules/exporter/rules2rules.py
--rw-r--r--   0        0        0      631 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/rules/exporter/rules2triples.py
--rw-r--r--   0        0        0       63 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/rules/importer/__init__.py
--rw-r--r--   0        0        0    13007 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/rules/importer/ontology2excel.py
--rw-r--r--   0        0        0    24210 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/rules/models.py
--rw-r--r--   0        0        0     8231 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/rules/to_rdf_path.py
--rw-r--r--   0        0        0        0 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/utils/__init__.py
--rw-r--r--   0        0        0      309 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/utils/auxiliary.py
--rw-r--r--   0        0        0      741 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/utils/cdf.py
--rw-r--r--   0        0        0    10682 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/utils/utils.py
--rw-r--r--   0        0        0     9995 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/workflows/base_workflows/graph2assets_relationships.py
--rw-r--r--   0        0        0     7093 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/workflows/base_workflows/graphs_and_rules.py
--rw-r--r--   0        0        0    14417 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/workflows/base_workflows/sheet2cdf.py
--rw-r--r--   0        0        0    11801 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/workflows/base_workflows/sme_graph_capture.py
--rw-r--r--   0        0        0      661 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/workflows/examples/__init__.py
--rw-r--r--   0        0        0      286 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/workflows/examples/data-models/power-grid-v0_1_0.graphql
--rw-r--r--   0        0        0    68445 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/workflows/examples/graph-sheets/power-grid-example.xlsx
--rw-r--r--   0        0        0    94607 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/workflows/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx
--rw-r--r--   0        0        0    14930 2023-07-26 07:33:59.214009 cognite_neat-0.18.1/cognite/neat/workflows/examples/ontologies/report.txt
--rw-r--r--   0        0        0    12820 2023-07-26 07:33:59.134009 cognite_neat-0.18.1/cognite/neat/workflows/examples/ontologies/transformation_rules.xlsx
--rw-r--r--   0        0        0    64516 2023-07-26 07:32:45.253853 cognite_neat-0.18.1/cognite/neat/workflows/examples/ontologies/wind-energy.owl
--rw-r--r--   0        0        0    80218 2023-07-26 07:32:45.257853 cognite_neat-0.18.1/cognite/neat/workflows/examples/rules/Rules-Nordic44-to-TNT.xlsx
--rw-r--r--   0        0        0    77381 2023-07-26 07:32:45.257853 cognite_neat-0.18.1/cognite/neat/workflows/examples/rules/power-grid-example.xlsx
--rw-r--r--   0        0        0    75865 2023-07-26 07:32:45.257853 cognite_neat-0.18.1/cognite/neat/workflows/examples/rules/rules-template.xlsx
--rw-r--r--   0        0        0    52650 2023-07-26 07:32:45.257853 cognite_neat-0.18.1/cognite/neat/workflows/examples/rules/sheet2cdf-transformation-rules.xlsx
--rw-r--r--   0        0        0    79964 2023-07-26 07:32:45.257853 cognite_neat-0.18.1/cognite/neat/workflows/examples/rules/source-to-solution-mapping-rules.xlsx
--rw-r--r--   0        0        0  1437851 2023-07-26 07:32:45.261853 cognite_neat-0.18.1/cognite/neat/workflows/examples/source-graphs/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0     1460 2023-07-26 07:32:45.261853 cognite_neat-0.18.1/cognite/neat/workflows/examples/workflows/basic/workflow.py
--rw-r--r--   0        0        0     1782 2023-07-26 07:32:45.261853 cognite_neat-0.18.1/cognite/neat/workflows/examples/workflows/basic/workflow.yaml
--rw-r--r--   0        0        0    15745 2023-07-26 07:32:45.261853 cognite_neat-0.18.1/cognite/neat/workflows/examples/workflows/default/workflow.py
--rw-r--r--   0        0        0     6774 2023-07-26 07:32:45.261853 cognite_neat-0.18.1/cognite/neat/workflows/examples/workflows/default/workflow.yaml
--rw-r--r--   0        0        0     3528 2023-07-26 07:32:45.261853 cognite_neat-0.18.1/cognite/neat/workflows/examples/workflows/fdm_schema_generation/workflow.py
--rw-r--r--   0        0        0     2573 2023-07-26 07:32:45.261853 cognite_neat-0.18.1/cognite/neat/workflows/examples/workflows/fdm_schema_generation/workflow.yaml
--rw-r--r--   0        0        0    11444 2023-07-26 07:32:45.261853 cognite_neat-0.18.1/cognite/neat/workflows/examples/workflows/graph_db_import/workflow.py
--rw-r--r--   0        0        0     4792 2023-07-26 07:32:45.261853 cognite_neat-0.18.1/cognite/neat/workflows/examples/workflows/graph_db_import/workflow.yaml
--rw-r--r--   0        0        0      324 2023-07-26 07:32:45.261853 cognite_neat-0.18.1/cognite/neat/workflows/examples/workflows/graph_to_asset_hierarchy/workflow.py
--rw-r--r--   0        0        0     8063 2023-07-26 07:32:45.261853 cognite_neat-0.18.1/cognite/neat/workflows/examples/workflows/graph_to_asset_hierarchy/workflow.yaml
--rw-r--r--   0        0        0      274 2023-07-26 07:32:45.261853 cognite_neat-0.18.1/cognite/neat/workflows/examples/workflows/sheet2cdf/workflow.py
--rw-r--r--   0        0        0     6668 2023-07-26 07:32:45.261853 cognite_neat-0.18.1/cognite/neat/workflows/examples/workflows/sheet2cdf/workflow.yaml
--rw-r--r--   0        0        0      301 2023-07-26 07:32:45.261853 cognite_neat-0.18.1/cognite/neat/workflows/examples/workflows/sme_graph_capture/workflow.py
--rw-r--r--   0        0        0     6837 2023-07-26 07:32:45.261853 cognite_neat-0.18.1/cognite/neat/workflows/examples/workflows/sme_graph_capture/workflow.yaml
--rw-r--r--   0        0        0        0 2023-07-26 07:32:45.261853 cognite_neat-0.18.1/cognite/neat/workflows/migration/__init__.py
--rw-r--r--   0        0        0     1581 2023-07-26 07:32:45.261853 cognite_neat-0.18.1/cognite/neat/workflows/migration/wf_manifests.py
--rw-r--r--   0        0        0      660 2023-07-26 07:32:45.261853 cognite_neat-0.18.1/cognite/neat/workflows/steps/data_contracts.py
--rw-r--r--   0        0        0     1996 2023-07-26 07:32:45.261853 cognite_neat-0.18.1/cognite/neat/workflows/steps/steps.py
--rw-r--r--   0        0        0      361 2023-07-26 07:32:45.261853 cognite_neat-0.18.1/cognite/neat/workflows/workflow/__init__.py
--rw-r--r--   0        0        0    23404 2023-07-26 07:32:45.261853 cognite_neat-0.18.1/cognite/neat/workflows/workflow/base.py
--rw-r--r--   0        0        0    17855 2023-07-26 07:32:45.261853 cognite_neat-0.18.1/cognite/neat/workflows/workflow/cdf_store.py
--rw-r--r--   0        0        0    11684 2023-07-26 07:32:45.261853 cognite_neat-0.18.1/cognite/neat/workflows/workflow/manager.py
--rw-r--r--   0        0        0     4907 2023-07-26 07:32:45.261853 cognite_neat-0.18.1/cognite/neat/workflows/workflow/model.py
--rw-r--r--   0        0        0     1008 2023-07-26 07:32:45.261853 cognite_neat-0.18.1/cognite/neat/workflows/workflow/step_model.py
--rw-r--r--   0        0        0      780 2023-07-26 07:32:45.261853 cognite_neat-0.18.1/cognite/neat/workflows/workflow/tasks.py
--rw-r--r--   0        0        0     6987 2023-07-26 07:32:45.261853 cognite_neat-0.18.1/cognite/neat/workflows/workflow/triggers.py
--rw-r--r--   0        0        0      453 2023-07-26 07:32:45.261853 cognite_neat-0.18.1/cognite/neat/workflows/workflow/utils.py
--rw-r--r--   0        0        0     2695 2023-07-26 07:32:45.725855 cognite_neat-0.18.1/pyproject.toml
--rw-r--r--   0        0        0    10637 1970-01-01 00:00:00.000000 cognite_neat-0.18.1/PKG-INFO
+-rw-r--r--   0        0        0    11351 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/LICENSE
+-rw-r--r--   0        0        0     8667 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/README.md
+-rw-r--r--   0        0        0       61 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/__init__.py
+-rw-r--r--   0        0        0       23 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/_version.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/api/__init__.py
+-rw-r--r--   0        0        0     2778 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/api/app.py
+-rw-r--r--   0        0        0     5611 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/api/configuration.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/api/data_classes/__init__.py
+-rw-r--r--   0        0        0     1390 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/api/data_classes/rest.py
+-rw-r--r--   0        0        0    24080 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/api/explorer.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/api/utils/__init__.py
+-rw-r--r--   0        0        0      412 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/api/utils/data_mapping.py
+-rw-r--r--   0        0        0     4622 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/api/utils/query_templates.py
+-rw-r--r--   0        0        0      357 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/main.py
+-rw-r--r--   0        0        0       16 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/ui/index.html
+-rw-r--r--   0        0        0      312 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/.gitignore
+-rw-r--r--   0        0        0     3359 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/README.md
+-rw-r--r--   0        0        0      464 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/asset-manifest.json
+-rw-r--r--   0        0        0     3870 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/favicon.ico
+-rw-r--r--   0        0        0      630 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/index.html
+-rw-r--r--   0        0        0     5347 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/logo192.png
+-rw-r--r--   0        0        0      492 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/manifest.json
+-rw-r--r--   0        0        0       67 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/robots.txt
+-rw-r--r--   0        0        0     8524 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
+-rw-r--r--   0        0        0    13319 2023-07-26 15:57:51.278903 cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
+-rw-r--r--   0        0        0  1370405 2023-07-26 15:57:51.286903 cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/static/js/main.694f3f8e.js
+-rw-r--r--   0        0        0     2667 2023-07-26 15:57:51.286903 cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/static/js/main.694f3f8e.js.LICENSE.txt
+-rw-r--r--   0        0        0  5883860 2023-07-26 15:57:51.322903 cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/static/js/main.694f3f8e.js.map
+-rw-r--r--   0        0        0     2633 2023-07-26 15:57:51.322903 cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
+-rw-r--r--   0        0        0      979 2023-07-26 15:57:51.326903 cognite_neat-0.18.2/cognite/neat/config.py
+-rw-r--r--   0        0        0      347 2023-07-26 15:57:51.326903 cognite_neat-0.18.2/cognite/neat/constants.py
+-rw-r--r--   0        0        0     1276 2023-07-26 15:57:51.326903 cognite_neat-0.18.2/cognite/neat/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:57:51.326903 cognite_neat-0.18.2/cognite/neat/graph/__init__.py
+-rw-r--r--   0        0        0  1437938 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0      368 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/examples/__init__.py
+-rw-r--r--   0        0        0      442 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/extractors/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/extractors/data_stores/__init__.py
+-rw-r--r--   0        0        0     1520 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/extractors/data_stores/metrics.py
+-rw-r--r--   0        0        0     9436 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/extractors/data_stores/oxrdflib.py
+-rw-r--r--   0        0        0     7255 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/extractors/graph_sheet_to_graph.py
+-rw-r--r--   0        0        0    11434 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/extractors/graph_store.py
+-rw-r--r--   0        0        0       68 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/extractors/mocks/__init__.py
+-rw-r--r--   0        0        0    12883 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/extractors/mocks/graph.py
+-rw-r--r--   0        0        0     1213 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/extractors/rdf_to_graph.py
+-rw-r--r--   0        0        0      432 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/loaders/__init__.py
+-rw-r--r--   0        0        0     2837 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/loaders/_exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/loaders/core/__init__.py
+-rw-r--r--   0        0        0     2279 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/loaders/core/labels.py
+-rw-r--r--   0        0        0     5043 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/loaders/core/models.py
+-rw-r--r--   0        0        0    39898 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/loaders/core/rdf_to_assets.py
+-rw-r--r--   0        0        0    20925 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/loaders/core/rdf_to_relationships.py
+-rw-r--r--   0        0        0     2650 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/loaders/validator.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/transformations/__init__.py
+-rw-r--r--   0        0        0       73 2023-07-26 15:57:51.330903 cognite_neat-0.18.2/cognite/neat/graph/transformations/query_generator/__init__.py
+-rw-r--r--   0        0        0     9592 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/graph/transformations/query_generator/sparql.py
+-rw-r--r--   0        0        0    11892 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/graph/transformations/transformer.py
+-rw-r--r--   0        0        0      379 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/__init__.py
+-rw-r--r--   0        0        0    49672 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/_exceptions.py
+-rw-r--r--   0        0        0    13038 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/_parser.py
+-rw-r--r--   0        0        0     3496 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/_validation.py
+-rw-r--r--   0        0        0     4777 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/analysis.py
+-rw-r--r--   0        0        0    80218 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/examples/Rules-Nordic44-to-TNT.xlsx
+-rw-r--r--   0        0        0      449 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/examples/__init__.py
+-rw-r--r--   0        0        0    77381 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/examples/power-grid-example.xlsx
+-rw-r--r--   0        0        0    75865 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/examples/rules-template.xlsx
+-rw-r--r--   0        0        0    52650 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/examples/sheet2cdf-transformation-rules.xlsx
+-rw-r--r--   0        0        0    79964 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/examples/source-to-solution-mapping-rules.xlsx
+-rw-r--r--   0        0        0        0 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/exporter/__init__.py
+-rw-r--r--   0        0        0      102 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/exporter/core/__init__.py
+-rw-r--r--   0        0        0      610 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/exporter/core/rules2labels.py
+-rw-r--r--   0        0        0       48 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/exporter/dm/rules2dms.py
+-rw-r--r--   0        0        0     5403 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/exporter/rules2graph_sheet.py
+-rw-r--r--   0        0        0     4763 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/exporter/rules2graphql.py
+-rw-r--r--   0        0        0    15643 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/exporter/rules2ontology.py
+-rw-r--r--   0        0        0     4019 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/exporter/rules2rules.py
+-rw-r--r--   0        0        0      631 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/exporter/rules2triples.py
+-rw-r--r--   0        0        0       63 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/importer/__init__.py
+-rw-r--r--   0        0        0    13007 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/importer/ontology2excel.py
+-rw-r--r--   0        0        0    24214 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/models.py
+-rw-r--r--   0        0        0     8231 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/rules/to_rdf_path.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/utils/__init__.py
+-rw-r--r--   0        0        0      309 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/utils/auxiliary.py
+-rw-r--r--   0        0        0      741 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/utils/cdf.py
+-rw-r--r--   0        0        0    10682 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/utils/utils.py
+-rw-r--r--   0        0        0      352 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/workflows/__init__.py
+-rw-r--r--   0        0        0    23386 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/workflows/base.py
+-rw-r--r--   0        0        0     9986 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/workflows/base_workflows/graph2assets_relationships.py
+-rw-r--r--   0        0        0     7066 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/workflows/base_workflows/graphs_and_rules.py
+-rw-r--r--   0        0        0    14390 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/workflows/base_workflows/sheet2cdf.py
+-rw-r--r--   0        0        0    11774 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/workflows/base_workflows/sme_graph_capture.py
+-rw-r--r--   0        0        0    17837 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/workflows/cdf_store.py
+-rw-r--r--   0        0        0     1442 2023-07-26 15:57:51.334903 cognite_neat-0.18.2/cognite/neat/workflows/examples/basic/workflow.py
+-rw-r--r--   0        0        0     1782 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/examples/basic/workflow.yaml
+-rw-r--r--   0        0        0    15718 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/examples/default/workflow.py
+-rw-r--r--   0        0        0     6774 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/examples/default/workflow.yaml
+-rw-r--r--   0        0        0     3536 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/examples/fdm_schema_generation/workflow.py
+-rw-r--r--   0        0        0     2573 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/examples/fdm_schema_generation/workflow.yaml
+-rw-r--r--   0        0        0    11435 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/examples/graph_db_import/workflow.py
+-rw-r--r--   0        0        0     4792 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/examples/graph_db_import/workflow.yaml
+-rw-r--r--   0        0        0      324 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/examples/graph_to_asset_hierarchy/workflow.py
+-rw-r--r--   0        0        0     8063 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/examples/graph_to_asset_hierarchy/workflow.yaml
+-rw-r--r--   0        0        0      274 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/examples/sheet2cdf/workflow.py
+-rw-r--r--   0        0        0     6668 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/examples/sheet2cdf/workflow.yaml
+-rw-r--r--   0        0        0      301 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/examples/sme_graph_capture/workflow.py
+-rw-r--r--   0        0        0     6837 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/examples/sme_graph_capture/workflow.yaml
+-rw-r--r--   0        0        0    11648 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/manager.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/migration/__init__.py
+-rw-r--r--   0        0        0     1581 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/migration/wf_manifests.py
+-rw-r--r--   0        0        0     4907 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/model.py
+-rw-r--r--   0        0        0     1008 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/step_model.py
+-rw-r--r--   0        0        0      651 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/steps/data_contracts.py
+-rw-r--r--   0        0        0     1978 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/steps/steps.py
+-rw-r--r--   0        0        0      771 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/tasks.py
+-rw-r--r--   0        0        0     6969 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/triggers.py
+-rw-r--r--   0        0        0      453 2023-07-26 15:57:51.338904 cognite_neat-0.18.2/cognite/neat/workflows/utils.py
+-rw-r--r--   0        0        0     2740 2023-07-26 15:57:51.846905 cognite_neat-0.18.2/pyproject.toml
+-rw-r--r--   0        0        0    10617 1970-01-01 00:00:00.000000 cognite_neat-0.18.2/PKG-INFO
```

### Comparing `cognite_neat-0.18.1/LICENSE` & `cognite_neat-0.18.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/README.md` & `cognite_neat-0.18.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,97 +1,95 @@
 # kNowlEdge grAph Transformer (NEAT)
 
 This is python package handles transformation of domain knowledge graphs (more detailed, overarching) to app specific knowledge graphs.
 
 ## Quickstart
 
 ### Option 1 - Python Package
+
 `neat` can be installed as a Python package, and a docker image for more robust execution and support such
 as `graphdb` for caching. This quickstart guide uses the Python package.
 
 ### Option 2 - Docker container
 
 Running NEAT as docker container :
 `docker run -p 8000:8000 --name neat cognite/neat:latest`
 
 Runnin NEAT as docker container with local data folder mounted :
 `docker run -p 8000:8000 --name neat -v $(shell pwd)/docker/vol_data:/app/data  cognite/neat:latest`
 
-
 ### Installation (Development setup)
+
 Prerequisites:
-* `poetry` installed on your system, [see installation](https://python-poetry.org/docs/).
-* `npm` installed on your system, [see installation](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
-* `react-scripts` installed on your system, [`npm i react-scripts`](https://www.npmjs.com/package/react-scripts)
+
+- `poetry` installed on your system, [see installation](https://python-poetry.org/docs/).
+- `npm` installed on your system, [see installation](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
+- `react-scripts` installed on your system, [`npm i react-scripts`](https://www.npmjs.com/package/react-scripts)
 
 1. Clone this repo: `git clone git@github.com:cognitedata/neat.git`
 2. Create wheel: `make build-python`. This will create a wheel in the `dist` folder.
 3. Install wheel in your preferred environment, `pip install dist/neat-[NEAT_VERSTION]-py3-none-any.whl`
 
-
 ### Run Neat (Python Package)
 
 Once installed you can run neat with the command
+
 ```bash
 neat
 ```
+
 This will open your browser and launch the neat application.
 
 Note this will automatically create a `data` folder in your current working directory, which is populated
 with default workflows, rule sheets, and source graphs. In addition, there is a `config.yaml` you can add
 your CDF credentials to allow `neat` access CDF.
 
 ![launch_neat](https://user-images.githubusercontent.com/60234212/228812422-c5e9519f-19e7-4f08-9617-66a790323c7e.gif)
 
-
 ## Documentation
 
 [Documentation](https://cognite-neat.readthedocs-hosted.com/en/latest/)
 
 ![](./docs/figs/high-level-io.png)
 
-
 ## Docker container build process
 
-
-``` make build-docker ```
+`make build-docker`
 
 ## Starting the application locally using GraphDB as external rdf store
 
 Run the command :
 
-``` make compose-up```
-
-The command starts NEAT container and GraphDB container and creates *vol_data* and *vol_shared* local folders that are mounted as volumes.
+` make compose-up`
 
-*vol_data* - is mounted only in NEAT container. It contains `config.yaml`, `workflows`, `rules`. You can set `load_examples` to `true` to populate it with examples.
+The command starts NEAT container and GraphDB container and creates _vol_data_ and _vol_shared_ local folders that are mounted as volumes.
 
-*vol_shared* - is mounted to both containers and files placed here become automatically visible for GraphDB import process. Main intension is to write files from NEAT container and make them available for GraphDB for import.
+_vol_data_ - is mounted only in NEAT container. It contains `config.yaml`, `workflows`, `rules`. You can set `load_examples` to `true` to populate it with examples.
 
+_vol_shared_ - is mounted to both containers and files placed here become automatically visible for GraphDB import process. Main intension is to write files from NEAT container and make them available for GraphDB for import.
 
 ## Web UI
 
-``` http://localhost:8000 ```
+`http://localhost:8000`
 
 Open API docs :
 
-``` http://localhost:8000/docs ```
+`http://localhost:8000/docs`
 
 Prom metrics :
 
-``` http://localhost:8000/metrics ```
-
+`http://localhost:8000/metrics`
 
 ## Workflows and configurations
 
 All configurations are divided into 2 categories :
+
 - global configurations - global for entire service , loaded at startup (config.yaml)
 - workflow configurations - local to workflow , loaded from workflow manifest (.yaml)
 
-
 ## Global configurations
 
 Global configurations loaded by the application during startup process, either from ENV variables or file.
 
 The application tries to load the configuration as follows.
 
 1. Try ENV variables. This is done by checking for the ENV variable `NEAT_CDF_PROJECT`, and if it exists load the rest
@@ -117,75 +115,78 @@
 ### Config file
 
 ```yaml
 workflows_store_type: file
 data_store_path: /app/data
 
 cdf_client:
-    project: get-power-grid
-    client_id: "623c2450-cfc2-43d6-9036-10e14dad8ccf"
-    client_secret: "my-super-secret"
-    client_name: neat-test-service
-    base_url: https://az-power-no-northeurope.cognitedata.com
-    scopes:
-      - https://az-power-no-northeurope.cognitedata.com/.default
-    token_url: https://login.microsoftonline.com/e55e1701-82f8-4c52-af10-28e4d942c589/oauth2/v2.0/token
+  project: get-power-grid
+  client_id: "623c2450-cfc2-43d6-9036-10e14dad8ccf"
+  client_secret: "my-super-secret"
+  client_name: neat-test-service
+  base_url: https://az-power-no-northeurope.cognitedata.com
+  scopes:
+    - https://az-power-no-northeurope.cognitedata.com/.default
+  token_url: https://login.microsoftonline.com/e55e1701-82f8-4c52-af10-28e4d942c589/oauth2/v2.0/token
 
 cdf_default_dataset_id: 2626756768281823
 workflow_downloader_filter:
-    - tag:grid
+  - tag:grid
 log_level: DEBUG
 ```
 
 ## Automatic workflow loading from CDF during application startup
 
 If `workflow_downloader_filter` is set, the app will try to download workflows from CDF based on provided filtering conditions .
 Filtering format :
+
 - `name:<workflows_name>=<workflow_version>` - loading workflow by name and version or latest by name if version is not set.
 - `tag:<tag_name>`- loading all workflows that tagged with specific tag.
 
 ## Workflow level configurations
 
 Each workflow can have own unique subset of configurations defined in `config.yaml` file. There is also a small subset of system
 configurations that can be set on workflow level.
 
 System configurations:
 
 - system.execution_reporting_type - controls how workflow execution log should be reported to CDF . Supported values : `all_disabled`, `all_enabled`(default)
 
 Example :
+
 ```yaml
--   group: system
-    name: system.execution_reporting_type
-    value: all_disabled
+- group: system
+  name: system.execution_reporting_type
+  value: all_disabled
 ```
 
 ## How to develop your first workflow
 
 The NEAT framework has few conventions :
+
 - Each workflow must reside in its own folder
 - Workflow folder must contain at least 2 files :
-    - `workflow.py` - steps implementation file
-    - `workflow.yaml` - manifest and configurations
+  - `workflow.py` - steps implementation file
+  - `workflow.yaml` - manifest and configurations
 
- ### Workflow steps implementation file
+### Workflow steps implementation file
 
- Must implement `BaseWorkflow` class from `from cognite.neat.core.workflow.base`
+Must implement `BaseWorkflow` class from `from cognite.neat.core.workflow.base`
 
- Each method that should be orchestrated by workflow engine must be prefixed with `step_` , each method must have single argument of `FlowMessage` type and return `FlowMessage` or `None`.
- FlowMessage is passed from one step to another and it's captured in execution log.
+Each method that should be orchestrated by workflow engine must be prefixed with `step_` , each method must have single argument of `FlowMessage` type and return `FlowMessage` or `None`.
+FlowMessage is passed from one step to another and it's captured in execution log.
 
 Simplest `workflow.py`
 
-````python
+```python
 
 import logging
 from cognite.client import CogniteClient
-from cognite.neat.workflows.workflow import BaseWorkflow
-from cognite.neat.workflows.workflow import FlowMessage
+from cognite.neat.workflows import BaseWorkflow
+from cognite.neat.workflows import FlowMessage
 
 
 class PlaygroundNeatWorkflow(BaseWorkflow):
     def __init__(self, name: str, client: CogniteClient):
         super().__init__(name, client, [])
 
     def step_run_experiment_1(self, flow_msg: FlowMessage = None):
@@ -193,90 +194,89 @@
         logging.info("Done running experiment 4444")
 
         return FlowMessage(output_text="Done running experiment 1")
 
     def step_cleanup(self, flow_msg: FlowMessage = None):
         logging.info("Cleanup")
 
-````
+```
 
 Manifest `workflow.yaml` , normally should be updated from UI
-````yaml
+
+```yaml
 configs:
--   group: source_rdf_store
+  - group: source_rdf_store
     label: null
     name: source_rdf_store.type
     options: null
     required: false
     type: null
     value: graphdb
 description: null
 groups:
--   description: null
+  - description: null
     id: experimentation_system
     label: Experimentation playground
     transition_to: null
     ui_config:
-        pos_x: 171
-        pos_y: 6
+      pos_x: 171
+      pos_y: 6
 implementation_module: null
 name: playground
 steps:
--   description: null
+  - description: null
     enabled: true
     group_id: null
     id: run_experiment_1
     label: Running first experiment
     method: null
     params: {}
     stype: pystep
     transition_to:
-    - cleanup
+      - cleanup
     trigger: false
     ui_config:
-        pos_x: 340
-        pos_y: 144
--   description: null
+      pos_x: 340
+      pos_y: 144
+  - description: null
     enabled: true
     group_id: null
     id: cleanup
     label: Cleanup
     method: null
     params: null
     stype: pystep
     transition_to: []
     trigger: false
     ui_config:
-        pos_x: 295
-        pos_y: 303
--   description: null
+      pos_x: 295
+      pos_y: 303
+  - description: null
     enabled: true
     group_id: null
     id: step_trigger
     label: HTTP trigger
     method: null
     params: {}
     stype: http_trigger
     transition_to:
-    - run_experiment_1
+      - run_experiment_1
     trigger: true
     ui_config:
-        pos_x: 336
-        pos_y: 44
--   description: null
+      pos_x: 336
+      pos_y: 44
+  - description: null
     enabled: false
     group_id: null
     id: step_295076
     label: Run every 10 sec
     method: null
     params:
-        interval: every 10 seconds
+      interval: every 10 seconds
     stype: time_trigger
     transition_to:
-    - run_experiment_1
+      - run_experiment_1
     trigger: true
     ui_config:
-        pos_x: 544
-        pos_y: 42
-
-
-````
+      pos_x: 544
+      pos_y: 42
+```
```

### Comparing `cognite_neat-0.18.1/cognite/neat/app/api/app.py` & `cognite_neat-0.18.2/cognite/neat/app/api/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 
 from cognite.client import CogniteClient
 from fastapi import FastAPI
 
 from cognite.neat.app.api.configuration import Config
 from cognite.neat.utils.utils import get_cognite_client_from_config
-from cognite.neat.workflows.workflow.cdf_store import CdfStore
-from cognite.neat.workflows.workflow.manager import WorkflowManager
-from cognite.neat.workflows.workflow.triggers import TriggerManager
+from cognite.neat.workflows.cdf_store import CdfStore
+from cognite.neat.workflows.manager import WorkflowManager
+from cognite.neat.workflows.triggers import TriggerManager
 
 
 class NeatApp:
     def __init__(self, config: Config, cdf_client: CogniteClient = None):
         self.config = config
         self.cdf_client: CogniteClient = None
         self.cdf_store: CdfStore = None
```

### Comparing `cognite_neat-0.18.1/cognite/neat/app/api/configuration.py` & `cognite_neat-0.18.2/cognite/neat/app/api/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/app/api/data_classes/rest.py` & `cognite_neat-0.18.2/cognite/neat/app/api/data_classes/rest.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/app/api/explorer.py` & `cognite_neat-0.18.2/cognite/neat/app/api/explorer.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 from prometheus_client import REGISTRY, Counter, make_asgi_app
 
 from cognite import neat
 from cognite.neat import constants, rules as rules_module
 from cognite.neat.graph.transformations import query_generator
 from cognite.neat.app.api.app import NeatApp
 from cognite.neat.app.api.configuration import Config, configure_logging
-from cognite.neat.graph.extractors.config import copy_examples_to_directory
-from cognite.neat.workflows.workflow import WorkflowFullStateReport
-from cognite.neat.workflows.workflow import utils
-from cognite.neat.workflows.workflow.base import WorkflowDefinition
-from cognite.neat.workflows.workflow.model import FlowMessage, WorkflowConfigItem
+from cognite.neat.config import copy_examples_to_directory
+from cognite.neat.workflows import WorkflowFullStateReport
+from cognite.neat.workflows import utils
+from cognite.neat.workflows.base import WorkflowDefinition
+from cognite.neat.workflows.model import FlowMessage, WorkflowConfigItem
 from cognite.neat.app.api.data_classes.rest import (
     DownloadFromCdfRequest,
     NodesAndEdgesRequest,
     QueryRequest,
     RuleRequest,
     RunWorkflowRequest,
     UploadToCdfRequest,
```

### Comparing `cognite_neat-0.18.1/cognite/neat/app/api/utils/query_templates.py` & `cognite_neat-0.18.2/cognite/neat/app/api/utils/query_templates.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/app/ui/neat-app/README.md` & `cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/app/ui/neat-app/build/favicon.ico` & `cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/app/ui/neat-app/build/index.html` & `cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/index.html`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/app/ui/neat-app/build/logo192.png` & `cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/logo192.png`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css` & `cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map` & `cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/app/ui/neat-app/build/static/js/main.694f3f8e.js` & `cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/static/js/main.694f3f8e.js`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/app/ui/neat-app/build/static/js/main.694f3f8e.js.LICENSE.txt` & `cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/static/js/main.694f3f8e.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/app/ui/neat-app/build/static/js/main.694f3f8e.js.map` & `cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/static/js/main.694f3f8e.js.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/app/ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg` & `cognite_neat-0.18.2/cognite/neat/app/ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/exceptions.py` & `cognite_neat-0.18.2/cognite/neat/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/graph/extractors/data_stores/metrics.py` & `cognite_neat-0.18.2/cognite/neat/graph/extractors/data_stores/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/graph/extractors/data_stores/oxrdflib.py` & `cognite_neat-0.18.2/cognite/neat/graph/extractors/data_stores/oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/graph/extractors/graph_sheet_to_graph.py` & `cognite_neat-0.18.2/cognite/neat/graph/extractors/graph_sheet_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/graph/extractors/graph_store.py` & `cognite_neat-0.18.2/cognite/neat/graph/extractors/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/graph/extractors/mocks/graph.py` & `cognite_neat-0.18.2/cognite/neat/graph/extractors/mocks/graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/graph/extractors/rdf_to_graph.py` & `cognite_neat-0.18.2/cognite/neat/graph/extractors/rdf_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/graph/loaders/_exceptions.py` & `cognite_neat-0.18.2/cognite/neat/graph/loaders/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/graph/loaders/core/labels.py` & `cognite_neat-0.18.2/cognite/neat/graph/loaders/core/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/graph/loaders/core/models.py` & `cognite_neat-0.18.2/cognite/neat/graph/loaders/core/models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/graph/loaders/core/rdf_to_assets.py` & `cognite_neat-0.18.2/cognite/neat/graph/loaders/core/rdf_to_assets.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/graph/loaders/core/rdf_to_relationships.py` & `cognite_neat-0.18.2/cognite/neat/graph/loaders/core/rdf_to_relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/graph/loaders/validator.py` & `cognite_neat-0.18.2/cognite/neat/graph/loaders/validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/graph/transformations/query_generator/sparql.py` & `cognite_neat-0.18.2/cognite/neat/graph/transformations/query_generator/sparql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/graph/transformations/transformer.py` & `cognite_neat-0.18.2/cognite/neat/graph/transformations/transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/rules/_exceptions.py` & `cognite_neat-0.18.2/cognite/neat/rules/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/rules/_parser.py` & `cognite_neat-0.18.2/cognite/neat/rules/_parser.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/rules/_validation.py` & `cognite_neat-0.18.2/cognite/neat/rules/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/rules/analysis.py` & `cognite_neat-0.18.2/cognite/neat/rules/analysis.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/rules/exporter/core/rules2labels.py` & `cognite_neat-0.18.2/cognite/neat/rules/exporter/core/rules2labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/rules/exporter/rules2graph_sheet.py` & `cognite_neat-0.18.2/cognite/neat/rules/exporter/rules2graph_sheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/rules/exporter/rules2graphql.py` & `cognite_neat-0.18.2/cognite/neat/rules/exporter/rules2graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/rules/exporter/rules2ontology.py` & `cognite_neat-0.18.2/cognite/neat/rules/exporter/rules2ontology.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/rules/exporter/rules2rules.py` & `cognite_neat-0.18.2/cognite/neat/rules/exporter/rules2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/rules/exporter/rules2triples.py` & `cognite_neat-0.18.2/cognite/neat/rules/exporter/rules2triples.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/rules/importer/ontology2excel.py` & `cognite_neat-0.18.2/cognite/neat/rules/importer/ontology2excel.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/rules/models.py` & `cognite_neat-0.18.2/cognite/neat/rules/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,17 +111,17 @@
 class URL(BaseModel):
     url: HttpUrl
 
 
 Description = constr(min_length=1, max_length=255)
 
 # regex expressions for compliance of Metadata sheet parsing
-prefix_compliance_regex = r"^([a-zA-Z]+[a-zA-Z0-9]*[_-]{0,1}[a-zA-Z0-9]+)+$"
+prefix_compliance_regex = r"^([a-zA-Z]+)([a-zA-Z0-9]*[_-]{0,1}[a-zA-Z0-9])+$"
 cdf_space_name_compliance_regex = rf"(?!^(space|cdf|dms|pg3|shared|system|node|edge)$)({prefix_compliance_regex})"
-data_model_name_compliance_regex = r"^([a-zA-Z]+[a-zA-Z0-9]*[_]{0,1}[a-zA-Z0-9])+$"
+data_model_name_compliance_regex = r"^([a-zA-Z]+)([a-zA-Z0-9]*[_-]{0,1}[a-zA-Z0-9])+$"
 version_compliance_regex = (
     r"^([0-9]+[_-]{1}[0-9]+[_-]{1}[0-9]+[_-]{1}[a-zA-Z0-9]+)|"
     r"([0-9]+[_-]{1}[0-9]+[_-]{1}[0-9]+)|([0-9]+[_-]{1}[0-9])|([0-9]+)$"
 )
 
 Prefix = constr(min_length=1, max_length=43)
 ExternalId = constr(min_length=1, max_length=255)
```

### Comparing `cognite_neat-0.18.1/cognite/neat/rules/to_rdf_path.py` & `cognite_neat-0.18.2/cognite/neat/rules/to_rdf_path.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/utils/cdf.py` & `cognite_neat-0.18.2/cognite/neat/utils/cdf.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/utils/utils.py` & `cognite_neat-0.18.2/cognite/neat/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/workflows/base_workflows/graph2assets_relationships.py` & `cognite_neat-0.18.2/cognite/neat/workflows/base_workflows/graph2assets_relationships.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from cognite.neat.graph.loaders.core.rdf_to_assets import categorize_assets, rdf2assets, upload_assets
 from cognite.neat.graph.loaders.core.rdf_to_relationships import (
     categorize_relationships,
     rdf2relationships,
     upload_relationships,
 )
 from cognite.neat.graph.loaders.validator import validate_asset_hierarchy
-from cognite.neat.workflows.workflow.model import FlowMessage
+from cognite.neat.workflows.model import FlowMessage
 
 with contextlib.suppress(ValueError):
     prom_cdf_resource_stats = Gauge(
         "neat_graph_to_asset_hierarchy_wf_cdf_resource_stats",
         "CDF resource stats before and after running fast_graph workflow",
         ["resource_type", "state"],
     )
```

### Comparing `cognite_neat-0.18.1/cognite/neat/workflows/base_workflows/graphs_and_rules.py` & `cognite_neat-0.18.2/cognite/neat/workflows/base_workflows/graphs_and_rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from cognite.neat import rules
 from cognite.neat.graph import extractors
 from cognite.neat.app.api.configuration import PREFIXES
 from cognite.neat.graph.extractors import NeatGraphStore, drop_graph_store
 from cognite.neat.rules.exporter.rules2triples import get_instances_as_triples
 from cognite.neat.rules.models import TransformationRules
 from cognite.neat.graph.transformations.transformer import RuleProcessingReport, domain2app_knowledge_graph
-from cognite.neat.workflows.workflow import utils
-from cognite.neat.workflows.workflow.base import BaseWorkflow, FlowMessage
-from cognite.neat.workflows.workflow.cdf_store import CdfStore
+from cognite.neat.workflows import utils
+from cognite.neat.workflows.base import BaseWorkflow, FlowMessage
+from cognite.neat.workflows.cdf_store import CdfStore
 
 
 class GraphsAndRulesBaseWorkflow(BaseWorkflow):
     def __init__(self, name: str, client: CogniteClient):
         super().__init__(name, client, [])
         self.dataset_id: int = 0
         self.source_graph: NeatGraphStore = None
```

### Comparing `cognite_neat-0.18.1/cognite/neat/workflows/base_workflows/sheet2cdf.py` & `cognite_neat-0.18.2/cognite/neat/workflows/base_workflows/sheet2cdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,17 +23,17 @@
     rdf2relationships,
     upload_relationships,
 )
 from cognite.neat.graph.extractors import NeatGraphStore
 from cognite.neat.rules.exporter.rules2triples import get_instances_as_triples
 from cognite.neat.rules.models import TransformationRules
 from cognite.neat.graph.loaders.validator import validate_asset_hierarchy
-from cognite.neat.workflows.workflow import utils
-from cognite.neat.workflows.workflow.base import BaseWorkflow, FlowMessage
-from cognite.neat.workflows.workflow.cdf_store import CdfStore
+from cognite.neat.workflows import utils
+from cognite.neat.workflows.base import BaseWorkflow, FlowMessage
+from cognite.neat.workflows.cdf_store import CdfStore
 
 with contextlib.suppress(ValueError):
     prom_cdf_resource_stats = Gauge(
         "neat_sheet2cdf_cdf_resource_stats",
         "CDF resource stats before and after running sheet2cdf workflow",
         ["resource_type", "state"],
     )
```

### Comparing `cognite_neat-0.18.1/cognite/neat/workflows/base_workflows/sme_graph_capture.py` & `cognite_neat-0.18.2/cognite/neat/workflows/base_workflows/sme_graph_capture.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
     rdf2relationships,
     upload_relationships,
 )
 from cognite.neat.graph.extractors import NeatGraphStore
 from cognite.neat.rules.models import TransformationRules
 from cognite.neat.utils.utils import add_triples
 from cognite.neat.graph.loaders.validator import validate_asset_hierarchy
-from cognite.neat.workflows.workflow import utils
-from cognite.neat.workflows.workflow.base import BaseWorkflow, FlowMessage
-from cognite.neat.workflows.workflow.cdf_store import CdfStore
+from cognite.neat.workflows import utils
+from cognite.neat.workflows.base import BaseWorkflow, FlowMessage
+from cognite.neat.workflows.cdf_store import CdfStore
 
 
 class SmeGraphCaptureBaseWorkflow(BaseWorkflow):
     def __init__(self, name: str, client: CogniteClient):
         super().__init__(name, client, [])
         self.counter = 0
         self.metrics.register_metric("counter_1", "", "counter", ["step"])
```

### Comparing `cognite_neat-0.18.1/cognite/neat/workflows/examples/rules/Rules-Nordic44-to-TNT.xlsx` & `cognite_neat-0.18.2/cognite/neat/rules/examples/Rules-Nordic44-to-TNT.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/workflows/examples/rules/power-grid-example.xlsx` & `cognite_neat-0.18.2/cognite/neat/rules/examples/power-grid-example.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/workflows/examples/rules/rules-template.xlsx` & `cognite_neat-0.18.2/cognite/neat/rules/examples/rules-template.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/workflows/examples/rules/sheet2cdf-transformation-rules.xlsx` & `cognite_neat-0.18.2/cognite/neat/rules/examples/sheet2cdf-transformation-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/workflows/examples/rules/source-to-solution-mapping-rules.xlsx` & `cognite_neat-0.18.2/cognite/neat/rules/examples/source-to-solution-mapping-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/workflows/examples/source-graphs/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.18.2/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml`

 * *Files 0% similar despite different names*

#### Comparing `cognite_neat-0.18.1/cognite/neat/workflows/examples/source-graphs/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.18.2/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml`

```diff
@@ -10,21 +10,21 @@
 			Added SIPS cases 1, 2 and 3 including PTC for case 4.
 2018-05-08: Version 35.
 			Made correction to the SIPS cases 1, 2 and 3 including PTC for case 4.
 2018-05-08: Version 36.
 			Minor corrections.
 2018-08-31:	Version 37
 			Added Energy Scheduling Area Ostfold and moved the substation Halden and Asker into this area.
-
+2023-07-26: Version 38. Purposely changed and defected graph for pupose of testing NEAT
 -->
   <md:FullModel rdf:about="urn:uuid:2dd9014f-bdfb-11e5-94fa-c8f73332c8f4">
     <md:Model.created>2018-08-31T13:47:55</md:Model.created>
     <md:Model.scenarioTime>2015-03-06T00:30:00</md:Model.scenarioTime>
     <pti:Model.createdBy>Statnett SF</pti:Model.createdBy>
-    <md:Model.version>37</md:Model.version>
+    <md:Model.version>38</md:Model.version>
     <md:Model.description>CGM Test model developed by Statnett SF. Nordic 44 bus system for the Nordic region</md:Model.description>
     <md:Model.modelingAuthoritySet>http://www.Statnett.no/IGM/Nordic44_CGM</md:Model.modelingAuthoritySet>
     <md:Model.profile>http://entsoe.eu/CIM/EquipmentCore/3/1</md:Model.profile>
     <md:Model.profile>http://entsoe.eu/CIM/EquipmentOperation/3/1</md:Model.profile>
     <md:Model.profile>http://entsoe.eu/CIM/EquipmentCore/3/2</md:Model.profile>
     <md:Model.profile>http://entsoe.eu/CIM/EquipmentOperation/3/2</md:Model.profile>
   </md:FullModel>
```

### Comparing `cognite_neat-0.18.1/cognite/neat/workflows/examples/workflows/basic/workflow.py` & `cognite_neat-0.18.2/cognite/neat/workflows/examples/basic/workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 
 from cognite.client import CogniteClient
 
-from cognite.neat.workflows.workflow import BaseWorkflow
-from cognite.neat.workflows.workflow import FlowMessage
+from cognite.neat.workflows import BaseWorkflow
+from cognite.neat.workflows import FlowMessage
 
 
 class BasicNeatWorkflow(BaseWorkflow):
     def __init__(self, name: str, client: CogniteClient):
         super().__init__(name, client, [])
         self.counter = 0
         self.metrics.register_metric("counter_1", "", "counter", ["step"])
```

### Comparing `cognite_neat-0.18.1/cognite/neat/workflows/examples/workflows/basic/workflow.yaml` & `cognite_neat-0.18.2/cognite/neat/workflows/examples/basic/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/workflows/examples/workflows/default/workflow.py` & `cognite_neat-0.18.2/cognite/neat/workflows/examples/default/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,17 @@
     upload_relationships,
 )
 from cognite.neat.graph.extractors import NeatGraphStore, drop_graph_store
 from cognite.neat.rules.exporter.rules2triples import get_instances_as_triples
 from cognite.neat.rules.models import TransformationRules
 from cognite.neat.graph.transformations.transformer import RuleProcessingReport, domain2app_knowledge_graph
 from cognite.neat.graph.loaders.validator import validate_asset_hierarchy
-from cognite.neat.workflows.workflow import utils
-from cognite.neat.workflows.workflow.base import BaseWorkflow, FlowMessage
-from cognite.neat.workflows.workflow.cdf_store import CdfStore
+from cognite.neat.workflows import utils
+from cognite.neat.workflows.base import BaseWorkflow, FlowMessage
+from cognite.neat.workflows.cdf_store import CdfStore
 
 with contextlib.suppress(ValueError):
     prom_cdf_resource_stats = Gauge(
         "neat_default_wf_cdf_resource_stats",
         "CDF resource stats before and after running default workflow",
         ["resource_type", "state"],
     )
```

### Comparing `cognite_neat-0.18.1/cognite/neat/workflows/examples/workflows/default/workflow.yaml` & `cognite_neat-0.18.2/cognite/neat/workflows/examples/default/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/workflows/examples/workflows/fdm_schema_generation/workflow.py` & `cognite_neat-0.18.2/cognite/neat/workflows/examples/fdm_schema_generation/workflow.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import logging
 import time
 from pathlib import Path
 
 from cognite.client import CogniteClient
 
 from cognite.neat import rules
-from cognite.neat.graph import loaders
+from cognite.neat.rules.exporter.rules2graphql import GraphQLSchema
 from cognite.neat.graph.extractors import NeatGraphStore
 from cognite.neat.rules.models import TransformationRules
-from cognite.neat.workflows.workflow import utils
-from cognite.neat.workflows.workflow.base import BaseWorkflow, FlowMessage
-from cognite.neat.workflows.workflow.cdf_store import CdfStore
+from cognite.neat.workflows import utils
+from cognite.neat.workflows.base import BaseWorkflow, FlowMessage
+from cognite.neat.workflows.cdf_store import CdfStore
 
 
 class FDMSchemaGenerationNeatWorkflow(BaseWorkflow):
     def __init__(self, name: str, client: CogniteClient):
         super().__init__(name, client, [])
         self.counter = 0
         self.metrics.register_metric("counter_1", "", "counter", ["step"])
@@ -54,15 +54,15 @@
         logging.info(f"Loaded prefixes {str(self.transformation_rules.prefixes)} rules")
         output_text = f"Loaded {len(self.transformation_rules.properties)} rules"
         logging.info(output_text)
         return FlowMessage(output_text=output_text)
 
     def step_generate_fdm_schema(self, flow_msg: FlowMessage = None):
         logging.info("Generating FDM schema")
-        self.data_model_gql = loaders.rules2graphql_schema(self.transformation_rules)
+        self.data_model_gql = GraphQLSchema(self.transformation_rules, verbose=True).schema
 
         default_name = (
             f"{self.transformation_rules.metadata.prefix}-"
             f"v{self.transformation_rules.metadata.version.strip().replace('.', '_')}"
             ".graphql"
         )
         schema_name = self.get_config_item_value("fdm_schema.file", default_name)
```

### Comparing `cognite_neat-0.18.1/cognite/neat/workflows/examples/workflows/fdm_schema_generation/workflow.yaml` & `cognite_neat-0.18.2/cognite/neat/workflows/examples/fdm_schema_generation/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/workflows/examples/workflows/graph_db_import/workflow.py` & `cognite_neat-0.18.2/cognite/neat/workflows/examples/graph_db_import/workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 import requests
 from cognite.client import CogniteClient
 
 from cognite.neat.graph.extractors import NeatGraphStore
 from cognite.neat.rules.models import TransformationRules
-from cognite.neat.workflows.workflow import BaseWorkflow, FlowMessage
+from cognite.neat.workflows import BaseWorkflow, FlowMessage
 
 
 class GraphDbImportNeatWorkflow(BaseWorkflow):
     def __init__(self, name: str, client: CogniteClient):
         super().__init__(name, client, [])
         self.dataset_id: int = 0
         self.current_step: str = None
```

### Comparing `cognite_neat-0.18.1/cognite/neat/workflows/examples/workflows/graph_db_import/workflow.yaml` & `cognite_neat-0.18.2/cognite/neat/workflows/examples/graph_db_import/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/workflows/examples/workflows/graph_to_asset_hierarchy/workflow.yaml` & `cognite_neat-0.18.2/cognite/neat/workflows/examples/graph_to_asset_hierarchy/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/workflows/examples/workflows/sheet2cdf/workflow.yaml` & `cognite_neat-0.18.2/cognite/neat/workflows/examples/sheet2cdf/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/workflows/examples/workflows/sme_graph_capture/workflow.yaml` & `cognite_neat-0.18.2/cognite/neat/workflows/examples/sme_graph_capture/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/workflows/migration/wf_manifests.py` & `cognite_neat-0.18.2/cognite/neat/workflows/migration/wf_manifests.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/workflows/steps/data_contracts.py` & `cognite_neat-0.18.2/cognite/neat/workflows/steps/data_contracts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 
 from cognite.client import CogniteClient
 
 from cognite.neat.graph.extractors import NeatGraphStore
 from cognite.neat.rules.models import TransformationRules
-from cognite.neat.workflows.workflow.step_model import DataContract
+from cognite.neat.workflows.step_model import DataContract
 
 
 class RulesData(DataContract):
     rules: TransformationRules
 
     @property
     def dataset_id(self) -> int:
```

### Comparing `cognite_neat-0.18.1/cognite/neat/workflows/steps/steps.py` & `cognite_neat-0.18.2/cognite/neat/workflows/steps/steps.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 from pathlib import Path
 from typing import Optional, Tuple
 
 from ...graph import extractors
 from cognite.neat.graph.loaders import upload_labels
 from cognite.neat.rules import parse_rules_from_excel_file
-from cognite.neat.workflows.workflow.model import FlowMessage
-from cognite.neat.workflows.workflow.step_model import Step
+from cognite.neat.workflows.model import FlowMessage
+from cognite.neat.workflows.step_model import Step
 from .data_contracts import ClientData, PathData, RulesData, SourceGraphData
 
 __all__ = [
     "LoadTransformationRules",
     "ConfiguringStores",
     "LoadInstancesToGraph",
     "CreateCDFLabels",
```

### Comparing `cognite_neat-0.18.1/cognite/neat/workflows/workflow/base.py` & `cognite_neat-0.18.2/cognite/neat/workflows/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 import yaml
 from cognite.client import CogniteClient
 from prometheus_client import Gauge
 
 from cognite.neat.graph.extractors.data_stores.metrics import NeatMetricsCollector
 from cognite.neat.exceptions import InvalidWorkFlowError
 from cognite.neat.utils.utils import retry_decorator
-from cognite.neat.workflows.workflow.model import (
+from cognite.neat.workflows.model import (
     FlowMessage,
     StepExecutionStatus,
     StepType,
     WorkflowConfigItem,
     WorkflowDefinition,
     WorkflowFullStateReport,
     WorkflowStartException,
     WorkflowState,
     WorkflowStepDefinition,
     WorkflowStepEvent,
     WorkflowSystemComponent,
 )
-from cognite.neat.workflows.workflow.tasks import WorkflowTaskBuilder
+from cognite.neat.workflows.tasks import WorkflowTaskBuilder
 
 from cognite.neat.app.api.configuration import Config
 from cognite.neat.utils.cdf import CogniteClientConfig
 from . import utils, cdf_store
 from .step_model import DataContract
 import cognite.neat.workflows.steps.steps
```

### Comparing `cognite_neat-0.18.1/cognite/neat/workflows/workflow/cdf_store.py` & `cognite_neat-0.18.2/cognite/neat/workflows/cdf_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from typing import Dict
 
 from cognite.client import CogniteClient
 from cognite.client.data_classes import Event, FileMetadataUpdate, LabelDefinition, LabelFilter
 from fastapi.encoders import jsonable_encoder
 from pydantic import BaseModel
 
-from cognite.neat.workflows.workflow.model import WorkflowFullStateReport, WorkflowState, WorkflowStepEvent
-from cognite.neat.workflows.workflow.utils import get_file_hash
+from cognite.neat.workflows.model import WorkflowFullStateReport, WorkflowState, WorkflowStepEvent
+from cognite.neat.workflows.utils import get_file_hash
 
 
 class NeatCdfResource(BaseModel):
     id: int = None
     name: str
     rtype: str
     last_updated_time: int = None
```

### Comparing `cognite_neat-0.18.1/cognite/neat/workflows/workflow/manager.py` & `cognite_neat-0.18.2/cognite/neat/workflows/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 import traceback
 from pathlib import Path
 
 from cognite.client import CogniteClient
 from prometheus_client import Gauge
 from pydantic import BaseModel
 
-from cognite.neat.workflows.workflow import BaseWorkflow
-from cognite.neat.workflows.workflow.base import WorkflowDefinition
-from cognite.neat.workflows.workflow.model import FlowMessage, InstanceStartMethod, WorkflowState
-from cognite.neat.workflows.workflow.tasks import WorkflowTaskBuilder
+from cognite.neat.workflows import BaseWorkflow
+from cognite.neat.workflows.base import WorkflowDefinition
+from cognite.neat.workflows.model import FlowMessage, InstanceStartMethod, WorkflowState
+from cognite.neat.workflows.tasks import WorkflowTaskBuilder
 
 live_workflow_instances = Gauge("neat_workflow_live_instances", "Count of live workflow instances", ["itype"])
 
 
 class WorkflowStartStatus(BaseModel):
     workflow_instance: BaseWorkflow = None
     is_success: bool = True
```

### Comparing `cognite_neat-0.18.1/cognite/neat/workflows/workflow/model.py` & `cognite_neat-0.18.2/cognite/neat/workflows/model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/workflows/workflow/step_model.py` & `cognite_neat-0.18.2/cognite/neat/workflows/step_model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.18.1/cognite/neat/workflows/workflow/tasks.py` & `cognite_neat-0.18.2/cognite/neat/workflows/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from cognite.client import CogniteClient
 
-from cognite.neat.workflows.workflow.model import FlowMessage
+from cognite.neat.workflows.model import FlowMessage
 
 
 class WorkflowTaskBuilder:
     """Collection of all base tasks for workflows.All tasks must run in the context of a workflow including threads."""
 
     def __init__(self, cdf_client: CogniteClient, worflow_manager):
         # TODO : figure out ciclura import and set type to WorkflowManager
```

### Comparing `cognite_neat-0.18.1/cognite/neat/workflows/workflow/triggers.py` & `cognite_neat-0.18.2/cognite/neat/workflows/triggers.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import logging
 import threading
 import time
 
 import schedule
 from fastapi import Depends, FastAPI, Request
 
-from cognite.neat.workflows.workflow.manager import WorkflowManager
-from cognite.neat.workflows.workflow.model import FlowMessage, StepType, WorkflowState
+from cognite.neat.workflows.manager import WorkflowManager
+from cognite.neat.workflows.model import FlowMessage, StepType, WorkflowState
 
 
 async def get_body(request: Request):
     return await request.body()
 
 
 fast_api_depends = Depends(get_body)
```

### Comparing `cognite_neat-0.18.1/pyproject.toml` & `cognite_neat-0.18.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-neat"
-version = "0.18.1"
+version = "0.18.2"
 readme = "README.md"
 description = "Knowledge graph transformation"
 authors = ["Nikola Vasiljevic <nikola.vasiljevic@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>",
     "Aleksandrs Livincovs <aleksandrs.livincovs@cognite.com>"]
 license = "Apache-2.0"
 documentation = "https://cognite-neat.readthedocs-hosted.com/"
@@ -60,14 +60,15 @@
 mkdocs =  {version="*", optional=true}
 mkdocs-jupyter = {version="*", optional=true}
 mkdocs-material-extensions = {version="*", optional=true}
 mkdocs-git-revision-date-localized-plugin = {version="*", optional=true}
 mkdocs-git-authors-plugin = {version="*", optional=true}
 mkdocs-gitbook = {version="*", optional=true}
 mkdocs-glightbox = {version="*", optional=true}
+jinja2 = {version = "^3.1.2", optional=true}
 
 [tool.poetry.extras]
 docs = ["mkdocs", "mkdocs-jupyter", "mkdocs-material-extensions", "mkdocs-git-revision-date-localized-plugin", "mkdocs-git-authors-plugin", "mkdocs-gitbook", "mkdocs-glightbox"]
 google = ["gspread", "google-api-python-client", "google-auth-oauthlib"]
 excel = ["openpyxl"]
 graphql = ["jinja2"]
 all = ["gspread", "google-api-python-client", "google-auth-oauthlib", "openpyxl", "jinja2"]
```

### Comparing `cognite_neat-0.18.1/PKG-INFO` & `cognite_neat-0.18.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-neat
-Version: 0.18.1
+Version: 0.18.2
 Summary: Knowledge graph transformation
 Home-page: https://cognite-neat.readthedocs-hosted.com/
 License: Apache-2.0
 Author: Nikola Vasiljevic
 Author-email: nikola.vasiljevic@cognite.com
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,14 +18,15 @@
 Requires-Dist: PyYAML
 Requires-Dist: cognite-sdk (>=6,<7)
 Requires-Dist: deepdiff
 Requires-Dist: fastapi (>=0.100,<0.101)
 Requires-Dist: google-api-python-client ; extra == "google" or extra == "all"
 Requires-Dist: google-auth-oauthlib ; extra == "google" or extra == "all"
 Requires-Dist: gspread ; extra == "google" or extra == "all"
+Requires-Dist: jinja2 (>=3.1.2,<4.0.0) ; extra == "graphql" or extra == "all"
 Requires-Dist: mkdocs ; extra == "docs"
 Requires-Dist: mkdocs-git-authors-plugin ; extra == "docs"
 Requires-Dist: mkdocs-git-revision-date-localized-plugin ; extra == "docs"
 Requires-Dist: mkdocs-gitbook ; extra == "docs"
 Requires-Dist: mkdocs-glightbox ; extra == "docs"
 Requires-Dist: mkdocs-jupyter ; extra == "docs"
 Requires-Dist: mkdocs-material-extensions ; extra == "docs"
@@ -47,97 +48,95 @@
 # kNowlEdge grAph Transformer (NEAT)
 
 This is python package handles transformation of domain knowledge graphs (more detailed, overarching) to app specific knowledge graphs.
 
 ## Quickstart
 
 ### Option 1 - Python Package
+
 `neat` can be installed as a Python package, and a docker image for more robust execution and support such
 as `graphdb` for caching. This quickstart guide uses the Python package.
 
 ### Option 2 - Docker container
 
 Running NEAT as docker container :
 `docker run -p 8000:8000 --name neat cognite/neat:latest`
 
 Runnin NEAT as docker container with local data folder mounted :
 `docker run -p 8000:8000 --name neat -v $(shell pwd)/docker/vol_data:/app/data  cognite/neat:latest`
 
-
 ### Installation (Development setup)
+
 Prerequisites:
-* `poetry` installed on your system, [see installation](https://python-poetry.org/docs/).
-* `npm` installed on your system, [see installation](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
-* `react-scripts` installed on your system, [`npm i react-scripts`](https://www.npmjs.com/package/react-scripts)
+
+- `poetry` installed on your system, [see installation](https://python-poetry.org/docs/).
+- `npm` installed on your system, [see installation](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
+- `react-scripts` installed on your system, [`npm i react-scripts`](https://www.npmjs.com/package/react-scripts)
 
 1. Clone this repo: `git clone git@github.com:cognitedata/neat.git`
 2. Create wheel: `make build-python`. This will create a wheel in the `dist` folder.
 3. Install wheel in your preferred environment, `pip install dist/neat-[NEAT_VERSTION]-py3-none-any.whl`
 
-
 ### Run Neat (Python Package)
 
 Once installed you can run neat with the command
+
 ```bash
 neat
 ```
+
 This will open your browser and launch the neat application.
 
 Note this will automatically create a `data` folder in your current working directory, which is populated
 with default workflows, rule sheets, and source graphs. In addition, there is a `config.yaml` you can add
 your CDF credentials to allow `neat` access CDF.
 
 ![launch_neat](https://user-images.githubusercontent.com/60234212/228812422-c5e9519f-19e7-4f08-9617-66a790323c7e.gif)
 
-
 ## Documentation
 
 [Documentation](https://cognite-neat.readthedocs-hosted.com/en/latest/)
 
 ![](./docs/figs/high-level-io.png)
 
-
 ## Docker container build process
 
-
-``` make build-docker ```
+`make build-docker`
 
 ## Starting the application locally using GraphDB as external rdf store
 
 Run the command :
 
-``` make compose-up```
-
-The command starts NEAT container and GraphDB container and creates *vol_data* and *vol_shared* local folders that are mounted as volumes.
+` make compose-up`
 
-*vol_data* - is mounted only in NEAT container. It contains `config.yaml`, `workflows`, `rules`. You can set `load_examples` to `true` to populate it with examples.
+The command starts NEAT container and GraphDB container and creates _vol_data_ and _vol_shared_ local folders that are mounted as volumes.
 
-*vol_shared* - is mounted to both containers and files placed here become automatically visible for GraphDB import process. Main intension is to write files from NEAT container and make them available for GraphDB for import.
+_vol_data_ - is mounted only in NEAT container. It contains `config.yaml`, `workflows`, `rules`. You can set `load_examples` to `true` to populate it with examples.
 
+_vol_shared_ - is mounted to both containers and files placed here become automatically visible for GraphDB import process. Main intension is to write files from NEAT container and make them available for GraphDB for import.
 
 ## Web UI
 
-``` http://localhost:8000 ```
+`http://localhost:8000`
 
 Open API docs :
 
-``` http://localhost:8000/docs ```
+`http://localhost:8000/docs`
 
 Prom metrics :
 
-``` http://localhost:8000/metrics ```
-
+`http://localhost:8000/metrics`
 
 ## Workflows and configurations
 
 All configurations are divided into 2 categories :
+
 - global configurations - global for entire service , loaded at startup (config.yaml)
 - workflow configurations - local to workflow , loaded from workflow manifest (.yaml)
 
-
 ## Global configurations
 
 Global configurations loaded by the application during startup process, either from ENV variables or file.
 
 The application tries to load the configuration as follows.
 
 1. Try ENV variables. This is done by checking for the ENV variable `NEAT_CDF_PROJECT`, and if it exists load the rest
@@ -163,75 +162,78 @@
 ### Config file
 
 ```yaml
 workflows_store_type: file
 data_store_path: /app/data
 
 cdf_client:
-    project: get-power-grid
-    client_id: "623c2450-cfc2-43d6-9036-10e14dad8ccf"
-    client_secret: "my-super-secret"
-    client_name: neat-test-service
-    base_url: https://az-power-no-northeurope.cognitedata.com
-    scopes:
-      - https://az-power-no-northeurope.cognitedata.com/.default
-    token_url: https://login.microsoftonline.com/e55e1701-82f8-4c52-af10-28e4d942c589/oauth2/v2.0/token
+  project: get-power-grid
+  client_id: "623c2450-cfc2-43d6-9036-10e14dad8ccf"
+  client_secret: "my-super-secret"
+  client_name: neat-test-service
+  base_url: https://az-power-no-northeurope.cognitedata.com
+  scopes:
+    - https://az-power-no-northeurope.cognitedata.com/.default
+  token_url: https://login.microsoftonline.com/e55e1701-82f8-4c52-af10-28e4d942c589/oauth2/v2.0/token
 
 cdf_default_dataset_id: 2626756768281823
 workflow_downloader_filter:
-    - tag:grid
+  - tag:grid
 log_level: DEBUG
 ```
 
 ## Automatic workflow loading from CDF during application startup
 
 If `workflow_downloader_filter` is set, the app will try to download workflows from CDF based on provided filtering conditions .
 Filtering format :
+
 - `name:<workflows_name>=<workflow_version>` - loading workflow by name and version or latest by name if version is not set.
 - `tag:<tag_name>`- loading all workflows that tagged with specific tag.
 
 ## Workflow level configurations
 
 Each workflow can have own unique subset of configurations defined in `config.yaml` file. There is also a small subset of system
 configurations that can be set on workflow level.
 
 System configurations:
 
 - system.execution_reporting_type - controls how workflow execution log should be reported to CDF . Supported values : `all_disabled`, `all_enabled`(default)
 
 Example :
+
 ```yaml
--   group: system
-    name: system.execution_reporting_type
-    value: all_disabled
+- group: system
+  name: system.execution_reporting_type
+  value: all_disabled
 ```
 
 ## How to develop your first workflow
 
 The NEAT framework has few conventions :
+
 - Each workflow must reside in its own folder
 - Workflow folder must contain at least 2 files :
-    - `workflow.py` - steps implementation file
-    - `workflow.yaml` - manifest and configurations
+  - `workflow.py` - steps implementation file
+  - `workflow.yaml` - manifest and configurations
 
- ### Workflow steps implementation file
+### Workflow steps implementation file
 
- Must implement `BaseWorkflow` class from `from cognite.neat.core.workflow.base`
+Must implement `BaseWorkflow` class from `from cognite.neat.core.workflow.base`
 
- Each method that should be orchestrated by workflow engine must be prefixed with `step_` , each method must have single argument of `FlowMessage` type and return `FlowMessage` or `None`.
- FlowMessage is passed from one step to another and it's captured in execution log.
+Each method that should be orchestrated by workflow engine must be prefixed with `step_` , each method must have single argument of `FlowMessage` type and return `FlowMessage` or `None`.
+FlowMessage is passed from one step to another and it's captured in execution log.
 
 Simplest `workflow.py`
 
-````python
+```python
 
 import logging
 from cognite.client import CogniteClient
-from cognite.neat.workflows.workflow import BaseWorkflow
-from cognite.neat.workflows.workflow import FlowMessage
+from cognite.neat.workflows import BaseWorkflow
+from cognite.neat.workflows import FlowMessage
 
 
 class PlaygroundNeatWorkflow(BaseWorkflow):
     def __init__(self, name: str, client: CogniteClient):
         super().__init__(name, client, [])
 
     def step_run_experiment_1(self, flow_msg: FlowMessage = None):
@@ -239,91 +241,90 @@
         logging.info("Done running experiment 4444")
 
         return FlowMessage(output_text="Done running experiment 1")
 
     def step_cleanup(self, flow_msg: FlowMessage = None):
         logging.info("Cleanup")
 
-````
+```
 
 Manifest `workflow.yaml` , normally should be updated from UI
-````yaml
+
+```yaml
 configs:
--   group: source_rdf_store
+  - group: source_rdf_store
     label: null
     name: source_rdf_store.type
     options: null
     required: false
     type: null
     value: graphdb
 description: null
 groups:
--   description: null
+  - description: null
     id: experimentation_system
     label: Experimentation playground
     transition_to: null
     ui_config:
-        pos_x: 171
-        pos_y: 6
+      pos_x: 171
+      pos_y: 6
 implementation_module: null
 name: playground
 steps:
--   description: null
+  - description: null
     enabled: true
     group_id: null
     id: run_experiment_1
     label: Running first experiment
     method: null
     params: {}
     stype: pystep
     transition_to:
-    - cleanup
+      - cleanup
     trigger: false
     ui_config:
-        pos_x: 340
-        pos_y: 144
--   description: null
+      pos_x: 340
+      pos_y: 144
+  - description: null
     enabled: true
     group_id: null
     id: cleanup
     label: Cleanup
     method: null
     params: null
     stype: pystep
     transition_to: []
     trigger: false
     ui_config:
-        pos_x: 295
-        pos_y: 303
--   description: null
+      pos_x: 295
+      pos_y: 303
+  - description: null
     enabled: true
     group_id: null
     id: step_trigger
     label: HTTP trigger
     method: null
     params: {}
     stype: http_trigger
     transition_to:
-    - run_experiment_1
+      - run_experiment_1
     trigger: true
     ui_config:
-        pos_x: 336
-        pos_y: 44
--   description: null
+      pos_x: 336
+      pos_y: 44
+  - description: null
     enabled: false
     group_id: null
     id: step_295076
     label: Run every 10 sec
     method: null
     params:
-        interval: every 10 seconds
+      interval: every 10 seconds
     stype: time_trigger
     transition_to:
-    - run_experiment_1
+      - run_experiment_1
     trigger: true
     ui_config:
-        pos_x: 544
-        pos_y: 42
-
-
-````
+      pos_x: 544
+      pos_y: 42
+```
```

