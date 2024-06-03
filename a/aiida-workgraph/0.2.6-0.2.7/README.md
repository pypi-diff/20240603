# Comparing `tmp/aiida_workgraph-0.2.6.tar.gz` & `tmp/aiida_workgraph-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida_workgraph-0.2.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiida_workgraph-0.2.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiida_workgraph-0.2.6.tar` & `aiida_workgraph-0.2.7.tar`

### file list

```diff
@@ -1,126 +1,128 @@
--rw-r--r--   0        0        0     1066 2023-12-11 16:36:18.395013 aiida_workgraph-0.2.6/LICENSE
--rw-r--r--   0        0        0     5318 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.6/README.md
--rw-r--r--   0        0        0      175 2024-05-23 10:18:29.324006 aiida_workgraph-0.2.6/aiida_workgraph/__init__.py
--rw-r--r--   0        0        0        0 2024-05-20 19:33:14.095414 aiida_workgraph-0.2.6/aiida_workgraph/calculations/__init__.py
--rw-r--r--   0        0        0     8238 2024-05-23 10:17:58.548150 aiida_workgraph-0.2.6/aiida_workgraph/calculations/python.py
--rw-r--r--   0        0        0     2114 2024-05-23 10:17:58.548150 aiida_workgraph-0.2.6/aiida_workgraph/calculations/python_parser.py
--rw-r--r--   0        0        0      279 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/cli/__init__.py
--rw-r--r--   0        0        0    12112 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/cli/cmd_graph.py
--rw-r--r--   0        0        0     1937 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/cli/cmd_web.py
--rw-r--r--   0        0        0      714 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/cli/cmd_workgraph.py
--rw-r--r--   0        0        0     6599 2024-05-18 09:24:02.309034 aiida_workgraph-0.2.6/aiida_workgraph/cli/query_workgraph.py
--rw-r--r--   0        0        0     2829 2024-05-22 09:59:58.253538 aiida_workgraph-0.2.6/aiida_workgraph/collection.py
--rw-r--r--   0        0        0    18855 2024-05-22 09:59:58.253538 aiida_workgraph-0.2.6/aiida_workgraph/decorator.py
--rw-r--r--   0        0        0        0 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/engine/__init__.py
--rw-r--r--   0        0        0    50042 2024-05-23 10:17:58.548150 aiida_workgraph-0.2.6/aiida_workgraph/engine/workgraph.py
--rw-r--r--   0        0        0        0 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/executors/__init__.py
--rw-r--r--   0        0        0      897 2024-05-07 20:56:57.572283 aiida_workgraph-0.2.6/aiida_workgraph/executors/builtin.py
--rw-r--r--   0        0        0      740 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.6/aiida_workgraph/executors/qe.py
--rw-r--r--   0        0        0      768 2024-05-07 20:56:57.572283 aiida_workgraph-0.2.6/aiida_workgraph/executors/test.py
--rw-r--r--   0        0        0     4151 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.6/aiida_workgraph/node.py
--rw-r--r--   0        0        0      847 2024-05-15 13:45:10.407702 aiida_workgraph-0.2.6/aiida_workgraph/nodes/__init__.py
--rw-r--r--   0        0        0     3957 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.6/aiida_workgraph/nodes/builtin.py
--rw-r--r--   0        0        0     2168 2024-05-15 13:45:10.407702 aiida_workgraph-0.2.6/aiida_workgraph/nodes/qe.py
--rw-r--r--   0        0        0     7233 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.6/aiida_workgraph/nodes/test.py
--rw-r--r--   0        0        0      141 2024-05-23 10:17:58.548150 aiida_workgraph-0.2.6/aiida_workgraph/orm/__init__.py
--rw-r--r--   0        0        0     4353 2024-05-23 10:17:58.548150 aiida_workgraph-0.2.6/aiida_workgraph/orm/atoms.py
--rw-r--r--   0        0        0     2619 2024-05-23 10:17:58.548150 aiida_workgraph-0.2.6/aiida_workgraph/orm/general_data.py
--rw-r--r--   0        0        0     1715 2024-05-23 10:17:58.548150 aiida_workgraph-0.2.6/aiida_workgraph/orm/serializer.py
--rw-r--r--   0        0        0     1214 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/orm/worktree.py
--rw-r--r--   0        0        0      115 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/properties/__init__.py
--rw-r--r--   0        0        0    10647 2024-05-15 13:45:10.407702 aiida_workgraph-0.2.6/aiida_workgraph/properties/built_in.py
--rw-r--r--   0        0        0     2131 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.6/aiida_workgraph/property.py
--rw-r--r--   0        0        0     1386 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.6/aiida_workgraph/socket.py
--rw-r--r--   0        0        0      111 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/sockets/__init__.py
--rw-r--r--   0        0        0     3760 2024-05-15 13:45:10.407702 aiida_workgraph-0.2.6/aiida_workgraph/sockets/built_in.py
--rw-r--r--   0        0        0     8697 2024-05-22 09:59:58.253538 aiida_workgraph-0.2.6/aiida_workgraph/utils/__init__.py
--rw-r--r--   0        0        0     6132 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.6/aiida_workgraph/utils/analysis.py
--rw-r--r--   0        0        0     1754 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.6/aiida_workgraph/utils/graph.py
--rw-r--r--   0        0        0      763 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/web/README.md
--rw-r--r--   0        0        0        0 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/web/backend/app/__init__.py
--rw-r--r--   0        0        0     2395 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/web/backend/app/api.py
--rw-r--r--   0        0        0     3638 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/web/backend/app/daemon.py
--rw-r--r--   0        0        0     2208 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.6/aiida_workgraph/web/backend/app/datanode.py
--rw-r--r--   0        0        0     6618 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.6/aiida_workgraph/web/backend/app/utils.py
--rw-r--r--   0        0        0     5130 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/web/backend/app/workgraph.py
--rw-r--r--   0        0        0      115 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/web/backend/main.py
--rw-r--r--   0        0        0      310 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/.gitignore
--rw-r--r--   0        0        0       62 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/.rete-patch
--rw-r--r--   0        0        0     2136 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/README.md
--rw-r--r--   0        0        0      517 2024-05-20 19:35:26.142370 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/asset-manifest.json
--rw-r--r--   0        0        0     3870 2024-05-20 19:34:56.150973 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/favicon.ico
--rw-r--r--   0        0        0      654 2024-05-20 19:35:26.142370 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/index.html
--rw-r--r--   0        0        0      306 2024-05-20 19:34:56.150973 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/manifest.json
--rw-r--r--   0        0        0       67 2024-05-20 19:34:56.150973 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/robots.txt
--rw-r--r--   0        0        0    18033 2024-05-20 19:35:26.170373 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/static/css/main.8ddb8b68.css
--rw-r--r--   0        0        0    46655 2024-05-20 19:35:26.170373 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/static/css/main.8ddb8b68.css.map
--rw-r--r--   0        0        0     4518 2024-05-20 19:35:26.170373 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/static/js/787.095790c7.chunk.js
--rw-r--r--   0        0        0    10597 2024-05-20 19:35:26.170373 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/static/js/787.095790c7.chunk.js.map
--rw-r--r--   0        0        0  3614868 2024-05-20 19:35:26.142370 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js
--rw-r--r--   0        0        0     3456 2024-05-20 19:35:26.170373 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js.LICENSE.txt
--rw-r--r--   0        0        0 13934230 2024-05-20 19:35:26.170373 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js.map
--rw-r--r--   0        0        0  1408324 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/package-lock.json
--rw-r--r--   0        0        0     2249 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/package.json
--rw-r--r--   0        0        0     3870 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/public/favicon.ico
--rw-r--r--   0        0        0     1324 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/public/index.html
--rw-r--r--   0        0        0      306 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/public/manifest.json
--rw-r--r--   0        0        0       67 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/public/robots.txt
--rw-r--r--   0        0        0     2443 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/App.css
--rw-r--r--   0        0        0     1143 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/App.js
--rw-r--r--   0        0        0      273 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/App.test.tsx
--rw-r--r--   0        0        0     1675 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/AtomsItem.js
--rw-r--r--   0        0        0       94 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/Data.js
--rw-r--r--   0        0        0      106 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/DataNode.js
--rw-r--r--   0        0        0      505 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/DataNodeItem.css
--rw-r--r--   0        0        0     1458 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/DataNodeItem.tsx
--rw-r--r--   0        0        0     5593 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/DataNodeTable.js
--rw-r--r--   0        0        0      116 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/Home.js
--rw-r--r--   0        0        0     1324 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/Layout.css
--rw-r--r--   0        0        0     1067 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/Layout.js
--rw-r--r--   0        0        0     5792 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/NodeDetails.js
--rw-r--r--   0        0        0     2784 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/Settings.js
--rw-r--r--   0        0        0     1025 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphDetail.js
--rw-r--r--   0        0        0     2631 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphDuration.js
--rw-r--r--   0        0        0     1129 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphIndicator.js
--rw-r--r--   0        0        0     8796 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphItem.tsx
--rw-r--r--   0        0        0     1064 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphItemStyles.ts
--rw-r--r--   0        0        0      837 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphLog.js
--rw-r--r--   0        0        0     3434 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphSummary.js
--rw-r--r--   0        0        0      990 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphTable.css
--rw-r--r--   0        0        0     7518 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphTable.js
--rw-r--r--   0        0        0      366 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/index.css
--rw-r--r--   0        0        0      554 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/index.tsx
--rw-r--r--   0        0        0     6007 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/logo.svg
--rw-r--r--   0        0        0       40 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/react-app-env.d.ts
--rw-r--r--   0        0        0      425 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/reportWebVitals.ts
--rw-r--r--   0        0        0      160 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete.css
--rw-r--r--   0        0        0     2787 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/customization.ts
--rw-r--r--   0        0        0      813 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/customization/CustomConnection.tsx
--rw-r--r--   0        0        0     4981 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/customization/CustomNode.tsx
--rw-r--r--   0        0        0      566 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/customization/CustomSocket.tsx
--rw-r--r--   0        0        0      540 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/customization/StyledNode.tsx
--rw-r--r--   0        0        0      602 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/customization/background.css
--rw-r--r--   0        0        0      378 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/customization/custom-background.ts
--rw-r--r--   0        0        0       94 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/customization/vars.ts
--rw-r--r--   0        0        0     4864 2024-05-04 20:38:47.853168 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/default.ts
--rw-r--r--   0        0        0      603 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/index.ts
--rw-r--r--   0        0        0      241 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/setupTests.ts
--rw-r--r--   0        0        0      535 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/tsconfig.json
--rw-r--r--   0        0        0       94 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/widget/.gitignore
--rw-r--r--   0        0        0      488 2024-04-13 07:05:41.907170 aiida_workgraph-0.2.6/aiida_workgraph/widget/.ipynb_checkpoints/example-checkpoint.ipynb
--rw-r--r--   0        0        0      552 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/widget/README.md
--rw-r--r--   0        0        0       71 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/widget/__init__.py
--rw-r--r--   0        0        0     7122 2024-05-03 14:17:12.929117 aiida_workgraph-0.2.6/aiida_workgraph/widget/js/default_rete.ts
--rw-r--r--   0        0        0      565 2024-04-22 20:35:00.919099 aiida_workgraph-0.2.6/aiida_workgraph/widget/js/widget.css
--rw-r--r--   0        0        0     5905 2024-04-22 20:35:00.919099 aiida_workgraph-0.2.6/aiida_workgraph/widget/js/widget.tsx
--rw-r--r--   0        0        0   148687 2024-04-22 20:35:00.923099 aiida_workgraph-0.2.6/aiida_workgraph/widget/package-lock.json
--rw-r--r--   0        0        0      851 2024-04-22 20:35:00.923099 aiida_workgraph-0.2.6/aiida_workgraph/widget/package.json
--rw-r--r--   0        0        0      765 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/widget/pyproject.toml
--rw-r--r--   0        0        0     1981 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.6/aiida_workgraph/widget/src/widget/__init__.py
--rw-r--r--   0        0        0      429 2024-05-20 19:36:16.932122 aiida_workgraph-0.2.6/aiida_workgraph/widget/src/widget/static/widget.css
--rw-r--r--   0        0        0  1796776 2024-05-20 19:36:16.932122 aiida_workgraph-0.2.6/aiida_workgraph/widget/src/widget/static/widget.js
--rw-r--r--   0        0        0      897 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.6/aiida_workgraph/widget/src/widget/utils.py
--rw-r--r--   0        0        0      453 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/widget/tsconfig.json
--rw-r--r--   0        0        0    14913 2024-05-20 19:33:14.095414 aiida_workgraph-0.2.6/aiida_workgraph/workgraph.py
--rw-r--r--   0        0        0     3216 2024-05-23 10:17:58.548150 aiida_workgraph-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     7358 1970-01-01 00:00:00.000000 aiida_workgraph-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-12-11 16:36:18.395013 aiida_workgraph-0.2.7/LICENSE
+-rw-r--r--   0        0        0     5319 2024-05-30 07:46:01.736427 aiida_workgraph-0.2.7/README.md
+-rw-r--r--   0        0        0      175 2024-06-03 13:21:00.373031 aiida_workgraph-0.2.7/aiida_workgraph/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 19:33:14.095414 aiida_workgraph-0.2.7/aiida_workgraph/calculations/__init__.py
+-rw-r--r--   0        0        0    10534 2024-06-03 07:09:41.525548 aiida_workgraph-0.2.7/aiida_workgraph/calculations/python.py
+-rw-r--r--   0        0        0     2138 2024-05-28 05:46:08.271800 aiida_workgraph-0.2.7/aiida_workgraph/calculations/python_parser.py
+-rw-r--r--   0        0        0      279 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.7/aiida_workgraph/cli/__init__.py
+-rw-r--r--   0        0        0    12112 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.7/aiida_workgraph/cli/cmd_graph.py
+-rw-r--r--   0        0        0     1937 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.7/aiida_workgraph/cli/cmd_web.py
+-rw-r--r--   0        0        0      714 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.7/aiida_workgraph/cli/cmd_workgraph.py
+-rw-r--r--   0        0        0     6599 2024-05-18 09:24:02.309034 aiida_workgraph-0.2.7/aiida_workgraph/cli/query_workgraph.py
+-rw-r--r--   0        0        0     3345 2024-05-29 08:53:33.372846 aiida_workgraph-0.2.7/aiida_workgraph/collection.py
+-rw-r--r--   0        0        0    21922 2024-06-03 13:20:44.967048 aiida_workgraph-0.2.7/aiida_workgraph/decorator.py
+-rw-r--r--   0        0        0        0 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.7/aiida_workgraph/engine/__init__.py
+-rw-r--r--   0        0        0     5720 2024-06-03 13:20:44.967048 aiida_workgraph-0.2.7/aiida_workgraph/engine/utils.py
+-rw-r--r--   0        0        0    48269 2024-06-02 15:22:40.773404 aiida_workgraph-0.2.7/aiida_workgraph/engine/workgraph.py
+-rw-r--r--   0        0        0        0 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.7/aiida_workgraph/executors/__init__.py
+-rw-r--r--   0        0        0      897 2024-05-07 20:56:57.572283 aiida_workgraph-0.2.7/aiida_workgraph/executors/builtin.py
+-rw-r--r--   0        0        0      740 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.7/aiida_workgraph/executors/qe.py
+-rw-r--r--   0        0        0      768 2024-05-07 20:56:57.572283 aiida_workgraph-0.2.7/aiida_workgraph/executors/test.py
+-rw-r--r--   0        0        0     4474 2024-05-29 21:08:21.050925 aiida_workgraph-0.2.7/aiida_workgraph/node.py
+-rw-r--r--   0        0        0      819 2024-05-29 08:53:33.372846 aiida_workgraph-0.2.7/aiida_workgraph/nodes/__init__.py
+-rw-r--r--   0        0        0     1656 2024-05-29 08:53:33.372846 aiida_workgraph-0.2.7/aiida_workgraph/nodes/builtin.py
+-rw-r--r--   0        0        0     2168 2024-05-15 13:45:10.407702 aiida_workgraph-0.2.7/aiida_workgraph/nodes/qe.py
+-rw-r--r--   0        0        0     7233 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.7/aiida_workgraph/nodes/test.py
+-rw-r--r--   0        0        0      153 2024-05-28 05:46:08.271800 aiida_workgraph-0.2.7/aiida_workgraph/orm/__init__.py
+-rw-r--r--   0        0        0     4353 2024-05-23 10:17:58.548150 aiida_workgraph-0.2.7/aiida_workgraph/orm/atoms.py
+-rw-r--r--   0        0        0     2619 2024-05-23 10:17:58.548150 aiida_workgraph-0.2.7/aiida_workgraph/orm/general_data.py
+-rw-r--r--   0        0        0     2992 2024-06-03 07:09:20.217660 aiida_workgraph-0.2.7/aiida_workgraph/orm/serializer.py
+-rw-r--r--   0        0        0     1214 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.7/aiida_workgraph/orm/worktree.py
+-rw-r--r--   0        0        0      115 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.7/aiida_workgraph/properties/__init__.py
+-rw-r--r--   0        0        0    10647 2024-05-15 13:45:10.407702 aiida_workgraph-0.2.7/aiida_workgraph/properties/built_in.py
+-rw-r--r--   0        0        0     2131 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.7/aiida_workgraph/property.py
+-rw-r--r--   0        0        0     1386 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.7/aiida_workgraph/socket.py
+-rw-r--r--   0        0        0      111 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.7/aiida_workgraph/sockets/__init__.py
+-rw-r--r--   0        0        0     3760 2024-05-15 13:45:10.407702 aiida_workgraph-0.2.7/aiida_workgraph/sockets/built_in.py
+-rw-r--r--   0        0        0     9599 2024-05-28 05:46:08.271800 aiida_workgraph-0.2.7/aiida_workgraph/utils/__init__.py
+-rw-r--r--   0        0        0     6132 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.7/aiida_workgraph/utils/analysis.py
+-rw-r--r--   0        0        0     1754 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.7/aiida_workgraph/utils/graph.py
+-rw-r--r--   0        0        0      763 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.7/aiida_workgraph/web/README.md
+-rw-r--r--   0        0        0        0 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.7/aiida_workgraph/web/backend/app/__init__.py
+-rw-r--r--   0        0        0     2395 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.7/aiida_workgraph/web/backend/app/api.py
+-rw-r--r--   0        0        0     3638 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.7/aiida_workgraph/web/backend/app/daemon.py
+-rw-r--r--   0        0        0     2208 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.7/aiida_workgraph/web/backend/app/datanode.py
+-rw-r--r--   0        0        0     6618 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.7/aiida_workgraph/web/backend/app/utils.py
+-rw-r--r--   0        0        0     5130 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.7/aiida_workgraph/web/backend/app/workgraph.py
+-rw-r--r--   0        0        0      115 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.7/aiida_workgraph/web/backend/main.py
+-rw-r--r--   0        0        0      310 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/.gitignore
+-rw-r--r--   0        0        0       62 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/.rete-patch
+-rw-r--r--   0        0        0     2136 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/README.md
+-rw-r--r--   0        0        0      517 2024-05-20 19:35:26.142370 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/build/asset-manifest.json
+-rw-r--r--   0        0        0     3870 2024-05-20 19:34:56.150973 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/build/favicon.ico
+-rw-r--r--   0        0        0      654 2024-05-20 19:35:26.142370 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/build/index.html
+-rw-r--r--   0        0        0      306 2024-05-20 19:34:56.150973 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/build/manifest.json
+-rw-r--r--   0        0        0       67 2024-05-20 19:34:56.150973 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/build/robots.txt
+-rw-r--r--   0        0        0    18033 2024-05-20 19:35:26.170373 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/build/static/css/main.8ddb8b68.css
+-rw-r--r--   0        0        0    46655 2024-05-20 19:35:26.170373 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/build/static/css/main.8ddb8b68.css.map
+-rw-r--r--   0        0        0     4518 2024-05-20 19:35:26.170373 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/build/static/js/787.095790c7.chunk.js
+-rw-r--r--   0        0        0    10597 2024-05-20 19:35:26.170373 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/build/static/js/787.095790c7.chunk.js.map
+-rw-r--r--   0        0        0  3614868 2024-05-20 19:35:26.142370 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js
+-rw-r--r--   0        0        0     3456 2024-05-20 19:35:26.170373 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js.LICENSE.txt
+-rw-r--r--   0        0        0 13934230 2024-05-20 19:35:26.170373 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js.map
+-rw-r--r--   0        0        0  1408324 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/package-lock.json
+-rw-r--r--   0        0        0     2249 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/package.json
+-rw-r--r--   0        0        0     3870 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/public/favicon.ico
+-rw-r--r--   0        0        0     1324 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/public/index.html
+-rw-r--r--   0        0        0      306 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/public/manifest.json
+-rw-r--r--   0        0        0       67 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/public/robots.txt
+-rw-r--r--   0        0        0     2443 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/App.css
+-rw-r--r--   0        0        0     1143 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/App.js
+-rw-r--r--   0        0        0      273 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/App.test.tsx
+-rw-r--r--   0        0        0     1675 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/AtomsItem.js
+-rw-r--r--   0        0        0       94 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/Data.js
+-rw-r--r--   0        0        0      106 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/DataNode.js
+-rw-r--r--   0        0        0      505 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/DataNodeItem.css
+-rw-r--r--   0        0        0     1458 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/DataNodeItem.tsx
+-rw-r--r--   0        0        0     5593 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/DataNodeTable.js
+-rw-r--r--   0        0        0      116 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/Home.js
+-rw-r--r--   0        0        0     1324 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/Layout.css
+-rw-r--r--   0        0        0     1067 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/Layout.js
+-rw-r--r--   0        0        0     5792 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/NodeDetails.js
+-rw-r--r--   0        0        0     2784 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/Settings.js
+-rw-r--r--   0        0        0     1025 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/WorkGraphDetail.js
+-rw-r--r--   0        0        0     2631 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/WorkGraphDuration.js
+-rw-r--r--   0        0        0     1129 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/WorkGraphIndicator.js
+-rw-r--r--   0        0        0     8796 2024-05-29 19:56:49.086499 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/WorkGraphItem.tsx
+-rw-r--r--   0        0        0     1064 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/WorkGraphItemStyles.ts
+-rw-r--r--   0        0        0      837 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/WorkGraphLog.js
+-rw-r--r--   0        0        0     3434 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/WorkGraphSummary.js
+-rw-r--r--   0        0        0      990 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/WorkGraphTable.css
+-rw-r--r--   0        0        0     7518 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/WorkGraphTable.js
+-rw-r--r--   0        0        0      366 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/index.css
+-rw-r--r--   0        0        0      554 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/index.tsx
+-rw-r--r--   0        0        0     6007 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/logo.svg
+-rw-r--r--   0        0        0       40 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/react-app-env.d.ts
+-rw-r--r--   0        0        0      425 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/reportWebVitals.ts
+-rw-r--r--   0        0        0      160 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/rete.css
+-rw-r--r--   0        0        0     2787 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/rete/customization.ts
+-rw-r--r--   0        0        0      813 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/rete/customization/CustomConnection.tsx
+-rw-r--r--   0        0        0     4981 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/rete/customization/CustomNode.tsx
+-rw-r--r--   0        0        0      566 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/rete/customization/CustomSocket.tsx
+-rw-r--r--   0        0        0      540 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/rete/customization/StyledNode.tsx
+-rw-r--r--   0        0        0      602 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/rete/customization/background.css
+-rw-r--r--   0        0        0      378 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/rete/customization/custom-background.ts
+-rw-r--r--   0        0        0       94 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/rete/customization/vars.ts
+-rw-r--r--   0        0        0     4864 2024-05-04 20:38:47.853168 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/rete/default.ts
+-rw-r--r--   0        0        0      603 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/rete/index.ts
+-rw-r--r--   0        0        0      241 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/setupTests.ts
+-rw-r--r--   0        0        0      535 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/tsconfig.json
+-rw-r--r--   0        0        0       94 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.7/aiida_workgraph/widget/.gitignore
+-rw-r--r--   0        0        0      488 2024-04-13 07:05:41.907170 aiida_workgraph-0.2.7/aiida_workgraph/widget/.ipynb_checkpoints/example-checkpoint.ipynb
+-rw-r--r--   0        0        0      552 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.7/aiida_workgraph/widget/README.md
+-rw-r--r--   0        0        0       71 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.7/aiida_workgraph/widget/__init__.py
+-rw-r--r--   0        0        0     7122 2024-05-29 13:43:34.925274 aiida_workgraph-0.2.7/aiida_workgraph/widget/js/default_rete.ts
+-rw-r--r--   0        0        0      565 2024-04-22 20:35:00.919099 aiida_workgraph-0.2.7/aiida_workgraph/widget/js/widget.css
+-rw-r--r--   0        0        0     5905 2024-04-22 20:35:00.919099 aiida_workgraph-0.2.7/aiida_workgraph/widget/js/widget.tsx
+-rw-r--r--   0        0        0   148687 2024-04-22 20:35:00.923099 aiida_workgraph-0.2.7/aiida_workgraph/widget/package-lock.json
+-rw-r--r--   0        0        0      851 2024-04-22 20:35:00.923099 aiida_workgraph-0.2.7/aiida_workgraph/widget/package.json
+-rw-r--r--   0        0        0      765 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.7/aiida_workgraph/widget/pyproject.toml
+-rw-r--r--   0        0        0     2770 2024-05-30 05:13:07.073987 aiida_workgraph-0.2.7/aiida_workgraph/widget/src/widget/__init__.py
+-rw-r--r--   0        0        0    10332 2024-05-30 07:12:32.597910 aiida_workgraph-0.2.7/aiida_workgraph/widget/src/widget/html_template.py
+-rw-r--r--   0        0        0      429 2024-05-20 19:36:16.932122 aiida_workgraph-0.2.7/aiida_workgraph/widget/src/widget/static/widget.css
+-rw-r--r--   0        0        0  1796776 2024-05-20 19:36:16.932122 aiida_workgraph-0.2.7/aiida_workgraph/widget/src/widget/static/widget.js
+-rw-r--r--   0        0        0      897 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.7/aiida_workgraph/widget/src/widget/utils.py
+-rw-r--r--   0        0        0      453 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.7/aiida_workgraph/widget/tsconfig.json
+-rw-r--r--   0        0        0    15395 2024-05-31 11:20:56.734414 aiida_workgraph-0.2.7/aiida_workgraph/workgraph.py
+-rw-r--r--   0        0        0     3216 2024-05-23 10:17:58.548150 aiida_workgraph-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     7359 1970-01-01 00:00:00.000000 aiida_workgraph-0.2.7/PKG-INFO
```

### Comparing `aiida_workgraph-0.2.6/LICENSE` & `aiida_workgraph-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/README.md` & `aiida_workgraph-0.2.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 [![PyPI version](https://badge.fury.io/py/aiida-workgraph.svg)](https://badge.fury.io/py/aiida-workgraph)
 [![Unit test](https://github.com/superstar54/aiida-workgraph/actions/workflows/ci.yaml/badge.svg)](https://github.com/superstar54/aiida-workgraph/actions/workflows/ci.yaml)
 [![codecov](https://codecov.io/gh/superstar54/aiida-workgraph/branch/main/graph/badge.svg)](https://codecov.io/gh/superstar54/aiida-workgraph)
 [![Docs status](https://readthedocs.org/projects/aiida-workgraph/badge)](http://aiida-workgraph.readthedocs.io/)
 
 Provides the third workflow component: `WorkGraph`, to design flexible node-based workflows using AiiDA.
 
+
 In AiiDA, there are two workflow components: `workfunction` and `WorkChain`. Workfunction is easy to implement but it does not support automatic checkpointing, which is important for long-running calculations. Workchain supports automatic checkpointing but it is difficult to implement and also not as flexible as the `workfunction`. AiiDA-WorkGraph provides the third component: `WorkGraph`. It is easy to implement and supports automatic checkpointing. It is also flexible and can be used to design complex workflows.
 
 
 Here is a detailed comparison between the ``WorkGraph`` with two AiiDA built-in workflow components.
 
 
 | Aspect                   | WorkFunction           | WorkChain                     | WorkGraph               |
```

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/calculations/python.py` & `aiida_workgraph-0.2.7/aiida_workgraph/calculations/python.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from __future__ import annotations
 
 import pathlib
 import typing as t
 
 from aiida.common.datastructures import CalcInfo, CodeInfo
 from aiida.common.folders import Folder
+from aiida.common.extendeddicts import AttributeDict
 from aiida.engine import CalcJob, CalcJobProcessSpec
 from aiida.orm import (
     Data,
     SinglefileData,
     Str,
     List,
     FolderData,
@@ -20,18 +21,14 @@
 
 __all__ = ("PythonJob",)
 
 
 class PythonJob(CalcJob):
     """Calcjob to run a Python function on a remote computer."""
 
-    # Default name of the subfolder that you want to create in the working directory,
-    # in which you want to place the files taken from parent_folder
-    _PARENT_SUBFOLDER = "./parent_folder/"
-
     _internal_retrieve_list = []
     _retrieve_singlefile_list = []
     _retrieve_temporary_list = []
 
     _DEFAULT_INPUT_FILE = "script.py"
     _DEFAULT_OUTPUT_FILE = "aiida.out"
 
@@ -50,37 +47,58 @@
             serializer=to_aiida_type,
             required=False,
         )
         spec.input(
             "function_name", valid_type=Str, serializer=to_aiida_type, required=False
         )
         spec.input_namespace(
-            "kwargs", valid_type=Data, required=False
-        )  # , serializer=general_serializer)
+            "function_kwargs", valid_type=Data, required=False
+        )  # , serializer=serialize_to_aiida_nodes)
         spec.input(
             "output_name_list",
             valid_type=List,
             required=False,
             serializer=to_aiida_type,
             help="The names of the output ports",
         )
         spec.input(
             "parent_folder",
             valid_type=(RemoteData, FolderData, SinglefileData),
             required=False,
             help="Use a local or remote folder as parent folder (for restarts and similar)",
         )
         spec.input(
+            "parent_folder_name",
+            valid_type=Str,
+            default=lambda: Str("./parent_folder/"),
+            required=False,
+            serializer=to_aiida_type,
+            help="""Default name of the subfolder that you want to create in the working directory,
+            in which you want to place the files taken from parent_folder""",
+        )
+        spec.input(
             "parent_output_folder",
             valid_type=Str,
             default=None,
             required=False,
             serializer=to_aiida_type,
             help="Name of the subfolder inside 'parent_folder' from which you want to copy the files",
         )
+        spec.input_namespace(
+            "upload_files",
+            valid_type=(FolderData, SinglefileData),
+            required=False,
+            help="The folder/files to upload",
+        )
+        spec.input_namespace(
+            "copy_files",
+            valid_type=(RemoteData,),
+            required=False,
+            help="The folder/files to copy from the remote computer",
+        )
         spec.input(
             "additional_retrieve_list",
             valid_type=List,
             default=None,
             required=False,
             serializer=to_aiida_type,
             help="The names of the files to retrieve",
@@ -125,16 +143,16 @@
         :returns: A :class:`aiida.common.datastructures.CalcInfo` instance.
         """
         import cloudpickle as pickle
 
         dirpath = pathlib.Path(folder._abspath)
         inputs: dict[str, t.Any]
 
-        if self.inputs.kwargs:
-            inputs = dict(self.inputs.kwargs)
+        if self.inputs.function_kwargs:
+            inputs = dict(self.inputs.function_kwargs)
         else:
             inputs = {}
         # get the value of pickled function
         function_source_code = self.inputs.function_source_code.value
         # create python script to run the function
         script = f"""
 import pickle
@@ -167,40 +185,74 @@
 
         if source is not None:
             if isinstance(source, RemoteData):
                 dirpath = pathlib.Path(source.get_remote_path())
                 if self.inputs.parent_output_folder is not None:
                     dirpath = (
                         pathlib.Path(source.get_remote_path())
-                        / self.inputs.parent_output_folder
+                        / self.inputs.parent_output_folder.value
                     )
                 remote_list.append(
-                    (source.computer.uuid, str(dirpath), self._PARENT_SUBFOLDER)
+                    (
+                        source.computer.uuid,
+                        str(dirpath),
+                        self.inputs.parent_folder_name.value,
+                    )
                 )
             elif isinstance(source, FolderData):
                 dirname = (
                     self.inputs.parent_output_folder.value
                     if self.inputs.parent_output_folder is not None
                     else ""
                 )
-                local_copy_list.append((source.uuid, dirname, self._PARENT_SUBFOLDER))
+                local_copy_list.append(
+                    (source.uuid, dirname, self.inputs.parent_folder_name.value)
+                )
             elif isinstance(source, SinglefileData):
                 local_copy_list.append((source.uuid, source.filename, source.filename))
+        if self.inputs.upload_files:
+            upload_files = self.inputs.upload_files
+            for key, source in upload_files.items():
+                # replace "_dot_" with "." in the key
+                key = key.replace("_dot_", ".")
+                if isinstance(source, FolderData):
+                    local_copy_list.append((source.uuid, "", key))
+                elif isinstance(source, SinglefileData):
+                    local_copy_list.append(
+                        (source.uuid, source.filename, source.filename)
+                    )
+                else:
+                    raise ValueError(
+                        f"""Input folder/file: {source} is not supported.
+Only AiiDA SinglefileData and FolderData are allowed."""
+                    )
+        if "copy_files" in self.inputs:
+            copy_files = self.inputs.copy_files
+            for key, source in copy_files.items():
+                # replace "_dot_" with "." in the key
+                key = key.replace("_dot_", ".")
+                dirpath = pathlib.Path(source.get_remote_path())
+                remote_list.append((source.computer.uuid, str(dirpath), key))
         # create pickle file for the inputs
         input_values = {}
         for key, value in inputs.items():
             if isinstance(value, Data) and hasattr(value, "value"):
                 # get the value of the pickled data
                 input_values[key] = value.value
+            # TODO: should check this recursively
+            elif isinstance(value, (AttributeDict, dict)):
+                # if the value is an AttributeDict, use recursively
+                input_values[key] = {k: v.value for k, v in value.items()}
             else:
                 raise ValueError(
                     f"Input data {value} is not supported. Only AiiDA data Node with a value attribute is allowed. "
                 )
         # save the value as a pickle file, the path is absolute
         filename = "inputs.pickle"
+        dirpath = pathlib.Path(folder._abspath)
         with folder.open(filename, "wb") as handle:
             pickle.dump(input_values, handle)
             # create a singlefiledata object for the pickled data
             file_data = SinglefileData(file=f"{dirpath}/{filename}")
             local_copy_list.append((file_data.uuid, file_data.filename, filename))
 
         codeinfo = CodeInfo()
```

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/cli/cmd_graph.py` & `aiida_workgraph-0.2.7/aiida_workgraph/cli/cmd_graph.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/cli/cmd_web.py` & `aiida_workgraph-0.2.7/aiida_workgraph/cli/cmd_web.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/cli/cmd_workgraph.py` & `aiida_workgraph-0.2.7/aiida_workgraph/cli/cmd_workgraph.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/cli/query_workgraph.py` & `aiida_workgraph-0.2.7/aiida_workgraph/cli/query_workgraph.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/collection.py` & `aiida_workgraph-0.2.7/aiida_workgraph/collection.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,25 +15,33 @@
         uuid: Optional[str] = None,
         on_remote: Optional[bool] = False,
         **kwargs: Any
     ) -> Any:
         from aiida_workgraph.decorator import (
             build_node_from_callable,
             build_PythonJob_node,
+            build_ShellJob_node,
         )
 
         # build the node on the fly if the identifier is a callable
         if callable(identifier):
             identifier = build_node_from_callable(identifier)
             if kwargs.pop("run_remotely", False):
+                if identifier.node.node_type.upper() == "GRAPH_BUILDER":
+                    raise ValueError(
+                        "GraphBuilder nodes cannot be run remotely. Please set run_remotely=False."
+                    )
                 # this is a PythonJob
-                identifier = build_PythonJob_node(identifier)
+                identifier, _ = build_PythonJob_node(identifier)
         if isinstance(identifier, str) and identifier.upper() == "PYTHONJOB":
             # copy the inputs and outputs from the function node to the PythonJob node
-            identifier = build_PythonJob_node(kwargs.pop("function"))
+            identifier, _ = build_PythonJob_node(kwargs.pop("function"))
+        if isinstance(identifier, str) and identifier.upper() == "SHELLJOB":
+            # copy the inputs and outputs from the function node to the SHELLJob node
+            identifier, _ = build_ShellJob_node(kwargs.pop("add_outputs", None))
         # Call the original new method
         return super().new(identifier, name, uuid, **kwargs)
 
 
 class WorkGraphPropertyCollection(PropertyCollection):
     def new(
         self,
```

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/decorator.py` & `aiida_workgraph-0.2.7/aiida_workgraph/decorator.py`

 * *Files 10% similar despite different names*

```diff
@@ -226,14 +226,15 @@
     executor = {
         "executor": pickle.dumps(executor),
         "type": ndata["node_type"],
         "is_pickle": True,
     }
     ndata["executor"] = executor
     node = create_node(ndata)
+    node.is_aiida_component = True
     return node, ndata
 
 
 def build_PythonJob_node(func: Callable) -> Node:
     """Build PythonJob node from function."""
     from aiida_workgraph.calculations.python import PythonJob
     from copy import deepcopy
@@ -255,23 +256,57 @@
     outputs = ndata["outputs"]
     for input in ndata_py["inputs"]:
         if input not in inputs:
             inputs.append(input)
     for output in ndata_py["outputs"]:
         if output not in outputs:
             outputs.append(output)
+    # change "copy_files" link_limit to 1e6
+    for input in inputs:
+        if input[1] == "copy_files":
+            input[2].update({"link_limit": 1e6})
     # append the kwargs of the PythonJob node to the function node
     kwargs = ndata["kwargs"]
     kwargs.extend(["computer", "code_label", "code_path", "prepend_text"])
     kwargs.extend(ndata_py["kwargs"])
     ndata["inputs"] = inputs
     ndata["outputs"] = outputs
     ndata["kwargs"] = kwargs
     ndata["node_type"] = "PYTHONJOB"
-    return create_node(ndata)
+    node = create_node(ndata)
+    node.is_aiida_component = True
+    return node, ndata
+
+
+def build_ShellJob_node(outputs=None) -> Node:
+    """Build PythonJob node from function."""
+    from aiida_shell.calculations.shell import ShellJob
+
+    ndata = {"executor": ShellJob, "node_type": "CALCJOB"}
+    _, ndata = build_node_from_AiiDA(ndata)
+    # Extend the outputs
+    ndata["outputs"].extend([["General", "stdout"], ["General", "stderr"]])
+    outputs = [] if outputs is None else outputs
+    # add user defined outputs
+    for output in outputs:
+        if output not in ndata["outputs"]:
+            ndata["outputs"].append(output)
+    #
+    ndata["identifier"] = "ShellJob"
+    ndata["inputs"].extend(
+        [
+            ["General", "command"],
+            ["General", "resolve_command"],
+        ]
+    )
+    ndata["kwargs"].extend(["command", "resolve_command"])
+    ndata["node_type"] = "SHELLJOB"
+    node = create_node(ndata)
+    node.is_aiida_component = True
+    return node, ndata
 
 
 def build_node_from_workgraph(wg: any) -> Node:
     """Build node from workgraph."""
     from aiida_workgraph.node import Node
 
     ndata = {"node_type": "workgraph"}
@@ -296,15 +331,14 @@
                 [f"{node.name}.{socket.name}", f"{node.name}.{socket.name}"]
             )
     kwargs = [input[1] for input in inputs]
     # add built-in sockets
     outputs.append(["General", "_outputs"])
     outputs.append(["General", "_wait"])
     inputs.append(["General", "_wait", {"link_limit": 1e6}])
-    inputs.append(["General", "_code"])
     ndata["node_class"] = Node
     ndata["kwargs"] = kwargs
     ndata["inputs"] = inputs
     ndata["outputs"] = outputs
     ndata["identifier"] = wg.name
     # TODO In order to reload the WorkGraph from process, "is_pickle" should be True
     # so I pickled the function here, but this is not necessary
@@ -317,30 +351,82 @@
     }
     ndata["executor"] = executor
     node = create_node(ndata)
     node.group_outputs = group_outputs
     return node
 
 
+def get_required_imports(func):
+    """Retrieve type hints and the corresponding module"""
+    from typing import get_type_hints, _SpecialForm
+
+    type_hints = get_type_hints(func)
+    imports = {}
+
+    def add_imports(type_hint):
+        if isinstance(
+            type_hint, _SpecialForm
+        ):  # Handle special forms like Any, Union, Optional
+            module_name = "typing"
+            type_name = type_hint._name or str(type_hint)
+        elif hasattr(
+            type_hint, "__origin__"
+        ):  # This checks for higher-order types like List, Dict
+            module_name = type_hint.__module__
+            type_name = type_hint._name
+            for arg in type_hint.__args__:
+                if arg is type(None):  # noqa: E721
+                    continue
+                add_imports(arg)  # Recursively add imports for each argument
+        elif hasattr(type_hint, "__module__"):
+            module_name = type_hint.__module__
+            type_name = type_hint.__name__
+        else:
+            return  # If no module or origin, we can't import it, e.g., for literals
+
+        if module_name not in imports:
+            imports[module_name] = set()
+        imports[module_name].add(type_name)
+
+    for _, type_hint in type_hints.items():
+        add_imports(type_hint)
+
+    return imports
+
+
 def serialize_function(func: Callable) -> Dict[str, Any]:
     """Serialize a function for storage or transmission."""
     import cloudpickle as pickle
     import inspect
     import textwrap
 
     source_code = inspect.getsource(func)
     source_code_lines = source_code.split("\n")
+    # we need save the source code explicitly, because in the case of jupyter notebook,
+    # the source code is not saved in the pickle file
     function_source_code = "\n".join(source_code_lines[1:])
     function_source_code = textwrap.dedent(function_source_code)
-
+    # we also need to include the necessary imports for the types used in the type hints.
+    try:
+        required_imports = get_required_imports(func)
+    except Exception as e:
+        required_imports = {}
+        print(f"Failed to get required imports for function {func.__name__}: {e}")
+    # Generate import statements
+    import_statements = "\n".join(
+        f"from {module} import {', '.join(types)}"
+        for module, types in required_imports.items()
+    )
     return {
         "executor": pickle.dumps(func),
         "type": "function",
         "is_pickle": True,
+        "function_name": func.__name__,
         "function_source_code": function_source_code,
+        "import_statements": import_statements,
     }
 
 
 def generate_ndata(
     func: Callable,
     identifier: str,
     inputs: List[Tuple[str, str]],
@@ -356,16 +442,14 @@
 
     args, kwargs, var_args, var_kwargs, _inputs = generate_input_sockets(
         func, inputs, properties
     )
     node_outputs = outputs
     # add built-in sockets
     _inputs.append(["General", "_wait", {"link_limit": 1e6}])
-    _inputs.append(["General", "_code"])
-    kwargs.append("_code")
     node_outputs.append(["General", "_wait"])
     node_outputs.append(["General", "_outputs"])
     ndata = {
         "node_class": Node,
         "identifier": identifier,
         "args": args,
         "kwargs": kwargs,
```

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/engine/workgraph.py` & `aiida_workgraph-0.2.7/aiida_workgraph/engine/workgraph.py`

 * *Files 6% similar despite different names*

```diff
@@ -390,25 +390,28 @@
         # try to resume the workgraph, if the workgraph is already resumed
         # by other awaitable, this will not work
         try:
             self.resume()
         except Exception as e:
             print(e)
 
+    def _build_process_label(self) -> str:
+        """Use the workgraph name as the process label."""
+        return f"WorkGraph<{self.inputs.wg['name']}>"
+
     def setup(self) -> None:
         # track if the awaitable callback is added to the runner
         self.ctx._awaitable_actions = []
         self.ctx.new_data = dict()
         self.ctx.input_nodes = dict()
         # read the latest workgraph data
         wgdata = self.read_wgdata_from_base()
         self.init_ctx(wgdata)
         #
         self.ctx.msgs = []
-        self.node.set_process_label(f"WorkGraph: {self.ctx.workgraph['name']}")
         self.ctx._execution_count = 0
         # init node results
         self.set_node_results()
         # while workgraph
         if self.ctx.workgraph["workgraph_type"].upper() == "WHILE":
             self.ctx._max_iteration = self.ctx.workgraph.get("max_iteration", 1000)
             should_run = self.check_while_conditions()
@@ -570,14 +573,15 @@
                 "CALCFUNCTION",
                 "WORKFUNCTION",
                 "CALCJOB",
                 "WORKCHAIN",
                 "GRAPH_BUILDER",
                 "WORKGRAPH",
                 "PYTHONJOB",
+                "SHELLJOB",
             ]
             and node["state"] == "RUNNING"
         ):
             self.set_node_result(node)
 
     def is_workgraph_finished(self) -> bool:
         """Check if the workgraph is finished.
@@ -677,14 +681,15 @@
             node = self.ctx.nodes[name]
             if node["metadata"]["node_type"].upper() in [
                 "CALCJOB",
                 "WORKCHAIN",
                 "GRAPH_BUILDER",
                 "WORKGRAPH",
                 "PYTHONJOB",
+                "SHELLJOB",
             ]:
                 if len(self._awaitables) > self.ctx.max_number_awaitables:
                     print(
                         MAX_NUMBER_AWAITABLES_MSG.format(
                             self.ctx.max_number_awaitables, name
                         )
                     )
@@ -695,17 +700,17 @@
             executor, _ = get_executor(node["executor"])
             print("executor: ", executor)
             args, kwargs, var_args, var_kwargs, args_dict = self.get_inputs(node)
             for i, key in enumerate(self.ctx.nodes[name]["metadata"]["args"]):
                 kwargs[key] = args[i]
             # update the port namespace
             kwargs = update_nested_dict_with_special_keys(kwargs)
-            # print("args: ", args)
-            # print("kwargs: ", kwargs)
-            # print("var_kwargs: ", var_kwargs)
+            print("args: ", args)
+            print("kwargs: ", kwargs)
+            print("var_kwargs: ", var_kwargs)
             # kwargs["meta.label"] = name
             # output must be a Data type or a mapping of {string: Data}
             node["results"] = {}
             if node["metadata"]["node_type"].upper() == "NODE":
                 print("node  type: node.")
                 results = self.run_executor(executor, [], kwargs, var_args, var_kwargs)
                 node["process"] = results
@@ -789,86 +794,50 @@
                 wg.save(metadata={"call_link_label": name})
                 print("submit workgraph: ")
                 process = self.submit(wg.process_inited)
                 node["process"] = process
                 self.ctx.nodes[name]["state"] = "RUNNING"
                 self.to_context(**{name: process})
             elif node["metadata"]["node_type"].upper() in ["WORKGRAPH"]:
-                from aiida_workgraph.utils import merge_properties
+                from .utils import prepare_for_workgraph_node
                 from aiida_workgraph.utils.analysis import WorkGraphSaver
 
-                print("node  type: workgraph.")
-                wgdata = node["executor"]["wgdata"]
-                wgdata["name"] = name
-                wgdata["metadata"]["group_outputs"] = self.ctx.nodes[name]["metadata"][
-                    "group_outputs"
-                ]
-                # update the workgraph data by kwargs
-                for node_name, data in kwargs.items():
-                    # because kwargs is updated using update_nested_dict_with_special_keys
-                    # which means the data is grouped by the node name
-                    for socket_name, value in data.items():
-                        wgdata["nodes"][node_name]["properties"][socket_name][
-                            "value"
-                        ] = value
-                # merge the properties
-                merge_properties(wgdata)
-                metadata = {"call_link_label": name}
-                inputs = {"wg": wgdata, "metadata": metadata}
+                inputs, wgdata = prepare_for_workgraph_node(node, kwargs)
                 process_inited = WorkGraphEngine(inputs=inputs)
                 process_inited.runner.persister.save_checkpoint(process_inited)
                 saver = WorkGraphSaver(process_inited.node, wgdata)
                 saver.save()
                 print("submit workgraph: ")
                 process = self.submit(process_inited)
                 node["process"] = process
                 self.ctx.nodes[name]["state"] = "RUNNING"
                 self.to_context(**{name: process})
             elif node["metadata"]["node_type"].upper() in ["PYTHONJOB"]:
                 from aiida_workgraph.calculations.python import PythonJob
-                from aiida_workgraph.orm.serializer import general_serializer
-                from aiida_workgraph.utils import get_or_create_code
+                from .utils import prepare_for_pythonjob
 
-                print("node  type: Python.")
-                # normal function does not have a process
-                code = kwargs.pop("code", None)
-                computer = kwargs.pop("computer", None)
-                code_label = kwargs.pop("code_label", None)
-                code_path = kwargs.pop("code_path", None)
-                prepend_text = kwargs.pop("prepend_text", None)
-                #
-                if code is None:
-                    code = get_or_create_code(
-                        computer=computer or "localhost",
-                        code_label=code_label or "python3",
-                        code_path=code_path,
-                        prepend_text=prepend_text,
-                    )
-                parent_folder = kwargs.pop("parent_folder", None)
-                metadata = kwargs.pop("metadata", {})
-                metadata.update({"call_link_label": name})
-                # get the source code of the function
-                function_name = executor.__name__
-                function_source_code = node["executor"]["function_source_code"]
-                # outputs
-                output_name_list = [output["name"] for output in node["outputs"]]
-                # serialize the kwargs into AiiDA Data
-                inputs = general_serializer(kwargs)
-                # transfer the args to kwargs
+                inputs = prepare_for_pythonjob(node, kwargs, var_kwargs)
+                # since aiida 2.5.0, we can pass inputs directly to the submit, no need to use **inputs
                 process = self.submit(
                     PythonJob,
-                    inputs={
-                        "function_source_code": orm.Str(function_source_code),
-                        "function_name": orm.Str(function_name),
-                        "code": code,
-                        "kwargs": inputs,
-                        "output_name_list": orm.List(output_name_list),
-                        "parent_folder": parent_folder,
-                        "metadata": metadata,
-                    },
+                    **inputs,
+                )
+                process.label = name
+                node["process"] = process
+                self.ctx.nodes[name]["state"] = "RUNNING"
+                self.to_context(**{name: process})
+            elif node["metadata"]["node_type"].upper() in ["SHELLJOB"]:
+                from aiida_shell.calculations.shell import ShellJob
+                from .utils import prepare_for_shelljob
+
+                inputs = prepare_for_shelljob(node, kwargs)
+                # since aiida 2.5.0, we can pass inputs directly to the submit, no need to use **inputs
+                process = self.submit(
+                    ShellJob,
+                    **inputs,
                 )
                 process.label = name
                 node["process"] = process
                 self.ctx.nodes[name]["state"] = "RUNNING"
                 self.to_context(**{name: process})
             elif node["metadata"]["node_type"].upper() in ["NORMAL"]:
                 print("node  type: Normal.")
```

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/executors/builtin.py` & `aiida_workgraph-0.2.7/aiida_workgraph/executors/builtin.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/executors/qe.py` & `aiida_workgraph-0.2.7/aiida_workgraph/executors/qe.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/executors/test.py` & `aiida_workgraph-0.2.7/aiida_workgraph/executors/test.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/node.py` & `aiida_workgraph-0.2.7/aiida_workgraph/node.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
     The class extends from node_graph.node.Node and add new
     attributes to it.
     """
 
     property_pool = property_pool
     socket_pool = socket_pool
+    is_aiida_component = False
 
     def __init__(
         self,
         to_context: Optional[List[Any]] = None,
         wait: List[Union[str, GraphNode]] = [],
         process: Optional[aiida.orm.ProcessNode] = None,
         pk: Optional[int] = None,
@@ -40,25 +41,26 @@
         )
         self.to_context = [] if to_context is None else to_context
         self.wait = [] if wait is None else wait
         self.process = process
         self.pk = pk
         self._widget = NodeGraphWidget(
             settings={"minmap": False},
-            style={"width": "40%", "height": "600px"},
+            style={"width": "80%", "height": "600px"},
         )
 
     def to_dict(self) -> Dict[str, Any]:
         ndata = super().to_dict()
         ndata["to_context"] = [] if self.to_context is None else self.to_context
         ndata["wait"] = [
             node if isinstance(node, str) else node.name for node in self.wait
         ]
         ndata["process"] = self.process.uuid if self.process else None
         ndata["metadata"]["pk"] = self.process.pk if self.process else None
+        ndata["metadata"]["is_aiida_component"] = self.is_aiida_component
 
         return ndata
 
     def set_from_protocol(self, *args: Any, **kwargs: Any) -> None:
         """For node support protocol, set the node from protocol data."""
         from aiida_workgraph.utils import get_executor, get_dict_from_builder
 
@@ -105,7 +107,12 @@
     def _repr_mimebundle_(self, *args: Any, **kwargs: Any) -> any:
         # if ipywdigets > 8.0.0, use _repr_mimebundle_ instead of _ipython_display_
         self._widget.from_node(self)
         if hasattr(self._widget, "_repr_mimebundle_"):
             return self._widget._repr_mimebundle_(*args, **kwargs)
         else:
             return self._widget._ipython_display_(*args, **kwargs)
+
+    def to_html(self, output: str = None, **kwargs):
+        """Write a standalone html file to visualize the node."""
+        self._widget.from_node(self)
+        return self._widget.to_html(output=output, **kwargs)
```

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/nodes/__init__.py` & `aiida_workgraph-0.2.7/aiida_workgraph/nodes/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from node_graph.utils import get_entries
-from .builtin import AiiDAGather, AiiDAToCtx, AiiDAFromCtx, AiiDAShell
+from .builtin import AiiDAGather, AiiDAToCtx, AiiDAFromCtx
 from .test import (
     AiiDAInt,
     AiiDAFloat,
     AiiDAString,
     AiiDAList,
     AiiDADict,
     AiiDANode,
@@ -19,15 +19,14 @@
     AiiDAStructure,
 )
 
 node_list = [
     AiiDAGather,
     AiiDAToCtx,
     AiiDAFromCtx,
-    AiiDAShell,
     AiiDAInt,
     AiiDAFloat,
     AiiDAString,
     AiiDAList,
     AiiDADict,
     AiiDANode,
     AiiDACode,
```

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/nodes/qe.py` & `aiida_workgraph-0.2.7/aiida_workgraph/nodes/qe.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/nodes/test.py` & `aiida_workgraph-0.2.7/aiida_workgraph/nodes/test.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/orm/atoms.py` & `aiida_workgraph-0.2.7/aiida_workgraph/orm/atoms.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/orm/general_data.py` & `aiida_workgraph-0.2.7/aiida_workgraph/orm/general_data.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/orm/worktree.py` & `aiida_workgraph-0.2.7/aiida_workgraph/orm/worktree.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/properties/built_in.py` & `aiida_workgraph-0.2.7/aiida_workgraph/properties/built_in.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/property.py` & `aiida_workgraph-0.2.7/aiida_workgraph/property.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/socket.py` & `aiida_workgraph-0.2.7/aiida_workgraph/socket.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/sockets/built_in.py` & `aiida_workgraph-0.2.7/aiida_workgraph/sockets/built_in.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/utils/__init__.py` & `aiida_workgraph-0.2.7/aiida_workgraph/utils/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -261,7 +261,31 @@
             filepath_executable=code_path,
             default_calc_job_plugin="workgraph.python",
             prepend_text=prepend_text,
         )
 
         code.store()
         return code
+
+
+def serialize_pythonjob_properties(wgdata):
+    """Serialize the PythonJob properties."""
+    from aiida_workgraph.orm.serializer import general_serializer
+
+    for _, node in wgdata["nodes"].items():
+        if not node["metadata"]["node_type"].upper() == "PYTHONJOB":
+            continue
+        # get the names kwargs for the PythonJob, which are the inputs before _wait
+        input_kwargs = []
+        for input in node["inputs"]:
+            if input["name"] == "_wait":
+                break
+            input_kwargs.append(input["name"])
+        for name in input_kwargs:
+            prop = node["properties"][name]
+            # if value is not None, not {}
+            if not (
+                prop["value"] is None
+                or isinstance(prop["value"], dict)
+                and prop["value"] == {}
+            ):
+                prop["value"] = general_serializer(prop["value"])
```

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/utils/analysis.py` & `aiida_workgraph-0.2.7/aiida_workgraph/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/utils/graph.py` & `aiida_workgraph-0.2.7/aiida_workgraph/utils/graph.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/README.md` & `aiida_workgraph-0.2.7/aiida_workgraph/web/README.md`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/backend/app/api.py` & `aiida_workgraph-0.2.7/aiida_workgraph/web/backend/app/api.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/backend/app/daemon.py` & `aiida_workgraph-0.2.7/aiida_workgraph/web/backend/app/daemon.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/backend/app/datanode.py` & `aiida_workgraph-0.2.7/aiida_workgraph/web/backend/app/datanode.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/backend/app/utils.py` & `aiida_workgraph-0.2.7/aiida_workgraph/web/backend/app/utils.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/backend/app/workgraph.py` & `aiida_workgraph-0.2.7/aiida_workgraph/web/backend/app/workgraph.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/README.md` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/README.md`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/asset-manifest.json` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/favicon.ico` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/index.html` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/static/css/main.8ddb8b68.css` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/build/static/css/main.8ddb8b68.css`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/static/css/main.8ddb8b68.css.map` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/build/static/css/main.8ddb8b68.css.map`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/static/js/787.095790c7.chunk.js` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/build/static/js/787.095790c7.chunk.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/static/js/787.095790c7.chunk.js.map` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/build/static/js/787.095790c7.chunk.js.map`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js.LICENSE.txt` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js.map` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js.map`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/package-lock.json` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/package.json` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/package.json`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/public/favicon.ico` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/public/index.html` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/public/index.html`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/App.css` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/App.css`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/App.js` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/App.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/AtomsItem.js` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/AtomsItem.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/DataNodeItem.tsx` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/DataNodeItem.tsx`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/DataNodeTable.js` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/DataNodeTable.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/Layout.css` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/Layout.css`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/Layout.js` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/Layout.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/NodeDetails.js` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/NodeDetails.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/Settings.js` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/Settings.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphDetail.js` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/WorkGraphDetail.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphDuration.js` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/WorkGraphDuration.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphIndicator.js` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/WorkGraphIndicator.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphItem.tsx` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/WorkGraphItem.tsx`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphItemStyles.ts` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/WorkGraphItemStyles.ts`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphLog.js` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/WorkGraphLog.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphSummary.js` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/WorkGraphSummary.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphTable.css` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/WorkGraphTable.css`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphTable.js` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/components/WorkGraphTable.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/index.tsx` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/index.tsx`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/logo.svg` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/logo.svg`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/customization.ts` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/rete/customization.ts`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/customization/CustomConnection.tsx` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/rete/customization/CustomConnection.tsx`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/customization/CustomNode.tsx` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/rete/customization/CustomNode.tsx`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/customization/CustomSocket.tsx` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/rete/customization/CustomSocket.tsx`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/customization/StyledNode.tsx` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/rete/customization/StyledNode.tsx`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/customization/background.css` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/rete/customization/background.css`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/default.ts` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/rete/default.ts`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/index.ts` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/src/rete/index.ts`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/tsconfig.json` & `aiida_workgraph-0.2.7/aiida_workgraph/web/frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/widget/README.md` & `aiida_workgraph-0.2.7/aiida_workgraph/widget/README.md`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/widget/js/default_rete.ts` & `aiida_workgraph-0.2.7/aiida_workgraph/widget/js/default_rete.ts`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/widget/js/widget.css` & `aiida_workgraph-0.2.7/aiida_workgraph/widget/js/widget.css`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/widget/js/widget.tsx` & `aiida_workgraph-0.2.7/aiida_workgraph/widget/js/widget.tsx`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/widget/package-lock.json` & `aiida_workgraph-0.2.7/aiida_workgraph/widget/package-lock.json`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/widget/package.json` & `aiida_workgraph-0.2.7/aiida_workgraph/widget/package.json`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/widget/pyproject.toml` & `aiida_workgraph-0.2.7/aiida_workgraph/widget/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/widget/src/widget/__init__.py` & `aiida_workgraph-0.2.7/aiida_workgraph/widget/src/widget/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -40,17 +40,35 @@
     def from_node(self, node: Any) -> None:
         ndata = node.to_dict()
         ndata.pop("properties", None)
         ndata.pop("executor", None)
         ndata.pop("node_class", None)
         ndata.pop("process", None)
         ndata["label"] = ndata["metadata"]["identifier"]
-        wgdata = {"nodes": {node.name: ndata}, "links": []}
+        wgdata = {"name": node.name, "nodes": {node.name: ndata}, "links": []}
         self.value = wgdata
 
+    def to_html(self, output: str = None, width: str = "100%", height: str = "600px"):
+        """Write a standalone html file to visualize the workgraph."""
+        from IPython.display import IFrame
+        from .html_template import html_template
+        import json
+
+        if output is None:
+            # create "html" folder if it does not exist
+            pathlib.Path("html").mkdir(exist_ok=True)
+            output = f"html/{self.value['name']}.html"
+        # Replace the placeholder with the actual workgraphData
+        html_content = html_template.replace(
+            "__WORKGRAPH_DATA__", json.dumps(self.value)
+        )
+        with open(output, "w") as f:
+            f.write(html_content)
+        return IFrame(output, width=width, height=height)
+
     @traitlets.observe("positions")
     def _observe_positions(self, change: Dict[str, Any]) -> None:
         if not self.parent:
             return
         if change["new"]:
             for name, pos in change["new"].items():
                 self.parent.nodes[name].position = pos
```

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/widget/src/widget/static/widget.js` & `aiida_workgraph-0.2.7/aiida_workgraph/widget/src/widget/static/widget.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/widget/src/widget/utils.py` & `aiida_workgraph-0.2.7/aiida_workgraph/widget/src/widget/utils.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/aiida_workgraph/workgraph.py` & `aiida_workgraph-0.2.7/aiida_workgraph/workgraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,29 +58,33 @@
 
     def run(self, inputs: Optional[Dict[str, Any]] = None) -> Any:
         """
         Run the AiiDA workgraph process and update the process status. The method uses AiiDA's engine to run
         the process and then calls the update method to update the state of the process.
         """
         from aiida_workgraph.engine.workgraph import WorkGraphEngine
-        from aiida_workgraph.utils import merge_properties
+        from aiida_workgraph.utils import (
+            merge_properties,
+            serialize_pythonjob_properties,
+        )
 
         # set node inputs
         if inputs is not None:
             for name, input in inputs.items():
                 if name not in self.nodes.keys():
                     raise KeyError(f"Node {name} not found in WorkGraph.")
                 self.nodes[name].set(input)
         # One can not run again if the process is alreay created. otherwise, a new process node will
         # be created again.
         if self.process is not None:
             print("Your workgraph is already created. Please use the submit() method.")
             return
         wgdata = self.to_dict()
         merge_properties(wgdata)
+        serialize_pythonjob_properties(wgdata)
         inputs = {"wg": wgdata}
         # init a process
         runner = get_manager().get_runner()
         process_inited = WorkGraphEngine(runner=runner, inputs=inputs)
         self.process = process_inited.node
         # save workgraph data into process node
         self.save_to_base(wgdata)
@@ -133,18 +137,22 @@
 
     def save(self, metadata: Optional[Dict[str, Any]] = None) -> None:
         """Save the udpated workgraph to the process
         This is only used for a running workgraph.
         Save the AiiDA workgraph process and update the process status.
         """
         from aiida_workgraph.engine.workgraph import WorkGraphEngine
-        from aiida_workgraph.utils import merge_properties
+        from aiida_workgraph.utils import (
+            merge_properties,
+            serialize_pythonjob_properties,
+        )
 
         wgdata = self.to_dict()
         merge_properties(wgdata)
+        serialize_pythonjob_properties(wgdata)
         metadata = metadata or {}
         inputs = {"wg": wgdata, "metadata": metadata}
         if self.process is None:
             # init a process node
             process_inited = WorkGraphEngine(inputs=inputs)
             process_inited.runner.persister.save_checkpoint(process_inited)
             self.process = process_inited.node
@@ -190,14 +198,15 @@
         Args:
             timeout (int): The maximum time in seconds to wait for the process to finish. Defaults to 50.
         """
 
         start = time.time()
         self.update()
         while self.state not in (
+            "KILLED",
             "PAUSED",
             "FINISHED",
             "FAILED",
             "CANCELLED",
             "EXCEPTED",
         ):
             time.sleep(0.5)
@@ -369,7 +378,12 @@
     def _repr_mimebundle_(self, *args, **kwargs):
         # if ipywdigets > 8.0.0, use _repr_mimebundle_ instead of _ipython_display_
         self._widget.from_workgraph(self)
         if hasattr(self._widget, "_repr_mimebundle_"):
             return self._widget._repr_mimebundle_(*args, **kwargs)
         else:
             return self._widget._ipython_display_(*args, **kwargs)
+
+    def to_html(self, output: str = None, **kwargs):
+        """Write a standalone html file to visualize the workgraph."""
+        self._widget.from_workgraph(self)
+        return self._widget.to_html(output=output, **kwargs)
```

### Comparing `aiida_workgraph-0.2.6/pyproject.toml` & `aiida_workgraph-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.6/PKG-INFO` & `aiida_workgraph-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-workgraph
-Version: 0.2.6
+Version: 0.2.7
 Summary: Design flexible node-based workflow for AiiDA calculation.
 Keywords: aiida,workflows
 Author-email: Xing Wang <xingwang1991@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 1 - Planning
 Classifier: Framework :: AiiDA
@@ -52,14 +52,15 @@
 [![PyPI version](https://badge.fury.io/py/aiida-workgraph.svg)](https://badge.fury.io/py/aiida-workgraph)
 [![Unit test](https://github.com/superstar54/aiida-workgraph/actions/workflows/ci.yaml/badge.svg)](https://github.com/superstar54/aiida-workgraph/actions/workflows/ci.yaml)
 [![codecov](https://codecov.io/gh/superstar54/aiida-workgraph/branch/main/graph/badge.svg)](https://codecov.io/gh/superstar54/aiida-workgraph)
 [![Docs status](https://readthedocs.org/projects/aiida-workgraph/badge)](http://aiida-workgraph.readthedocs.io/)
 
 Provides the third workflow component: `WorkGraph`, to design flexible node-based workflows using AiiDA.
 
+
 In AiiDA, there are two workflow components: `workfunction` and `WorkChain`. Workfunction is easy to implement but it does not support automatic checkpointing, which is important for long-running calculations. Workchain supports automatic checkpointing but it is difficult to implement and also not as flexible as the `workfunction`. AiiDA-WorkGraph provides the third component: `WorkGraph`. It is easy to implement and supports automatic checkpointing. It is also flexible and can be used to design complex workflows.
 
 
 Here is a detailed comparison between the ``WorkGraph`` with two AiiDA built-in workflow components.
 
 
 | Aspect                   | WorkFunction           | WorkChain                     | WorkGraph               |
```

