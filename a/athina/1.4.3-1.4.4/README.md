# Comparing `tmp/athina-1.4.3.tar.gz` & `tmp/athina-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athina-1.4.3.tar", max compression
+gzip compressed data, was "athina-1.4.4.tar", max compression
```

## Comparing `athina-1.4.3.tar` & `athina-1.4.4.tar`

### file list

```diff
@@ -1,155 +1,156 @@
--rw-r--r--   0        0        0     8595 2024-05-03 15:41:49.406642 athina-1.4.3/README.md
--rw-r--r--   0        0        0      169 2024-05-03 15:41:49.406999 athina-1.4.3/athina/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.176900 athina-1.4.3/athina/cli/__init__.py
--rw-r--r--   0        0        0     5390 2024-05-05 12:00:16.321612 athina-1.4.3/athina/cli/cli.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.177123 athina-1.4.3/athina/constants/__init__.py
--rw-r--r--   0        0        0      517 2024-03-19 22:27:57.177236 athina-1.4.3/athina/constants/messages.py
--rw-r--r--   0        0        0       72 2024-05-03 15:41:49.407935 athina-1.4.3/athina/datasets/__init__.py
--rw-r--r--   0        0        0   218970 2024-05-03 15:41:49.408467 athina-1.4.3/athina/datasets/conversations.json
--rw-r--r--   0        0        0     3315 2024-05-29 20:37:43.202700 athina-1.4.3/athina/datasets/dataset.py
--rw-r--r--   0        0        0     3355 2024-03-19 22:27:57.177821 athina-1.4.3/athina/datasets/summarization_sample.py
--rw-r--r--   0        0        0     2675 2024-05-03 15:41:49.409340 athina-1.4.3/athina/datasets/yc_query_mini.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.177993 athina-1.4.3/athina/errors/__init__.py
--rw-r--r--   0        0        0      801 2024-03-19 22:27:57.178079 athina-1.4.3/athina/errors/exceptions.py
--rw-r--r--   0        0        0     5016 2024-05-29 18:23:51.695514 athina-1.4.3/athina/evals/__init__.py
--rw-r--r--   0        0        0     8354 2024-05-16 19:27:48.886844 athina-1.4.3/athina/evals/base_evaluator.py
--rw-r--r--   0        0        0     4259 2024-05-16 19:27:48.887245 athina-1.4.3/athina/evals/conversation/conversation_coherence/evaluator.py
--rw-r--r--   0        0        0     1198 2024-05-03 15:41:49.410542 athina-1.4.3/athina/evals/conversation/conversation_coherence/prompt.py
--rw-r--r--   0        0        0     4414 2024-05-16 19:27:48.887449 athina-1.4.3/athina/evals/conversation/conversation_resolution/evaluator.py
--rw-r--r--   0        0        0     1104 2024-05-03 15:41:49.410767 athina-1.4.3/athina/evals/conversation/conversation_resolution/prompt.py
--rw-r--r--   0        0        0     2984 2024-05-29 18:23:51.695664 athina-1.4.3/athina/evals/eval_type.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.179006 athina-1.4.3/athina/evals/function/__init__.py
--rw-r--r--   0        0        0     3780 2024-05-16 19:27:48.888106 athina-1.4.3/athina/evals/function/function_evaluator.py
--rw-r--r--   0        0        0    20171 2024-05-29 18:23:51.696561 athina-1.4.3/athina/evals/function/functions.py
--rw-r--r--   0        0        0    11066 2024-05-29 18:23:51.697020 athina-1.4.3/athina/evals/function/wrapper.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.179629 athina-1.4.3/athina/evals/grounded/__init__.py
--rw-r--r--   0        0        0     4298 2024-05-16 19:27:48.888364 athina-1.4.3/athina/evals/grounded/grounded_evaluator.py
--rw-r--r--   0        0        0     4178 2024-03-19 22:27:57.179870 athina-1.4.3/athina/evals/grounded/similarity.py
--rw-r--r--   0        0        0     1708 2024-03-19 22:27:57.179950 athina-1.4.3/athina/evals/grounded/wrapper.py
--rw-r--r--   0        0        0     3369 2024-06-01 12:17:30.040063 athina-1.4.3/athina/evals/guardrails/correct_language/evaluator.py
--rw-r--r--   0        0        0     2820 2024-06-01 12:17:30.040433 athina-1.4.3/athina/evals/guardrails/detect_pii/evaluator.py
--rw-r--r--   0        0        0     3048 2024-06-01 12:17:30.041633 athina-1.4.3/athina/evals/guardrails/gibberish_text/evaluator.py
--rw-r--r--   0        0        0     2701 2024-06-01 12:17:30.042051 athina-1.4.3/athina/evals/guardrails/no_secrets_present/evaluator.py
--rw-r--r--   0        0        0     3141 2024-06-01 12:17:30.042309 athina-1.4.3/athina/evals/guardrails/politeness_check/evaluator.py
--rw-r--r--   0        0        0     2656 2024-06-01 12:17:30.042455 athina-1.4.3/athina/evals/guardrails/profanity_free/evaluator.py
--rw-r--r--   0        0        0     2833 2024-06-01 12:17:30.042729 athina-1.4.3/athina/evals/guardrails/reading_time/evaluator.py
--rw-r--r--   0        0        0     3779 2024-06-01 12:17:30.042875 athina-1.4.3/athina/evals/guardrails/restrict_to_topic/evaluator.py
--rw-r--r--   0        0        0     3804 2024-06-01 12:17:30.043033 athina-1.4.3/athina/evals/guardrails/sensitive_topics/evaluator.py
--rw-r--r--   0        0        0     2972 2024-06-01 12:17:30.043310 athina-1.4.3/athina/evals/guardrails/sfw/evaluator.py
--rw-r--r--   0        0        0     2857 2024-06-01 12:17:30.043604 athina-1.4.3/athina/evals/guardrails/toxic_language/evaluator.py
--rw-r--r--   0        0        0     3180 2024-06-01 12:17:30.043965 athina-1.4.3/athina/evals/guardrails/unusual_prompt/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180226 athina-1.4.3/athina/evals/llm/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180328 athina-1.4.3/athina/evals/llm/context_contains_enough_information/__init__.py
--rw-r--r--   0        0        0     3004 2024-05-16 19:27:48.889580 athina-1.4.3/athina/evals/llm/context_contains_enough_information/evaluator.py
--rw-r--r--   0        0        0     1867 2024-03-19 22:27:57.180505 athina-1.4.3/athina/evals/llm/context_contains_enough_information/examples.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180583 athina-1.4.3/athina/evals/llm/custom_prompt/__init__.py
--rw-r--r--   0        0        0     2857 2024-05-29 18:23:47.847799 athina-1.4.3/athina/evals/llm/custom_prompt/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180792 athina-1.4.3/athina/evals/llm/does_response_answer_query/__init__.py
--rw-r--r--   0        0        0     2632 2024-05-03 15:41:49.417364 athina-1.4.3/athina/evals/llm/does_response_answer_query/evaluator.py
--rw-r--r--   0        0        0     1186 2024-03-19 22:27:57.180970 athina-1.4.3/athina/evals/llm/does_response_answer_query/examples.py
--rw-r--r--   0        0        0     1238 2024-03-19 22:27:57.181044 athina-1.4.3/athina/evals/llm/example.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.181120 athina-1.4.3/athina/evals/llm/faithfulness/__init__.py
--rw-r--r--   0        0        0     2599 2024-05-03 15:41:49.417490 athina-1.4.3/athina/evals/llm/faithfulness/evaluator.py
--rw-r--r--   0        0        0     1335 2024-03-19 22:27:57.181288 athina-1.4.3/athina/evals/llm/faithfulness/examples.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.181361 athina-1.4.3/athina/evals/llm/grading_criteria/__init__.py
--rw-r--r--   0        0        0     2209 2024-05-16 19:27:48.889913 athina-1.4.3/athina/evals/llm/grading_criteria/evaluator.py
--rw-r--r--   0        0        0     5821 2024-05-03 15:41:49.418273 athina-1.4.3/athina/evals/llm/groundedness/evaluator.py
--rw-r--r--   0        0        0     1601 2024-03-19 22:27:57.181666 athina-1.4.3/athina/evals/llm/groundedness/prompt.py
--rw-r--r--   0        0        0     4982 2024-05-05 09:24:29.466550 athina-1.4.3/athina/evals/llm/llm_evaluator.py
--rw-r--r--   0        0        0    10915 2024-05-03 15:41:49.418745 athina-1.4.3/athina/evals/llm/summary_accuracy/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182165 athina-1.4.3/athina/evals/ragas/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182276 athina-1.4.3/athina/evals/ragas/answer_correctness/__init__.py
--rw-r--r--   0        0        0     2383 2024-05-03 15:41:49.419035 athina-1.4.3/athina/evals/ragas/answer_correctness/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182502 athina-1.4.3/athina/evals/ragas/answer_relevancy/__init__.py
--rw-r--r--   0        0        0     2441 2024-05-03 15:41:49.419202 athina-1.4.3/athina/evals/ragas/answer_relevancy/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182699 athina-1.4.3/athina/evals/ragas/answer_semantic_similarity/__init__.py
--rw-r--r--   0        0        0     2440 2024-05-03 15:41:49.419340 athina-1.4.3/athina/evals/ragas/answer_semantic_similarity/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182961 athina-1.4.3/athina/evals/ragas/coherence/__init__.py
--rw-r--r--   0        0        0     2187 2024-05-03 15:41:49.419789 athina-1.4.3/athina/evals/ragas/coherence/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183170 athina-1.4.3/athina/evals/ragas/conciseness/__init__.py
--rw-r--r--   0        0        0     2223 2024-05-03 15:41:49.420084 athina-1.4.3/athina/evals/ragas/conciseness/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183377 athina-1.4.3/athina/evals/ragas/context_precision/__init__.py
--rw-r--r--   0        0        0     2521 2024-05-03 15:41:49.420494 athina-1.4.3/athina/evals/ragas/context_precision/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183558 athina-1.4.3/athina/evals/ragas/context_recall/__init__.py
--rw-r--r--   0        0        0     2316 2024-05-03 15:41:49.420634 athina-1.4.3/athina/evals/ragas/context_recall/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183719 athina-1.4.3/athina/evals/ragas/context_relevancy/__init__.py
--rw-r--r--   0        0        0     2159 2024-05-03 15:41:49.420776 athina-1.4.3/athina/evals/ragas/context_relevancy/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183882 athina-1.4.3/athina/evals/ragas/faithfulness/__init__.py
--rw-r--r--   0        0        0     2370 2024-05-03 15:41:49.420918 athina-1.4.3/athina/evals/ragas/faithfulness/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.184050 athina-1.4.3/athina/evals/ragas/harmfulness/__init__.py
--rw-r--r--   0        0        0     2164 2024-05-03 15:41:49.421222 athina-1.4.3/athina/evals/ragas/harmfulness/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.184253 athina-1.4.3/athina/evals/ragas/maliciousness/__init__.py
--rw-r--r--   0        0        0     2127 2024-05-03 15:41:49.421640 athina-1.4.3/athina/evals/ragas/maliciousness/evaluator.py
--rw-r--r--   0        0        0     3298 2024-05-03 15:41:49.421803 athina-1.4.3/athina/evals/ragas/ragas_evaluator.py
--rw-r--r--   0        0        0     5154 2024-05-03 15:41:49.422152 athina-1.4.3/athina/evals/safety/content_moderation/evaluator.py
--rw-r--r--   0        0        0     3387 2024-05-03 15:41:49.422800 athina-1.4.3/athina/evals/safety/pii_detection/evaluator.py
--rw-r--r--   0        0        0     4370 2024-05-03 15:41:49.424028 athina-1.4.3/athina/evals/safety/prompt_injection/evaluator.py
--rw-r--r--   0        0        0      106 2024-05-03 15:41:49.424321 athina-1.4.3/athina/guard/exception.py
--rw-r--r--   0        0        0     1404 2024-05-03 15:41:49.424686 athina-1.4.3/athina/guard/guard.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.184508 athina-1.4.3/athina/helpers/__init__.py
--rw-r--r--   0        0        0     5739 2024-05-16 19:27:48.890218 athina-1.4.3/athina/helpers/athina_logging_helper.py
--rw-r--r--   0        0        0     1351 2024-03-19 22:27:57.184662 athina-1.4.3/athina/helpers/config.py
--rw-r--r--   0        0        0      122 2024-05-29 19:56:29.342493 athina-1.4.3/athina/helpers/constants.py
--rw-r--r--   0        0        0      790 2024-05-16 19:27:48.890420 athina-1.4.3/athina/helpers/dataset_helper.py
--rw-r--r--   0        0        0      172 2024-03-19 22:27:57.184807 athina-1.4.3/athina/helpers/eval_helper.py
--rw-r--r--   0        0        0      642 2024-03-19 22:27:57.184880 athina-1.4.3/athina/helpers/function_eval_util.py
--rw-r--r--   0        0        0     5152 2024-05-29 18:23:51.699858 athina-1.4.3/athina/helpers/get_evaluator.py
--rw-r--r--   0        0        0      135 2024-05-25 05:42:57.983530 athina-1.4.3/athina/helpers/jinja_helper.py
--rw-r--r--   0        0        0     2469 2024-05-22 07:52:50.227484 athina-1.4.3/athina/helpers/json.py
--rw-r--r--   0        0        0      403 2024-03-19 22:27:57.185114 athina-1.4.3/athina/helpers/kwparser.py
--rw-r--r--   0        0        0      894 2024-05-03 15:41:49.425348 athina-1.4.3/athina/helpers/loader_helper.py
--rw-r--r--   0        0        0     3051 2024-03-19 22:27:57.185252 athina-1.4.3/athina/helpers/logger.py
--rw-r--r--   0        0        0      265 2024-03-19 22:27:57.185337 athina-1.4.3/athina/helpers/package_helper.py
--rw-r--r--   0        0        0     5296 2024-03-19 22:27:57.185429 athina-1.4.3/athina/helpers/run_helper.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.185498 athina-1.4.3/athina/interfaces/__init__.py
--rw-r--r--   0        0        0     3905 2024-05-03 15:41:49.425463 athina-1.4.3/athina/interfaces/athina.py
--rw-r--r--   0        0        0      132 2024-03-19 22:27:57.185654 athina-1.4.3/athina/interfaces/data.py
--rw-r--r--   0        0        0     2065 2024-05-14 15:59:10.451321 athina-1.4.3/athina/interfaces/model.py
--rw-r--r--   0        0        0      100 2024-03-19 22:27:57.185783 athina-1.4.3/athina/interfaces/openai.py
--rw-r--r--   0        0        0     2944 2024-05-05 12:12:32.954417 athina-1.4.3/athina/interfaces/result.py
--rw-r--r--   0        0        0      126 2024-03-19 22:27:57.185951 athina-1.4.3/athina/keys/__init__.py
--rw-r--r--   0        0        0      322 2024-03-19 22:27:57.186019 athina-1.4.3/athina/keys/athina_api_key.py
--rw-r--r--   0        0        0      236 2024-03-19 22:27:57.186085 athina-1.4.3/athina/keys/openai_api_key.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.186149 athina-1.4.3/athina/llms/__init__.py
--rw-r--r--   0        0        0     1368 2024-05-22 07:52:50.227988 athina-1.4.3/athina/llms/abstract_llm_service.py
--rw-r--r--   0        0        0     1524 2024-05-22 07:52:50.228405 athina-1.4.3/athina/llms/litellm_service.py
--rw-r--r--   0        0        0     3461 2024-05-29 18:23:47.848584 athina-1.4.3/athina/llms/openai_service.py
--rw-r--r--   0        0        0      337 2024-03-19 22:27:57.186378 athina-1.4.3/athina/llms/question_answerer.py
--rw-r--r--   0        0        0     2874 2024-05-21 13:33:12.522927 athina-1.4.3/athina/llms/question_answerer_bulk.py
--rw-r--r--   0        0        0     3675 2024-03-19 22:27:57.186521 athina-1.4.3/athina/llms/question_answerer_cot.py
--rw-r--r--   0        0        0     6674 2024-05-03 15:41:49.426272 athina-1.4.3/athina/llms/question_answerer_with_retrieval.py
--rw-r--r--   0        0        0     2402 2024-03-19 22:27:57.186684 athina-1.4.3/athina/llms/question_generator.py
--rw-r--r--   0        0        0      323 2024-05-03 15:41:49.426530 athina-1.4.3/athina/loaders/__init__.py
--rw-r--r--   0        0        0     2326 2024-05-16 23:56:49.987467 athina-1.4.3/athina/loaders/base_loader.py
--rw-r--r--   0        0        0     2179 2024-05-16 19:27:48.890989 athina-1.4.3/athina/loaders/conversation_loader.py
--rw-r--r--   0        0        0     6507 2024-05-17 01:08:19.006440 athina-1.4.3/athina/loaders/loader.py
--rw-r--r--   0        0        0     3597 2024-05-16 19:27:48.892946 athina-1.4.3/athina/loaders/response_loader.py
--rw-r--r--   0        0        0     2970 2024-05-03 17:07:59.624449 athina-1.4.3/athina/loaders/summary_loader.py
--rw-r--r--   0        0        0     2380 2024-05-03 15:41:49.427400 athina-1.4.3/athina/loaders/text_loader.py
--rw-r--r--   0        0        0     1854 2024-03-19 22:27:57.187257 athina-1.4.3/athina/metrics/agreement_score.py
--rw-r--r--   0        0        0     2448 2024-03-19 22:27:57.187346 athina-1.4.3/athina/metrics/contradiction_score.py
--rw-r--r--   0        0        0     1342 2024-03-19 22:27:57.187416 athina-1.4.3/athina/metrics/groundedness.py
--rw-r--r--   0        0        0     2209 2024-03-19 22:27:57.187494 athina-1.4.3/athina/metrics/hallucination_score.py
--rw-r--r--   0        0        0      246 2024-03-19 22:27:57.187555 athina-1.4.3/athina/metrics/metric.py
--rw-r--r--   0        0        0     3000 2024-05-03 15:41:49.427514 athina-1.4.3/athina/metrics/metric_type.py
--rw-r--r--   0        0        0      393 2024-03-19 22:27:57.187682 athina-1.4.3/athina/metrics/passed.py
--rw-r--r--   0        0        0      275 2024-03-19 22:27:57.187758 athina-1.4.3/athina/metrics/ragas_metric.py
--rw-r--r--   0        0        0      509 2024-03-19 22:27:57.187846 athina-1.4.3/athina/metrics/similarity_score.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.187933 athina-1.4.3/athina/runner/__init__.py
--rw-r--r--   0        0        0     7034 2024-05-30 05:39:04.348672 athina-1.4.3/athina/runner/run.py
--rw-r--r--   0        0        0      418 2024-05-30 05:39:04.349357 athina-1.4.3/athina/runner/run_wrapper.py
--rw-r--r--   0        0        0     5729 2024-05-29 18:23:51.700266 athina-1.4.3/athina/scripts/guardrails.py
--rw-r--r--   0        0        0    13810 2024-05-29 20:37:14.247205 athina-1.4.3/athina/services/athina_api_service.py
--rw-r--r--   0        0        0      472 2024-05-29 18:23:47.849253 athina-1.4.3/athina/steps/__init__.py
--rw-r--r--   0        0        0     2107 2024-05-28 05:27:42.582035 athina-1.4.3/athina/steps/api.py
--rw-r--r--   0        0        0     4456 2024-05-22 07:52:50.229580 athina-1.4.3/athina/steps/base.py
--rw-r--r--   0        0        0     1729 2024-05-22 07:52:50.229864 athina-1.4.3/athina/steps/chain.py
--rw-r--r--   0        0        0     1346 2024-05-27 14:49:53.587855 athina-1.4.3/athina/steps/classify_text.py
--rw-r--r--   0        0        0     1501 2024-05-22 07:52:50.230002 athina-1.4.3/athina/steps/conditional.py
--rw-r--r--   0        0        0        0 2024-05-22 07:52:50.230033 athina-1.4.3/athina/steps/debug.py
--rw-r--r--   0        0        0     1440 2024-05-27 14:49:53.588354 athina-1.4.3/athina/steps/extract_entities.py
--rw-r--r--   0        0        0      646 2024-05-22 07:52:50.230202 athina-1.4.3/athina/steps/iterator.py
--rw-r--r--   0        0        0     4581 2024-06-01 12:17:34.394862 athina-1.4.3/athina/steps/llm.py
--rw-r--r--   0        0        0      787 2024-05-22 07:52:50.230543 athina-1.4.3/athina/steps/transform.py
--rw-r--r--   0        0        0     1090 2024-06-01 12:18:16.572578 athina-1.4.3/pyproject.toml
--rw-r--r--   0        0        0     9904 1970-01-01 00:00:00.000000 athina-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0     8595 2024-05-03 15:41:49.406642 athina-1.4.4/README.md
+-rw-r--r--   0        0        0      169 2024-05-03 15:41:49.406999 athina-1.4.4/athina/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.176900 athina-1.4.4/athina/cli/__init__.py
+-rw-r--r--   0        0        0     5390 2024-05-05 12:00:16.321612 athina-1.4.4/athina/cli/cli.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.177123 athina-1.4.4/athina/constants/__init__.py
+-rw-r--r--   0        0        0      517 2024-03-19 22:27:57.177236 athina-1.4.4/athina/constants/messages.py
+-rw-r--r--   0        0        0       72 2024-05-03 15:41:49.407935 athina-1.4.4/athina/datasets/__init__.py
+-rw-r--r--   0        0        0   218970 2024-05-03 15:41:49.408467 athina-1.4.4/athina/datasets/conversations.json
+-rw-r--r--   0        0        0     3269 2024-06-02 09:05:02.010373 athina-1.4.4/athina/datasets/dataset.py
+-rw-r--r--   0        0        0     3355 2024-03-19 22:27:57.177821 athina-1.4.4/athina/datasets/summarization_sample.py
+-rw-r--r--   0        0        0     2675 2024-05-03 15:41:49.409340 athina-1.4.4/athina/datasets/yc_query_mini.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.177993 athina-1.4.4/athina/errors/__init__.py
+-rw-r--r--   0        0        0      801 2024-03-19 22:27:57.178079 athina-1.4.4/athina/errors/exceptions.py
+-rw-r--r--   0        0        0     5045 2024-06-02 09:05:02.010856 athina-1.4.4/athina/evals/__init__.py
+-rw-r--r--   0        0        0     8354 2024-05-16 19:27:48.886844 athina-1.4.4/athina/evals/base_evaluator.py
+-rw-r--r--   0        0        0     4259 2024-05-16 19:27:48.887245 athina-1.4.4/athina/evals/conversation/conversation_coherence/evaluator.py
+-rw-r--r--   0        0        0     1198 2024-05-03 15:41:49.410542 athina-1.4.4/athina/evals/conversation/conversation_coherence/prompt.py
+-rw-r--r--   0        0        0     4414 2024-05-16 19:27:48.887449 athina-1.4.4/athina/evals/conversation/conversation_resolution/evaluator.py
+-rw-r--r--   0        0        0     1104 2024-05-03 15:41:49.410767 athina-1.4.4/athina/evals/conversation/conversation_resolution/prompt.py
+-rw-r--r--   0        0        0     3011 2024-06-02 09:05:02.011104 athina-1.4.4/athina/evals/eval_type.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.179006 athina-1.4.4/athina/evals/function/__init__.py
+-rw-r--r--   0        0        0     3780 2024-05-16 19:27:48.888106 athina-1.4.4/athina/evals/function/function_evaluator.py
+-rw-r--r--   0        0        0    25401 2024-06-02 09:05:02.011769 athina-1.4.4/athina/evals/function/functions.py
+-rw-r--r--   0        0        0    11535 2024-06-02 09:05:02.012236 athina-1.4.4/athina/evals/function/wrapper.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.179629 athina-1.4.4/athina/evals/grounded/__init__.py
+-rw-r--r--   0        0        0     4298 2024-05-16 19:27:48.888364 athina-1.4.4/athina/evals/grounded/grounded_evaluator.py
+-rw-r--r--   0        0        0     4445 2024-06-02 09:05:02.012524 athina-1.4.4/athina/evals/grounded/similarity.py
+-rw-r--r--   0        0        0     1708 2024-03-19 22:27:57.179950 athina-1.4.4/athina/evals/grounded/wrapper.py
+-rw-r--r--   0        0        0     3369 2024-06-01 12:17:30.040063 athina-1.4.4/athina/evals/guardrails/correct_language/evaluator.py
+-rw-r--r--   0        0        0     2820 2024-06-01 12:17:30.040433 athina-1.4.4/athina/evals/guardrails/detect_pii/evaluator.py
+-rw-r--r--   0        0        0     3048 2024-06-01 12:17:30.041633 athina-1.4.4/athina/evals/guardrails/gibberish_text/evaluator.py
+-rw-r--r--   0        0        0     2701 2024-06-02 09:05:02.012838 athina-1.4.4/athina/evals/guardrails/no_secrets_present/evaluator.py
+-rw-r--r--   0        0        0     3141 2024-06-01 12:17:30.042309 athina-1.4.4/athina/evals/guardrails/politeness_check/evaluator.py
+-rw-r--r--   0        0        0     2656 2024-06-01 12:17:30.042455 athina-1.4.4/athina/evals/guardrails/profanity_free/evaluator.py
+-rw-r--r--   0        0        0     2833 2024-06-01 12:17:30.042729 athina-1.4.4/athina/evals/guardrails/reading_time/evaluator.py
+-rw-r--r--   0        0        0     3779 2024-06-01 12:17:30.042875 athina-1.4.4/athina/evals/guardrails/restrict_to_topic/evaluator.py
+-rw-r--r--   0        0        0     3804 2024-06-01 12:17:30.043033 athina-1.4.4/athina/evals/guardrails/sensitive_topics/evaluator.py
+-rw-r--r--   0        0        0     2972 2024-06-01 12:17:30.043310 athina-1.4.4/athina/evals/guardrails/sfw/evaluator.py
+-rw-r--r--   0        0        0     2857 2024-06-01 12:17:30.043604 athina-1.4.4/athina/evals/guardrails/toxic_language/evaluator.py
+-rw-r--r--   0        0        0     3180 2024-06-01 12:17:30.043965 athina-1.4.4/athina/evals/guardrails/unusual_prompt/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180226 athina-1.4.4/athina/evals/llm/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180328 athina-1.4.4/athina/evals/llm/context_contains_enough_information/__init__.py
+-rw-r--r--   0        0        0     3004 2024-05-16 19:27:48.889580 athina-1.4.4/athina/evals/llm/context_contains_enough_information/evaluator.py
+-rw-r--r--   0        0        0     1867 2024-03-19 22:27:57.180505 athina-1.4.4/athina/evals/llm/context_contains_enough_information/examples.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180583 athina-1.4.4/athina/evals/llm/custom_prompt/__init__.py
+-rw-r--r--   0        0        0     2857 2024-05-29 18:23:47.847799 athina-1.4.4/athina/evals/llm/custom_prompt/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180792 athina-1.4.4/athina/evals/llm/does_response_answer_query/__init__.py
+-rw-r--r--   0        0        0     2632 2024-05-03 15:41:49.417364 athina-1.4.4/athina/evals/llm/does_response_answer_query/evaluator.py
+-rw-r--r--   0        0        0     1186 2024-03-19 22:27:57.180970 athina-1.4.4/athina/evals/llm/does_response_answer_query/examples.py
+-rw-r--r--   0        0        0     1238 2024-03-19 22:27:57.181044 athina-1.4.4/athina/evals/llm/example.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.181120 athina-1.4.4/athina/evals/llm/faithfulness/__init__.py
+-rw-r--r--   0        0        0     2599 2024-05-03 15:41:49.417490 athina-1.4.4/athina/evals/llm/faithfulness/evaluator.py
+-rw-r--r--   0        0        0     1335 2024-03-19 22:27:57.181288 athina-1.4.4/athina/evals/llm/faithfulness/examples.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.181361 athina-1.4.4/athina/evals/llm/grading_criteria/__init__.py
+-rw-r--r--   0        0        0     2209 2024-05-16 19:27:48.889913 athina-1.4.4/athina/evals/llm/grading_criteria/evaluator.py
+-rw-r--r--   0        0        0     5821 2024-05-03 15:41:49.418273 athina-1.4.4/athina/evals/llm/groundedness/evaluator.py
+-rw-r--r--   0        0        0     1601 2024-03-19 22:27:57.181666 athina-1.4.4/athina/evals/llm/groundedness/prompt.py
+-rw-r--r--   0        0        0     4982 2024-05-05 09:24:29.466550 athina-1.4.4/athina/evals/llm/llm_evaluator.py
+-rw-r--r--   0        0        0    10915 2024-05-03 15:41:49.418745 athina-1.4.4/athina/evals/llm/summary_accuracy/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182165 athina-1.4.4/athina/evals/ragas/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182276 athina-1.4.4/athina/evals/ragas/answer_correctness/__init__.py
+-rw-r--r--   0        0        0     2383 2024-05-03 15:41:49.419035 athina-1.4.4/athina/evals/ragas/answer_correctness/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182502 athina-1.4.4/athina/evals/ragas/answer_relevancy/__init__.py
+-rw-r--r--   0        0        0     2441 2024-05-03 15:41:49.419202 athina-1.4.4/athina/evals/ragas/answer_relevancy/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182699 athina-1.4.4/athina/evals/ragas/answer_semantic_similarity/__init__.py
+-rw-r--r--   0        0        0     2440 2024-05-03 15:41:49.419340 athina-1.4.4/athina/evals/ragas/answer_semantic_similarity/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182961 athina-1.4.4/athina/evals/ragas/coherence/__init__.py
+-rw-r--r--   0        0        0     2187 2024-05-03 15:41:49.419789 athina-1.4.4/athina/evals/ragas/coherence/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183170 athina-1.4.4/athina/evals/ragas/conciseness/__init__.py
+-rw-r--r--   0        0        0     2223 2024-05-03 15:41:49.420084 athina-1.4.4/athina/evals/ragas/conciseness/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183377 athina-1.4.4/athina/evals/ragas/context_precision/__init__.py
+-rw-r--r--   0        0        0     2521 2024-05-03 15:41:49.420494 athina-1.4.4/athina/evals/ragas/context_precision/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183558 athina-1.4.4/athina/evals/ragas/context_recall/__init__.py
+-rw-r--r--   0        0        0     2316 2024-05-03 15:41:49.420634 athina-1.4.4/athina/evals/ragas/context_recall/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183719 athina-1.4.4/athina/evals/ragas/context_relevancy/__init__.py
+-rw-r--r--   0        0        0     2159 2024-05-03 15:41:49.420776 athina-1.4.4/athina/evals/ragas/context_relevancy/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183882 athina-1.4.4/athina/evals/ragas/faithfulness/__init__.py
+-rw-r--r--   0        0        0     2370 2024-05-03 15:41:49.420918 athina-1.4.4/athina/evals/ragas/faithfulness/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.184050 athina-1.4.4/athina/evals/ragas/harmfulness/__init__.py
+-rw-r--r--   0        0        0     2164 2024-05-03 15:41:49.421222 athina-1.4.4/athina/evals/ragas/harmfulness/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.184253 athina-1.4.4/athina/evals/ragas/maliciousness/__init__.py
+-rw-r--r--   0        0        0     2127 2024-05-03 15:41:49.421640 athina-1.4.4/athina/evals/ragas/maliciousness/evaluator.py
+-rw-r--r--   0        0        0     3298 2024-05-03 15:41:49.421803 athina-1.4.4/athina/evals/ragas/ragas_evaluator.py
+-rw-r--r--   0        0        0     5154 2024-05-03 15:41:49.422152 athina-1.4.4/athina/evals/safety/content_moderation/evaluator.py
+-rw-r--r--   0        0        0     3387 2024-05-03 15:41:49.422800 athina-1.4.4/athina/evals/safety/pii_detection/evaluator.py
+-rw-r--r--   0        0        0     4370 2024-05-03 15:41:49.424028 athina-1.4.4/athina/evals/safety/prompt_injection/evaluator.py
+-rw-r--r--   0        0        0      106 2024-05-03 15:41:49.424321 athina-1.4.4/athina/guard/exception.py
+-rw-r--r--   0        0        0     1404 2024-05-03 15:41:49.424686 athina-1.4.4/athina/guard/guard.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.184508 athina-1.4.4/athina/helpers/__init__.py
+-rw-r--r--   0        0        0     5739 2024-05-16 19:27:48.890218 athina-1.4.4/athina/helpers/athina_logging_helper.py
+-rw-r--r--   0        0        0     1351 2024-03-19 22:27:57.184662 athina-1.4.4/athina/helpers/config.py
+-rw-r--r--   0        0        0      122 2024-05-29 19:56:29.342493 athina-1.4.4/athina/helpers/constants.py
+-rw-r--r--   0        0        0      790 2024-05-16 19:27:48.890420 athina-1.4.4/athina/helpers/dataset_helper.py
+-rw-r--r--   0        0        0      172 2024-03-19 22:27:57.184807 athina-1.4.4/athina/helpers/eval_helper.py
+-rw-r--r--   0        0        0      642 2024-03-19 22:27:57.184880 athina-1.4.4/athina/helpers/function_eval_util.py
+-rw-r--r--   0        0        0     5187 2024-06-02 09:05:02.013120 athina-1.4.4/athina/helpers/get_evaluator.py
+-rw-r--r--   0        0        0      135 2024-05-25 05:42:57.983530 athina-1.4.4/athina/helpers/jinja_helper.py
+-rw-r--r--   0        0        0     3001 2024-06-02 09:05:02.013693 athina-1.4.4/athina/helpers/json.py
+-rw-r--r--   0        0        0      403 2024-03-19 22:27:57.185114 athina-1.4.4/athina/helpers/kwparser.py
+-rw-r--r--   0        0        0      894 2024-05-03 15:41:49.425348 athina-1.4.4/athina/helpers/loader_helper.py
+-rw-r--r--   0        0        0     3051 2024-03-19 22:27:57.185252 athina-1.4.4/athina/helpers/logger.py
+-rw-r--r--   0        0        0      265 2024-03-19 22:27:57.185337 athina-1.4.4/athina/helpers/package_helper.py
+-rw-r--r--   0        0        0     5296 2024-03-19 22:27:57.185429 athina-1.4.4/athina/helpers/run_helper.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.185498 athina-1.4.4/athina/interfaces/__init__.py
+-rw-r--r--   0        0        0     3894 2024-06-02 09:05:02.013894 athina-1.4.4/athina/interfaces/athina.py
+-rw-r--r--   0        0        0      132 2024-03-19 22:27:57.185654 athina-1.4.4/athina/interfaces/data.py
+-rw-r--r--   0        0        0     2065 2024-05-14 15:59:10.451321 athina-1.4.4/athina/interfaces/model.py
+-rw-r--r--   0        0        0      100 2024-03-19 22:27:57.185783 athina-1.4.4/athina/interfaces/openai.py
+-rw-r--r--   0        0        0     2944 2024-05-05 12:12:32.954417 athina-1.4.4/athina/interfaces/result.py
+-rw-r--r--   0        0        0      126 2024-03-19 22:27:57.185951 athina-1.4.4/athina/keys/__init__.py
+-rw-r--r--   0        0        0      322 2024-03-19 22:27:57.186019 athina-1.4.4/athina/keys/athina_api_key.py
+-rw-r--r--   0        0        0      236 2024-03-19 22:27:57.186085 athina-1.4.4/athina/keys/openai_api_key.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.186149 athina-1.4.4/athina/llms/__init__.py
+-rw-r--r--   0        0        0     1368 2024-05-22 07:52:50.227988 athina-1.4.4/athina/llms/abstract_llm_service.py
+-rw-r--r--   0        0        0     1524 2024-05-22 07:52:50.228405 athina-1.4.4/athina/llms/litellm_service.py
+-rw-r--r--   0        0        0     3461 2024-05-29 18:23:47.848584 athina-1.4.4/athina/llms/openai_service.py
+-rw-r--r--   0        0        0      337 2024-03-19 22:27:57.186378 athina-1.4.4/athina/llms/question_answerer.py
+-rw-r--r--   0        0        0     2874 2024-05-21 13:33:12.522927 athina-1.4.4/athina/llms/question_answerer_bulk.py
+-rw-r--r--   0        0        0     3675 2024-03-19 22:27:57.186521 athina-1.4.4/athina/llms/question_answerer_cot.py
+-rw-r--r--   0        0        0     6674 2024-05-03 15:41:49.426272 athina-1.4.4/athina/llms/question_answerer_with_retrieval.py
+-rw-r--r--   0        0        0     2402 2024-03-19 22:27:57.186684 athina-1.4.4/athina/llms/question_generator.py
+-rw-r--r--   0        0        0      376 2024-06-02 09:05:02.014076 athina-1.4.4/athina/loaders/__init__.py
+-rw-r--r--   0        0        0     2315 2024-06-02 09:05:02.014257 athina-1.4.4/athina/loaders/base_loader.py
+-rw-r--r--   0        0        0     1986 2024-06-02 09:05:02.014530 athina-1.4.4/athina/loaders/conversation_loader.py
+-rw-r--r--   0        0        0     2834 2024-06-02 09:05:02.014749 athina-1.4.4/athina/loaders/json_loader.py
+-rw-r--r--   0        0        0     6507 2024-05-17 01:08:19.006440 athina-1.4.4/athina/loaders/loader.py
+-rw-r--r--   0        0        0     3597 2024-05-16 19:27:48.892946 athina-1.4.4/athina/loaders/response_loader.py
+-rw-r--r--   0        0        0     3065 2024-06-02 09:05:02.015031 athina-1.4.4/athina/loaders/summary_loader.py
+-rw-r--r--   0        0        0     2722 2024-06-02 09:05:02.015205 athina-1.4.4/athina/loaders/text_loader.py
+-rw-r--r--   0        0        0     1854 2024-03-19 22:27:57.187257 athina-1.4.4/athina/metrics/agreement_score.py
+-rw-r--r--   0        0        0     2448 2024-03-19 22:27:57.187346 athina-1.4.4/athina/metrics/contradiction_score.py
+-rw-r--r--   0        0        0     1342 2024-03-19 22:27:57.187416 athina-1.4.4/athina/metrics/groundedness.py
+-rw-r--r--   0        0        0     2209 2024-03-19 22:27:57.187494 athina-1.4.4/athina/metrics/hallucination_score.py
+-rw-r--r--   0        0        0      246 2024-03-19 22:27:57.187555 athina-1.4.4/athina/metrics/metric.py
+-rw-r--r--   0        0        0     3000 2024-05-03 15:41:49.427514 athina-1.4.4/athina/metrics/metric_type.py
+-rw-r--r--   0        0        0      393 2024-03-19 22:27:57.187682 athina-1.4.4/athina/metrics/passed.py
+-rw-r--r--   0        0        0      275 2024-03-19 22:27:57.187758 athina-1.4.4/athina/metrics/ragas_metric.py
+-rw-r--r--   0        0        0      509 2024-03-19 22:27:57.187846 athina-1.4.4/athina/metrics/similarity_score.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.187933 athina-1.4.4/athina/runner/__init__.py
+-rw-r--r--   0        0        0     7034 2024-05-30 05:39:04.348672 athina-1.4.4/athina/runner/run.py
+-rw-r--r--   0        0        0      418 2024-05-30 05:39:04.349357 athina-1.4.4/athina/runner/run_wrapper.py
+-rw-r--r--   0        0        0     5729 2024-05-29 18:23:51.700266 athina-1.4.4/athina/scripts/guardrails.py
+-rw-r--r--   0        0        0    13810 2024-05-29 20:37:14.247205 athina-1.4.4/athina/services/athina_api_service.py
+-rw-r--r--   0        0        0      472 2024-05-29 18:23:47.849253 athina-1.4.4/athina/steps/__init__.py
+-rw-r--r--   0        0        0     2107 2024-05-28 05:27:42.582035 athina-1.4.4/athina/steps/api.py
+-rw-r--r--   0        0        0     4456 2024-05-22 07:52:50.229580 athina-1.4.4/athina/steps/base.py
+-rw-r--r--   0        0        0     1729 2024-05-22 07:52:50.229864 athina-1.4.4/athina/steps/chain.py
+-rw-r--r--   0        0        0     1346 2024-05-27 14:49:53.587855 athina-1.4.4/athina/steps/classify_text.py
+-rw-r--r--   0        0        0     1501 2024-05-22 07:52:50.230002 athina-1.4.4/athina/steps/conditional.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:52:50.230033 athina-1.4.4/athina/steps/debug.py
+-rw-r--r--   0        0        0     1440 2024-05-27 14:49:53.588354 athina-1.4.4/athina/steps/extract_entities.py
+-rw-r--r--   0        0        0      646 2024-05-22 07:52:50.230202 athina-1.4.4/athina/steps/iterator.py
+-rw-r--r--   0        0        0     4581 2024-06-01 12:17:34.394862 athina-1.4.4/athina/steps/llm.py
+-rw-r--r--   0        0        0      787 2024-05-22 07:52:50.230543 athina-1.4.4/athina/steps/transform.py
+-rw-r--r--   0        0        0     1136 2024-06-02 09:05:02.017058 athina-1.4.4/pyproject.toml
+-rw-r--r--   0        0        0     9992 1970-01-01 00:00:00.000000 athina-1.4.4/PKG-INFO
```

### Comparing `athina-1.4.3/README.md` & `athina-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/cli/cli.py` & `athina-1.4.4/athina/cli/cli.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/constants/messages.py` & `athina-1.4.4/athina/constants/messages.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/datasets/conversations.json` & `athina-1.4.4/athina/datasets/conversations.json`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/datasets/dataset.py` & `athina-1.4.4/athina/datasets/dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-import os
-import json
 from typing import Any, List, Optional
-import requests
-from dataclasses import dataclass, field, asdict
+from dataclasses import dataclass, field
 from athina.services.athina_api_service import AthinaApiService
 
 
 
 @dataclass
 class DatasetRow:
     query: Optional[str] = None
```

### Comparing `athina-1.4.3/athina/datasets/summarization_sample.py` & `athina-1.4.4/athina/datasets/summarization_sample.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/datasets/yc_query_mini.py` & `athina-1.4.4/athina/datasets/yc_query_mini.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/errors/exceptions.py` & `athina-1.4.4/athina/errors/exceptions.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/__init__.py` & `athina-1.4.4/athina/evals/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,16 @@
     Equals,
     StartsWith,
     EndsWith,
     LengthLessThan,
     LengthGreaterThan,
     LengthBetween,
     ApiCall,
-    OneLine
+    OneLine,
+    JsonEval
 )
 from athina.evals.grounded.wrapper import AnswerSimilarity, ContextSimilarity
 from athina.evals.guardrails.gibberish_text.evaluator import NotGibberishText
 from athina.evals.guardrails.sfw.evaluator import SafeForWorkText
 from athina.evals.guardrails.sensitive_topics.evaluator import ContainsNoSensitiveTopics
 from athina.evals.guardrails.profanity_free.evaluator import ProfanityFree
 from athina.evals.guardrails.detect_pii.evaluator import DetectPII
@@ -135,9 +136,10 @@
     "ReadingTime",
     "DetectPII",
     "ToxicLanguage",
     "CorrectLanguage",
     "NoSecretsPresent",
     "RestrictToTopic",
     "NotUnusualPrompt",
-    "PolitenessCheck"
-]
+    "PolitenessCheck",
+    "JsonEval"
+]
```

### Comparing `athina-1.4.3/athina/evals/base_evaluator.py` & `athina-1.4.4/athina/evals/base_evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/conversation/conversation_coherence/evaluator.py` & `athina-1.4.4/athina/evals/conversation/conversation_coherence/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/conversation/conversation_coherence/prompt.py` & `athina-1.4.4/athina/evals/conversation/conversation_coherence/prompt.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/conversation/conversation_resolution/evaluator.py` & `athina-1.4.4/athina/evals/conversation/conversation_resolution/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/conversation/conversation_resolution/prompt.py` & `athina-1.4.4/athina/evals/conversation/conversation_resolution/prompt.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/eval_type.py` & `athina-1.4.4/athina/evals/eval_type.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     EQUALS = "Equals"
     STARTS_WITH = "StartsWith"
     ENDS_WITH = "EndsWith"
     LENGTH_LESS_THAN = "LengthLessThan"
     LENGTH_GREATER_THAN = "LengthGreaterThan"
     LENGTH_BETWEEN = "LengthBetween"
     ONE_LINE = "OneLine"
+    JSON_EVAL = "JsonEval"
     API_CALL = "ApiCall"
     SAFE_FOR_WORK_TEXT = "SafeForWorkText"
     NOT_GIBBERISH_TEXT = "NotGibberishText"
     CONTAINS_NO_SENSITIVE_TOPICS = "ContainsNoSensitiveTopics"
     OPENAI_CONTENT_MODERATION = "OpenAiContentModeration"
     PII_DETECTION = "PiiDetection"
     PROMPT_INJECTION= "PromptInjection"
```

### Comparing `athina-1.4.3/athina/evals/function/function_evaluator.py` & `athina-1.4.4/athina/evals/function/function_evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/function/functions.py` & `athina-1.4.4/athina/evals/function/functions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,18 @@
+import os
 import re
 import json
 import requests
-from typing import Any, Optional
+from typing import Any, Dict, Optional, Union
+from athina.evals.grounded.similarity import CosineSimilarity
+from athina.helpers.logger import logger
+from athina.errors.exceptions import NoOpenAiApiKeyException
+from athina.helpers.json import extract_json_path, validate_json
+from athina.keys.openai_api_key import OpenAiApiKey
+from athina.llms.openai_service import OpenAiService
 
 
 def _standardize_url(url):
     """
     Generate a standardized URL by adding 'http://' if it's missing.
 
     Args:
@@ -582,14 +589,134 @@
         dict: A dictionary containing the result of the check and the reason for the result.
     """
     if "\n" in text or len(text.splitlines()) > 1:
         return {"result": False, "reason": "output contains multiple lines"}
     else:
         return {"result": True, "reason": "output is a single line"}
 
+def json_eval(
+    actual_json: Union[dict, str],
+    expected_json: Union[dict, str],
+    **kwargs
+) -> Dict[str, Any]:
+    """
+    Check if the actual JSON and expected JSON match the schema definition and follow validation rules.
+
+    Args:
+        actual_json (dict or str): The actual JSON string to compare against the expected JSON.
+        expected_json (dict or str): The expected JSON string to compare against the actual JSON.
+
+    """
+    try:
+        actual_json = _load_json(actual_json)
+        expected_json = _load_json(expected_json)
+        schema = _get_schema(kwargs)
+
+        if not schema:
+            return {"result": False, "reason": "Schema not provided"}
+
+        if not (_validate_json_with_schema(actual_json, schema) and _validate_json_with_schema(expected_json, schema)):
+            return {"result": False, "reason": "Schema validation failed"}
+
+        validations = kwargs.get("validations", [])
+        if validations:
+            for validation in validations:
+                if not _apply_validation(actual_json, expected_json, validation):
+                    return {"result": False, "reason": "Validation failed"}
+
+        return {"result": True, "reason": "Json eval passed"}
+    except Exception as e:
+        logger.error(f"Error occurred during eval: {e}")
+        raise e
+
+def _load_json(json_data: Union[dict, str]) -> dict:
+    if isinstance(json_data, str):
+        return json.loads(json_data)
+    return json_data
+
+def _get_schema(kwargs: Dict[str, Any]) -> dict:
+    schema = kwargs.get("schema")
+    if schema and isinstance(schema, str):
+        return json.loads(schema.replace("\n", "").replace("\t", ""))
+    return schema
+
+def _validate_json_with_schema(json_data: dict, schema: dict) -> bool:
+    return validate_json(json_data, schema)
+
+def _apply_validation(actual_json: dict, expected_json: dict, validation: dict) -> bool:
+    validating_function = validation.get("validating_function")
+    json_path = validation.get("json_path")
+    actual_value = extract_json_path(actual_json, json_path)
+    expected_value = extract_json_path(expected_json, json_path)
+
+    if validating_function == "Equals":
+        return _validate_equals(actual_value, expected_value, json_path)
+    elif validating_function == "Cosine Similarity":
+        return _validate_cosine_similarity(actual_value, expected_value, validation)
+    elif validating_function == "LLM Similarity":
+        return _validate_llm_similarity(actual_value, expected_value, validation)
+    else:
+        logger.error(f"Validation function {validating_function} not supported")
+        return False
+
+def _validate_equals(actual_value: Any, expected_value: Any, json_path: str) -> bool:
+    if actual_value != expected_value:
+        logger.error(f"JSON path {json_path} does not match expected value")
+        return False
+    return True
+
+def _validate_cosine_similarity(actual_value: str, expected_value: str, validation: dict) -> bool:
+    threshold = validation.get("pass_threshold", 0.8)
+    cosine_similarity = CosineSimilarity().compare(str(actual_value), str(expected_value))
+    if cosine_similarity < threshold:
+        logger.error(f"Cosine similarity score {cosine_similarity} is less than the threshold {threshold}")
+        return False
+    return True
+
+def _validate_llm_similarity(actual_value: str, expected_value: str, validation: dict) -> bool:
+    open_ai_api_key = validation.get("open_ai_api_key") or OpenAiApiKey.get_key() or os.environ.get("OPENAI_API_KEY")
+    if not open_ai_api_key:
+        raise NoOpenAiApiKeyException()
+
+    OpenAiApiKey.set_key(open_ai_api_key)
+    llm_service = OpenAiService()
+
+    system_message = """
+    You are an expert at evaluating whether two given strings are similar or not. Consider semantic similarity also while evaluating.
+    You MUST return a JSON object with the following fields: 
+    - result: Result must be either 'Pass' or 'Fail'.
+    - explanation: An explanation of why the result is Pass or Fail.
+    - score: Any matching score you have used to come to the result.
+    """
+
+    user_message = f"""
+    Following are two strings:
+    1. String 1: {actual_value}.
+    2. String 2: {expected_value}.
+    """
+
+    response = llm_service.json_completion(
+        model=validation.get("model", "gpt-3.5-turbo"),
+        messages=[
+            {"role": "system", "content": system_message},
+            {"role": "user", "content": user_message},
+        ],
+        temperature=0.0,
+    )
+
+    try:
+        result = response["result"]
+        explanation = response["explanation"]
+        if result == "Fail":
+            logger.error(f"LLM Similarity validation failed: {explanation}")
+            return False
+        return True
+    except Exception as e:
+        logger.error(f"Error occurred during LLM similarity validation: {e}")
+        return False
 
 """
 A dictionary containing the available operations and their corresponding functions.
 """
 operations = {
     "Regex": regex,
     "ContainsAny": contains_any,
@@ -606,9 +733,10 @@
     "Equals": equals,
     "StartsWith": starts_with,
     "EndsWith": ends_with,
     "LengthLessThan": length_less_than,
     "LengthGreaterThan": length_greater_than,
     "LengthBetween": length_between,
     "ApiCall": api_call,
-    "OneLine": one_line
+    "OneLine": one_line,
+    "JsonEval": json_eval,
 }
```

### Comparing `athina-1.4.3/athina/evals/function/wrapper.py` & `athina-1.4.4/athina/evals/function/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,8 +350,23 @@
         """
         Initialize the OneLine function evaluator.
         """
         super().__init__(
             function_name=FunctionEvalTypeId.ONE_LINE.value,
             function_arguments={},
             display_name=display_name,
+        )
+
+
+class JsonEval(FunctionEvaluator):
+    def __init__(self, schema: str, validations = None, display_name: Optional[str] = None):
+        """
+        Initialize the JsonEval function evaluator.
+        """
+        super().__init__(
+            function_name=FunctionEvalTypeId.JSON_EVAL.value,
+            function_arguments={
+                "schema": schema,
+                "validations": validations,
+            },
+            display_name=display_name,
         )
```

### Comparing `athina-1.4.3/athina/evals/grounded/grounded_evaluator.py` & `athina-1.4.4/athina/evals/grounded/grounded_evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/grounded/similarity.py` & `athina-1.4.4/athina/evals/grounded/similarity.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 import math
 from abc import ABC, abstractmethod
 
 class Comparator(ABC):
     @abstractmethod
     def compare(self, string1, string2):
         pass
@@ -18,15 +19,24 @@
         magnitude_vec2 = math.sqrt(sum([val**2 for val in vector2]))
         if magnitude_vec1 * magnitude_vec2 == 0:
             # Avoid division by zero
             return 0
         return dot_product / (magnitude_vec1 * magnitude_vec2)
 
     def _tokenize(self, string):
-        return string.lower().split()
+        """
+        Tokenize the input string into a list of words.
+        
+        Args:
+            string (str): The string to tokenize.
+        
+        Returns:
+            list: A list of lowercased words from the string.
+        """
+        return re.findall(r'\b\w+\b', string.lower())
 
     def _create_combined_set(self, string1, string2):
         return set(self._tokenize(string1)).union(set(self._tokenize(string2)))
 
     def _vectorize(self, string, combined_set):
         tokenized = self._tokenize(string)
         vector = [tokenized.count(word) for word in combined_set]
```

### Comparing `athina-1.4.3/athina/evals/grounded/wrapper.py` & `athina-1.4.4/athina/evals/grounded/wrapper.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/guardrails/correct_language/evaluator.py` & `athina-1.4.4/athina/evals/guardrails/correct_language/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/guardrails/detect_pii/evaluator.py` & `athina-1.4.4/athina/evals/guardrails/detect_pii/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/guardrails/gibberish_text/evaluator.py` & `athina-1.4.4/athina/evals/guardrails/gibberish_text/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/guardrails/no_secrets_present/evaluator.py` & `athina-1.4.4/athina/evals/guardrails/no_secrets_present/evaluator.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         metrics = []
         try:
             text = kwargs["response"]
             # Setup Guard
             guard = Guard.from_string(validators=[self.validator])
             # Pass LLM output through guard
             guard_result = guard.parse(text)
-            grade_reason = "Text contains secrets" if guard_result.validation_passed else "Text has no secrets"
+            grade_reason = "Text contains no secrets" if guard_result.validation_passed else "Text has secrets"
             # Boolean evaluator
             metrics.append(
                 EvalResultMetric(
                     id=MetricType.PASSED.value,
                     value=float(guard_result.validation_passed),
                 )
             )
```

### Comparing `athina-1.4.3/athina/evals/guardrails/politeness_check/evaluator.py` & `athina-1.4.4/athina/evals/guardrails/politeness_check/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/guardrails/profanity_free/evaluator.py` & `athina-1.4.4/athina/evals/guardrails/profanity_free/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/guardrails/reading_time/evaluator.py` & `athina-1.4.4/athina/evals/guardrails/reading_time/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/guardrails/restrict_to_topic/evaluator.py` & `athina-1.4.4/athina/evals/guardrails/restrict_to_topic/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/guardrails/sensitive_topics/evaluator.py` & `athina-1.4.4/athina/evals/guardrails/sensitive_topics/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/guardrails/sfw/evaluator.py` & `athina-1.4.4/athina/evals/guardrails/sfw/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/guardrails/toxic_language/evaluator.py` & `athina-1.4.4/athina/evals/guardrails/toxic_language/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/guardrails/unusual_prompt/evaluator.py` & `athina-1.4.4/athina/evals/guardrails/unusual_prompt/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/llm/context_contains_enough_information/evaluator.py` & `athina-1.4.4/athina/evals/llm/context_contains_enough_information/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/llm/context_contains_enough_information/examples.py` & `athina-1.4.4/athina/evals/llm/context_contains_enough_information/examples.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/llm/custom_prompt/evaluator.py` & `athina-1.4.4/athina/evals/llm/custom_prompt/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/llm/does_response_answer_query/evaluator.py` & `athina-1.4.4/athina/evals/llm/does_response_answer_query/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/llm/does_response_answer_query/examples.py` & `athina-1.4.4/athina/evals/llm/does_response_answer_query/examples.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/llm/example.py` & `athina-1.4.4/athina/evals/llm/example.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/llm/faithfulness/evaluator.py` & `athina-1.4.4/athina/evals/llm/faithfulness/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/llm/faithfulness/examples.py` & `athina-1.4.4/athina/evals/llm/faithfulness/examples.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/llm/grading_criteria/evaluator.py` & `athina-1.4.4/athina/evals/llm/grading_criteria/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/llm/groundedness/evaluator.py` & `athina-1.4.4/athina/evals/llm/groundedness/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/llm/groundedness/prompt.py` & `athina-1.4.4/athina/evals/llm/groundedness/prompt.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/llm/llm_evaluator.py` & `athina-1.4.4/athina/evals/llm/llm_evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/llm/summary_accuracy/evaluator.py` & `athina-1.4.4/athina/evals/llm/summary_accuracy/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/ragas/answer_correctness/evaluator.py` & `athina-1.4.4/athina/evals/ragas/answer_correctness/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/ragas/answer_relevancy/evaluator.py` & `athina-1.4.4/athina/evals/ragas/answer_relevancy/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/ragas/answer_semantic_similarity/evaluator.py` & `athina-1.4.4/athina/evals/ragas/answer_semantic_similarity/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/ragas/coherence/evaluator.py` & `athina-1.4.4/athina/evals/ragas/coherence/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/ragas/conciseness/evaluator.py` & `athina-1.4.4/athina/evals/ragas/conciseness/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/ragas/context_precision/evaluator.py` & `athina-1.4.4/athina/evals/ragas/context_precision/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/ragas/context_recall/evaluator.py` & `athina-1.4.4/athina/evals/ragas/context_recall/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/ragas/context_relevancy/evaluator.py` & `athina-1.4.4/athina/evals/ragas/context_relevancy/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/ragas/faithfulness/evaluator.py` & `athina-1.4.4/athina/evals/ragas/faithfulness/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/ragas/harmfulness/evaluator.py` & `athina-1.4.4/athina/evals/ragas/harmfulness/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/ragas/maliciousness/evaluator.py` & `athina-1.4.4/athina/evals/ragas/maliciousness/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/ragas/ragas_evaluator.py` & `athina-1.4.4/athina/evals/ragas/ragas_evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/safety/content_moderation/evaluator.py` & `athina-1.4.4/athina/evals/safety/content_moderation/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/safety/pii_detection/evaluator.py` & `athina-1.4.4/athina/evals/safety/pii_detection/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/evals/safety/prompt_injection/evaluator.py` & `athina-1.4.4/athina/evals/safety/prompt_injection/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/guard/guard.py` & `athina-1.4.4/athina/guard/guard.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/helpers/athina_logging_helper.py` & `athina-1.4.4/athina/helpers/athina_logging_helper.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/helpers/config.py` & `athina-1.4.4/athina/helpers/config.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/helpers/dataset_helper.py` & `athina-1.4.4/athina/helpers/dataset_helper.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/helpers/function_eval_util.py` & `athina-1.4.4/athina/helpers/function_eval_util.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/helpers/get_evaluator.py` & `athina-1.4.4/athina/helpers/get_evaluator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from athina.evals import Regex, ContainsAny, ContainsAll, Contains, ContainsNone, ContainsJson, ContainsEmail, IsJson, IsEmail, NoInvalidLinks, ContainsLink, ContainsValidLink, Equals, StartsWith, EndsWith, LengthLessThan, LengthGreaterThan, LengthBetween, ApiCall, DoesResponseAnswerQuery, Faithfulness, BaseEvaluator, ContextContainsEnoughInformation, SummaryAccuracy, Groundedness, GradingCriteria, CustomPrompt, RagasContextRelevancy, RagasAnswerRelevancy, RagasAnswerCorrectness, RagasAnswerSemanticSimilarity, RagasCoherence, RagasConciseness, RagasContextPrecision, RagasContextRecall, RagasFaithfulness, RagasHarmfulness, RagasMaliciousness, NotGibberishText, SafeForWorkText, ContainsNoSensitiveTopics, OpenAiContentModeration, PiiDetection, PromptInjection, ProfanityFree, ReadingTime, DetectPII, ToxicLanguage, CorrectLanguage, NoSecretsPresent, RestrictToTopic, NotUnusualPrompt, PolitenessCheck, OneLine
+from athina.evals import Regex, ContainsAny, ContainsAll, Contains, ContainsNone, ContainsJson, ContainsEmail, IsJson, IsEmail, NoInvalidLinks, ContainsLink, ContainsValidLink, Equals, StartsWith, EndsWith, LengthLessThan, LengthGreaterThan, LengthBetween, ApiCall, DoesResponseAnswerQuery, Faithfulness, BaseEvaluator, ContextContainsEnoughInformation, SummaryAccuracy, Groundedness, GradingCriteria, CustomPrompt, RagasContextRelevancy, RagasAnswerRelevancy, RagasAnswerCorrectness, RagasAnswerSemanticSimilarity, RagasCoherence, RagasConciseness, RagasContextPrecision, RagasContextRecall, RagasFaithfulness, RagasHarmfulness, RagasMaliciousness, NotGibberishText, SafeForWorkText, ContainsNoSensitiveTopics, OpenAiContentModeration, PiiDetection, PromptInjection, ProfanityFree, ReadingTime, DetectPII, ToxicLanguage, CorrectLanguage, NoSecretsPresent, RestrictToTopic, NotUnusualPrompt, PolitenessCheck, OneLine, JsonEval
 from athina.evals.grounded.similarity import CosineSimilarity, JaccardSimilarity, JaroWincklerSimilarity, NormalisedLevenshteinSimilarity, SorensenDiceSimilarity
 from athina.evals.grounded.wrapper import AnswerSimilarity, ContextSimilarity
 
 grounded_operations = {
     "AnswerSimilarity": AnswerSimilarity,
     "ContextSimilarity": ContextSimilarity,
 }
@@ -24,14 +24,15 @@
     "StartsWith": StartsWith,
     "EndsWith": EndsWith,
     "LengthLessThan": LengthLessThan,
     "LengthGreaterThan": LengthGreaterThan,
     "LengthBetween": LengthBetween,
     "ApiCall": ApiCall,
     "OneLine": OneLine,
+    "JsonEval": JsonEval
 }
 
 safety_operations = {
     "SafeForWorkText": SafeForWorkText,
     "NotGibberishText": NotGibberishText,
     "ContainsNoSensitiveTopics": ContainsNoSensitiveTopics,
     "OpenAiContentModeration" : OpenAiContentModeration,
```

### Comparing `athina-1.4.3/athina/helpers/json.py` & `athina-1.4.4/athina/helpers/json.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import json
+import jsonschema
+from jsonpath_ng import parse
+from jsonschema import validate
 from typing import Any, Optional
 
-
 class JsonHelper:
     @staticmethod
     def _extract_json(data_string: str) -> str:
         """
         Extracts a JSON string from a larger string.
         Assumes the JSON content starts with '{' and continues to the end of the input string.
         """
@@ -33,14 +35,28 @@
         # In case you cannot handle an error, return None
         if text is None:
             return None
         response_json_format = JsonHelper._extract_json(text)
         response_json = JsonHelper._load_json_from_text(response_json_format)
         return response_json
 
+def validate_json(json_data, schema):
+    try:
+        validate(instance=json_data, schema=schema)
+        return True
+    except jsonschema.exceptions.ValidationError as err:
+        return False
+
+def extract_json_path(json_data, json_path):
+    try:
+        jsonpath_expr = parse(json_path)
+        match = jsonpath_expr.find(json_data)
+        return [match.value for match in match] if match else None
+    except Exception as e:
+        return None
 
 # New and improved JsonExtractor
 # - can extract top-level arrays as well
 # - uses stack based approach
 class JsonExtractor:
     @staticmethod
     def extract_first_json_entity(text: str) -> Optional[Any]:
```

### Comparing `athina-1.4.3/athina/helpers/loader_helper.py` & `athina-1.4.4/athina/helpers/loader_helper.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/helpers/logger.py` & `athina-1.4.4/athina/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/helpers/run_helper.py` & `athina-1.4.4/athina/helpers/run_helper.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/interfaces/athina.py` & `athina-1.4.4/athina/interfaces/athina.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import json
 from enum import Enum
 from dataclasses import dataclass, asdict
 from typing import Optional, Dict, List, TypedDict, Any
+
 from .openai import OpenAiPromptMessage
 from .result import EvalResultMetric, DatapointFieldAnnotation
 
 
 @dataclass
 class AthinaInference:
     """Athina PromptRun class"""
```

### Comparing `athina-1.4.3/athina/interfaces/model.py` & `athina-1.4.4/athina/interfaces/model.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/interfaces/result.py` & `athina-1.4.4/athina/interfaces/result.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/llms/abstract_llm_service.py` & `athina-1.4.4/athina/llms/abstract_llm_service.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/llms/litellm_service.py` & `athina-1.4.4/athina/llms/litellm_service.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/llms/openai_service.py` & `athina-1.4.4/athina/llms/openai_service.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/llms/question_answerer_bulk.py` & `athina-1.4.4/athina/llms/question_answerer_bulk.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/llms/question_answerer_cot.py` & `athina-1.4.4/athina/llms/question_answerer_cot.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/llms/question_answerer_with_retrieval.py` & `athina-1.4.4/athina/llms/question_answerer_with_retrieval.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/llms/question_generator.py` & `athina-1.4.4/athina/llms/question_generator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/loaders/base_loader.py` & `athina-1.4.4/athina/loaders/base_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import ABC, abstractmethod
 from enum import Enum
-from typing import TypedDict, List
+from typing import List
 import json
 from athina.interfaces.data import DataPoint
 
 
 class LoadFormat(Enum):
     """Supported load formats."""
```

### Comparing `athina-1.4.3/athina/loaders/conversation_loader.py` & `athina-1.4.4/athina/loaders/conversation_loader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 from typing import List, Optional, Dict
 from athina.interfaces.athina import AthinaFilters
-from athina.interfaces.data import DataPoint as BaseDataPoint
-from .base_loader import BaseLoader
-from dataclasses import asdict
-from athina.services.athina_api_service import AthinaApiService
 
 
 class ConversationLoader():
     """
     This class is a data loader for conversation data
 
     Attributes:
```

### Comparing `athina-1.4.3/athina/loaders/loader.py` & `athina-1.4.4/athina/loaders/loader.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/loaders/response_loader.py` & `athina-1.4.4/athina/loaders/response_loader.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/loaders/summary_loader.py` & `athina-1.4.4/athina/loaders/summary_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from dataclasses import asdict
 from typing import List, Optional
 from athina.interfaces.athina import AthinaFilters
 from athina.interfaces.data import DataPoint
+from athina.services.athina_api_service import AthinaApiService
 from .base_loader import BaseLoader
 
 
 class SummaryDataPoint(DataPoint):
     """Data point for an LLM generated summary."""
     document: str
     response: str # summary
```

### Comparing `athina-1.4.3/athina/metrics/agreement_score.py` & `athina-1.4.4/athina/metrics/agreement_score.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/metrics/contradiction_score.py` & `athina-1.4.4/athina/metrics/contradiction_score.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/metrics/groundedness.py` & `athina-1.4.4/athina/metrics/groundedness.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/metrics/hallucination_score.py` & `athina-1.4.4/athina/metrics/hallucination_score.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/metrics/metric_type.py` & `athina-1.4.4/athina/metrics/metric_type.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/runner/run.py` & `athina-1.4.4/athina/runner/run.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/scripts/guardrails.py` & `athina-1.4.4/athina/scripts/guardrails.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/services/athina_api_service.py` & `athina-1.4.4/athina/services/athina_api_service.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/steps/api.py` & `athina-1.4.4/athina/steps/api.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/steps/base.py` & `athina-1.4.4/athina/steps/base.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/steps/chain.py` & `athina-1.4.4/athina/steps/chain.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/steps/classify_text.py` & `athina-1.4.4/athina/steps/classify_text.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/steps/conditional.py` & `athina-1.4.4/athina/steps/conditional.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/steps/extract_entities.py` & `athina-1.4.4/athina/steps/extract_entities.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/steps/iterator.py` & `athina-1.4.4/athina/steps/iterator.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/steps/llm.py` & `athina-1.4.4/athina/steps/llm.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/athina/steps/transform.py` & `athina-1.4.4/athina/steps/transform.py`

 * *Files identical despite different names*

### Comparing `athina-1.4.3/pyproject.toml` & `athina-1.4.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "athina"
-version = "1.4.3"
+version = "1.4.4"
 description = "Python SDK to configure and run evaluations for your LLM-based application"
 authors = ["Shiv Sakhuja <shiv@athina.ai>", "Akshat Gupta <akshat@athina.ai>", "Vivek Aditya <vivek@athina.ai>", "Akhil Bisht <akhil@athina.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 retrying = "^1.3.4"
@@ -23,14 +23,16 @@
 litellm = "1.35.6"
 jinja2 = "^3.1.4"
 marvin = "^2.3.4"
 pydantic = "2.6.3"
 pydantic-settings = "2.2.1"
 pydantic_core = "2.16.3"
 tokenizers = ">=0.19,<0.20"
+jsonschema = "^4.20.0"
+jsonpath-ng = "^1.6.0"
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.27.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `athina-1.4.3/PKG-INFO` & `athina-1.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: athina
-Version: 1.4.3
+Version: 1.4.4
 Summary: Python SDK to configure and run evaluations for your LLM-based application
 Author: Shiv Sakhuja
 Author-email: shiv@athina.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: colorlog (>=6.7.0,<7.0.0)
 Requires-Dist: datasets (>=2.16.0,<3.0.0)
 Requires-Dist: jinja2 (>=3.1.4,<4.0.0)
+Requires-Dist: jsonpath-ng (>=1.6.0,<2.0.0)
+Requires-Dist: jsonschema (>=4.20.0,<5.0.0)
 Requires-Dist: langchain (>=0.0.350)
 Requires-Dist: langchain-openai (>=0.0.3,<0.0.4)
 Requires-Dist: litellm (==1.35.6)
 Requires-Dist: llama-index (>=0.9.40,<0.10.0)
 Requires-Dist: marvin (>=2.3.4,<3.0.0)
 Requires-Dist: openai (>=1.3.4,<2.0.0)
 Requires-Dist: pandas
```

