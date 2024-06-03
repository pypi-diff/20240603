# Comparing `tmp/gigachain_experimental-0.0.59.tar.gz` & `tmp/gigachain_experimental-0.0.59.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigachain_experimental-0.0.59.tar", max compression
+gzip compressed data, was "gigachain_experimental-0.0.59.1.tar", max compression
```

## Comparing `gigachain_experimental-0.0.59.tar` & `gigachain_experimental-0.0.59.1.tar`

### file list

```diff
@@ -1,159 +1,165 @@
--rw-r--r--   0        0        0     1067 2023-12-18 12:05:46.761829 gigachain_experimental-0.0.59/LICENSE
--rw-r--r--   0        0        0      731 2023-10-06 14:43:01.321479 gigachain_experimental-0.0.59/README.md
--rw-r--r--   0        0        0      271 2023-10-19 12:57:52.560036 gigachain_experimental-0.0.59/langchain_experimental/__init__.py
--rw-r--r--   0        0        0      643 2024-04-19 07:38:33.791741 gigachain_experimental-0.0.59/langchain_experimental/agents/__init__.py
--rw-r--r--   0        0        0      653 2023-11-10 13:07:49.949600 gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/__init__.py
--rw-r--r--   0        0        0       19 2023-10-30 16:05:53.796780 gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/csv/__init__.py
--rw-r--r--   0        0        0     2407 2024-02-22 08:54:03.015149 gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/csv/base.py
--rw-r--r--   0        0        0       22 2023-10-19 12:57:52.561598 gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/pandas/__init__.py
--rw-r--r--   0        0        0    11933 2024-05-06 14:45:38.336392 gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/pandas/base.py
--rw-r--r--   0        0        0     1113 2023-10-19 12:57:52.562307 gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/pandas/prompt.py
--rw-r--r--   0        0        0        0 2023-10-19 12:57:52.562706 gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/python/__init__.py
--rw-r--r--   0        0        0     2229 2024-04-19 07:38:33.794226 gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/python/base.py
--rw-r--r--   0        0        0      513 2023-10-19 12:57:52.563558 gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/python/prompt.py
--rw-r--r--   0        0        0       20 2023-10-19 12:57:52.564007 gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/spark/__init__.py
--rw-r--r--   0        0        0     2766 2024-04-19 07:38:33.794958 gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/spark/base.py
--rw-r--r--   0        0        0      295 2023-10-19 12:57:52.565847 gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/spark/prompt.py
--rw-r--r--   0        0        0       23 2023-10-19 12:57:52.566362 gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/xorbits/__init__.py
--rw-r--r--   0        0        0     3148 2024-04-19 07:38:33.795570 gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/xorbits/base.py
--rw-r--r--   0        0        0     1070 2023-10-19 12:57:52.567043 gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/xorbits/prompt.py
--rw-r--r--   0        0        0      866 2024-04-19 07:38:33.796200 gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/__init__.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.490847 gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/autogpt/__init__.py
--rw-r--r--   0        0        0     5448 2024-05-06 14:45:38.337698 gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/autogpt/agent.py
--rw-r--r--   0        0        0     1148 2024-05-06 14:45:38.338529 gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/autogpt/memory.py
--rw-r--r--   0        0        0     1909 2024-03-28 12:44:20.391604 gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/autogpt/output_parser.py
--rw-r--r--   0        0        0     4989 2024-05-06 14:45:38.339455 gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/autogpt/prompt.py
--rw-r--r--   0        0        0     7963 2024-03-28 12:44:20.393342 gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/autogpt/prompt_generator.py
--rw-r--r--   0        0        0      514 2023-08-21 13:51:28.493975 gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/baby_agi/__init__.py
--rw-r--r--   0        0        0     8692 2024-04-19 07:38:33.797136 gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/baby_agi/baby_agi.py
--rw-r--r--   0        0        0     1668 2024-04-19 07:38:33.797963 gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/baby_agi/task_creation.py
--rw-r--r--   0        0        0      967 2024-04-19 07:38:33.798539 gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/baby_agi/task_execution.py
--rw-r--r--   0        0        0     1283 2024-04-19 07:38:33.799080 gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/baby_agi/task_prioritization.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.495536 gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/hugginggpt/__init__.py
--rw-r--r--   0        0        0     1133 2024-03-28 12:44:20.397027 gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/hugginggpt/hugginggpt.py
--rw-r--r--   0        0        0     1747 2024-04-19 07:38:33.800134 gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/hugginggpt/repsonse_generator.py
--rw-r--r--   0        0        0     4631 2024-05-06 14:45:38.340696 gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/hugginggpt/task_executor.py
--rw-r--r--   0        0        0     7869 2024-05-06 14:45:38.342283 gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/hugginggpt/task_planner.py
--rw-r--r--   0        0        0      674 2024-04-19 07:38:33.803295 gigachain_experimental-0.0.59/langchain_experimental/chat_models/__init__.py
--rw-r--r--   0        0        0     6068 2024-04-19 07:38:33.804258 gigachain_experimental-0.0.59/langchain_experimental/chat_models/llm_wrapper.py
--rw-r--r--   0        0        0     2190 2024-04-19 07:38:33.804875 gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/__init__.py
--rw-r--r--   0        0        0     6669 2024-04-19 07:38:33.805769 gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/amazon_comprehend_moderation.py
--rw-r--r--   0        0        0     7416 2024-04-19 07:38:33.806215 gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/base_moderation.py
--rw-r--r--   0        0        0     2390 2024-03-28 12:44:20.407747 gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/base_moderation_callbacks.py
--rw-r--r--   0        0        0     1614 2024-03-28 12:44:20.409023 gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/base_moderation_config.py
--rw-r--r--   0        0        0      192 2023-09-04 05:57:22.495380 gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/base_moderation_enums.py
--rw-r--r--   0        0        0     1054 2024-03-28 12:44:20.409588 gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/base_moderation_exceptions.py
--rw-r--r--   0        0        0     6834 2024-03-28 12:44:20.410890 gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/pii.py
--rw-r--r--   0        0        0     3142 2024-03-28 12:44:20.411826 gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/prompt_safety.py
--rw-r--r--   0        0        0     8134 2024-03-28 12:44:20.413206 gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/toxicity.py
--rw-r--r--   0        0        0      103 2023-10-03 07:51:15.765558 gigachain_experimental-0.0.59/langchain_experimental/cpal/README.md
--rw-r--r--   0        0        0      750 2024-04-19 07:38:33.806637 gigachain_experimental-0.0.59/langchain_experimental/cpal/__init__.py
--rw-r--r--   0        0        0    11097 2024-05-06 14:45:38.343644 gigachain_experimental-0.0.59/langchain_experimental/cpal/base.py
--rw-r--r--   0        0        0      246 2023-08-21 13:51:28.498799 gigachain_experimental-0.0.59/langchain_experimental/cpal/constants.py
--rw-r--r--   0        0        0     9183 2024-03-28 12:44:20.416997 gigachain_experimental-0.0.59/langchain_experimental/cpal/models.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.499460 gigachain_experimental-0.0.59/langchain_experimental/cpal/templates/__init__.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.499832 gigachain_experimental-0.0.59/langchain_experimental/cpal/templates/univariate/__init__.py
--rw-r--r--   0        0        0     2548 2023-10-19 12:57:52.577909 gigachain_experimental-0.0.59/langchain_experimental/cpal/templates/univariate/causal.py
--rw-r--r--   0        0        0      853 2023-10-19 12:57:52.579560 gigachain_experimental-0.0.59/langchain_experimental/cpal/templates/univariate/intervention.py
--rw-r--r--   0        0        0     2905 2023-10-19 12:57:52.581896 gigachain_experimental-0.0.59/langchain_experimental/cpal/templates/univariate/narrative.py
--rw-r--r--   0        0        0     5468 2023-10-19 12:57:52.583797 gigachain_experimental-0.0.59/langchain_experimental/cpal/templates/univariate/query.py
--rw-r--r--   0        0        0      631 2024-04-19 07:38:33.808411 gigachain_experimental-0.0.59/langchain_experimental/data_anonymizer/__init__.py
--rw-r--r--   0        0        0     1811 2024-03-28 12:44:20.419349 gigachain_experimental-0.0.59/langchain_experimental/data_anonymizer/base.py
--rw-r--r--   0        0        0     4793 2024-03-28 12:44:20.420547 gigachain_experimental-0.0.59/langchain_experimental/data_anonymizer/deanonymizer_mapping.py
--rw-r--r--   0        0        0     6801 2024-03-28 12:44:20.421773 gigachain_experimental-0.0.59/langchain_experimental/data_anonymizer/deanonymizer_matching_strategies.py
--rw-r--r--   0        0        0     2861 2024-03-28 12:44:20.422573 gigachain_experimental-0.0.59/langchain_experimental/data_anonymizer/faker_presidio_mapping.py
--rw-r--r--   0        0        0    17162 2024-03-28 12:44:20.423295 gigachain_experimental-0.0.59/langchain_experimental/data_anonymizer/presidio.py
--rw-r--r--   0        0        0      368 2024-04-19 07:38:33.808667 gigachain_experimental-0.0.59/langchain_experimental/fallacy_removal/__init__.py
--rw-r--r--   0        0        0      263 2024-04-19 07:38:33.809470 gigachain_experimental-0.0.59/langchain_experimental/generative_agents/__init__.py
--rw-r--r--   0        0        0    10252 2024-04-19 07:38:33.810327 gigachain_experimental-0.0.59/langchain_experimental/generative_agents/generative_agent.py
--rw-r--r--   0        0        0    13381 2024-05-06 14:45:38.345363 gigachain_experimental-0.0.59/langchain_experimental/generative_agents/memory.py
--rw-r--r--   0        0        0      308 2024-04-19 07:38:33.811851 gigachain_experimental-0.0.59/langchain_experimental/graph_transformers/__init__.py
--rw-r--r--   0        0        0    13383 2024-05-24 11:13:19.177918 gigachain_experimental-0.0.59/langchain_experimental/graph_transformers/diffbot.py
--rw-r--r--   0        0        0    26322 2024-05-24 11:13:19.179496 gigachain_experimental-0.0.59/langchain_experimental/graph_transformers/llm.py
--rw-r--r--   0        0        0       94 2024-04-19 07:38:33.814674 gigachain_experimental-0.0.59/langchain_experimental/llm_bash/__init__.py
--rw-r--r--   0        0        0     4459 2024-04-19 07:38:33.815315 gigachain_experimental-0.0.59/langchain_experimental/llm_bash/base.py
--rw-r--r--   0        0        0     5708 2024-03-28 12:44:20.431110 gigachain_experimental-0.0.59/langchain_experimental/llm_bash/bash.py
--rw-r--r--   0        0        0     2043 2024-05-06 14:45:38.347288 gigachain_experimental-0.0.59/langchain_experimental/llm_bash/prompt.py
--rw-r--r--   0        0        0      164 2024-04-19 07:38:33.815701 gigachain_experimental-0.0.59/langchain_experimental/llm_symbolic_math/__init__.py
--rw-r--r--   0        0        0     5801 2024-05-06 14:45:38.348165 gigachain_experimental-0.0.59/langchain_experimental/llm_symbolic_math/base.py
--rw-r--r--   0        0        0     1092 2024-05-06 14:45:38.348833 gigachain_experimental-0.0.59/langchain_experimental/llm_symbolic_math/prompt.py
--rw-r--r--   0        0        0      453 2024-04-19 07:38:33.816657 gigachain_experimental-0.0.59/langchain_experimental/llms/__init__.py
--rw-r--r--   0        0        0     8763 2024-05-24 11:13:19.180609 gigachain_experimental-0.0.59/langchain_experimental/llms/anthropic_functions.py
--rw-r--r--   0        0        0     2233 2024-04-19 07:38:33.818900 gigachain_experimental-0.0.59/langchain_experimental/llms/jsonformer_decoder.py
--rw-r--r--   0        0        0     4349 2024-04-19 07:38:33.820071 gigachain_experimental-0.0.59/langchain_experimental/llms/llamaapi.py
--rw-r--r--   0        0        0     2848 2024-04-19 07:38:33.820539 gigachain_experimental-0.0.59/langchain_experimental/llms/lmformatenforcer_decoder.py
--rw-r--r--   0        0        0    14354 2024-05-06 14:45:38.350675 gigachain_experimental-0.0.59/langchain_experimental/llms/ollama_functions.py
--rw-r--r--   0        0        0     2347 2024-04-19 07:38:33.821338 gigachain_experimental-0.0.59/langchain_experimental/llms/rellm_decoder.py
--rw-r--r--   0        0        0      346 2024-04-19 07:38:33.821711 gigachain_experimental-0.0.59/langchain_experimental/open_clip/__init__.py
--rw-r--r--   0        0        0     3383 2024-03-28 12:44:20.442806 gigachain_experimental-0.0.59/langchain_experimental/open_clip/open_clip.py
--rw-r--r--   0        0        0      120 2023-11-10 13:07:49.953805 gigachain_experimental-0.0.59/langchain_experimental/openai_assistant/__init__.py
--rw-r--r--   0        0        0      185 2023-11-15 10:30:09.322265 gigachain_experimental-0.0.59/langchain_experimental/openai_assistant/base.py
--rw-r--r--   0        0        0      330 2024-04-19 07:38:33.822200 gigachain_experimental-0.0.59/langchain_experimental/pal_chain/__init__.py
--rw-r--r--   0        0        0    13325 2024-04-19 07:38:33.822709 gigachain_experimental-0.0.59/langchain_experimental/pal_chain/base.py
--rw-r--r--   0        0        0     3542 2024-05-06 14:45:38.353511 gigachain_experimental-0.0.59/langchain_experimental/pal_chain/colored_object_prompt.py
--rw-r--r--   0        0        0     5772 2024-05-06 14:45:38.355134 gigachain_experimental-0.0.59/langchain_experimental/pal_chain/math_prompt.py
--rw-r--r--   0        0        0      488 2024-04-19 07:38:33.823092 gigachain_experimental-0.0.59/langchain_experimental/plan_and_execute/__init__.py
--rw-r--r--   0        0        0     3575 2024-04-19 07:38:33.823608 gigachain_experimental-0.0.59/langchain_experimental/plan_and_execute/agent_executor.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.508275 gigachain_experimental-0.0.59/langchain_experimental/plan_and_execute/executors/__init__.py
--rw-r--r--   0        0        0     1463 2024-01-18 15:16:40.555727 gigachain_experimental-0.0.59/langchain_experimental/plan_and_execute/executors/agent_executor.py
--rw-r--r--   0        0        0     1274 2024-04-19 07:38:33.824068 gigachain_experimental-0.0.59/langchain_experimental/plan_and_execute/executors/base.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.509270 gigachain_experimental-0.0.59/langchain_experimental/plan_and_execute/planners/__init__.py
--rw-r--r--   0        0        0     1572 2024-04-19 07:38:33.824672 gigachain_experimental-0.0.59/langchain_experimental/plan_and_execute/planners/base.py
--rw-r--r--   0        0        0     2319 2024-05-06 14:45:38.356213 gigachain_experimental-0.0.59/langchain_experimental/plan_and_execute/planners/chat_planner.py
--rw-r--r--   0        0        0     1439 2024-03-28 12:44:20.445521 gigachain_experimental-0.0.59/langchain_experimental/plan_and_execute/schema.py
--rw-r--r--   0        0        0      369 2024-04-19 07:38:33.825351 gigachain_experimental-0.0.59/langchain_experimental/prompt_injection_identifier/__init__.py
--rw-r--r--   0        0        0     3381 2024-05-06 14:45:38.356762 gigachain_experimental-0.0.59/langchain_experimental/prompt_injection_identifier/hugging_face_identifier.py
--rw-r--r--   0        0        0      174 2024-04-19 07:38:33.826287 gigachain_experimental-0.0.59/langchain_experimental/prompts/__init__.py
--rw-r--r--   0        0        0       82 2024-05-06 14:45:38.357304 gigachain_experimental-0.0.59/langchain_experimental/prompts/load.py
--rw-r--r--   0        0        0        0 2023-08-22 08:04:55.368181 gigachain_experimental-0.0.59/langchain_experimental/py.typed
--rw-r--r--   0        0        0     1285 2023-08-24 07:36:02.836411 gigachain_experimental-0.0.59/langchain_experimental/pydantic_v1/__init__.py
--rw-r--r--   0        0        0      548 2023-08-24 07:36:02.836900 gigachain_experimental-0.0.59/langchain_experimental/pydantic_v1/dataclasses.py
--rw-r--r--   0        0        0      520 2023-08-24 07:36:02.837404 gigachain_experimental-0.0.59/langchain_experimental/pydantic_v1/main.py
--rw-r--r--   0        0        0      518 2024-04-19 07:38:33.827066 gigachain_experimental-0.0.59/langchain_experimental/recommenders/__init__.py
--rw-r--r--   0        0        0     7967 2024-04-19 07:38:33.827709 gigachain_experimental-0.0.59/langchain_experimental/recommenders/amazon_personalize.py
--rw-r--r--   0        0        0     6974 2024-05-06 14:45:38.359152 gigachain_experimental-0.0.59/langchain_experimental/recommenders/amazon_personalize_chain.py
--rw-r--r--   0        0        0      200 2024-04-19 07:38:33.829182 gigachain_experimental-0.0.59/langchain_experimental/retrievers/__init__.py
--rw-r--r--   0        0        0     1253 2024-04-19 07:38:33.829861 gigachain_experimental-0.0.59/langchain_experimental/retrievers/vector_sql_database.py
--rw-r--r--   0        0        0     1447 2024-04-19 07:38:33.830696 gigachain_experimental-0.0.59/langchain_experimental/rl_chain/__init__.py
--rw-r--r--   0        0        0    23251 2024-05-06 14:45:38.359748 gigachain_experimental-0.0.59/langchain_experimental/rl_chain/base.py
--rw-r--r--   0        0        0     1989 2024-03-28 12:44:20.456634 gigachain_experimental-0.0.59/langchain_experimental/rl_chain/metrics.py
--rw-r--r--   0        0        0     2126 2024-03-28 12:44:20.457637 gigachain_experimental-0.0.59/langchain_experimental/rl_chain/model_repository.py
--rw-r--r--   0        0        0    16289 2024-05-06 14:45:38.360601 gigachain_experimental-0.0.59/langchain_experimental/rl_chain/pick_best_chain.py
--rw-r--r--   0        0        0      556 2024-03-28 12:44:20.459800 gigachain_experimental-0.0.59/langchain_experimental/rl_chain/vw_logger.py
--rw-r--r--   0        0        0      946 2024-04-19 07:38:33.832517 gigachain_experimental-0.0.59/langchain_experimental/smart_llm/__init__.py
--rw-r--r--   0        0        0    14438 2024-05-06 14:45:38.362010 gigachain_experimental-0.0.59/langchain_experimental/smart_llm/base.py
--rw-r--r--   0        0        0      202 2024-04-19 07:38:33.834385 gigachain_experimental-0.0.59/langchain_experimental/sql/__init__.py
--rw-r--r--   0        0        0    13257 2024-05-06 14:45:38.362879 gigachain_experimental-0.0.59/langchain_experimental/sql/base.py
--rw-r--r--   0        0        0     4663 2024-05-06 14:45:38.363512 gigachain_experimental-0.0.59/langchain_experimental/sql/prompt.py
--rw-r--r--   0        0        0     9856 2024-05-06 14:45:38.364173 gigachain_experimental-0.0.59/langchain_experimental/sql/vector_sql.py
--rw-r--r--   0        0        0     1576 2024-04-19 07:38:33.836627 gigachain_experimental-0.0.59/langchain_experimental/synthetic_data/__init__.py
--rw-r--r--   0        0        0      464 2024-05-06 14:45:38.364970 gigachain_experimental-0.0.59/langchain_experimental/synthetic_data/prompts.py
--rw-r--r--   0        0        0       75 2024-04-19 07:38:33.837144 gigachain_experimental-0.0.59/langchain_experimental/tabular_synthetic_data/__init__.py
--rw-r--r--   0        0        0     5346 2024-05-06 14:45:38.365645 gigachain_experimental-0.0.59/langchain_experimental/tabular_synthetic_data/base.py
--rw-r--r--   0        0        0     2523 2024-04-19 07:38:33.837650 gigachain_experimental-0.0.59/langchain_experimental/tabular_synthetic_data/openai.py
--rw-r--r--   0        0        0      417 2024-05-06 14:45:38.366178 gigachain_experimental-0.0.59/langchain_experimental/tabular_synthetic_data/prompts.py
--rw-r--r--   0        0        0     9850 2024-05-06 14:45:38.366807 gigachain_experimental-0.0.59/langchain_experimental/text_splitter.py
--rw-r--r--   0        0        0      180 2024-04-19 07:38:33.839237 gigachain_experimental-0.0.59/langchain_experimental/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-10-19 12:57:52.604149 gigachain_experimental-0.0.59/langchain_experimental/tools/python/__init__.py
--rw-r--r--   0        0        0     4768 2024-04-19 07:38:33.840630 gigachain_experimental-0.0.59/langchain_experimental/tools/python/tool.py
--rw-r--r--   0        0        0      425 2024-04-19 07:38:33.841264 gigachain_experimental-0.0.59/langchain_experimental/tot/__init__.py
--rw-r--r--   0        0        0     4858 2024-04-19 07:38:33.842457 gigachain_experimental-0.0.59/langchain_experimental/tot/base.py
--rw-r--r--   0        0        0     1410 2024-04-19 07:38:33.843054 gigachain_experimental-0.0.59/langchain_experimental/tot/checker.py
--rw-r--r--   0        0        0     1666 2023-08-21 13:51:28.515184 gigachain_experimental-0.0.59/langchain_experimental/tot/controller.py
--rw-r--r--   0        0        0     1467 2024-03-28 12:44:20.474461 gigachain_experimental-0.0.59/langchain_experimental/tot/memory.py
--rw-r--r--   0        0        0     4797 2024-04-19 07:38:33.843690 gigachain_experimental-0.0.59/langchain_experimental/tot/prompts.py
--rw-r--r--   0        0        0      504 2024-03-28 12:44:20.475874 gigachain_experimental-0.0.59/langchain_experimental/tot/thought.py
--rw-r--r--   0        0        0     3123 2024-05-06 14:45:38.367342 gigachain_experimental-0.0.59/langchain_experimental/tot/thought_generation.py
--rw-r--r--   0        0        0      148 2024-04-19 07:38:33.844253 gigachain_experimental-0.0.59/langchain_experimental/utilities/__init__.py
--rw-r--r--   0        0        0     2690 2024-05-06 14:45:38.367934 gigachain_experimental-0.0.59/langchain_experimental/utilities/python.py
--rw-r--r--   0        0        0      114 2024-04-19 07:38:33.844644 gigachain_experimental-0.0.59/langchain_experimental/video_captioning/__init__.py
--rw-r--r--   0        0        0     5034 2024-04-19 07:38:33.845065 gigachain_experimental-0.0.59/langchain_experimental/video_captioning/base.py
--rw-r--r--   0        0        0     4880 2024-04-19 07:38:33.845525 gigachain_experimental-0.0.59/langchain_experimental/video_captioning/models.py
--rw-r--r--   0        0        0     4369 2024-04-19 07:38:33.845977 gigachain_experimental-0.0.59/langchain_experimental/video_captioning/prompts.py
--rw-r--r--   0        0        0     3196 2024-04-19 07:38:33.846553 gigachain_experimental-0.0.59/langchain_experimental/video_captioning/services/audio_service.py
--rw-r--r--   0        0        0    11301 2024-04-19 07:38:33.847251 gigachain_experimental-0.0.59/langchain_experimental/video_captioning/services/caption_service.py
--rw-r--r--   0        0        0     4932 2024-04-19 07:38:33.848536 gigachain_experimental-0.0.59/langchain_experimental/video_captioning/services/combine_service.py
--rw-r--r--   0        0        0     3773 2024-04-19 07:38:33.848986 gigachain_experimental-0.0.59/langchain_experimental/video_captioning/services/image_service.py
--rw-r--r--   0        0        0      459 2024-04-19 07:38:33.849333 gigachain_experimental-0.0.59/langchain_experimental/video_captioning/services/srt_service.py
--rw-r--r--   0        0        0     4065 2024-05-24 11:13:58.827756 gigachain_experimental-0.0.59/pyproject.toml
--rw-r--r--   0        0        0     2076 1970-01-01 00:00:00.000000 gigachain_experimental-0.0.59/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-12-18 12:05:46.761829 gigachain_experimental-0.0.59.1/LICENSE
+-rw-r--r--   0        0        0      731 2023-10-06 14:43:01.321479 gigachain_experimental-0.0.59.1/README.md
+-rw-r--r--   0        0        0      532 2024-06-03 09:22:22.985203 gigachain_experimental-0.0.59.1/langchain_experimental/__init__.py
+-rw-r--r--   0        0        0      643 2024-04-19 07:38:33.791741 gigachain_experimental-0.0.59.1/langchain_experimental/agents/__init__.py
+-rw-r--r--   0        0        0      653 2023-11-10 13:07:49.949600 gigachain_experimental-0.0.59.1/langchain_experimental/agents/agent_toolkits/__init__.py
+-rw-r--r--   0        0        0       19 2023-10-30 16:05:53.796780 gigachain_experimental-0.0.59.1/langchain_experimental/agents/agent_toolkits/csv/__init__.py
+-rw-r--r--   0        0        0     2407 2024-02-22 08:54:03.015149 gigachain_experimental-0.0.59.1/langchain_experimental/agents/agent_toolkits/csv/base.py
+-rw-r--r--   0        0        0        0 2024-06-03 09:19:02.771114 gigachain_experimental-0.0.59.1/langchain_experimental/agents/agent_toolkits/gigapython/__init__.py
+-rw-r--r--   0        0        0     3366 2024-06-03 09:19:02.772437 gigachain_experimental-0.0.59.1/langchain_experimental/agents/agent_toolkits/gigapython/base.py
+-rw-r--r--   0        0        0      675 2024-06-03 09:19:02.772925 gigachain_experimental-0.0.59.1/langchain_experimental/agents/agent_toolkits/gigapython/parser.py
+-rw-r--r--   0        0        0       22 2023-10-19 12:57:52.561598 gigachain_experimental-0.0.59.1/langchain_experimental/agents/agent_toolkits/pandas/__init__.py
+-rw-r--r--   0        0        0    11933 2024-05-06 14:45:38.336392 gigachain_experimental-0.0.59.1/langchain_experimental/agents/agent_toolkits/pandas/base.py
+-rw-r--r--   0        0        0     1113 2023-10-19 12:57:52.562307 gigachain_experimental-0.0.59.1/langchain_experimental/agents/agent_toolkits/pandas/prompt.py
+-rw-r--r--   0        0        0        0 2023-10-19 12:57:52.562706 gigachain_experimental-0.0.59.1/langchain_experimental/agents/agent_toolkits/python/__init__.py
+-rw-r--r--   0        0        0     2229 2024-04-19 07:38:33.794226 gigachain_experimental-0.0.59.1/langchain_experimental/agents/agent_toolkits/python/base.py
+-rw-r--r--   0        0        0      513 2023-10-19 12:57:52.563558 gigachain_experimental-0.0.59.1/langchain_experimental/agents/agent_toolkits/python/prompt.py
+-rw-r--r--   0        0        0       20 2023-10-19 12:57:52.564007 gigachain_experimental-0.0.59.1/langchain_experimental/agents/agent_toolkits/spark/__init__.py
+-rw-r--r--   0        0        0     2766 2024-04-19 07:38:33.794958 gigachain_experimental-0.0.59.1/langchain_experimental/agents/agent_toolkits/spark/base.py
+-rw-r--r--   0        0        0      295 2023-10-19 12:57:52.565847 gigachain_experimental-0.0.59.1/langchain_experimental/agents/agent_toolkits/spark/prompt.py
+-rw-r--r--   0        0        0       23 2023-10-19 12:57:52.566362 gigachain_experimental-0.0.59.1/langchain_experimental/agents/agent_toolkits/xorbits/__init__.py
+-rw-r--r--   0        0        0     3148 2024-04-19 07:38:33.795570 gigachain_experimental-0.0.59.1/langchain_experimental/agents/agent_toolkits/xorbits/base.py
+-rw-r--r--   0        0        0     1070 2023-10-19 12:57:52.567043 gigachain_experimental-0.0.59.1/langchain_experimental/agents/agent_toolkits/xorbits/prompt.py
+-rw-r--r--   0        0        0      866 2024-04-19 07:38:33.796200 gigachain_experimental-0.0.59.1/langchain_experimental/autonomous_agents/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.490847 gigachain_experimental-0.0.59.1/langchain_experimental/autonomous_agents/autogpt/__init__.py
+-rw-r--r--   0        0        0     5448 2024-05-06 14:45:38.337698 gigachain_experimental-0.0.59.1/langchain_experimental/autonomous_agents/autogpt/agent.py
+-rw-r--r--   0        0        0     1148 2024-05-06 14:45:38.338529 gigachain_experimental-0.0.59.1/langchain_experimental/autonomous_agents/autogpt/memory.py
+-rw-r--r--   0        0        0     1909 2024-03-28 12:44:20.391604 gigachain_experimental-0.0.59.1/langchain_experimental/autonomous_agents/autogpt/output_parser.py
+-rw-r--r--   0        0        0     4989 2024-05-06 14:45:38.339455 gigachain_experimental-0.0.59.1/langchain_experimental/autonomous_agents/autogpt/prompt.py
+-rw-r--r--   0        0        0     7963 2024-03-28 12:44:20.393342 gigachain_experimental-0.0.59.1/langchain_experimental/autonomous_agents/autogpt/prompt_generator.py
+-rw-r--r--   0        0        0      514 2023-08-21 13:51:28.493975 gigachain_experimental-0.0.59.1/langchain_experimental/autonomous_agents/baby_agi/__init__.py
+-rw-r--r--   0        0        0     8692 2024-04-19 07:38:33.797136 gigachain_experimental-0.0.59.1/langchain_experimental/autonomous_agents/baby_agi/baby_agi.py
+-rw-r--r--   0        0        0     1668 2024-04-19 07:38:33.797963 gigachain_experimental-0.0.59.1/langchain_experimental/autonomous_agents/baby_agi/task_creation.py
+-rw-r--r--   0        0        0      967 2024-04-19 07:38:33.798539 gigachain_experimental-0.0.59.1/langchain_experimental/autonomous_agents/baby_agi/task_execution.py
+-rw-r--r--   0        0        0     1283 2024-04-19 07:38:33.799080 gigachain_experimental-0.0.59.1/langchain_experimental/autonomous_agents/baby_agi/task_prioritization.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.495536 gigachain_experimental-0.0.59.1/langchain_experimental/autonomous_agents/hugginggpt/__init__.py
+-rw-r--r--   0        0        0     1133 2024-03-28 12:44:20.397027 gigachain_experimental-0.0.59.1/langchain_experimental/autonomous_agents/hugginggpt/hugginggpt.py
+-rw-r--r--   0        0        0     1747 2024-04-19 07:38:33.800134 gigachain_experimental-0.0.59.1/langchain_experimental/autonomous_agents/hugginggpt/repsonse_generator.py
+-rw-r--r--   0        0        0     4631 2024-05-06 14:45:38.340696 gigachain_experimental-0.0.59.1/langchain_experimental/autonomous_agents/hugginggpt/task_executor.py
+-rw-r--r--   0        0        0     7869 2024-05-06 14:45:38.342283 gigachain_experimental-0.0.59.1/langchain_experimental/autonomous_agents/hugginggpt/task_planner.py
+-rw-r--r--   0        0        0      674 2024-04-19 07:38:33.803295 gigachain_experimental-0.0.59.1/langchain_experimental/chat_models/__init__.py
+-rw-r--r--   0        0        0     6068 2024-04-19 07:38:33.804258 gigachain_experimental-0.0.59.1/langchain_experimental/chat_models/llm_wrapper.py
+-rw-r--r--   0        0        0     2190 2024-04-19 07:38:33.804875 gigachain_experimental-0.0.59.1/langchain_experimental/comprehend_moderation/__init__.py
+-rw-r--r--   0        0        0     6669 2024-04-19 07:38:33.805769 gigachain_experimental-0.0.59.1/langchain_experimental/comprehend_moderation/amazon_comprehend_moderation.py
+-rw-r--r--   0        0        0     7416 2024-04-19 07:38:33.806215 gigachain_experimental-0.0.59.1/langchain_experimental/comprehend_moderation/base_moderation.py
+-rw-r--r--   0        0        0     2390 2024-03-28 12:44:20.407747 gigachain_experimental-0.0.59.1/langchain_experimental/comprehend_moderation/base_moderation_callbacks.py
+-rw-r--r--   0        0        0     1614 2024-03-28 12:44:20.409023 gigachain_experimental-0.0.59.1/langchain_experimental/comprehend_moderation/base_moderation_config.py
+-rw-r--r--   0        0        0      192 2023-09-04 05:57:22.495380 gigachain_experimental-0.0.59.1/langchain_experimental/comprehend_moderation/base_moderation_enums.py
+-rw-r--r--   0        0        0     1054 2024-03-28 12:44:20.409588 gigachain_experimental-0.0.59.1/langchain_experimental/comprehend_moderation/base_moderation_exceptions.py
+-rw-r--r--   0        0        0     6834 2024-03-28 12:44:20.410890 gigachain_experimental-0.0.59.1/langchain_experimental/comprehend_moderation/pii.py
+-rw-r--r--   0        0        0     3142 2024-03-28 12:44:20.411826 gigachain_experimental-0.0.59.1/langchain_experimental/comprehend_moderation/prompt_safety.py
+-rw-r--r--   0        0        0     8134 2024-03-28 12:44:20.413206 gigachain_experimental-0.0.59.1/langchain_experimental/comprehend_moderation/toxicity.py
+-rw-r--r--   0        0        0      103 2023-10-03 07:51:15.765558 gigachain_experimental-0.0.59.1/langchain_experimental/cpal/README.md
+-rw-r--r--   0        0        0      750 2024-04-19 07:38:33.806637 gigachain_experimental-0.0.59.1/langchain_experimental/cpal/__init__.py
+-rw-r--r--   0        0        0    11097 2024-05-06 14:45:38.343644 gigachain_experimental-0.0.59.1/langchain_experimental/cpal/base.py
+-rw-r--r--   0        0        0      246 2023-08-21 13:51:28.498799 gigachain_experimental-0.0.59.1/langchain_experimental/cpal/constants.py
+-rw-r--r--   0        0        0     9183 2024-03-28 12:44:20.416997 gigachain_experimental-0.0.59.1/langchain_experimental/cpal/models.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.499460 gigachain_experimental-0.0.59.1/langchain_experimental/cpal/templates/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.499832 gigachain_experimental-0.0.59.1/langchain_experimental/cpal/templates/univariate/__init__.py
+-rw-r--r--   0        0        0     2548 2023-10-19 12:57:52.577909 gigachain_experimental-0.0.59.1/langchain_experimental/cpal/templates/univariate/causal.py
+-rw-r--r--   0        0        0      853 2023-10-19 12:57:52.579560 gigachain_experimental-0.0.59.1/langchain_experimental/cpal/templates/univariate/intervention.py
+-rw-r--r--   0        0        0     2905 2023-10-19 12:57:52.581896 gigachain_experimental-0.0.59.1/langchain_experimental/cpal/templates/univariate/narrative.py
+-rw-r--r--   0        0        0     5468 2023-10-19 12:57:52.583797 gigachain_experimental-0.0.59.1/langchain_experimental/cpal/templates/univariate/query.py
+-rw-r--r--   0        0        0      631 2024-04-19 07:38:33.808411 gigachain_experimental-0.0.59.1/langchain_experimental/data_anonymizer/__init__.py
+-rw-r--r--   0        0        0     1811 2024-03-28 12:44:20.419349 gigachain_experimental-0.0.59.1/langchain_experimental/data_anonymizer/base.py
+-rw-r--r--   0        0        0     4793 2024-03-28 12:44:20.420547 gigachain_experimental-0.0.59.1/langchain_experimental/data_anonymizer/deanonymizer_mapping.py
+-rw-r--r--   0        0        0     6801 2024-03-28 12:44:20.421773 gigachain_experimental-0.0.59.1/langchain_experimental/data_anonymizer/deanonymizer_matching_strategies.py
+-rw-r--r--   0        0        0     2861 2024-03-28 12:44:20.422573 gigachain_experimental-0.0.59.1/langchain_experimental/data_anonymizer/faker_presidio_mapping.py
+-rw-r--r--   0        0        0    17162 2024-03-28 12:44:20.423295 gigachain_experimental-0.0.59.1/langchain_experimental/data_anonymizer/presidio.py
+-rw-r--r--   0        0        0      368 2024-04-19 07:38:33.808667 gigachain_experimental-0.0.59.1/langchain_experimental/fallacy_removal/__init__.py
+-rw-r--r--   0        0        0      263 2024-04-19 07:38:33.809470 gigachain_experimental-0.0.59.1/langchain_experimental/generative_agents/__init__.py
+-rw-r--r--   0        0        0    10252 2024-04-19 07:38:33.810327 gigachain_experimental-0.0.59.1/langchain_experimental/generative_agents/generative_agent.py
+-rw-r--r--   0        0        0    13381 2024-05-06 14:45:38.345363 gigachain_experimental-0.0.59.1/langchain_experimental/generative_agents/memory.py
+-rw-r--r--   0        0        0      308 2024-04-19 07:38:33.811851 gigachain_experimental-0.0.59.1/langchain_experimental/graph_transformers/__init__.py
+-rw-r--r--   0        0        0    13383 2024-05-24 11:13:19.177918 gigachain_experimental-0.0.59.1/langchain_experimental/graph_transformers/diffbot.py
+-rw-r--r--   0        0        0    26322 2024-05-24 11:13:19.179496 gigachain_experimental-0.0.59.1/langchain_experimental/graph_transformers/llm.py
+-rw-r--r--   0        0        0       94 2024-04-19 07:38:33.814674 gigachain_experimental-0.0.59.1/langchain_experimental/llm_bash/__init__.py
+-rw-r--r--   0        0        0     4459 2024-04-19 07:38:33.815315 gigachain_experimental-0.0.59.1/langchain_experimental/llm_bash/base.py
+-rw-r--r--   0        0        0     5708 2024-03-28 12:44:20.431110 gigachain_experimental-0.0.59.1/langchain_experimental/llm_bash/bash.py
+-rw-r--r--   0        0        0     2043 2024-05-06 14:45:38.347288 gigachain_experimental-0.0.59.1/langchain_experimental/llm_bash/prompt.py
+-rw-r--r--   0        0        0      164 2024-04-19 07:38:33.815701 gigachain_experimental-0.0.59.1/langchain_experimental/llm_symbolic_math/__init__.py
+-rw-r--r--   0        0        0     5801 2024-05-06 14:45:38.348165 gigachain_experimental-0.0.59.1/langchain_experimental/llm_symbolic_math/base.py
+-rw-r--r--   0        0        0     1092 2024-05-06 14:45:38.348833 gigachain_experimental-0.0.59.1/langchain_experimental/llm_symbolic_math/prompt.py
+-rw-r--r--   0        0        0      453 2024-04-19 07:38:33.816657 gigachain_experimental-0.0.59.1/langchain_experimental/llms/__init__.py
+-rw-r--r--   0        0        0     8763 2024-05-24 11:13:19.180609 gigachain_experimental-0.0.59.1/langchain_experimental/llms/anthropic_functions.py
+-rw-r--r--   0        0        0     2233 2024-04-19 07:38:33.818900 gigachain_experimental-0.0.59.1/langchain_experimental/llms/jsonformer_decoder.py
+-rw-r--r--   0        0        0     4349 2024-04-19 07:38:33.820071 gigachain_experimental-0.0.59.1/langchain_experimental/llms/llamaapi.py
+-rw-r--r--   0        0        0     2848 2024-04-19 07:38:33.820539 gigachain_experimental-0.0.59.1/langchain_experimental/llms/lmformatenforcer_decoder.py
+-rw-r--r--   0        0        0    14354 2024-05-06 14:45:38.350675 gigachain_experimental-0.0.59.1/langchain_experimental/llms/ollama_functions.py
+-rw-r--r--   0        0        0     2347 2024-04-19 07:38:33.821338 gigachain_experimental-0.0.59.1/langchain_experimental/llms/rellm_decoder.py
+-rw-r--r--   0        0        0      346 2024-04-19 07:38:33.821711 gigachain_experimental-0.0.59.1/langchain_experimental/open_clip/__init__.py
+-rw-r--r--   0        0        0     3383 2024-03-28 12:44:20.442806 gigachain_experimental-0.0.59.1/langchain_experimental/open_clip/open_clip.py
+-rw-r--r--   0        0        0      120 2023-11-10 13:07:49.953805 gigachain_experimental-0.0.59.1/langchain_experimental/openai_assistant/__init__.py
+-rw-r--r--   0        0        0      185 2023-11-15 10:30:09.322265 gigachain_experimental-0.0.59.1/langchain_experimental/openai_assistant/base.py
+-rw-r--r--   0        0        0      330 2024-04-19 07:38:33.822200 gigachain_experimental-0.0.59.1/langchain_experimental/pal_chain/__init__.py
+-rw-r--r--   0        0        0    13325 2024-04-19 07:38:33.822709 gigachain_experimental-0.0.59.1/langchain_experimental/pal_chain/base.py
+-rw-r--r--   0        0        0     3542 2024-05-06 14:45:38.353511 gigachain_experimental-0.0.59.1/langchain_experimental/pal_chain/colored_object_prompt.py
+-rw-r--r--   0        0        0     5772 2024-05-06 14:45:38.355134 gigachain_experimental-0.0.59.1/langchain_experimental/pal_chain/math_prompt.py
+-rw-r--r--   0        0        0      488 2024-04-19 07:38:33.823092 gigachain_experimental-0.0.59.1/langchain_experimental/plan_and_execute/__init__.py
+-rw-r--r--   0        0        0     3575 2024-04-19 07:38:33.823608 gigachain_experimental-0.0.59.1/langchain_experimental/plan_and_execute/agent_executor.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.508275 gigachain_experimental-0.0.59.1/langchain_experimental/plan_and_execute/executors/__init__.py
+-rw-r--r--   0        0        0     1463 2024-01-18 15:16:40.555727 gigachain_experimental-0.0.59.1/langchain_experimental/plan_and_execute/executors/agent_executor.py
+-rw-r--r--   0        0        0     1274 2024-04-19 07:38:33.824068 gigachain_experimental-0.0.59.1/langchain_experimental/plan_and_execute/executors/base.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.509270 gigachain_experimental-0.0.59.1/langchain_experimental/plan_and_execute/planners/__init__.py
+-rw-r--r--   0        0        0     1572 2024-04-19 07:38:33.824672 gigachain_experimental-0.0.59.1/langchain_experimental/plan_and_execute/planners/base.py
+-rw-r--r--   0        0        0     2319 2024-05-06 14:45:38.356213 gigachain_experimental-0.0.59.1/langchain_experimental/plan_and_execute/planners/chat_planner.py
+-rw-r--r--   0        0        0     1439 2024-03-28 12:44:20.445521 gigachain_experimental-0.0.59.1/langchain_experimental/plan_and_execute/schema.py
+-rw-r--r--   0        0        0      369 2024-04-19 07:38:33.825351 gigachain_experimental-0.0.59.1/langchain_experimental/prompt_injection_identifier/__init__.py
+-rw-r--r--   0        0        0     3381 2024-05-06 14:45:38.356762 gigachain_experimental-0.0.59.1/langchain_experimental/prompt_injection_identifier/hugging_face_identifier.py
+-rw-r--r--   0        0        0      174 2024-04-19 07:38:33.826287 gigachain_experimental-0.0.59.1/langchain_experimental/prompts/__init__.py
+-rw-r--r--   0        0        0       82 2024-05-06 14:45:38.357304 gigachain_experimental-0.0.59.1/langchain_experimental/prompts/load.py
+-rw-r--r--   0        0        0        0 2023-08-22 08:04:55.368181 gigachain_experimental-0.0.59.1/langchain_experimental/py.typed
+-rw-r--r--   0        0        0     1285 2023-08-24 07:36:02.836411 gigachain_experimental-0.0.59.1/langchain_experimental/pydantic_v1/__init__.py
+-rw-r--r--   0        0        0      548 2023-08-24 07:36:02.836900 gigachain_experimental-0.0.59.1/langchain_experimental/pydantic_v1/dataclasses.py
+-rw-r--r--   0        0        0      520 2023-08-24 07:36:02.837404 gigachain_experimental-0.0.59.1/langchain_experimental/pydantic_v1/main.py
+-rw-r--r--   0        0        0      518 2024-04-19 07:38:33.827066 gigachain_experimental-0.0.59.1/langchain_experimental/recommenders/__init__.py
+-rw-r--r--   0        0        0     7967 2024-04-19 07:38:33.827709 gigachain_experimental-0.0.59.1/langchain_experimental/recommenders/amazon_personalize.py
+-rw-r--r--   0        0        0     6974 2024-05-06 14:45:38.359152 gigachain_experimental-0.0.59.1/langchain_experimental/recommenders/amazon_personalize_chain.py
+-rw-r--r--   0        0        0      200 2024-04-19 07:38:33.829182 gigachain_experimental-0.0.59.1/langchain_experimental/retrievers/__init__.py
+-rw-r--r--   0        0        0     1253 2024-04-19 07:38:33.829861 gigachain_experimental-0.0.59.1/langchain_experimental/retrievers/vector_sql_database.py
+-rw-r--r--   0        0        0     1447 2024-04-19 07:38:33.830696 gigachain_experimental-0.0.59.1/langchain_experimental/rl_chain/__init__.py
+-rw-r--r--   0        0        0    23251 2024-05-06 14:45:38.359748 gigachain_experimental-0.0.59.1/langchain_experimental/rl_chain/base.py
+-rw-r--r--   0        0        0     1989 2024-03-28 12:44:20.456634 gigachain_experimental-0.0.59.1/langchain_experimental/rl_chain/metrics.py
+-rw-r--r--   0        0        0     2126 2024-03-28 12:44:20.457637 gigachain_experimental-0.0.59.1/langchain_experimental/rl_chain/model_repository.py
+-rw-r--r--   0        0        0    16289 2024-05-06 14:45:38.360601 gigachain_experimental-0.0.59.1/langchain_experimental/rl_chain/pick_best_chain.py
+-rw-r--r--   0        0        0      556 2024-03-28 12:44:20.459800 gigachain_experimental-0.0.59.1/langchain_experimental/rl_chain/vw_logger.py
+-rw-r--r--   0        0        0      946 2024-04-19 07:38:33.832517 gigachain_experimental-0.0.59.1/langchain_experimental/smart_llm/__init__.py
+-rw-r--r--   0        0        0    14438 2024-05-06 14:45:38.362010 gigachain_experimental-0.0.59.1/langchain_experimental/smart_llm/base.py
+-rw-r--r--   0        0        0      202 2024-04-19 07:38:33.834385 gigachain_experimental-0.0.59.1/langchain_experimental/sql/__init__.py
+-rw-r--r--   0        0        0    13257 2024-05-06 14:45:38.362879 gigachain_experimental-0.0.59.1/langchain_experimental/sql/base.py
+-rw-r--r--   0        0        0     4663 2024-05-06 14:45:38.363512 gigachain_experimental-0.0.59.1/langchain_experimental/sql/prompt.py
+-rw-r--r--   0        0        0     9856 2024-05-06 14:45:38.364173 gigachain_experimental-0.0.59.1/langchain_experimental/sql/vector_sql.py
+-rw-r--r--   0        0        0     1576 2024-04-19 07:38:33.836627 gigachain_experimental-0.0.59.1/langchain_experimental/synthetic_data/__init__.py
+-rw-r--r--   0        0        0      464 2024-05-06 14:45:38.364970 gigachain_experimental-0.0.59.1/langchain_experimental/synthetic_data/prompts.py
+-rw-r--r--   0        0        0       75 2024-04-19 07:38:33.837144 gigachain_experimental-0.0.59.1/langchain_experimental/tabular_synthetic_data/__init__.py
+-rw-r--r--   0        0        0     5346 2024-05-06 14:45:38.365645 gigachain_experimental-0.0.59.1/langchain_experimental/tabular_synthetic_data/base.py
+-rw-r--r--   0        0        0     2523 2024-04-19 07:38:33.837650 gigachain_experimental-0.0.59.1/langchain_experimental/tabular_synthetic_data/openai.py
+-rw-r--r--   0        0        0      417 2024-05-06 14:45:38.366178 gigachain_experimental-0.0.59.1/langchain_experimental/tabular_synthetic_data/prompts.py
+-rw-r--r--   0        0        0     9850 2024-05-06 14:45:38.366807 gigachain_experimental-0.0.59.1/langchain_experimental/text_splitter.py
+-rw-r--r--   0        0        0      180 2024-04-19 07:38:33.839237 gigachain_experimental-0.0.59.1/langchain_experimental/tools/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-03 09:19:02.773171 gigachain_experimental-0.0.59.1/langchain_experimental/tools/gigapython/__init__.py
+-rw-r--r--   0        0        0     2482 2024-06-03 09:19:02.773588 gigachain_experimental-0.0.59.1/langchain_experimental/tools/gigapython/tools.py
+-rw-r--r--   0        0        0        0 2023-10-19 12:57:52.604149 gigachain_experimental-0.0.59.1/langchain_experimental/tools/python/__init__.py
+-rw-r--r--   0        0        0     4768 2024-04-19 07:38:33.840630 gigachain_experimental-0.0.59.1/langchain_experimental/tools/python/tool.py
+-rw-r--r--   0        0        0      425 2024-04-19 07:38:33.841264 gigachain_experimental-0.0.59.1/langchain_experimental/tot/__init__.py
+-rw-r--r--   0        0        0     4858 2024-04-19 07:38:33.842457 gigachain_experimental-0.0.59.1/langchain_experimental/tot/base.py
+-rw-r--r--   0        0        0     1410 2024-04-19 07:38:33.843054 gigachain_experimental-0.0.59.1/langchain_experimental/tot/checker.py
+-rw-r--r--   0        0        0     1666 2023-08-21 13:51:28.515184 gigachain_experimental-0.0.59.1/langchain_experimental/tot/controller.py
+-rw-r--r--   0        0        0     1467 2024-03-28 12:44:20.474461 gigachain_experimental-0.0.59.1/langchain_experimental/tot/memory.py
+-rw-r--r--   0        0        0     4797 2024-04-19 07:38:33.843690 gigachain_experimental-0.0.59.1/langchain_experimental/tot/prompts.py
+-rw-r--r--   0        0        0      504 2024-03-28 12:44:20.475874 gigachain_experimental-0.0.59.1/langchain_experimental/tot/thought.py
+-rw-r--r--   0        0        0     3123 2024-05-06 14:45:38.367342 gigachain_experimental-0.0.59.1/langchain_experimental/tot/thought_generation.py
+-rw-r--r--   0        0        0      237 2024-06-03 09:19:02.774119 gigachain_experimental-0.0.59.1/langchain_experimental/utilities/__init__.py
+-rw-r--r--   0        0        0     3399 2024-06-03 09:19:02.774483 gigachain_experimental-0.0.59.1/langchain_experimental/utilities/gigapython.py
+-rw-r--r--   0        0        0     2690 2024-05-06 14:45:38.367934 gigachain_experimental-0.0.59.1/langchain_experimental/utilities/python.py
+-rw-r--r--   0        0        0      114 2024-04-19 07:38:33.844644 gigachain_experimental-0.0.59.1/langchain_experimental/video_captioning/__init__.py
+-rw-r--r--   0        0        0     5034 2024-04-19 07:38:33.845065 gigachain_experimental-0.0.59.1/langchain_experimental/video_captioning/base.py
+-rw-r--r--   0        0        0     4880 2024-04-19 07:38:33.845525 gigachain_experimental-0.0.59.1/langchain_experimental/video_captioning/models.py
+-rw-r--r--   0        0        0     4369 2024-04-19 07:38:33.845977 gigachain_experimental-0.0.59.1/langchain_experimental/video_captioning/prompts.py
+-rw-r--r--   0        0        0     3196 2024-04-19 07:38:33.846553 gigachain_experimental-0.0.59.1/langchain_experimental/video_captioning/services/audio_service.py
+-rw-r--r--   0        0        0    11301 2024-04-19 07:38:33.847251 gigachain_experimental-0.0.59.1/langchain_experimental/video_captioning/services/caption_service.py
+-rw-r--r--   0        0        0     4932 2024-04-19 07:38:33.848536 gigachain_experimental-0.0.59.1/langchain_experimental/video_captioning/services/combine_service.py
+-rw-r--r--   0        0        0     3773 2024-04-19 07:38:33.848986 gigachain_experimental-0.0.59.1/langchain_experimental/video_captioning/services/image_service.py
+-rw-r--r--   0        0        0      459 2024-04-19 07:38:33.849333 gigachain_experimental-0.0.59.1/langchain_experimental/video_captioning/services/srt_service.py
+-rw-r--r--   0        0        0     4067 2024-06-03 09:21:58.779704 gigachain_experimental-0.0.59.1/pyproject.toml
+-rw-r--r--   0        0        0     2078 1970-01-01 00:00:00.000000 gigachain_experimental-0.0.59.1/PKG-INFO
```

### Comparing `gigachain_experimental-0.0.59/LICENSE` & `gigachain_experimental-0.0.59.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/README.md` & `gigachain_experimental-0.0.59.1/README.md`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/agents/__init__.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/__init__.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/agents/agent_toolkits/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/csv/base.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/agents/agent_toolkits/csv/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/pandas/base.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/agents/agent_toolkits/pandas/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/pandas/prompt.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/agents/agent_toolkits/pandas/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/python/base.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/agents/agent_toolkits/python/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/python/prompt.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/agents/agent_toolkits/python/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/spark/base.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/agents/agent_toolkits/spark/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/xorbits/base.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/agents/agent_toolkits/xorbits/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/xorbits/prompt.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/agents/agent_toolkits/xorbits/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/__init__.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/autonomous_agents/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/autogpt/agent.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/autonomous_agents/autogpt/agent.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/autogpt/memory.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/autonomous_agents/autogpt/memory.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/autogpt/output_parser.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/autonomous_agents/autogpt/output_parser.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/autogpt/prompt.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/autonomous_agents/autogpt/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/autogpt/prompt_generator.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/autonomous_agents/autogpt/prompt_generator.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/baby_agi/__init__.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/autonomous_agents/baby_agi/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/baby_agi/baby_agi.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/autonomous_agents/baby_agi/baby_agi.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/baby_agi/task_creation.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/autonomous_agents/baby_agi/task_creation.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/baby_agi/task_execution.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/autonomous_agents/baby_agi/task_execution.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/baby_agi/task_prioritization.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/autonomous_agents/baby_agi/task_prioritization.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/hugginggpt/hugginggpt.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/autonomous_agents/hugginggpt/hugginggpt.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/hugginggpt/repsonse_generator.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/autonomous_agents/hugginggpt/repsonse_generator.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/hugginggpt/task_executor.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/autonomous_agents/hugginggpt/task_executor.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/hugginggpt/task_planner.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/autonomous_agents/hugginggpt/task_planner.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/chat_models/__init__.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/chat_models/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/chat_models/llm_wrapper.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/chat_models/llm_wrapper.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/__init__.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/comprehend_moderation/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/amazon_comprehend_moderation.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/comprehend_moderation/amazon_comprehend_moderation.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/base_moderation.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/comprehend_moderation/base_moderation.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/base_moderation_callbacks.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/comprehend_moderation/base_moderation_callbacks.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/base_moderation_config.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/comprehend_moderation/base_moderation_config.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/base_moderation_exceptions.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/comprehend_moderation/base_moderation_exceptions.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/pii.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/comprehend_moderation/pii.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/prompt_safety.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/comprehend_moderation/prompt_safety.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/toxicity.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/comprehend_moderation/toxicity.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/cpal/__init__.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/cpal/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/cpal/base.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/cpal/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/cpal/models.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/cpal/models.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/cpal/templates/univariate/causal.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/cpal/templates/univariate/causal.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/cpal/templates/univariate/intervention.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/cpal/templates/univariate/intervention.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/cpal/templates/univariate/narrative.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/cpal/templates/univariate/narrative.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/cpal/templates/univariate/query.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/cpal/templates/univariate/query.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/data_anonymizer/__init__.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/data_anonymizer/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/data_anonymizer/base.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/data_anonymizer/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/data_anonymizer/deanonymizer_mapping.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/data_anonymizer/deanonymizer_mapping.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/data_anonymizer/deanonymizer_matching_strategies.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/data_anonymizer/deanonymizer_matching_strategies.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/data_anonymizer/faker_presidio_mapping.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/data_anonymizer/faker_presidio_mapping.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/data_anonymizer/presidio.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/data_anonymizer/presidio.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/generative_agents/generative_agent.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/generative_agents/generative_agent.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/generative_agents/memory.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/generative_agents/memory.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/graph_transformers/diffbot.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/graph_transformers/diffbot.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/graph_transformers/llm.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/graph_transformers/llm.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/llm_bash/base.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/llm_bash/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/llm_bash/bash.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/llm_bash/bash.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/llm_bash/prompt.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/llm_bash/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/llm_symbolic_math/base.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/llm_symbolic_math/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/llm_symbolic_math/prompt.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/llm_symbolic_math/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/llms/anthropic_functions.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/llms/anthropic_functions.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/llms/jsonformer_decoder.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/llms/jsonformer_decoder.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/llms/llamaapi.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/llms/llamaapi.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/llms/lmformatenforcer_decoder.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/llms/lmformatenforcer_decoder.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/llms/ollama_functions.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/llms/ollama_functions.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/llms/rellm_decoder.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/llms/rellm_decoder.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/open_clip/open_clip.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/open_clip/open_clip.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/pal_chain/base.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/pal_chain/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/pal_chain/colored_object_prompt.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/pal_chain/colored_object_prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/pal_chain/math_prompt.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/pal_chain/math_prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/plan_and_execute/agent_executor.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/plan_and_execute/agent_executor.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/plan_and_execute/executors/agent_executor.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/plan_and_execute/executors/agent_executor.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/plan_and_execute/executors/base.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/plan_and_execute/executors/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/plan_and_execute/planners/base.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/plan_and_execute/planners/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/plan_and_execute/planners/chat_planner.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/plan_and_execute/planners/chat_planner.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/plan_and_execute/schema.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/plan_and_execute/schema.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/prompt_injection_identifier/hugging_face_identifier.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/prompt_injection_identifier/hugging_face_identifier.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/pydantic_v1/__init__.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/pydantic_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/pydantic_v1/dataclasses.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/pydantic_v1/dataclasses.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/pydantic_v1/main.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/pydantic_v1/main.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/recommenders/__init__.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/recommenders/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/recommenders/amazon_personalize.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/recommenders/amazon_personalize.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/recommenders/amazon_personalize_chain.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/recommenders/amazon_personalize_chain.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/retrievers/vector_sql_database.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/retrievers/vector_sql_database.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/rl_chain/__init__.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/rl_chain/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/rl_chain/base.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/rl_chain/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/rl_chain/metrics.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/rl_chain/metrics.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/rl_chain/model_repository.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/rl_chain/model_repository.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/rl_chain/pick_best_chain.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/rl_chain/pick_best_chain.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/rl_chain/vw_logger.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/rl_chain/vw_logger.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/smart_llm/__init__.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/smart_llm/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/smart_llm/base.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/smart_llm/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/sql/base.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/sql/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/sql/prompt.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/sql/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/sql/vector_sql.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/sql/vector_sql.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/synthetic_data/__init__.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/synthetic_data/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/tabular_synthetic_data/base.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/tabular_synthetic_data/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/tabular_synthetic_data/openai.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/tabular_synthetic_data/openai.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/text_splitter.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/text_splitter.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/tools/python/tool.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/tools/python/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/tot/base.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/tot/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/tot/checker.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/tot/checker.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/tot/controller.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/tot/controller.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/tot/memory.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/tot/memory.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/tot/prompts.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/tot/prompts.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/tot/thought_generation.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/tot/thought_generation.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/utilities/python.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/utilities/python.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/video_captioning/base.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/video_captioning/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/video_captioning/models.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/video_captioning/models.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/video_captioning/prompts.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/video_captioning/prompts.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/video_captioning/services/audio_service.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/video_captioning/services/audio_service.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/video_captioning/services/caption_service.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/video_captioning/services/caption_service.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/video_captioning/services/combine_service.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/video_captioning/services/combine_service.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/langchain_experimental/video_captioning/services/image_service.py` & `gigachain_experimental-0.0.59.1/langchain_experimental/video_captioning/services/image_service.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.59/pyproject.toml` & `gigachain_experimental-0.0.59.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gigachain-experimental"
-version = "0.0.59"
+version = "0.0.59.1"
 description = "Building applications with LLMs through composability"
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ai-forever/gigachain"
 packages = [
     {include = "langchain_experimental"}
```

### Comparing `gigachain_experimental-0.0.59/PKG-INFO` & `gigachain_experimental-0.0.59.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigachain-experimental
-Version: 0.0.59
+Version: 0.0.59.1
 Summary: Building applications with LLMs through composability
 Home-page: https://github.com/ai-forever/gigachain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

