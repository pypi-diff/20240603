# Comparing `tmp/swarmauri-0.2.9.tar.gz` & `tmp/swarmauri-0.3.0.dev13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarmauri-0.2.9.tar", last modified: Wed May 22 03:00:08 2024, max compression
+gzip compressed data, was "swarmauri-0.3.0.dev13.tar", last modified: Mon Jun  3 12:35:08 2024, max compression
```

## Comparing `swarmauri-0.2.9.tar` & `swarmauri-0.3.0.dev13.tar`

### file list

```diff
@@ -1,520 +1,528 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.443001 swarmauri-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-05-22 03:00:08.439001 swarmauri-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-22 02:59:56.000000 swarmauri-0.2.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 03:00:08.443001 swarmauri-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-22 02:59:56.000000 swarmauri-0.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.355001 swarmauri-0.2.9/swarmauri/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.355001 swarmauri-0.2.9/swarmauri/community/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/community/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.355001 swarmauri-0.2.9/swarmauri/community/document_stores/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/community/document_stores/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.355001 swarmauri-0.2.9/swarmauri/community/document_stores/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/community/document_stores/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.355001 swarmauri-0.2.9/swarmauri/community/document_stores/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/community/document_stores/concrete/RedisDocumentStore.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/community/document_stores/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.355001 swarmauri-0.2.9/swarmauri/community/retrievers/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/community/retrievers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.355001 swarmauri-0.2.9/swarmauri/community/retrievers/base/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/community/retrievers/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.355001 swarmauri-0.2.9/swarmauri/community/retrievers/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/community/retrievers/concrete/RedisDocumentRetriever.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/community/retrievers/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.355001 swarmauri-0.2.9/swarmauri/community/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/community/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.355001 swarmauri-0.2.9/swarmauri/community/tools/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/community/tools/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.359001 swarmauri-0.2.9/swarmauri/community/tools/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/community/tools/concrete/DownloadPdfTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/community/tools/concrete/EntityRecognitionTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/community/tools/concrete/GmailReadTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/community/tools/concrete/GmailSendTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/community/tools/concrete/PaCMAP.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/community/tools/concrete/SentimentAnalysisTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/community/tools/concrete/WebScrapingTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/community/tools/concrete/ZapierHookTool.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/community/tools/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.359001 swarmauri-0.2.9/swarmauri/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.359001 swarmauri-0.2.9/swarmauri/core/agent_apis/
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/agent_apis/IAgentCommands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/agent_apis/IAgentRouterCRUD.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/agent_apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.359001 swarmauri-0.2.9/swarmauri/core/agent_factories/
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/agent_factories/IAgentFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/agent_factories/IExportConf.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/agent_factories/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.363000 swarmauri-0.2.9/swarmauri/core/agents/
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/agents/IAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/agents/IAgentConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/agents/IAgentName.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/agents/IAgentParser.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/agents/IAgentRetrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/agents/IAgentSystemContext.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/agents/IAgentToolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/agents/IAgentVectorStore.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.363000 swarmauri-0.2.9/swarmauri/core/chains/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/chains/ICallableChain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/chains/IChain.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/chains/IChainContext.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/chains/IChainContextLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/chains/IChainDependencyResolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/chains/IChainFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/chains/IChainStep.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/chains/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.363000 swarmauri-0.2.9/swarmauri/core/chunkers/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/chunkers/IChunker.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/chunkers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.363000 swarmauri-0.2.9/swarmauri/core/conversations/
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/conversations/IConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/conversations/IMaxSize.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/conversations/ISystemContext.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/conversations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.363000 swarmauri-0.2.9/swarmauri/core/distances/
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/distances/IDistanceSimilarity.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/distances/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.363000 swarmauri-0.2.9/swarmauri/core/document_stores/
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/document_stores/IDocumentRetrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/document_stores/IDocumentStore.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/document_stores/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.367000 swarmauri-0.2.9/swarmauri/core/documents/
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/documents/IDocument.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/documents/IEmbed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/documents/IExperimentDocument.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/documents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.367000 swarmauri-0.2.9/swarmauri/core/experiment_stores/
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/experiment_stores/IExperimentStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/experiment_stores/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.367000 swarmauri-0.2.9/swarmauri/core/messages/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/messages/IMessage.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/messages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.367000 swarmauri-0.2.9/swarmauri/core/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/metrics/IAggMeasurements.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/metrics/ICalculateMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/metrics/IMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/metrics/IThreshold.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.367000 swarmauri-0.2.9/swarmauri/core/models/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/models/IFit.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/models/IModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/models/IPredict.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.367000 swarmauri-0.2.9/swarmauri/core/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/parsers/IParser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.371001 swarmauri-0.2.9/swarmauri/core/prompts/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/prompts/IPrompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/prompts/IPromptMatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/prompts/ITemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/prompts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.371001 swarmauri-0.2.9/swarmauri/core/swarm_apis/
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/swarm_apis/IAgentRegistrationAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/swarm_apis/ISwarmAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/swarm_apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.371001 swarmauri-0.2.9/swarmauri/core/swarms/
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/swarms/ISwarm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/swarms/ISwarmAgentRegistration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/swarms/ISwarmChainCRUD.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/swarms/ISwarmComponent.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/swarms/ISwarmConfigurationExporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/swarms/ISwarmFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.371001 swarmauri-0.2.9/swarmauri/core/toolkits/
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/toolkits/IToolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/toolkits/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.371001 swarmauri-0.2.9/swarmauri/core/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/tools/IParameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/tools/ITool.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.371001 swarmauri-0.2.9/swarmauri/core/tracing/
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/tracing/IChainTracer.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/tracing/ITraceContext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/tracing/ITracer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/tracing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.375001 swarmauri-0.2.9/swarmauri/core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/utils/ITransactional.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.375001 swarmauri-0.2.9/swarmauri/core/vector_stores/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/vector_stores/IAngleBetweenVectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/vector_stores/IDecompose.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/vector_stores/IDivergence.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/vector_stores/IGradient.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/vector_stores/IOrthogonalProject.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/vector_stores/IProject.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/vector_stores/IReflect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/vector_stores/ISaveLoadStore.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/vector_stores/ISimilarity.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/vector_stores/ISimiliarityQuery.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/vector_stores/IVectorArithmetic.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/vector_stores/IVectorBasisCheck.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/vector_stores/IVectorLinearCombination.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/vector_stores/IVectorNorm.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/vector_stores/IVectorRetrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/vector_stores/IVectorRotate.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/vector_stores/IVectorSpan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/vector_stores/IVectorStore.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/vector_stores/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.379001 swarmauri-0.2.9/swarmauri/core/vectorizers/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/vectorizers/IFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/vectorizers/ISaveModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/vectorizers/IVectorize.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/vectorizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.379001 swarmauri-0.2.9/swarmauri/core/vectors/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/vectors/IVector.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/vectors/IVectorMeta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/vectors/IVectorProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/vectors/IVectorTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/core/vectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.379001 swarmauri-0.2.9/swarmauri/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.379001 swarmauri-0.2.9/swarmauri/experimental/chains/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/chains/IChainFormatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/chains/IChainNotification.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/chains/IChainPersistence.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/chains/IChainScheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/chains/TypeAgnosticCallableChain.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/chains/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.379001 swarmauri-0.2.9/swarmauri/experimental/conversations/
--rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/conversations/ConsensusBuildingConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/conversations/SemanticConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/conversations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.383000 swarmauri-0.2.9/swarmauri/experimental/distances/
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/distances/CanberraDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/distances/ChebyshevDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/distances/HaversineDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/distances/ManhattanDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/distances/MinkowskiDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/distances/SSASimilarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/distances/SSIVSimilarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     6910 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/distances/ScannVectorStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/distances/SorensenDiceDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/distances/SquaredEuclideanDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/distances/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.383000 swarmauri-0.2.9/swarmauri/experimental/document_stores/
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/document_stores/TriplesDocumentStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/document_stores/Word2VecDocumentStore.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/document_stores/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.383000 swarmauri-0.2.9/swarmauri/experimental/models/
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/models/HierarchicalAttentionModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/models/SageMaker.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.383000 swarmauri-0.2.9/swarmauri/experimental/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/parsers/PDFToTextParser.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.387001 swarmauri-0.2.9/swarmauri/experimental/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/tools/CypherQueryTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/tools/FileDownloaderTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/tools/LinkedInArticleTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/tools/OutlookSendMailTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/tools/SQLite3QueryTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/tools/TwitterPostTool.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.387001 swarmauri-0.2.9/swarmauri/experimental/tracing/
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/tracing/RemoteTrace.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/tracing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.387001 swarmauri-0.2.9/swarmauri/experimental/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/utils/ISerializable.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/utils/get_last_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/utils/log_prompt_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/utils/save_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.387001 swarmauri-0.2.9/swarmauri/experimental/vector_stores/
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/vector_stores/TriplesDocumentStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/vector_stores/Word2VecDocumentStore.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/vector_stores/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.387001 swarmauri-0.2.9/swarmauri/experimental/vectorizers/
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/vectorizers/DGLVectorizer.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/experimental/vectorizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.387001 swarmauri-0.2.9/swarmauri/standard/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.387001 swarmauri-0.2.9/swarmauri/standard/agent_factories/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/agent_factories/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.387001 swarmauri-0.2.9/swarmauri/standard/agent_factories/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/agent_factories/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.391001 swarmauri-0.2.9/swarmauri/standard/agent_factories/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/agent_factories/concrete/AgentFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/agent_factories/concrete/ConfDrivenAgentFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/agent_factories/concrete/JsonAgentFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/agent_factories/concrete/ReflectiveAgentFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/agent_factories/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.391001 swarmauri-0.2.9/swarmauri/standard/agents/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.391001 swarmauri-0.2.9/swarmauri/standard/agents/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/agents/base/AgentBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/agents/base/AgentRetrieveBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/agents/base/ConversationAgentBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/agents/base/NamedAgentBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/agents/base/SystemContextAgentBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/agents/base/ToolAgentBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/agents/base/VectorStoreAgentBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/agents/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.391001 swarmauri-0.2.9/swarmauri/standard/agents/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/agents/concrete/ChatSwarmAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/agents/concrete/MultiPartyChatSwarmAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/agents/concrete/MultiPartyToolAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/agents/concrete/QAAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/agents/concrete/RagAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/agents/concrete/SimpleConversationAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/agents/concrete/ToolAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/agents/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.391001 swarmauri-0.2.9/swarmauri/standard/apis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.391001 swarmauri-0.2.9/swarmauri/standard/apis/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/apis/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.391001 swarmauri-0.2.9/swarmauri/standard/apis/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/apis/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.391001 swarmauri-0.2.9/swarmauri/standard/chains/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/chains/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.395001 swarmauri-0.2.9/swarmauri/standard/chains/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/chains/base/ChainBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/chains/base/ChainContextBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/chains/base/ChainStepBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/chains/base/PromptContextChainBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/chains/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.395001 swarmauri-0.2.9/swarmauri/standard/chains/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/chains/concrete/CallableChain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/chains/concrete/ChainStep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/chains/concrete/ContextChain.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/chains/concrete/PromptContextChain.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/chains/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.395001 swarmauri-0.2.9/swarmauri/standard/chunkers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/chunkers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.395001 swarmauri-0.2.9/swarmauri/standard/chunkers/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/chunkers/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.395001 swarmauri-0.2.9/swarmauri/standard/chunkers/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/chunkers/concrete/DelimiterBasedChunker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/chunkers/concrete/FixedLengthChunker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/chunkers/concrete/MdSnippetChunker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/chunkers/concrete/SimpleSentenceChunker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/chunkers/concrete/SlidingWindowChunker.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/chunkers/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.395001 swarmauri-0.2.9/swarmauri/standard/conversations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/conversations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.395001 swarmauri-0.2.9/swarmauri/standard/conversations/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/conversations/base/ConversationBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/conversations/base/SystemContextBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/conversations/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.399001 swarmauri-0.2.9/swarmauri/standard/conversations/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/conversations/concrete/LimitedSizeConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/conversations/concrete/LimitedSystemContextConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/conversations/concrete/MaxSizeConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/conversations/concrete/MaxSystemContextConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/conversations/concrete/SessionCacheConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/conversations/concrete/SharedConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/conversations/concrete/SimpleConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/conversations/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.399001 swarmauri-0.2.9/swarmauri/standard/distances/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/distances/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.399001 swarmauri-0.2.9/swarmauri/standard/distances/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/distances/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.399001 swarmauri-0.2.9/swarmauri/standard/distances/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/distances/concrete/ChiSquaredDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/distances/concrete/CosineDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/distances/concrete/EuclideanDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/distances/concrete/JaccardIndexDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/distances/concrete/LevenshteinDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/distances/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.399001 swarmauri-0.2.9/swarmauri/standard/document_stores/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/document_stores/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.399001 swarmauri-0.2.9/swarmauri/standard/document_stores/base/
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/document_stores/base/DocumentStoreBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/document_stores/base/DocumentStoreRetrieveBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/document_stores/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.399001 swarmauri-0.2.9/swarmauri/standard/document_stores/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/document_stores/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.399001 swarmauri-0.2.9/swarmauri/standard/documents/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/documents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.403001 swarmauri-0.2.9/swarmauri/standard/documents/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/documents/base/DocumentBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/documents/base/EmbeddedBase.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/documents/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.403001 swarmauri-0.2.9/swarmauri/standard/documents/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/documents/concrete/Document.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/documents/concrete/EmbeddedDocument.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/documents/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.403001 swarmauri-0.2.9/swarmauri/standard/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.403001 swarmauri-0.2.9/swarmauri/standard/exceptions/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/exceptions/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.403001 swarmauri-0.2.9/swarmauri/standard/exceptions/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/exceptions/concrete/IndexErrorWithContext.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/exceptions/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.403001 swarmauri-0.2.9/swarmauri/standard/messages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/messages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.403001 swarmauri-0.2.9/swarmauri/standard/messages/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/messages/base/MessageBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/messages/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.403001 swarmauri-0.2.9/swarmauri/standard/messages/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/messages/concrete/AgentMessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/messages/concrete/FunctionMessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/messages/concrete/HumanMessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/messages/concrete/SystemMessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/messages/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.403001 swarmauri-0.2.9/swarmauri/standard/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.407001 swarmauri-0.2.9/swarmauri/standard/metrics/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/metrics/base/AggregateMetricBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/metrics/base/CalculateMetricBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/metrics/base/MetricBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/metrics/base/ThresholdMetricBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/metrics/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.407001 swarmauri-0.2.9/swarmauri/standard/metrics/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/metrics/concrete/FirstImpressionMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/metrics/concrete/HitRateAtK.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/metrics/concrete/ImpressionAtK.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/metrics/concrete/MeanMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/metrics/concrete/StaticValueMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/metrics/concrete/SystemUsabilityScaleMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/metrics/concrete/TaskSuccessRateMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/metrics/concrete/ThresholdMeanMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/metrics/concrete/TimeOnTaskMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/metrics/concrete/ZeroMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/metrics/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.407001 swarmauri-0.2.9/swarmauri/standard/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.407001 swarmauri-0.2.9/swarmauri/standard/models/base/
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/models/base/ModelBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/models/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.411001 swarmauri-0.2.9/swarmauri/standard/models/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/models/concrete/AnthropicModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/models/concrete/AzureGPT.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/models/concrete/CohereModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/models/concrete/GeminiProModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/models/concrete/GroqModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/models/concrete/GroqToolModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/models/concrete/MistralModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/models/concrete/MistralToolModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/models/concrete/OpenAIImageGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/models/concrete/OpenAIModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/models/concrete/OpenAIToolModel.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/models/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.411001 swarmauri-0.2.9/swarmauri/standard/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.411001 swarmauri-0.2.9/swarmauri/standard/parsers/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/parsers/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.415001 swarmauri-0.2.9/swarmauri/standard/parsers/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/parsers/concrete/BERTEmbeddingParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/parsers/concrete/CSVParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/parsers/concrete/EntityRecognitionParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/parsers/concrete/HtmlTagStripParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/parsers/concrete/KeywordExtractorParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/parsers/concrete/MarkdownParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/parsers/concrete/OpenAPISpecParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/parsers/concrete/PhoneNumberExtractorParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/parsers/concrete/PythonParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/parsers/concrete/RegExParser.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/parsers/concrete/TFIDFParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/parsers/concrete/TextBlobNounParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/parsers/concrete/TextBlobSentenceParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/parsers/concrete/URLExtractorParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/parsers/concrete/XMLParser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/parsers/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.415001 swarmauri-0.2.9/swarmauri/standard/prompts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/prompts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.415001 swarmauri-0.2.9/swarmauri/standard/prompts/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/prompts/base/BasePromptMatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/prompts/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.415001 swarmauri-0.2.9/swarmauri/standard/prompts/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/prompts/concrete/Prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/prompts/concrete/PromptGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/prompts/concrete/PromptMatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/prompts/concrete/PromptTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/prompts/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.415001 swarmauri-0.2.9/swarmauri/standard/states/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/states/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.415001 swarmauri-0.2.9/swarmauri/standard/states/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/states/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.415001 swarmauri-0.2.9/swarmauri/standard/states/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/states/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.415001 swarmauri-0.2.9/swarmauri/standard/swarms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.415001 swarmauri-0.2.9/swarmauri/standard/swarms/base/
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/swarms/base/SwarmComponentBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/swarms/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.415001 swarmauri-0.2.9/swarmauri/standard/swarms/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/swarms/concrete/SimpleSwarmFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/swarms/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.415001 swarmauri-0.2.9/swarmauri/standard/toolkits/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/toolkits/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.415001 swarmauri-0.2.9/swarmauri/standard/toolkits/base/
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/toolkits/base/ToolkitBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/toolkits/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.419000 swarmauri-0.2.9/swarmauri/standard/toolkits/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/toolkits/concrete/Toolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/toolkits/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.419000 swarmauri-0.2.9/swarmauri/standard/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.419000 swarmauri-0.2.9/swarmauri/standard/tools/base/
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/tools/base/ToolBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/tools/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.419000 swarmauri-0.2.9/swarmauri/standard/tools/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/tools/concrete/AdditionTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/tools/concrete/CalculatorTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/tools/concrete/CodeInterpreterTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/tools/concrete/ImportMemoryModuleTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/tools/concrete/Parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/tools/concrete/TestTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/tools/concrete/WeatherTool.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/tools/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.419000 swarmauri-0.2.9/swarmauri/standard/tracing/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/tracing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.419000 swarmauri-0.2.9/swarmauri/standard/tracing/base/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/tracing/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.423001 swarmauri-0.2.9/swarmauri/standard/tracing/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/tracing/concrete/CallableTracer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/tracing/concrete/ChainTracer.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/tracing/concrete/SimpleTraceContext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/tracing/concrete/SimpleTracer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/tracing/concrete/TracedVariable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/tracing/concrete/VariableTracer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/tracing/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.423001 swarmauri-0.2.9/swarmauri/standard/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/utils/apply_metaclass.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/utils/decorate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/utils/get_class_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/utils/json_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/utils/load_documents_from_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/utils/memoize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/utils/sql_log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.423001 swarmauri-0.2.9/swarmauri/standard/vector_stores/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/vector_stores/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.423001 swarmauri-0.2.9/swarmauri/standard/vector_stores/base/
--rw-r--r--   0 runner    (1001) docker     (127)     6796 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/vector_stores/base/SaveLoadStoreBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/vector_stores/base/VectorDocumentStoreBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/vector_stores/base/VectorDocumentStoreRetrieveBase.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/vector_stores/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.423001 swarmauri-0.2.9/swarmauri/standard/vector_stores/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/vector_stores/concrete/Doc2VecVectorStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/vector_stores/concrete/MLMVectorStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/vector_stores/concrete/SpatialDocVectorStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/vector_stores/concrete/TFIDFVectorStore.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/vector_stores/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.423001 swarmauri-0.2.9/swarmauri/standard/vectorizers/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/vectorizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.427001 swarmauri-0.2.9/swarmauri/standard/vectorizers/base/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/vectorizers/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.427001 swarmauri-0.2.9/swarmauri/standard/vectorizers/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/vectorizers/concrete/Doc2VecVectorizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8078 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/vectorizers/concrete/MLMVectorizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/vectorizers/concrete/NMFVectorizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/vectorizers/concrete/SpatialDocVectorizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/vectorizers/concrete/TFIDFVectorizer.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/vectorizers/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.427001 swarmauri-0.2.9/swarmauri/standard/vectors/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/vectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.427001 swarmauri-0.2.9/swarmauri/standard/vectors/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/vectors/base/VectorBase.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/vectors/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.427001 swarmauri-0.2.9/swarmauri/standard/vectors/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/vectors/concrete/SimpleVector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/vectors/concrete/VectorProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 02:59:56.000000 swarmauri-0.2.9/swarmauri/standard/vectors/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:08.427001 swarmauri-0.2.9/swarmauri.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-05-22 03:00:08.000000 swarmauri-0.2.9/swarmauri.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19089 2024-05-22 03:00:08.000000 swarmauri-0.2.9/swarmauri.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 03:00:08.000000 swarmauri-0.2.9/swarmauri.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-22 03:00:08.000000 swarmauri-0.2.9/swarmauri.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 03:00:08.000000 swarmauri-0.2.9/swarmauri.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.592800 swarmauri-0.3.0.dev13/
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-06-03 12:35:08.592800 swarmauri-0.3.0.dev13/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 12:35:08.592800 swarmauri-0.3.0.dev13/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.504800 swarmauri-0.3.0.dev13/swarmauri/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.508800 swarmauri-0.3.0.dev13/swarmauri/community/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/community/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.508800 swarmauri-0.3.0.dev13/swarmauri/community/document_stores/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/community/document_stores/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.508800 swarmauri-0.3.0.dev13/swarmauri/community/document_stores/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/community/document_stores/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.508800 swarmauri-0.3.0.dev13/swarmauri/community/document_stores/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/community/document_stores/concrete/RedisDocumentStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/community/document_stores/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.508800 swarmauri-0.3.0.dev13/swarmauri/community/retrievers/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/community/retrievers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.508800 swarmauri-0.3.0.dev13/swarmauri/community/retrievers/base/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/community/retrievers/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.508800 swarmauri-0.3.0.dev13/swarmauri/community/retrievers/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/community/retrievers/concrete/RedisDocumentRetriever.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/community/retrievers/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.508800 swarmauri-0.3.0.dev13/swarmauri/community/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/community/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.508800 swarmauri-0.3.0.dev13/swarmauri/community/tools/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/community/tools/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.508800 swarmauri-0.3.0.dev13/swarmauri/community/tools/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/community/tools/concrete/DownloadPdfTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/community/tools/concrete/EntityRecognitionTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/community/tools/concrete/GmailReadTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/community/tools/concrete/GmailSendTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/community/tools/concrete/PaCMAP.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/community/tools/concrete/SentimentAnalysisTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/community/tools/concrete/WebScrapingTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/community/tools/concrete/ZapierHookTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/community/tools/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.512800 swarmauri-0.3.0.dev13/swarmauri/community/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (127)    10110 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/community/vector_stores/AnnoyVectorStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/community/vector_stores/ChromadbVectorStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6267 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/community/vector_stores/QdrantVectorStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/community/vector_stores/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.512800 swarmauri-0.3.0.dev13/swarmauri/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/BaseComponent.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.512800 swarmauri-0.3.0.dev13/swarmauri/core/agent_apis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/agent_apis/IAgentCommands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/agent_apis/IAgentRouterCRUD.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/agent_apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.512800 swarmauri-0.3.0.dev13/swarmauri/core/agent_factories/
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/agent_factories/IAgentFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/agent_factories/IExportConf.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/agent_factories/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.512800 swarmauri-0.3.0.dev13/swarmauri/core/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/agents/IAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/agents/IAgentConversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/agents/IAgentName.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/agents/IAgentParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/agents/IAgentRetrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/agents/IAgentSystemContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/agents/IAgentToolkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/agents/IAgentVectorStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.516800 swarmauri-0.3.0.dev13/swarmauri/core/chains/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/chains/ICallableChain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/chains/IChain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/chains/IChainContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/chains/IChainContextLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/chains/IChainDependencyResolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/chains/IChainFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/chains/IChainStep.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/chains/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.516800 swarmauri-0.3.0.dev13/swarmauri/core/chunkers/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/chunkers/IChunker.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/chunkers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.516800 swarmauri-0.3.0.dev13/swarmauri/core/conversations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/conversations/IConversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/conversations/IMaxSize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/conversations/ISystemContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/conversations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.516800 swarmauri-0.3.0.dev13/swarmauri/core/distances/
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/distances/IDistanceSimilarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/distances/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.516800 swarmauri-0.3.0.dev13/swarmauri/core/document_stores/
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/document_stores/IDocumentRetrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/document_stores/IDocumentStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/document_stores/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.520800 swarmauri-0.3.0.dev13/swarmauri/core/documents/
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/documents/IDocument.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/documents/IEmbed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/documents/IExperimentDocument.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/documents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.520800 swarmauri-0.3.0.dev13/swarmauri/core/experiment_stores/
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/experiment_stores/IExperimentStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/experiment_stores/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.520800 swarmauri-0.3.0.dev13/swarmauri/core/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/messages/IMessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/messages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.520800 swarmauri-0.3.0.dev13/swarmauri/core/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/metrics/IAggMeasurements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/metrics/ICalculateMetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/metrics/IMetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/metrics/IThreshold.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.520800 swarmauri-0.3.0.dev13/swarmauri/core/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/models/IFit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/models/IModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/models/IPredict.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.520800 swarmauri-0.3.0.dev13/swarmauri/core/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/parsers/IParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.520800 swarmauri-0.3.0.dev13/swarmauri/core/prompts/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/prompts/IPrompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/prompts/IPromptMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/prompts/ITemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/prompts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.524800 swarmauri-0.3.0.dev13/swarmauri/core/swarm_apis/
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/swarm_apis/IAgentRegistrationAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/swarm_apis/ISwarmAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/swarm_apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.524800 swarmauri-0.3.0.dev13/swarmauri/core/swarms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/swarms/ISwarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/swarms/ISwarmAgentRegistration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/swarms/ISwarmChainCRUD.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/swarms/ISwarmComponent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/swarms/ISwarmConfigurationExporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/swarms/ISwarmFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.524800 swarmauri-0.3.0.dev13/swarmauri/core/toolkits/
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/toolkits/IToolkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/toolkits/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.524800 swarmauri-0.3.0.dev13/swarmauri/core/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/tools/IParameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/tools/ITool.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.524800 swarmauri-0.3.0.dev13/swarmauri/core/tracing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/tracing/IChainTracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/tracing/ITraceContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/tracing/ITracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/tracing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.524800 swarmauri-0.3.0.dev13/swarmauri/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/utils/ITransactional.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.528800 swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/IAngleBetweenVectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/IDecompose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/IDivergence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/IGradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/IOrthogonalProject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/IProject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/IReflect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/ISaveLoadStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/ISimilarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/ISimiliarityQuery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/IVectorArithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/IVectorBasisCheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/IVectorLinearCombination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/IVectorNorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/IVectorRetrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/IVectorRotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/IVectorSpan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/IVectorStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.528800 swarmauri-0.3.0.dev13/swarmauri/core/vectorizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/vectorizers/IFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/vectorizers/ISaveModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/vectorizers/IVectorize.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/vectorizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.532800 swarmauri-0.3.0.dev13/swarmauri/core/vectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/vectors/IVector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/vectors/IVectorMeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/vectors/IVectorProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/vectors/IVectorTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/core/vectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.532800 swarmauri-0.3.0.dev13/swarmauri/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/RemoteUniversalBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.532800 swarmauri-0.3.0.dev13/swarmauri/experimental/chains/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/chains/IChainFormatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/chains/IChainNotification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/chains/IChainPersistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/chains/IChainScheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/chains/TypeAgnosticCallableChain.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/chains/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.532800 swarmauri-0.3.0.dev13/swarmauri/experimental/conversations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/conversations/ConsensusBuildingConversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/conversations/SemanticConversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/conversations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.536800 swarmauri-0.3.0.dev13/swarmauri/experimental/distances/
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/distances/CanberraDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/distances/ChebyshevDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/distances/HaversineDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/distances/ManhattanDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/distances/MinkowskiDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/distances/SSASimilarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/distances/SSIVSimilarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6910 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/distances/ScannVectorStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/distances/SorensenDiceDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/distances/SquaredEuclideanDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/distances/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.536800 swarmauri-0.3.0.dev13/swarmauri/experimental/document_stores/
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/document_stores/TriplesDocumentStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/document_stores/Word2VecDocumentStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/document_stores/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.536800 swarmauri-0.3.0.dev13/swarmauri/experimental/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/models/HierarchicalAttentionModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/models/SageMaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.536800 swarmauri-0.3.0.dev13/swarmauri/experimental/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/parsers/PDFToTextParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.536800 swarmauri-0.3.0.dev13/swarmauri/experimental/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/tools/CypherQueryTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/tools/FileDownloaderTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/tools/LinkedInArticleTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/tools/OutlookSendMailTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/tools/SQLite3QueryTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/tools/TwitterPostTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.536800 swarmauri-0.3.0.dev13/swarmauri/experimental/tracing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/tracing/RemoteTrace.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/tracing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.540800 swarmauri-0.3.0.dev13/swarmauri/experimental/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/utils/ISerializable.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/utils/get_last_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/utils/log_prompt_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/utils/save_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.540800 swarmauri-0.3.0.dev13/swarmauri/experimental/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/vector_stores/TriplesDocumentStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/vector_stores/Word2VecDocumentStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/vector_stores/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.540800 swarmauri-0.3.0.dev13/swarmauri/experimental/vectorizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/vectorizers/DGLVectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/experimental/vectorizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.540800 swarmauri-0.3.0.dev13/swarmauri/standard/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.540800 swarmauri-0.3.0.dev13/swarmauri/standard/agent_factories/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/agent_factories/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.540800 swarmauri-0.3.0.dev13/swarmauri/standard/agent_factories/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/agent_factories/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.540800 swarmauri-0.3.0.dev13/swarmauri/standard/agent_factories/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/agent_factories/concrete/AgentFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/agent_factories/concrete/ConfDrivenAgentFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/agent_factories/concrete/JsonAgentFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/agent_factories/concrete/ReflectiveAgentFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/agent_factories/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.540800 swarmauri-0.3.0.dev13/swarmauri/standard/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.544800 swarmauri-0.3.0.dev13/swarmauri/standard/agents/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/agents/base/AgentBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/agents/base/AgentRetrieveBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/agents/base/ConversationAgentBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/agents/base/NamedAgentBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/agents/base/SystemContextAgentBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/agents/base/ToolAgentBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/agents/base/VectorStoreAgentBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/agents/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.544800 swarmauri-0.3.0.dev13/swarmauri/standard/agents/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/agents/concrete/ChatSwarmAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/agents/concrete/MultiPartyChatSwarmAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/agents/concrete/MultiPartyToolAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/agents/concrete/QAAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/agents/concrete/RagAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/agents/concrete/SimpleConversationAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/agents/concrete/ToolAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/agents/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.544800 swarmauri-0.3.0.dev13/swarmauri/standard/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.544800 swarmauri-0.3.0.dev13/swarmauri/standard/apis/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/apis/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.544800 swarmauri-0.3.0.dev13/swarmauri/standard/apis/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/apis/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.544800 swarmauri-0.3.0.dev13/swarmauri/standard/chains/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/chains/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.544800 swarmauri-0.3.0.dev13/swarmauri/standard/chains/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/chains/base/ChainBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/chains/base/ChainContextBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/chains/base/ChainStepBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/chains/base/PromptContextChainBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/chains/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.548800 swarmauri-0.3.0.dev13/swarmauri/standard/chains/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/chains/concrete/CallableChain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/chains/concrete/ChainStep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/chains/concrete/ContextChain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/chains/concrete/PromptContextChain.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/chains/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.548800 swarmauri-0.3.0.dev13/swarmauri/standard/chunkers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/chunkers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.548800 swarmauri-0.3.0.dev13/swarmauri/standard/chunkers/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/chunkers/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.548800 swarmauri-0.3.0.dev13/swarmauri/standard/chunkers/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/chunkers/concrete/DelimiterBasedChunker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/chunkers/concrete/FixedLengthChunker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/chunkers/concrete/MdSnippetChunker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/chunkers/concrete/SimpleSentenceChunker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/chunkers/concrete/SlidingWindowChunker.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/chunkers/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.548800 swarmauri-0.3.0.dev13/swarmauri/standard/conversations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/conversations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.548800 swarmauri-0.3.0.dev13/swarmauri/standard/conversations/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/conversations/base/ConversationBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/conversations/base/SystemContextBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/conversations/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.548800 swarmauri-0.3.0.dev13/swarmauri/standard/conversations/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/conversations/concrete/LimitedSizeConversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/conversations/concrete/LimitedSystemContextConversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/conversations/concrete/MaxSizeConversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/conversations/concrete/MaxSystemContextConversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/conversations/concrete/SessionCacheConversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/conversations/concrete/SharedConversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/conversations/concrete/SimpleConversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/conversations/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.552800 swarmauri-0.3.0.dev13/swarmauri/standard/distances/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/distances/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.552800 swarmauri-0.3.0.dev13/swarmauri/standard/distances/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/distances/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.552800 swarmauri-0.3.0.dev13/swarmauri/standard/distances/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/distances/concrete/ChiSquaredDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/distances/concrete/CosineDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/distances/concrete/EuclideanDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/distances/concrete/JaccardIndexDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/distances/concrete/LevenshteinDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/distances/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.552800 swarmauri-0.3.0.dev13/swarmauri/standard/document_stores/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/document_stores/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.552800 swarmauri-0.3.0.dev13/swarmauri/standard/document_stores/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/document_stores/base/DocumentStoreBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/document_stores/base/DocumentStoreRetrieveBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/document_stores/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.552800 swarmauri-0.3.0.dev13/swarmauri/standard/document_stores/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/document_stores/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.552800 swarmauri-0.3.0.dev13/swarmauri/standard/documents/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/documents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.552800 swarmauri-0.3.0.dev13/swarmauri/standard/documents/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/documents/base/DocumentBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/documents/base/EmbeddedBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/documents/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.556800 swarmauri-0.3.0.dev13/swarmauri/standard/documents/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/documents/concrete/Document.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/documents/concrete/EmbeddedDocument.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/documents/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.556800 swarmauri-0.3.0.dev13/swarmauri/standard/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.556800 swarmauri-0.3.0.dev13/swarmauri/standard/exceptions/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/exceptions/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.556800 swarmauri-0.3.0.dev13/swarmauri/standard/exceptions/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/exceptions/concrete/IndexErrorWithContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/exceptions/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.556800 swarmauri-0.3.0.dev13/swarmauri/standard/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/messages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.556800 swarmauri-0.3.0.dev13/swarmauri/standard/messages/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/messages/base/MessageBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/messages/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.556800 swarmauri-0.3.0.dev13/swarmauri/standard/messages/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/messages/concrete/AgentMessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/messages/concrete/FunctionMessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/messages/concrete/HumanMessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/messages/concrete/SystemMessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/messages/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.556800 swarmauri-0.3.0.dev13/swarmauri/standard/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.556800 swarmauri-0.3.0.dev13/swarmauri/standard/metrics/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/metrics/base/AggregateMetricBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/metrics/base/CalculateMetricBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/metrics/base/MetricBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/metrics/base/ThresholdMetricBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/metrics/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.560800 swarmauri-0.3.0.dev13/swarmauri/standard/metrics/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/metrics/concrete/FirstImpressionMetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/metrics/concrete/HitRateAtK.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/metrics/concrete/ImpressionAtK.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/metrics/concrete/MeanMetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/metrics/concrete/StaticValueMetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/metrics/concrete/SystemUsabilityScaleMetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/metrics/concrete/TaskSuccessRateMetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/metrics/concrete/ThresholdMeanMetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/metrics/concrete/TimeOnTaskMetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/metrics/concrete/ZeroMetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/metrics/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.560800 swarmauri-0.3.0.dev13/swarmauri/standard/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.560800 swarmauri-0.3.0.dev13/swarmauri/standard/models/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/models/base/ModelBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/models/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.560800 swarmauri-0.3.0.dev13/swarmauri/standard/models/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/models/concrete/AnthropicModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/models/concrete/AzureGPT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/models/concrete/CohereModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/models/concrete/GeminiProModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/models/concrete/GroqModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/models/concrete/GroqToolModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/models/concrete/MistralModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/models/concrete/MistralToolModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/models/concrete/OpenAIImageGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/models/concrete/OpenAIModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/models/concrete/OpenAIToolModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/models/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.564800 swarmauri-0.3.0.dev13/swarmauri/standard/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.564800 swarmauri-0.3.0.dev13/swarmauri/standard/parsers/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/parsers/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.564800 swarmauri-0.3.0.dev13/swarmauri/standard/parsers/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/parsers/concrete/BERTEmbeddingParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/parsers/concrete/CSVParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/parsers/concrete/EntityRecognitionParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/parsers/concrete/HtmlTagStripParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/parsers/concrete/KeywordExtractorParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/parsers/concrete/MarkdownParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/parsers/concrete/OpenAPISpecParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/parsers/concrete/PhoneNumberExtractorParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/parsers/concrete/PythonParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/parsers/concrete/RegExParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/parsers/concrete/TFIDFParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/parsers/concrete/TextBlobNounParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/parsers/concrete/TextBlobSentenceParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/parsers/concrete/URLExtractorParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/parsers/concrete/XMLParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/parsers/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.564800 swarmauri-0.3.0.dev13/swarmauri/standard/prompts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/prompts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.564800 swarmauri-0.3.0.dev13/swarmauri/standard/prompts/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/prompts/base/BasePromptMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/prompts/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.568800 swarmauri-0.3.0.dev13/swarmauri/standard/prompts/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/prompts/concrete/Prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/prompts/concrete/PromptGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/prompts/concrete/PromptMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/prompts/concrete/PromptTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/prompts/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.568800 swarmauri-0.3.0.dev13/swarmauri/standard/states/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/states/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.568800 swarmauri-0.3.0.dev13/swarmauri/standard/states/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/states/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.568800 swarmauri-0.3.0.dev13/swarmauri/standard/states/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/states/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.568800 swarmauri-0.3.0.dev13/swarmauri/standard/swarms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.568800 swarmauri-0.3.0.dev13/swarmauri/standard/swarms/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/swarms/base/SwarmComponentBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/swarms/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.568800 swarmauri-0.3.0.dev13/swarmauri/standard/swarms/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/swarms/concrete/SimpleSwarmFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/swarms/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.568800 swarmauri-0.3.0.dev13/swarmauri/standard/toolkits/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/toolkits/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.568800 swarmauri-0.3.0.dev13/swarmauri/standard/toolkits/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/toolkits/base/ToolkitBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/toolkits/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.568800 swarmauri-0.3.0.dev13/swarmauri/standard/toolkits/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/toolkits/concrete/Toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/toolkits/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.568800 swarmauri-0.3.0.dev13/swarmauri/standard/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.568800 swarmauri-0.3.0.dev13/swarmauri/standard/tools/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/tools/base/ParameterBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/tools/base/ToolBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/tools/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.572800 swarmauri-0.3.0.dev13/swarmauri/standard/tools/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/tools/concrete/AdditionTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/tools/concrete/CalculatorTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/tools/concrete/CodeInterpreterTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/tools/concrete/ImportMemoryModuleTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/tools/concrete/Parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/tools/concrete/TestTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/tools/concrete/WeatherTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/tools/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.572800 swarmauri-0.3.0.dev13/swarmauri/standard/tracing/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/tracing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.572800 swarmauri-0.3.0.dev13/swarmauri/standard/tracing/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/tracing/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.572800 swarmauri-0.3.0.dev13/swarmauri/standard/tracing/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/tracing/concrete/CallableTracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/tracing/concrete/ChainTracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/tracing/concrete/SimpleTraceContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/tracing/concrete/SimpleTracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/tracing/concrete/TracedVariable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/tracing/concrete/VariableTracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/tracing/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.572800 swarmauri-0.3.0.dev13/swarmauri/standard/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/utils/apply_metaclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/utils/decorate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/utils/get_class_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/utils/json_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/utils/load_documents_from_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/utils/memoize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/utils/sql_log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.572800 swarmauri-0.3.0.dev13/swarmauri/standard/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/vector_stores/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.576800 swarmauri-0.3.0.dev13/swarmauri/standard/vector_stores/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     6796 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/vector_stores/base/SaveLoadStoreBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/vector_stores/base/VectorDocumentStoreBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/vector_stores/base/VectorDocumentStoreRetrieveBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/vector_stores/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.576800 swarmauri-0.3.0.dev13/swarmauri/standard/vector_stores/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/vector_stores/concrete/Doc2VecVectorStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/vector_stores/concrete/MLMVectorStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/vector_stores/concrete/SpatialDocVectorStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/vector_stores/concrete/TFIDFVectorStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/vector_stores/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.576800 swarmauri-0.3.0.dev13/swarmauri/standard/vectorizers/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/vectorizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.576800 swarmauri-0.3.0.dev13/swarmauri/standard/vectorizers/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/vectorizers/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.576800 swarmauri-0.3.0.dev13/swarmauri/standard/vectorizers/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/vectorizers/concrete/Doc2VecVectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8078 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/vectorizers/concrete/MLMVectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/vectorizers/concrete/NMFVectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/vectorizers/concrete/SpatialDocVectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/vectorizers/concrete/TFIDFVectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/vectorizers/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.576800 swarmauri-0.3.0.dev13/swarmauri/standard/vectors/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/vectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.576800 swarmauri-0.3.0.dev13/swarmauri/standard/vectors/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/vectors/base/VectorBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/vectors/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.580800 swarmauri-0.3.0.dev13/swarmauri/standard/vectors/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/vectors/concrete/SimpleVector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/vectors/concrete/VectorProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-03 12:34:56.000000 swarmauri-0.3.0.dev13/swarmauri/standard/vectors/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:35:08.580800 swarmauri-0.3.0.dev13/swarmauri.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-06-03 12:35:08.000000 swarmauri-0.3.0.dev13/swarmauri.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19426 2024-06-03 12:35:08.000000 swarmauri-0.3.0.dev13/swarmauri.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 12:35:08.000000 swarmauri-0.3.0.dev13/swarmauri.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-06-03 12:35:08.000000 swarmauri-0.3.0.dev13/swarmauri.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-03 12:35:08.000000 swarmauri-0.3.0.dev13/swarmauri.egg-info/top_level.txt
```

### Comparing `swarmauri-0.2.9/PKG-INFO` & `swarmauri-0.3.0.dev13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarmauri
-Version: 0.2.9
+Version: 0.3.0.dev13
 Summary: This repository includes core interfaces, standard ABCs and concrete references, third party plugins, and experimental modules for the swarmaURI framework.
 Home-page: http://github.com/swarmauri/swarmauri-sdk
 Author: Jacob Stewart
 Author-email: corporate@swarmauri.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `swarmauri-0.2.9/README.md` & `swarmauri-0.3.0.dev13/README.md`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/setup.py` & `swarmauri-0.3.0.dev13/setup.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/community/document_stores/concrete/RedisDocumentStore.py` & `swarmauri-0.3.0.dev13/swarmauri/community/document_stores/concrete/RedisDocumentStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/community/retrievers/concrete/RedisDocumentRetriever.py` & `swarmauri-0.3.0.dev13/swarmauri/community/retrievers/concrete/RedisDocumentRetriever.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/community/tools/concrete/DownloadPdfTool.py` & `swarmauri-0.3.0.dev13/swarmauri/community/tools/concrete/DownloadPdfTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/community/tools/concrete/EntityRecognitionTool.py` & `swarmauri-0.3.0.dev13/swarmauri/community/tools/concrete/EntityRecognitionTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/community/tools/concrete/GmailReadTool.py` & `swarmauri-0.3.0.dev13/swarmauri/community/tools/concrete/GmailReadTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/community/tools/concrete/GmailSendTool.py` & `swarmauri-0.3.0.dev13/swarmauri/community/tools/concrete/GmailSendTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/community/tools/concrete/PaCMAP.py` & `swarmauri-0.3.0.dev13/swarmauri/community/tools/concrete/PaCMAP.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/community/tools/concrete/SentimentAnalysisTool.py` & `swarmauri-0.3.0.dev13/swarmauri/community/tools/concrete/SentimentAnalysisTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/community/tools/concrete/WebScrapingTool.py` & `swarmauri-0.3.0.dev13/swarmauri/community/tools/concrete/WebScrapingTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/community/tools/concrete/ZapierHookTool.py` & `swarmauri-0.3.0.dev13/swarmauri/community/tools/concrete/ZapierHookTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/agent_apis/IAgentCommands.py` & `swarmauri-0.3.0.dev13/swarmauri/core/agent_apis/IAgentCommands.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/agent_apis/IAgentRouterCRUD.py` & `swarmauri-0.3.0.dev13/swarmauri/core/agent_apis/IAgentRouterCRUD.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/agent_factories/IAgentFactory.py` & `swarmauri-0.3.0.dev13/swarmauri/core/agent_factories/IAgentFactory.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/agent_factories/IExportConf.py` & `swarmauri-0.3.0.dev13/swarmauri/core/agent_factories/IExportConf.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/agents/IAgent.py` & `swarmauri-0.3.0.dev13/swarmauri/core/agents/IAgent.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/chains/IChain.py` & `swarmauri-0.3.0.dev13/swarmauri/core/chains/IChain.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/chains/IChainDependencyResolver.py` & `swarmauri-0.3.0.dev13/swarmauri/core/chains/IChainDependencyResolver.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/chains/IChainFactory.py` & `swarmauri-0.3.0.dev13/swarmauri/core/chains/IChainFactory.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/chains/IChainStep.py` & `swarmauri-0.3.0.dev13/swarmauri/core/chains/IChainStep.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/conversations/IConversation.py` & `swarmauri-0.3.0.dev13/swarmauri/core/conversations/IConversation.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/conversations/ISystemContext.py` & `swarmauri-0.3.0.dev13/swarmauri/core/conversations/ISystemContext.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/distances/IDistanceSimilarity.py` & `swarmauri-0.3.0.dev13/swarmauri/core/distances/IDistanceSimilarity.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/document_stores/IDocumentRetrieve.py` & `swarmauri-0.3.0.dev13/swarmauri/core/document_stores/IDocumentRetrieve.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/document_stores/IDocumentStore.py` & `swarmauri-0.3.0.dev13/swarmauri/core/document_stores/IDocumentStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/documents/IDocument.py` & `swarmauri-0.3.0.dev13/swarmauri/core/metrics/IMetric.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,63 @@
+from typing import Any
 from abc import ABC, abstractmethod
-from typing import Dict
 
-class IDocument(ABC):
-    @abstractmethod
-    def __init__(self, id: str, content: str, metadata: Dict):
-        pass
+class IMetric(ABC):
+    """
+    Defines a general interface for metrics within the SwarmaURI system.
+    Metrics can be anything from system performance measurements to
+    machine learning model evaluation metrics.
+    """
 
     @property
     @abstractmethod
-    def id(self) -> str:
-        """
-        Get the document's ID.
+    def name(self) -> str:
         """
-        pass
+        The name identifier for the metric.
 
-    @id.setter
-    @abstractmethod
-    def id(self, value: str) -> None:
-        """
-        Set the document's ID.
+        Returns:
+            str: The name of the metric.
         """
         pass
 
     @property
     @abstractmethod
-    def content(self) -> str:
-        """
-        Get the document's content.
+    def value(self) -> Any:
         """
-        pass
+        Current value of the metric.
 
-    @content.setter
-    @abstractmethod
-    def content(self, value: str) -> None:
-        """
-        Set the document's content.
+        Returns:
+            The metric's value. The type depends on the specific metric implementation.
         """
         pass
 
     @property
     @abstractmethod
-    def metadata(self) -> Dict:
+    def unit(self) -> str:
         """
-        Get the document's metadata.
+        The unit of measurement for the metric.
+
+        Returns:
+            str: The unit of measurement (e.g., 'seconds', 'Mbps').
         """
         pass
 
-    @metadata.setter
+    @unit.setter
     @abstractmethod
-    def metadata(self, value: Dict) -> None:
+    def unit(self, value: str) -> None:
         """
-        Set the document's metadata.
+        Update the unit of measurement for the metric.
+
+        Args:
+            value (str): The new unit of measurement for the metric.
         """
         pass
 
-    # Including the abstract methods __str__ and __repr__ definitions for completeness.
     @abstractmethod
-    def __str__(self) -> str:
-        pass
+    def __call__(self, **kwargs) -> Any:
+        """
+        Retrieves the current value of the metric.
 
-    @abstractmethod
-    def __repr__(self) -> str:
-        pass
-    
-    def __setitem__(self, key, value):
-        """Allow setting items like a dict for metadata."""
-        self.metadata[key] = value
-
-    def __getitem__(self, key):
-        """Allow getting items like a dict for metadata."""
-        return self.metadata.get(key)
+        Returns:
+            The current value of the metric.
+        """
+        pass
```

### Comparing `swarmauri-0.2.9/swarmauri/core/documents/IExperimentDocument.py` & `swarmauri-0.3.0.dev13/swarmauri/core/documents/IExperimentDocument.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/experiment_stores/IExperimentStore.py` & `swarmauri-0.3.0.dev13/swarmauri/core/experiment_stores/IExperimentStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/experiment_stores/__init__.py` & `swarmauri-0.3.0.dev13/swarmauri/core/experiment_stores/__init__.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/messages/IMessage.py` & `swarmauri-0.3.0.dev13/swarmauri/core/messages/IMessage.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/metrics/IAggMeasurements.py` & `swarmauri-0.3.0.dev13/swarmauri/core/metrics/IAggMeasurements.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/metrics/ICalculateMetric.py` & `swarmauri-0.3.0.dev13/swarmauri/core/metrics/ICalculateMetric.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/metrics/IMetric.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/metrics/base/MetricBase.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,59 @@
 from typing import Any
 from abc import ABC, abstractmethod
+from swarmauri.core.metrics.IMetric import IMetric
 
-class IMetric(ABC):
+class MetricBase(IMetric, ABC):
     """
-    Defines a general interface for metrics within the SwarmaURI system.
-    Metrics can be anything from system performance measurements to
-    machine learning model evaluation metrics.
+    A base implementation of the IMetric interface that provides the foundation
+    for specific metric implementations.
     """
 
+    def __init__(self, name: str, unit: str):
+        """
+        Initializes the metric with a name and unit of measurement.
+
+        Args:
+            name (str): The name of the metric.
+            unit (str): The unit of measurement for the metric (e.g., 'seconds', 'accuracy').
+        """
+        self._name = name
+        self._unit = unit
+        self._value = None  # Initialize with None, or a default value as appropriate
+
     @property
-    @abstractmethod
     def name(self) -> str:
         """
-        The name identifier for the metric.
-
-        Returns:
-            str: The name of the metric.
+        The metric's name identifier.
         """
-        pass
+        return self._name
 
     @property
-    @abstractmethod
     def value(self) -> Any:
         """
-        Current value of the metric.
-
-        Returns:
-            The metric's value. The type depends on the specific metric implementation.
+        The current value of the metric.
         """
-        pass
+        return self._value
 
     @property
-    @abstractmethod
     def unit(self) -> str:
         """
         The unit of measurement for the metric.
-
-        Returns:
-            str: The unit of measurement (e.g., 'seconds', 'Mbps').
         """
-        pass
+        return self._unit
 
     @unit.setter
-    @abstractmethod
     def unit(self, value: str) -> None:
         """
-        Update the unit of measurement for the metric.
-
-        Args:
-            value (str): The new unit of measurement for the metric.
+        Set the unit of measurement for the metric.
         """
-        pass
+        self._unit = value
 
     @abstractmethod
     def __call__(self, **kwargs) -> Any:
         """
         Retrieves the current value of the metric.
 
         Returns:
             The current value of the metric.
         """
-        pass
+        return self.value
```

### Comparing `swarmauri-0.2.9/swarmauri/core/parsers/IParser.py` & `swarmauri-0.3.0.dev13/swarmauri/core/parsers/IParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/prompts/IPromptMatrix.py` & `swarmauri-0.3.0.dev13/swarmauri/core/prompts/IPromptMatrix.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/prompts/ITemplate.py` & `swarmauri-0.3.0.dev13/swarmauri/core/prompts/ITemplate.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/swarm_apis/IAgentRegistrationAPI.py` & `swarmauri-0.3.0.dev13/swarmauri/core/swarm_apis/IAgentRegistrationAPI.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/swarm_apis/ISwarmAPI.py` & `swarmauri-0.3.0.dev13/swarmauri/core/swarm_apis/ISwarmAPI.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/swarms/ISwarm.py` & `swarmauri-0.3.0.dev13/swarmauri/core/swarms/ISwarm.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/swarms/ISwarmAgentRegistration.py` & `swarmauri-0.3.0.dev13/swarmauri/core/swarms/ISwarmAgentRegistration.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/swarms/ISwarmChainCRUD.py` & `swarmauri-0.3.0.dev13/swarmauri/core/swarms/ISwarmChainCRUD.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/swarms/ISwarmConfigurationExporter.py` & `swarmauri-0.3.0.dev13/swarmauri/core/swarms/ISwarmConfigurationExporter.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/swarms/ISwarmFactory.py` & `swarmauri-0.3.0.dev13/swarmauri/core/swarms/ISwarmFactory.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/toolkits/IToolkit.py` & `swarmauri-0.3.0.dev13/swarmauri/core/toolkits/IToolkit.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/tools/IParameter.py` & `swarmauri-0.3.0.dev13/swarmauri/core/tools/IParameter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC, abstractmethod
-from typing import Optional, List, Any
+from typing import Optional, List, Any, Union
 
 class IParameter(ABC):
     """
     An abstract class to represent a parameter for a tool.
     """
 
     @property
@@ -68,20 +68,20 @@
         """
         Abstract setter for setting the required status of the parameter.
         """
         pass
 
     @property
     @abstractmethod
-    def enum(self) -> Optional[List[Any]]:
+    def enum(self) -> Union[List[str], None]:
         """
         Abstract property for getting the enum list of the parameter.
         """
         pass
 
     @enum.setter
     @abstractmethod
-    def enum(self, value: Optional[List[Any]]):
+    def enum(self, value: List[str]):
         """
         Abstract setter for setting the enum list of the parameter.
         """
         pass
```

### Comparing `swarmauri-0.2.9/swarmauri/core/tracing/IChainTracer.py` & `swarmauri-0.3.0.dev13/swarmauri/core/tracing/IChainTracer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/tracing/ITraceContext.py` & `swarmauri-0.3.0.dev13/swarmauri/core/tracing/ITraceContext.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/tracing/ITracer.py` & `swarmauri-0.3.0.dev13/swarmauri/core/tracing/ITracer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/utils/ITransactional.py` & `swarmauri-0.3.0.dev13/swarmauri/core/utils/ITransactional.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/vector_stores/IAngleBetweenVectors.py` & `swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/IAngleBetweenVectors.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/vector_stores/IDecompose.py` & `swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/IDecompose.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/vector_stores/IDivergence.py` & `swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/IDivergence.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/vector_stores/IGradient.py` & `swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/IGradient.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/vector_stores/IOrthogonalProject.py` & `swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/IOrthogonalProject.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/vector_stores/IProject.py` & `swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/IProject.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/vector_stores/IReflect.py` & `swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/IReflect.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/vector_stores/ISaveLoadStore.py` & `swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/ISaveLoadStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/vector_stores/ISimilarity.py` & `swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/ISimilarity.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/vector_stores/ISimiliarityQuery.py` & `swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/ISimiliarityQuery.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/vector_stores/IVectorArithmetic.py` & `swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/IVectorArithmetic.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/vector_stores/IVectorBasisCheck.py` & `swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/IVectorBasisCheck.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/vector_stores/IVectorLinearCombination.py` & `swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/IVectorLinearCombination.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/vector_stores/IVectorNorm.py` & `swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/IVectorNorm.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/vector_stores/IVectorRetrieve.py` & `swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/IVectorRetrieve.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/vector_stores/IVectorRotate.py` & `swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/IVectorRotate.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/vector_stores/IVectorSpan.py` & `swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/IVectorSpan.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/vector_stores/IVectorStore.py` & `swarmauri-0.3.0.dev13/swarmauri/core/vector_stores/IVectorStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/vectorizers/ISaveModel.py` & `swarmauri-0.3.0.dev13/swarmauri/core/vectorizers/ISaveModel.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/vectorizers/IVectorize.py` & `swarmauri-0.3.0.dev13/swarmauri/core/vectorizers/IVectorize.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/vectors/IVector.py` & `swarmauri-0.3.0.dev13/swarmauri/core/vectors/IVector.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/vectors/IVectorMeta.py` & `swarmauri-0.3.0.dev13/swarmauri/core/vectors/IVectorMeta.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/vectors/IVectorProduct.py` & `swarmauri-0.3.0.dev13/swarmauri/core/vectors/IVectorProduct.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/core/vectors/IVectorTransform.py` & `swarmauri-0.3.0.dev13/swarmauri/core/vectors/IVectorTransform.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/experimental/chains/TypeAgnosticCallableChain.py` & `swarmauri-0.3.0.dev13/swarmauri/experimental/chains/TypeAgnosticCallableChain.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/experimental/conversations/ConsensusBuildingConversation.py` & `swarmauri-0.3.0.dev13/swarmauri/experimental/conversations/ConsensusBuildingConversation.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/experimental/conversations/SemanticConversation.py` & `swarmauri-0.3.0.dev13/swarmauri/experimental/conversations/SemanticConversation.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/experimental/distances/CanberraDistance.py` & `swarmauri-0.3.0.dev13/swarmauri/experimental/distances/CanberraDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/experimental/distances/ChebyshevDistance.py` & `swarmauri-0.3.0.dev13/swarmauri/experimental/distances/ChebyshevDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/experimental/distances/HaversineDistance.py` & `swarmauri-0.3.0.dev13/swarmauri/experimental/distances/HaversineDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/experimental/distances/ManhattanDistance.py` & `swarmauri-0.3.0.dev13/swarmauri/experimental/distances/ManhattanDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/experimental/distances/MinkowskiDistance.py` & `swarmauri-0.3.0.dev13/swarmauri/experimental/distances/MinkowskiDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/experimental/distances/SSASimilarity.py` & `swarmauri-0.3.0.dev13/swarmauri/experimental/distances/SSASimilarity.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/experimental/distances/SSIVSimilarity.py` & `swarmauri-0.3.0.dev13/swarmauri/experimental/distances/SSIVSimilarity.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/experimental/distances/ScannVectorStore.py` & `swarmauri-0.3.0.dev13/swarmauri/experimental/distances/ScannVectorStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/experimental/distances/SorensenDiceDistance.py` & `swarmauri-0.3.0.dev13/swarmauri/experimental/distances/SorensenDiceDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/experimental/distances/SquaredEuclideanDistance.py` & `swarmauri-0.3.0.dev13/swarmauri/experimental/distances/SquaredEuclideanDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/experimental/document_stores/TriplesDocumentStore.py` & `swarmauri-0.3.0.dev13/swarmauri/experimental/document_stores/TriplesDocumentStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/experimental/document_stores/Word2VecDocumentStore.py` & `swarmauri-0.3.0.dev13/swarmauri/experimental/document_stores/Word2VecDocumentStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/experimental/models/HierarchicalAttentionModel.py` & `swarmauri-0.3.0.dev13/swarmauri/experimental/models/HierarchicalAttentionModel.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/experimental/models/SageMaker.py` & `swarmauri-0.3.0.dev13/swarmauri/experimental/models/SageMaker.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/experimental/parsers/PDFToTextParser.py` & `swarmauri-0.3.0.dev13/swarmauri/experimental/parsers/PDFToTextParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/experimental/tools/CypherQueryTool.py` & `swarmauri-0.3.0.dev13/swarmauri/experimental/tools/CypherQueryTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/experimental/tools/FileDownloaderTool.py` & `swarmauri-0.3.0.dev13/swarmauri/experimental/tools/FileDownloaderTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/experimental/tools/LinkedInArticleTool.py` & `swarmauri-0.3.0.dev13/swarmauri/experimental/tools/LinkedInArticleTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/experimental/tools/OutlookSendMailTool.py` & `swarmauri-0.3.0.dev13/swarmauri/experimental/tools/OutlookSendMailTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/experimental/tools/SQLite3QueryTool.py` & `swarmauri-0.3.0.dev13/swarmauri/experimental/tools/SQLite3QueryTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/experimental/tools/TwitterPostTool.py` & `swarmauri-0.3.0.dev13/swarmauri/experimental/tools/TwitterPostTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/experimental/tracing/RemoteTrace.py` & `swarmauri-0.3.0.dev13/swarmauri/experimental/tracing/RemoteTrace.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/experimental/utils/ISerializable.py` & `swarmauri-0.3.0.dev13/swarmauri/experimental/utils/ISerializable.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/experimental/utils/get_last_frame.py` & `swarmauri-0.3.0.dev13/swarmauri/experimental/utils/get_last_frame.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/experimental/utils/log_prompt_response.py` & `swarmauri-0.3.0.dev13/swarmauri/experimental/utils/log_prompt_response.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/experimental/utils/save_schema.py` & `swarmauri-0.3.0.dev13/swarmauri/experimental/utils/save_schema.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/experimental/vector_stores/TriplesDocumentStore.py` & `swarmauri-0.3.0.dev13/swarmauri/experimental/vector_stores/TriplesDocumentStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/experimental/vector_stores/Word2VecDocumentStore.py` & `swarmauri-0.3.0.dev13/swarmauri/experimental/vector_stores/Word2VecDocumentStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/experimental/vectorizers/DGLVectorizer.py` & `swarmauri-0.3.0.dev13/swarmauri/experimental/vectorizers/DGLVectorizer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/agent_factories/concrete/AgentFactory.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/agent_factories/concrete/AgentFactory.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/agent_factories/concrete/ConfDrivenAgentFactory.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/agent_factories/concrete/ConfDrivenAgentFactory.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/agent_factories/concrete/JsonAgentFactory.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/agent_factories/concrete/JsonAgentFactory.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/agent_factories/concrete/ReflectiveAgentFactory.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/agent_factories/concrete/ReflectiveAgentFactory.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/agents/base/AgentBase.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/agents/base/AgentBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/agents/base/SystemContextAgentBase.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/agents/base/SystemContextAgentBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/agents/base/VectorStoreAgentBase.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/agents/base/VectorStoreAgentBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/agents/concrete/ChatSwarmAgent.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/agents/concrete/ChatSwarmAgent.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/agents/concrete/MultiPartyChatSwarmAgent.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/agents/concrete/MultiPartyChatSwarmAgent.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/agents/concrete/MultiPartyToolAgent.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/agents/concrete/MultiPartyToolAgent.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/agents/concrete/RagAgent.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/agents/concrete/RagAgent.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/agents/concrete/SimpleConversationAgent.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/agents/concrete/SimpleConversationAgent.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/agents/concrete/ToolAgent.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/agents/concrete/ToolAgent.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/chains/base/ChainBase.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/chains/base/ChainBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/chains/base/ChainContextBase.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/chains/base/ChainContextBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/chains/base/ChainStepBase.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/chains/base/ChainStepBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/chains/base/PromptContextChainBase.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/chains/base/PromptContextChainBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/chains/concrete/CallableChain.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/chains/concrete/CallableChain.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/chains/concrete/ChainStep.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/chains/concrete/ChainStep.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/chains/concrete/ContextChain.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/chains/concrete/ContextChain.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/chains/concrete/PromptContextChain.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/chains/concrete/PromptContextChain.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/chunkers/concrete/DelimiterBasedChunker.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/chunkers/concrete/DelimiterBasedChunker.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/chunkers/concrete/FixedLengthChunker.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/chunkers/concrete/FixedLengthChunker.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/chunkers/concrete/MdSnippetChunker.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/chunkers/concrete/MdSnippetChunker.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/chunkers/concrete/SimpleSentenceChunker.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/chunkers/concrete/SimpleSentenceChunker.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/chunkers/concrete/SlidingWindowChunker.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/chunkers/concrete/SlidingWindowChunker.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/conversations/base/ConversationBase.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/conversations/base/ConversationBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/conversations/base/SystemContextBase.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/conversations/base/SystemContextBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/conversations/concrete/LimitedSizeConversation.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/conversations/concrete/LimitedSizeConversation.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/conversations/concrete/LimitedSystemContextConversation.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/conversations/concrete/LimitedSystemContextConversation.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/conversations/concrete/MaxSizeConversation.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/conversations/concrete/MaxSizeConversation.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/conversations/concrete/MaxSystemContextConversation.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/conversations/concrete/MaxSystemContextConversation.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/conversations/concrete/SessionCacheConversation.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/conversations/concrete/SessionCacheConversation.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/conversations/concrete/SharedConversation.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/conversations/concrete/SharedConversation.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/distances/concrete/ChiSquaredDistance.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/distances/concrete/ChiSquaredDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/distances/concrete/CosineDistance.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/distances/concrete/CosineDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/distances/concrete/EuclideanDistance.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/distances/concrete/EuclideanDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/distances/concrete/JaccardIndexDistance.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/distances/concrete/JaccardIndexDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/distances/concrete/LevenshteinDistance.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/distances/concrete/LevenshteinDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/document_stores/base/DocumentStoreBase.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/document_stores/base/DocumentStoreBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/document_stores/base/DocumentStoreRetrieveBase.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/document_stores/base/DocumentStoreRetrieveBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/documents/base/DocumentBase.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/documents/base/DocumentBase.py`

 * *Files 7% similar despite different names*

```diff
@@ -66,7 +66,15 @@
                 'content': self.content, 
                 'metadata': self.metadata}
       
     @classmethod
     def from_dict(cls, data):
         data.pop("type", None)
         return cls(**data)
+
+    def __setitem__(self, key, value):
+        """Allow setting items like a dict for metadata."""
+        self.metadata[key] = value
+
+    def __getitem__(self, key):
+        """Allow getting items like a dict for metadata."""
+        return self.metadata.get(key)
```

### Comparing `swarmauri-0.2.9/swarmauri/standard/documents/base/EmbeddedBase.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/documents/base/EmbeddedBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/exceptions/concrete/IndexErrorWithContext.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/exceptions/concrete/IndexErrorWithContext.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/messages/base/MessageBase.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/messages/base/MessageBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/messages/concrete/FunctionMessage.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/messages/concrete/FunctionMessage.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/messages/concrete/HumanMessage.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/messages/concrete/HumanMessage.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/messages/concrete/SystemMessage.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/messages/concrete/SystemMessage.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/metrics/base/AggregateMetricBase.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/metrics/base/AggregateMetricBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/metrics/base/CalculateMetricBase.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/metrics/base/CalculateMetricBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/metrics/base/MetricBase.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/metrics/concrete/MeanMetric.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,59 +1,48 @@
-from typing import Any
-from abc import ABC, abstractmethod
-from swarmauri.core.metrics.IMetric import IMetric
+from swarmauri.standard.metrics.base.AggregateMetricBase import AggregateMetricBase
 
-class MetricBase(IMetric, ABC):
-    """
-    A base implementation of the IMetric interface that provides the foundation
-    for specific metric implementations.
+class MeanMetric(AggregateMetricBase):
     """
+    A metric that calculates the mean (average) of a list of numerical values.
 
+    Attributes:
+        name (str): The name of the metric.
+        unit (str): The unit of measurement for the mean (e.g., "degrees", "points").
+        _value (float): The calculated mean of the measurements.
+        _measurements (list): A list of measurements (numerical values) to average.
+    """
     def __init__(self, name: str, unit: str):
         """
-        Initializes the metric with a name and unit of measurement.
+        Initialize the MeanMetric with its name and unit.
 
         Args:
-            name (str): The name of the metric.
-            unit (str): The unit of measurement for the metric (e.g., 'seconds', 'accuracy').
-        """
-        self._name = name
-        self._unit = unit
-        self._value = None  # Initialize with None, or a default value as appropriate
-
-    @property
-    def name(self) -> str:
-        """
-        The metric's name identifier.
-        """
-        return self._name
-
-    @property
-    def value(self) -> Any:
+            name (str): The name identifier for the metric.
+            unit (str): The unit of measurement for the mean.
         """
-        The current value of the metric.
+        # Calling the constructor of the base class
+        super().__init__(name, unit)
+    
+    def add_measurement(self, measurement) -> None:
         """
-        return self._value
+        Adds a measurement to the internal list of measurements.
 
-    @property
-    def unit(self) -> str:
-        """
-        The unit of measurement for the metric.
-        """
-        return self._unit
-
-    @unit.setter
-    def unit(self, value: str) -> None:
-        """
-        Set the unit of measurement for the metric.
+        Args:
+            measurement (float): A numerical value to be added to the list of measurements.
         """
-        self._unit = value
+        # Append the measurement to the internal list
+        self._measurements.append(measurement)
 
-    @abstractmethod
-    def __call__(self, **kwargs) -> Any:
+    def calculate(self) -> float:
         """
-        Retrieves the current value of the metric.
-
+        Calculate the mean of all added measurements.
+        
         Returns:
-            The current value of the metric.
+            float: The mean of the measurements or None if no measurements have been added.
         """
-        return self.value
+        if not self._measurements:
+            return None  # Return None if there are no measurements
+        # Calculate the mean
+        mean = sum(self._measurements) / len(self._measurements)
+        # Update the metric's value
+        self.update(mean)
+        # Return the calculated mean
+        return mean
```

### Comparing `swarmauri-0.2.9/swarmauri/standard/metrics/base/ThresholdMetricBase.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/metrics/base/ThresholdMetricBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/metrics/concrete/FirstImpressionMetric.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/metrics/concrete/FirstImpressionMetric.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/metrics/concrete/HitRateAtK.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/metrics/concrete/HitRateAtK.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/metrics/concrete/ImpressionAtK.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/metrics/concrete/ImpressionAtK.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/metrics/concrete/StaticValueMetric.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/metrics/concrete/StaticValueMetric.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/metrics/concrete/SystemUsabilityScaleMetric.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/metrics/concrete/SystemUsabilityScaleMetric.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/metrics/concrete/TaskSuccessRateMetric.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/metrics/concrete/TaskSuccessRateMetric.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/metrics/concrete/ThresholdMeanMetric.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/metrics/concrete/ThresholdMeanMetric.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/metrics/concrete/TimeOnTaskMetric.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/metrics/concrete/TimeOnTaskMetric.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/metrics/concrete/ZeroMetric.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/metrics/concrete/ZeroMetric.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/models/base/ModelBase.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/models/base/ModelBase.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import ABC, abstractmethod
 from typing import Any
-from ....core.models.IModel import IModel
+from swarmauri.core.models.IModel import IModel
 
 class ModelBase(IModel, ABC):
     """
     Concrete implementation of the IModel abstract base class.
     This version includes managing the model name through a property and a setter.
     """
     @abstractmethod
```

### Comparing `swarmauri-0.2.9/swarmauri/standard/models/concrete/AnthropicModel.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/models/concrete/AnthropicModel.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/models/concrete/AzureGPT.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/models/concrete/AzureGPT.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/models/concrete/CohereModel.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/models/concrete/CohereModel.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/models/concrete/GeminiProModel.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/models/concrete/GeminiProModel.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/models/concrete/GroqModel.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/models/concrete/GroqModel.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/models/concrete/GroqToolModel.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/models/concrete/GroqToolModel.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/models/concrete/MistralModel.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/models/concrete/MistralModel.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/models/concrete/MistralToolModel.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/models/concrete/MistralToolModel.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/models/concrete/OpenAIImageGenerator.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/models/concrete/OpenAIImageGenerator.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/models/concrete/OpenAIModel.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/models/concrete/OpenAIModel.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/models/concrete/OpenAIToolModel.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/models/concrete/OpenAIToolModel.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/parsers/concrete/BERTEmbeddingParser.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/parsers/concrete/BERTEmbeddingParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/parsers/concrete/CSVParser.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/parsers/concrete/CSVParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/parsers/concrete/EntityRecognitionParser.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/parsers/concrete/EntityRecognitionParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/parsers/concrete/HtmlTagStripParser.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/parsers/concrete/HtmlTagStripParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/parsers/concrete/KeywordExtractorParser.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/parsers/concrete/KeywordExtractorParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/parsers/concrete/MarkdownParser.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/parsers/concrete/MarkdownParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/parsers/concrete/OpenAPISpecParser.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/parsers/concrete/OpenAPISpecParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/parsers/concrete/PhoneNumberExtractorParser.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/parsers/concrete/PhoneNumberExtractorParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/parsers/concrete/PythonParser.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/parsers/concrete/PythonParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/parsers/concrete/RegExParser.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/parsers/concrete/RegExParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/parsers/concrete/TFIDFParser.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/parsers/concrete/TFIDFParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/parsers/concrete/TextBlobNounParser.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/parsers/concrete/TextBlobNounParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/parsers/concrete/TextBlobSentenceParser.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/parsers/concrete/TextBlobSentenceParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/parsers/concrete/URLExtractorParser.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/parsers/concrete/URLExtractorParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/parsers/concrete/XMLParser.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/parsers/concrete/XMLParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/prompts/base/BasePromptMatrix.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/prompts/base/BasePromptMatrix.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/prompts/concrete/Prompt.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/prompts/concrete/Prompt.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/prompts/concrete/PromptGenerator.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/prompts/concrete/PromptGenerator.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/prompts/concrete/PromptTemplate.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/prompts/concrete/PromptTemplate.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/swarms/base/SwarmComponentBase.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/swarms/base/SwarmComponentBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/swarms/concrete/SimpleSwarmFactory.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/swarms/concrete/SimpleSwarmFactory.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/toolkits/base/ToolkitBase.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/toolkits/base/ToolkitBase.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC, abstractmethod
 from typing import Dict
-from ....core.toolkits.IToolkit import IToolkit
-from ....core.tools.ITool import ITool  
+from swarmauri.core.toolkits.IToolkit import IToolkit
+from swarmauri.core.tools.ITool import ITool  
 
 class ToolkitBase(IToolkit, ABC):
     """
     A class representing a toolkit used by Swarm Agents.
     Tools are maintained in a dictionary keyed by the tool's name.
     """
```

### Comparing `swarmauri-0.2.9/swarmauri/standard/tools/concrete/AdditionTool.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/tools/concrete/AdditionTool.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-from ..base.ToolBase import ToolBase
-from .Parameter import Parameter
+from typing import List
+from dataclasses import dataclass, field
+from swarmauri.standard.tools.base.ToolBase import ToolBase 
+from swarmauri.standard.tools.concrete.Parameter import Parameter
 
+@dataclass
 class AdditionTool(ToolBase):
-    
-    def __init__(self):
-        parameters = [
+    version: str = "0.0.1"
+    parameters: List[Parameter] = field(default_factory=lambda: [
             Parameter(
                 name="x",
                 type="integer",
                 description="The left operand",
                 required=True
             ),
             Parameter(
                 name="y",
                 type="integer",
                 description="The right operand",
                 required=True
             )
-        ]
-        super().__init__(name="TestTool", 
-                         description="This opens a program based on the user's request.", 
-                         parameters=parameters)
+        ])
+
+    description: str = "This tool has two numbers together"
+
 
     def __call__(self, x: int, y: int) -> int:
         """
         Add two numbers x and y and return the sum.
 
         Parameters:
         - x (int): The first number.
         - y (int): The second number.
 
         Returns:
-        - int: The sum of x and y.
+        - str: The sum of x and y.
         """
-        return x + y
+        return str(x + y)
```

### Comparing `swarmauri-0.2.9/swarmauri/standard/tools/concrete/CalculatorTool.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/tools/concrete/CalculatorTool.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,38 @@
-from swarmauri.standard.tools.base.ToolBase import ToolBase  # Adjust the import path as necessary
-from swarmauri.standard.tools.concrete.Parameter import Parameter
+from dataclasses import dataclass, field
+from typing import List, Optional
+from swarmauri.standard.tools.base.ToolBase import ToolBase, Parameter
 
+@dataclass
 class CalculatorTool(ToolBase):
-    def __init__(self):
-        parameters = [
-            Parameter(
-                name="operation",
-                type="string",
-                description="The arithmetic operation to perform ('add', 'subtract', 'multiply', 'divide').",
-                required=True,
-                enum=["add", "subtract", "multiply", "divide"]
-            ),
-            Parameter(
-                name="x",
-                type="number",
-                description="The left operand for the operation.",
-                required=True
-            ),
-            Parameter(
-                name="y",
-                type="number",
-                description="The right operand for the operation.",
-                required=True
-            )
-        ]
-        super().__init__(name="CalculatorTool", 
-                         description="Performs basic arithmetic operations.",
-                         parameters=parameters)
+    version: str = "1.0.0"
+    parameters: List[Parameter] = field(default_factory=lambda: [
+        Parameter(
+            name="operation",
+            type="string",
+            description="The arithmetic operation to perform ('add', 'subtract', 'multiply', 'divide').",
+            required=True,
+            enum=["add", "subtract", "multiply", "divide"]
+        ),
+        Parameter(
+            name="x",
+            type="number",
+            description="The left operand for the operation.",
+            required=True
+        ),
+        Parameter(
+            name="y",
+            type="number",
+            description="The right operand for the operation.",
+            required=True
+        )
+    ])
+    description: str = "Performs basic arithmetic operations."
 
     def __call__(self, operation: str, x: float, y: float) -> str:
-        """
-        Executes the specified arithmetic operation on the given operands.
-        
-        Parameters:
-            operation (str): The arithmetic operation to perform.
-            x (float): The left operand.
-            y (float): The right operand.
-        
-        Returns:
-            str: Result of the arithmetic operation.
-        """
         try:
             if operation == "add":
                 result = x + y
             elif operation == "subtract":
                 result = x - y
             elif operation == "multiply":
                 result = x * y
@@ -51,8 +40,8 @@
                 if y == 0:
                     return "Error: Division by zero."
                 result = x / y
             else:
                 return "Error: Unknown operation."
             return str(result)
         except Exception as e:
-            return f"An error occurred: {str(e)}"
+            return f"An error occurred: {str(e)}"
```

### Comparing `swarmauri-0.2.9/swarmauri/standard/tools/concrete/CodeInterpreterTool.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/tools/concrete/CodeInterpreterTool.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import sys
 import io
-from swarmauri.standard.tools.base.ToolBase import ToolBase  # Adjust the import path as necessary
-from swarmauri.standard.tools.concrete.Parameter import Parameter  # Assuming a parameter structure is used
+from dataclasses import dataclass, field
+from typing import List
+from swarmauri.standard.tools.base.ToolBase import ToolBase 
+from swarmauri.standard.tools.concrete.Parameter import Parameter 
 
+@dataclass
 class CodeInterpreterTool(ToolBase):
-    def __init__(self):
-        # Example of initializing the tool with parameters if necessary
-        parameters = [
+    version: str = "1.0.0"
+    parameters: List[Parameter] = field(default_factory=lambda: [
             Parameter(
                 name="user_code",
                 type="string",
                 description=("Executes the provided Python code snippet in a secure sandbox environment. "
                              "This tool is designed to interpret the execution of the python code snippet."
                              "Returns the output"),
                 required=True
             )
-        ]
-        super().__init__(name="CodeInterpreterTool", 
-                         description="Executes provided Python code and captures its output.",
-                         parameters=parameters)
+        ])
+    description: str = "Executes provided Python code and captures its output."
+    
+
 
     def __call__(self, user_code: str) -> str:
         """
         Executes the provided user code and captures its stdout output.
         
         Parameters:
             user_code (str): Python code to be executed.
```

### Comparing `swarmauri-0.2.9/swarmauri/standard/tools/concrete/ImportMemoryModuleTool.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/tools/concrete/ImportMemoryModuleTool.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-# standard/tools/concrete/ImportMemoryModuleTool.py
 import sys
 import types
 import importlib
-from swarmauri.standard.tools.base.ToolBase import ToolBase
-from swarmauri.standard.tools.concrete.Parameter import Parameter
-
+from dataclasses import dataclass, field
+from typing import List
+from swarmauri.standard.tools.base.ToolBase import ToolBase 
+from swarmauri.standard.tools.concrete.Parameter import Parameter 
 
+@dataclass
 class ImportMemoryModuleTool(ToolBase):
-    def __init__(self):
-        # Define the parameters required by the tool
-        parameters = [
+    version: str = "1.0.0"
+    
+    # Define the parameters required by the tool
+    parameters: List[Parameter] = field(default_factory=lambda: [
             Parameter(
                 name="name",
                 type="string",
                 description="Name of the new module.",
                 required=True
             ),
             Parameter(
@@ -24,20 +26,18 @@
             ),
             Parameter(
                 name="package_path",
                 type="string",
                 description="Dot-separated package path where the new module should be inserted.",
                 required=True
             )
-        ]
+        ])
         
-        # Call the ToolBase initializer
-        super().__init__(name="ImportMemoryModuleTool", 
-                         description="Dynamically imports a module from memory into a specified package path.",
-                         parameters=parameters)
+    description: str = "Dynamically imports a module from memory into a specified package path."
+    
 
     def __call__(self, name: str, code: str, package_path: str) -> str:
         """
         Dynamically creates a module from a code snippet and inserts it into the specified package path.
 
         Args:
             name (str): Name of the new module.
```

### Comparing `swarmauri-0.2.9/swarmauri/standard/tools/concrete/TestTool.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/tools/concrete/TestTool.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,30 @@
+from typing import List
+from dataclasses import dataclass, field
 import json
 import subprocess as sp
-from ..base.ToolBase import ToolBase
-from .Parameter import Parameter
+from swarmauri.standard.tools.base.ToolBase import ToolBase 
+from swarmauri.standard.tools.concrete.Parameter import Parameter 
 
+@dataclass
 class TestTool(ToolBase):
-    def __init__(self):
-        parameters = [
-            Parameter(
-                name="program",
-                type="string",
-                description="The program that the user wants to open ('notepad' or 'calc' or 'mspaint')",
-                required=True,
-                enum=["notepad", "calc", "mspaint"]
-            )
-        ]
+    version: str = "1.0.0"
         
-        super().__init__(name="TestTool", 
-                         description="This opens a program based on the user's request.", 
-                         parameters=parameters)
+    # Define the parameters required by the tool
+    parameters: List[Parameter] = field(default_factory=lambda: [
+        Parameter(
+            name="program",
+            type="string",
+            description="The program that the user wants to open ('notepad' or 'calc' or 'mspaint')",
+            required=True,
+            enum=["notepad", "calc", "mspaint"]
+        )
+    ])
+    
+    description: str = "This opens a program based on the user's request."
+
 
     def __call__(self, program) -> str:
         # sp.check_output(program)
         # Here you would implement the actual logic for fetching the weather information.
         # For demonstration, let's just return the parameters as a string.
         return f"Program Opened: {program}\n"
```

### Comparing `swarmauri-0.2.9/swarmauri/standard/tracing/concrete/CallableTracer.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/tracing/concrete/CallableTracer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/tracing/concrete/ChainTracer.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/tracing/concrete/ChainTracer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/tracing/concrete/SimpleTraceContext.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/tracing/concrete/SimpleTraceContext.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/tracing/concrete/SimpleTracer.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/tracing/concrete/SimpleTracer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/tracing/concrete/TracedVariable.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/tracing/concrete/TracedVariable.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/tracing/concrete/VariableTracer.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/tracing/concrete/VariableTracer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/utils/decorate.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/utils/decorate.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/utils/get_class_hash.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/utils/get_class_hash.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/utils/json_validator.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/utils/json_validator.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/utils/load_documents_from_json.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/utils/load_documents_from_json.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/utils/sql_log.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/utils/sql_log.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/vector_stores/base/SaveLoadStoreBase.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/vector_stores/base/SaveLoadStoreBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/vector_stores/base/VectorDocumentStoreBase.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/vector_stores/base/VectorDocumentStoreBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/vector_stores/base/VectorDocumentStoreRetrieveBase.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/vector_stores/base/VectorDocumentStoreRetrieveBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/vector_stores/concrete/Doc2VecVectorStore.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/vector_stores/concrete/Doc2VecVectorStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/vector_stores/concrete/MLMVectorStore.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/vector_stores/concrete/MLMVectorStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/vector_stores/concrete/SpatialDocVectorStore.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/vector_stores/concrete/SpatialDocVectorStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/vector_stores/concrete/TFIDFVectorStore.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/vector_stores/concrete/TFIDFVectorStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/vectorizers/concrete/Doc2VecVectorizer.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/vectorizers/concrete/Doc2VecVectorizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from swarmauri.core.vectorizers.IVectorize import IVectorize
 from swarmauri.core.vectorizers.IFeature import IFeature
 from swarmauri.core.vectors.IVector import IVector
 from swarmauri.standard.vectors.concrete.SimpleVector import SimpleVector
 from swarmauri.core.vectorizers.ISaveModel import ISaveModel
 
 class Doc2VecVectorizer(IVectorize, IFeature, ISaveModel):
-    def __init__(self):
-        self.model = Doc2Vec(vector_size=2000, window=10, min_count=1, workers=5)
+    def __init__(self, vector_size = 2000):
+        self.model = Doc2Vec(vector_size=vector_size, window=10, min_count=1, workers=5)
 
     def extract_features(self):
         return list(self.model.wv.key_to_index.keys())
 
     def fit(self, documents: List[str], labels=None) -> None:
         tagged_data = [TaggedDocument(words=_d.split(), 
             tags=[str(i)]) for i, _d in enumerate(documents)]
```

### Comparing `swarmauri-0.2.9/swarmauri/standard/vectorizers/concrete/MLMVectorizer.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/vectorizers/concrete/MLMVectorizer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/vectorizers/concrete/NMFVectorizer.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/vectorizers/concrete/NMFVectorizer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/vectorizers/concrete/SpatialDocVectorizer.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/vectorizers/concrete/SpatialDocVectorizer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/vectorizers/concrete/TFIDFVectorizer.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/vectorizers/concrete/TFIDFVectorizer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/vectors/base/VectorBase.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/vectors/base/VectorBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri/standard/vectors/concrete/VectorProduct.py` & `swarmauri-0.3.0.dev13/swarmauri/standard/vectors/concrete/VectorProduct.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.2.9/swarmauri.egg-info/PKG-INFO` & `swarmauri-0.3.0.dev13/swarmauri.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarmauri
-Version: 0.2.9
+Version: 0.3.0.dev13
 Summary: This repository includes core interfaces, standard ABCs and concrete references, third party plugins, and experimental modules for the swarmaURI framework.
 Home-page: http://github.com/swarmauri/swarmauri-sdk
 Author: Jacob Stewart
 Author-email: corporate@swarmauri.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `swarmauri-0.2.9/swarmauri.egg-info/SOURCES.txt` & `swarmauri-0.3.0.dev13/swarmauri.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,19 @@
 swarmauri/community/tools/concrete/GmailReadTool.py
 swarmauri/community/tools/concrete/GmailSendTool.py
 swarmauri/community/tools/concrete/PaCMAP.py
 swarmauri/community/tools/concrete/SentimentAnalysisTool.py
 swarmauri/community/tools/concrete/WebScrapingTool.py
 swarmauri/community/tools/concrete/ZapierHookTool.py
 swarmauri/community/tools/concrete/__init__.py
+swarmauri/community/vector_stores/AnnoyVectorStore.py
+swarmauri/community/vector_stores/ChromadbVectorStore.py
+swarmauri/community/vector_stores/QdrantVectorStore.py
+swarmauri/community/vector_stores/__init__.py
+swarmauri/core/BaseComponent.py
 swarmauri/core/__init__.py
 swarmauri/core/agent_apis/IAgentCommands.py
 swarmauri/core/agent_apis/IAgentRouterCRUD.py
 swarmauri/core/agent_apis/__init__.py
 swarmauri/core/agent_factories/IAgentFactory.py
 swarmauri/core/agent_factories/IExportConf.py
 swarmauri/core/agent_factories/__init__.py
@@ -129,14 +134,15 @@
 swarmauri/core/vectorizers/IVectorize.py
 swarmauri/core/vectorizers/__init__.py
 swarmauri/core/vectors/IVector.py
 swarmauri/core/vectors/IVectorMeta.py
 swarmauri/core/vectors/IVectorProduct.py
 swarmauri/core/vectors/IVectorTransform.py
 swarmauri/core/vectors/__init__.py
+swarmauri/experimental/RemoteUniversalBase.py
 swarmauri/experimental/__init__.py
 swarmauri/experimental/chains/IChainFormatter.py
 swarmauri/experimental/chains/IChainNotification.py
 swarmauri/experimental/chains/IChainPersistence.py
 swarmauri/experimental/chains/IChainScheduler.py
 swarmauri/experimental/chains/TypeAgnosticCallableChain.py
 swarmauri/experimental/chains/__init__.py
@@ -340,14 +346,15 @@
 swarmauri/standard/swarms/concrete/__init__.py
 swarmauri/standard/toolkits/__init__.py
 swarmauri/standard/toolkits/base/ToolkitBase.py
 swarmauri/standard/toolkits/base/__init__.py
 swarmauri/standard/toolkits/concrete/Toolkit.py
 swarmauri/standard/toolkits/concrete/__init__.py
 swarmauri/standard/tools/__init__.py
+swarmauri/standard/tools/base/ParameterBase.py
 swarmauri/standard/tools/base/ToolBase.py
 swarmauri/standard/tools/base/__init__.py
 swarmauri/standard/tools/concrete/AdditionTool.py
 swarmauri/standard/tools/concrete/CalculatorTool.py
 swarmauri/standard/tools/concrete/CodeInterpreterTool.py
 swarmauri/standard/tools/concrete/ImportMemoryModuleTool.py
 swarmauri/standard/tools/concrete/Parameter.py
```

### Comparing `swarmauri-0.2.9/swarmauri.egg-info/requires.txt` & `swarmauri-0.3.0.dev13/swarmauri.egg-info/requires.txt`

 * *Files identical despite different names*

