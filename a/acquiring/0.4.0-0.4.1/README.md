# Comparing `tmp/acquiring-0.4.0.tar.gz` & `tmp/acquiring-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acquiring-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "acquiring-0.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `acquiring-0.4.0.tar` & `acquiring-0.4.1.tar`

### file list

```diff
@@ -1,128 +1,130 @@
--rw-r--r--   0        0        0       28 2024-04-08 09:12:12.325260 acquiring-0.4.0/.adr-dir
--rw-r--r--   0        0        0      135 2024-06-01 13:31:37.596614 acquiring-0.4.0/.env.example
--rw-r--r--   0        0        0     3104 2024-04-29 15:06:04.143509 acquiring-0.4.0/.gitignore
--rw-r--r--   0        0        0      211 2024-06-01 13:31:30.121387 acquiring-0.4.0/.markdownlint.json
--rw-r--r--   0        0        0     3069 2024-05-26 15:58:35.566595 acquiring-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      438 2024-04-10 10:25:12.720112 acquiring-0.4.0/.readthedocs.yaml
--rw-r--r--   0        0        0     2076 2024-06-01 13:22:41.842198 acquiring-0.4.0/CHANGELOG.md
--rw-r--r--   0        0        0     1234 2024-04-12 07:54:52.741316 acquiring-0.4.0/Dockerfile
--rw-r--r--   0        0        0     1070 2024-04-07 19:04:14.604203 acquiring-0.4.0/LICENSE
--rw-r--r--   0        0        0      190 2024-04-09 20:23:33.063639 acquiring-0.4.0/MANIFEST.in
--rw-r--r--   0        0        0     2071 2024-06-01 13:01:58.987256 acquiring-0.4.0/README.md
--rw-r--r--   0        0        0      173 2024-06-01 13:14:33.064610 acquiring-0.4.0/acquiring/__init__.py
--rw-r--r--   0        0        0      616 2024-04-23 21:15:41.949805 acquiring-0.4.0/acquiring/apps.py
--rw-r--r--   0        0        0        0 2024-04-15 21:24:21.472983 acquiring-0.4.0/acquiring/contrib/__init__.py
--rw-r--r--   0        0        0      407 2024-04-12 14:53:46.923556 acquiring-0.4.0/acquiring/contrib/paypal/__init__.py
--rw-r--r--   0        0        0     6358 2024-05-30 10:13:58.938564 acquiring-0.4.0/acquiring/contrib/paypal/adapter.py
--rw-r--r--   0        0        0      178 2024-04-07 19:04:14.605022 acquiring-0.4.0/acquiring/contrib/paypal/blocks/__init__.py
--rw-r--r--   0        0        0     1290 2024-05-17 14:00:23.251940 acquiring-0.4.0/acquiring/contrib/paypal/blocks/paypal_after_creating_order.py
--rw-r--r--   0        0        0     1997 2024-05-30 10:17:16.865113 acquiring-0.4.0/acquiring/contrib/paypal/blocks/paypal_create_order.py
--rw-r--r--   0        0        0     1571 2024-05-29 22:36:24.230122 acquiring-0.4.0/acquiring/contrib/paypal/domain.py
--rw-r--r--   0        0        0      701 2024-06-01 13:02:19.861189 acquiring-0.4.0/acquiring/domain/__init__.py
--rw-r--r--   0        0        0     1809 2024-05-29 22:18:48.938327 acquiring-0.4.0/acquiring/domain/blocks.py
--rw-r--r--   0        0        0     7134 2024-05-27 17:46:09.097963 acquiring-0.4.0/acquiring/domain/decision_logic.py
--rw-r--r--   0        0        0      976 2024-05-29 22:18:48.939034 acquiring-0.4.0/acquiring/domain/events.py
--rw-r--r--   0        0        0     4409 2024-05-29 22:24:56.271672 acquiring-0.4.0/acquiring/domain/payments.py
--rw-r--r--   0        0        0     1741 2024-05-29 22:36:11.448770 acquiring-0.4.0/acquiring/domain/providers.py
--rw-r--r--   0        0        0    20975 2024-06-01 13:01:58.987389 acquiring-0.4.0/acquiring/domain/sagas.py
--rw-r--r--   0        0        0     1313 2024-05-26 10:26:36.790316 acquiring-0.4.0/acquiring/enums.py
--rw-r--r--   0        0        0     1632 2024-06-01 13:01:58.987406 acquiring-0.4.0/acquiring/protocols/__init__.py
--rw-r--r--   0        0        0      376 2024-05-29 22:18:48.939484 acquiring-0.4.0/acquiring/protocols/events.py
--rw-r--r--   0        0        0     3106 2024-05-29 22:25:12.800542 acquiring-0.4.0/acquiring/protocols/payments.py
--rw-r--r--   0        0        0      829 2024-05-29 22:36:31.647078 acquiring-0.4.0/acquiring/protocols/providers.py
--rw-r--r--   0        0        0     2180 2024-05-26 11:24:05.527621 acquiring-0.4.0/acquiring/protocols/storage.py
--rw-r--r--   0        0        0      401 2024-04-23 17:52:13.537616 acquiring-0.4.0/acquiring/settings.py
--rw-r--r--   0        0        0      211 2024-04-23 17:50:49.596526 acquiring-0.4.0/acquiring/storage/__init__.py
--rw-r--r--   0        0        0      427 2024-04-29 08:48:45.522667 acquiring-0.4.0/acquiring/storage/django/__init__.py
--rw-r--r--   0        0        0     6589 2024-06-01 13:01:58.987376 acquiring-0.4.0/acquiring/storage/django/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-04-23 17:30:44.249631 acquiring-0.4.0/acquiring/storage/django/migrations/__init__.py
--rw-r--r--   0        0        0     9190 2024-06-01 13:01:58.987446 acquiring-0.4.0/acquiring/storage/django/models.py
--rw-r--r--   0        0        0     4864 2024-05-31 21:27:51.033502 acquiring-0.4.0/acquiring/storage/django/repositories.py
--rw-r--r--   0        0        0     2447 2024-05-26 11:24:05.530031 acquiring-0.4.0/acquiring/storage/django/unit_of_work.py
--rw-r--r--   0        0        0      249 2024-05-31 21:28:49.667470 acquiring-0.4.0/acquiring/storage/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2275 2024-04-22 21:40:07.708206 acquiring-0.4.0/acquiring/storage/sqlalchemy/migrations/env.py
--rw-r--r--   0        0        0      635 2024-04-12 20:54:32.999638 acquiring-0.4.0/acquiring/storage/sqlalchemy/migrations/script.py.mako
--rw-r--r--   0        0        0     1973 2024-05-31 21:20:47.859831 acquiring-0.4.0/acquiring/storage/sqlalchemy/migrations/versions/87b793f35b89_add_acquiring_models.py
--rw-r--r--   0        0        0     4232 2024-05-31 21:27:50.910863 acquiring-0.4.0/acquiring/storage/sqlalchemy/models.py
--rw-r--r--   0        0        0     1991 2024-05-31 21:48:37.611107 acquiring-0.4.0/acquiring/storage/sqlalchemy/repositories.py
--rw-r--r--   0        0        0     2208 2024-05-26 11:24:05.530007 acquiring-0.4.0/acquiring/storage/sqlalchemy/unit_of_work.py
--rw-r--r--   0        0        0      358 2024-04-15 21:24:04.465544 acquiring-0.4.0/acquiring/utils.py
--rw-r--r--   0        0        0     3683 2024-04-23 17:33:13.035493 acquiring-0.4.0/alembic.ini
--rw-r--r--   0        0        0      712 2024-04-29 15:02:03.580627 acquiring-0.4.0/docker-compose.yaml
--rw-r--r--   0        0        0      394 2024-04-10 10:23:35.861556 acquiring-0.4.0/docs/Dockerfile
--rw-r--r--   0        0        0      483 2024-04-08 09:12:13.455703 acquiring-0.4.0/docs/architecture/decisions/0001-record-architecture-decisions.md
--rw-r--r--   0        0        0     1395 2024-04-10 14:01:00.812132 acquiring-0.4.0/docs/architecture/decisions/0002-use-tacit-tests.md
--rw-r--r--   0        0        0     1641 2024-04-10 18:18:42.875494 acquiring-0.4.0/docs/architecture/decisions/0003-documentation-is-code.md
--rw-r--r--   0        0        0     1012 2024-04-10 21:28:47.193576 acquiring-0.4.0/docs/architecture/decisions/0004-reduce-doctests-to-a-minimum.md
--rw-r--r--   0        0        0     3453 2024-04-13 18:02:53.958745 acquiring-0.4.0/docs/architecture/decisions/0005-maybe-functions-considered-harmful.md
--rw-r--r--   0        0        0     2647 2024-04-14 21:02:55.401009 acquiring-0.4.0/docs/architecture/decisions/0006-use-import-module-more-often-than-from-module-import.md
--rw-r--r--   0        0        0      647 2024-04-18 11:37:03.298067 acquiring-0.4.0/docs/architecture/decisions/0007-type-sparingly-but-with-confidence.md
--rw-r--r--   0        0        0     2200 2024-05-30 13:37:37.864709 acquiring-0.4.0/docs/architecture/decisions/0008-domain-logic-happens-in-native-python.md
--rw-r--r--   0        0        0     1345 2024-04-25 10:17:21.246825 acquiring-0.4.0/docs/architecture/decisions/0009-do-not-use-if-type-checking.md
--rw-r--r--   0        0        0     1102 2024-04-28 21:12:22.951710 acquiring-0.4.0/docs/architecture/decisions/0010-exceptions-can-express-domain-concepts-too.md
--rw-r--r--   0        0        0      988 2024-05-06 16:10:08.334738 acquiring-0.4.0/docs/architecture/decisions/0011-worse-is-better.md
--rw-r--r--   0        0        0      416 2024-05-15 16:50:09.923734 acquiring-0.4.0/docs/architecture/decisions/0012-usage-driven-design.md
--rw-r--r--   0        0        0     1860 2024-06-01 13:01:59.040588 acquiring-0.4.0/docs/architecture/decisions/0013-separate-void-and-refund-operation-types.md
--rw-r--r--   0        0        0      569 2024-05-29 22:35:27.374182 acquiring-0.4.0/docs/architecture/decisions/0014-created-at-are-internal-datetimes-timestamps-are-external.md
--rw-r--r--   0        0        0     9049 2024-05-30 22:11:19.726387 acquiring-0.4.0/docs/architecture/decisions/0015-the-elements-of-acquiring-architecture.md
--rw-r--r--   0        0        0     1590 2024-04-14 21:14:41.043915 acquiring-0.4.0/docs/architecture/index.md
--rw-r--r--   0        0        0      751 2024-06-01 13:01:59.036083 acquiring-0.4.0/docs/index.md
--rw-r--r--   0        0        0      103 2024-04-10 18:23:18.673084 acquiring-0.4.0/docs/requirements.txt
--rwxr-xr-x   0        0        0      666 2024-04-07 19:04:14.607704 acquiring-0.4.0/manage.py
--rw-r--r--   0        0        0      164 2024-04-16 14:08:55.167288 acquiring-0.4.0/mkdocs.yml
--rw-r--r--   0        0        0     1865 2024-05-26 15:59:35.361519 acquiring-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      158 2024-04-12 14:51:26.788691 acquiring-0.4.0/requirements/base.txt
--rw-r--r--   0        0        0      136 2024-04-07 19:04:14.607992 acquiring-0.4.0/requirements/development-django.txt
--rw-r--r--   0        0        0       69 2024-04-12 09:27:58.484325 acquiring-0.4.0/requirements/development-sqlalchemy.txt
--rw-r--r--   0        0        0      634 2024-04-15 21:31:52.585788 acquiring-0.4.0/requirements/development.txt
--rw-r--r--   0        0        0       74 2024-04-07 19:04:14.608127 acquiring-0.4.0/requirements/packaging.txt
--rw-r--r--   0        0        0        0 2024-04-07 19:04:14.608351 acquiring-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0     9993 2024-05-30 10:15:47.865303 acquiring-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0      100 2024-04-12 14:53:46.923656 acquiring-0.4.0/tests/contrib/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 19:04:14.608767 acquiring-0.4.0/tests/contrib/paypal/__init__.py
--rw-r--r--   0        0        0     6011 2024-05-30 10:22:12.891786 acquiring-0.4.0/tests/contrib/paypal/blocks/test_paypal_after_creating_order.py
--rw-r--r--   0        0        0     4975 2024-05-30 10:17:16.886617 acquiring-0.4.0/tests/contrib/paypal/blocks/test_paypal_create_order.py
--rw-r--r--   0        0        0     2836 2024-05-17 14:06:52.895692 acquiring-0.4.0/tests/contrib/paypal/test_adapter.py
--rw-r--r--   0        0        0        0 2024-04-07 19:04:14.610219 acquiring-0.4.0/tests/domain/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 19:04:14.610302 acquiring-0.4.0/tests/domain/blocks/__init__.py
--rw-r--r--   0        0        0     2616 2024-05-30 10:14:28.893896 acquiring-0.4.0/tests/domain/blocks/test_wrapped_by_block_events.py
--rw-r--r--   0        0        0      845 2024-05-28 17:50:19.138678 acquiring-0.4.0/tests/domain/factories.py
--rw-r--r--   0        0        0        0 2024-04-07 19:04:14.610549 acquiring-0.4.0/tests/domain/flows/__init__.py
--rw-r--r--   0        0        0     1898 2024-05-16 11:01:09.097657 acquiring-0.4.0/tests/domain/flows/conftest.py
--rw-r--r--   0        0        0     9431 2024-06-01 13:01:58.987319 acquiring-0.4.0/tests/domain/flows/test_after_confirm.py
--rw-r--r--   0        0        0     7858 2024-06-01 13:01:58.987328 acquiring-0.4.0/tests/domain/flows/test_after_pay.py
--rw-r--r--   0        0        0     8554 2024-06-01 13:01:58.987299 acquiring-0.4.0/tests/domain/flows/test_confirm.py
--rw-r--r--   0        0        0     1839 2024-06-01 13:01:58.987288 acquiring-0.4.0/tests/domain/flows/test_define_payment_flow.py
--rw-r--r--   0        0        0    10121 2024-06-01 13:01:58.987309 acquiring-0.4.0/tests/domain/flows/test_initialize.py
--rw-r--r--   0        0        0     7568 2024-06-01 13:01:58.987271 acquiring-0.4.0/tests/domain/flows/test_pay.py
--rw-r--r--   0        0        0    13987 2024-06-01 13:01:58.987357 acquiring-0.4.0/tests/domain/flows/test_process_actions.py
--rw-r--r--   0        0        0     8815 2024-06-01 13:02:11.642449 acquiring-0.4.0/tests/domain/flows/test_refresh_payment_method.py
--rw-r--r--   0        0        0        0 2024-04-07 19:04:14.611424 acquiring-0.4.0/tests/domain/providers/__init__.py
--rw-r--r--   0        0        0     3321 2024-05-31 21:29:44.877433 acquiring-0.4.0/tests/domain/providers/test_wrapped_by_transaction.py
--rw-r--r--   0        0        0    53408 2024-06-01 13:02:11.106521 acquiring-0.4.0/tests/domain/test_decision_logic.py
--rw-r--r--   0        0        0     1814 2024-05-30 10:05:51.292007 acquiring-0.4.0/tests/protocols.py
--rw-r--r--   0        0        0        0 2024-04-12 13:19:52.684632 acquiring-0.4.0/tests/storage/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 13:20:06.748701 acquiring-0.4.0/tests/storage/django/__init__.py
--rw-r--r--   0        0        0     1318 2024-05-29 22:26:32.922884 acquiring-0.4.0/tests/storage/django/factories.py
--rw-r--r--   0        0        0        0 2024-04-12 13:18:56.952489 acquiring-0.4.0/tests/storage/django/repositories/__init__.py
--rw-r--r--   0        0        0     2725 2024-05-29 22:18:48.950099 acquiring-0.4.0/tests/storage/django/repositories/test_block_event_repository.py
--rw-r--r--   0        0        0     3136 2024-05-29 22:26:30.831884 acquiring-0.4.0/tests/storage/django/repositories/test_payment_method_repository.py
--rw-r--r--   0        0        0     1658 2024-05-31 21:35:59.016271 acquiring-0.4.0/tests/storage/django/repositories/test_payment_operation_repository.py
--rw-r--r--   0        0        0     2428 2024-05-29 22:29:51.792891 acquiring-0.4.0/tests/storage/django/repositories/test_token_repository.py
--rw-r--r--   0        0        0     1270 2024-05-30 10:16:51.018244 acquiring-0.4.0/tests/storage/django/repositories/test_transaction_repository.py
--rw-r--r--   0        0        0     9705 2024-05-24 10:43:45.311465 acquiring-0.4.0/tests/storage/django/repositories/test_unit_of_work.py
--rw-r--r--   0        0        0      518 2024-05-16 11:01:09.114699 acquiring-0.4.0/tests/storage/django/test_migrations.py
--rw-r--r--   0        0        0      937 2024-05-24 10:43:31.338785 acquiring-0.4.0/tests/storage/django/test_models.py
--rw-r--r--   0        0        0        0 2024-04-12 13:27:27.777130 acquiring-0.4.0/tests/storage/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2049 2024-05-16 11:00:30.051582 acquiring-0.4.0/tests/storage/sqlalchemy/conftest.py
--rw-r--r--   0        0        0      873 2024-05-28 15:41:53.449800 acquiring-0.4.0/tests/storage/sqlalchemy/factories.py
--rw-r--r--   0        0        0        0 2024-04-12 13:27:36.895251 acquiring-0.4.0/tests/storage/sqlalchemy/repositories/__init__.py
--rw-r--r--   0        0        0     2432 2024-05-16 11:01:09.118294 acquiring-0.4.0/tests/storage/sqlalchemy/repositories/test_payment_method_repository.py
--rw-r--r--   0        0        0     1674 2024-05-31 21:48:38.308166 acquiring-0.4.0/tests/storage/sqlalchemy/repositories/test_payment_operation_repository.py
--rw-r--r--   0        0        0    11090 2024-05-18 03:17:33.934948 acquiring-0.4.0/tests/storage/sqlalchemy/repositories/test_unit_of_work.py
--rw-r--r--   0        0        0       32 2024-04-13 21:49:54.429636 acquiring-0.4.0/tests/storage/sqlalchemy/test_migrations.py
--rw-r--r--   0        0        0      634 2024-04-25 08:54:50.066518 acquiring-0.4.0/tests/storage/test_tacit.py
--rw-r--r--   0        0        0      370 2024-05-16 11:01:09.120540 acquiring-0.4.0/tests/storage/utils.py
--rw-r--r--   0        0        0     2511 2024-05-16 11:00:30.057049 acquiring-0.4.0/tests/tacit/test_files.py
--rw-r--r--   0        0        0      835 2024-04-07 19:04:14.611782 acquiring-0.4.0/tox.ini
--rw-r--r--   0        0        0     3102 1970-01-01 00:00:00.000000 acquiring-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       28 2024-04-08 09:12:12.325260 acquiring-0.4.1/.adr-dir
+-rw-r--r--   0        0        0      135 2024-06-03 10:54:04.750917 acquiring-0.4.1/.env.example
+-rw-r--r--   0        0        0     3104 2024-06-01 21:21:57.502949 acquiring-0.4.1/.gitignore
+-rw-r--r--   0        0        0      211 2024-06-01 13:31:30.121387 acquiring-0.4.1/.markdownlint.json
+-rw-r--r--   0        0        0     3443 2024-06-01 21:57:26.085346 acquiring-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      438 2024-04-10 10:25:12.720112 acquiring-0.4.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     2216 2024-06-03 10:51:30.437497 acquiring-0.4.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1234 2024-04-12 07:54:52.741316 acquiring-0.4.1/Dockerfile
+-rw-r--r--   0        0        0     1070 2024-04-07 19:04:14.604203 acquiring-0.4.1/LICENSE
+-rw-r--r--   0        0        0      190 2024-04-09 20:23:33.063639 acquiring-0.4.1/MANIFEST.in
+-rw-r--r--   0        0        0     2071 2024-06-01 13:01:58.987256 acquiring-0.4.1/README.md
+-rw-r--r--   0        0        0      173 2024-06-03 10:53:45.023251 acquiring-0.4.1/acquiring/__init__.py
+-rw-r--r--   0        0        0      616 2024-04-23 21:15:41.949805 acquiring-0.4.1/acquiring/apps.py
+-rw-r--r--   0        0        0        0 2024-04-15 21:24:21.472983 acquiring-0.4.1/acquiring/contrib/__init__.py
+-rw-r--r--   0        0        0      407 2024-04-12 14:53:46.923556 acquiring-0.4.1/acquiring/contrib/paypal/__init__.py
+-rw-r--r--   0        0        0     6358 2024-05-30 10:13:58.938564 acquiring-0.4.1/acquiring/contrib/paypal/adapter.py
+-rw-r--r--   0        0        0      178 2024-04-07 19:04:14.605022 acquiring-0.4.1/acquiring/contrib/paypal/blocks/__init__.py
+-rw-r--r--   0        0        0     1290 2024-05-17 14:00:23.251940 acquiring-0.4.1/acquiring/contrib/paypal/blocks/paypal_after_creating_order.py
+-rw-r--r--   0        0        0     1997 2024-05-30 10:17:16.865113 acquiring-0.4.1/acquiring/contrib/paypal/blocks/paypal_create_order.py
+-rw-r--r--   0        0        0     1571 2024-05-29 22:36:24.230122 acquiring-0.4.1/acquiring/contrib/paypal/domain.py
+-rw-r--r--   0        0        0      701 2024-06-01 13:02:19.861189 acquiring-0.4.1/acquiring/domain/__init__.py
+-rw-r--r--   0        0        0     1809 2024-05-29 22:18:48.938327 acquiring-0.4.1/acquiring/domain/blocks.py
+-rw-r--r--   0        0        0     7134 2024-05-27 17:46:09.097963 acquiring-0.4.1/acquiring/domain/decision_logic.py
+-rw-r--r--   0        0        0      976 2024-05-29 22:18:48.939034 acquiring-0.4.1/acquiring/domain/events.py
+-rw-r--r--   0        0        0     4409 2024-05-29 22:24:56.271672 acquiring-0.4.1/acquiring/domain/payments.py
+-rw-r--r--   0        0        0     1741 2024-05-29 22:36:11.448770 acquiring-0.4.1/acquiring/domain/providers.py
+-rw-r--r--   0        0        0    20975 2024-06-01 13:01:58.987389 acquiring-0.4.1/acquiring/domain/sagas.py
+-rw-r--r--   0        0        0     1313 2024-05-26 10:26:36.790316 acquiring-0.4.1/acquiring/enums.py
+-rw-r--r--   0        0        0     1632 2024-06-01 13:01:58.987406 acquiring-0.4.1/acquiring/protocols/__init__.py
+-rw-r--r--   0        0        0      376 2024-05-29 22:18:48.939484 acquiring-0.4.1/acquiring/protocols/events.py
+-rw-r--r--   0        0        0     3106 2024-05-29 22:25:12.800542 acquiring-0.4.1/acquiring/protocols/payments.py
+-rw-r--r--   0        0        0      829 2024-05-29 22:36:31.647078 acquiring-0.4.1/acquiring/protocols/providers.py
+-rw-r--r--   0        0        0     2180 2024-05-26 11:24:05.527621 acquiring-0.4.1/acquiring/protocols/storage.py
+-rw-r--r--   0        0        0      401 2024-04-23 17:52:13.537616 acquiring-0.4.1/acquiring/settings.py
+-rw-r--r--   0        0        0      211 2024-04-23 17:50:49.596526 acquiring-0.4.1/acquiring/storage/__init__.py
+-rw-r--r--   0        0        0      427 2024-04-29 08:48:45.522667 acquiring-0.4.1/acquiring/storage/django/__init__.py
+-rw-r--r--   0        0        0     6589 2024-06-01 13:01:58.987376 acquiring-0.4.1/acquiring/storage/django/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:30:44.249631 acquiring-0.4.1/acquiring/storage/django/migrations/__init__.py
+-rw-r--r--   0        0        0     9190 2024-06-02 20:46:47.040440 acquiring-0.4.1/acquiring/storage/django/models.py
+-rw-r--r--   0        0        0     4864 2024-05-31 21:27:51.033502 acquiring-0.4.1/acquiring/storage/django/repositories.py
+-rw-r--r--   0        0        0     2447 2024-05-26 11:24:05.530031 acquiring-0.4.1/acquiring/storage/django/unit_of_work.py
+-rw-r--r--   0        0        0      249 2024-05-31 21:28:49.667470 acquiring-0.4.1/acquiring/storage/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2275 2024-04-22 21:40:07.708206 acquiring-0.4.1/acquiring/storage/sqlalchemy/migrations/env.py
+-rw-r--r--   0        0        0      635 2024-04-12 20:54:32.999638 acquiring-0.4.1/acquiring/storage/sqlalchemy/migrations/script.py.mako
+-rw-r--r--   0        0        0     1973 2024-05-31 21:20:47.859831 acquiring-0.4.1/acquiring/storage/sqlalchemy/migrations/versions/87b793f35b89_add_acquiring_models.py
+-rw-r--r--   0        0        0     4232 2024-05-31 21:27:50.910863 acquiring-0.4.1/acquiring/storage/sqlalchemy/models.py
+-rw-r--r--   0        0        0     1991 2024-05-31 21:48:37.611107 acquiring-0.4.1/acquiring/storage/sqlalchemy/repositories.py
+-rw-r--r--   0        0        0     2208 2024-05-26 11:24:05.530007 acquiring-0.4.1/acquiring/storage/sqlalchemy/unit_of_work.py
+-rw-r--r--   0        0        0      358 2024-04-15 21:24:04.465544 acquiring-0.4.1/acquiring/utils.py
+-rw-r--r--   0        0        0     3683 2024-04-23 17:33:13.035493 acquiring-0.4.1/alembic.ini
+-rw-r--r--   0        0        0      716 2024-06-03 10:53:03.082823 acquiring-0.4.1/docker-compose.yaml
+-rw-r--r--   0        0        0      446 2024-06-01 21:32:41.882066 acquiring-0.4.1/docs/Dockerfile
+-rw-r--r--   0        0        0      483 2024-04-08 09:12:13.455703 acquiring-0.4.1/docs/architecture/decisions/0001-record-architecture-decisions.md
+-rw-r--r--   0        0        0     1395 2024-04-10 14:01:00.812132 acquiring-0.4.1/docs/architecture/decisions/0002-use-tacit-tests.md
+-rw-r--r--   0        0        0     1641 2024-04-10 18:18:42.875494 acquiring-0.4.1/docs/architecture/decisions/0003-documentation-is-code.md
+-rw-r--r--   0        0        0     1012 2024-04-10 21:28:47.193576 acquiring-0.4.1/docs/architecture/decisions/0004-reduce-doctests-to-a-minimum.md
+-rw-r--r--   0        0        0     3453 2024-04-13 18:02:53.958745 acquiring-0.4.1/docs/architecture/decisions/0005-maybe-functions-considered-harmful.md
+-rw-r--r--   0        0        0     2647 2024-04-14 21:02:55.401009 acquiring-0.4.1/docs/architecture/decisions/0006-use-import-module-more-often-than-from-module-import.md
+-rw-r--r--   0        0        0      647 2024-04-18 11:37:03.298067 acquiring-0.4.1/docs/architecture/decisions/0007-type-sparingly-but-with-confidence.md
+-rw-r--r--   0        0        0     2200 2024-05-30 13:37:37.864709 acquiring-0.4.1/docs/architecture/decisions/0008-domain-logic-happens-in-native-python.md
+-rw-r--r--   0        0        0     1345 2024-04-25 10:17:21.246825 acquiring-0.4.1/docs/architecture/decisions/0009-do-not-use-if-type-checking.md
+-rw-r--r--   0        0        0     1102 2024-04-28 21:12:22.951710 acquiring-0.4.1/docs/architecture/decisions/0010-exceptions-can-express-domain-concepts-too.md
+-rw-r--r--   0        0        0      988 2024-05-06 16:10:08.334738 acquiring-0.4.1/docs/architecture/decisions/0011-worse-is-better.md
+-rw-r--r--   0        0        0      416 2024-05-15 16:50:09.923734 acquiring-0.4.1/docs/architecture/decisions/0012-usage-driven-design.md
+-rw-r--r--   0        0        0     1860 2024-06-01 13:01:59.040588 acquiring-0.4.1/docs/architecture/decisions/0013-separate-void-and-refund-operation-types.md
+-rw-r--r--   0        0        0      569 2024-05-29 22:35:27.374182 acquiring-0.4.1/docs/architecture/decisions/0014-created-at-are-internal-datetimes-timestamps-are-external.md
+-rw-r--r--   0        0        0     9049 2024-05-30 22:11:19.726387 acquiring-0.4.1/docs/architecture/decisions/0015-the-elements-of-acquiring-architecture.md
+-rw-r--r--   0        0        0     1590 2024-04-14 21:14:41.043915 acquiring-0.4.1/docs/architecture/index.md
+-rw-r--r--   0        0        0      751 2024-06-02 14:07:44.557116 acquiring-0.4.1/docs/index.md
+-rw-r--r--   0        0        0      103 2024-04-10 18:23:18.673084 acquiring-0.4.1/docs/requirements.txt
+-rwxr-xr-x   0        0        0      666 2024-04-07 19:04:14.607704 acquiring-0.4.1/manage.py
+-rw-r--r--   0        0        0       60 2024-06-01 23:18:01.814333 acquiring-0.4.1/material/overrides/main.html
+-rw-r--r--   0        0        0      247 2024-06-02 14:29:34.178006 acquiring-0.4.1/mkdocs.yml
+-rw-r--r--   0        0        0     1879 2024-06-03 10:47:55.755820 acquiring-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-06-03 10:30:37.846074 acquiring-0.4.1/qa/project/__init__.py
+-rw-r--r--   0        0        0      158 2024-06-03 10:48:26.432116 acquiring-0.4.1/requirements/base.txt
+-rw-r--r--   0        0        0      136 2024-04-07 19:04:14.607992 acquiring-0.4.1/requirements/development-django.txt
+-rw-r--r--   0        0        0       69 2024-04-12 09:27:58.484325 acquiring-0.4.1/requirements/development-sqlalchemy.txt
+-rw-r--r--   0        0        0      634 2024-04-15 21:31:52.585788 acquiring-0.4.1/requirements/development.txt
+-rw-r--r--   0        0        0       74 2024-04-07 19:04:14.608127 acquiring-0.4.1/requirements/packaging.txt
+-rw-r--r--   0        0        0        0 2024-04-07 19:04:14.608351 acquiring-0.4.1/tests/__init__.py
+-rw-r--r--   0        0        0     9993 2024-05-30 10:15:47.865303 acquiring-0.4.1/tests/conftest.py
+-rw-r--r--   0        0        0      100 2024-04-12 14:53:46.923656 acquiring-0.4.1/tests/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 19:04:14.608767 acquiring-0.4.1/tests/contrib/paypal/__init__.py
+-rw-r--r--   0        0        0     6011 2024-05-30 10:22:12.891786 acquiring-0.4.1/tests/contrib/paypal/blocks/test_paypal_after_creating_order.py
+-rw-r--r--   0        0        0     4975 2024-05-30 10:17:16.886617 acquiring-0.4.1/tests/contrib/paypal/blocks/test_paypal_create_order.py
+-rw-r--r--   0        0        0     2836 2024-05-17 14:06:52.895692 acquiring-0.4.1/tests/contrib/paypal/test_adapter.py
+-rw-r--r--   0        0        0        0 2024-04-07 19:04:14.610219 acquiring-0.4.1/tests/domain/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 19:04:14.610302 acquiring-0.4.1/tests/domain/blocks/__init__.py
+-rw-r--r--   0        0        0     2616 2024-05-30 10:14:28.893896 acquiring-0.4.1/tests/domain/blocks/test_wrapped_by_block_events.py
+-rw-r--r--   0        0        0      845 2024-05-28 17:50:19.138678 acquiring-0.4.1/tests/domain/factories.py
+-rw-r--r--   0        0        0        0 2024-04-07 19:04:14.610549 acquiring-0.4.1/tests/domain/flows/__init__.py
+-rw-r--r--   0        0        0     1898 2024-05-16 11:01:09.097657 acquiring-0.4.1/tests/domain/flows/conftest.py
+-rw-r--r--   0        0        0     9242 2024-06-02 20:47:41.091873 acquiring-0.4.1/tests/domain/flows/test_after_confirm.py
+-rw-r--r--   0        0        0     7634 2024-06-02 20:47:41.078445 acquiring-0.4.1/tests/domain/flows/test_after_pay.py
+-rw-r--r--   0        0        0     8330 2024-06-02 20:47:41.090465 acquiring-0.4.1/tests/domain/flows/test_confirm.py
+-rw-r--r--   0        0        0     1839 2024-06-01 13:01:58.987288 acquiring-0.4.1/tests/domain/flows/test_define_payment_flow.py
+-rw-r--r--   0        0        0     9747 2024-06-02 20:47:41.109258 acquiring-0.4.1/tests/domain/flows/test_initialize.py
+-rw-r--r--   0        0        0     7340 2024-06-02 20:47:41.082245 acquiring-0.4.1/tests/domain/flows/test_pay.py
+-rw-r--r--   0        0        0    13547 2024-06-02 20:47:41.160945 acquiring-0.4.1/tests/domain/flows/test_process_actions.py
+-rw-r--r--   0        0        0     8815 2024-06-01 13:02:11.642449 acquiring-0.4.1/tests/domain/flows/test_refresh_payment_method.py
+-rw-r--r--   0        0        0        0 2024-04-07 19:04:14.611424 acquiring-0.4.1/tests/domain/providers/__init__.py
+-rw-r--r--   0        0        0     3321 2024-05-31 21:29:44.877433 acquiring-0.4.1/tests/domain/providers/test_wrapped_by_transaction.py
+-rw-r--r--   0        0        0    53408 2024-06-01 13:02:11.106521 acquiring-0.4.1/tests/domain/test_decision_logic.py
+-rw-r--r--   0        0        0     1814 2024-05-30 10:05:51.292007 acquiring-0.4.1/tests/protocols.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:19:52.684632 acquiring-0.4.1/tests/storage/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:20:06.748701 acquiring-0.4.1/tests/storage/django/__init__.py
+-rw-r--r--   0        0        0     1318 2024-05-29 22:26:32.922884 acquiring-0.4.1/tests/storage/django/factories.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:18:56.952489 acquiring-0.4.1/tests/storage/django/repositories/__init__.py
+-rw-r--r--   0        0        0     2725 2024-05-29 22:18:48.950099 acquiring-0.4.1/tests/storage/django/repositories/test_block_event_repository.py
+-rw-r--r--   0        0        0     3136 2024-05-29 22:26:30.831884 acquiring-0.4.1/tests/storage/django/repositories/test_payment_method_repository.py
+-rw-r--r--   0        0        0     1399 2024-06-02 20:47:40.495044 acquiring-0.4.1/tests/storage/django/repositories/test_payment_operation_repository.py
+-rw-r--r--   0        0        0     2428 2024-05-29 22:29:51.792891 acquiring-0.4.1/tests/storage/django/repositories/test_token_repository.py
+-rw-r--r--   0        0        0     1270 2024-05-30 10:16:51.018244 acquiring-0.4.1/tests/storage/django/repositories/test_transaction_repository.py
+-rw-r--r--   0        0        0     9705 2024-05-24 10:43:45.311465 acquiring-0.4.1/tests/storage/django/repositories/test_unit_of_work.py
+-rw-r--r--   0        0        0      518 2024-05-16 11:01:09.114699 acquiring-0.4.1/tests/storage/django/test_migrations.py
+-rw-r--r--   0        0        0      937 2024-05-24 10:43:31.338785 acquiring-0.4.1/tests/storage/django/test_models.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:27:27.777130 acquiring-0.4.1/tests/storage/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2049 2024-05-16 11:00:30.051582 acquiring-0.4.1/tests/storage/sqlalchemy/conftest.py
+-rw-r--r--   0        0        0      873 2024-05-28 15:41:53.449800 acquiring-0.4.1/tests/storage/sqlalchemy/factories.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:27:36.895251 acquiring-0.4.1/tests/storage/sqlalchemy/repositories/__init__.py
+-rw-r--r--   0        0        0     2432 2024-05-16 11:01:09.118294 acquiring-0.4.1/tests/storage/sqlalchemy/repositories/test_payment_method_repository.py
+-rw-r--r--   0        0        0     1609 2024-06-02 20:47:41.023693 acquiring-0.4.1/tests/storage/sqlalchemy/repositories/test_payment_operation_repository.py
+-rw-r--r--   0        0        0    11090 2024-05-18 03:17:33.934948 acquiring-0.4.1/tests/storage/sqlalchemy/repositories/test_unit_of_work.py
+-rw-r--r--   0        0        0       32 2024-04-13 21:49:54.429636 acquiring-0.4.1/tests/storage/sqlalchemy/test_migrations.py
+-rw-r--r--   0        0        0      634 2024-04-25 08:54:50.066518 acquiring-0.4.1/tests/storage/test_tacit.py
+-rw-r--r--   0        0        0      370 2024-05-16 11:01:09.120540 acquiring-0.4.1/tests/storage/utils.py
+-rw-r--r--   0        0        0     2511 2024-05-16 11:00:30.057049 acquiring-0.4.1/tests/tacit/test_files.py
+-rw-r--r--   0        0        0      835 2024-04-07 19:04:14.611782 acquiring-0.4.1/tox.ini
+-rw-r--r--   0        0        0     3153 1970-01-01 00:00:00.000000 acquiring-0.4.1/PKG-INFO
```

### Comparing `acquiring-0.4.0/.gitignore` & `acquiring-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/.pre-commit-config.yaml` & `acquiring-0.4.1/.pre-commit-config.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     -   id: trailing-whitespace
 -   repo: https://github.com/PyCQA/bandit
     rev: 1.7.8
     hooks:
     -   id: bandit
         args: ["-c", "pyproject.toml"]
 -   repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.4.5
+    rev: v0.4.7
     hooks:
     -   id: ruff
         args: [ --fix ]
 -   repo: https://github.com/jorisroovers/gitlint
     rev: v0.19.1
     hooks:
       - id: gitlint
@@ -78,22 +78,35 @@
 #     -   id: detect-secrets
 #         args: ['--baseline', '.secrets.baseline']
 # -   repo: https://github.com/mgedmin/check-manifest
 #     rev: "0.49"
 #     hooks:
 #     -   id: check-manifest
 -   repo: https://github.com/gitleaks/gitleaks
-    rev: v8.18.2
+    rev: v8.18.3
     hooks:
     -   id: gitleaks
 -   repo: https://gitlab.com/adam-moss/pre-commit-trailer
     rev: v1.1.0
     hooks:
     -   id: add-pre-commit-config-trailer
 -   repo: https://github.com/Mateusz-Grzelinski/actionlint-py
-    rev: v1.7.0.14
+    rev: v1.7.1.15
     hooks:
     -   id: actionlint
 -   repo: https://github.com/igorshubovych/markdownlint-cli
-    rev: v0.40.0
+    rev: v0.41.0
     hooks:
     -   id: markdownlint
+-   repo: https://github.com/Lucas-C/pre-commit-hooks-lxml
+    rev: v1.1.0
+    hooks:
+    -   id: forbid-html-img-without-alt-text
+    -   id: forbid-non-std-html-attributes
+    -   id: detect-missing-css-classes
+        args:
+        - --css-files-dir
+        - .
+        - --html-files-dir
+        - .
+    -   id: html-tags-blacklist
+    -   id: html-attributes-blacklist
```

### Comparing `acquiring-0.4.0/CHANGELOG.md` & `acquiring-0.4.1/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 Follows the format of [Common-Changelog](https://common-changelog.org)
 
+## 0.4.1 - 2024-06-03 [Alpha Release]
+
+### Added
+
+- Added package dependencies `deal` and `requests` explicitly in pyproject.toml (alvaro)
+
 ## 0.4.0 - 2024-06-01 [Alpha Release]
 
 ### Changed
 
 - Rename PaymentFlow as PaymentSaga (alvaro)
 - Implement PaymentOperation model in storage/sqlalchemy and its associated Repository (alvaro)
 - Ensure immutability of Wide events (Transaction, BlockEvent, PaymentOperation) (alvaro)
```

### Comparing `acquiring-0.4.0/Dockerfile` & `acquiring-0.4.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/LICENSE` & `acquiring-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/README.md` & `acquiring-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/acquiring/apps.py` & `acquiring-0.4.1/acquiring/apps.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/acquiring/contrib/paypal/adapter.py` & `acquiring-0.4.1/acquiring/contrib/paypal/adapter.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/acquiring/contrib/paypal/blocks/paypal_after_creating_order.py` & `acquiring-0.4.1/acquiring/contrib/paypal/blocks/paypal_after_creating_order.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/acquiring/contrib/paypal/blocks/paypal_create_order.py` & `acquiring-0.4.1/acquiring/contrib/paypal/blocks/paypal_create_order.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/acquiring/contrib/paypal/domain.py` & `acquiring-0.4.1/acquiring/contrib/paypal/domain.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/acquiring/domain/__init__.py` & `acquiring-0.4.1/acquiring/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/acquiring/domain/blocks.py` & `acquiring-0.4.1/acquiring/domain/blocks.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/acquiring/domain/decision_logic.py` & `acquiring-0.4.1/acquiring/domain/decision_logic.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/acquiring/domain/events.py` & `acquiring-0.4.1/acquiring/domain/events.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/acquiring/domain/payments.py` & `acquiring-0.4.1/acquiring/domain/payments.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/acquiring/domain/providers.py` & `acquiring-0.4.1/acquiring/domain/providers.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/acquiring/domain/sagas.py` & `acquiring-0.4.1/acquiring/domain/sagas.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/acquiring/enums.py` & `acquiring-0.4.1/acquiring/enums.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/acquiring/protocols/__init__.py` & `acquiring-0.4.1/acquiring/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/acquiring/protocols/payments.py` & `acquiring-0.4.1/acquiring/protocols/payments.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/acquiring/protocols/providers.py` & `acquiring-0.4.1/acquiring/protocols/providers.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/acquiring/protocols/storage.py` & `acquiring-0.4.1/acquiring/protocols/storage.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/acquiring/storage/django/migrations/0001_initial.py` & `acquiring-0.4.1/acquiring/storage/django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/acquiring/storage/django/models.py` & `acquiring-0.4.1/acquiring/storage/django/models.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/acquiring/storage/django/repositories.py` & `acquiring-0.4.1/acquiring/storage/django/repositories.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/acquiring/storage/django/unit_of_work.py` & `acquiring-0.4.1/acquiring/storage/django/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/acquiring/storage/sqlalchemy/migrations/env.py` & `acquiring-0.4.1/acquiring/storage/sqlalchemy/migrations/env.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/acquiring/storage/sqlalchemy/migrations/script.py.mako` & `acquiring-0.4.1/acquiring/storage/sqlalchemy/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/acquiring/storage/sqlalchemy/migrations/versions/87b793f35b89_add_acquiring_models.py` & `acquiring-0.4.1/acquiring/storage/sqlalchemy/migrations/versions/87b793f35b89_add_acquiring_models.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/acquiring/storage/sqlalchemy/models.py` & `acquiring-0.4.1/acquiring/storage/sqlalchemy/models.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/acquiring/storage/sqlalchemy/repositories.py` & `acquiring-0.4.1/acquiring/storage/sqlalchemy/repositories.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/acquiring/storage/sqlalchemy/unit_of_work.py` & `acquiring-0.4.1/acquiring/storage/sqlalchemy/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/alembic.ini` & `acquiring-0.4.1/alembic.ini`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/docker-compose.yaml` & `acquiring-0.4.1/docker-compose.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -31,12 +31,12 @@
     volumes:
       - .:/code
 
   docs:
     build:
       context: .
       dockerfile: docs/Dockerfile
-    command: mkdocs serve --dev-addr 0.0.0.0:8008
+    command: mkdocs serve --dev-addr 0.0.0.0:8008 --watch-theme
     volumes:
-      - ./docs:/app/docs
+      - .:/app
     ports:
       - 8008:8008
```

### Comparing `acquiring-0.4.0/docs/architecture/decisions/0002-use-tacit-tests.md` & `acquiring-0.4.1/docs/architecture/decisions/0002-use-tacit-tests.md`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/docs/architecture/decisions/0003-documentation-is-code.md` & `acquiring-0.4.1/docs/architecture/decisions/0003-documentation-is-code.md`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/docs/architecture/decisions/0004-reduce-doctests-to-a-minimum.md` & `acquiring-0.4.1/docs/architecture/decisions/0004-reduce-doctests-to-a-minimum.md`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/docs/architecture/decisions/0005-maybe-functions-considered-harmful.md` & `acquiring-0.4.1/docs/architecture/decisions/0005-maybe-functions-considered-harmful.md`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/docs/architecture/decisions/0006-use-import-module-more-often-than-from-module-import.md` & `acquiring-0.4.1/docs/architecture/decisions/0006-use-import-module-more-often-than-from-module-import.md`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/docs/architecture/decisions/0007-type-sparingly-but-with-confidence.md` & `acquiring-0.4.1/docs/architecture/decisions/0007-type-sparingly-but-with-confidence.md`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/docs/architecture/decisions/0008-domain-logic-happens-in-native-python.md` & `acquiring-0.4.1/docs/architecture/decisions/0008-domain-logic-happens-in-native-python.md`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/docs/architecture/decisions/0009-do-not-use-if-type-checking.md` & `acquiring-0.4.1/docs/architecture/decisions/0009-do-not-use-if-type-checking.md`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/docs/architecture/decisions/0010-exceptions-can-express-domain-concepts-too.md` & `acquiring-0.4.1/docs/architecture/decisions/0010-exceptions-can-express-domain-concepts-too.md`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/docs/architecture/decisions/0011-worse-is-better.md` & `acquiring-0.4.1/docs/architecture/decisions/0011-worse-is-better.md`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/docs/architecture/decisions/0013-separate-void-and-refund-operation-types.md` & `acquiring-0.4.1/docs/architecture/decisions/0013-separate-void-and-refund-operation-types.md`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/docs/architecture/decisions/0014-created-at-are-internal-datetimes-timestamps-are-external.md` & `acquiring-0.4.1/docs/architecture/decisions/0014-created-at-are-internal-datetimes-timestamps-are-external.md`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/docs/architecture/decisions/0015-the-elements-of-acquiring-architecture.md` & `acquiring-0.4.1/docs/architecture/decisions/0015-the-elements-of-acquiring-architecture.md`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/docs/architecture/index.md` & `acquiring-0.4.1/docs/architecture/index.md`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/docs/index.md` & `acquiring-0.4.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/manage.py` & `acquiring-0.4.1/manage.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/pyproject.toml` & `acquiring-0.4.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,18 @@
     "Typing :: Typed",
 ]
 dynamic = ["version", "description"]
 license = {file = "LICENSE"}
 name = "acquiring"
 readme = "README.md"
 requires-python = ">=3.8"
-long_description = {file = "README.md"}
+dependencies = [
+    "deal >3.2.0",
+    "requests",
+]
 
 [project.urls]
 Home = "https://github.com/acquiringlabs/acquiring"
 
 [project.optional-dependencies]
 django = ["django>=4.2"]
 sqlalchemy = ["sqlalchemy>=1.4"]
```

### Comparing `acquiring-0.4.0/requirements/development.txt` & `acquiring-0.4.1/requirements/development.txt`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/tests/conftest.py` & `acquiring-0.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/tests/contrib/paypal/blocks/test_paypal_after_creating_order.py` & `acquiring-0.4.1/tests/contrib/paypal/blocks/test_paypal_after_creating_order.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/tests/contrib/paypal/blocks/test_paypal_create_order.py` & `acquiring-0.4.1/tests/contrib/paypal/blocks/test_paypal_create_order.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/tests/contrib/paypal/test_adapter.py` & `acquiring-0.4.1/tests/contrib/paypal/test_adapter.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/tests/domain/blocks/test_wrapped_by_block_events.py` & `acquiring-0.4.1/tests/domain/blocks/test_wrapped_by_block_events.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/tests/domain/factories.py` & `acquiring-0.4.1/tests/domain/factories.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/tests/domain/flows/conftest.py` & `acquiring-0.4.1/tests/domain/flows/conftest.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/tests/domain/flows/test_after_confirm.py` & `acquiring-0.4.1/tests/domain/flows/test_after_confirm.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,14 @@
         after_confirm_blocks=[
             fake_block(  # type:ignore[call-arg]
                 fake_response_status=operation_status,
             ),
         ],
     ).after_confirm(payment_method)
 
-    # then the payment flow returns the correct Operation Response
     payment_operations = payment_method.payment_operations
     assert len(payment_operations) == 10
 
     assert payment_operations[0].type == OperationTypeEnum.INITIALIZE
     assert payment_operations[0].status == OperationStatusEnum.STARTED
 
     assert payment_operations[1].type == OperationTypeEnum.INITIALIZE
@@ -200,15 +199,15 @@
     ],
     fake_transaction_repository_class: Callable[
         [Optional[set[protocols.Transaction]]],
         type[test_protocols.FakeRepository],
     ],
     fake_unit_of_work: type[test_protocols.FakeUnitOfWork],
 ) -> None:
-    # Given a payment method that cannot initialize
+
     payment_attempt = factories.PaymentAttemptFactory()
     payment_method_id = uuid.uuid4()
     payment_method = factories.PaymentMethodFactory(
         payment_attempt=payment_attempt,
         id=payment_method_id,
         confirmable=False,
     )
@@ -225,11 +224,10 @@
         process_action_block=fake_process_action_block(),
         pay_blocks=[],
         after_pay_blocks=[],
         confirm_block=fake_block(),
         after_confirm_blocks=[],
     ).after_confirm(payment_method)
 
-    # then the payment flow returns a failed status operation response
     assert result.type == OperationTypeEnum.AFTER_CONFIRM
     assert result.status == OperationStatusEnum.FAILED
     result.error_message == "PaymentMethod cannot go through this operation"
```

### Comparing `acquiring-0.4.0/tests/domain/flows/test_after_pay.py` & `acquiring-0.4.1/tests/domain/flows/test_after_pay.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         [Optional[set[protocols.Transaction]]],
         type[test_protocols.FakeRepository],
     ],
     fake_unit_of_work: type[test_protocols.FakeUnitOfWork],
     operation_status: OperationStatusEnum,
     result_status: OperationStatusEnum,
 ) -> None:
-    # given a valid payment attempt
+
     payment_attempt = factories.PaymentAttemptFactory()
     payment_method_id = uuid.uuid4()
     payment_method = factories.PaymentMethodFactory(
         payment_attempt=payment_attempt,
         id=payment_method_id,
         confirmable=True,
         payment_operations=[
@@ -104,15 +104,14 @@
         after_pay_blocks=[
             fake_block(fake_response_status=operation_status)  # type:ignore[call-arg]
         ],
         confirm_block=None,
         after_confirm_blocks=[],
     ).after_pay(payment_method)
 
-    # then the payment flow returns the correct Operation Response
     payment_operations = payment_method.payment_operations
     assert len(payment_operations) == 6
 
     assert payment_operations[0].type == OperationTypeEnum.INITIALIZE
     assert payment_operations[0].status == OperationStatusEnum.STARTED
 
     assert payment_operations[1].type == OperationTypeEnum.INITIALIZE
@@ -157,15 +156,15 @@
     ],
     fake_transaction_repository_class: Callable[
         [Optional[set[protocols.Transaction]]],
         type[test_protocols.FakeRepository],
     ],
     fake_unit_of_work: type[test_protocols.FakeUnitOfWork],
 ) -> None:
-    # Given a payment method that cannot initialize
+
     payment_attempt = factories.PaymentAttemptFactory()
     payment_method_id = uuid.uuid4()
     payment_method = factories.PaymentMethodFactory(
         payment_attempt=payment_attempt,
         id=payment_method_id,
         confirmable=True,
         payment_operations=[
@@ -190,11 +189,10 @@
         process_action_block=fake_process_action_block(),
         pay_blocks=[],
         after_pay_blocks=[],
         confirm_block=None,
         after_confirm_blocks=[],
     ).after_pay(payment_method)
 
-    # then the payment flow returns a failed status operation response
     assert result.type == OperationTypeEnum.AFTER_PAY
     assert result.status == OperationStatusEnum.FAILED
     result.error_message == "PaymentMethod cannot go through this operation"
```

### Comparing `acquiring-0.4.0/tests/domain/flows/test_confirm.py` & `acquiring-0.4.1/tests/domain/flows/test_confirm.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         [Optional[set[protocols.Transaction]]],
         type[test_protocols.FakeRepository],
     ],
     result_status: OperationStatusEnum,
     operation_status: OperationStatusEnum,
     fake_unit_of_work: type[test_protocols.FakeUnitOfWork],
 ) -> None:
-    # given a valid payment attempt
+
     payment_attempt = factories.PaymentAttemptFactory()
     payment_method_id = uuid.uuid4()
     payment_method = factories.PaymentMethodFactory(
         payment_attempt=payment_attempt,
         id=payment_method_id,
         confirmable=True,
         payment_operations=[
@@ -119,15 +119,14 @@
         process_action_block=fake_process_action_block(),
         pay_blocks=[],
         after_pay_blocks=[],
         confirm_block=fake_block(fake_response_status=operation_status),  # type:ignore[call-arg]
         after_confirm_blocks=[],
     ).confirm(payment_method)
 
-    # then the payment flow returns the correct Operation Response
     payment_operations = payment_method.payment_operations
     assert len(payment_operations) == 8
 
     assert payment_operations[0].type == OperationTypeEnum.INITIALIZE
     assert payment_operations[0].status == OperationStatusEnum.STARTED
 
     assert payment_operations[1].type == OperationTypeEnum.INITIALIZE
@@ -178,15 +177,15 @@
     ],
     fake_transaction_repository_class: Callable[
         [Optional[set[protocols.Transaction]]],
         type[test_protocols.FakeRepository],
     ],
     fake_unit_of_work: type[test_protocols.FakeUnitOfWork],
 ) -> None:
-    # Given a payment method that cannot initialize
+
     payment_attempt = factories.PaymentAttemptFactory()
     payment_method_id = uuid.uuid4()
     payment_method = factories.PaymentMethodFactory(
         payment_attempt=payment_attempt, id=payment_method_id, confirmable=False
     )
     assert dl.can_confirm(payment_method) is False
 
@@ -201,11 +200,10 @@
         process_action_block=fake_process_action_block(),
         pay_blocks=[],
         after_pay_blocks=[],
         confirm_block=fake_block(),
         after_confirm_blocks=[],
     ).confirm(payment_method)
 
-    # then the payment flow returns a failed status operation response
     assert result.type == OperationTypeEnum.CONFIRM
     assert result.status == OperationStatusEnum.FAILED
     result.error_message == "PaymentMethod cannot go through this operation"
```

### Comparing `acquiring-0.4.0/tests/domain/flows/test_define_payment_flow.py` & `acquiring-0.4.1/tests/domain/flows/test_define_payment_flow.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/tests/domain/flows/test_initialize.py` & `acquiring-0.4.1/tests/domain/flows/test_initialize.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,23 +55,22 @@
         [Optional[set[protocols.Transaction]]],
         type[test_protocols.FakeRepository],
     ],
     block_response_actions: list[dict],
     payment_operations_status: OperationStatusEnum,
     fake_unit_of_work: type[test_protocols.FakeUnitOfWork],
 ) -> None:
-    # given a valid payment attempt
+
     payment_attempt = factories.PaymentAttemptFactory()
     payment_method_id = uuid.uuid4()
     payment_method = factories.PaymentMethodFactory(
         payment_attempt=payment_attempt,
         id=payment_method_id,
     )
 
-    # when Initializing
     unit_of_work = fake_unit_of_work(
         payment_method_repository_class=fake_payment_method_repository_class([payment_method]),
         payment_operation_repository_class=fake_payment_operation_repository_class(
             set(payment_method.payment_operations)
         ),
         block_event_repository_class=fake_block_event_repository_class(set()),
         transaction_repository_class=fake_transaction_repository_class(set()),
@@ -86,15 +85,14 @@
         process_action_block=fake_process_action_block(),
         pay_blocks=[],
         after_pay_blocks=[],
         confirm_block=None,
         after_confirm_blocks=[],
     ).initialize(payment_method)
 
-    # then the payment flow returns the correct Operation Response
     payment_operations = payment_method.payment_operations
     assert len(payment_operations) == 2
 
     assert payment_operations[0].type == OperationTypeEnum.INITIALIZE
     assert payment_operations[0].status == OperationStatusEnum.STARTED
 
     assert payment_operations[1].type == OperationTypeEnum.INITIALIZE
@@ -139,23 +137,22 @@
     fake_transaction_repository_class: Callable[
         [Optional[set[protocols.Transaction]]],
         type[test_protocols.FakeRepository],
     ],
     fake_unit_of_work: type[test_protocols.FakeUnitOfWork],
     payment_operations_status: OperationStatusEnum,
 ) -> None:
-    # given a valid payment attempt
+
     payment_attempt = factories.PaymentAttemptFactory()
     payment_method_id = uuid.uuid4()
     payment_method = factories.PaymentMethodFactory(
         payment_attempt=payment_attempt,
         id=payment_method_id,
     )
 
-    # when Initializing
     unit_of_work = fake_unit_of_work(
         payment_method_repository_class=fake_payment_method_repository_class([payment_method]),
         payment_operation_repository_class=fake_payment_operation_repository_class(
             set(payment_method.payment_operations)
         ),
         block_event_repository_class=fake_block_event_repository_class(set()),
         transaction_repository_class=fake_transaction_repository_class(set()),
@@ -174,15 +171,14 @@
         process_action_block=fake_process_action_block(),
         pay_blocks=[],
         after_pay_blocks=[],
         confirm_block=None,
         after_confirm_blocks=[],
     ).initialize(payment_method)
 
-    # then the payment flow returns the correct Operation Response
     payment_operations = payment_method.payment_operations
     assert len(payment_operations) == 4
 
     assert payment_operations[0].type == OperationTypeEnum.INITIALIZE
     assert payment_operations[0].status == OperationStatusEnum.STARTED
 
     assert payment_operations[1].type == OperationTypeEnum.INITIALIZE
@@ -221,15 +217,15 @@
     ],
     fake_transaction_repository_class: Callable[
         [Optional[set[protocols.Transaction]]],
         type[test_protocols.FakeRepository],
     ],
     fake_unit_of_work: type[test_protocols.FakeUnitOfWork],
 ) -> None:
-    # Given a payment method that cannot initialize
+
     payment_attempt = factories.PaymentAttemptFactory()
     payment_method_id = uuid.uuid4()
     payment_method = factories.PaymentMethodFactory(
         payment_attempt=payment_attempt,
         id=payment_method_id,
         payment_operations=[
             domain.PaymentOperation(
@@ -256,11 +252,10 @@
         process_action_block=fake_process_action_block(),
         pay_blocks=[],
         after_pay_blocks=[],
         confirm_block=None,
         after_confirm_blocks=[],
     ).initialize(payment_method)
 
-    # then the payment flow returns a failed status operation response
     assert result.type == OperationTypeEnum.INITIALIZE
     assert result.status == OperationStatusEnum.FAILED
     result.error_message == "PaymentMethod cannot go through this operation"
```

### Comparing `acquiring-0.4.0/tests/domain/flows/test_pay.py` & `acquiring-0.4.1/tests/domain/flows/test_pay.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         [Optional[set[protocols.Transaction]]],
         type[test_protocols.FakeRepository],
     ],
     fake_unit_of_work: type[test_protocols.FakeUnitOfWork],
     result_status: OperationStatusEnum,
     operation_status: OperationStatusEnum,
 ) -> None:
-    # given a valid payment attempt
+
     payment_attempt = factories.PaymentAttemptFactory()
     payment_method_id = uuid.uuid4()
     payment_method = factories.PaymentMethodFactory(
         payment_attempt=payment_attempt,
         id=payment_method_id,
     )
 
@@ -79,15 +79,14 @@
             fake_block(fake_response_status=operation_status)  # type:ignore[call-arg]
         ],
         after_pay_blocks=[],
         confirm_block=None,
         after_confirm_blocks=[],
     ).initialize(payment_method)
 
-    # then the payment flow returns the correct Operation Response
     payment_operations = payment_method.payment_operations
     assert len(payment_operations) == 4
 
     assert payment_operations[0].type == OperationTypeEnum.INITIALIZE
     assert payment_operations[0].status == OperationStatusEnum.STARTED
 
     assert payment_operations[1].type == OperationTypeEnum.INITIALIZE
@@ -126,24 +125,23 @@
     ],
     fake_transaction_repository_class: Callable[
         [Optional[set[protocols.Transaction]]],
         type[test_protocols.FakeRepository],
     ],
     fake_unit_of_work: type[test_protocols.FakeUnitOfWork],
 ) -> None:
-    # given a valid payment attempt
+
     payment_attempt = factories.PaymentAttemptFactory()
     payment_method_id = uuid.uuid4()
     payment_method = factories.PaymentMethodFactory(
         payment_attempt=payment_attempt,
         id=payment_method_id,
     )
     action = {"test": "action"}
 
-    # when Initializing
     unit_of_work = fake_unit_of_work(
         payment_method_repository_class=fake_payment_method_repository_class([payment_method]),
         payment_operation_repository_class=fake_payment_operation_repository_class(
             set(payment_method.payment_operations)
         ),
         block_event_repository_class=fake_block_event_repository_class(set()),
         transaction_repository_class=fake_transaction_repository_class(set()),
@@ -162,15 +160,14 @@
             )
         ],
         after_pay_blocks=[],
         confirm_block=None,
         after_confirm_blocks=[],
     ).initialize(payment_method)
 
-    # then the payment flow returns the correct Operation Response
     payment_operations = payment_method.payment_operations
     assert len(payment_operations) == 4
 
     assert payment_operations[0].type == OperationTypeEnum.INITIALIZE
     assert payment_operations[0].status == OperationStatusEnum.STARTED
 
     assert payment_operations[1].type == OperationTypeEnum.INITIALIZE
```

### Comparing `acquiring-0.4.0/tests/domain/flows/test_process_actions.py` & `acquiring-0.4.1/tests/domain/flows/test_process_actions.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     ],
     fake_transaction_repository_class: Callable[
         [Optional[set[protocols.Transaction]]],
         type[test_protocols.FakeRepository],
     ],
     fake_unit_of_work: type[test_protocols.FakeUnitOfWork],
 ) -> None:
-    # given a valid payment attempt
+
     payment_attempt = factories.PaymentAttemptFactory()
     payment_method_id = uuid.uuid4()
     payment_method = factories.PaymentMethodFactory(
         payment_attempt=payment_attempt,
         id=payment_method_id,
         confirmable=True,
         payment_operations=[
@@ -68,15 +68,14 @@
         ),
         pay_blocks=[],
         after_pay_blocks=[],
         confirm_block=None,
         after_confirm_blocks=[],
     ).process_action(payment_method, action_data={})
 
-    # then the payment flow returns a failed status Operation Response
     assert result.type == OperationTypeEnum.PROCESS_ACTION
     assert result.status == OperationStatusEnum.FAILED
 
     assert result.payment_method is not None
     assert result.payment_method.id == payment_method.id
 
     payment_operations = payment_method.payment_operations
@@ -115,15 +114,15 @@
     ],
     fake_transaction_repository_class: Callable[
         [Optional[set[protocols.Transaction]]],
         type[test_protocols.FakeRepository],
     ],
     fake_unit_of_work: type[test_protocols.FakeUnitOfWork],
 ) -> None:
-    # given a valid payment attempt
+
     payment_attempt = factories.PaymentAttemptFactory()
     payment_method_id = uuid.uuid4()
     payment_method = factories.PaymentMethodFactory(
         payment_attempt=payment_attempt,
         id=payment_method_id,
         confirmable=True,
         payment_operations=[
@@ -156,15 +155,14 @@
         ),  # type:ignore[call-arg]
         pay_blocks=[fake_block(fake_response_status=OperationStatusEnum.COMPLETED)],  # type:ignore[call-arg]
         after_pay_blocks=[],
         confirm_block=None,
         after_confirm_blocks=[],
     ).process_action(payment_method, action_data={})
 
-    # then the payment flow returns a failed status Operation Response
     assert result.type == OperationTypeEnum.PAY
     assert result.status == OperationStatusEnum.COMPLETED
 
     assert result.payment_method is not None
     assert result.payment_method.id == payment_method.id
 
     payment_operations = payment_method.payment_operations
@@ -208,15 +206,15 @@
     ],
     fake_transaction_repository_class: Callable[
         [Optional[set[protocols.Transaction]]],
         type[test_protocols.FakeRepository],
     ],
     fake_unit_of_work: type[test_protocols.FakeUnitOfWork],
 ) -> None:
-    # given a valid payment attempt
+
     payment_attempt = factories.PaymentAttemptFactory()
     payment_method_id = uuid.uuid4()
     payment_method = factories.PaymentMethodFactory(
         payment_attempt=payment_attempt,
         id=payment_method_id,
         confirmable=True,
         payment_operations=[
@@ -247,15 +245,14 @@
         process_action_block=None,  # not present
         pay_blocks=[],
         after_pay_blocks=[],
         confirm_block=None,
         after_confirm_blocks=[],
     ).process_action(payment_method, action_data={})
 
-    # then the payment flow returns a failed status Operation Response
     assert result.type == OperationTypeEnum.PROCESS_ACTION
     assert result.status == OperationStatusEnum.NOT_PERFORMED
 
     assert result.payment_method is not None
     assert result.payment_method.id == payment_method.id
 
     payment_operations = payment_method.payment_operations
@@ -294,15 +291,15 @@
     ],
     fake_transaction_repository_class: Callable[
         [Optional[set[protocols.Transaction]]],
         type[test_protocols.FakeRepository],
     ],
     fake_unit_of_work: type[test_protocols.FakeUnitOfWork],
 ) -> None:
-    # Given a payment method that cannot initialize
+
     payment_attempt = factories.PaymentAttemptFactory()
     payment_method_id = uuid.uuid4()
     payment_method = factories.PaymentMethodFactory(
         payment_attempt=payment_attempt,
         id=payment_method_id,
         confirmable=True,
         payment_operations=[
@@ -330,11 +327,10 @@
         ),  # type:ignore[call-arg]
         pay_blocks=[],
         after_pay_blocks=[],
         confirm_block=None,
         after_confirm_blocks=[],
     ).process_action(payment_method, action_data={})
 
-    # then the payment flow returns a failed status operation response
     assert result.type == OperationTypeEnum.PROCESS_ACTION
     assert result.status == OperationStatusEnum.FAILED
     result.error_message == "PaymentMethod cannot go through this operation"
```

### Comparing `acquiring-0.4.0/tests/domain/flows/test_refresh_payment_method.py` & `acquiring-0.4.1/tests/domain/flows/test_refresh_payment_method.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/tests/domain/providers/test_wrapped_by_transaction.py` & `acquiring-0.4.1/tests/domain/providers/test_wrapped_by_transaction.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/tests/domain/test_decision_logic.py` & `acquiring-0.4.1/tests/domain/test_decision_logic.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/tests/protocols.py` & `acquiring-0.4.1/tests/protocols.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/tests/storage/django/factories.py` & `acquiring-0.4.1/tests/storage/django/factories.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/tests/storage/django/repositories/test_block_event_repository.py` & `acquiring-0.4.1/tests/storage/django/repositories/test_block_event_repository.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/tests/storage/django/repositories/test_payment_method_repository.py` & `acquiring-0.4.1/tests/storage/django/repositories/test_payment_method_repository.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/tests/storage/django/repositories/test_payment_operation_repository.py` & `acquiring-0.4.1/tests/storage/django/repositories/test_payment_operation_repository.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,29 +16,26 @@
 @pytest.mark.parametrize(
     "operation_type, operation_status", product(enums.OperationTypeEnum, enums.OperationStatusEnum)
 )
 def test_givenExistingPaymentMethodRow_whenCallingRepositoryAdd_thenPaymentOperationGetsCreated(
     operation_type: enums.OperationTypeEnum,
     operation_status: enums.OperationStatusEnum,
 ) -> None:
-    # Given existing payment method row in payment methods table
+
     db_payment_attempt = PaymentAttemptFactory()
     db_payment_method = PaymentMethodFactory(payment_attempt_id=db_payment_attempt.id)
     payment_method = db_payment_method.to_domain()
 
-    # When calling PaymentOperationRepository.add_payment_operation
     storage.django.PaymentOperationRepository().add(
         payment_method=payment_method,
         type=operation_type,
         status=operation_status,
     )
 
-    # Then PaymentOperation gets created
     payment_operation = storage.django.models.PaymentOperation.objects.get(
         payment_method_id=db_payment_method.id,
         status=operation_status,
         type=operation_type,
     )
 
-    # And payment method gets the payment operation added after add_payment_operation
     assert len(payment_method.payment_operations) == 1
     assert payment_method.payment_operations[0] == payment_operation.to_domain()
```

### Comparing `acquiring-0.4.0/tests/storage/django/repositories/test_token_repository.py` & `acquiring-0.4.1/tests/storage/django/repositories/test_token_repository.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/tests/storage/django/repositories/test_transaction_repository.py` & `acquiring-0.4.1/tests/storage/django/repositories/test_transaction_repository.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/tests/storage/django/repositories/test_unit_of_work.py` & `acquiring-0.4.1/tests/storage/django/repositories/test_unit_of_work.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/tests/storage/django/test_migrations.py` & `acquiring-0.4.1/tests/storage/django/test_migrations.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/tests/storage/django/test_models.py` & `acquiring-0.4.1/tests/storage/django/test_models.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/tests/storage/sqlalchemy/conftest.py` & `acquiring-0.4.1/tests/storage/sqlalchemy/conftest.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/tests/storage/sqlalchemy/factories.py` & `acquiring-0.4.1/tests/storage/sqlalchemy/factories.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/tests/storage/sqlalchemy/repositories/test_payment_method_repository.py` & `acquiring-0.4.1/tests/storage/sqlalchemy/repositories/test_payment_method_repository.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/tests/storage/sqlalchemy/repositories/test_payment_operation_repository.py` & `acquiring-0.4.1/tests/storage/sqlalchemy/repositories/test_payment_operation_repository.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 def test_givenCorrectData_whenCallingRepositoryAdd_thenPaymentOperationGetsCreated(
     session: "orm.Session",
     sqlalchemy_assert_num_queries: Callable,
     operation_type: enums.OperationTypeEnum,
     operation_status: enums.OperationStatusEnum,
 ) -> None:
 
-    # Given existing payment method row in payment methods table
     db_payment_attempt = factories.PaymentAttemptFactory()
     db_payment_method = factories.PaymentMethodFactory(payment_attempt_id=db_payment_attempt.id)
     payment_method = db_payment_method.to_domain()
 
     with sqlalchemy_assert_num_queries(5):
         result = storage.sqlalchemy.PaymentOperationRepository(session=session).add(
             payment_method=payment_method,
```

### Comparing `acquiring-0.4.0/tests/storage/sqlalchemy/repositories/test_unit_of_work.py` & `acquiring-0.4.1/tests/storage/sqlalchemy/repositories/test_unit_of_work.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/tests/storage/test_tacit.py` & `acquiring-0.4.1/tests/storage/test_tacit.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/tests/tacit/test_files.py` & `acquiring-0.4.1/tests/tacit/test_files.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/tox.ini` & `acquiring-0.4.1/tox.ini`

 * *Files identical despite different names*

### Comparing `acquiring-0.4.0/PKG-INFO` & `acquiring-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acquiring
-Version: 0.4.0
+Version: 0.4.1
 Summary: Payment Orchestration Library for Python
 Author-email: Alvaro Duran <alvaro.duranb@hotmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -13,14 +13,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Office/Business :: Financial :: Point-Of-Sale
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
+Requires-Dist: deal >3.2.0
+Requires-Dist: requests
 Requires-Dist: django>=4.2 ; extra == "django"
 Requires-Dist: sqlalchemy>=1.4 ; extra == "sqlalchemy"
 Project-URL: Home, https://github.com/acquiringlabs/acquiring
 Provides-Extra: django
 Provides-Extra: sqlalchemy
 
 # Acquiring
```

