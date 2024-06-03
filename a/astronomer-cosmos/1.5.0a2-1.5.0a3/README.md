# Comparing `tmp/astronomer_cosmos-1.5.0a2.tar.gz` & `tmp/astronomer_cosmos-1.5.0a3.tar.gz`

## Comparing `astronomer_cosmos-1.5.0a2.tar` & `astronomer_cosmos-1.5.0a3.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/__init__.py
--rw-r--r--   0        0        0    10978 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/cache.py
--rw-r--r--   0        0        0    15300 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/config.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/constants.py
--rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/converter.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/exceptions.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/log.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/airflow/__init__.py
--rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/airflow/dag.py
--rw-r--r--   0        0        0    13398 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/airflow/graph.py
--rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/airflow/task_group.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/core/__init__.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/core/airflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/core/graph/__init__.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/core/graph/entities.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/dbt/__init__.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/dbt/executable.py
--rw-r--r--   0        0        0    18591 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/dbt/graph.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/dbt/project.py
--rw-r--r--   0        0        0    17017 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/dbt/selector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/dbt/parser/__init__.py
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/dbt/parser/output.py
--rw-r--r--   0        0        0    16190 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/dbt/parser/project.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/hooks/__init__.py
--rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/hooks/subprocess.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/operators/__init__.py
--rw-r--r--   0        0        0     4000 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/operators/aws_eks.py
--rw-r--r--   0        0        0     4949 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/operators/azure_container_instance.py
--rw-r--r--   0        0        0    15005 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/operators/base.py
--rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/operators/docker.py
--rw-r--r--   0        0        0     9450 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/operators/kubernetes.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/operators/lazy_load.py
--rw-r--r--   0        0        0    33470 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/operators/local.py
--rw-r--r--   0        0        0     6282 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/operators/virtualenv.py
--rw-r--r--   0        0        0     6843 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/plugin/__init__.py
--rw-r--r--   0        0        0    13431 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/plugin/static/iframeResizer.contentWindow.min.js
--rw-r--r--   0        0        0    14167 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/plugin/static/iframeResizer.min.js
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/plugin/templates/dbt_docs.html
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/plugin/templates/dbt_docs_not_set_up.html
--rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/profiles/__init__.py
--rwxr-xr-x   0        0        0    11466 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/profiles/base.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/profiles/athena/__init__.py
--rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/profiles/athena/access_key.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/profiles/bigquery/__init__.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/profiles/bigquery/oauth.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/profiles/bigquery/service_account_file.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/profiles/bigquery/service_account_keyfile_dict.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/profiles/databricks/__init__.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/profiles/databricks/token.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/profiles/exasol/__init__.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/profiles/exasol/user_pass.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/profiles/postgres/__init__.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/profiles/postgres/user_pass.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/profiles/redshift/__init__.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/profiles/redshift/user_pass.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/profiles/snowflake/__init__.py
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/profiles/snowflake/user_encrypted_privatekey_env_variable.py
--rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/profiles/snowflake/user_encrypted_privatekey_file.py
--rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/profiles/snowflake/user_pass.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/profiles/snowflake/user_privatekey.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/profiles/spark/__init__.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/profiles/spark/thrift.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/profiles/trino/__init__.py
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/profiles/trino/base.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/profiles/trino/certificate.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/profiles/trino/jwt.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/profiles/trino/ldap.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/profiles/vertica/__init__.py
--rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/cosmos/profiles/vertica/user_pass.py
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/LICENSE
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/README.rst
--rw-r--r--   0        0        0     6180 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/pyproject.toml
--rw-r--r--   0        0        0     7853 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a2/PKG-INFO
+-rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/__init__.py
+-rw-r--r--   0        0        0     7542 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/cache.py
+-rw-r--r--   0        0        0    15300 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/config.py
+-rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/constants.py
+-rw-r--r--   0        0        0    12871 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/converter.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/exceptions.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/log.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/airflow/__init__.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/airflow/dag.py
+-rw-r--r--   0        0        0    13398 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/airflow/graph.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/airflow/task_group.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/core/__init__.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/core/airflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/core/graph/__init__.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/core/graph/entities.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/dbt/__init__.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/dbt/executable.py
+-rw-r--r--   0        0        0    20143 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/dbt/graph.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/dbt/project.py
+-rw-r--r--   0        0        0    17017 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/dbt/selector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/dbt/parser/__init__.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/dbt/parser/output.py
+-rw-r--r--   0        0        0    16190 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/dbt/parser/project.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/hooks/__init__.py
+-rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/hooks/subprocess.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/operators/__init__.py
+-rw-r--r--   0        0        0     4000 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/operators/aws_eks.py
+-rw-r--r--   0        0        0     4949 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/operators/azure_container_instance.py
+-rw-r--r--   0        0        0    15005 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/operators/base.py
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/operators/docker.py
+-rw-r--r--   0        0        0     9450 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/operators/kubernetes.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/operators/lazy_load.py
+-rw-r--r--   0        0        0    33448 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/operators/local.py
+-rw-r--r--   0        0        0     6282 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/operators/virtualenv.py
+-rw-r--r--   0        0        0     6843 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/plugin/__init__.py
+-rw-r--r--   0        0        0    13431 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/plugin/static/iframeResizer.contentWindow.min.js
+-rw-r--r--   0        0        0    14167 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/plugin/static/iframeResizer.min.js
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/plugin/templates/dbt_docs.html
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/plugin/templates/dbt_docs_not_set_up.html
+-rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/profiles/__init__.py
+-rwxr-xr-x   0        0        0    11466 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/profiles/base.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/profiles/athena/__init__.py
+-rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/profiles/athena/access_key.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/profiles/bigquery/__init__.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/profiles/bigquery/oauth.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/profiles/bigquery/service_account_file.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/profiles/bigquery/service_account_keyfile_dict.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/profiles/databricks/__init__.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/profiles/databricks/token.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/profiles/exasol/__init__.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/profiles/exasol/user_pass.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/profiles/postgres/__init__.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/profiles/postgres/user_pass.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/profiles/redshift/__init__.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/profiles/redshift/user_pass.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/profiles/snowflake/__init__.py
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/profiles/snowflake/user_encrypted_privatekey_env_variable.py
+-rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/profiles/snowflake/user_encrypted_privatekey_file.py
+-rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/profiles/snowflake/user_pass.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/profiles/snowflake/user_privatekey.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/profiles/spark/__init__.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/profiles/spark/thrift.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/profiles/trino/__init__.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/profiles/trino/base.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/profiles/trino/certificate.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/profiles/trino/jwt.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/profiles/trino/ldap.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/profiles/vertica/__init__.py
+-rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/cosmos/profiles/vertica/user_pass.py
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/LICENSE
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/README.rst
+-rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/pyproject.toml
+-rw-r--r--   0        0        0     7869 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a3/PKG-INFO
```

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/__init__.py` & `astronomer_cosmos-1.5.0a3/cosmos/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # type: ignore # ignores "Cannot assign to a type" MyPy error
 
 """
 Astronomer Cosmos is a library for rendering dbt workflows in Airflow.
 
 Contains dags, task groups, and operators.
 """
-__version__ = "1.5.0a2"
+__version__ = "1.5.0a3"
 
 
 from cosmos.airflow.dag import DbtDag
 from cosmos.airflow.task_group import DbtTaskGroup
 from cosmos.config import (
     ExecutionConfig,
     ProfileConfig,
```

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/config.py` & `astronomer_cosmos-1.5.0a3/cosmos/config.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/constants.py` & `astronomer_cosmos-1.5.0a3/cosmos/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     Supported ways to load a `dbt` project into a `DbtGraph` instance.
     """
 
     AUTOMATIC = "automatic"
     CUSTOM = "custom"
     DBT_LS = "dbt_ls"
     DBT_LS_FILE = "dbt_ls_file"
+    DBT_LS_CACHE = "dbt_ls_cache"
     DBT_MANIFEST = "dbt_manifest"
 
 
 class TestBehavior(Enum):
     """
     Behavior of the tests.
     """
```

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/converter.py` & `astronomer_cosmos-1.5.0a3/cosmos/converter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # mypy: ignore-errors
 # ignoring enum Mypy errors
 
 from __future__ import annotations
 
 import copy
 import inspect
+import os
+import platform
+import time
 from typing import Any, Callable
 from warnings import warn
 
 from airflow.models.dag import DAG
 from airflow.utils.task_group import TaskGroup
 
 from cosmos import cache, settings
@@ -222,26 +225,36 @@
         validate_adapted_user_config(execution_config, project_config, render_config)
 
         env_vars = project_config.env_vars or operator_args.get("env")
         dbt_vars = project_config.dbt_vars or operator_args.get("vars")
 
         cache_dir = None
         if settings.enable_cache:
-            cache_dir = cache._obtain_cache_dir_path(cache_identifier=cache._create_cache_identifier(dag, task_group))
+            cache_identifier = cache._create_cache_identifier(dag, task_group)
+            cache_dir = cache._obtain_cache_dir_path(cache_identifier=cache_identifier)
 
+        previous_time = time.process_time()
         self.dbt_graph = DbtGraph(
             project=project_config,
             render_config=render_config,
             execution_config=execution_config,
             profile_config=profile_config,
             cache_dir=cache_dir,
+            cache_identifier=cache_identifier,
             dbt_vars=dbt_vars,
         )
         self.dbt_graph.load(method=render_config.load_method, execution_mode=execution_config.execution_mode)
 
+        current_time = time.process_time()
+        elapsed_time = current_time - previous_time
+        logger.info(
+            f"Cosmos performance [{platform.node()}|{os.getpid()}]: It took {elapsed_time:.3}s to parse the dbt project for DAG {dag.dag_id} using {self.dbt_graph.load_method}"
+        )
+        previous_time = current_time
+
         task_args = {
             **operator_args,
             "project_dir": execution_config.project_path,
             "partial_parse": project_config.partial_parse,
             "profile_config": profile_config,
             "emit_datasets": render_config.emit_datasets,
             "env": env_vars,
@@ -268,7 +281,13 @@
             execution_mode=execution_config.execution_mode,
             task_args=task_args,
             test_indirect_selection=execution_config.test_indirect_selection,
             dbt_project_name=project_config.project_name,
             on_warning_callback=on_warning_callback,
             render_config=render_config,
         )
+
+        current_time = time.process_time()
+        elapsed_time = current_time - previous_time
+        logger.info(
+            f"Cosmos performance [{platform.node()}|{os.getpid()}]: It took {elapsed_time:.3}s to build the Airflow DAG {dag.dag_id}."
+        )
```

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/log.py` & `astronomer_cosmos-1.5.0a3/cosmos/log.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/settings.py` & `astronomer_cosmos-1.5.0a3/cosmos/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from airflow.configuration import conf
 
 from cosmos.constants import DEFAULT_COSMOS_CACHE_DIR_NAME, DEFAULT_OPENLINEAGE_NAMESPACE
 
 # In MacOS users may want to set the envvar `TMPDIR` if they do not want the value of the temp directory to change
 DEFAULT_CACHE_DIR = Path(tempfile.gettempdir(), DEFAULT_COSMOS_CACHE_DIR_NAME)
 cache_dir = Path(conf.get("cosmos", "cache_dir", fallback=DEFAULT_CACHE_DIR) or DEFAULT_CACHE_DIR)
-
 enable_cache = conf.getboolean("cosmos", "enable_cache", fallback=True)
 experimental_cache = conf.getboolean("cosmos", "experimental_cache", fallback=False)
 propagate_logs = conf.getboolean("cosmos", "propagate_logs", fallback=True)
 dbt_docs_dir = conf.get("cosmos", "dbt_docs_dir", fallback=None)
 dbt_docs_conn_id = conf.get("cosmos", "dbt_docs_conn_id", fallback=None)
 
 try:
```

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/airflow/graph.py` & `astronomer_cosmos-1.5.0a3/cosmos/airflow/graph.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/core/airflow.py` & `astronomer_cosmos-1.5.0a3/cosmos/core/airflow.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/core/graph/entities.py` & `astronomer_cosmos-1.5.0a3/cosmos/core/graph/entities.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/dbt/graph.py` & `astronomer_cosmos-1.5.0a3/cosmos/dbt/graph.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from __future__ import annotations
 
 import itertools
 import json
 import os
+import platform
 import tempfile
 from dataclasses import dataclass, field
 from pathlib import Path
 from subprocess import PIPE, Popen
 from typing import Any
 
 import yaml
+from airflow.models import Variable
 
-from cosmos import cache
+from cosmos import cache, settings
 from cosmos.config import ExecutionConfig, ProfileConfig, ProjectConfig, RenderConfig
 from cosmos.constants import (
     DBT_LOG_DIR_NAME,
     DBT_LOG_FILENAME,
     DBT_LOG_PATH_ENVVAR,
     DBT_TARGET_DIR_NAME,
     DBT_TARGET_PATH_ENVVAR,
@@ -94,15 +96,15 @@
     if returncode or "Error" in stdout.replace("WarnErrorOptions", ""):
         details = stderr or stdout
         raise CosmosLoadDbtException(f"Unable to run {command} due to the error:\n{details}")
 
     return stdout
 
 
-def parse_dbt_ls_output(project_path: Path, ls_stdout: str) -> dict[str, DbtNode]:
+def parse_dbt_ls_output(project_path: Path | None, ls_stdout: str) -> dict[str, DbtNode]:
     """Parses the output of `dbt ls` into a dictionary of `DbtNode` instances."""
     nodes = {}
     for line in ls_stdout.split("\n"):
         try:
             node_dict = json.loads(line.strip())
         except json.decoder.JSONDecodeError:
             logger.debug("Skipped dbt ls line: %s", line)
@@ -126,30 +128,33 @@
     Supports different ways of loading the `dbt` project into this representation.
 
     Different loading methods can result in different `nodes` and `filtered_nodes`.
     """
 
     nodes: dict[str, DbtNode] = dict()
     filtered_nodes: dict[str, DbtNode] = dict()
+    load_method: LoadMode = LoadMode.AUTOMATIC
 
     def __init__(
         self,
         project: ProjectConfig,
         render_config: RenderConfig = RenderConfig(),
         execution_config: ExecutionConfig = ExecutionConfig(),
         profile_config: ProfileConfig | None = None,
         cache_dir: Path | None = None,
+        cache_identifier: str = "UNDEFINED",
         # dbt_vars only supported for LegacyDbtProject
         dbt_vars: dict[str, str] | None = None,
     ):
         self.project = project
         self.render_config = render_config
         self.profile_config = profile_config
         self.execution_config = execution_config
         self.cache_dir = cache_dir
+        self.cache_identifier = cache_identifier
         self.dbt_vars = dbt_vars or {}
 
     def load(
         self,
         method: LoadMode = LoadMode.AUTOMATIC,
         execution_mode: ExecutionMode = ExecutionMode.LOCAL,
     ) -> None:
@@ -159,41 +164,61 @@
         :param method: How to load `nodes` from a `dbt` project (automatically, using custom parser, using dbt manifest
             or dbt ls)
         :param execution_mode: Where Cosmos should run each dbt task (e.g. ExecutionMode.KUBERNETES)
 
         Fundamentally, there are two different execution paths
         There is automatic, and manual.
         """
-
         load_method = {
             LoadMode.CUSTOM: self.load_via_custom_parser,
             LoadMode.DBT_LS: self.load_via_dbt_ls,
             LoadMode.DBT_LS_FILE: self.load_via_dbt_ls_file,
+            LoadMode.DBT_LS_CACHE: self.load_via_dbt_ls_cache,
             LoadMode.DBT_MANIFEST: self.load_from_dbt_manifest,
         }
 
         if method == LoadMode.AUTOMATIC:
             if self.project.is_manifest_available():
                 self.load_from_dbt_manifest()
             else:
                 if execution_mode == ExecutionMode.LOCAL and self.profile_config:
                     try:
-                        self.load_via_dbt_ls()
+                        if not self.load_via_dbt_ls_cache():
+                            self.load_via_dbt_ls()
                     except FileNotFoundError:
                         self.load_via_custom_parser()
                 else:
                     self.load_via_custom_parser()
         else:
             load_method[method]()
 
         self.update_node_dependency()
 
         logger.info("Total nodes: %i", len(self.nodes))
         logger.info("Total filtered nodes: %i", len(self.nodes))
 
+    def load_via_dbt_ls_cache(self) -> bool:
+        """
+        Load dbt ls cache
+        """
+        logger.info(f"Trying to parse the dbt project using dbt ls cache {self.cache_identifier}...")
+        if settings.enable_cache and settings.experimental_cache:
+            dbt_ls_cache = Variable.get(self.cache_identifier, "")
+            if dbt_ls_cache:
+                logger.info(
+                    f"Cosmos performance [{platform.node()}|{os.getpid()}]: The cache size for {self.cache_identifier} is {len(dbt_ls_cache.encode('utf-8'))}"
+                )
+                self.load_method = LoadMode.DBT_LS_CACHE
+                project_path = self.render_config.project_path
+                nodes = parse_dbt_ls_output(project_path=project_path, ls_stdout=dbt_ls_cache)
+                self.nodes = nodes
+                self.filtered_nodes = nodes
+                return True
+        return False
+
     def run_dbt_ls(
         self, dbt_cmd: str, project_path: Path, tmp_dir: Path, env_vars: dict[str, str]
     ) -> dict[str, DbtNode]:
         """Runs dbt ls command and returns the parsed nodes."""
         ls_command = [dbt_cmd, "ls", "--output", "json"]
 
         if self.render_config.exclude:
@@ -219,26 +244,30 @@
         log_filepath = self.log_dir / DBT_LOG_FILENAME
         logger.debug("dbt logs available in: %s", log_filepath)
         if log_filepath.exists():
             with open(log_filepath) as logfile:
                 for line in logfile:
                     logger.debug(line.strip())
 
+        if settings.enable_cache and settings.experimental_cache:
+            Variable.set(self.cache_identifier, stdout)
+
         nodes = parse_dbt_ls_output(project_path, stdout)
         return nodes
 
     def load_via_dbt_ls(self) -> None:
         """
         This is the most accurate way of loading `dbt` projects and filtering them out, since it uses the `dbt` command
         line for both parsing and filtering the nodes.
 
         Updates in-place:
         * self.nodes
         * self.filtered_nodes
         """
+        self.load_method = LoadMode.DBT_LS
         self.render_config.validate_dbt_command(fallback_cmd=self.execution_config.dbt_executable_path)
         dbt_cmd = self.render_config.dbt_executable_path
         dbt_cmd = dbt_cmd.as_posix() if isinstance(dbt_cmd, Path) else dbt_cmd
 
         logger.info(f"Trying to parse the dbt project in `{self.render_config.project_path}` using dbt ls...")
         if not self.render_config.project_path or not self.execution_config.project_path:
             raise CosmosLoadDbtException(
@@ -306,14 +335,15 @@
         This is between dbt ls and full manifest. It allows to use the output (needs to be json output) of the dbt ls as a
         file stored in the image you run Cosmos on. The advantage is that you can use the parser from LoadMode.DBT_LS without
         actually running dbt ls every time. BUT you will need one dbt ls file for each separate group.
 
         This technically should increase performance and also removes the necessity to have your whole dbt project copied
         to the airflow image.
         """
+        self.load_method = LoadMode.DBT_LS_FILE
         logger.info("Trying to parse the dbt project `%s` using a dbt ls output file...", self.project.project_name)
 
         if not self.render_config.is_dbt_ls_file_available():
             raise CosmosLoadDbtException(f"Unable to load dbt ls file using {self.render_config.dbt_ls_path}")
 
         project_path = self.render_config.project_path
         if not project_path:
@@ -333,14 +363,15 @@
         Internally, it uses the legacy Cosmos DbtProject representation and converts it to the current
         nodes list representation.
 
         Updates in-place:
         * self.nodes
         * self.filtered_nodes
         """
+        self.load_method = LoadMode.CUSTOM
         logger.info("Trying to parse the dbt project `%s` using a custom Cosmos method...", self.project.project_name)
 
         if self.render_config.selector:
             raise CosmosLoadDbtException(
                 "RenderConfig.selector is not yet supported when loading dbt projects using the LoadMode.CUSTOM parser."
             )
 
@@ -391,14 +422,15 @@
         However, since the Manifest does not represent filters, it relies on the Custom Cosmos implementation
         to filter out the nodes relevant to the user (based on self.exclude and self.select).
 
         Updates in-place:
         * self.nodes
         * self.filtered_nodes
         """
+        self.load_method = LoadMode.DBT_MANIFEST
         logger.info("Trying to parse the dbt project `%s` using a dbt manifest...", self.project.project_name)
 
         if self.render_config.selector:
             raise CosmosLoadDbtException(
                 "RenderConfig.selector is not yet supported when loading dbt projects using the LoadMode.DBT_MANIFEST parser."
             )
```

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/dbt/project.py` & `astronomer_cosmos-1.5.0a3/cosmos/dbt/project.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/dbt/selector.py` & `astronomer_cosmos-1.5.0a3/cosmos/dbt/selector.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/dbt/parser/output.py` & `astronomer_cosmos-1.5.0a3/cosmos/dbt/parser/output.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/dbt/parser/project.py` & `astronomer_cosmos-1.5.0a3/cosmos/dbt/parser/project.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/hooks/subprocess.py` & `astronomer_cosmos-1.5.0a3/cosmos/hooks/subprocess.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/operators/__init__.py` & `astronomer_cosmos-1.5.0a3/cosmos/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/operators/aws_eks.py` & `astronomer_cosmos-1.5.0a3/cosmos/operators/aws_eks.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/operators/azure_container_instance.py` & `astronomer_cosmos-1.5.0a3/cosmos/operators/azure_container_instance.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/operators/base.py` & `astronomer_cosmos-1.5.0a3/cosmos/operators/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/operators/docker.py` & `astronomer_cosmos-1.5.0a3/cosmos/operators/docker.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/operators/kubernetes.py` & `astronomer_cosmos-1.5.0a3/cosmos/operators/kubernetes.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/operators/local.py` & `astronomer_cosmos-1.5.0a3/cosmos/operators/local.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,18 +175,16 @@
             logger.info("dbtRunner is available. Using dbtRunner for invoking dbt.")
         self._set_invocation_methods()
 
     def handle_exception_subprocess(self, result: FullOutputSubprocessResult) -> None:
         if self.skip_exit_code is not None and result.exit_code == self.skip_exit_code:
             raise AirflowSkipException(f"dbt command returned exit code {self.skip_exit_code}. Skipping.")
         elif result.exit_code != 0:
-            raise AirflowException(
-                f"dbt command failed. The command returned a non-zero exit code {result.exit_code}. Details: ",
-                *result.full_output,
-            )
+            logger.error("\n".join(result.full_output))
+            raise AirflowException(f"dbt command failed. The command returned a non-zero exit code {result.exit_code}.")
 
     def handle_exception_dbt_runner(self, result: dbtRunnerResult) -> None:
         """dbtRunnerResult has an attribute `success` that is False if the command failed."""
         if not result.success:
             if result.exception:
                 raise AirflowException(f"dbt invocation did not complete with unhandled error: {result.exception}")
             else:
```

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/operators/virtualenv.py` & `astronomer_cosmos-1.5.0a3/cosmos/operators/virtualenv.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/plugin/__init__.py` & `astronomer_cosmos-1.5.0a3/cosmos/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/plugin/static/iframeResizer.contentWindow.min.js` & `astronomer_cosmos-1.5.0a3/cosmos/plugin/static/iframeResizer.contentWindow.min.js`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/plugin/static/iframeResizer.min.js` & `astronomer_cosmos-1.5.0a3/cosmos/plugin/static/iframeResizer.min.js`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/profiles/__init__.py` & `astronomer_cosmos-1.5.0a3/cosmos/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/profiles/base.py` & `astronomer_cosmos-1.5.0a3/cosmos/profiles/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/profiles/athena/access_key.py` & `astronomer_cosmos-1.5.0a3/cosmos/profiles/athena/access_key.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/profiles/bigquery/oauth.py` & `astronomer_cosmos-1.5.0a3/cosmos/profiles/bigquery/oauth.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/profiles/bigquery/service_account_file.py` & `astronomer_cosmos-1.5.0a3/cosmos/profiles/bigquery/service_account_file.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/profiles/bigquery/service_account_keyfile_dict.py` & `astronomer_cosmos-1.5.0a3/cosmos/profiles/bigquery/service_account_keyfile_dict.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/profiles/databricks/token.py` & `astronomer_cosmos-1.5.0a3/cosmos/profiles/databricks/token.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/profiles/exasol/user_pass.py` & `astronomer_cosmos-1.5.0a3/cosmos/profiles/exasol/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/profiles/postgres/user_pass.py` & `astronomer_cosmos-1.5.0a3/cosmos/profiles/postgres/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/profiles/redshift/user_pass.py` & `astronomer_cosmos-1.5.0a3/cosmos/profiles/redshift/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/profiles/snowflake/__init__.py` & `astronomer_cosmos-1.5.0a3/cosmos/profiles/snowflake/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/profiles/snowflake/user_encrypted_privatekey_env_variable.py` & `astronomer_cosmos-1.5.0a3/cosmos/profiles/snowflake/user_encrypted_privatekey_env_variable.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/profiles/snowflake/user_encrypted_privatekey_file.py` & `astronomer_cosmos-1.5.0a3/cosmos/profiles/snowflake/user_encrypted_privatekey_file.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/profiles/snowflake/user_pass.py` & `astronomer_cosmos-1.5.0a3/cosmos/profiles/snowflake/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/profiles/snowflake/user_privatekey.py` & `astronomer_cosmos-1.5.0a3/cosmos/profiles/snowflake/user_privatekey.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/profiles/spark/thrift.py` & `astronomer_cosmos-1.5.0a3/cosmos/profiles/spark/thrift.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/profiles/trino/base.py` & `astronomer_cosmos-1.5.0a3/cosmos/profiles/trino/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/profiles/trino/certificate.py` & `astronomer_cosmos-1.5.0a3/cosmos/profiles/trino/certificate.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/profiles/trino/jwt.py` & `astronomer_cosmos-1.5.0a3/cosmos/profiles/trino/jwt.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/profiles/trino/ldap.py` & `astronomer_cosmos-1.5.0a3/cosmos/profiles/trino/ldap.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/cosmos/profiles/vertica/user_pass.py` & `astronomer_cosmos-1.5.0a3/cosmos/profiles/vertica/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/.gitignore` & `astronomer_cosmos-1.5.0a3/.gitignore`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/LICENSE` & `astronomer_cosmos-1.5.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/README.rst` & `astronomer_cosmos-1.5.0a3/README.rst`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.5.0a2/pyproject.toml` & `astronomer_cosmos-1.5.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 dbt-databricks = ["dbt-databricks"]
 dbt-exasol = ["dbt-exasol"]
 dbt-postgres = ["dbt-postgres"]
 dbt-redshift = ["dbt-redshift"]
 dbt-snowflake = ["dbt-snowflake"]
 dbt-spark = ["dbt-spark"]
 dbt-vertica = ["dbt-vertica<=1.5.4"]
-openlineage = ["openlineage-integration-common", "openlineage-airflow"]
+openlineage = ["openlineage-integration-common!=1.15.0", "openlineage-airflow"]
 all = ["astronomer-cosmos[dbt-all]", "astronomer-cosmos[openlineage]"]
 docs = [
     "sphinx",
     "pydata-sphinx-theme",
     "sphinx-autobuild",
     "sphinx-autoapi",
     "apache-airflow-providers-cncf-kubernetes>=5.1.1",
@@ -117,19 +117,19 @@
 ######################################
 # TESTING
 ######################################
 
 [tool.hatch.envs.tests]
 dependencies = [
     "astronomer-cosmos[tests]",
-    "apache-airflow-providers-postgres",
     "apache-airflow-providers-cncf-kubernetes>=5.1.1",
     "apache-airflow-providers-amazon>=3.0.0,<8.20.0", # https://github.com/apache/airflow/issues/39103
     "apache-airflow-providers-docker>=3.5.0",
     "apache-airflow-providers-microsoft-azure",
+    "apache-airflow-providers-postgres",
     "types-PyYAML",
     "types-attrs",
     "types-requests",
     "types-python-dateutil",
     "Werkzeug<3.0.0",
     "apache-airflow=={matrix:airflow}.0",
 ]
```

### Comparing `astronomer_cosmos-1.5.0a2/PKG-INFO` & `astronomer_cosmos-1.5.0a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: astronomer-cosmos
-Version: 1.5.0a2
+Version: 1.5.0a3
 Summary: Orchestrate your dbt projects in Airflow
 Project-URL: Homepage, https://github.com/astronomer/astronomer-cosmos
 Project-URL: Documentation, https://astronomer.github.io/astronomer-cosmos
 Project-URL: Source code, https://github.com/astronomer/astronomer-cosmos
 Author-email: Astronomer <humans@astronomer.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -39,15 +39,15 @@
 Requires-Dist: dbt-exasol; extra == 'all'
 Requires-Dist: dbt-postgres; extra == 'all'
 Requires-Dist: dbt-redshift; extra == 'all'
 Requires-Dist: dbt-snowflake; extra == 'all'
 Requires-Dist: dbt-spark; extra == 'all'
 Requires-Dist: dbt-vertica; extra == 'all'
 Requires-Dist: openlineage-airflow; extra == 'all'
-Requires-Dist: openlineage-integration-common; extra == 'all'
+Requires-Dist: openlineage-integration-common!=1.15.0; extra == 'all'
 Provides-Extra: aws-eks
 Requires-Dist: apache-airflow-providers-amazon<8.20.0,>=8.0.0; extra == 'aws-eks'
 Provides-Extra: azure-container-instance
 Requires-Dist: apache-airflow-providers-microsoft-azure>=8.4.0; extra == 'azure-container-instance'
 Provides-Extra: dbt-all
 Requires-Dist: dbt-athena; extra == 'dbt-all'
 Requires-Dist: dbt-bigquery; extra == 'dbt-all'
@@ -85,15 +85,15 @@
 Requires-Dist: sphinx; extra == 'docs'
 Requires-Dist: sphinx-autoapi; extra == 'docs'
 Requires-Dist: sphinx-autobuild; extra == 'docs'
 Provides-Extra: kubernetes
 Requires-Dist: apache-airflow-providers-cncf-kubernetes>=5.1.1; extra == 'kubernetes'
 Provides-Extra: openlineage
 Requires-Dist: openlineage-airflow; extra == 'openlineage'
-Requires-Dist: openlineage-integration-common; extra == 'openlineage'
+Requires-Dist: openlineage-integration-common!=1.15.0; extra == 'openlineage'
 Provides-Extra: tests
 Requires-Dist: packaging; extra == 'tests'
 Requires-Dist: pre-commit; extra == 'tests'
 Requires-Dist: pytest-cov; extra == 'tests'
 Requires-Dist: pytest-describe; extra == 'tests'
 Requires-Dist: pytest-dotenv; extra == 'tests'
 Requires-Dist: pytest-split; extra == 'tests'
```

