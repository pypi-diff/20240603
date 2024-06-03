# Comparing `tmp/cognite_neat-0.78.2.tar.gz` & `tmp/cognite_neat-0.78.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_neat-0.78.2.tar", max compression
+gzip compressed data, was "cognite_neat-0.78.3.tar", max compression
```

## Comparing `cognite_neat-0.78.2.tar` & `cognite_neat-0.78.3.tar`

### file list

```diff
@@ -1,282 +1,282 @@
--rw-r--r--   0        0        0    11351 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/LICENSE
--rw-r--r--   0        0        0     6775 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/README.md
--rw-r--r--   0        0        0       61 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/__init__.py
--rw-r--r--   0        0        0       23 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/_version.py
--rw-r--r--   0        0        0        0 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/api/__init__.py
--rw-r--r--   0        0        0      152 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/api/asgi/metrics.py
--rw-r--r--   0        0        0     4232 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/api/configuration.py
--rw-r--r--   0        0        0       90 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/api/context_manager/__init__.py
--rw-r--r--   0        0        0      380 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/api/context_manager/manager.py
--rw-r--r--   0        0        0        0 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/api/data_classes/__init__.py
--rw-r--r--   0        0        0     1675 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/api/data_classes/rest.py
--rw-r--r--   0        0        0     1891 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/api/explorer.py
--rw-r--r--   0        0        0      585 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/api/routers/configuration.py
--rw-r--r--   0        0        0     3523 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/api/routers/core.py
--rw-r--r--   0        0        0     4597 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/api/routers/crud.py
--rw-r--r--   0        0        0    13686 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/api/routers/data_exploration.py
--rw-r--r--   0        0        0      210 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/api/routers/metrics.py
--rw-r--r--   0        0        0     8121 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/api/routers/rules.py
--rw-r--r--   0        0        0    12393 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/api/routers/workflows.py
--rw-r--r--   0        0        0        0 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/api/utils/__init__.py
--rw-r--r--   0        0        0      564 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/api/utils/data_mapping.py
--rw-r--r--   0        0        0      806 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/api/utils/logging.py
--rw-r--r--   0        0        0     4594 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/api/utils/query_templates.py
--rw-r--r--   0        0        0      357 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/main.py
--rw-r--r--   0        0        0        0 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/monitoring/__init__.py
--rw-r--r--   0        0        0     2690 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/monitoring/metrics.py
--rw-r--r--   0        0        0       16 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/ui/index.html
--rw-r--r--   0        0        0      312 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/ui/neat-app/.gitignore
--rw-r--r--   0        0        0     3359 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/ui/neat-app/README.md
--rw-r--r--   0        0        0      464 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/ui/neat-app/build/asset-manifest.json
--rw-r--r--   0        0        0    15406 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/ui/neat-app/build/favicon.ico
--rw-r--r--   0        0        0    10756 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg
--rw-r--r--   0        0        0     8374 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg
--rw-r--r--   0        0        0     5333 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg
--rw-r--r--   0        0        0      629 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/ui/neat-app/build/index.html
--rw-r--r--   0        0        0   344557 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/ui/neat-app/build/logo192.png
--rw-r--r--   0        0        0      492 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/ui/neat-app/build/manifest.json
--rw-r--r--   0        0        0       67 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/ui/neat-app/build/robots.txt
--rw-r--r--   0        0        0     8524 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
--rw-r--r--   0        0        0    13319 2024-05-31 12:10:13.171062 cognite_neat-0.78.2/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
--rw-r--r--   0        0        0  1423717 2024-05-31 12:10:13.179062 cognite_neat-0.78.2/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js
--rw-r--r--   0        0        0     2667 2024-05-31 12:10:13.179062 cognite_neat-0.78.2/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.LICENSE.txt
--rw-r--r--   0        0        0  6282875 2024-05-31 12:10:13.203062 cognite_neat-0.78.2/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.map
--rw-r--r--   0        0        0   240334 2024-05-31 12:10:13.203062 cognite_neat-0.78.2/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg
--rw-r--r--   0        0        0     6145 2024-05-31 12:10:13.211062 cognite_neat-0.78.2/cognite/neat/config.py
--rw-r--r--   0        0        0     1300 2024-05-31 12:10:13.211062 cognite_neat-0.78.2/cognite/neat/constants.py
--rw-r--r--   0        0        0     4268 2024-05-31 12:10:13.211062 cognite_neat-0.78.2/cognite/neat/exceptions.py
--rw-r--r--   0        0        0       73 2024-05-31 12:10:13.211062 cognite_neat-0.78.2/cognite/neat/graph/__init__.py
--rw-r--r--   0        0        0  1439359 2024-05-31 12:10:13.215062 cognite_neat-0.78.2/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
--rw-r--r--   0        0        0  1437996 2024-05-31 12:10:13.219062 cognite_neat-0.78.2/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0      368 2024-05-31 12:10:13.219062 cognite_neat-0.78.2/cognite/neat/graph/examples/__init__.py
--rw-r--r--   0        0        0    45798 2024-05-31 12:10:13.219062 cognite_neat-0.78.2/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
--rw-r--r--   0        0        0     3401 2024-05-31 12:10:13.219062 cognite_neat-0.78.2/cognite/neat/graph/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-31 12:10:13.219062 cognite_neat-0.78.2/cognite/neat/graph/extractors/__init__.py
--rw-r--r--   0        0        0      356 2024-05-31 12:10:13.219062 cognite_neat-0.78.2/cognite/neat/graph/extractors/_base.py
--rw-r--r--   0        0        0    14961 2024-05-31 12:10:13.219062 cognite_neat-0.78.2/cognite/neat/graph/extractors/_mock_graph_generator.py
--rw-r--r--   0        0        0      149 2024-05-31 12:10:13.219062 cognite_neat-0.78.2/cognite/neat/graph/models.py
--rw-r--r--   0        0        0      543 2024-05-31 12:10:13.219062 cognite_neat-0.78.2/cognite/neat/graph/stores/__init__.py
--rw-r--r--   0        0        0    13473 2024-05-31 12:10:13.219062 cognite_neat-0.78.2/cognite/neat/graph/stores/_base.py
--rw-r--r--   0        0        0     1776 2024-05-31 12:10:13.219062 cognite_neat-0.78.2/cognite/neat/graph/stores/_graphdb_store.py
--rw-r--r--   0        0        0     1420 2024-05-31 12:10:13.219062 cognite_neat-0.78.2/cognite/neat/graph/stores/_memory_store.py
--rw-r--r--   0        0        0     5448 2024-05-31 12:10:13.219062 cognite_neat-0.78.2/cognite/neat/graph/stores/_oxigraph_store.py
--rw-r--r--   0        0        0     9569 2024-05-31 12:10:13.219062 cognite_neat-0.78.2/cognite/neat/graph/stores/_oxrdflib.py
--rw-r--r--   0        0        0     1244 2024-05-31 12:10:13.219062 cognite_neat-0.78.2/cognite/neat/graph/stores/_rdf_to_graph.py
--rw-r--r--   0        0        0        0 2024-05-31 12:10:13.219062 cognite_neat-0.78.2/cognite/neat/legacy/__init__.py
--rw-r--r--   0        0        0       73 2024-05-31 12:10:13.219062 cognite_neat-0.78.2/cognite/neat/legacy/graph/__init__.py
--rw-r--r--   0        0        0  1439359 2024-05-31 12:10:13.223062 cognite_neat-0.78.2/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
--rw-r--r--   0        0        0  1437996 2024-05-31 12:10:13.223062 cognite_neat-0.78.2/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0      368 2024-05-31 12:10:13.223062 cognite_neat-0.78.2/cognite/neat/legacy/graph/examples/__init__.py
--rw-r--r--   0        0        0    45798 2024-05-31 12:10:13.223062 cognite_neat-0.78.2/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx
--rw-r--r--   0        0        0     3401 2024-05-31 12:10:13.223062 cognite_neat-0.78.2/cognite/neat/legacy/graph/exceptions.py
--rw-r--r--   0        0        0      258 2024-05-31 12:10:13.223062 cognite_neat-0.78.2/cognite/neat/legacy/graph/extractors/__init__.py
--rw-r--r--   0        0        0      363 2024-05-31 12:10:13.223062 cognite_neat-0.78.2/cognite/neat/legacy/graph/extractors/_base.py
--rw-r--r--   0        0        0    11734 2024-05-31 12:10:13.223062 cognite_neat-0.78.2/cognite/neat/legacy/graph/extractors/_dexpi.py
--rw-r--r--   0        0        0    17695 2024-05-31 12:10:13.223062 cognite_neat-0.78.2/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py
--rw-r--r--   0        0        0    14908 2024-05-31 12:10:13.223062 cognite_neat-0.78.2/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py
--rw-r--r--   0        0        0      701 2024-05-31 12:10:13.223062 cognite_neat-0.78.2/cognite/neat/legacy/graph/loaders/__init__.py
--rw-r--r--   0        0        0    23823 2024-05-31 12:10:13.223062 cognite_neat-0.78.2/cognite/neat/legacy/graph/loaders/_asset_loader.py
--rw-r--r--   0        0        0     2383 2024-05-31 12:10:13.223062 cognite_neat-0.78.2/cognite/neat/legacy/graph/loaders/_base.py
--rw-r--r--   0        0        0     2835 2024-05-31 12:10:13.223062 cognite_neat-0.78.2/cognite/neat/legacy/graph/loaders/_exceptions.py
--rw-r--r--   0        0        0        0 2024-05-31 12:10:13.223062 cognite_neat-0.78.2/cognite/neat/legacy/graph/loaders/core/__init__.py
--rw-r--r--   0        0        0     2321 2024-05-31 12:10:13.223062 cognite_neat-0.78.2/cognite/neat/legacy/graph/loaders/core/labels.py
--rw-r--r--   0        0        0     5023 2024-05-31 12:10:13.223062 cognite_neat-0.78.2/cognite/neat/legacy/graph/loaders/core/models.py
--rw-r--r--   0        0        0    40464 2024-05-31 12:10:13.223062 cognite_neat-0.78.2/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py
--rw-r--r--   0        0        0    22707 2024-05-31 12:10:13.223062 cognite_neat-0.78.2/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py
--rw-r--r--   0        0        0    12979 2024-05-31 12:10:13.223062 cognite_neat-0.78.2/cognite/neat/legacy/graph/loaders/rdf_to_dms.py
--rw-r--r--   0        0        0     3328 2024-05-31 12:10:13.223062 cognite_neat-0.78.2/cognite/neat/legacy/graph/loaders/validator.py
--rw-r--r--   0        0        0      149 2024-05-31 12:10:13.223062 cognite_neat-0.78.2/cognite/neat/legacy/graph/models.py
--rw-r--r--   0        0        0      543 2024-05-31 12:10:13.223062 cognite_neat-0.78.2/cognite/neat/legacy/graph/stores/__init__.py
--rw-r--r--   0        0        0    14289 2024-05-31 12:10:13.223062 cognite_neat-0.78.2/cognite/neat/legacy/graph/stores/_base.py
--rw-r--r--   0        0        0     1776 2024-05-31 12:10:13.223062 cognite_neat-0.78.2/cognite/neat/legacy/graph/stores/_graphdb_store.py
--rw-r--r--   0        0        0     1420 2024-05-31 12:10:13.223062 cognite_neat-0.78.2/cognite/neat/legacy/graph/stores/_memory_store.py
--rw-r--r--   0        0        0     5448 2024-05-31 12:10:13.223062 cognite_neat-0.78.2/cognite/neat/legacy/graph/stores/_oxigraph_store.py
--rw-r--r--   0        0        0     9569 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/graph/stores/_oxrdflib.py
--rw-r--r--   0        0        0     1244 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/graph/stores/_rdf_to_graph.py
--rw-r--r--   0        0        0        0 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/graph/transformations/__init__.py
--rw-r--r--   0        0        0     4765 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/graph/transformations/entity_matcher.py
--rw-r--r--   0        0        0       73 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/graph/transformations/query_generator/__init__.py
--rw-r--r--   0        0        0    18719 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/graph/transformations/query_generator/sparql.py
--rw-r--r--   0        0        0    14737 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/graph/transformations/transformer.py
--rw-r--r--   0        0        0        0 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/rules/__init__.py
--rw-r--r--   0        0        0     8610 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/rules/analysis.py
--rw-r--r--   0        0        0    58987 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx
--rw-r--r--   0        0        0    80226 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx
--rw-r--r--   0        0        0      858 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/rules/examples/__init__.py
--rw-r--r--   0        0        0     2598 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/rules/examples/power-grid-containers.yaml
--rw-r--r--   0        0        0    77055 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/rules/examples/power-grid-example.xlsx
--rw-r--r--   0        0        0     5567 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/rules/examples/power-grid-model.yaml
--rw-r--r--   0        0        0    75865 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/rules/examples/rules-template.xlsx
--rw-r--r--   0        0        0    52433 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx
--rw-r--r--   0        0        0    26008 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/rules/examples/skos-rules.xlsx
--rw-r--r--   0        0        0    79981 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx
--rw-r--r--   0        0        0    65934 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/rules/examples/wind-energy.owl
--rw-r--r--   0        0        0   123868 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/rules/exceptions.py
--rw-r--r--   0        0        0      574 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/rules/exporters/__init__.py
--rw-r--r--   0        0        0     1453 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/rules/exporters/_base.py
--rw-r--r--   0        0        0      102 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/rules/exporters/_core/__init__.py
--rw-r--r--   0        0        0      771 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/rules/exporters/_core/rules2labels.py
--rw-r--r--   0        0        0    36813 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/rules/exporters/_rules2dms.py
--rw-r--r--   0        0        0     8312 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/rules/exporters/_rules2excel.py
--rw-r--r--   0        0        0     6251 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/rules/exporters/_rules2graphql.py
--rw-r--r--   0        0        0    18458 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/rules/exporters/_rules2ontology.py
--rw-r--r--   0        0        0    28805 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py
--rw-r--r--   0        0        0     3881 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/rules/exporters/_rules2rules.py
--rw-r--r--   0        0        0     1085 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/rules/exporters/_rules2triples.py
--rw-r--r--   0        0        0     5767 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/rules/exporters/_validation.py
--rw-r--r--   0        0        0      636 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/rules/importers/__init__.py
--rw-r--r--   0        0        0     2273 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/rules/importers/_base.py
--rw-r--r--   0        0        0     6476 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/rules/importers/_dict2rules.py
--rw-r--r--   0        0        0     7697 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/rules/importers/_dms2rules.py
--rw-r--r--   0        0        0    12093 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/rules/importers/_graph2rules.py
--rw-r--r--   0        0        0     1610 2024-05-31 12:10:13.227062 cognite_neat-0.78.2/cognite/neat/legacy/rules/importers/_json2rules.py
--rw-r--r--   0        0        0       63 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/legacy/rules/importers/_owl2rules/__init__.py
--rw-r--r--   0        0        0     8304 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     9407 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     8019 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0    10557 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0     1502 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py
--rw-r--r--   0        0        0      421 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/legacy/rules/importers/_xsd2rules.py
--rw-r--r--   0        0        0     1601 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/legacy/rules/importers/_yaml2rules.py
--rw-r--r--   0        0        0      127 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/legacy/rules/models/__init__.py
--rw-r--r--   0        0        0     4989 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/legacy/rules/models/_base.py
--rw-r--r--   0        0        0    12382 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/legacy/rules/models/raw_rules.py
--rw-r--r--   0        0        0     7351 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/legacy/rules/models/rdfpath.py
--rw-r--r--   0        0        0    51091 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/legacy/rules/models/rules.py
--rw-r--r--   0        0        0      171 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/legacy/rules/models/tables.py
--rw-r--r--   0        0        0     4402 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/legacy/rules/models/value_types.py
--rw-r--r--   0        0        0     1898 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/legacy/workflows/examples/Export_DMS/workflow.yaml
--rw-r--r--   0        0        0     3604 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/legacy/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
--rw-r--r--   0        0        0     3384 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/legacy/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
--rw-r--r--   0        0        0     6205 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/legacy/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
--rw-r--r--   0        0        0     1364 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/legacy/workflows/examples/Import_DMS/workflow.yaml
--rw-r--r--   0        0        0     2722 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/legacy/workflows/examples/Ontology_to_Data_Model/workflow.yaml
--rw-r--r--   0        0        0     1395 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/legacy/workflows/examples/Validate_Rules/workflow.yaml
--rw-r--r--   0        0        0     1326 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/legacy/workflows/examples/Validate_Solution_Model/workflow.yaml
--rw-r--r--   0        0        0     2296 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/legacy/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
--rw-r--r--   0        0        0     2579 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/legacy/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
--rw-r--r--   0        0        0        0 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/py.typed
--rw-r--r--   0        0        0        0 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/rules/__init__.py
--rw-r--r--   0        0        0      170 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/rules/_shared.py
--rw-r--r--   0        0        0      115 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/rules/analysis/__init__.py
--rw-r--r--   0        0        0      669 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/rules/analysis/_base.py
--rw-r--r--   0        0        0    19179 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/rules/analysis/_information_rules.py
--rw-r--r--   0        0        0      374 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/rules/examples/__init__.py
--rw-r--r--   0        0        0    65934 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/rules/examples/wind-energy.owl
--rw-r--r--   0        0        0   123868 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/rules/exceptions.py
--rw-r--r--   0        0        0      413 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/rules/exporters/__init__.py
--rw-r--r--   0        0        0     1511 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/rules/exporters/_base.py
--rw-r--r--   0        0        0     1976 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/rules/exporters/_models.py
--rw-r--r--   0        0        0    13688 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/rules/exporters/_rules2dms.py
--rw-r--r--   0        0        0    14248 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/rules/exporters/_rules2excel.py
--rw-r--r--   0        0        0    20120 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/rules/exporters/_rules2ontology.py
--rw-r--r--   0        0        0     3026 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/rules/exporters/_rules2yaml.py
--rw-r--r--   0        0        0     4078 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/rules/exporters/_validation.py
--rw-r--r--   0        0        0      481 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/rules/importers/__init__.py
--rw-r--r--   0        0        0     4274 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/rules/importers/_base.py
--rw-r--r--   0        0        0    18994 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/rules/importers/_dms2rules.py
--rw-r--r--   0        0        0       68 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/rules/importers/_dtdl2rules/__init__.py
--rw-r--r--   0        0        0    12134 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
--rw-r--r--   0        0        0    12663 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
--rw-r--r--   0        0        0     6718 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
--rw-r--r--   0        0        0    11897 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/rules/importers/_dtdl2rules/spec.py
--rw-r--r--   0        0        0    11187 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/rules/importers/_inference2rules.py
--rw-r--r--   0        0        0       63 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/rules/importers/_owl2rules/__init__.py
--rw-r--r--   0        0        0     7357 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     7527 2024-05-31 12:10:13.231062 cognite_neat-0.78.2/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     7297 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0     6358 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0    12438 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/importers/_spreadsheet2rules.py
--rw-r--r--   0        0        0     4275 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/importers/_yaml2rules.py
--rw-r--r--   0        0        0      563 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/issues/__init__.py
--rw-r--r--   0        0        0     6438 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/issues/base.py
--rw-r--r--   0        0        0    23617 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/issues/dms.py
--rw-r--r--   0        0        0     5748 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/issues/fileread.py
--rw-r--r--   0        0        0     3385 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/issues/formatters.py
--rw-r--r--   0        0        0    13417 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/issues/importing.py
--rw-r--r--   0        0        0    15825 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/issues/spreadsheet.py
--rw-r--r--   0        0        0     4964 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/issues/spreadsheet_file.py
--rw-r--r--   0        0        0      782 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/models/__init__.py
--rw-r--r--   0        0        0    11010 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/models/_base.py
--rw-r--r--   0        0        0    11030 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/models/_rdfpath.py
--rw-r--r--   0        0        0      305 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/models/_types/__init__.py
--rw-r--r--   0        0        0      929 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/models/_types/_base.py
--rw-r--r--   0        0        0     3203 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/models/_types/_field.py
--rw-r--r--   0        0        0     6078 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/models/data_types.py
--rw-r--r--   0        0        0      491 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/models/dms/__init__.py
--rw-r--r--   0        0        0     5959 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/models/dms/_converter.py
--rw-r--r--   0        0        0    24486 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/models/dms/_exporter.py
--rw-r--r--   0        0        0    16070 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/models/dms/_rules.py
--rw-r--r--   0        0        0    13467 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/models/dms/_rules_input.py
--rw-r--r--   0        0        0    43808 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/models/dms/_schema.py
--rw-r--r--   0        0        0     6406 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/models/dms/_serializer.py
--rw-r--r--   0        0        0    13937 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/models/dms/_validation.py
--rw-r--r--   0        0        0     2814 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/models/domain.py
--rw-r--r--   0        0        0    16898 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/models/entities.py
--rw-r--r--   0        0        0      291 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/models/information/__init__.py
--rw-r--r--   0        0        0    11029 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/models/information/_converter.py
--rw-r--r--   0        0        0    13268 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/models/information/_rules.py
--rw-r--r--   0        0        0    10147 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/models/information/_rules_input.py
--rw-r--r--   0        0        0     3503 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/models/information/_serializer.py
--rw-r--r--   0        0        0     7528 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/models/information/_validation.py
--rw-r--r--   0        0        0     7157 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/rules/models/wrapped_entities.py
--rw-r--r--   0        0        0       68 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/utils/__init__.py
--rw-r--r--   0        0        0      309 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/utils/auxiliary.py
--rw-r--r--   0        0        0     2422 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/utils/cdf.py
--rw-r--r--   0        0        0     5831 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/utils/cdf_classes.py
--rw-r--r--   0        0        0      483 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/utils/cdf_loaders/__init__.py
--rw-r--r--   0        0        0     2057 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/utils/cdf_loaders/_base.py
--rw-r--r--   0        0        0    11336 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/utils/cdf_loaders/_data_modeling.py
--rw-r--r--   0        0        0     6303 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/utils/cdf_loaders/_ingestion.py
--rw-r--r--   0        0        0     3844 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/utils/cdf_loaders/data_classes.py
--rw-r--r--   0        0        0      981 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/utils/exceptions.py
--rw-r--r--   0        0        0     2714 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/utils/spreadsheet.py
--rw-r--r--   0        0        0     3082 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/utils/text.py
--rw-r--r--   0        0        0    12919 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/utils/utils.py
--rw-r--r--   0        0        0      992 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/utils/xml.py
--rw-r--r--   0        0        0      396 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/workflows/__init__.py
--rw-r--r--   0        0        0     1348 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/workflows/_exceptions.py
--rw-r--r--   0        0        0    26800 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/workflows/base.py
--rw-r--r--   0        0        0    18016 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/workflows/cdf_store.py
--rw-r--r--   0        0        0     1987 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/workflows/examples/Export_DMS/workflow.yaml
--rw-r--r--   0        0        0     3604 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
--rw-r--r--   0        0        0     3384 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
--rw-r--r--   0        0        0     6205 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
--rw-r--r--   0        0        0     1364 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/workflows/examples/Import_DMS/workflow.yaml
--rw-r--r--   0        0        0     2722 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml
--rw-r--r--   0        0        0     1395 2024-05-31 12:10:13.235062 cognite_neat-0.78.2/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml
--rw-r--r--   0        0        0     1326 2024-05-31 12:10:13.239062 cognite_neat-0.78.2/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml
--rw-r--r--   0        0        0     2296 2024-05-31 12:10:13.239062 cognite_neat-0.78.2/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
--rw-r--r--   0        0        0     2579 2024-05-31 12:10:13.239062 cognite_neat-0.78.2/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
--rw-r--r--   0        0        0    14102 2024-05-31 12:10:13.239062 cognite_neat-0.78.2/cognite/neat/workflows/manager.py
--rw-r--r--   0        0        0        0 2024-05-31 12:10:13.239062 cognite_neat-0.78.2/cognite/neat/workflows/migration/__init__.py
--rw-r--r--   0        0        0     3992 2024-05-31 12:10:13.239062 cognite_neat-0.78.2/cognite/neat/workflows/migration/steps.py
--rw-r--r--   0        0        0     1556 2024-05-31 12:10:13.239062 cognite_neat-0.78.2/cognite/neat/workflows/migration/wf_manifests.py
--rw-r--r--   0        0        0     6570 2024-05-31 12:10:13.239062 cognite_neat-0.78.2/cognite/neat/workflows/model.py
--rw-r--r--   0        0        0        0 2024-05-31 12:10:13.239062 cognite_neat-0.78.2/cognite/neat/workflows/steps/__init__.py
--rw-r--r--   0        0        0     3009 2024-05-31 12:10:13.239062 cognite_neat-0.78.2/cognite/neat/workflows/steps/data_contracts.py
--rw-r--r--   0        0        0        0 2024-05-31 12:10:13.239062 cognite_neat-0.78.2/cognite/neat/workflows/steps/lib/__init__.py
--rw-r--r--   0        0        0      225 2024-05-31 12:10:13.239062 cognite_neat-0.78.2/cognite/neat/workflows/steps/lib/current/__init__.py
--rw-r--r--   0        0        0     5161 2024-05-31 12:10:13.239062 cognite_neat-0.78.2/cognite/neat/workflows/steps/lib/current/graph_extractor.py
--rw-r--r--   0        0        0     2341 2024-05-31 12:10:13.239062 cognite_neat-0.78.2/cognite/neat/workflows/steps/lib/current/graph_loader.py
--rw-r--r--   0        0        0     6295 2024-05-31 12:10:13.239062 cognite_neat-0.78.2/cognite/neat/workflows/steps/lib/current/graph_store.py
--rw-r--r--   0        0        0    23822 2024-05-31 12:10:13.239062 cognite_neat-0.78.2/cognite/neat/workflows/steps/lib/current/rules_exporter.py
--rw-r--r--   0        0        0    15190 2024-05-31 12:10:13.239062 cognite_neat-0.78.2/cognite/neat/workflows/steps/lib/current/rules_importer.py
--rw-r--r--   0        0        0     4844 2024-05-31 12:10:13.239062 cognite_neat-0.78.2/cognite/neat/workflows/steps/lib/current/rules_validator.py
--rw-r--r--   0        0        0       32 2024-05-31 12:10:13.239062 cognite_neat-0.78.2/cognite/neat/workflows/steps/lib/io/__init__.py
--rw-r--r--   0        0        0    16874 2024-05-31 12:10:13.239062 cognite_neat-0.78.2/cognite/neat/workflows/steps/lib/io/io_steps.py
--rw-r--r--   0        0        0      274 2024-05-31 12:10:13.239062 cognite_neat-0.78.2/cognite/neat/workflows/steps/lib/legacy/__init__.py
--rw-r--r--   0        0        0     3919 2024-05-31 12:10:13.239062 cognite_neat-0.78.2/cognite/neat/workflows/steps/lib/legacy/graph_contextualization.py
--rw-r--r--   0        0        0    29357 2024-05-31 12:10:13.239062 cognite_neat-0.78.2/cognite/neat/workflows/steps/lib/legacy/graph_extractor.py
--rw-r--r--   0        0        0    27265 2024-05-31 12:10:13.239062 cognite_neat-0.78.2/cognite/neat/workflows/steps/lib/legacy/graph_loader.py
--rw-r--r--   0        0        0    12704 2024-05-31 12:10:13.239062 cognite_neat-0.78.2/cognite/neat/workflows/steps/lib/legacy/graph_store.py
--rw-r--r--   0        0        0     2351 2024-05-31 12:10:13.239062 cognite_neat-0.78.2/cognite/neat/workflows/steps/lib/legacy/graph_transformer.py
--rw-r--r--   0        0        0    20462 2024-05-31 12:10:13.239062 cognite_neat-0.78.2/cognite/neat/workflows/steps/lib/legacy/rules_exporter.py
--rw-r--r--   0        0        0    28065 2024-05-31 12:10:13.239062 cognite_neat-0.78.2/cognite/neat/workflows/steps/lib/legacy/rules_importer.py
--rw-r--r--   0        0        0     2943 2024-05-31 12:10:13.239062 cognite_neat-0.78.2/cognite/neat/workflows/steps/step_model.py
--rw-r--r--   0        0        0    11007 2024-05-31 12:10:13.239062 cognite_neat-0.78.2/cognite/neat/workflows/steps_registry.py
--rw-r--r--   0        0        0      788 2024-05-31 12:10:13.239062 cognite_neat-0.78.2/cognite/neat/workflows/tasks.py
--rw-r--r--   0        0        0     7071 2024-05-31 12:10:13.239062 cognite_neat-0.78.2/cognite/neat/workflows/triggers.py
--rw-r--r--   0        0        0      453 2024-05-31 12:10:13.239062 cognite_neat-0.78.2/cognite/neat/workflows/utils.py
--rw-r--r--   0        0        0     4584 2024-05-31 12:10:13.627066 cognite_neat-0.78.2/pyproject.toml
--rw-r--r--   0        0        0     9306 1970-01-01 00:00:00.000000 cognite_neat-0.78.2/PKG-INFO
+-rw-r--r--   0        0        0    11351 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/LICENSE
+-rw-r--r--   0        0        0     6775 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/README.md
+-rw-r--r--   0        0        0       61 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/__init__.py
+-rw-r--r--   0        0        0       23 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/_version.py
+-rw-r--r--   0        0        0        0 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/api/__init__.py
+-rw-r--r--   0        0        0      152 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/api/asgi/metrics.py
+-rw-r--r--   0        0        0     4232 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/api/configuration.py
+-rw-r--r--   0        0        0       90 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/api/context_manager/__init__.py
+-rw-r--r--   0        0        0      380 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/api/context_manager/manager.py
+-rw-r--r--   0        0        0        0 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/api/data_classes/__init__.py
+-rw-r--r--   0        0        0     1675 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/api/data_classes/rest.py
+-rw-r--r--   0        0        0     1891 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/api/explorer.py
+-rw-r--r--   0        0        0      585 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/api/routers/configuration.py
+-rw-r--r--   0        0        0     3523 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/api/routers/core.py
+-rw-r--r--   0        0        0     4597 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/api/routers/crud.py
+-rw-r--r--   0        0        0    13686 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/api/routers/data_exploration.py
+-rw-r--r--   0        0        0      210 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/api/routers/metrics.py
+-rw-r--r--   0        0        0     8121 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/api/routers/rules.py
+-rw-r--r--   0        0        0    12393 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/api/routers/workflows.py
+-rw-r--r--   0        0        0        0 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/api/utils/__init__.py
+-rw-r--r--   0        0        0      564 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/api/utils/data_mapping.py
+-rw-r--r--   0        0        0      806 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/api/utils/logging.py
+-rw-r--r--   0        0        0     4594 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/api/utils/query_templates.py
+-rw-r--r--   0        0        0      357 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/main.py
+-rw-r--r--   0        0        0        0 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/monitoring/__init__.py
+-rw-r--r--   0        0        0     2690 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/monitoring/metrics.py
+-rw-r--r--   0        0        0       16 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/ui/index.html
+-rw-r--r--   0        0        0      312 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/ui/neat-app/.gitignore
+-rw-r--r--   0        0        0     3359 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/ui/neat-app/README.md
+-rw-r--r--   0        0        0      464 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/ui/neat-app/build/asset-manifest.json
+-rw-r--r--   0        0        0    15406 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/ui/neat-app/build/favicon.ico
+-rw-r--r--   0        0        0    10756 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg
+-rw-r--r--   0        0        0     8374 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg
+-rw-r--r--   0        0        0     5333 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg
+-rw-r--r--   0        0        0      629 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/ui/neat-app/build/index.html
+-rw-r--r--   0        0        0   344557 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/ui/neat-app/build/logo192.png
+-rw-r--r--   0        0        0      492 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/ui/neat-app/build/manifest.json
+-rw-r--r--   0        0        0       67 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/ui/neat-app/build/robots.txt
+-rw-r--r--   0        0        0     8524 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
+-rw-r--r--   0        0        0    13319 2024-06-03 13:18:42.649262 cognite_neat-0.78.3/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
+-rw-r--r--   0        0        0  1423717 2024-06-03 13:18:42.657262 cognite_neat-0.78.3/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js
+-rw-r--r--   0        0        0     2667 2024-06-03 13:18:42.657262 cognite_neat-0.78.3/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.LICENSE.txt
+-rw-r--r--   0        0        0  6282875 2024-06-03 13:18:42.681262 cognite_neat-0.78.3/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.map
+-rw-r--r--   0        0        0   240334 2024-06-03 13:18:42.681262 cognite_neat-0.78.3/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg
+-rw-r--r--   0        0        0     6145 2024-06-03 13:18:42.689262 cognite_neat-0.78.3/cognite/neat/config.py
+-rw-r--r--   0        0        0     1300 2024-06-03 13:18:42.689262 cognite_neat-0.78.3/cognite/neat/constants.py
+-rw-r--r--   0        0        0     4268 2024-06-03 13:18:42.689262 cognite_neat-0.78.3/cognite/neat/exceptions.py
+-rw-r--r--   0        0        0       73 2024-06-03 13:18:42.689262 cognite_neat-0.78.3/cognite/neat/graph/__init__.py
+-rw-r--r--   0        0        0  1439359 2024-06-03 13:18:42.693262 cognite_neat-0.78.3/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
+-rw-r--r--   0        0        0  1437996 2024-06-03 13:18:42.697262 cognite_neat-0.78.3/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0      368 2024-06-03 13:18:42.697262 cognite_neat-0.78.3/cognite/neat/graph/examples/__init__.py
+-rw-r--r--   0        0        0    45798 2024-06-03 13:18:42.697262 cognite_neat-0.78.3/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
+-rw-r--r--   0        0        0     3401 2024-06-03 13:18:42.697262 cognite_neat-0.78.3/cognite/neat/graph/exceptions.py
+-rw-r--r--   0        0        0        0 2024-06-03 13:18:42.697262 cognite_neat-0.78.3/cognite/neat/graph/extractors/__init__.py
+-rw-r--r--   0        0        0      356 2024-06-03 13:18:42.697262 cognite_neat-0.78.3/cognite/neat/graph/extractors/_base.py
+-rw-r--r--   0        0        0    14961 2024-06-03 13:18:42.697262 cognite_neat-0.78.3/cognite/neat/graph/extractors/_mock_graph_generator.py
+-rw-r--r--   0        0        0      149 2024-06-03 13:18:42.697262 cognite_neat-0.78.3/cognite/neat/graph/models.py
+-rw-r--r--   0        0        0      543 2024-06-03 13:18:42.697262 cognite_neat-0.78.3/cognite/neat/graph/stores/__init__.py
+-rw-r--r--   0        0        0    13473 2024-06-03 13:18:42.697262 cognite_neat-0.78.3/cognite/neat/graph/stores/_base.py
+-rw-r--r--   0        0        0     1776 2024-06-03 13:18:42.697262 cognite_neat-0.78.3/cognite/neat/graph/stores/_graphdb_store.py
+-rw-r--r--   0        0        0     1420 2024-06-03 13:18:42.697262 cognite_neat-0.78.3/cognite/neat/graph/stores/_memory_store.py
+-rw-r--r--   0        0        0     5448 2024-06-03 13:18:42.697262 cognite_neat-0.78.3/cognite/neat/graph/stores/_oxigraph_store.py
+-rw-r--r--   0        0        0     9569 2024-06-03 13:18:42.697262 cognite_neat-0.78.3/cognite/neat/graph/stores/_oxrdflib.py
+-rw-r--r--   0        0        0     1244 2024-06-03 13:18:42.697262 cognite_neat-0.78.3/cognite/neat/graph/stores/_rdf_to_graph.py
+-rw-r--r--   0        0        0        0 2024-06-03 13:18:42.697262 cognite_neat-0.78.3/cognite/neat/legacy/__init__.py
+-rw-r--r--   0        0        0       73 2024-06-03 13:18:42.697262 cognite_neat-0.78.3/cognite/neat/legacy/graph/__init__.py
+-rw-r--r--   0        0        0  1439359 2024-06-03 13:18:42.701262 cognite_neat-0.78.3/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
+-rw-r--r--   0        0        0  1437996 2024-06-03 13:18:42.701262 cognite_neat-0.78.3/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0      368 2024-06-03 13:18:42.701262 cognite_neat-0.78.3/cognite/neat/legacy/graph/examples/__init__.py
+-rw-r--r--   0        0        0    45798 2024-06-03 13:18:42.701262 cognite_neat-0.78.3/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx
+-rw-r--r--   0        0        0     3401 2024-06-03 13:18:42.701262 cognite_neat-0.78.3/cognite/neat/legacy/graph/exceptions.py
+-rw-r--r--   0        0        0      258 2024-06-03 13:18:42.701262 cognite_neat-0.78.3/cognite/neat/legacy/graph/extractors/__init__.py
+-rw-r--r--   0        0        0      363 2024-06-03 13:18:42.701262 cognite_neat-0.78.3/cognite/neat/legacy/graph/extractors/_base.py
+-rw-r--r--   0        0        0    11734 2024-06-03 13:18:42.701262 cognite_neat-0.78.3/cognite/neat/legacy/graph/extractors/_dexpi.py
+-rw-r--r--   0        0        0    17695 2024-06-03 13:18:42.701262 cognite_neat-0.78.3/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py
+-rw-r--r--   0        0        0    14908 2024-06-03 13:18:42.701262 cognite_neat-0.78.3/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py
+-rw-r--r--   0        0        0      701 2024-06-03 13:18:42.701262 cognite_neat-0.78.3/cognite/neat/legacy/graph/loaders/__init__.py
+-rw-r--r--   0        0        0    23823 2024-06-03 13:18:42.701262 cognite_neat-0.78.3/cognite/neat/legacy/graph/loaders/_asset_loader.py
+-rw-r--r--   0        0        0     2383 2024-06-03 13:18:42.701262 cognite_neat-0.78.3/cognite/neat/legacy/graph/loaders/_base.py
+-rw-r--r--   0        0        0     2835 2024-06-03 13:18:42.701262 cognite_neat-0.78.3/cognite/neat/legacy/graph/loaders/_exceptions.py
+-rw-r--r--   0        0        0        0 2024-06-03 13:18:42.701262 cognite_neat-0.78.3/cognite/neat/legacy/graph/loaders/core/__init__.py
+-rw-r--r--   0        0        0     2321 2024-06-03 13:18:42.701262 cognite_neat-0.78.3/cognite/neat/legacy/graph/loaders/core/labels.py
+-rw-r--r--   0        0        0     5023 2024-06-03 13:18:42.701262 cognite_neat-0.78.3/cognite/neat/legacy/graph/loaders/core/models.py
+-rw-r--r--   0        0        0    40464 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py
+-rw-r--r--   0        0        0    22707 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py
+-rw-r--r--   0        0        0    12979 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/graph/loaders/rdf_to_dms.py
+-rw-r--r--   0        0        0     3328 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/graph/loaders/validator.py
+-rw-r--r--   0        0        0      149 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/graph/models.py
+-rw-r--r--   0        0        0      543 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/graph/stores/__init__.py
+-rw-r--r--   0        0        0    14289 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/graph/stores/_base.py
+-rw-r--r--   0        0        0     1776 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/graph/stores/_graphdb_store.py
+-rw-r--r--   0        0        0     1420 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/graph/stores/_memory_store.py
+-rw-r--r--   0        0        0     5448 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/graph/stores/_oxigraph_store.py
+-rw-r--r--   0        0        0     9569 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/graph/stores/_oxrdflib.py
+-rw-r--r--   0        0        0     1244 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/graph/stores/_rdf_to_graph.py
+-rw-r--r--   0        0        0        0 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/graph/transformations/__init__.py
+-rw-r--r--   0        0        0     4765 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/graph/transformations/entity_matcher.py
+-rw-r--r--   0        0        0       73 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/graph/transformations/query_generator/__init__.py
+-rw-r--r--   0        0        0    18719 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/graph/transformations/query_generator/sparql.py
+-rw-r--r--   0        0        0    14737 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/graph/transformations/transformer.py
+-rw-r--r--   0        0        0        0 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/rules/__init__.py
+-rw-r--r--   0        0        0     8610 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/rules/analysis.py
+-rw-r--r--   0        0        0    58987 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx
+-rw-r--r--   0        0        0    80226 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx
+-rw-r--r--   0        0        0      858 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/rules/examples/__init__.py
+-rw-r--r--   0        0        0     2598 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/rules/examples/power-grid-containers.yaml
+-rw-r--r--   0        0        0    77055 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/rules/examples/power-grid-example.xlsx
+-rw-r--r--   0        0        0     5567 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/rules/examples/power-grid-model.yaml
+-rw-r--r--   0        0        0    75865 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/rules/examples/rules-template.xlsx
+-rw-r--r--   0        0        0    52433 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx
+-rw-r--r--   0        0        0    26008 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/rules/examples/skos-rules.xlsx
+-rw-r--r--   0        0        0    79981 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx
+-rw-r--r--   0        0        0    65934 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/rules/examples/wind-energy.owl
+-rw-r--r--   0        0        0   123868 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/rules/exceptions.py
+-rw-r--r--   0        0        0      574 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/rules/exporters/__init__.py
+-rw-r--r--   0        0        0     1453 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/rules/exporters/_base.py
+-rw-r--r--   0        0        0      102 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/rules/exporters/_core/__init__.py
+-rw-r--r--   0        0        0      771 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/rules/exporters/_core/rules2labels.py
+-rw-r--r--   0        0        0    36813 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/rules/exporters/_rules2dms.py
+-rw-r--r--   0        0        0     8312 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/rules/exporters/_rules2excel.py
+-rw-r--r--   0        0        0     6251 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/rules/exporters/_rules2graphql.py
+-rw-r--r--   0        0        0    18458 2024-06-03 13:18:42.705262 cognite_neat-0.78.3/cognite/neat/legacy/rules/exporters/_rules2ontology.py
+-rw-r--r--   0        0        0    28805 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py
+-rw-r--r--   0        0        0     3881 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/legacy/rules/exporters/_rules2rules.py
+-rw-r--r--   0        0        0     1085 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/legacy/rules/exporters/_rules2triples.py
+-rw-r--r--   0        0        0     5767 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/legacy/rules/exporters/_validation.py
+-rw-r--r--   0        0        0      636 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/legacy/rules/importers/__init__.py
+-rw-r--r--   0        0        0     2273 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/legacy/rules/importers/_base.py
+-rw-r--r--   0        0        0     6476 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/legacy/rules/importers/_dict2rules.py
+-rw-r--r--   0        0        0     7697 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/legacy/rules/importers/_dms2rules.py
+-rw-r--r--   0        0        0    12093 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/legacy/rules/importers/_graph2rules.py
+-rw-r--r--   0        0        0     1610 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/legacy/rules/importers/_json2rules.py
+-rw-r--r--   0        0        0       63 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/legacy/rules/importers/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     8304 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     9407 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     8019 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0    10557 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0     1502 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py
+-rw-r--r--   0        0        0      421 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/legacy/rules/importers/_xsd2rules.py
+-rw-r--r--   0        0        0     1601 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/legacy/rules/importers/_yaml2rules.py
+-rw-r--r--   0        0        0      127 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/legacy/rules/models/__init__.py
+-rw-r--r--   0        0        0     4989 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/legacy/rules/models/_base.py
+-rw-r--r--   0        0        0    12382 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/legacy/rules/models/raw_rules.py
+-rw-r--r--   0        0        0     7351 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/legacy/rules/models/rdfpath.py
+-rw-r--r--   0        0        0    51091 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/legacy/rules/models/rules.py
+-rw-r--r--   0        0        0      171 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/legacy/rules/models/tables.py
+-rw-r--r--   0        0        0     4402 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/legacy/rules/models/value_types.py
+-rw-r--r--   0        0        0     1898 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/legacy/workflows/examples/Export_DMS/workflow.yaml
+-rw-r--r--   0        0        0     3604 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/legacy/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
+-rw-r--r--   0        0        0     3384 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/legacy/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
+-rw-r--r--   0        0        0     6205 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/legacy/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
+-rw-r--r--   0        0        0     1364 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/legacy/workflows/examples/Import_DMS/workflow.yaml
+-rw-r--r--   0        0        0     2722 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/legacy/workflows/examples/Ontology_to_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0     1395 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/legacy/workflows/examples/Validate_Rules/workflow.yaml
+-rw-r--r--   0        0        0     1326 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/legacy/workflows/examples/Validate_Solution_Model/workflow.yaml
+-rw-r--r--   0        0        0     2296 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/legacy/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
+-rw-r--r--   0        0        0     2579 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/legacy/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0        0 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/py.typed
+-rw-r--r--   0        0        0        0 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/rules/__init__.py
+-rw-r--r--   0        0        0      170 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/rules/_shared.py
+-rw-r--r--   0        0        0      115 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/rules/analysis/__init__.py
+-rw-r--r--   0        0        0      669 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/rules/analysis/_base.py
+-rw-r--r--   0        0        0    19179 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/rules/analysis/_information_rules.py
+-rw-r--r--   0        0        0      374 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/rules/examples/__init__.py
+-rw-r--r--   0        0        0    65934 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/rules/examples/wind-energy.owl
+-rw-r--r--   0        0        0   123868 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/rules/exceptions.py
+-rw-r--r--   0        0        0      413 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/rules/exporters/__init__.py
+-rw-r--r--   0        0        0     1511 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/rules/exporters/_base.py
+-rw-r--r--   0        0        0     1976 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/rules/exporters/_models.py
+-rw-r--r--   0        0        0    13688 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/rules/exporters/_rules2dms.py
+-rw-r--r--   0        0        0    14248 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/rules/exporters/_rules2excel.py
+-rw-r--r--   0        0        0    20388 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/rules/exporters/_rules2ontology.py
+-rw-r--r--   0        0        0     3026 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/rules/exporters/_rules2yaml.py
+-rw-r--r--   0        0        0     4078 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/rules/exporters/_validation.py
+-rw-r--r--   0        0        0      481 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/rules/importers/__init__.py
+-rw-r--r--   0        0        0     4274 2024-06-03 13:18:42.709262 cognite_neat-0.78.3/cognite/neat/rules/importers/_base.py
+-rw-r--r--   0        0        0    18994 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/importers/_dms2rules.py
+-rw-r--r--   0        0        0       68 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/importers/_dtdl2rules/__init__.py
+-rw-r--r--   0        0        0    12134 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
+-rw-r--r--   0        0        0    12663 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
+-rw-r--r--   0        0        0     6718 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
+-rw-r--r--   0        0        0    11897 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/importers/_dtdl2rules/spec.py
+-rw-r--r--   0        0        0    11213 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/importers/_inference2rules.py
+-rw-r--r--   0        0        0       63 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/importers/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     7357 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     7527 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     7297 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0     6358 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0    12438 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/importers/_spreadsheet2rules.py
+-rw-r--r--   0        0        0     4275 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/importers/_yaml2rules.py
+-rw-r--r--   0        0        0      563 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/issues/__init__.py
+-rw-r--r--   0        0        0     6438 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/issues/base.py
+-rw-r--r--   0        0        0    23617 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/issues/dms.py
+-rw-r--r--   0        0        0     5748 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/issues/fileread.py
+-rw-r--r--   0        0        0     3385 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/issues/formatters.py
+-rw-r--r--   0        0        0    13417 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/issues/importing.py
+-rw-r--r--   0        0        0    15825 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/issues/spreadsheet.py
+-rw-r--r--   0        0        0     4964 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/issues/spreadsheet_file.py
+-rw-r--r--   0        0        0      782 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/models/__init__.py
+-rw-r--r--   0        0        0    11010 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/models/_base.py
+-rw-r--r--   0        0        0    11030 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/models/_rdfpath.py
+-rw-r--r--   0        0        0      305 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/models/_types/__init__.py
+-rw-r--r--   0        0        0      929 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/models/_types/_base.py
+-rw-r--r--   0        0        0     3203 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/models/_types/_field.py
+-rw-r--r--   0        0        0     6078 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/models/data_types.py
+-rw-r--r--   0        0        0      491 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/models/dms/__init__.py
+-rw-r--r--   0        0        0     5959 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/models/dms/_converter.py
+-rw-r--r--   0        0        0    24486 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/models/dms/_exporter.py
+-rw-r--r--   0        0        0    16070 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/models/dms/_rules.py
+-rw-r--r--   0        0        0    13467 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/models/dms/_rules_input.py
+-rw-r--r--   0        0        0    43808 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/models/dms/_schema.py
+-rw-r--r--   0        0        0     6406 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/models/dms/_serializer.py
+-rw-r--r--   0        0        0    13937 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/models/dms/_validation.py
+-rw-r--r--   0        0        0     2814 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/models/domain.py
+-rw-r--r--   0        0        0    18868 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/models/entities.py
+-rw-r--r--   0        0        0      291 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/models/information/__init__.py
+-rw-r--r--   0        0        0    11029 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/models/information/_converter.py
+-rw-r--r--   0        0        0    13476 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/models/information/_rules.py
+-rw-r--r--   0        0        0    10418 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/models/information/_rules_input.py
+-rw-r--r--   0        0        0     3503 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/models/information/_serializer.py
+-rw-r--r--   0        0        0     7528 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/models/information/_validation.py
+-rw-r--r--   0        0        0     7157 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/rules/models/wrapped_entities.py
+-rw-r--r--   0        0        0       68 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/utils/__init__.py
+-rw-r--r--   0        0        0      309 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/utils/auxiliary.py
+-rw-r--r--   0        0        0     2422 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/utils/cdf.py
+-rw-r--r--   0        0        0     5831 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/utils/cdf_classes.py
+-rw-r--r--   0        0        0      483 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/utils/cdf_loaders/__init__.py
+-rw-r--r--   0        0        0     2057 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/utils/cdf_loaders/_base.py
+-rw-r--r--   0        0        0    11336 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/utils/cdf_loaders/_data_modeling.py
+-rw-r--r--   0        0        0     6303 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/utils/cdf_loaders/_ingestion.py
+-rw-r--r--   0        0        0     3844 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/utils/cdf_loaders/data_classes.py
+-rw-r--r--   0        0        0      981 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/utils/exceptions.py
+-rw-r--r--   0        0        0     2714 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/utils/spreadsheet.py
+-rw-r--r--   0        0        0     3082 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/utils/text.py
+-rw-r--r--   0        0        0    12919 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/utils/utils.py
+-rw-r--r--   0        0        0      992 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/utils/xml.py
+-rw-r--r--   0        0        0      396 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/workflows/__init__.py
+-rw-r--r--   0        0        0     1348 2024-06-03 13:18:42.713262 cognite_neat-0.78.3/cognite/neat/workflows/_exceptions.py
+-rw-r--r--   0        0        0    26800 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/base.py
+-rw-r--r--   0        0        0    18016 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/cdf_store.py
+-rw-r--r--   0        0        0     1987 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/examples/Export_DMS/workflow.yaml
+-rw-r--r--   0        0        0     3604 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
+-rw-r--r--   0        0        0     3384 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
+-rw-r--r--   0        0        0     6205 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
+-rw-r--r--   0        0        0     1364 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/examples/Import_DMS/workflow.yaml
+-rw-r--r--   0        0        0     2722 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0     1395 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml
+-rw-r--r--   0        0        0     1326 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml
+-rw-r--r--   0        0        0     2296 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
+-rw-r--r--   0        0        0     2579 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0    14102 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/manager.py
+-rw-r--r--   0        0        0        0 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/migration/__init__.py
+-rw-r--r--   0        0        0     3992 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/migration/steps.py
+-rw-r--r--   0        0        0     1556 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/migration/wf_manifests.py
+-rw-r--r--   0        0        0     6570 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/model.py
+-rw-r--r--   0        0        0        0 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/steps/__init__.py
+-rw-r--r--   0        0        0     3009 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/steps/data_contracts.py
+-rw-r--r--   0        0        0        0 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/steps/lib/__init__.py
+-rw-r--r--   0        0        0      225 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/steps/lib/current/__init__.py
+-rw-r--r--   0        0        0     5161 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/steps/lib/current/graph_extractor.py
+-rw-r--r--   0        0        0     2341 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/steps/lib/current/graph_loader.py
+-rw-r--r--   0        0        0     6295 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/steps/lib/current/graph_store.py
+-rw-r--r--   0        0        0    23822 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/steps/lib/current/rules_exporter.py
+-rw-r--r--   0        0        0    14697 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/steps/lib/current/rules_importer.py
+-rw-r--r--   0        0        0     4844 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/steps/lib/current/rules_validator.py
+-rw-r--r--   0        0        0       32 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/steps/lib/io/__init__.py
+-rw-r--r--   0        0        0    16874 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/steps/lib/io/io_steps.py
+-rw-r--r--   0        0        0      274 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/steps/lib/legacy/__init__.py
+-rw-r--r--   0        0        0     3919 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/steps/lib/legacy/graph_contextualization.py
+-rw-r--r--   0        0        0    29357 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/steps/lib/legacy/graph_extractor.py
+-rw-r--r--   0        0        0    27265 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/steps/lib/legacy/graph_loader.py
+-rw-r--r--   0        0        0    12704 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/steps/lib/legacy/graph_store.py
+-rw-r--r--   0        0        0     2351 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/steps/lib/legacy/graph_transformer.py
+-rw-r--r--   0        0        0    20462 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/steps/lib/legacy/rules_exporter.py
+-rw-r--r--   0        0        0    28065 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/steps/lib/legacy/rules_importer.py
+-rw-r--r--   0        0        0     2943 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/steps/step_model.py
+-rw-r--r--   0        0        0    11007 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/steps_registry.py
+-rw-r--r--   0        0        0      788 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/tasks.py
+-rw-r--r--   0        0        0     7071 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/triggers.py
+-rw-r--r--   0        0        0      453 2024-06-03 13:18:42.717262 cognite_neat-0.78.3/cognite/neat/workflows/utils.py
+-rw-r--r--   0        0        0     4584 2024-06-03 13:18:43.109267 cognite_neat-0.78.3/pyproject.toml
+-rw-r--r--   0        0        0     9306 1970-01-01 00:00:00.000000 cognite_neat-0.78.3/PKG-INFO
```

### Comparing `cognite_neat-0.78.2/LICENSE` & `cognite_neat-0.78.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/README.md` & `cognite_neat-0.78.3/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/app/api/configuration.py` & `cognite_neat-0.78.3/cognite/neat/app/api/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/app/api/data_classes/rest.py` & `cognite_neat-0.78.3/cognite/neat/app/api/data_classes/rest.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/app/api/explorer.py` & `cognite_neat-0.78.3/cognite/neat/app/api/explorer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/app/api/routers/configuration.py` & `cognite_neat-0.78.3/cognite/neat/app/api/routers/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/app/api/routers/core.py` & `cognite_neat-0.78.3/cognite/neat/app/api/routers/core.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/app/api/routers/crud.py` & `cognite_neat-0.78.3/cognite/neat/app/api/routers/crud.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/app/api/routers/data_exploration.py` & `cognite_neat-0.78.3/cognite/neat/app/api/routers/data_exploration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/app/api/routers/rules.py` & `cognite_neat-0.78.3/cognite/neat/app/api/routers/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/app/api/routers/workflows.py` & `cognite_neat-0.78.3/cognite/neat/app/api/routers/workflows.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/app/api/utils/data_mapping.py` & `cognite_neat-0.78.3/cognite/neat/app/api/utils/data_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/app/api/utils/logging.py` & `cognite_neat-0.78.3/cognite/neat/app/api/utils/logging.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/app/api/utils/query_templates.py` & `cognite_neat-0.78.3/cognite/neat/app/api/utils/query_templates.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/app/monitoring/metrics.py` & `cognite_neat-0.78.3/cognite/neat/app/monitoring/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/app/ui/neat-app/README.md` & `cognite_neat-0.78.3/cognite/neat/app/ui/neat-app/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/app/ui/neat-app/build/favicon.ico` & `cognite_neat-0.78.3/cognite/neat/app/ui/neat-app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg` & `cognite_neat-0.78.3/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg` & `cognite_neat-0.78.3/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg` & `cognite_neat-0.78.3/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/app/ui/neat-app/build/index.html` & `cognite_neat-0.78.3/cognite/neat/app/ui/neat-app/build/index.html`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/app/ui/neat-app/build/logo192.png` & `cognite_neat-0.78.3/cognite/neat/app/ui/neat-app/build/logo192.png`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css` & `cognite_neat-0.78.3/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map` & `cognite_neat-0.78.3/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js` & `cognite_neat-0.78.3/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.LICENSE.txt` & `cognite_neat-0.78.3/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.map` & `cognite_neat-0.78.3/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg` & `cognite_neat-0.78.3/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/config.py` & `cognite_neat-0.78.3/cognite/neat/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/constants.py` & `cognite_neat-0.78.3/cognite/neat/constants.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/exceptions.py` & `cognite_neat-0.78.3/cognite/neat/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml` & `cognite_neat-0.78.3/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.78.3/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx` & `cognite_neat-0.78.3/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/graph/exceptions.py` & `cognite_neat-0.78.3/cognite/neat/graph/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/graph/extractors/_mock_graph_generator.py` & `cognite_neat-0.78.3/cognite/neat/graph/extractors/_mock_graph_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/graph/stores/__init__.py` & `cognite_neat-0.78.3/cognite/neat/graph/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/graph/stores/_base.py` & `cognite_neat-0.78.3/cognite/neat/graph/stores/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/graph/stores/_graphdb_store.py` & `cognite_neat-0.78.3/cognite/neat/graph/stores/_graphdb_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/graph/stores/_memory_store.py` & `cognite_neat-0.78.3/cognite/neat/graph/stores/_memory_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/graph/stores/_oxigraph_store.py` & `cognite_neat-0.78.3/cognite/neat/graph/stores/_oxigraph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/graph/stores/_oxrdflib.py` & `cognite_neat-0.78.3/cognite/neat/graph/stores/_oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/graph/stores/_rdf_to_graph.py` & `cognite_neat-0.78.3/cognite/neat/graph/stores/_rdf_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml` & `cognite_neat-0.78.3/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.78.3/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx` & `cognite_neat-0.78.3/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/graph/exceptions.py` & `cognite_neat-0.78.3/cognite/neat/legacy/graph/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/graph/extractors/_dexpi.py` & `cognite_neat-0.78.3/cognite/neat/legacy/graph/extractors/_dexpi.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py` & `cognite_neat-0.78.3/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py` & `cognite_neat-0.78.3/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/graph/loaders/__init__.py` & `cognite_neat-0.78.3/cognite/neat/legacy/graph/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/graph/loaders/_asset_loader.py` & `cognite_neat-0.78.3/cognite/neat/legacy/graph/loaders/_asset_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/graph/loaders/_base.py` & `cognite_neat-0.78.3/cognite/neat/legacy/graph/loaders/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/graph/loaders/_exceptions.py` & `cognite_neat-0.78.3/cognite/neat/legacy/graph/loaders/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/graph/loaders/core/labels.py` & `cognite_neat-0.78.3/cognite/neat/legacy/graph/loaders/core/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/graph/loaders/core/models.py` & `cognite_neat-0.78.3/cognite/neat/legacy/graph/loaders/core/models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py` & `cognite_neat-0.78.3/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py` & `cognite_neat-0.78.3/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/graph/loaders/rdf_to_dms.py` & `cognite_neat-0.78.3/cognite/neat/legacy/graph/loaders/rdf_to_dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/graph/loaders/validator.py` & `cognite_neat-0.78.3/cognite/neat/legacy/graph/loaders/validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/graph/stores/__init__.py` & `cognite_neat-0.78.3/cognite/neat/legacy/graph/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/graph/stores/_base.py` & `cognite_neat-0.78.3/cognite/neat/legacy/graph/stores/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/graph/stores/_graphdb_store.py` & `cognite_neat-0.78.3/cognite/neat/legacy/graph/stores/_graphdb_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/graph/stores/_memory_store.py` & `cognite_neat-0.78.3/cognite/neat/legacy/graph/stores/_memory_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/graph/stores/_oxigraph_store.py` & `cognite_neat-0.78.3/cognite/neat/legacy/graph/stores/_oxigraph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/graph/stores/_oxrdflib.py` & `cognite_neat-0.78.3/cognite/neat/legacy/graph/stores/_oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/graph/stores/_rdf_to_graph.py` & `cognite_neat-0.78.3/cognite/neat/legacy/graph/stores/_rdf_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/graph/transformations/entity_matcher.py` & `cognite_neat-0.78.3/cognite/neat/legacy/graph/transformations/entity_matcher.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/graph/transformations/query_generator/sparql.py` & `cognite_neat-0.78.3/cognite/neat/legacy/graph/transformations/query_generator/sparql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/graph/transformations/transformer.py` & `cognite_neat-0.78.3/cognite/neat/legacy/graph/transformations/transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/analysis.py` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/analysis.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/examples/__init__.py` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/examples/power-grid-containers.yaml` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/examples/power-grid-containers.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/examples/power-grid-example.xlsx` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/examples/power-grid-example.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/examples/power-grid-model.yaml` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/examples/power-grid-model.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/examples/rules-template.xlsx` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/examples/rules-template.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/examples/skos-rules.xlsx` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/examples/skos-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/examples/wind-energy.owl` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/examples/wind-energy.owl`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/exceptions.py` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/exporters/__init__.py` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/exporters/_base.py` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/exporters/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/exporters/_core/rules2labels.py` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/exporters/_core/rules2labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/exporters/_rules2dms.py` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/exporters/_rules2dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/exporters/_rules2excel.py` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/exporters/_rules2excel.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/exporters/_rules2graphql.py` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/exporters/_rules2graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/exporters/_rules2ontology.py` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/exporters/_rules2ontology.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/exporters/_rules2rules.py` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/exporters/_rules2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/exporters/_rules2triples.py` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/exporters/_rules2triples.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/exporters/_validation.py` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/exporters/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/importers/__init__.py` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/importers/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/importers/_base.py` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/importers/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/importers/_dict2rules.py` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/importers/_dict2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/importers/_dms2rules.py` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/importers/_dms2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/importers/_graph2rules.py` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/importers/_graph2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/importers/_json2rules.py` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/importers/_json2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/importers/_yaml2rules.py` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/importers/_yaml2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/models/_base.py` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/models/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/models/raw_rules.py` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/models/raw_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/models/rdfpath.py` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/models/rdfpath.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/models/rules.py` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/models/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/rules/models/value_types.py` & `cognite_neat-0.78.3/cognite/neat/legacy/rules/models/value_types.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/workflows/examples/Export_DMS/workflow.yaml` & `cognite_neat-0.78.3/cognite/neat/legacy/workflows/examples/Export_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/workflows/examples/Export_Rules_to_Ontology/workflow.yaml` & `cognite_neat-0.78.3/cognite/neat/legacy/workflows/examples/Export_Rules_to_Ontology/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml` & `cognite_neat-0.78.3/cognite/neat/legacy/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml` & `cognite_neat-0.78.3/cognite/neat/legacy/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/workflows/examples/Import_DMS/workflow.yaml` & `cognite_neat-0.78.3/cognite/neat/legacy/workflows/examples/Import_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/workflows/examples/Ontology_to_Data_Model/workflow.yaml` & `cognite_neat-0.78.3/cognite/neat/legacy/workflows/examples/Ontology_to_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/workflows/examples/Validate_Rules/workflow.yaml` & `cognite_neat-0.78.3/cognite/neat/legacy/workflows/examples/Validate_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/workflows/examples/Validate_Solution_Model/workflow.yaml` & `cognite_neat-0.78.3/cognite/neat/legacy/workflows/examples/Validate_Solution_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml` & `cognite_neat-0.78.3/cognite/neat/legacy/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/legacy/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml` & `cognite_neat-0.78.3/cognite/neat/legacy/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/analysis/_base.py` & `cognite_neat-0.78.3/cognite/neat/rules/analysis/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/analysis/_information_rules.py` & `cognite_neat-0.78.3/cognite/neat/rules/analysis/_information_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/examples/wind-energy.owl` & `cognite_neat-0.78.3/cognite/neat/rules/examples/wind-energy.owl`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/exceptions.py` & `cognite_neat-0.78.3/cognite/neat/rules/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/exporters/_base.py` & `cognite_neat-0.78.3/cognite/neat/rules/exporters/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/exporters/_models.py` & `cognite_neat-0.78.3/cognite/neat/rules/exporters/_models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/exporters/_rules2dms.py` & `cognite_neat-0.78.3/cognite/neat/rules/exporters/_rules2dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/exporters/_rules2excel.py` & `cognite_neat-0.78.3/cognite/neat/rules/exporters/_rules2excel.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/exporters/_rules2ontology.py` & `cognite_neat-0.78.3/cognite/neat/rules/exporters/_rules2ontology.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,15 +327,15 @@
             owl_property.type_.add(OWL[definition.type_])
 
             if isinstance(definition.value_type, DataType):
                 owl_property.range_.add(XSD[definition.value_type.xsd])
             elif isinstance(definition.value_type, ClassEntity):
                 owl_property.range_.add(namespace[str(definition.value_type.suffix)])
             else:
-                raise ValueError(f"Value type {definition.value_type} is not supported")
+                raise ValueError(f"Value type {definition.value_type.type_} is not supported")
             owl_property.domain.add(namespace[str(definition.class_.suffix)])
             owl_property.label.add(definition.name or definition.property_)
             if definition.description:
                 owl_property.comment.add(definition.description)
 
         return owl_property
 
@@ -545,22 +545,26 @@
 
     @property
     def triples(self) -> list[tuple]:
         return self.path_triples + self.node_kind_triples + self.cardinality_triples
 
     @classmethod
     def from_property(cls, definition: InformationProperty, namespace: Namespace) -> "SHACLPropertyShape":
+        # TODO requires PR to fix MultiValueType and UnknownValueType
+        if isinstance(definition.value_type, ClassEntity):
+            expected_value_type = namespace[f"{definition.value_type.suffix}Shape"]
+        elif isinstance(definition.value_type, DataType):
+            expected_value_type = XSD[definition.value_type.xsd]
+        else:
+            raise ValueError(f"Value type {definition.value_type.type_} is not supported")
+
         return cls(
             id_=BNode(),
             path=namespace[definition.property_],
             node_kind=SHACL.IRI if definition.type_ == EntityTypes.object_property else SHACL.Literal,
-            expected_value_type=(
-                namespace[f"{definition.value_type.suffix}Shape"]
-                if isinstance(definition.value_type, ClassEntity)
-                else XSD[definition.value_type.xsd]
-            ),
+            expected_value_type=expected_value_type,
             min_count=definition.min_count,
             max_count=(
                 int(definition.max_count) if definition.max_count and definition.max_count != float("inf") else None
             ),
             namespace=namespace,
         )
```

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/exporters/_rules2yaml.py` & `cognite_neat-0.78.3/cognite/neat/rules/exporters/_rules2yaml.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/exporters/_validation.py` & `cognite_neat-0.78.3/cognite/neat/rules/exporters/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/importers/_base.py` & `cognite_neat-0.78.3/cognite/neat/rules/importers/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/importers/_dms2rules.py` & `cognite_neat-0.78.3/cognite/neat/rules/importers/_dms2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py` & `cognite_neat-0.78.3/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py` & `cognite_neat-0.78.3/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py` & `cognite_neat-0.78.3/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/importers/_dtdl2rules/spec.py` & `cognite_neat-0.78.3/cognite/neat/rules/importers/_dtdl2rules/spec.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/importers/_inference2rules.py` & `cognite_neat-0.78.3/cognite/neat/rules/importers/_inference2rules.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,27 @@
+import re
 from datetime import datetime
 from pathlib import Path
 from typing import Literal, cast, overload
 
 from rdflib import Graph, Namespace, URIRef
 from rdflib import Literal as RdfLiteral
 
 import cognite.neat.rules.issues as issues
 from cognite.neat.constants import PREFIXES
 from cognite.neat.graph.stores import NeatGraphStoreBase
 from cognite.neat.rules.importers._base import BaseImporter, Rules, _handle_issues
 from cognite.neat.rules.issues import IssueList
 from cognite.neat.rules.models import InformationRules, RoleTypes
 from cognite.neat.rules.models._base import MatchType
-from cognite.neat.rules.models.entities import ClassEntity
 from cognite.neat.rules.models.information import (
     InformationMetadata,
     InformationRulesInput,
 )
-from cognite.neat.utils.utils import get_namespace, remove_namespace, replace_non_alphanumeric_with_underscore
+from cognite.neat.utils.utils import get_namespace, remove_namespace
 
 ORDERED_CLASSES_QUERY = """SELECT ?class (count(?s) as ?instances )
                            WHERE { ?s a ?class . }
                            group by ?class order by DESC(?instances)"""
 
 INSTANCES_OF_CLASS_QUERY = """SELECT ?s WHERE { ?s a <class> . }"""
 
@@ -35,57 +35,49 @@
 class InferenceImporter(BaseImporter):
     """Rules inference through analysis of knowledge graph provided in various formats.
 
     Args:
         issue_list: Issue list to store issues
         graph: Knowledge graph
         max_number_of_instance: Maximum number of instances to be used in inference
-        make_compliant: If True, NEAT will attempt to make the imported rules compliant with CDF
     """
 
-    def __init__(
-        self, issue_list: IssueList, graph: Graph, make_compliant: bool = False, max_number_of_instance: int = -1
-    ):
+    def __init__(self, issue_list: IssueList, graph: Graph, max_number_of_instance: int = -1):
         self.issue_list = issue_list
         self.graph = graph
         self.max_number_of_instance = max_number_of_instance
-        self.make_compliant = make_compliant
 
     @classmethod
-    def from_graph_store(
-        cls, store: NeatGraphStoreBase, make_compliant: bool = False, max_number_of_instance: int = -1
-    ):
+    def from_graph_store(cls, store: NeatGraphStoreBase, max_number_of_instance: int = -1):
         issue_list = IssueList(title="Inferred from graph store")
 
-        return cls(
-            issue_list, store.graph, make_compliant=make_compliant, max_number_of_instance=max_number_of_instance
-        )
+        return cls(issue_list, store.graph, max_number_of_instance=max_number_of_instance)
 
     @classmethod
-    def from_rdf_file(cls, filepath: Path, make_compliant: bool = False, max_number_of_instance: int = -1):
+    def from_rdf_file(cls, filepath: Path, max_number_of_instance: int = -1):
         issue_list = IssueList(title=f"'{filepath.name}'")
 
         graph = Graph()
         try:
             graph.parse(filepath)
         except Exception:
             issue_list.append(issues.fileread.FileReadError(filepath))
 
-        return cls(issue_list, graph, make_compliant=make_compliant, max_number_of_instance=max_number_of_instance)
+        return cls(issue_list, graph, max_number_of_instance=max_number_of_instance)
 
     @classmethod
-    def from_json_file(cls, filepath: Path, make_compliant: bool = False, max_number_of_instance: int = -1):
+    def from_json_file(cls, filepath: Path, max_number_of_instance: int = -1):
         raise NotImplementedError("JSON file format is not supported yet.")
 
     @classmethod
-    def from_yaml_file(cls, filepath: Path, make_compliant: bool = False, max_number_of_instance: int = -1):
+    def from_yaml_file(cls, filepath: Path, max_number_of_instance: int = -1):
         raise NotImplementedError("YAML file format is not supported yet.")
 
     @classmethod
-    def from_xml_file(cls, filepath: Path, make_compliant: bool = False, max_number_of_instance: int = -1):
+    def from_xml_file(cls, filepath: Path, max_number_of_instance: int = -1):
         raise NotImplementedError("JSON file format is not supported yet.")
 
     @overload
     def to_rules(self, errors: Literal["raise"], role: RoleTypes | None = None) -> Rules: ...
 
     @overload
     def to_rules(
@@ -113,17 +105,14 @@
         with _handle_issues(self.issue_list) as future:
             rules: InformationRules
             rules = InformationRulesInput.load(rules_dict).as_rules()
 
         if future.result == "failure" or self.issue_list.has_errors:
             return self._return_or_raise(self.issue_list, errors)
 
-        if self.make_compliant and rules:
-            self._make_dms_compliant_rules(rules)
-
         return self._to_output(
             rules,
             self.issue_list,
             errors=errors,
             role=role,
         )
 
@@ -151,15 +140,15 @@
                 # handles cases when class id is already present in classes
                 class_id = f"{class_id}_{len(classes)+1}"
 
             classes[class_id] = {
                 "class_": class_id,
                 "reference": class_uri,
                 "match_type": MatchType.exact,
-                "comment": f"Inferred from knowledge graph, where this class has {no_instances} instances",
+                "comment": f"Inferred from knowledge graph, where this class has <{no_instances}> instances",
             }
 
         # Infers all the properties of the class
         for class_id, class_definition in classes.items():
             for (instance,) in self.graph.query(  # type: ignore[misc]
                 INSTANCES_OF_CLASS_QUERY.replace("class", class_definition["reference"])
                 if self.max_number_of_instance < 0
@@ -175,31 +164,57 @@
 
                     # this is to skip rdf:type property
                     if not value_type_uri:
                         continue
 
                     self._add_uri_namespace_to_prefixes(cast(URIRef, value_type_uri), prefixes)
                     value_type_id = remove_namespace(value_type_uri)
-                    id_ = f"{class_id}:{property_id}:{value_type_id}"
+                    id_ = f"{class_id}:{property_id}"
 
                     definition = {
                         "class_": class_id,
                         "property_": property_id,
                         "max_count": cast(RdfLiteral, occurrence).value,
                         "value_type": value_type_id,
                         "reference": property_uri,
+                        "comment": (
+                            f"Class <{class_id}> has property <{property_id}> with "
+                            f"value type <{value_type_id}> which occurs <1> times in the graph"
+                        ),
                     }
 
                     # USE CASE 1: If property is not present in properties
                     if id_ not in properties:
                         properties[id_] = definition
-                    # USE CASE 2: If property is present in properties but with different max count
-                    elif id_ in properties and not (properties[id_]["max_count"] == definition["max_count"]):
+
+                    # USE CASE 2: first time redefinition, value type change to multi
+                    elif id_ in properties and definition["value_type"] not in properties[id_]["value_type"]:
+                        properties[id_]["value_type"] = properties[id_]["value_type"] + " | " + definition["value_type"]
+                        properties[id_]["comment"] = (
+                            properties[id_]["comment"] + ", with" + definition["comment"].split("with")[1]
+                        )
+
+                    # USE CASE 3: existing but max count is different
+                    elif (
+                        id_ in properties
+                        and definition["value_type"] in properties[id_]["value_type"]
+                        and not (properties[id_]["max_count"] == definition["max_count"])
+                    ):
                         properties[id_]["max_count"] = max(properties[id_]["max_count"], definition["max_count"])
 
+                        properties[id_]["comment"] = self._update_value_type_occurrence_in_comment(
+                            definition["value_type"], properties[id_]["comment"]
+                        )
+
+                    # USE CASE 4: Just update the comment with occurrence
+                    else:
+                        properties[id_]["comment"] = self._update_value_type_occurrence_in_comment(
+                            definition["value_type"], properties[id_]["comment"]
+                        )
+
         return {
             "metadata": self._default_metadata().model_dump(),
             "classes": list(classes.values()),
             "properties": list(properties.values()),
             "prefixes": prefixes,
         }
 
@@ -224,40 +239,21 @@
             updated=datetime.now(),
             description="Inferred model from knowledge graph",
             prefix="inferred",
             namespace="http://purl.org/cognite/neat/inferred/",
         )
 
     @classmethod
-    def _make_dms_compliant_rules(cls, rules: InformationRules) -> None:
-        cls._fix_property_redefinition(rules)
-        cls._fix_naming_of_entities(rules)
-
-    @classmethod
-    def _fix_property_redefinition(cls, rules: InformationRules) -> None:
-        seen = set()
-        for i, property_ in enumerate(rules.properties.data):
-            prop_id = f"{property_.class_}.{property_.property_}"
-            if prop_id in seen:
-                property_.property_ = f"{property_.property_}_{i+1}"
-                seen.add(f"{property_.class_}.{property_.property_}")
-            else:
-                seen.add(prop_id)
+    def _update_value_type_occurrence_in_comment(cls, value_type: str, comment: str) -> str:
+        occurrence = cls._read_value_type_occurrence_from_comment(value_type, comment)
+        return comment.replace(
+            f"with value type <{value_type}> which occurs <{occurrence}> times in the graph",
+            f"with value type <{value_type}> which occurs <{occurrence+1}> times in the graph",
+        )
 
     @classmethod
-    def _fix_naming_of_entities(cls, rules: InformationRules) -> None:
-        # Fixing class ids
-        for class_ in rules.classes:
-            class_.class_ = class_.class_.as_dms_compliant_entity()
-            class_.parent = [parent.as_dms_compliant_entity() for parent in class_.parent] if class_.parent else None
-
-        # Fixing property definitions
-        for property_ in rules.properties:
-            # fix class id
-            property_.class_ = property_.class_.as_dms_compliant_entity()
-
-            # fix property id
-            property_.property_ = replace_non_alphanumeric_with_underscore(property_.property_)
-
-            # fix value type
-            if isinstance(property_.value_type, ClassEntity):
-                property_.value_type = property_.value_type.as_dms_compliant_entity()
+    def _read_value_type_occurrence_from_comment(cls, value_type: str, comment: str) -> int:
+        return int(
+            cast(
+                re.Match, re.search(rf"with value type <{value_type}> which occurs <(\d+)> times in the graph", comment)
+            ).group(1)
+        )
```

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/importers/_owl2rules/_owl2classes.py` & `cognite_neat-0.78.3/cognite/neat/rules/importers/_owl2rules/_owl2classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py` & `cognite_neat-0.78.3/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/importers/_owl2rules/_owl2properties.py` & `cognite_neat-0.78.3/cognite/neat/rules/importers/_owl2rules/_owl2properties.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/importers/_owl2rules/_owl2rules.py` & `cognite_neat-0.78.3/cognite/neat/rules/importers/_owl2rules/_owl2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/importers/_spreadsheet2rules.py` & `cognite_neat-0.78.3/cognite/neat/rules/importers/_spreadsheet2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/importers/_yaml2rules.py` & `cognite_neat-0.78.3/cognite/neat/rules/importers/_yaml2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/issues/__init__.py` & `cognite_neat-0.78.3/cognite/neat/rules/issues/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/issues/base.py` & `cognite_neat-0.78.3/cognite/neat/rules/issues/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/issues/dms.py` & `cognite_neat-0.78.3/cognite/neat/rules/issues/dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/issues/fileread.py` & `cognite_neat-0.78.3/cognite/neat/rules/issues/fileread.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/issues/formatters.py` & `cognite_neat-0.78.3/cognite/neat/rules/issues/formatters.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/issues/importing.py` & `cognite_neat-0.78.3/cognite/neat/rules/issues/importing.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/issues/spreadsheet.py` & `cognite_neat-0.78.3/cognite/neat/rules/issues/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/issues/spreadsheet_file.py` & `cognite_neat-0.78.3/cognite/neat/rules/issues/spreadsheet_file.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/models/__init__.py` & `cognite_neat-0.78.3/cognite/neat/rules/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/models/_base.py` & `cognite_neat-0.78.3/cognite/neat/rules/models/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/models/_rdfpath.py` & `cognite_neat-0.78.3/cognite/neat/rules/models/_rdfpath.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/models/_types/_base.py` & `cognite_neat-0.78.3/cognite/neat/rules/models/_types/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/models/_types/_field.py` & `cognite_neat-0.78.3/cognite/neat/rules/models/_types/_field.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/models/data_types.py` & `cognite_neat-0.78.3/cognite/neat/rules/models/data_types.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/models/dms/_converter.py` & `cognite_neat-0.78.3/cognite/neat/rules/models/dms/_converter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/models/dms/_exporter.py` & `cognite_neat-0.78.3/cognite/neat/rules/models/dms/_exporter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/models/dms/_rules.py` & `cognite_neat-0.78.3/cognite/neat/rules/models/dms/_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/models/dms/_rules_input.py` & `cognite_neat-0.78.3/cognite/neat/rules/models/dms/_rules_input.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/models/dms/_schema.py` & `cognite_neat-0.78.3/cognite/neat/rules/models/dms/_schema.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/models/dms/_serializer.py` & `cognite_neat-0.78.3/cognite/neat/rules/models/dms/_serializer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/models/dms/_validation.py` & `cognite_neat-0.78.3/cognite/neat/rules/models/dms/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/models/domain.py` & `cognite_neat-0.78.3/cognite/neat/rules/models/domain.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/models/entities.py` & `cognite_neat-0.78.3/cognite/neat/rules/models/entities.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 import re
 import sys
 from abc import ABC, abstractmethod
 from functools import total_ordering
 from typing import Annotated, Any, ClassVar, Generic, TypeVar, cast
 
 from cognite.client.data_classes.data_modeling.ids import ContainerId, DataModelId, NodeId, PropertyId, ViewId
-from pydantic import AnyHttpUrl, BaseModel, BeforeValidator, Field, PlainSerializer, model_serializer, model_validator
+from pydantic import (
+    AnyHttpUrl,
+    BaseModel,
+    BeforeValidator,
+    Field,
+    PlainSerializer,
+    model_serializer,
+    model_validator,
+)
 
+from cognite.neat.rules.models.data_types import DataType
 from cognite.neat.utils.utils import replace_non_alphanumeric_with_underscore
 
 if sys.version_info >= (3, 11):
     from enum import StrEnum
     from typing import Self
 else:
     from backports.strenum import StrEnum
@@ -34,14 +43,15 @@
     dms_value_type = "dms_value_type"
     dms_node = "dms_node"
     view = "view"
     reference_entity = "reference_entity"
     container = "container"
     datamodel = "datamodel"
     undefined = "undefined"
+    multi_value_type = "multi_value_type"
 
 
 # ALLOWED
 _ALLOWED_PATTERN = r"[^a-zA-Z0-9-_.]"
 
 # FOR PARSING STRINGS:
 _PREFIX_REGEX = r"[a-zA-Z]+[a-zA-Z0-9-_.]*[a-zA-Z0-9]+"
@@ -54,14 +64,15 @@
     rf"^(?P<prefix>{_PREFIX_REGEX}):(?P<suffix>{_SUFFIX_REGEX})\(version=(?P<version>{_VERSION_REGEX})\)$"
 )
 _CLASS_ID_REGEX = rf"(?P<{EntityTypes.class_}>{_ENTITY_ID_REGEX})"
 _CLASS_ID_REGEX_COMPILED = re.compile(rf"^{_CLASS_ID_REGEX}$")
 _PROPERTY_ID_REGEX = rf"\((?P<{EntityTypes.property_}>{_ENTITY_ID_REGEX})\)"
 
 _ENTITY_PATTERN = re.compile(r"^(?P<prefix>.*?):?(?P<suffix>[^(:]*)(\((?P<content>[^)]+)\))?$")
+_MULTI_VALUE_TYPE_PATTERN = re.compile(r"^(?P<types>.*?)(\((?P<content>[^)]+)\))?$")
 
 
 class _UndefinedType(BaseModel): ...
 
 
 class _UnknownType(BaseModel):
     def __str__(self) -> str:
@@ -234,19 +245,14 @@
         space = default_space if isinstance(self.prefix, _UndefinedType) else self.prefix
         return ViewEntity(space=space, externalId=str(self.suffix), version=version)
 
     def as_container_entity(self, default_space: str) -> "ContainerEntity":
         space = default_space if isinstance(self.prefix, _UndefinedType) else self.prefix
         return ContainerEntity(space=space, externalId=str(self.suffix))
 
-    def as_dms_compliant_entity(self) -> "Self":
-        new_entity = self.model_copy(deep=True)
-        new_entity.suffix = replace_non_alphanumeric_with_underscore(new_entity.suffix)
-        return new_entity
-
 
 class ParentClassEntity(ClassEntity):
     type_: ClassVar[EntityTypes] = EntityTypes.parent_class
 
     def as_class_entity(self) -> ClassEntity:
         return ClassEntity(prefix=self.prefix, suffix=self.suffix, version=self.version)
 
@@ -260,14 +266,68 @@
     def id(self) -> str:
         return str(Unknown)
 
 
 T_ID = TypeVar("T_ID", bound=ContainerId | ViewId | DataModelId | PropertyId | NodeId | None)
 
 
+class MultiValueTypeInfo(BaseModel):
+    type_: ClassVar[EntityTypes] = EntityTypes.multi_value_type
+    types: list[DataType | ClassEntity]
+
+    def __str__(self) -> str:
+        return " | ".join([str(t) for t in self.types])
+
+    @model_serializer(when_used="unless-none", return_type=str)
+    def as_str(self) -> str:
+        return str(self)
+
+    @classmethod
+    def load(cls, data: Any) -> "MultiValueTypeInfo":
+        # already instance of MultiValueTypeInfo
+        if isinstance(data, cls):
+            return data
+
+        # it is a raw string that needs to be parsed
+        elif isinstance(data, str):
+            return cls.model_validate({_PARSE: data})
+
+        # it is dict that needs to be parsed
+        else:
+            return cls.model_validate(data)
+
+    @model_validator(mode="before")
+    def _load(cls, data: Any) -> "dict | MultiValueTypeInfo":
+        if isinstance(data, dict) and _PARSE in data:
+            data = data[_PARSE]
+        elif isinstance(data, dict):
+            return data
+        else:
+            raise ValueError(f"Cannot load {cls.__name__} from {data}")
+
+        result = cls._parse(data)
+        return result
+
+    @classmethod
+    def _parse(cls, raw: str) -> dict:
+        if not (types := [type_.strip() for type_ in raw.split("|")]):
+            return {"types": [UnknownEntity()]}
+        else:
+            return {
+                "types": [
+                    DataType.load(type_) if DataType.is_data_type(type_) else ClassEntity.load(type_) for type_ in types
+                ]
+            }
+
+    def set_default_prefix(self, prefix: str):
+        for type_ in self.types:
+            if isinstance(type_, ClassEntity) and type_.prefix is Undefined:
+                type_.prefix = prefix
+
+
 class DMSEntity(Entity, Generic[T_ID], ABC):
     type_: ClassVar[EntityTypes] = EntityTypes.undefined
     prefix: str = Field(alias="space")
     suffix: str = Field(alias="externalId")
 
     @classmethod
     def load(cls: "type[T_DMSEntity]", data: Any, **defaults) -> "T_DMSEntity | DMSUnknownEntity":  # type: ignore[override]
@@ -293,14 +353,19 @@
     @abstractmethod
     def from_id(cls, id: T_ID) -> Self:
         raise NotImplementedError("Method from_id must be implemented in subclasses")
 
     def as_class(self) -> ClassEntity:
         return ClassEntity(prefix=self.space, suffix=self.external_id)
 
+    def as_dms_compliant_entity(self) -> "Self":
+        new_entity = self.model_copy(deep=True)
+        new_entity.suffix = replace_non_alphanumeric_with_underscore(new_entity.suffix)
+        return new_entity
+
 
 T_DMSEntity = TypeVar("T_DMSEntity", bound=DMSEntity)
 
 
 class ContainerEntity(DMSEntity[ContainerId]):
     type_: ClassVar[EntityTypes] = EntityTypes.container
```

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/models/information/_converter.py` & `cognite_neat-0.78.3/cognite/neat/rules/models/information/_converter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/models/information/_rules.py` & `cognite_neat-0.78.3/cognite/neat/rules/models/information/_rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     VersionType,
 )
 from cognite.neat.rules.models.data_types import DataType
 from cognite.neat.rules.models.domain import DomainRules
 from cognite.neat.rules.models.entities import (
     ClassEntity,
     EntityTypes,
+    MultiValueTypeInfo,
     ParentClassEntity,
     ParentEntityList,
     ReferenceEntity,
     Undefined,
     UnknownEntity,
     URLEntity,
 )
@@ -158,15 +159,17 @@
               knowledge graph. Defaults to None (no transformation)
     """
 
     class_: ClassEntity = Field(alias="Class")
     property_: PropertyType = Field(alias="Property")
     name: str | None = Field(alias="Name", default=None)
     description: str | None = Field(alias="Description", default=None)
-    value_type: DataType | ClassEntity | UnknownEntity = Field(alias="Value Type", union_mode="left_to_right")
+    value_type: DataType | ClassEntity | MultiValueTypeInfo | UnknownEntity = Field(
+        alias="Value Type", union_mode="left_to_right"
+    )
     min_count: int | None = Field(alias="Min Count", default=None)
     max_count: int | float | None = Field(alias="Max Count", default=None)
     default: Any | None = Field(alias="Default", default=None)
     reference: URLEntity | ReferenceEntity | None = Field(alias="Reference", default=None, union_mode="left_to_right")
     match_type: MatchType | None = Field(alias="Match Type", default=None)
     rule_type: str | TransformationRuleType | None = Field(alias="Rule Type", default=None)
     rule: str | AllReferences | SingleProperty | Hop | RawLookup | SPARQLQuery | Traversal | None = Field(
@@ -273,14 +276,18 @@
 
     @model_validator(mode="after")
     def update_entities_prefix(self) -> Self:
         # update expected_value_types
         for property_ in self.properties:
             if isinstance(property_.value_type, ClassEntity) and property_.value_type.prefix is Undefined:
                 property_.value_type.prefix = self.metadata.prefix
+
+            if isinstance(property_.value_type, MultiValueTypeInfo):
+                property_.value_type.set_default_prefix(self.metadata.prefix)
+
             if property_.class_.prefix is Undefined:
                 property_.class_.prefix = self.metadata.prefix
 
         # update parent classes
         for class_ in self.classes:
             if class_.parent:
                 for parent in cast(list[ParentClassEntity], class_.parent):
```

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/models/information/_rules_input.py` & `cognite_neat-0.78.3/cognite/neat/rules/models/information/_rules_input.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,21 @@
 from datetime import datetime
 from typing import Any, Literal, cast, overload
 
 from rdflib import Namespace
 
 from cognite.neat.rules.models._base import DataModelType, ExtensionCategory, SchemaCompleteness, _add_alias
 from cognite.neat.rules.models.data_types import DataType
-from cognite.neat.rules.models.entities import ClassEntity, ParentClassEntity, Unknown, UnknownEntity
+from cognite.neat.rules.models.entities import (
+    ClassEntity,
+    MultiValueTypeInfo,
+    ParentClassEntity,
+    Unknown,
+    UnknownEntity,
+)
 
 from ._rules import InformationClass, InformationMetadata, InformationProperty, InformationRules
 
 
 @dataclass
 class InformationMetadataInput:
     schema_: Literal["complete", "partial", "extended"]
@@ -117,18 +123,23 @@
             reference=data.get("reference", None),
             match_type=data.get("match_type", None),
             rule_type=data.get("rule_type", None),
             rule=data.get("rule", None),
         )
 
     def dump(self, default_prefix: str) -> dict[str, Any]:
-        value_type: DataType | ClassEntity | UnknownEntity
+        value_type: MultiValueTypeInfo | DataType | ClassEntity | UnknownEntity
 
         # property holding xsd data type
-        if DataType.is_data_type(self.value_type):
+        # check if it is multi value type
+        if "|" in self.value_type:
+            value_type = MultiValueTypeInfo.load(self.value_type)
+            value_type.set_default_prefix(default_prefix)
+
+        elif DataType.is_data_type(self.value_type):
             value_type = DataType.load(self.value_type)
 
         # unknown value type
         elif self.value_type == str(Unknown):
             value_type = UnknownEntity()
 
         # property holding link to class
@@ -253,14 +264,15 @@
             reference = InformationRulesInput.load(self.reference.model_dump()).dump()
         last: dict[str, Any] | None = None
         if isinstance(self.last, InformationRulesInput):
             last = self.last.dump()
         elif isinstance(self.last, InformationRules):
             # We need to load through the InformationRulesInput to set the correct default space and version
             last = InformationRulesInput.load(self.last.model_dump()).dump()
+
         return dict(
             Metadata=self.metadata.dump(),
             Properties=[prop.dump(default_prefix) for prop in self.properties],
             Classes=[class_.dump(default_prefix) for class_ in self.classes],
             Last=last,
             Reference=reference,
         )
```

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/models/information/_serializer.py` & `cognite_neat-0.78.3/cognite/neat/rules/models/information/_serializer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/models/information/_validation.py` & `cognite_neat-0.78.3/cognite/neat/rules/models/information/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/rules/models/wrapped_entities.py` & `cognite_neat-0.78.3/cognite/neat/rules/models/wrapped_entities.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/utils/cdf.py` & `cognite_neat-0.78.3/cognite/neat/utils/cdf.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/utils/cdf_classes.py` & `cognite_neat-0.78.3/cognite/neat/utils/cdf_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/utils/cdf_loaders/_base.py` & `cognite_neat-0.78.3/cognite/neat/utils/cdf_loaders/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/utils/cdf_loaders/_data_modeling.py` & `cognite_neat-0.78.3/cognite/neat/utils/cdf_loaders/_data_modeling.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/utils/cdf_loaders/_ingestion.py` & `cognite_neat-0.78.3/cognite/neat/utils/cdf_loaders/_ingestion.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/utils/cdf_loaders/data_classes.py` & `cognite_neat-0.78.3/cognite/neat/utils/cdf_loaders/data_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/utils/exceptions.py` & `cognite_neat-0.78.3/cognite/neat/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/utils/spreadsheet.py` & `cognite_neat-0.78.3/cognite/neat/utils/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/utils/text.py` & `cognite_neat-0.78.3/cognite/neat/utils/text.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/utils/utils.py` & `cognite_neat-0.78.3/cognite/neat/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/utils/xml.py` & `cognite_neat-0.78.3/cognite/neat/utils/xml.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/_exceptions.py` & `cognite_neat-0.78.3/cognite/neat/workflows/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/base.py` & `cognite_neat-0.78.3/cognite/neat/workflows/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/cdf_store.py` & `cognite_neat-0.78.3/cognite/neat/workflows/cdf_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/examples/Export_DMS/workflow.yaml` & `cognite_neat-0.78.3/cognite/neat/workflows/examples/Export_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml` & `cognite_neat-0.78.3/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml` & `cognite_neat-0.78.3/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml` & `cognite_neat-0.78.3/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/examples/Import_DMS/workflow.yaml` & `cognite_neat-0.78.3/cognite/neat/workflows/examples/Import_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml` & `cognite_neat-0.78.3/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml` & `cognite_neat-0.78.3/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml` & `cognite_neat-0.78.3/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml` & `cognite_neat-0.78.3/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml` & `cognite_neat-0.78.3/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/manager.py` & `cognite_neat-0.78.3/cognite/neat/workflows/manager.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/migration/steps.py` & `cognite_neat-0.78.3/cognite/neat/workflows/migration/steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/migration/wf_manifests.py` & `cognite_neat-0.78.3/cognite/neat/workflows/migration/wf_manifests.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/model.py` & `cognite_neat-0.78.3/cognite/neat/workflows/model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/steps/data_contracts.py` & `cognite_neat-0.78.3/cognite/neat/workflows/steps/data_contracts.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/steps/lib/current/graph_extractor.py` & `cognite_neat-0.78.3/cognite/neat/workflows/steps/lib/current/graph_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/steps/lib/current/graph_loader.py` & `cognite_neat-0.78.3/cognite/neat/workflows/steps/lib/current/graph_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/steps/lib/current/graph_store.py` & `cognite_neat-0.78.3/cognite/neat/workflows/steps/lib/current/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/steps/lib/current/rules_exporter.py` & `cognite_neat-0.78.3/cognite/neat/workflows/steps/lib/current/rules_exporter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/steps/lib/current/rules_importer.py` & `cognite_neat-0.78.3/cognite/neat/workflows/steps/lib/current/rules_importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,24 +273,14 @@
         Configurable(
             name="Role",
             value="infer",
             label="For what role Rules are intended?",
             options=["infer", *RoleTypes.__members__.keys()],
         ),
         Configurable(
-            name="Make compliant",
-            value="True",
-            label=(
-                "Attempt to make the imported Rules compliant, by fixing "
-                "redefinition of properties and by making ids of entities compliant with"
-                " CDF-allowed set of characters ."
-            ),
-            options=["True", "False"],
-        ),
-        Configurable(
             name="Maximum number of instances to process",
             value="-1",
             label=(
                 "Maximum number of instances to process"
                 " to infer rules from the RDF file. Default -1 means all instances."
             ),
         ),
@@ -298,15 +288,14 @@
 
     def run(self, flow_message: FlowMessage) -> (FlowMessage, MultiRuleData):  # type: ignore[syntax, override]
         if self.configs is None or self.data_store_path is None:
             raise StepNotInitialized(type(self).__name__)
 
         file_path = self.configs.get("File path", None)
         full_path = flow_message.payload.get("full_path", None) if flow_message.payload else None
-        make_compliant = self.configs.get("Make compliant", "True") == "True"
 
         try:
             max_number_of_instance = int(self.configs.get("Maximum number of instances to process", -1))
         except ValueError:
             error_text = "Maximum number of instances to process should be an integer value"
             return FlowMessage(error_text=error_text, step_execution_status=StepExecutionStatus.ABORT_AND_FAIL)
 
@@ -321,15 +310,15 @@
         # if role is None, it will be inferred from the rules file
         role = self.configs.get("Role")
         role_enum = None
         if role != "infer" and role is not None:
             role_enum = RoleTypes[role]
 
         inference_importer = importers.InferenceImporter.from_rdf_file(
-            rdf_file_path, make_compliant=make_compliant, max_number_of_instance=max_number_of_instance
+            rdf_file_path, max_number_of_instance=max_number_of_instance
         )
         rules, issues = inference_importer.to_rules(errors="continue", role=role_enum)
 
         if rules is None:
             output_dir = self.config.staging_path
             report_writer = FORMATTER_BY_NAME[self.configs["Report formatter"]]()
             report_writer.write_to_file(issues, file_or_dir_path=output_dir)
```

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/steps/lib/current/rules_validator.py` & `cognite_neat-0.78.3/cognite/neat/workflows/steps/lib/current/rules_validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/steps/lib/io/io_steps.py` & `cognite_neat-0.78.3/cognite/neat/workflows/steps/lib/io/io_steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/steps/lib/legacy/graph_contextualization.py` & `cognite_neat-0.78.3/cognite/neat/workflows/steps/lib/legacy/graph_contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/steps/lib/legacy/graph_extractor.py` & `cognite_neat-0.78.3/cognite/neat/workflows/steps/lib/legacy/graph_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/steps/lib/legacy/graph_loader.py` & `cognite_neat-0.78.3/cognite/neat/workflows/steps/lib/legacy/graph_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/steps/lib/legacy/graph_store.py` & `cognite_neat-0.78.3/cognite/neat/workflows/steps/lib/legacy/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/steps/lib/legacy/graph_transformer.py` & `cognite_neat-0.78.3/cognite/neat/workflows/steps/lib/legacy/graph_transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/steps/lib/legacy/rules_exporter.py` & `cognite_neat-0.78.3/cognite/neat/workflows/steps/lib/legacy/rules_exporter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/steps/lib/legacy/rules_importer.py` & `cognite_neat-0.78.3/cognite/neat/workflows/steps/lib/legacy/rules_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/steps/step_model.py` & `cognite_neat-0.78.3/cognite/neat/workflows/steps/step_model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/steps_registry.py` & `cognite_neat-0.78.3/cognite/neat/workflows/steps_registry.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/tasks.py` & `cognite_neat-0.78.3/cognite/neat/workflows/tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/cognite/neat/workflows/triggers.py` & `cognite_neat-0.78.3/cognite/neat/workflows/triggers.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.78.2/pyproject.toml` & `cognite_neat-0.78.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-neat"
-version = "0.78.2"
+version = "0.78.3"
 readme = "README.md"
 description = "Knowledge graph transformation"
 authors = [
     "Nikola Vasiljevic <nikola.vasiljevic@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>",
     "Aleksandrs Livincovs <aleksandrs.livincovs@cognite.com>",
 ]
```

### Comparing `cognite_neat-0.78.2/PKG-INFO` & `cognite_neat-0.78.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-neat
-Version: 0.78.2
+Version: 0.78.3
 Summary: Knowledge graph transformation
 Home-page: https://cognite-neat.readthedocs-hosted.com/
 License: Apache-2.0
 Author: Nikola Vasiljevic
 Author-email: nikola.vasiljevic@cognite.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

