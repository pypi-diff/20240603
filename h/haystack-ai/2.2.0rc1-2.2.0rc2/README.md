# Comparing `tmp/haystack_ai-2.2.0rc1.tar.gz` & `tmp/haystack_ai-2.2.0rc2.tar.gz`

## Comparing `haystack_ai-2.2.0rc1.tar` & `haystack_ai-2.2.0rc2.tar`

### file list

```diff
@@ -1,192 +1,192 @@
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/VERSION.txt
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/__init__.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/errors.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/lazy_imports.py
--rw-r--r--   0        0        0    13540 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/logging.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/version.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/__init__.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/audio/__init__.py
--rw-r--r--   0        0        0     7568 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/audio/whisper_local.py
--rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/audio/whisper_remote.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/builders/__init__.py
--rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/builders/answer_builder.py
--rw-r--r--   0        0        0    11033 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/builders/chat_prompt_builder.py
--rw-r--r--   0        0        0     9739 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/builders/dynamic_chat_prompt_builder.py
--rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/builders/dynamic_prompt_builder.py
--rw-r--r--   0        0        0     9940 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/builders/prompt_builder.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/caching/__init__.py
--rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/caching/cache_checker.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/classifiers/__init__.py
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/classifiers/document_language_classifier.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/connectors/__init__.py
--rw-r--r--   0        0        0    13952 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/connectors/openapi_service.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/converters/__init__.py
--rw-r--r--   0        0        0    24753 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/converters/azure.py
--rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/converters/html.py
--rw-r--r--   0        0        0     3962 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/converters/markdown.py
--rw-r--r--   0        0        0    11424 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/converters/openapi_functions.py
--rw-r--r--   0        0        0     5625 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/converters/output_adapter.py
--rw-r--r--   0        0        0     6703 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/converters/pdfminer.py
--rw-r--r--   0        0        0     6739 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/converters/pypdf.py
--rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/converters/tika.py
--rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/converters/txt.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/converters/utils.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/embedders/__init__.py
--rw-r--r--   0        0        0     9362 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/embedders/azure_document_embedder.py
--rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/embedders/azure_text_embedder.py
--rw-r--r--   0        0        0    11013 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/embedders/hugging_face_api_document_embedder.py
--rw-r--r--   0        0        0     8116 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/embedders/hugging_face_api_text_embedder.py
--rw-r--r--   0        0        0     8782 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/embedders/hugging_face_tei_document_embedder.py
--rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/embedders/hugging_face_tei_text_embedder.py
--rw-r--r--   0        0        0     8587 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/embedders/openai_document_embedder.py
--rw-r--r--   0        0        0     5889 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/embedders/openai_text_embedder.py
--rw-r--r--   0        0        0     7107 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/embedders/sentence_transformers_document_embedder.py
--rw-r--r--   0        0        0     5766 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/embedders/sentence_transformers_text_embedder.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/embedders/backends/__init__.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/embedders/backends/sentence_transformers_backend.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/evaluators/__init__.py
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/evaluators/answer_exact_match.py
--rw-r--r--   0        0        0     7202 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/evaluators/context_relevance.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/evaluators/document_map.py
--rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/evaluators/document_mrr.py
--rw-r--r--   0        0        0     4937 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/evaluators/document_recall.py
--rw-r--r--   0        0        0     8201 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/evaluators/faithfulness.py
--rw-r--r--   0        0        0    14488 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/evaluators/llm_evaluator.py
--rw-r--r--   0        0        0     8244 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/evaluators/sas_evaluator.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/extractors/__init__.py
--rw-r--r--   0        0        0    16470 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/extractors/named_entity_extractor.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/fetchers/__init__.py
--rw-r--r--   0        0        0     9573 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/fetchers/link_content.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/generators/__init__.py
--rw-r--r--   0        0        0     9435 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/generators/azure.py
--rw-r--r--   0        0        0    10023 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/generators/hugging_face_api.py
--rw-r--r--   0        0        0    11720 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/generators/hugging_face_local.py
--rw-r--r--   0        0        0    13515 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/generators/hugging_face_tgi.py
--rw-r--r--   0        0        0    14480 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/generators/openai.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/generators/utils.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/generators/chat/__init__.py
--rw-r--r--   0        0        0    10030 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/generators/chat/azure.py
--rw-r--r--   0        0        0    11302 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/generators/chat/hugging_face_api.py
--rw-r--r--   0        0        0    17938 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/generators/chat/hugging_face_local.py
--rw-r--r--   0        0        0    16274 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/generators/chat/hugging_face_tgi.py
--rw-r--r--   0        0        0    17962 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/generators/chat/openai.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/joiners/__init__.py
--rw-r--r--   0        0        0     6566 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/joiners/branch.py
--rw-r--r--   0        0        0     6954 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/joiners/document_joiner.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/others/__init__.py
--rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/others/multiplexer.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/preprocessors/__init__.py
--rw-r--r--   0        0        0    10489 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/preprocessors/document_cleaner.py
--rw-r--r--   0        0        0     6845 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/preprocessors/document_splitter.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/preprocessors/text_cleaner.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/rankers/__init__.py
--rw-r--r--   0        0        0     6213 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/rankers/lost_in_the_middle.py
--rw-r--r--   0        0        0    17159 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/rankers/meta_field.py
--rw-r--r--   0        0        0    11066 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/rankers/sentence_transformers_diversity.py
--rw-r--r--   0        0        0    11691 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/rankers/transformers_similarity.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/readers/__init__.py
--rw-r--r--   0        0        0    28999 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/readers/extractive.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/retrievers/__init__.py
--rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/retrievers/filter_retriever.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/retrievers/in_memory/__init__.py
--rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/retrievers/in_memory/bm25_retriever.py
--rw-r--r--   0        0        0     6217 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/retrievers/in_memory/embedding_retriever.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/routers/__init__.py
--rw-r--r--   0        0        0    10262 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/routers/conditional_router.py
--rw-r--r--   0        0        0     5931 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/routers/file_type_router.py
--rw-r--r--   0        0        0     4333 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/routers/metadata_router.py
--rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/routers/text_language_router.py
--rw-r--r--   0        0        0     9671 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/routers/zero_shot_text_router.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/samplers/__init__.py
--rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/samplers/top_p.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/validators/__init__.py
--rw-r--r--   0        0        0    10439 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/validators/json_schema.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/websearch/__init__.py
--rw-r--r--   0        0        0     6893 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/websearch/searchapi.py
--rw-r--r--   0        0        0     6861 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/websearch/serper_dev.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/writers/__init__.py
--rw-r--r--   0        0        0     4595 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/writers/document_writer.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/__init__.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/errors.py
--rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/serialization.py
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/type_utils.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/component/__init__.py
--rw-r--r--   0        0        0    18609 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/component/component.py
--rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/component/sockets.py
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/component/types.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/pipeline/__init__.py
--rw-r--r--   0        0        0    36291 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/pipeline/base.py
--rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/pipeline/descriptions.py
--rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/pipeline/draw.py
--rw-r--r--   0        0        0    21292 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/pipeline/pipeline.py
--rw-r--r--   0        0        0     5629 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/pipeline/template.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/pipeline/utils.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/pipeline/predefined/chat_with_website.yaml.jinja2
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/pipeline/predefined/generative_qa.yaml.jinja2
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/pipeline/predefined/indexing.yaml.jinja2
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/pipeline/predefined/rag.yaml.jinja2
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/dataclasses/__init__.py
--rw-r--r--   0        0        0     6074 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/dataclasses/answer.py
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/dataclasses/byte_stream.py
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/dataclasses/chat_message.py
--rw-r--r--   0        0        0     8500 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/dataclasses/document.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/dataclasses/sparse_embedding.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/dataclasses/streaming_chunk.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/document_stores/__init__.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/document_stores/errors/__init__.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/document_stores/errors/errors.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/document_stores/in_memory/__init__.py
--rw-r--r--   0        0        0    23733 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/document_stores/in_memory/document_store.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/document_stores/types/__init__.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/document_stores/types/policy.py
--rw-r--r--   0        0        0     4888 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/document_stores/types/protocol.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/evaluation/__init__.py
--rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/evaluation/eval_run_result.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/marshal/__init__.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/marshal/protocol.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/marshal/yaml.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/telemetry/__init__.py
--rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/telemetry/_environment.py
--rw-r--r--   0        0        0     7495 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/telemetry/_telemetry.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/__init__.py
--rw-r--r--   0        0        0    63265 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/document_store.py
--rw-r--r--   0        0        0     8160 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/factory.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/test_utils.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/sample_components/__init__.py
--rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/sample_components/accumulate.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/sample_components/add_value.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/sample_components/concatenate.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/sample_components/double.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/sample_components/fstring.py
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/sample_components/greet.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/sample_components/hello.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/sample_components/joiner.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/sample_components/parity.py
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/sample_components/remainder.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/sample_components/repeat.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/sample_components/self_loop.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/sample_components/subtract.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/sample_components/sum.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/sample_components/text_splitter.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/sample_components/threshold.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/tracing/__init__.py
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/tracing/datadog.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/tracing/opentelemetry.py
--rw-r--r--   0        0        0     7794 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/tracing/tracer.py
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/tracing/utils.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/utils/__init__.py
--rw-r--r--   0        0        0     6710 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/utils/auth.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/utils/callable_serialization.py
--rw-r--r--   0        0        0    15539 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/utils/device.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/utils/expit.py
--rw-r--r--   0        0        0    11846 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/utils/filters.py
--rw-r--r--   0        0        0    15621 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/utils/hf.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/utils/jupyter.py
--rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/utils/requests_utils.py
--rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/utils/type_serialization.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/utils/url_validation.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/.gitignore
--rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/LICENSE
--rw-r--r--   0        0        0    11365 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/README.md
--rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/pyproject.toml
--rw-r--r--   0        0        0    13236 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/PKG-INFO
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/VERSION.txt
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/__init__.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/errors.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/lazy_imports.py
+-rw-r--r--   0        0        0    13540 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/logging.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/version.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/__init__.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/audio/__init__.py
+-rw-r--r--   0        0        0     7568 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/audio/whisper_local.py
+-rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/audio/whisper_remote.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/builders/__init__.py
+-rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/builders/answer_builder.py
+-rw-r--r--   0        0        0    11033 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/builders/chat_prompt_builder.py
+-rw-r--r--   0        0        0     9739 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/builders/dynamic_chat_prompt_builder.py
+-rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/builders/dynamic_prompt_builder.py
+-rw-r--r--   0        0        0     9940 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/builders/prompt_builder.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/caching/__init__.py
+-rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/caching/cache_checker.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/classifiers/__init__.py
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/classifiers/document_language_classifier.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/connectors/__init__.py
+-rw-r--r--   0        0        0    13952 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/connectors/openapi_service.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/converters/__init__.py
+-rw-r--r--   0        0        0    24753 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/converters/azure.py
+-rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/converters/html.py
+-rw-r--r--   0        0        0     3962 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/converters/markdown.py
+-rw-r--r--   0        0        0    11424 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/converters/openapi_functions.py
+-rw-r--r--   0        0        0     5625 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/converters/output_adapter.py
+-rw-r--r--   0        0        0     6703 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/converters/pdfminer.py
+-rw-r--r--   0        0        0     6739 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/converters/pypdf.py
+-rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/converters/tika.py
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/converters/txt.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/converters/utils.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/embedders/__init__.py
+-rw-r--r--   0        0        0     9362 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/embedders/azure_document_embedder.py
+-rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/embedders/azure_text_embedder.py
+-rw-r--r--   0        0        0    11013 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/embedders/hugging_face_api_document_embedder.py
+-rw-r--r--   0        0        0     8116 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/embedders/hugging_face_api_text_embedder.py
+-rw-r--r--   0        0        0     8782 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/embedders/hugging_face_tei_document_embedder.py
+-rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/embedders/hugging_face_tei_text_embedder.py
+-rw-r--r--   0        0        0     8587 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/embedders/openai_document_embedder.py
+-rw-r--r--   0        0        0     5889 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/embedders/openai_text_embedder.py
+-rw-r--r--   0        0        0     7107 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/embedders/sentence_transformers_document_embedder.py
+-rw-r--r--   0        0        0     5766 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/embedders/sentence_transformers_text_embedder.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/embedders/backends/__init__.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/embedders/backends/sentence_transformers_backend.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/evaluators/__init__.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/evaluators/answer_exact_match.py
+-rw-r--r--   0        0        0     7202 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/evaluators/context_relevance.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/evaluators/document_map.py
+-rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/evaluators/document_mrr.py
+-rw-r--r--   0        0        0     4937 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/evaluators/document_recall.py
+-rw-r--r--   0        0        0     8201 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/evaluators/faithfulness.py
+-rw-r--r--   0        0        0    14488 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/evaluators/llm_evaluator.py
+-rw-r--r--   0        0        0     8244 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/evaluators/sas_evaluator.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/extractors/__init__.py
+-rw-r--r--   0        0        0    16470 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/extractors/named_entity_extractor.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/fetchers/__init__.py
+-rw-r--r--   0        0        0     9573 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/fetchers/link_content.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/generators/__init__.py
+-rw-r--r--   0        0        0     9435 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/generators/azure.py
+-rw-r--r--   0        0        0    10023 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/generators/hugging_face_api.py
+-rw-r--r--   0        0        0    11720 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/generators/hugging_face_local.py
+-rw-r--r--   0        0        0    13515 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/generators/hugging_face_tgi.py
+-rw-r--r--   0        0        0    14480 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/generators/openai.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/generators/utils.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/generators/chat/__init__.py
+-rw-r--r--   0        0        0    10030 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/generators/chat/azure.py
+-rw-r--r--   0        0        0    11302 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/generators/chat/hugging_face_api.py
+-rw-r--r--   0        0        0    17938 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/generators/chat/hugging_face_local.py
+-rw-r--r--   0        0        0    16274 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/generators/chat/hugging_face_tgi.py
+-rw-r--r--   0        0        0    17962 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/generators/chat/openai.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/joiners/__init__.py
+-rw-r--r--   0        0        0     6566 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/joiners/branch.py
+-rw-r--r--   0        0        0     6954 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/joiners/document_joiner.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/others/__init__.py
+-rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/others/multiplexer.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/preprocessors/__init__.py
+-rw-r--r--   0        0        0    10489 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/preprocessors/document_cleaner.py
+-rw-r--r--   0        0        0     6845 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/preprocessors/document_splitter.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/preprocessors/text_cleaner.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/rankers/__init__.py
+-rw-r--r--   0        0        0     6213 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/rankers/lost_in_the_middle.py
+-rw-r--r--   0        0        0    17159 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/rankers/meta_field.py
+-rw-r--r--   0        0        0    11066 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/rankers/sentence_transformers_diversity.py
+-rw-r--r--   0        0        0    11691 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/rankers/transformers_similarity.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/readers/__init__.py
+-rw-r--r--   0        0        0    28999 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/readers/extractive.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/retrievers/__init__.py
+-rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/retrievers/filter_retriever.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/retrievers/in_memory/__init__.py
+-rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/retrievers/in_memory/bm25_retriever.py
+-rw-r--r--   0        0        0     6217 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/retrievers/in_memory/embedding_retriever.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/routers/__init__.py
+-rw-r--r--   0        0        0    10262 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/routers/conditional_router.py
+-rw-r--r--   0        0        0     5931 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/routers/file_type_router.py
+-rw-r--r--   0        0        0     4333 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/routers/metadata_router.py
+-rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/routers/text_language_router.py
+-rw-r--r--   0        0        0     9671 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/routers/zero_shot_text_router.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/samplers/__init__.py
+-rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/samplers/top_p.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/validators/__init__.py
+-rw-r--r--   0        0        0    10439 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/validators/json_schema.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/websearch/__init__.py
+-rw-r--r--   0        0        0     6893 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/websearch/searchapi.py
+-rw-r--r--   0        0        0     6861 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/websearch/serper_dev.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/writers/__init__.py
+-rw-r--r--   0        0        0     4595 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/components/writers/document_writer.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/core/__init__.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/core/errors.py
+-rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/core/serialization.py
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/core/type_utils.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/core/component/__init__.py
+-rw-r--r--   0        0        0    18609 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/core/component/component.py
+-rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/core/component/sockets.py
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/core/component/types.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/core/pipeline/__init__.py
+-rw-r--r--   0        0        0    36291 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/core/pipeline/base.py
+-rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/core/pipeline/descriptions.py
+-rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/core/pipeline/draw.py
+-rw-r--r--   0        0        0    21292 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/core/pipeline/pipeline.py
+-rw-r--r--   0        0        0     5629 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/core/pipeline/template.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/core/pipeline/utils.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/core/pipeline/predefined/chat_with_website.yaml.jinja2
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/core/pipeline/predefined/generative_qa.yaml.jinja2
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/core/pipeline/predefined/indexing.yaml.jinja2
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/core/pipeline/predefined/rag.yaml.jinja2
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/dataclasses/__init__.py
+-rw-r--r--   0        0        0     6074 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/dataclasses/answer.py
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/dataclasses/byte_stream.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/dataclasses/chat_message.py
+-rw-r--r--   0        0        0     8500 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/dataclasses/document.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/dataclasses/sparse_embedding.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/dataclasses/streaming_chunk.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/document_stores/__init__.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/document_stores/errors/__init__.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/document_stores/errors/errors.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/document_stores/in_memory/__init__.py
+-rw-r--r--   0        0        0    23733 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/document_stores/in_memory/document_store.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/document_stores/types/__init__.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/document_stores/types/policy.py
+-rw-r--r--   0        0        0     4888 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/document_stores/types/protocol.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/evaluation/__init__.py
+-rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/evaluation/eval_run_result.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/marshal/__init__.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/marshal/protocol.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/marshal/yaml.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/telemetry/__init__.py
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/telemetry/_environment.py
+-rw-r--r--   0        0        0     7495 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/telemetry/_telemetry.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/testing/__init__.py
+-rw-r--r--   0        0        0    63265 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/testing/document_store.py
+-rw-r--r--   0        0        0     8160 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/testing/factory.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/testing/test_utils.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/testing/sample_components/__init__.py
+-rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/testing/sample_components/accumulate.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/testing/sample_components/add_value.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/testing/sample_components/concatenate.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/testing/sample_components/double.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/testing/sample_components/fstring.py
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/testing/sample_components/greet.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/testing/sample_components/hello.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/testing/sample_components/joiner.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/testing/sample_components/parity.py
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/testing/sample_components/remainder.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/testing/sample_components/repeat.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/testing/sample_components/self_loop.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/testing/sample_components/subtract.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/testing/sample_components/sum.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/testing/sample_components/text_splitter.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/testing/sample_components/threshold.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/tracing/__init__.py
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/tracing/datadog.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/tracing/opentelemetry.py
+-rw-r--r--   0        0        0     7794 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/tracing/tracer.py
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/tracing/utils.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/utils/__init__.py
+-rw-r--r--   0        0        0     6710 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/utils/auth.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/utils/callable_serialization.py
+-rw-r--r--   0        0        0    15539 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/utils/device.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/utils/expit.py
+-rw-r--r--   0        0        0    11846 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/utils/filters.py
+-rw-r--r--   0        0        0    15621 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/utils/hf.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/utils/jupyter.py
+-rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/utils/requests_utils.py
+-rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/utils/type_serialization.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/haystack/utils/url_validation.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/.gitignore
+-rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/LICENSE
+-rw-r--r--   0        0        0    11365 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/README.md
+-rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/pyproject.toml
+-rw-r--r--   0        0        0    13236 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc2/PKG-INFO
```

### Comparing `haystack_ai-2.2.0rc1/haystack/__init__.py` & `haystack_ai-2.2.0rc2/haystack/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/lazy_imports.py` & `haystack_ai-2.2.0rc2/haystack/lazy_imports.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/logging.py` & `haystack_ai-2.2.0rc2/haystack/logging.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/audio/whisper_local.py` & `haystack_ai-2.2.0rc2/haystack/components/audio/whisper_local.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/audio/whisper_remote.py` & `haystack_ai-2.2.0rc2/haystack/components/audio/whisper_remote.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/builders/__init__.py` & `haystack_ai-2.2.0rc2/haystack/components/builders/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/builders/answer_builder.py` & `haystack_ai-2.2.0rc2/haystack/components/builders/answer_builder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/builders/chat_prompt_builder.py` & `haystack_ai-2.2.0rc2/haystack/components/builders/chat_prompt_builder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/builders/dynamic_chat_prompt_builder.py` & `haystack_ai-2.2.0rc2/haystack/components/builders/dynamic_chat_prompt_builder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/builders/dynamic_prompt_builder.py` & `haystack_ai-2.2.0rc2/haystack/components/builders/dynamic_prompt_builder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/builders/prompt_builder.py` & `haystack_ai-2.2.0rc2/haystack/components/builders/prompt_builder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/caching/cache_checker.py` & `haystack_ai-2.2.0rc2/haystack/components/caching/cache_checker.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/classifiers/document_language_classifier.py` & `haystack_ai-2.2.0rc2/haystack/components/classifiers/document_language_classifier.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/connectors/openapi_service.py` & `haystack_ai-2.2.0rc2/haystack/components/connectors/openapi_service.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/converters/__init__.py` & `haystack_ai-2.2.0rc2/haystack/components/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/converters/azure.py` & `haystack_ai-2.2.0rc2/haystack/components/converters/azure.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/converters/html.py` & `haystack_ai-2.2.0rc2/haystack/components/converters/html.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/converters/markdown.py` & `haystack_ai-2.2.0rc2/haystack/components/converters/markdown.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/converters/openapi_functions.py` & `haystack_ai-2.2.0rc2/haystack/components/converters/openapi_functions.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/converters/output_adapter.py` & `haystack_ai-2.2.0rc2/haystack/components/converters/output_adapter.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/converters/pdfminer.py` & `haystack_ai-2.2.0rc2/haystack/components/converters/pdfminer.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/converters/pypdf.py` & `haystack_ai-2.2.0rc2/haystack/components/converters/pypdf.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/converters/tika.py` & `haystack_ai-2.2.0rc2/haystack/components/converters/tika.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/converters/txt.py` & `haystack_ai-2.2.0rc2/haystack/components/converters/txt.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/converters/utils.py` & `haystack_ai-2.2.0rc2/haystack/components/converters/utils.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/embedders/__init__.py` & `haystack_ai-2.2.0rc2/haystack/components/embedders/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/embedders/azure_document_embedder.py` & `haystack_ai-2.2.0rc2/haystack/components/embedders/azure_document_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/embedders/azure_text_embedder.py` & `haystack_ai-2.2.0rc2/haystack/components/embedders/azure_text_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/embedders/hugging_face_api_document_embedder.py` & `haystack_ai-2.2.0rc2/haystack/components/embedders/hugging_face_api_document_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/embedders/hugging_face_api_text_embedder.py` & `haystack_ai-2.2.0rc2/haystack/components/embedders/hugging_face_api_text_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/embedders/hugging_face_tei_document_embedder.py` & `haystack_ai-2.2.0rc2/haystack/components/embedders/hugging_face_tei_document_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/embedders/hugging_face_tei_text_embedder.py` & `haystack_ai-2.2.0rc2/haystack/components/embedders/hugging_face_tei_text_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/embedders/openai_document_embedder.py` & `haystack_ai-2.2.0rc2/haystack/components/embedders/openai_document_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/embedders/openai_text_embedder.py` & `haystack_ai-2.2.0rc2/haystack/components/embedders/openai_text_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/embedders/sentence_transformers_document_embedder.py` & `haystack_ai-2.2.0rc2/haystack/components/embedders/sentence_transformers_document_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/embedders/sentence_transformers_text_embedder.py` & `haystack_ai-2.2.0rc2/haystack/components/embedders/sentence_transformers_text_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/embedders/backends/sentence_transformers_backend.py` & `haystack_ai-2.2.0rc2/haystack/components/embedders/backends/sentence_transformers_backend.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/evaluators/__init__.py` & `haystack_ai-2.2.0rc2/haystack/components/evaluators/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/evaluators/answer_exact_match.py` & `haystack_ai-2.2.0rc2/haystack/components/evaluators/answer_exact_match.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/evaluators/context_relevance.py` & `haystack_ai-2.2.0rc2/haystack/components/evaluators/context_relevance.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/evaluators/document_map.py` & `haystack_ai-2.2.0rc2/haystack/components/evaluators/document_map.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/evaluators/document_mrr.py` & `haystack_ai-2.2.0rc2/haystack/components/evaluators/document_mrr.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/evaluators/document_recall.py` & `haystack_ai-2.2.0rc2/haystack/components/evaluators/document_recall.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/evaluators/faithfulness.py` & `haystack_ai-2.2.0rc2/haystack/components/evaluators/faithfulness.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/evaluators/llm_evaluator.py` & `haystack_ai-2.2.0rc2/haystack/components/evaluators/llm_evaluator.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/evaluators/sas_evaluator.py` & `haystack_ai-2.2.0rc2/haystack/components/evaluators/sas_evaluator.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/extractors/named_entity_extractor.py` & `haystack_ai-2.2.0rc2/haystack/components/extractors/named_entity_extractor.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/fetchers/link_content.py` & `haystack_ai-2.2.0rc2/haystack/components/fetchers/link_content.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/generators/__init__.py` & `haystack_ai-2.2.0rc2/haystack/components/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/generators/azure.py` & `haystack_ai-2.2.0rc2/haystack/components/generators/azure.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/generators/hugging_face_api.py` & `haystack_ai-2.2.0rc2/haystack/components/generators/hugging_face_api.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/generators/hugging_face_local.py` & `haystack_ai-2.2.0rc2/haystack/components/generators/hugging_face_local.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/generators/hugging_face_tgi.py` & `haystack_ai-2.2.0rc2/haystack/components/generators/hugging_face_tgi.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/generators/openai.py` & `haystack_ai-2.2.0rc2/haystack/components/generators/openai.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/generators/utils.py` & `haystack_ai-2.2.0rc2/haystack/components/generators/utils.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/generators/chat/__init__.py` & `haystack_ai-2.2.0rc2/haystack/components/generators/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/generators/chat/azure.py` & `haystack_ai-2.2.0rc2/haystack/components/generators/chat/azure.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/generators/chat/hugging_face_api.py` & `haystack_ai-2.2.0rc2/haystack/components/generators/chat/hugging_face_api.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/generators/chat/hugging_face_local.py` & `haystack_ai-2.2.0rc2/haystack/components/generators/chat/hugging_face_local.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/generators/chat/hugging_face_tgi.py` & `haystack_ai-2.2.0rc2/haystack/components/generators/chat/hugging_face_tgi.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/generators/chat/openai.py` & `haystack_ai-2.2.0rc2/haystack/components/generators/chat/openai.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/joiners/branch.py` & `haystack_ai-2.2.0rc2/haystack/components/joiners/branch.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/joiners/document_joiner.py` & `haystack_ai-2.2.0rc2/haystack/components/joiners/document_joiner.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/others/multiplexer.py` & `haystack_ai-2.2.0rc2/haystack/components/others/multiplexer.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/preprocessors/document_cleaner.py` & `haystack_ai-2.2.0rc2/haystack/components/preprocessors/document_cleaner.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/preprocessors/document_splitter.py` & `haystack_ai-2.2.0rc2/haystack/components/preprocessors/document_splitter.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/preprocessors/text_cleaner.py` & `haystack_ai-2.2.0rc2/haystack/components/preprocessors/text_cleaner.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/rankers/__init__.py` & `haystack_ai-2.2.0rc2/haystack/components/rankers/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/rankers/lost_in_the_middle.py` & `haystack_ai-2.2.0rc2/haystack/components/rankers/lost_in_the_middle.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/rankers/meta_field.py` & `haystack_ai-2.2.0rc2/haystack/components/rankers/meta_field.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/rankers/sentence_transformers_diversity.py` & `haystack_ai-2.2.0rc2/haystack/components/rankers/sentence_transformers_diversity.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/rankers/transformers_similarity.py` & `haystack_ai-2.2.0rc2/haystack/components/rankers/transformers_similarity.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/readers/extractive.py` & `haystack_ai-2.2.0rc2/haystack/components/readers/extractive.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/retrievers/filter_retriever.py` & `haystack_ai-2.2.0rc2/haystack/components/retrievers/filter_retriever.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/retrievers/in_memory/bm25_retriever.py` & `haystack_ai-2.2.0rc2/haystack/components/retrievers/in_memory/bm25_retriever.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/retrievers/in_memory/embedding_retriever.py` & `haystack_ai-2.2.0rc2/haystack/components/retrievers/in_memory/embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/routers/__init__.py` & `haystack_ai-2.2.0rc2/haystack/components/routers/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/routers/conditional_router.py` & `haystack_ai-2.2.0rc2/haystack/components/routers/conditional_router.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/routers/file_type_router.py` & `haystack_ai-2.2.0rc2/haystack/components/routers/file_type_router.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/routers/metadata_router.py` & `haystack_ai-2.2.0rc2/haystack/components/routers/metadata_router.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/routers/text_language_router.py` & `haystack_ai-2.2.0rc2/haystack/components/routers/text_language_router.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/routers/zero_shot_text_router.py` & `haystack_ai-2.2.0rc2/haystack/components/routers/zero_shot_text_router.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/samplers/top_p.py` & `haystack_ai-2.2.0rc2/haystack/components/samplers/top_p.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/validators/json_schema.py` & `haystack_ai-2.2.0rc2/haystack/components/validators/json_schema.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/websearch/searchapi.py` & `haystack_ai-2.2.0rc2/haystack/components/websearch/searchapi.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/websearch/serper_dev.py` & `haystack_ai-2.2.0rc2/haystack/components/websearch/serper_dev.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/components/writers/document_writer.py` & `haystack_ai-2.2.0rc2/haystack/components/writers/document_writer.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/core/errors.py` & `haystack_ai-2.2.0rc2/haystack/core/errors.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/core/serialization.py` & `haystack_ai-2.2.0rc2/haystack/core/serialization.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/core/type_utils.py` & `haystack_ai-2.2.0rc2/haystack/core/type_utils.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/core/component/component.py` & `haystack_ai-2.2.0rc2/haystack/core/component/component.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/core/component/sockets.py` & `haystack_ai-2.2.0rc2/haystack/core/component/sockets.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/core/component/types.py` & `haystack_ai-2.2.0rc2/haystack/core/component/types.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/core/pipeline/base.py` & `haystack_ai-2.2.0rc2/haystack/core/pipeline/base.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/core/pipeline/descriptions.py` & `haystack_ai-2.2.0rc2/haystack/core/pipeline/descriptions.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/core/pipeline/draw.py` & `haystack_ai-2.2.0rc2/haystack/core/pipeline/draw.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/core/pipeline/pipeline.py` & `haystack_ai-2.2.0rc2/haystack/core/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/core/pipeline/template.py` & `haystack_ai-2.2.0rc2/haystack/core/pipeline/template.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/core/pipeline/utils.py` & `haystack_ai-2.2.0rc2/haystack/core/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/core/pipeline/predefined/chat_with_website.yaml.jinja2` & `haystack_ai-2.2.0rc2/haystack/core/pipeline/predefined/chat_with_website.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/core/pipeline/predefined/generative_qa.yaml.jinja2` & `haystack_ai-2.2.0rc2/haystack/core/pipeline/predefined/generative_qa.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/core/pipeline/predefined/indexing.yaml.jinja2` & `haystack_ai-2.2.0rc2/haystack/core/pipeline/predefined/indexing.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/core/pipeline/predefined/rag.yaml.jinja2` & `haystack_ai-2.2.0rc2/haystack/core/pipeline/predefined/rag.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/dataclasses/__init__.py` & `haystack_ai-2.2.0rc2/haystack/dataclasses/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/dataclasses/answer.py` & `haystack_ai-2.2.0rc2/haystack/dataclasses/answer.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/dataclasses/byte_stream.py` & `haystack_ai-2.2.0rc2/haystack/dataclasses/byte_stream.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/dataclasses/chat_message.py` & `haystack_ai-2.2.0rc2/haystack/dataclasses/chat_message.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/dataclasses/document.py` & `haystack_ai-2.2.0rc2/haystack/dataclasses/document.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/dataclasses/sparse_embedding.py` & `haystack_ai-2.2.0rc2/haystack/dataclasses/sparse_embedding.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/dataclasses/streaming_chunk.py` & `haystack_ai-2.2.0rc2/haystack/dataclasses/streaming_chunk.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/document_stores/in_memory/document_store.py` & `haystack_ai-2.2.0rc2/haystack/document_stores/in_memory/document_store.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/document_stores/types/protocol.py` & `haystack_ai-2.2.0rc2/haystack/document_stores/types/protocol.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/evaluation/eval_run_result.py` & `haystack_ai-2.2.0rc2/haystack/evaluation/eval_run_result.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/marshal/protocol.py` & `haystack_ai-2.2.0rc2/haystack/marshal/protocol.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/marshal/yaml.py` & `haystack_ai-2.2.0rc2/haystack/marshal/yaml.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/telemetry/_environment.py` & `haystack_ai-2.2.0rc2/haystack/telemetry/_environment.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/telemetry/_telemetry.py` & `haystack_ai-2.2.0rc2/haystack/telemetry/_telemetry.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/testing/document_store.py` & `haystack_ai-2.2.0rc2/haystack/testing/document_store.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/testing/factory.py` & `haystack_ai-2.2.0rc2/haystack/testing/factory.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/testing/test_utils.py` & `haystack_ai-2.2.0rc2/haystack/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/testing/sample_components/__init__.py` & `haystack_ai-2.2.0rc2/haystack/testing/sample_components/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/testing/sample_components/accumulate.py` & `haystack_ai-2.2.0rc2/haystack/testing/sample_components/accumulate.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/testing/sample_components/add_value.py` & `haystack_ai-2.2.0rc2/haystack/testing/sample_components/add_value.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/testing/sample_components/concatenate.py` & `haystack_ai-2.2.0rc2/haystack/testing/sample_components/concatenate.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/testing/sample_components/fstring.py` & `haystack_ai-2.2.0rc2/haystack/testing/sample_components/fstring.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/testing/sample_components/greet.py` & `haystack_ai-2.2.0rc2/haystack/testing/sample_components/greet.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/testing/sample_components/joiner.py` & `haystack_ai-2.2.0rc2/haystack/testing/sample_components/joiner.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/testing/sample_components/parity.py` & `haystack_ai-2.2.0rc2/haystack/testing/sample_components/parity.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/testing/sample_components/remainder.py` & `haystack_ai-2.2.0rc2/haystack/testing/sample_components/remainder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/testing/sample_components/self_loop.py` & `haystack_ai-2.2.0rc2/haystack/testing/sample_components/self_loop.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/testing/sample_components/subtract.py` & `haystack_ai-2.2.0rc2/haystack/testing/sample_components/subtract.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/testing/sample_components/threshold.py` & `haystack_ai-2.2.0rc2/haystack/testing/sample_components/threshold.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/tracing/datadog.py` & `haystack_ai-2.2.0rc2/haystack/tracing/datadog.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/tracing/opentelemetry.py` & `haystack_ai-2.2.0rc2/haystack/tracing/opentelemetry.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/tracing/tracer.py` & `haystack_ai-2.2.0rc2/haystack/tracing/tracer.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/tracing/utils.py` & `haystack_ai-2.2.0rc2/haystack/tracing/utils.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/utils/__init__.py` & `haystack_ai-2.2.0rc2/haystack/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/utils/auth.py` & `haystack_ai-2.2.0rc2/haystack/utils/auth.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/utils/callable_serialization.py` & `haystack_ai-2.2.0rc2/haystack/utils/callable_serialization.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/utils/device.py` & `haystack_ai-2.2.0rc2/haystack/utils/device.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/utils/filters.py` & `haystack_ai-2.2.0rc2/haystack/utils/filters.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/utils/hf.py` & `haystack_ai-2.2.0rc2/haystack/utils/hf.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/utils/jupyter.py` & `haystack_ai-2.2.0rc2/haystack/utils/jupyter.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/utils/requests_utils.py` & `haystack_ai-2.2.0rc2/haystack/utils/requests_utils.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/haystack/utils/type_serialization.py` & `haystack_ai-2.2.0rc2/haystack/utils/type_serialization.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/.gitignore` & `haystack_ai-2.2.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/LICENSE` & `haystack_ai-2.2.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/README.md` & `haystack_ai-2.2.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/pyproject.toml` & `haystack_ai-2.2.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.2.0rc1/PKG-INFO` & `haystack_ai-2.2.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: haystack-ai
-Version: 2.2.0rc1
+Version: 2.2.0rc2
 Summary: LLM framework to build customizable, production-ready LLM applications. Connect components (models, vector DBs, file converters) to pipelines or agents that can interact with your data.
 Project-URL: CI: GitHub, https://github.com/deepset-ai/haystack/actions
 Project-URL: Docs: RTD, https://haystack.deepset.ai/overview/intro
 Project-URL: GitHub: issues, https://github.com/deepset-ai/haystack/issues
 Project-URL: GitHub: repo, https://github.com/deepset-ai/haystack
 Project-URL: Homepage, https://github.com/deepset-ai/haystack
 Author-email: "deepset.ai" <malte.pietsch@deepset.ai>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: haystack-ai Version: 2.2.0rc1 Summary: LLM
+Metadata-Version: 2.3 Name: haystack-ai Version: 2.2.0rc2 Summary: LLM
 framework to build customizable, production-ready LLM applications. Connect
 components (models, vector DBs, file converters) to pipelines or agents that
 can interact with your data. Project-URL: CI: GitHub, https://github.com/
 deepset-ai/haystack/actions Project-URL: Docs: RTD, https://
 haystack.deepset.ai/overview/intro Project-URL: GitHub: issues, https://
 github.com/deepset-ai/haystack/issues Project-URL: GitHub: repo, https://
 github.com/deepset-ai/haystack Project-URL: Homepage, https://github.com/
```

