# Comparing `tmp/logfire-0.38.0.tar.gz` & `tmp/logfire-0.39.0.tar.gz`

## Comparing `logfire-0.38.0.tar` & `logfire-0.39.0.tar`

### file list

```diff
@@ -1,130 +1,139 @@
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 logfire-0.38.0/Makefile
--rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/__main__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/cli.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/exceptions.py
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/propagate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/py.typed
--rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/testing.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/version.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/__init__.py
--rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/ast_utils.py
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/async_.py
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/auth.py
--rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/backfill.py
--rw-r--r--   0        0        0    18512 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/cli.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/collect_system_info.py
--rw-r--r--   0        0        0    56682 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/config.py
--rw-r--r--   0        0        0    11225 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/config_params.py
--rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/constants.py
--rw-r--r--   0        0        0    19127 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/formatter.py
--rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/instrument.py
--rw-r--r--   0        0        0     9035 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/json_encoder.py
--rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/json_formatter.py
--rw-r--r--   0        0        0    13081 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/json_schema.py
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/json_types.py
--rw-r--r--   0        0        0    64101 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/main.py
--rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/metrics.py
--rw-r--r--   0        0        0     8756 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/scrubbing.py
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/stack_info.py
--rw-r--r--   0        0        0    10602 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/tracer.py
--rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/utils.py
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/auto_trace/__init__.py
--rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/auto_trace/import_hook.py
--rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/auto_trace/rewrite_ast.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/auto_trace/types.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/exporters/__init__.py
--rw-r--r--   0        0        0    18968 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/exporters/console.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/exporters/fallback.py
--rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/exporters/file.py
--rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/exporters/otlp.py
--rw-r--r--   0        0        0     8977 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/exporters/processor_wrapper.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/exporters/remove_pending.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/exporters/wrapper.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/integrations/__init__.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/integrations/asyncpg.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/integrations/django.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/integrations/executors.py
--rw-r--r--   0        0        0    10656 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/integrations/fastapi.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/integrations/httpx.py
--rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/integrations/psycopg.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/integrations/requests.py
--rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/integrations/llm_providers/anthropic.py
--rw-r--r--   0        0        0     7683 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/integrations/llm_providers/llm_provider.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/integrations/llm_providers/openai.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/integrations/llm_providers/types.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/integrations/__init__.py
--rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/integrations/logging.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/integrations/loguru.py
--rw-r--r--   0        0        0    19169 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/integrations/pydantic.py
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/integrations/structlog.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/__init__.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/conftest.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/module_used_for_tests.py
--rw-r--r--   0        0        0    19034 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_auto_trace.py
--rw-r--r--   0        0        0     9988 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_backfill.py
--rw-r--r--   0        0        0    47077 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_cli.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_collect_package_resources.py
--rw-r--r--   0        0        0    53700 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_configure.py
--rw-r--r--   0        0        0    29388 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_console_exporter.py
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_formatter.py
--rw-r--r--   0        0        0    45893 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_json_args.py
--rw-r--r--   0        0        0    19936 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_json_args_formatting.py
--rw-r--r--   0        0        0   108461 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_logfire.py
--rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_loguru.py
--rw-r--r--   0        0        0    11324 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_metrics.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_no_production.py
--rw-r--r--   0        0        0    54162 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_pydantic_plugin.py
--rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_sampling.py
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_secret_scrubbing.py
--rw-r--r--   0        0        0     7270 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_slow_async_callbacks.py
--rw-r--r--   0        0        0     8126 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_source_code_extraction.py
--rw-r--r--   0        0        0    12433 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_stdlib_logging.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_structlog.py
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_testing.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_utils.py
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/auto_trace_samples/__init__.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/auto_trace_samples/foo.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/auto_trace_samples/simple_nesting.py
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/exporters/test_fallback_exporter.py
--rw-r--r--   0        0        0     8384 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/exporters/test_file_exporter.py
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/exporters/test_otlp_session.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/exporters/test_remove_pending.py
--rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/exporters/test_retry_fewer_spans.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/import_used_for_tests/__init__.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/import_used_for_tests/slow_async_callbacks_example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/import_used_for_tests/a/__init__.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/import_used_for_tests/a/b.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/__init__.py
--rw-r--r--   0        0        0    24476 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/test_anthropic.py
--rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/test_asgi.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/test_asyncpg.py
--rw-r--r--   0        0        0     4769 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/test_django.py
--rw-r--r--   0        0        0    44449 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/test_fastapi.py
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/test_flask.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/test_httpx.py
--rw-r--r--   0        0        0    44244 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/test_openai.py
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/test_psycopg.py
--rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/test_requests.py
--rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/test_sqlalchemy.py
--rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/test_starlette.py
--rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/test_wsgi.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/django_test_project/__init__.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/django_test_project/manage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/django_test_project/django_test_app/__init__.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/django_test_project/django_test_app/admin.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/django_test_project/django_test_app/apps.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/django_test_project/django_test_app/models.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/django_test_project/django_test_app/urls.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/django_test_project/django_test_app/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/django_test_project/django_test_app/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/django_test_project/django_test_site/__init__.py
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/django_test_project/django_test_site/settings.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/django_test_project/django_test_site/urls.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/django_test_project/django_test_site/wsgi.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 logfire-0.38.0/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 logfire-0.38.0/LICENSE
--rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 logfire-0.38.0/README.md
--rw-r--r--   0        0        0     8521 2020-02-02 00:00:00.000000 logfire-0.38.0/pyproject.toml
--rw-r--r--   0        0        0     7731 2020-02-02 00:00:00.000000 logfire-0.38.0/PKG-INFO
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 logfire-0.39.0/Makefile
+-rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/__main__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/cli.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/exceptions.py
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/propagate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/py.typed
+-rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/testing.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/version.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/__init__.py
+-rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/ast_utils.py
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/async_.py
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/auth.py
+-rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/backfill.py
+-rw-r--r--   0        0        0    18512 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/cli.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/collect_system_info.py
+-rw-r--r--   0        0        0    56682 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/config.py
+-rw-r--r--   0        0        0    11225 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/config_params.py
+-rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/constants.py
+-rw-r--r--   0        0        0    19127 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/formatter.py
+-rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/instrument.py
+-rw-r--r--   0        0        0     9035 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/json_encoder.py
+-rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/json_formatter.py
+-rw-r--r--   0        0        0    13081 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/json_schema.py
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/json_types.py
+-rw-r--r--   0        0        0    67837 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/main.py
+-rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/metrics.py
+-rw-r--r--   0        0        0     8756 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/scrubbing.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/stack_info.py
+-rw-r--r--   0        0        0    10602 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/tracer.py
+-rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/utils.py
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/auto_trace/__init__.py
+-rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/auto_trace/import_hook.py
+-rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/auto_trace/rewrite_ast.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/auto_trace/types.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/exporters/__init__.py
+-rw-r--r--   0        0        0    18968 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/exporters/console.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/exporters/fallback.py
+-rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/exporters/file.py
+-rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/exporters/otlp.py
+-rw-r--r--   0        0        0     8977 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/exporters/processor_wrapper.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/exporters/remove_pending.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/exporters/wrapper.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/integrations/__init__.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/integrations/aiohttp_client.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/integrations/asyncpg.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/integrations/django.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/integrations/executors.py
+-rw-r--r--   0        0        0    10656 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/integrations/fastapi.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/integrations/flask.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/integrations/httpx.py
+-rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/integrations/psycopg.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/integrations/pymongo.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/integrations/redis.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/integrations/requests.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/integrations/sqlalchemy.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/integrations/starlette.py
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/integrations/llm_providers/anthropic.py
+-rw-r--r--   0        0        0     7683 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/integrations/llm_providers/llm_provider.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/integrations/llm_providers/openai.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/_internal/integrations/llm_providers/types.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/integrations/__init__.py
+-rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/integrations/logging.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/integrations/loguru.py
+-rw-r--r--   0        0        0    19169 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/integrations/pydantic.py
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 logfire-0.39.0/logfire/integrations/structlog.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/__init__.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/conftest.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/module_used_for_tests.py
+-rw-r--r--   0        0        0    19034 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/test_auto_trace.py
+-rw-r--r--   0        0        0     9988 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/test_backfill.py
+-rw-r--r--   0        0        0    47077 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/test_cli.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/test_collect_package_resources.py
+-rw-r--r--   0        0        0    53700 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/test_configure.py
+-rw-r--r--   0        0        0    29388 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/test_console_exporter.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/test_formatter.py
+-rw-r--r--   0        0        0    45893 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/test_json_args.py
+-rw-r--r--   0        0        0    19936 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/test_json_args_formatting.py
+-rw-r--r--   0        0        0   108461 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/test_logfire.py
+-rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/test_loguru.py
+-rw-r--r--   0        0        0    11324 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/test_metrics.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/test_no_production.py
+-rw-r--r--   0        0        0    54162 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/test_pydantic_plugin.py
+-rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/test_sampling.py
+-rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/test_secret_scrubbing.py
+-rw-r--r--   0        0        0     7270 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/test_slow_async_callbacks.py
+-rw-r--r--   0        0        0     8126 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/test_source_code_extraction.py
+-rw-r--r--   0        0        0    12433 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/test_stdlib_logging.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/test_structlog.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/test_testing.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/test_utils.py
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/auto_trace_samples/__init__.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/auto_trace_samples/foo.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/auto_trace_samples/simple_nesting.py
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/exporters/test_fallback_exporter.py
+-rw-r--r--   0        0        0     8384 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/exporters/test_file_exporter.py
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/exporters/test_otlp_session.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/exporters/test_remove_pending.py
+-rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/exporters/test_retry_fewer_spans.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/import_used_for_tests/__init__.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/import_used_for_tests/slow_async_callbacks_example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/import_used_for_tests/a/__init__.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/import_used_for_tests/a/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/otel_integrations/__init__.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/otel_integrations/test_aiohttp_client.py
+-rw-r--r--   0        0        0    24476 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/otel_integrations/test_anthropic.py
+-rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/otel_integrations/test_asgi.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/otel_integrations/test_asyncpg.py
+-rw-r--r--   0        0        0     4769 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/otel_integrations/test_django.py
+-rw-r--r--   0        0        0    44449 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/otel_integrations/test_fastapi.py
+-rw-r--r--   0        0        0     5187 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/otel_integrations/test_flask.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/otel_integrations/test_httpx.py
+-rw-r--r--   0        0        0    44244 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/otel_integrations/test_openai.py
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/otel_integrations/test_psycopg.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/otel_integrations/test_pymongo.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/otel_integrations/test_redis.py
+-rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/otel_integrations/test_requests.py
+-rw-r--r--   0        0        0     7883 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/otel_integrations/test_sqlalchemy.py
+-rw-r--r--   0        0        0     7389 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/otel_integrations/test_starlette.py
+-rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/otel_integrations/test_wsgi.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/otel_integrations/django_test_project/__init__.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/otel_integrations/django_test_project/manage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/otel_integrations/django_test_project/django_test_app/__init__.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/otel_integrations/django_test_project/django_test_app/admin.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/otel_integrations/django_test_project/django_test_app/apps.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/otel_integrations/django_test_project/django_test_app/models.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/otel_integrations/django_test_project/django_test_app/urls.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/otel_integrations/django_test_project/django_test_app/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/otel_integrations/django_test_project/django_test_app/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/otel_integrations/django_test_project/django_test_site/__init__.py
+-rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/otel_integrations/django_test_project/django_test_site/settings.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/otel_integrations/django_test_project/django_test_site/urls.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 logfire-0.39.0/tests/otel_integrations/django_test_project/django_test_site/wsgi.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 logfire-0.39.0/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 logfire-0.39.0/LICENSE
+-rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 logfire-0.39.0/README.md
+-rw-r--r--   0        0        0     8652 2020-02-02 00:00:00.000000 logfire-0.39.0/pyproject.toml
+-rw-r--r--   0        0        0     7731 2020-02-02 00:00:00.000000 logfire-0.39.0/PKG-INFO
```

### Comparing `logfire-0.38.0/Makefile` & `logfire-0.39.0/Makefile`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/__init__.py` & `logfire-0.39.0/logfire/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -31,14 +31,20 @@
 instrument_openai = DEFAULT_LOGFIRE_INSTANCE.instrument_openai
 instrument_anthropic = DEFAULT_LOGFIRE_INSTANCE.instrument_anthropic
 instrument_asyncpg = DEFAULT_LOGFIRE_INSTANCE.instrument_asyncpg
 instrument_httpx = DEFAULT_LOGFIRE_INSTANCE.instrument_httpx
 instrument_requests = DEFAULT_LOGFIRE_INSTANCE.instrument_requests
 instrument_psycopg = DEFAULT_LOGFIRE_INSTANCE.instrument_psycopg
 instrument_django = DEFAULT_LOGFIRE_INSTANCE.instrument_django
+instrument_flask = DEFAULT_LOGFIRE_INSTANCE.instrument_flask
+instrument_starlette = DEFAULT_LOGFIRE_INSTANCE.instrument_starlette
+instrument_aiohttp_client = DEFAULT_LOGFIRE_INSTANCE.instrument_aiohttp_client
+instrument_sqlalchemy = DEFAULT_LOGFIRE_INSTANCE.instrument_sqlalchemy
+instrument_redis = DEFAULT_LOGFIRE_INSTANCE.instrument_redis
+instrument_pymongo = DEFAULT_LOGFIRE_INSTANCE.instrument_pymongo
 shutdown = DEFAULT_LOGFIRE_INSTANCE.shutdown
 with_tags = DEFAULT_LOGFIRE_INSTANCE.with_tags
 # with_trace_sample_rate = DEFAULT_LOGFIRE_INSTANCE.with_trace_sample_rate
 with_settings = DEFAULT_LOGFIRE_INSTANCE.with_settings
 
 # Logging
 log = DEFAULT_LOGFIRE_INSTANCE.log
```

### Comparing `logfire-0.38.0/logfire/propagate.py` & `logfire-0.39.0/logfire/propagate.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/testing.py` & `logfire-0.39.0/logfire/testing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/ast_utils.py` & `logfire-0.39.0/logfire/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/async_.py` & `logfire-0.39.0/logfire/_internal/async_.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/auth.py` & `logfire-0.39.0/logfire/_internal/auth.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/backfill.py` & `logfire-0.39.0/logfire/_internal/backfill.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/cli.py` & `logfire-0.39.0/logfire/_internal/cli.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/config.py` & `logfire-0.39.0/logfire/_internal/config.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/config_params.py` & `logfire-0.39.0/logfire/_internal/config_params.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/constants.py` & `logfire-0.39.0/logfire/_internal/constants.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/formatter.py` & `logfire-0.39.0/logfire/_internal/formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/instrument.py` & `logfire-0.39.0/logfire/_internal/instrument.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/json_encoder.py` & `logfire-0.39.0/logfire/_internal/json_encoder.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/json_formatter.py` & `logfire-0.39.0/logfire/_internal/json_formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/json_schema.py` & `logfire-0.39.0/logfire/_internal/json_schema.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/json_types.py` & `logfire-0.39.0/logfire/_internal/json_types.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/main.py` & `logfire-0.39.0/logfire/_internal/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,15 +64,17 @@
 from .utils import uniquify_sequence
 
 if TYPE_CHECKING:
     import anthropic
     import openai
     from django.http import HttpRequest, HttpResponse
     from fastapi import FastAPI
+    from flask.app import Flask
     from opentelemetry.metrics import _Gauge as Gauge
+    from starlette.applications import Starlette
     from starlette.requests import Request
     from starlette.websockets import WebSocket
 
 
 try:
     from pydantic import ValidationError
 except ImportError:  # pragma: no cover
@@ -1111,14 +1113,86 @@
                 particularly `enable_commenter` and `commenter_options`.
         """
         from .integrations.psycopg import instrument_psycopg
 
         self._warn_if_not_initialized_for_instrumentation()
         return instrument_psycopg(conn_or_module, **kwargs)
 
+    def instrument_flask(self, app: Flask, **kwargs: Any):
+        """Instrument `app` so that spans are automatically created for each request.
+
+        Uses the
+        [OpenTelemetry Flask Instrumentation](https://opentelemetry-python-contrib.readthedocs.io/en/latest/instrumentation/flask/flask.html)
+        library, specifically `FlaskInstrumentor().instrument_app()`, to which it passes `**kwargs`.
+        """
+        from .integrations.flask import instrument_flask
+
+        self._warn_if_not_initialized_for_instrumentation()
+        return instrument_flask(app, **kwargs)
+
+    def instrument_starlette(self, app: Starlette, **kwargs: Any):
+        """Instrument `app` so that spans are automatically created for each request.
+
+        Uses the
+        [OpenTelemetry Starlette Instrumentation](https://opentelemetry-python-contrib.readthedocs.io/en/latest/instrumentation/starlette/starlette.html)
+        library, specifically `StarletteInstrumentor.instrument_app()`, to which it passes `**kwargs`.
+        """
+        from .integrations.starlette import instrument_starlette
+
+        self._warn_if_not_initialized_for_instrumentation()
+        return instrument_starlette(app, **kwargs)
+
+    def instrument_aiohttp_client(self, **kwargs: Any):
+        """Instrument the `aiohttp` module so that spans are automatically created for each client request.
+
+        Uses the
+        [OpenTelemetry aiohttp client Instrumentation](https://opentelemetry-python-contrib.readthedocs.io/en/latest/instrumentation/aiohttp_client/aiohttp_client.html)
+        library, specifically `AioHttpClientInstrumentor().instrument()`, to which it passes `**kwargs`.
+        """
+        from .integrations.aiohttp_client import instrument_aiohttp_client
+
+        self._warn_if_not_initialized_for_instrumentation()
+        return instrument_aiohttp_client(**kwargs)
+
+    def instrument_sqlalchemy(self, **kwargs: Any):
+        """Instrument the `sqlalchemy` module so that spans are automatically created for each query.
+
+        Uses the
+        [OpenTelemetry SQLAlchemy Instrumentation](https://opentelemetry-python-contrib.readthedocs.io/en/latest/instrumentation/sqlalchemy/sqlalchemy.html)
+        library, specifically `SQLAlchemyInstrumentor().instrument()`, to which it passes `**kwargs`.
+        """
+        from .integrations.sqlalchemy import instrument_sqlalchemy
+
+        self._warn_if_not_initialized_for_instrumentation()
+        return instrument_sqlalchemy(**kwargs)
+
+    def instrument_pymongo(self, **kwargs: Any):
+        """Instrument the `pymongo` module so that spans are automatically created for each operation.
+
+        Uses the
+        [OpenTelemetry pymongo Instrumentation](https://opentelemetry-python-contrib.readthedocs.io/en/latest/instrumentation/pymongo/pymongo.html)
+            library, specifically `PymongoInstrumentor().instrument()`, to which it passes `**kwargs`.
+        """
+        from .integrations.pymongo import instrument_pymongo
+
+        self._warn_if_not_initialized_for_instrumentation()
+        return instrument_pymongo(**kwargs)
+
+    def instrument_redis(self, **kwargs: Any):
+        """Instrument the `redis` module so that spans are automatically created for each operation.
+
+        Uses the
+        [OpenTelemetry Redis Instrumentation](https://opentelemetry-python-contrib.readthedocs.io/en/latest/instrumentation/redis/redis.html)
+        library, specifically `RedisInstrumentor().instrument()`, to which it passes `**kwargs`.
+        """
+        from .integrations.redis import instrument_redis
+
+        self._warn_if_not_initialized_for_instrumentation()
+        return instrument_redis(**kwargs)
+
     def metric_counter(self, name: str, *, unit: str = '', description: str = '') -> Counter:
         """Create a counter metric.
 
         A counter is a cumulative metric that represents a single numerical value that only ever goes up.
 
         ```py
         import logfire
```

### Comparing `logfire-0.38.0/logfire/_internal/metrics.py` & `logfire-0.39.0/logfire/_internal/metrics.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/scrubbing.py` & `logfire-0.39.0/logfire/_internal/scrubbing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/stack_info.py` & `logfire-0.39.0/logfire/_internal/stack_info.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/tracer.py` & `logfire-0.39.0/logfire/_internal/tracer.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/utils.py` & `logfire-0.39.0/logfire/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/auto_trace/__init__.py` & `logfire-0.39.0/logfire/_internal/auto_trace/__init__.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/auto_trace/import_hook.py` & `logfire-0.39.0/logfire/_internal/auto_trace/import_hook.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/auto_trace/rewrite_ast.py` & `logfire-0.39.0/logfire/_internal/auto_trace/rewrite_ast.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/auto_trace/types.py` & `logfire-0.39.0/logfire/_internal/auto_trace/types.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/exporters/console.py` & `logfire-0.39.0/logfire/_internal/exporters/console.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/exporters/fallback.py` & `logfire-0.39.0/logfire/_internal/exporters/fallback.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/exporters/file.py` & `logfire-0.39.0/logfire/_internal/exporters/file.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/exporters/otlp.py` & `logfire-0.39.0/logfire/_internal/exporters/otlp.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/exporters/processor_wrapper.py` & `logfire-0.39.0/logfire/_internal/exporters/processor_wrapper.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/exporters/remove_pending.py` & `logfire-0.39.0/logfire/_internal/exporters/remove_pending.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/exporters/wrapper.py` & `logfire-0.39.0/logfire/_internal/exporters/wrapper.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/integrations/executors.py` & `logfire-0.39.0/logfire/_internal/integrations/executors.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/integrations/fastapi.py` & `logfire-0.39.0/logfire/_internal/integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/integrations/psycopg.py` & `logfire-0.39.0/logfire/_internal/integrations/psycopg.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/integrations/llm_providers/anthropic.py` & `logfire-0.39.0/logfire/_internal/integrations/llm_providers/anthropic.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/integrations/llm_providers/llm_provider.py` & `logfire-0.39.0/logfire/_internal/integrations/llm_providers/llm_provider.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/_internal/integrations/llm_providers/openai.py` & `logfire-0.39.0/logfire/_internal/integrations/llm_providers/openai.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/integrations/logging.py` & `logfire-0.39.0/logfire/integrations/logging.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/integrations/loguru.py` & `logfire-0.39.0/logfire/integrations/loguru.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/integrations/pydantic.py` & `logfire-0.39.0/logfire/integrations/pydantic.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/logfire/integrations/structlog.py` & `logfire-0.39.0/logfire/integrations/structlog.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/conftest.py` & `logfire-0.39.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/test_auto_trace.py` & `logfire-0.39.0/tests/test_auto_trace.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/test_backfill.py` & `logfire-0.39.0/tests/test_backfill.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/test_cli.py` & `logfire-0.39.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/test_collect_package_resources.py` & `logfire-0.39.0/tests/test_collect_package_resources.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/test_configure.py` & `logfire-0.39.0/tests/test_configure.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/test_console_exporter.py` & `logfire-0.39.0/tests/test_console_exporter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/test_formatter.py` & `logfire-0.39.0/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/test_json_args.py` & `logfire-0.39.0/tests/test_json_args.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/test_json_args_formatting.py` & `logfire-0.39.0/tests/test_json_args_formatting.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/test_logfire.py` & `logfire-0.39.0/tests/test_logfire.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/test_loguru.py` & `logfire-0.39.0/tests/test_loguru.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/test_metrics.py` & `logfire-0.39.0/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/test_no_production.py` & `logfire-0.39.0/tests/test_no_production.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/test_pydantic_plugin.py` & `logfire-0.39.0/tests/test_pydantic_plugin.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/test_sampling.py` & `logfire-0.39.0/tests/test_sampling.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/test_secret_scrubbing.py` & `logfire-0.39.0/tests/test_secret_scrubbing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/test_slow_async_callbacks.py` & `logfire-0.39.0/tests/test_slow_async_callbacks.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/test_source_code_extraction.py` & `logfire-0.39.0/tests/test_source_code_extraction.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/test_stdlib_logging.py` & `logfire-0.39.0/tests/test_stdlib_logging.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/test_structlog.py` & `logfire-0.39.0/tests/test_structlog.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/test_testing.py` & `logfire-0.39.0/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/test_utils.py` & `logfire-0.39.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/utils.py` & `logfire-0.39.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/exporters/test_fallback_exporter.py` & `logfire-0.39.0/tests/exporters/test_fallback_exporter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/exporters/test_file_exporter.py` & `logfire-0.39.0/tests/exporters/test_file_exporter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/exporters/test_otlp_session.py` & `logfire-0.39.0/tests/exporters/test_otlp_session.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/exporters/test_remove_pending.py` & `logfire-0.39.0/tests/exporters/test_remove_pending.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/exporters/test_retry_fewer_spans.py` & `logfire-0.39.0/tests/exporters/test_retry_fewer_spans.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/import_used_for_tests/slow_async_callbacks_example.py` & `logfire-0.39.0/tests/import_used_for_tests/slow_async_callbacks_example.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/otel_integrations/test_anthropic.py` & `logfire-0.39.0/tests/otel_integrations/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/otel_integrations/test_asgi.py` & `logfire-0.39.0/tests/otel_integrations/test_asgi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/otel_integrations/test_asyncpg.py` & `logfire-0.39.0/tests/otel_integrations/test_asyncpg.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/otel_integrations/test_django.py` & `logfire-0.39.0/tests/otel_integrations/test_django.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/otel_integrations/test_fastapi.py` & `logfire-0.39.0/tests/otel_integrations/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/otel_integrations/test_flask.py` & `logfire-0.39.0/tests/otel_integrations/test_flask.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import opentelemetry.instrumentation.flask
 from flask import Flask
 from inline_snapshot import snapshot
-from opentelemetry.instrumentation.flask import FlaskInstrumentor
 from opentelemetry.propagate import inject
 from werkzeug.test import Client
 
 import logfire
 from logfire.testing import TestExporter, TimeGenerator
 
 
 def test_flask_instrumentation(exporter: TestExporter, time_generator: TimeGenerator) -> None:
     app = Flask(__name__)
-    FlaskInstrumentor().instrument_app(app)  # type: ignore
+    logfire.instrument_flask(app)
 
     @app.route('/')
     def homepage():  # type: ignore
         logfire.info('inside request handler')
         return 'middleware test'
 
     client = Client(app)
```

### Comparing `logfire-0.38.0/tests/otel_integrations/test_httpx.py` & `logfire-0.39.0/tests/otel_integrations/test_httpx.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/otel_integrations/test_openai.py` & `logfire-0.39.0/tests/otel_integrations/test_openai.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/otel_integrations/test_psycopg.py` & `logfire-0.39.0/tests/otel_integrations/test_psycopg.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/otel_integrations/test_requests.py` & `logfire-0.39.0/tests/otel_integrations/test_requests.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/otel_integrations/test_sqlalchemy.py` & `logfire-0.39.0/tests/otel_integrations/test_sqlalchemy.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from inline_snapshot import snapshot
 from sqlalchemy.engine import Engine, create_engine
 from sqlalchemy.orm import DeclarativeBase, Mapped, Session, mapped_column
 from sqlalchemy.sql import text
 from sqlalchemy.types import Integer, String
 
+import logfire
 from logfire.testing import TestExporter
 
 
 @contextmanager
 def sqlite_engine(path: Path) -> Iterator[Engine]:
     path.unlink(missing_ok=True)
     engine = create_engine(f'sqlite:///{path}')
@@ -22,15 +23,15 @@
 
 
 def test_sqlalchemy_instrumentation(exporter: TestExporter):
     with sqlite_engine(Path('example.db')) as engine:
         # Need to  ensure this import happens _after_ importing sqlalchemy
         from opentelemetry.instrumentation.sqlalchemy import SQLAlchemyInstrumentor
 
-        SQLAlchemyInstrumentor().instrument(engine=engine, enable_commenter=True, commenter_options={})  # type: ignore
+        logfire.instrument_sqlalchemy(engine=engine, enable_commenter=True, commenter_options={})
 
         class Base(DeclarativeBase):
             pass
 
         # `auth` is in default scrubbing patterns, but `db.statement` attribute is in scrubbing SAFE_KEYS.
         # So, logfire shouldn't redact `auth` in the `db.statement` attribute.
         class AuthRecord(Base):
```

### Comparing `logfire-0.38.0/tests/otel_integrations/test_starlette.py` & `logfire-0.39.0/tests/otel_integrations/test_starlette.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from inline_snapshot import snapshot
 from opentelemetry.instrumentation.starlette import StarletteInstrumentor
 from starlette.applications import Starlette
 from starlette.routing import Route, WebSocketRoute
 from starlette.testclient import TestClient
 from starlette.websockets import WebSocket
 
+import logfire
 from logfire.testing import TestExporter
 
 
 async def secret(path_param: str):
     raise ValueError('test exception')
 
 
@@ -27,15 +28,15 @@
     routes = [
         Route('/secret/{path_param}', secret),
         WebSocketRoute('/ws', websocket_endpoint),
     ]
 
     app = Starlette(routes=routes)
     try:
-        StarletteInstrumentor.instrument_app(app)  # type: ignore
+        logfire.instrument_starlette(app)
         yield app
     finally:
         StarletteInstrumentor.uninstrument_app(app)
 
 
 @pytest.fixture()
 def client(app: Starlette) -> TestClient:
```

### Comparing `logfire-0.38.0/tests/otel_integrations/test_wsgi.py` & `logfire-0.39.0/tests/otel_integrations/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/otel_integrations/django_test_project/manage.py` & `logfire-0.39.0/tests/otel_integrations/django_test_project/manage.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/tests/otel_integrations/django_test_project/django_test_site/settings.py` & `logfire-0.39.0/tests/otel_integrations/django_test_project/django_test_site/settings.py`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/LICENSE` & `logfire-0.39.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/README.md` & `logfire-0.39.0/README.md`

 * *Files identical despite different names*

### Comparing `logfire-0.38.0/pyproject.toml` & `logfire-0.39.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "logfire"
-version = "0.38.0"
+version = "0.39.0"
 description = "The best Python observability tool! 🪵🔥"
 authors = [
     { name = "Pydantic Team", email = "engineering@pydantic.dev" },
     { name = "Samuel Colvin", email = "samuel@pydantic.dev" },
     { name = "Hasan Ramezani", email = "hasan@pydantic.dev" },
     { name = "Adrian Garcia Badaracco", email = "adrian@pydantic.dev" },
     { name = "David Montague", email = "david@pydantic.dev" },
@@ -77,14 +77,17 @@
 logfire = "logfire.testing"
 
 [tool.rye]
 managed = true
 dev-dependencies = [
     "anyio",
     "httpx",
+    "aiohttp",
+    "redis",
+    "pymongo",
     "starlette",
     "fastapi",
     "Flask",
     "django",
     "dirty-equals",
     "pytest",
     "pytest-django",
@@ -105,14 +108,16 @@
     "opentelemetry-instrumentation-httpx",
     "opentelemetry-instrumentation-requests",
     "opentelemetry-instrumentation-sqlalchemy",
     "opentelemetry-instrumentation-system-metrics",
     "opentelemetry-instrumentation-asyncpg",
     "opentelemetry-instrumentation-psycopg",
     "opentelemetry-instrumentation-psycopg2",
+    "opentelemetry-instrumentation-redis",
+    "opentelemetry-instrumentation-pymongo",
     "gitpython",
     "eval-type-backport",
     "requests-mock",
     "inline-snapshot",
     "structlog",
     "loguru",
     "ruff",
```

### Comparing `logfire-0.38.0/PKG-INFO` & `logfire-0.39.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: logfire
-Version: 0.38.0
+Version: 0.39.0
 Summary: The best Python observability tool! 🪵🔥
 Author-email: Pydantic Team <engineering@pydantic.dev>, Samuel Colvin <samuel@pydantic.dev>, Hasan Ramezani <hasan@pydantic.dev>, Adrian Garcia Badaracco <adrian@pydantic.dev>, David Montague <david@pydantic.dev>, Marcelo Trylesinski <marcelo@pydantic.dev>, David Hewitt <david.hewitt@pydantic.dev>, Alex Hall <alex@pydantic.dev>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
```

