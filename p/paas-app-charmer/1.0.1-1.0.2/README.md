# Comparing `tmp/paas_app_charmer-1.0.1.tar.gz` & `tmp/paas_app_charmer-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paas_app_charmer-1.0.1.tar", last modified: Thu May 23 07:17:20 2024, max compression
+gzip compressed data, was "paas_app_charmer-1.0.2.tar", last modified: Mon Jun  3 07:52:04 2024, max compression
```

## Comparing `paas_app_charmer-1.0.1.tar` & `paas_app_charmer-1.0.2.tar`

### file list

```diff
@@ -1,48 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:17:20.962857 paas_app_charmer-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-23 07:17:20.962857 paas_app_charmer-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:17:20.958857 paas_app_charmer-1.0.1/paas_app_charmer/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:17:20.958857 paas_app_charmer-1.0.1/paas_app_charmer/_gunicorn/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/_gunicorn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10036 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/_gunicorn/charm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/_gunicorn/charm_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/_gunicorn/observability.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/_gunicorn/secret_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     7159 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/_gunicorn/webserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/_gunicorn/wsgi_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/database_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/databases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:17:20.958857 paas_app_charmer-1.0.1/paas_app_charmer/django/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/django/charm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:17:20.954857 paas_app_charmer-1.0.1/paas_app_charmer/django/cos/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:17:20.958857 paas_app_charmer-1.0.1/paas_app_charmer/django/cos/grafana_dashboards/
--rw-r--r--   0 runner    (1001) docker     (127)    26134 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/django/cos/grafana_dashboards/django.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:17:20.962857 paas_app_charmer-1.0.1/paas_app_charmer/django/cos/loki_alert_rules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/django/cos/loki_alert_rules/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:17:20.962857 paas_app_charmer-1.0.1/paas_app_charmer/django/cos/prometheus_alert_rules/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/django/cos/prometheus_alert_rules/django.rule
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:17:20.962857 paas_app_charmer-1.0.1/paas_app_charmer/flask/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/flask/charm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:17:20.954857 paas_app_charmer-1.0.1/paas_app_charmer/flask/cos/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:17:20.962857 paas_app_charmer-1.0.1/paas_app_charmer/flask/cos/grafana_dashboards/
--rw-r--r--   0 runner    (1001) docker     (127)    26108 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/flask/cos/grafana_dashboards/flask.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:17:20.962857 paas_app_charmer-1.0.1/paas_app_charmer/flask/cos/loki_alert_rules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/flask/cos/loki_alert_rules/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:17:20.962857 paas_app_charmer-1.0.1/paas_app_charmer/flask/cos/prometheus_alert_rules/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/flask/cos/prometheus_alert_rules/flask.rule
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/secret_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:17:20.962857 paas_app_charmer-1.0.1/paas_app_charmer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-23 07:17:20.000000 paas_app_charmer-1.0.1/paas_app_charmer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-23 07:17:20.000000 paas_app_charmer-1.0.1/paas_app_charmer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 07:17:20.000000 paas_app_charmer-1.0.1/paas_app_charmer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-23 07:17:20.000000 paas_app_charmer-1.0.1/paas_app_charmer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-23 07:17:20.000000 paas_app_charmer-1.0.1/paas_app_charmer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 07:17:20.962857 paas_app_charmer-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:52:04.628904 paas_app_charmer-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-06-03 07:52:04.628904 paas_app_charmer-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-06-03 07:52:00.000000 paas_app_charmer-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:52:04.624904 paas_app_charmer-1.0.2/paas_app_charmer/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-06-03 07:52:00.000000 paas_app_charmer-1.0.2/paas_app_charmer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:52:04.624904 paas_app_charmer-1.0.2/paas_app_charmer/_gunicorn/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-03 07:52:00.000000 paas_app_charmer-1.0.2/paas_app_charmer/_gunicorn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9893 2024-06-03 07:52:00.000000 paas_app_charmer-1.0.2/paas_app_charmer/_gunicorn/charm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-06-03 07:52:00.000000 paas_app_charmer-1.0.2/paas_app_charmer/_gunicorn/charm_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-06-03 07:52:00.000000 paas_app_charmer-1.0.2/paas_app_charmer/_gunicorn/observability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-06-03 07:52:00.000000 paas_app_charmer-1.0.2/paas_app_charmer/_gunicorn/secret_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7159 2024-06-03 07:52:00.000000 paas_app_charmer-1.0.2/paas_app_charmer/_gunicorn/webserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-06-03 07:52:00.000000 paas_app_charmer-1.0.2/paas_app_charmer/_gunicorn/wsgi_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-06-03 07:52:00.000000 paas_app_charmer-1.0.2/paas_app_charmer/database_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-06-03 07:52:00.000000 paas_app_charmer-1.0.2/paas_app_charmer/databases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:52:04.624904 paas_app_charmer-1.0.2/paas_app_charmer/django/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-06-03 07:52:00.000000 paas_app_charmer-1.0.2/paas_app_charmer/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-06-03 07:52:00.000000 paas_app_charmer-1.0.2/paas_app_charmer/django/charm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:52:04.620904 paas_app_charmer-1.0.2/paas_app_charmer/django/cos/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:52:04.624904 paas_app_charmer-1.0.2/paas_app_charmer/django/cos/grafana_dashboards/
+-rw-r--r--   0 runner    (1001) docker     (127)    26134 2024-06-03 07:52:00.000000 paas_app_charmer-1.0.2/paas_app_charmer/django/cos/grafana_dashboards/django.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:52:04.624904 paas_app_charmer-1.0.2/paas_app_charmer/django/cos/loki_alert_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 07:52:00.000000 paas_app_charmer-1.0.2/paas_app_charmer/django/cos/loki_alert_rules/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:52:04.624904 paas_app_charmer-1.0.2/paas_app_charmer/django/cos/prometheus_alert_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-06-03 07:52:00.000000 paas_app_charmer-1.0.2/paas_app_charmer/django/cos/prometheus_alert_rules/django.rule
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-06-03 07:52:00.000000 paas_app_charmer-1.0.2/paas_app_charmer/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:52:04.628904 paas_app_charmer-1.0.2/paas_app_charmer/flask/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-06-03 07:52:00.000000 paas_app_charmer-1.0.2/paas_app_charmer/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-06-03 07:52:00.000000 paas_app_charmer-1.0.2/paas_app_charmer/flask/charm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:52:04.620904 paas_app_charmer-1.0.2/paas_app_charmer/flask/cos/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:52:04.628904 paas_app_charmer-1.0.2/paas_app_charmer/flask/cos/grafana_dashboards/
+-rw-r--r--   0 runner    (1001) docker     (127)    26108 2024-06-03 07:52:00.000000 paas_app_charmer-1.0.2/paas_app_charmer/flask/cos/grafana_dashboards/flask.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:52:04.628904 paas_app_charmer-1.0.2/paas_app_charmer/flask/cos/loki_alert_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 07:52:00.000000 paas_app_charmer-1.0.2/paas_app_charmer/flask/cos/loki_alert_rules/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:52:04.628904 paas_app_charmer-1.0.2/paas_app_charmer/flask/cos/prometheus_alert_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-06-03 07:52:00.000000 paas_app_charmer-1.0.2/paas_app_charmer/flask/cos/prometheus_alert_rules/flask.rule
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-06-03 07:52:00.000000 paas_app_charmer-1.0.2/paas_app_charmer/secret_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:52:04.628904 paas_app_charmer-1.0.2/paas_app_charmer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-06-03 07:52:04.000000 paas_app_charmer-1.0.2/paas_app_charmer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-06-03 07:52:04.000000 paas_app_charmer-1.0.2/paas_app_charmer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 07:52:04.000000 paas_app_charmer-1.0.2/paas_app_charmer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-03 07:52:04.000000 paas_app_charmer-1.0.2/paas_app_charmer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-06-03 07:52:04.000000 paas_app_charmer-1.0.2/paas_app_charmer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-06-03 07:52:00.000000 paas_app_charmer-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-06-03 07:52:00.000000 paas_app_charmer-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 07:52:04.628904 paas_app_charmer-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-06-03 07:52:00.000000 paas_app_charmer-1.0.2/setup.py
```

### Comparing `paas_app_charmer-1.0.1/PKG-INFO` & `paas_app_charmer-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paas-app-charmer
-Version: 1.0.1
+Version: 1.0.2
 Summary: Companion library for PaaS app charmer.
 Author-email: Canonical IS DevOps team <is-devops-team@canonical.com>
 Project-URL: Repository, https://github.com/canonical/paas-app-charmer
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `paas_app_charmer-1.0.1/README.md` & `paas_app_charmer-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `paas_app_charmer-1.0.1/paas_app_charmer/_gunicorn/charm.py` & `paas_app_charmer-1.0.2/paas_app_charmer/_gunicorn/charm.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from paas_app_charmer._gunicorn.observability import Observability
 from paas_app_charmer._gunicorn.secret_storage import GunicornSecretStorage
 from paas_app_charmer._gunicorn.webserver import GunicornWebserver
 from paas_app_charmer._gunicorn.wsgi_app import WsgiApp
 from paas_app_charmer.database_migration import DatabaseMigration, DatabaseMigrationStatus
 from paas_app_charmer.databases import Databases, make_database_requirers
 from paas_app_charmer.exceptions import CharmConfigInvalidError
-from paas_app_charmer.helpers import load_requires
 
 logger = logging.getLogger(__name__)
 
 
 class GunicornBase(abc.ABC, ops.CharmBase):  # pylint: disable=too-many-instance-attributes
     """Gunicorn-based charm service mixin.
 
@@ -37,15 +36,14 @@
         """Return the framework related configurations."""
 
     @abc.abstractmethod
     def get_cos_dir(self) -> str:
         """Return the directory with COS related files."""
 
     on = RedisRelationCharmEvents()
-    _store = ops.StoredState()
 
     def __init__(self, framework: ops.Framework, wsgi_framework: str) -> None:
         """Initialize the instance.
 
         Args:
             framework: operator framework.
             wsgi_framework: WSGI framework name.
@@ -57,18 +55,17 @@
         self._database_requirers = make_database_requirers(self, self.app.name)
         try:
             wsgi_config = self.get_wsgi_config()
         except CharmConfigInvalidError as exc:
             self._update_app_and_unit_status(ops.BlockedStatus(exc.msg))
             return
 
-        requires = load_requires()
-        if "redis" in requires and requires["redis"]["interface"] == "redis":
-            self._store.set_default(redis_relation={})
-            self._redis = RedisRequires(charm=self, _stored=self._store, relation_name="redis")
+        requires = self.framework.meta.requires
+        if "redis" in requires and requires["redis"].interface_name == "redis":
+            self._redis = RedisRequires(charm=self, relation_name="redis")
             self.framework.observe(self.on.redis_relation_updated, self._on_redis_relation_updated)
         else:
             self._redis = None
 
         self._charm_state = CharmState.from_charm(
             charm=self,
             framework=wsgi_framework,
```

### Comparing `paas_app_charmer-1.0.1/paas_app_charmer/_gunicorn/charm_state.py` & `paas_app_charmer-1.0.2/paas_app_charmer/_gunicorn/charm_state.py`

 * *Files identical despite different names*

### Comparing `paas_app_charmer-1.0.1/paas_app_charmer/_gunicorn/observability.py` & `paas_app_charmer-1.0.2/paas_app_charmer/_gunicorn/observability.py`

 * *Files identical despite different names*

### Comparing `paas_app_charmer-1.0.1/paas_app_charmer/_gunicorn/secret_storage.py` & `paas_app_charmer-1.0.2/paas_app_charmer/_gunicorn/secret_storage.py`

 * *Files identical despite different names*

### Comparing `paas_app_charmer-1.0.1/paas_app_charmer/_gunicorn/webserver.py` & `paas_app_charmer-1.0.2/paas_app_charmer/_gunicorn/webserver.py`

 * *Files identical despite different names*

### Comparing `paas_app_charmer-1.0.1/paas_app_charmer/_gunicorn/wsgi_app.py` & `paas_app_charmer-1.0.2/paas_app_charmer/_gunicorn/wsgi_app.py`

 * *Files identical despite different names*

### Comparing `paas_app_charmer-1.0.1/paas_app_charmer/database_migration.py` & `paas_app_charmer-1.0.2/paas_app_charmer/database_migration.py`

 * *Files identical despite different names*

### Comparing `paas_app_charmer-1.0.1/paas_app_charmer/databases.py` & `paas_app_charmer-1.0.2/paas_app_charmer/databases.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 
 import logging
 import typing
 
 import ops
 from charms.data_platform_libs.v0.data_interfaces import DatabaseRequires
 
-from paas_app_charmer.helpers import load_requires
-
 SUPPORTED_DB_INTERFACES = {
     "mysql_client": "mysql",
     "postgresql_client": "postgresql",
     "mongodb_client": "mongodb",
 }
 
 logger = logging.getLogger(__name__)
@@ -36,17 +34,17 @@
         charm: The requiring charm.
         database_name: the required database name
 
     Returns: A dictionary which is the database uri environment variable name and the
         value is the corresponding database requirer object.
     """
     db_interfaces = (
-        SUPPORTED_DB_INTERFACES[require["interface"]]
-        for require in load_requires().values()
-        if require["interface"] in SUPPORTED_DB_INTERFACES
+        SUPPORTED_DB_INTERFACES[require.interface_name]
+        for require in charm.framework.meta.requires.values()
+        if require.interface_name in SUPPORTED_DB_INTERFACES
     )
     # automatically create database relation requirers to manage database relations
     # one database relation requirer is required for each of the database relations
     # create a dictionary to hold the requirers
     databases = {
         name: (
             DatabaseRequires(
```

### Comparing `paas_app_charmer-1.0.1/paas_app_charmer/django/charm.py` & `paas_app_charmer-1.0.2/paas_app_charmer/django/charm.py`

 * *Files identical despite different names*

### Comparing `paas_app_charmer-1.0.1/paas_app_charmer/django/cos/grafana_dashboards/django.json` & `paas_app_charmer-1.0.2/paas_app_charmer/django/cos/grafana_dashboards/django.json`

 * *Files identical despite different names*

### Comparing `paas_app_charmer-1.0.1/paas_app_charmer/exceptions.py` & `paas_app_charmer-1.0.2/paas_app_charmer/exceptions.py`

 * *Files identical despite different names*

### Comparing `paas_app_charmer-1.0.1/paas_app_charmer/flask/charm.py` & `paas_app_charmer-1.0.2/paas_app_charmer/flask/charm.py`

 * *Files identical despite different names*

### Comparing `paas_app_charmer-1.0.1/paas_app_charmer/flask/cos/grafana_dashboards/flask.json` & `paas_app_charmer-1.0.2/paas_app_charmer/flask/cos/grafana_dashboards/flask.json`

 * *Files identical despite different names*

### Comparing `paas_app_charmer-1.0.1/paas_app_charmer/secret_storage.py` & `paas_app_charmer-1.0.2/paas_app_charmer/secret_storage.py`

 * *Files identical despite different names*

### Comparing `paas_app_charmer-1.0.1/paas_app_charmer.egg-info/PKG-INFO` & `paas_app_charmer-1.0.2/paas_app_charmer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paas-app-charmer
-Version: 1.0.1
+Version: 1.0.2
 Summary: Companion library for PaaS app charmer.
 Author-email: Canonical IS DevOps team <is-devops-team@canonical.com>
 Project-URL: Repository, https://github.com/canonical/paas-app-charmer
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `paas_app_charmer-1.0.1/paas_app_charmer.egg-info/SOURCES.txt` & `paas_app_charmer-1.0.2/paas_app_charmer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 pyproject.toml
 requirements.txt
 setup.py
 paas_app_charmer/__init__.py
 paas_app_charmer/database_migration.py
 paas_app_charmer/databases.py
 paas_app_charmer/exceptions.py
-paas_app_charmer/helpers.py
 paas_app_charmer/secret_storage.py
 paas_app_charmer.egg-info/PKG-INFO
 paas_app_charmer.egg-info/SOURCES.txt
 paas_app_charmer.egg-info/dependency_links.txt
 paas_app_charmer.egg-info/requires.txt
 paas_app_charmer.egg-info/top_level.txt
 paas_app_charmer/_gunicorn/__init__.py
```

### Comparing `paas_app_charmer-1.0.1/pyproject.toml` & `paas_app_charmer-1.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright 2024 Canonical Ltd.
 # See LICENSE file for licensing details.
 [project]
 name = "paas-app-charmer"
-version = "1.0.1"
+version = "1.0.2"
 description = "Companion library for PaaS app charmer."
 readme = "README.md"
 authors = [
     {name = "Canonical IS DevOps team", email="is-devops-team@canonical.com"},
 ]
 requires-python = ">=3.10"
 dynamic = ["dependencies"]
@@ -40,14 +40,21 @@
 minversion = "6.0"
 log_cli_level = "INFO"
 
 # Formatting tools configuration
 [tool.black]
 line-length = 99
 target-version = ["py38"]
+extend-exclude = '''
+
+(
+  examples/flask/lib/.*
+  |   examples/django/charm/lib/.*
+)
+'''
 
 [tool.isort]
 line_length = 99
 profile = "black"
 
 # Linting tools configuration
 [tool.flake8]
```

