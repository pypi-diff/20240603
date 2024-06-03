# Comparing `tmp/eodash_catalog-0.0.6.tar.gz` & `tmp/eodash_catalog-0.0.7.tar.gz`

## Comparing `eodash_catalog-0.0.6.tar` & `eodash_catalog-0.0.7.tar`

### file list

```diff
@@ -1,547 +1,547 @@
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/requirements.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/.gitignore
--rw-r--r--   0        0        0  2079434 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/pip.pyz
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/pyvenv.cfg
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/bin/Activate.ps1
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/bin/activate
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/bin/activate.csh
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/bin/activate.fish
--rwxr-xr-x   0        0        0      278 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/bin/pip
--rwxr-xr-x   0        0        0      278 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/bin/pip3
--rwxr-xr-x   0        0        0      278 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/bin/pip3.10
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/bin/python -> python3
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/bin/python3 -> /bin/python3
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/bin/python3.10 -> python3
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/__init__.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/__main__.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/__pip-runner__.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/py.typed
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/__init__.py
--rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/build_env.py
--rw-r--r--   0        0        0    10370 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/cache.py
--rw-r--r--   0        0        0    14006 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/configuration.py
--rw-r--r--   0        0        0    23634 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/exceptions.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/main.py
--rw-r--r--   0        0        0     7152 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/pyproject.py
--rw-r--r--   0        0        0     8378 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/self_outdated_check.py
--rw-r--r--   0        0        0    11801 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/wheel_builder.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/cli/__init__.py
--rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/cli/autocompletion.py
--rw-r--r--   0        0        0     8733 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/cli/base_command.py
--rw-r--r--   0        0        0    30064 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/cli/cmdoptions.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/cli/command_context.py
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/cli/main.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/cli/main_parser.py
--rw-r--r--   0        0        0    10781 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/cli/parser.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/cli/progress_bars.py
--rw-r--r--   0        0        0    18369 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/cli/req_command.py
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/cli/spinners.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/cli/status_codes.py
--rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/__init__.py
--rw-r--r--   0        0        0     7944 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/cache.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/check.py
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/completion.py
--rw-r--r--   0        0        0     9766 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/configuration.py
--rw-r--r--   0        0        0     6777 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/debug.py
--rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/download.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/freeze.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/hash.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/help.py
--rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/index.py
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/inspect.py
--rw-r--r--   0        0        0    28782 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/install.py
--rw-r--r--   0        0        0    12450 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/list.py
--rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/search.py
--rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/show.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/uninstall.py
--rw-r--r--   0        0        0     6476 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/wheel.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/distributions/__init__.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/distributions/base.py
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/distributions/installed.py
--rw-r--r--   0        0        0     6709 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/distributions/sdist.py
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/distributions/wheel.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/index/__init__.py
--rw-r--r--   0        0        0    16590 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/index/collector.py
--rw-r--r--   0        0        0    37843 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/index/package_finder.py
--rw-r--r--   0        0        0     8688 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/index/sources.py
--rw-r--r--   0        0        0    15365 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/locations/__init__.py
--rw-r--r--   0        0        0     6009 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/locations/_distutils.py
--rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/locations/_sysconfig.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/locations/base.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/metadata/__init__.py
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/metadata/_json.py
--rw-r--r--   0        0        0    25907 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/metadata/base.py
--rw-r--r--   0        0        0    10035 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/metadata/pkg_resources.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-r--r--   0        0        0     7456 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/models/__init__.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/models/candidate.py
--rw-r--r--   0        0        0     6889 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/models/direct_url.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/models/format_control.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/models/index.py
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/models/installation_report.py
--rw-r--r--   0        0        0    20777 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/models/link.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/models/scheme.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/models/search_scope.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/models/selection_prefs.py
--rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/models/target_python.py
--rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/models/wheel.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/network/__init__.py
--rw-r--r--   0        0        0    20541 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/network/auth.py
--rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/network/cache.py
--rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/network/download.py
--rw-r--r--   0        0        0     7638 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/network/lazy_wheel.py
--rw-r--r--   0        0        0    18698 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/network/session.py
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/network/utils.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/network/xmlrpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/operations/__init__.py
--rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/operations/check.py
--rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/operations/freeze.py
--rw-r--r--   0        0        0    28128 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/operations/prepare.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/operations/install/__init__.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-r--r--   0        0        0    27311 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/operations/install/wheel.py
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/req/__init__.py
--rw-r--r--   0        0        0    19018 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/req/constructors.py
--rw-r--r--   0        0        0    17790 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/req/req_file.py
--rw-r--r--   0        0        0    35460 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/req/req_install.py
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/req/req_set.py
--rw-r--r--   0        0        0    24551 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/req/req_uninstall.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/resolution/__init__.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/resolution/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-r--r--   0        0        0    24025 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/resolution/legacy/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-r--r--   0        0        0    21052 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-r--r--   0        0        0    32292 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-r--r--   0        0        0     9824 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-r--r--   0        0        0    12592 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/__init__.py
--rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/_jaraco_text.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/_log.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/appdirs.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/compat.py
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/datetime.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/deprecation.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/egg_link.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/encoding.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/entrypoints.py
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/filesystem.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/filetypes.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/glibc.py
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/hashes.py
--rw-r--r--   0        0        0    11603 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/logging.py
--rw-r--r--   0        0        0    23623 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/misc.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/models.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/packaging.py
--rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/setuptools_build.py
--rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/subprocess.py
--rw-r--r--   0        0        0     9312 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/temp_dir.py
--rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/unpacking.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/urls.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/virtualenv.py
--rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/wheel.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/vcs/__init__.py
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/vcs/bazaar.py
--rw-r--r--   0        0        0    18121 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/vcs/git.py
--rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/vcs/mercurial.py
--rw-r--r--   0        0        0    11729 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/vcs/subversion.py
--rw-r--r--   0        0        0    22787 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/__init__.py
--rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/six.py
--rw-r--r--   0        0        0   111130 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/typing_extensions.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/vendor.txt
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/cache.py
--rw-r--r--   0        0        0    18384 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/py.typed
--rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/wrapper.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-r--r--   0        0        0     5352 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/certifi/__init__.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/certifi/__main__.py
--rw-r--r--   0        0        0   281617 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/certifi/cacert.pem
--rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/certifi/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/certifi/py.typed
--rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/__init__.py
--rw-r--r--   0        0        0    31274 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/big5freq.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/big5prober.py
--rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetprober.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/enums.py
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/escprober.py
--rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/escsm.py
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-r--r--   0        0        0    13566 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-r--r--   0        0        0    36913 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-r--r--   0        0        0    20735 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-r--r--   0        0        0    14537 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-r--r--   0        0        0    25796 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-r--r--   0        0        0    42498 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/johabprober.py
--rw-r--r--   0        0        0    27055 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-r--r--   0        0        0   104562 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-r--r--   0        0        0    98484 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-r--r--   0        0        0    98196 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-r--r--   0        0        0   101363 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-r--r--   0        0        0   128035 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-r--r--   0        0        0   102774 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-r--r--   0        0        0    95372 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/macromanprober.py
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-r--r--   0        0        0    30391 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcssm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/py.typed
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/resultdict.py
--rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-r--r--   0        0        0    14848 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-r--r--   0        0        0    13560 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/ansi.py
--rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/initialise.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/win32.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/winterm.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/__init__.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/ansi_test.py
--rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
--rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/initialise_test.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/isatty_test.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/utils.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/winterm_test.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/__init__.py
--rw-r--r--   0        0        0    41487 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/compat.py
--rw-r--r--   0        0        0    51965 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/database.py
--rw-r--r--   0        0        0    20797 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/index.py
--rw-r--r--   0        0        0    51767 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/locators.py
--rw-r--r--   0        0        0    14168 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/manifest.py
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/markers.py
--rw-r--r--   0        0        0    39693 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/metadata.py
--rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/resources.py
--rw-r--r--   0        0        0    18315 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/scripts.py
--rw-r--r--   0        0        0    97792 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/t32.exe
--rw-r--r--   0        0        0   182784 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/t64-arm.exe
--rw-r--r--   0        0        0   108032 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/t64.exe
--rw-r--r--   0        0        0    67530 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/util.py
--rw-r--r--   0        0        0    23747 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/version.py
--rw-r--r--   0        0        0    91648 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/w32.exe
--rw-r--r--   0        0        0   168448 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/w64-arm.exe
--rw-r--r--   0        0        0   101888 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/w64.exe
--rw-r--r--   0        0        0    43958 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/wheel.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distro/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distro/__main__.py
--rw-r--r--   0        0        0    49330 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distro/distro.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distro/py.typed
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/idna/__init__.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/idna/codec.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/idna/compat.py
--rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/idna/core.py
--rw-r--r--   0        0        0    44375 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/idna/idnadata.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/idna/intranges.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/idna/package_data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/idna/py.typed
--rw-r--r--   0        0        0   206539 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/idna/uts46data.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/msgpack/__init__.py
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/msgpack/ext.py
--rw-r--r--   0        0        0    34544 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/msgpack/fallback.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/markers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/py.typed
--rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/version.py
--rw-r--r--   0        0        0   109364 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pkg_resources/__init__.py
--rw-r--r--   0        0        0    20155 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/android.py
--rw-r--r--   0        0        0     7132 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/api.py
--rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/macos.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/py.typed
--rw-r--r--   0        0        0     8809 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/unix.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/version.py
--rw-r--r--   0        0        0     9573 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/windows.py
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/__init__.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/__main__.py
--rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/cmdline.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/console.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/filter.py
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatter.py
--rw-r--r--   0        0        0    34618 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexer.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/modeline.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/plugin.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/regexopt.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/scanner.py
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/style.py
--rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/token.py
--rw-r--r--   0        0        0    63223 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/unistring.py
--rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/util.py
--rw-r--r--   0        0        0    40386 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-r--r--   0        0        0    35610 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-r--r--   0        0        0    21938 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-r--r--   0        0        0    19351 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-r--r--   0        0        0    12130 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-r--r--   0        0        0    72281 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-r--r--   0        0        0    53424 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-r--r--   0        0        0     9116 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-r--r--   0        0        0     6567 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/actions.py
--rw-r--r--   0        0        0    13387 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/common.py
--rw-r--r--   0        0        0   224445 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/core.py
--rw-r--r--   0        0        0     9523 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-r--r--   0        0        0    38646 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/py.typed
--rw-r--r--   0        0        0    26692 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/results.py
--rw-r--r--   0        0        0    13488 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/testing.py
--rw-r--r--   0        0        0    10646 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-r--r--   0        0        0     8670 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/util.py
--rw-r--r--   0        0        0    24215 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/__init__.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_compat.py
--rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_impl.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
--rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
--rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/requests/__init__.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/requests/__version__.py
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-r--r--   0        0        0    19697 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/requests/adapters.py
--rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/requests/api.py
--rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/requests/auth.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/requests/certs.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/requests/compat.py
--rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/requests/cookies.py
--rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/requests/exceptions.py
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/requests/help.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/requests/hooks.py
--rw-r--r--   0        0        0    35288 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/requests/models.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/requests/packages.py
--rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/requests/sessions.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/requests/status_codes.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/requests/structures.py
--rw-r--r--   0        0        0    33460 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/requests/utils.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/__init__.py
--rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/providers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/py.typed
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-r--r--   0        0        0    20511 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/structs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/__init__.py
--rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/__main__.py
--rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_export_format.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_extension.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_fileno.py
--rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_inspect.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_log_render.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_loop.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_null_file.py
--rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_palettes.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_pick.py
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_ratio.py
--rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_spinners.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_stack.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_timer.py
--rw-r--r--   0        0        0    22820 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_win32_console.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_windows.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_wrap.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/abc.py
--rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/align.py
--rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/ansi.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/bar.py
--rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/box.py
--rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/cells.py
--rw-r--r--   0        0        0    18224 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/color.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/color_triplet.py
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/columns.py
--rw-r--r--   0        0        0    99218 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/console.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/constrain.py
--rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/containers.py
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/control.py
--rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/default_styles.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/diagnose.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/emoji.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/errors.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/file_proxy.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/filesize.py
--rw-r--r--   0        0        0     9584 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/highlighter.py
--rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/json.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/jupyter.py
--rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/layout.py
--rw-r--r--   0        0        0    14273 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/live.py
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/live_render.py
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/logging.py
--rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/markup.py
--rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/measure.py
--rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/padding.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/pager.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/palette.py
--rw-r--r--   0        0        0    10574 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/panel.py
--rw-r--r--   0        0        0    35852 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/pretty.py
--rw-r--r--   0        0        0    59706 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/progress.py
--rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/progress_bar.py
--rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/prompt.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/protocol.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/py.typed
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/region.py
--rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/repr.py
--rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/rule.py
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/scope.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/screen.py
--rw-r--r--   0        0        0    24247 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/segment.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/spinner.py
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/status.py
--rw-r--r--   0        0        0    27073 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/style.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/styled.py
--rw-r--r--   0        0        0    35173 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/syntax.py
--rw-r--r--   0        0        0    39684 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/table.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-r--r--   0        0        0    45525 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/text.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/theme.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/themes.py
--rw-r--r--   0        0        0    29604 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/traceback.py
--rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/tree.py
--rw-r--r--   0        0        0    20493 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/__init__.py
--rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/_utils.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/after.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/before.py
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/nap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/py.typed
--rw-r--r--   0        0        0     8746 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/retry.py
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/stop.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/wait.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/tomli/_types.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/tomli/py.typed
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/truststore/__init__.py
--rw-r--r--   0        0        0     9893 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/truststore/_api.py
--rw-r--r--   0        0        0    17694 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/truststore/_macos.py
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/truststore/_openssl.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/truststore/_ssl_constants.py
--rw-r--r--   0        0        0    17468 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/truststore/_windows.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/truststore/py.typed
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/__init__.py
--rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/_collections.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/_version.py
--rw-r--r--   0        0        0    20300 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/connection.py
--rw-r--r--   0        0        0    39990 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/connectionpool.py
--rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/fields.py
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/filepost.py
--rw-r--r--   0        0        0    19752 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-r--r--   0        0        0     6691 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/request.py
--rw-r--r--   0        0        0    30641 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
--rw-r--r--   0        0        0    11036 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-r--r--   0        0        0    17081 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-r--r--   0        0        0    34448 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0        0        0    17632 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/__init__.py
--rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/request.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/response.py
--rw-r--r--   0        0        0    22013 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-r--r--   0        0        0    17177 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0        0        0     6895 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-r--r--   0        0        0    14296 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/url.py
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/webencodings/__init__.py
--rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/webencodings/labels.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/webencodings/tests.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/webencodings/x_user_defined.py
--rw-r--r--   0        0        0    10388 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip-24.0.dist-info/AUTHORS.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip-24.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip-24.0.dist-info/LICENSE.txt
--rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip-24.0.dist-info/METADATA
--rw-r--r--   0        0        0    78936 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip-24.0.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip-24.0.dist-info/REQUESTED
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip-24.0.dist-info/WHEEL
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip-24.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip-24.0.dist-info/top_level.txt
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.vscode/extensions.json
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.vscode/settings.json
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/src/eodash_catalog/__about__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/src/eodash_catalog/__init__.py
--rw-r--r--   0        0        0    11007 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/src/eodash_catalog/duration.py
--rw-r--r--   0        0        0    60962 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/src/eodash_catalog/generate_indicators.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/src/eodash_catalog/sh_endpoint.py
--rw-r--r--   0        0        0     6097 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/src/eodash_catalog/utils.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/.gitignore
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/LICENSE.txt
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/README.md
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 eodash_catalog-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/requirements.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/.gitignore
+-rw-r--r--   0        0        0  2079434 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/pip.pyz
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/pyvenv.cfg
+-rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/bin/Activate.ps1
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/bin/activate
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/bin/activate.csh
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/bin/activate.fish
+-rwxr-xr-x   0        0        0      278 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/bin/pip
+-rwxr-xr-x   0        0        0      278 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/bin/pip3
+-rwxr-xr-x   0        0        0      278 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/bin/pip3.10
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/bin/python -> python3
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/bin/python3 -> /bin/python3
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/bin/python3.10 -> python3
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/__init__.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/__main__.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/__pip-runner__.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/py.typed
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/__init__.py
+-rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/build_env.py
+-rw-r--r--   0        0        0    10370 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/cache.py
+-rw-r--r--   0        0        0    14006 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/configuration.py
+-rw-r--r--   0        0        0    23634 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/exceptions.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/main.py
+-rw-r--r--   0        0        0     7152 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/pyproject.py
+-rw-r--r--   0        0        0     8378 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/self_outdated_check.py
+-rw-r--r--   0        0        0    11801 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/wheel_builder.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/cli/__init__.py
+-rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/cli/autocompletion.py
+-rw-r--r--   0        0        0     8733 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/cli/base_command.py
+-rw-r--r--   0        0        0    30064 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/cli/command_context.py
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/cli/main.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/cli/main_parser.py
+-rw-r--r--   0        0        0    10781 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/cli/parser.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/cli/progress_bars.py
+-rw-r--r--   0        0        0    18369 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/cli/req_command.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/cli/spinners.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/cli/status_codes.py
+-rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/__init__.py
+-rw-r--r--   0        0        0     7944 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/cache.py
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/check.py
+-rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/completion.py
+-rw-r--r--   0        0        0     9766 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/configuration.py
+-rw-r--r--   0        0        0     6777 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/debug.py
+-rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/download.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/freeze.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/hash.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/help.py
+-rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/index.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/inspect.py
+-rw-r--r--   0        0        0    28782 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/install.py
+-rw-r--r--   0        0        0    12450 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/list.py
+-rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/search.py
+-rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/show.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/uninstall.py
+-rw-r--r--   0        0        0     6476 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/wheel.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/distributions/__init__.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/distributions/base.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/distributions/installed.py
+-rw-r--r--   0        0        0     6709 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/distributions/sdist.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/distributions/wheel.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/index/__init__.py
+-rw-r--r--   0        0        0    16590 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/index/collector.py
+-rw-r--r--   0        0        0    37843 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/index/package_finder.py
+-rw-r--r--   0        0        0     8688 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/index/sources.py
+-rw-r--r--   0        0        0    15365 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/locations/__init__.py
+-rw-r--r--   0        0        0     6009 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/locations/_distutils.py
+-rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/locations/base.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/metadata/__init__.py
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/metadata/_json.py
+-rw-r--r--   0        0        0    25907 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/metadata/base.py
+-rw-r--r--   0        0        0    10035 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/metadata/pkg_resources.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/__init__.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_compat.py
+-rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_dists.py
+-rw-r--r--   0        0        0     7456 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_envs.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/models/__init__.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/models/candidate.py
+-rw-r--r--   0        0        0     6889 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/models/direct_url.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/models/format_control.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/models/index.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/models/installation_report.py
+-rw-r--r--   0        0        0    20777 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/models/link.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/models/scheme.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/models/search_scope.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/models/selection_prefs.py
+-rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/models/target_python.py
+-rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/models/wheel.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/network/__init__.py
+-rw-r--r--   0        0        0    20541 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/network/auth.py
+-rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/network/cache.py
+-rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/network/download.py
+-rw-r--r--   0        0        0     7638 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-r--r--   0        0        0    18698 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/network/session.py
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/network/utils.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/network/xmlrpc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/operations/__init__.py
+-rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/operations/check.py
+-rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/operations/freeze.py
+-rw-r--r--   0        0        0    28128 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/operations/prepare.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/operations/install/__init__.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-r--r--   0        0        0    27311 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/operations/install/wheel.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/req/__init__.py
+-rw-r--r--   0        0        0    19018 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/req/constructors.py
+-rw-r--r--   0        0        0    17790 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/req/req_file.py
+-rw-r--r--   0        0        0    35460 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/req/req_install.py
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/req/req_set.py
+-rw-r--r--   0        0        0    24551 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/req/req_uninstall.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/resolution/__init__.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/resolution/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-r--r--   0        0        0    24025 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/resolution/legacy/resolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-r--r--   0        0        0    21052 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-r--r--   0        0        0    32292 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-r--r--   0        0        0     9824 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-r--r--   0        0        0    12592 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/_jaraco_text.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/_log.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/appdirs.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/compat.py
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/datetime.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/deprecation.py
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/egg_link.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/encoding.py
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/entrypoints.py
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/filesystem.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/filetypes.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/glibc.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/hashes.py
+-rw-r--r--   0        0        0    11603 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/logging.py
+-rw-r--r--   0        0        0    23623 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/misc.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/models.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/packaging.py
+-rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/subprocess.py
+-rw-r--r--   0        0        0     9312 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/temp_dir.py
+-rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/unpacking.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/urls.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/virtualenv.py
+-rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/wheel.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/vcs/__init__.py
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/vcs/bazaar.py
+-rw-r--r--   0        0        0    18121 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/vcs/git.py
+-rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/vcs/mercurial.py
+-rw-r--r--   0        0        0    11729 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/vcs/subversion.py
+-rw-r--r--   0        0        0    22787 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/__init__.py
+-rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/six.py
+-rw-r--r--   0        0        0   111130 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/typing_extensions.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/vendor.txt
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/cache.py
+-rw-r--r--   0        0        0    18384 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/py.typed
+-rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/wrapper.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-r--r--   0        0        0     5352 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/certifi/__init__.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/certifi/__main__.py
+-rw-r--r--   0        0        0   281617 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/certifi/cacert.pem
+-rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/certifi/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/certifi/py.typed
+-rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/__init__.py
+-rw-r--r--   0        0        0    31274 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetprober.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/enums.py
+-rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/escprober.py
+-rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/escsm.py
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-r--r--   0        0        0    13566 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-r--r--   0        0        0    36913 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-r--r--   0        0        0    20735 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-r--r--   0        0        0    14537 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-r--r--   0        0        0    25796 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-r--r--   0        0        0    42498 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/johabfreq.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/johabprober.py
+-rw-r--r--   0        0        0    27055 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-r--r--   0        0        0   104562 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-r--r--   0        0        0    98484 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-r--r--   0        0        0    98196 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-r--r--   0        0        0   101363 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-r--r--   0        0        0   128035 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-r--r--   0        0        0   102774 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-r--r--   0        0        0    95372 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/macromanprober.py
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-r--r--   0        0        0    30391 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcssm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/py.typed
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/resultdict.py
+-rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-r--r--   0        0        0    14848 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/utf1632prober.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-r--r--   0        0        0    13560 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/__init__.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/ansi.py
+-rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/initialise.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/win32.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/winterm.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/__init__.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/ansi_test.py
+-rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
+-rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/initialise_test.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/isatty_test.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/utils.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/winterm_test.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/__init__.py
+-rw-r--r--   0        0        0    41487 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/compat.py
+-rw-r--r--   0        0        0    51965 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/database.py
+-rw-r--r--   0        0        0    20797 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/index.py
+-rw-r--r--   0        0        0    51767 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/locators.py
+-rw-r--r--   0        0        0    14168 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/manifest.py
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/markers.py
+-rw-r--r--   0        0        0    39693 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/metadata.py
+-rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/resources.py
+-rw-r--r--   0        0        0    18315 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/scripts.py
+-rw-r--r--   0        0        0    97792 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/t32.exe
+-rw-r--r--   0        0        0   182784 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/t64-arm.exe
+-rw-r--r--   0        0        0   108032 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/t64.exe
+-rw-r--r--   0        0        0    67530 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/util.py
+-rw-r--r--   0        0        0    23747 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/version.py
+-rw-r--r--   0        0        0    91648 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/w32.exe
+-rw-r--r--   0        0        0   168448 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/w64-arm.exe
+-rw-r--r--   0        0        0   101888 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/w64.exe
+-rw-r--r--   0        0        0    43958 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/wheel.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distro/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distro/__main__.py
+-rw-r--r--   0        0        0    49330 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distro/distro.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distro/py.typed
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/idna/__init__.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/idna/codec.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/idna/compat.py
+-rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/idna/core.py
+-rw-r--r--   0        0        0    44375 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/idna/idnadata.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/idna/intranges.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/idna/package_data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/idna/py.typed
+-rw-r--r--   0        0        0   206539 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/idna/uts46data.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/msgpack/ext.py
+-rw-r--r--   0        0        0    34544 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/msgpack/fallback.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/py.typed
+-rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/version.py
+-rw-r--r--   0        0        0   109364 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pkg_resources/__init__.py
+-rw-r--r--   0        0        0    20155 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/android.py
+-rw-r--r--   0        0        0     7132 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/api.py
+-rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/py.typed
+-rw-r--r--   0        0        0     8809 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/version.py
+-rw-r--r--   0        0        0     9573 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/windows.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/__init__.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/__main__.py
+-rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/cmdline.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/console.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/filter.py
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatter.py
+-rw-r--r--   0        0        0    34618 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexer.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/modeline.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/plugin.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/regexopt.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/scanner.py
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/sphinxext.py
+-rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/style.py
+-rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/token.py
+-rw-r--r--   0        0        0    63223 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/unistring.py
+-rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/util.py
+-rw-r--r--   0        0        0    40386 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rw-r--r--   0        0        0    35610 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/html.py
+-rw-r--r--   0        0        0    21938 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/img.py
+-rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rw-r--r--   0        0        0    19351 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/other.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-r--r--   0        0        0    12130 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-r--r--   0        0        0    72281 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-r--r--   0        0        0    53424 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/python.py
+-rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rw-r--r--   0        0        0     9116 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/__init__.py
+-rw-r--r--   0        0        0     6567 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/actions.py
+-rw-r--r--   0        0        0    13387 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/common.py
+-rw-r--r--   0        0        0   224445 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/core.py
+-rw-r--r--   0        0        0     9523 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0        0        0    38646 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/py.typed
+-rw-r--r--   0        0        0    26692 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/results.py
+-rw-r--r--   0        0        0    13488 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/testing.py
+-rw-r--r--   0        0        0    10646 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/unicode.py
+-rw-r--r--   0        0        0     8670 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/util.py
+-rw-r--r--   0        0        0    24215 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/__init__.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_compat.py
+-rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_impl.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
+-rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
+-rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/requests/__init__.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/requests/__version__.py
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-r--r--   0        0        0    19697 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/requests/adapters.py
+-rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/requests/api.py
+-rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/requests/auth.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/requests/certs.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/requests/compat.py
+-rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/requests/cookies.py
+-rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/requests/exceptions.py
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/requests/help.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/requests/hooks.py
+-rw-r--r--   0        0        0    35288 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/requests/models.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/requests/packages.py
+-rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/requests/sessions.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/requests/status_codes.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/requests/structures.py
+-rw-r--r--   0        0        0    33460 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/requests/utils.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/__init__.py
+-rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/py.typed
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-r--r--   0        0        0    20511 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/structs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/__init__.py
+-rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/__main__.py
+-rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_cell_widths.py
+-rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_export_format.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_extension.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_fileno.py
+-rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_inspect.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_log_render.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_loop.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_null_file.py
+-rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_palettes.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_pick.py
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_ratio.py
+-rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_spinners.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_stack.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_timer.py
+-rw-r--r--   0        0        0    22820 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_win32_console.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_windows.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_windows_renderer.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_wrap.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/abc.py
+-rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/align.py
+-rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/ansi.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/bar.py
+-rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/box.py
+-rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/cells.py
+-rw-r--r--   0        0        0    18224 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/color.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/color_triplet.py
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/columns.py
+-rw-r--r--   0        0        0    99218 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/console.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/constrain.py
+-rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/containers.py
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/control.py
+-rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/default_styles.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/diagnose.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/emoji.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/errors.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/file_proxy.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/filesize.py
+-rw-r--r--   0        0        0     9584 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/highlighter.py
+-rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/json.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/jupyter.py
+-rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/layout.py
+-rw-r--r--   0        0        0    14273 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/live.py
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/live_render.py
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/logging.py
+-rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/markup.py
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/measure.py
+-rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/padding.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/pager.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/palette.py
+-rw-r--r--   0        0        0    10574 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/panel.py
+-rw-r--r--   0        0        0    35852 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/pretty.py
+-rw-r--r--   0        0        0    59706 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/progress.py
+-rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/progress_bar.py
+-rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/prompt.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/protocol.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/py.typed
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/region.py
+-rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/repr.py
+-rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/rule.py
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/scope.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/screen.py
+-rw-r--r--   0        0        0    24247 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/segment.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/spinner.py
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/status.py
+-rw-r--r--   0        0        0    27073 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/style.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/styled.py
+-rw-r--r--   0        0        0    35173 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/syntax.py
+-rw-r--r--   0        0        0    39684 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/table.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/terminal_theme.py
+-rw-r--r--   0        0        0    45525 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/text.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/theme.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/themes.py
+-rw-r--r--   0        0        0    29604 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/traceback.py
+-rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/tree.py
+-rw-r--r--   0        0        0    20493 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/after.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/before.py
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/nap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/py.typed
+-rw-r--r--   0        0        0     8746 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/retry.py
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/stop.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/wait.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/tomli/py.typed
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/truststore/__init__.py
+-rw-r--r--   0        0        0     9893 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/truststore/_api.py
+-rw-r--r--   0        0        0    17694 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/truststore/_macos.py
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/truststore/_openssl.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/truststore/_ssl_constants.py
+-rw-r--r--   0        0        0    17468 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/truststore/_windows.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/truststore/py.typed
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/_version.py
+-rw-r--r--   0        0        0    20300 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/connection.py
+-rw-r--r--   0        0        0    39990 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/connectionpool.py
+-rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/fields.py
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/filepost.py
+-rw-r--r--   0        0        0    19752 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-r--r--   0        0        0     6691 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/request.py
+-rw-r--r--   0        0        0    30641 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+-rw-r--r--   0        0        0    11036 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0        0        0    17081 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0        0        0    34448 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0        0        0    17632 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/__init__.py
+-rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-r--r--   0        0        0    22013 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-r--r--   0        0        0    17177 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0        0        0     6895 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-r--r--   0        0        0    14296 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/wait.py
+-rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/webencodings/labels.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/webencodings/tests.py
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/webencodings/x_user_defined.py
+-rw-r--r--   0        0        0    10388 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip-24.0.dist-info/AUTHORS.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip-24.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip-24.0.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip-24.0.dist-info/METADATA
+-rw-r--r--   0        0        0    78936 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip-24.0.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip-24.0.dist-info/REQUESTED
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip-24.0.dist-info/WHEEL
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip-24.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip-24.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.vscode/extensions.json
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.vscode/settings.json
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/src/eodash_catalog/__about__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/src/eodash_catalog/__init__.py
+-rw-r--r--   0        0        0    11007 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/src/eodash_catalog/duration.py
+-rw-r--r--   0        0        0    61029 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/src/eodash_catalog/generate_indicators.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/src/eodash_catalog/sh_endpoint.py
+-rw-r--r--   0        0        0     6114 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/src/eodash_catalog/utils.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/LICENSE.txt
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/README.md
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 eodash_catalog-0.0.7/PKG-INFO
```

### Comparing `eodash_catalog-0.0.6/.venv/pip.pyz` & `eodash_catalog-0.0.7/.venv/pip.pyz`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/bin/Activate.ps1` & `eodash_catalog-0.0.7/.venv/bin/Activate.ps1`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/bin/activate` & `eodash_catalog-0.0.7/.venv/bin/activate`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/bin/activate.csh` & `eodash_catalog-0.0.7/.venv/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/bin/activate.fish` & `eodash_catalog-0.0.7/.venv/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/__main__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/__pip-runner__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/__pip-runner__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/__init__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/build_env.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/build_env.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/cache.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/configuration.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/configuration.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/exceptions.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/pyproject.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/pyproject.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/self_outdated_check.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/self_outdated_check.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/wheel_builder.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/wheel_builder.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/cli/autocompletion.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/cli/base_command.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/cli/base_command.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/cli/cmdoptions.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/cli/cmdoptions.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/cli/command_context.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/cli/command_context.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/cli/main.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/cli/main_parser.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/cli/main_parser.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/cli/parser.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/cli/parser.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/cli/progress_bars.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/cli/progress_bars.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/cli/req_command.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/cli/req_command.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/cli/spinners.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/cli/spinners.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/__init__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/cache.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/cache.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/check.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/check.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/completion.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/completion.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/configuration.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/configuration.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/debug.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/debug.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/download.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/download.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/freeze.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/hash.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/hash.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/help.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/help.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/index.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/index.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/inspect.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/install.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/install.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/list.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/list.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/search.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/search.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/show.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/show.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/uninstall.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/commands/wheel.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/commands/wheel.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/distributions/__init__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/distributions/base.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/distributions/base.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/distributions/installed.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/distributions/installed.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/distributions/sdist.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/distributions/sdist.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/distributions/wheel.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/distributions/wheel.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/index/collector.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/index/collector.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/index/package_finder.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/index/package_finder.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/index/sources.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/index/sources.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/locations/__init__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/locations/_distutils.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/locations/_distutils.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/locations/_sysconfig.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/locations/_sysconfig.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/locations/base.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/locations/base.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/metadata/__init__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/metadata/_json.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/metadata/_json.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/metadata/base.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/metadata/base.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/metadata/pkg_resources.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/metadata/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_compat.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_compat.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_dists.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_dists.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_envs.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_envs.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/models/candidate.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/models/candidate.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/models/direct_url.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/models/direct_url.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/models/format_control.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/models/format_control.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/models/index.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/models/index.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/models/installation_report.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/models/installation_report.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/models/link.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/models/link.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/models/scheme.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/models/scheme.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/models/search_scope.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/models/search_scope.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/models/selection_prefs.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/models/selection_prefs.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/models/target_python.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/models/target_python.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/models/wheel.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/models/wheel.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/network/auth.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/network/auth.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/network/cache.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/network/cache.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/network/download.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/network/download.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/network/lazy_wheel.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/network/lazy_wheel.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/network/session.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/network/session.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/network/utils.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/network/utils.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/network/xmlrpc.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/network/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/operations/check.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/operations/check.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/operations/freeze.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/operations/freeze.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/operations/prepare.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/operations/prepare.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/operations/install/editable_legacy.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/operations/install/editable_legacy.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/operations/install/wheel.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/operations/install/wheel.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/req/__init__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/req/__init__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/req/constructors.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/req/constructors.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/req/req_file.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/req/req_file.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/req/req_install.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/req/req_install.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/req/req_set.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/req/req_set.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/req/req_uninstall.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/req/req_uninstall.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/resolution/base.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/resolution/base.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/resolution/legacy/resolver.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/resolution/legacy/resolver.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/base.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/base.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/candidates.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/candidates.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/factory.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/factory.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/provider.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/provider.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/reporter.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/reporter.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/requirements.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/requirements.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/resolver.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/resolver.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/_jaraco_text.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/_jaraco_text.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/_log.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/_log.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/appdirs.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/compat.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/compat.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/compatibility_tags.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/deprecation.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/direct_url_helpers.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/direct_url_helpers.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/egg_link.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/egg_link.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/encoding.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/entrypoints.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/entrypoints.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/filesystem.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/filetypes.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/filetypes.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/glibc.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/glibc.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/hashes.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/logging.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/logging.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/misc.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/models.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/models.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/packaging.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/setuptools_build.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/setuptools_build.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/subprocess.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/temp_dir.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/temp_dir.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/unpacking.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/unpacking.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/urls.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/urls.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/virtualenv.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/utils/wheel.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/utils/wheel.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/vcs/__init__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/vcs/bazaar.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/vcs/git.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/vcs/git.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/vcs/mercurial.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/vcs/mercurial.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/vcs/subversion.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/vcs/subversion.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_internal/vcs/versioncontrol.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_internal/vcs/versioncontrol.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/__init__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/six.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/typing_extensions.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/__init__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/_cmd.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/adapter.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/cache.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/controller.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/filewrapper.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/heuristics.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/serialize.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/wrapper.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/wrapper.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/certifi/cacert.pem` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/certifi/core.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/certifi/core.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/__init__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/big5freq.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/big5prober.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/chardistribution.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetgroupprober.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetprober.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/codingstatemachine.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/codingstatemachinedict.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/codingstatemachinedict.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/cp949prober.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/enums.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/escprober.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/escsm.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/eucjpprober.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrfreq.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrprober.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwfreq.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwprober.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312freq.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312prober.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/hebrewprober.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/jisfreq.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/johabfreq.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/johabfreq.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/johabprober.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/johabprober.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/jpcntx.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/langbulgarianmodel.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/langgreekmodel.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/langhebrewmodel.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/langhungarianmodel.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/langrussianmodel.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/langrussianmodel.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/langthaimodel.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/langturkishmodel.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/latin1prober.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/macromanprober.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/macromanprober.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcharsetprober.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcsgroupprober.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcssm.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcharsetprober.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcsgroupprober.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/sjisprober.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/universaldetector.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/utf1632prober.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/utf1632prober.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/utf8prober.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/cli/chardetect.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/languages.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/languages.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/ansi.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/ansitowin32.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/initialise.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/win32.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/winterm.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/ansi_test.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/ansi_test.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/initialise_test.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/initialise_test.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/isatty_test.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/isatty_test.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/utils.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/utils.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/winterm_test.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/winterm_test.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/__init__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/__init__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/compat.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/database.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/database.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/index.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/index.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/locators.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/manifest.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/manifest.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/markers.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/markers.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/metadata.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/metadata.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/resources.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/scripts.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/scripts.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/t32.exe` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/t32.exe`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/t64-arm.exe` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/t64-arm.exe`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/t64.exe` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/t64.exe`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/util.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/util.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/version.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/version.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/w32.exe` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/w32.exe`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/w64-arm.exe` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/w64-arm.exe`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/w64.exe` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/w64.exe`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/wheel.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distro/__init__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distro/__init__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/distro/distro.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/distro/distro.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/idna/__init__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/idna/codec.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/idna/codec.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/idna/core.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/idna/core.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/idna/idnadata.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/idna/intranges.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/idna/uts46data.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/msgpack/__init__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/msgpack/exceptions.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/msgpack/ext.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/msgpack/fallback.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/__about__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/_manylinux.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/_musllinux.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/_structures.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/markers.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/requirements.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/specifiers.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/tags.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/utils.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/version.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pkg_resources/__init__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__init__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__main__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/android.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/api.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/macos.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/unix.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/windows.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/__init__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/cmdline.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/console.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/console.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/filter.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatter.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexer.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/modeline.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/plugin.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/regexopt.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/scanner.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/sphinxext.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/style.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/style.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/token.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/token.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/unistring.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/util.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/util.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/filters/__init__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/__init__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/_mapping.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/bbcode.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/groff.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/groff.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/html.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/img.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/irc.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/latex.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/other.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/rtf.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/svg.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal256.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/__init__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/_mapping.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/python.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/styles/__init__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/__init__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/actions.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/common.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/core.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/exceptions.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/helpers.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/results.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/testing.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/unicode.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/util.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/diagram/__init__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_impl.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_impl.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/requests/__init__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/requests/_internal_utils.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/requests/adapters.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/requests/api.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/requests/auth.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/requests/certs.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/requests/certs.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/requests/compat.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/requests/cookies.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/requests/exceptions.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/requests/help.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/requests/help.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/requests/hooks.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/requests/models.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/requests/packages.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/requests/packages.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/requests/sessions.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/requests/status_codes.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/requests/structures.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/requests/utils.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/__init__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/__init__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/providers.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/providers.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/reporters.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/reporters.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/resolvers.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/resolvers.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/structs.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/structs.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/__init__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/__main__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_cell_widths.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_codes.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_replace.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_replace.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_export_format.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_export_format.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_fileno.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_fileno.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_inspect.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_log_render.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_loop.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_null_file.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_null_file.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_palettes.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_ratio.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_spinners.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_win32_console.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_win32_console.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_windows.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_windows_renderer.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_windows_renderer.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_wrap.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/abc.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/abc.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/align.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/align.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/ansi.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/bar.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/bar.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/box.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/box.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/cells.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/cells.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/color.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/color.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/color_triplet.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/columns.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/columns.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/console.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/console.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/constrain.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/containers.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/containers.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/control.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/control.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/default_styles.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/diagnose.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/diagnose.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/emoji.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/errors.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/errors.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/file_proxy.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/filesize.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/highlighter.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/json.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/json.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/jupyter.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/layout.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/layout.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/live.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/live.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/live_render.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/logging.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/logging.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/markup.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/markup.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/measure.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/measure.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/padding.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/padding.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/pager.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/pager.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/palette.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/palette.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/panel.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/panel.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/pretty.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/progress.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/progress.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/progress_bar.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/prompt.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/protocol.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/repr.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/repr.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/rule.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/rule.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/scope.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/scope.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/screen.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/screen.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/segment.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/segment.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/spinner.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/status.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/status.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/style.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/style.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/styled.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/styled.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/syntax.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/table.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/table.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/terminal_theme.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/text.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/text.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/theme.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/theme.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/traceback.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/rich/tree.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/rich/tree.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/__init__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/__init__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/_asyncio.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/_asyncio.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/_utils.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/_utils.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/after.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/after.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/before.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/before.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/before_sleep.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/before_sleep.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/nap.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/nap.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/retry.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/retry.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/stop.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/stop.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/tornadoweb.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/tornadoweb.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/wait.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/wait.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/tomli/_parser.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/tomli/_re.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/truststore/_api.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/truststore/_api.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/truststore/_macos.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/truststore/_macos.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/truststore/_openssl.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/truststore/_openssl.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/truststore/_ssl_constants.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/truststore/_ssl_constants.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/truststore/_windows.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/truststore/_windows.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/__init__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/_collections.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/connection.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/connectionpool.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/exceptions.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/fields.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/filepost.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/poolmanager.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/request.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/response.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/appengine.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/securetransport.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/socks.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/six.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/__init__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/connection.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/proxy.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/request.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/response.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/retry.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssltransport.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/timeout.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/url.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/wait.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/webencodings/__init__.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/webencodings/labels.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/webencodings/mklabels.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/webencodings/tests.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip/_vendor/webencodings/x_user_defined.py` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip-24.0.dist-info/AUTHORS.txt` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip-24.0.dist-info/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip-24.0.dist-info/LICENSE.txt` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip-24.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip-24.0.dist-info/METADATA` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip-24.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/.venv/lib/python3.10/site-packages/pip-24.0.dist-info/RECORD` & `eodash_catalog-0.0.7/.venv/lib/python3.10/site-packages/pip-24.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/src/eodash_catalog/duration.py` & `eodash_catalog-0.0.7/src/eodash_catalog/duration.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/src/eodash_catalog/generate_indicators.py` & `eodash_catalog-0.0.7/src/eodash_catalog/generate_indicators.py`

 * *Files 0% similar despite different names*

```diff
@@ -358,15 +358,17 @@
     if not endpoint.get("Type") == "OverwriteTimes" or not endpoint.get(
         "OverwriteBBox"
     ):
         # some endpoints allow "narrowed-down" capabilities per-layer, which we utilize to not
         # have to process full service capabilities XML
         capabilities_url = endpoint["EndPoint"]
         spatial_extent, times = retrieveExtentFromWMSWMTS(
-            capabilities_url, endpoint["LayerId"], wmts=wmts
+            capabilities_url, endpoint["LayerId"],
+            version=endpoint.get('Version', '1.1.1'),
+            wmts=wmts,
         )
     # Create an item per time to allow visualization in stac clients
     if len(times) > 0 and not endpoint.get("Disable_Items"):
         for t in times:
             item = Item(
                 id=t,
                 bbox=spatial_extent,
```

### Comparing `eodash_catalog-0.0.6/src/eodash_catalog/sh_endpoint.py` & `eodash_catalog-0.0.7/src/eodash_catalog/sh_endpoint.py`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/src/eodash_catalog/utils.py` & `eodash_catalog-0.0.7/src/eodash_catalog/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,20 +26,20 @@
 
 
 def create_geojson_point(lon, lat):
     point = {"type": "Point", "coordinates": [lon, lat]}
     return {"type": "Feature", "geometry": point, "properties": {}}
 
 
-def retrieveExtentFromWMSWMTS(capabilties_url, layer, wmts=False):
+def retrieveExtentFromWMSWMTS(capabilties_url, layer, version='1.1.1', wmts=False):
     times = []
     service = None
     try:
         if not wmts:
-            service = WebMapService(capabilties_url, version="1.1.1")
+            service = WebMapService(capabilties_url, version=version)
         else:
             service = WebMapTileService(capabilties_url)
         if layer in list(service.contents):
             tps = []
             if not wmts and service[layer].timepositions != None:
                 tps = service[layer].timepositions
             elif wmts:
```

### Comparing `eodash_catalog-0.0.6/LICENSE.txt` & `eodash_catalog-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/README.md` & `eodash_catalog-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/pyproject.toml` & `eodash_catalog-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `eodash_catalog-0.0.6/PKG-INFO` & `eodash_catalog-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodash_catalog
-Version: 0.0.6
+Version: 0.0.7
 Summary: This package is intended to help create a compatible STAC catalog for the eodash dashboard client. It supports configuration of multiple endpoint types for information extraction.
 Project-URL: Documentation, https://github.com/eodash/eodash_catalog#readme
 Project-URL: Issues, https://github.com/eodash/eodash_catalog/issues
 Project-URL: Source, https://github.com/eodash/eodash_catalog
 Author-email: Daniel Santillan <daniel.santillan@eox.at>
 License-Expression: MIT
 License-File: LICENSE.txt
```

