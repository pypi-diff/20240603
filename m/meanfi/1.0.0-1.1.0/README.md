# Comparing `tmp/meanfi-1.0.0.tar.gz` & `tmp/meanfi-1.1.0.tar.gz`

## Comparing `meanfi-1.0.0.tar` & `meanfi-1.1.0.tar`

### file list

```diff
@@ -1,437 +1,444 @@
--rw-r--r--   0        0        0    28740 2020-02-02 00:00:00.000000 meanfi-1.0.0/docs/build/html/_modules/meanfi/mf.html
--rw-r--r--   0        0        0    25300 2020-02-02 00:00:00.000000 meanfi-1.0.0/docs/build/html/_modules/meanfi/model.html
--rw-r--r--   0        0        0    15350 2020-02-02 00:00:00.000000 meanfi-1.0.0/docs/build/html/_modules/meanfi/observables.html
--rw-r--r--   0        0        0    22141 2020-02-02 00:00:00.000000 meanfi-1.0.0/docs/build/html/_modules/meanfi/solvers.html
--rw-r--r--   0        0        0    39144 2020-02-02 00:00:00.000000 meanfi-1.0.0/docs/build/html/_modules/meanfi/kwant_helper/utils.html
--rw-r--r--   0        0        0    17052 2020-02-02 00:00:00.000000 meanfi-1.0.0/docs/build/html/_modules/meanfi/params/rparams.html
--rw-r--r--   0        0        0    18446 2020-02-02 00:00:00.000000 meanfi-1.0.0/docs/build/html/_modules/meanfi/tb/tb.html
--rw-r--r--   0        0        0    24323 2020-02-02 00:00:00.000000 meanfi-1.0.0/docs/build/html/_modules/meanfi/tb/transforms.html
--rw-r--r--   0        0        0    23015 2020-02-02 00:00:00.000000 meanfi-1.0.0/docs/build/html/_modules/meanfi/tb/utils.html
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 meanfi-1.0.0/docs/build/html/_sources/AUTHORS.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/docs/source/AUTHORS.md -> ../../AUTHORS.md
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 meanfi-1.0.0/meanfi/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 meanfi-1.0.0/meanfi/_version.py
--rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 meanfi-1.0.0/meanfi/mf.py
--rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 meanfi-1.0.0/meanfi/model.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 meanfi-1.0.0/meanfi/observables.py
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 meanfi-1.0.0/meanfi/solvers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/meanfi/kwant_helper/__init__.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 meanfi-1.0.0/meanfi/kwant_helper/kwant_examples.py
--rw-r--r--   0        0        0     5637 2020-02-02 00:00:00.000000 meanfi-1.0.0/meanfi/kwant_helper/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/meanfi/params/__init__.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 meanfi-1.0.0/meanfi/params/param_transforms.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 meanfi-1.0.0/meanfi/params/rparams.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/meanfi/tb/__init__.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 meanfi-1.0.0/meanfi/tb/tb.py
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 meanfi-1.0.0/meanfi/tb/transforms.py
--rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 meanfi-1.0.0/meanfi/tb/utils.py
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 meanfi-1.0.0/meanfi/tests/test_graphene.py
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 meanfi-1.0.0/meanfi/tests/test_hat.py
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 meanfi-1.0.0/meanfi/tests/test_hubbard.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 meanfi-1.0.0/meanfi/tests/test_params.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 meanfi-1.0.0/meanfi/tests/test_tb.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 meanfi-1.0.0/meanfi/tests/test_zero_hint.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/Babel-2.14.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/Brotli-1.1.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/PySocks-1.7.1.dist-info/LICENSE
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/PyYAML-6.0.1.dist-info/LICENSE
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/SQLAlchemy-2.0.30.dist-info/LICENSE
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/SecretStorage-3.3.3.dist-info/LICENSE
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/accessible_pygments-0.0.4.dist-info/LICENSE
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/anyio-4.3.0.dist-info/LICENSE
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/asttokens-2.4.1.dist-info/LICENSE
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/attrs-23.2.0.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/backports.tarfile-1.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/beautifulsoup4-4.12.3.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/certifi-2024.2.2.dist-info/LICENSE
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/cffi-1.16.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/charset_normalizer-3.3.2.dist-info/LICENSE
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/comm-0.2.2.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/contourpy-1.2.1.dist-info/LICENSE
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/cryptography-42.0.7.dist-info/LICENSE
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/cycler-0.12.1.dist-info/LICENSE
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/debugpy/_vendored/pydevd/pydevd_plugins/extensions/README.md
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/debugpy-1.8.1.dist-info/LICENSE
--rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/exceptiongroup-1.2.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/fastjsonschema-2.19.1.dist-info/LICENSE
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/filelock-3.14.0.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/fonttools-4.51.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/greenlet-3.0.3.dist-info/LICENSE
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/h2-4.1.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/hyperframe-6.0.1.dist-info/LICENSE
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/hyperlink-21.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/importlib_metadata-7.1.0.dist-info/LICENSE
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/importlib_resources-6.4.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/iniconfig-2.0.0.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/ipykernel-6.29.3.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/ipython-8.22.2.dist-info/LICENSE
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/jaraco.classes-3.4.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/jaraco.context-5.3.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/jaraco.functools-4.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0    12658 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/jedi/third_party/typeshed/LICENSE
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/jeepney-0.8.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/jupyter_cache-1.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/jupyter_client-8.6.1.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/jupyter_core-5.7.2.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/keyring-25.2.0.dist-info/LICENSE
--rw-r--r--   0        0        0     3279 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/kiwisolver-1.4.5.dist-info/LICENSE
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/matplotlib-3.8.4.dist-info/LICENSE
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/matplotlib_inline-0.1.7.dist-info/LICENSE
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/admon/LICENSE
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/container/LICENSE
--rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/container/README.md
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/deflist/LICENSE
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/deflist/README.md
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/footnote/LICENSE
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/front_matter/LICENSE
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/texmath/LICENSE
--rw-r--r--   0        0        0     5191 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/texmath/README.md
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins-0.4.0.dist-info/LICENSE
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdurl-0.1.2.dist-info/LICENSE
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/_version.py
--rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/mf.py
--rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/model.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/observables.py
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/solvers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/kwant_helper/__init__.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/kwant_helper/kwant_examples.py
--rw-r--r--   0        0        0     5637 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/kwant_helper/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/params/__init__.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/params/param_transforms.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/params/rparams.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/tb/__init__.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/tb/tb.py
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/tb/transforms.py
--rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/tb/utils.py
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/tests/test_graphene.py
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/tests/test_hat.py
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/tests/test_hubbard.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/tests/test_params.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/tests/test_tb.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/tests/test_zero_hint.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi-1.0.0.dist-info/licenses/AUTHORS.md
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi-1.0.0.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/more_itertools-10.2.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mpmath-1.3.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/myst_nb-1.1.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/myst_parser-3.0.1.dist-info/LICENSE
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/nbclient-0.10.0.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/nbformat-5.10.4.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/nest_asyncio-1.6.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/numpy/ma/LICENSE
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/packaging-24.0.dist-info/LICENSE
--rw-r--r--   0        0        0    16726 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pathspec-0.12.1.dist-info/LICENSE
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pexpect-4.9.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pickleshare-0.7.5.dist-info/LICENSE
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pillow-10.3.0.dist-info/LICENSE
--rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pkgutil_resolve_name-1.3.10.dist-info/LICENSE
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/platformdirs-4.2.1.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pluggy-1.5.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/prompt_toolkit-3.0.42.dist-info/LICENSE
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/psutil-5.9.8.dist-info/LICENSE
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/ptyprocess-0.7.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pycparser-2.22.dist-info/LICENSE
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pydata_sphinx_theme-0.15.2.dist-info/LICENSE
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pygments-2.18.0.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pyparsing-3.1.2.dist-info/LICENSE
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pytest-8.2.0.dist-info/LICENSE
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/python_dateutil-2.9.0.dist-info/LICENSE
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/qsymm-1.4.0.dist-info/AUTHORS.md
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/qsymm-1.4.0.dist-info/LICENSE
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/requests-2.31.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/rich-13.7.1.dist-info/LICENSE
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/rpds_py-0.18.1.dist-info/license_files/LICENSE
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/scipy/_lib/_uarray/LICENSE
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/setuptools_scm-8.1.0.dist-info/LICENSE
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/shellingham-1.5.4.dist-info/LICENSE
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/six-1.16.0.dist-info/LICENSE
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sniffio-1.3.1.dist-info/LICENSE
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinx_book_theme/assets/translations/README.md
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinx_book_theme-1.1.2.dist-info/LICENSE
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinx_copybutton-0.5.2.dist-info/LICENSE
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinx_tippy-0.4.3.dist-info/LICENSE
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinx_togglebutton-0.3.2.dist-info/LICENSE
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinxcontrib_applehelp-1.0.8.dist-info/LICENSE
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinxcontrib_devhelp-1.0.6.dist-info/LICENSE
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinxcontrib_htmlhelp-2.0.5.dist-info/LICENSE
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinxcontrib_jsmath-1.0.1.dist-info/LICENSE
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinxcontrib_qthelp-1.0.7.dist-info/LICENSE
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinxcontrib_serializinghtml-1.1.10.dist-info/LICENSE
--rw-r--r--   0        0        0     7885 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sympy-1.12.dist-info/LICENSE
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/tabulate-0.9.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/tomli-2.0.1.dist-info/LICENSE
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/tomli_w-1.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/tomlkit-0.12.5.dist-info/LICENSE
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/tornado-6.4.dist-info/LICENSE
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/traitlets-5.14.3.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/trove_classifiers-2024.4.10.dist-info/LICENSE
--rw-r--r--   0        0        0    13936 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/typing_extensions-4.11.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/virtualenv-20.26.1.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/wcwidth-0.2.13.dist-info/LICENSE
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/zipp-3.17.0.dist-info/LICENSE
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/zmq/backend/cffi/README.md
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/zstandard-0.19.0.dist-info/LICENSE
--rw-r--r--   0        0        0    16562 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/envs/meanfi-docs/share/doc/libjpeg-turbo/README.md
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/_openmp_mutex-4.5-2_gnu/info/licenses/LICENSE
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/_openmp_mutex-4.5-2_gnu/info/recipe/parent/LICENSE
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/anyio-4.3.0-pyhd8ed1ab_0/info/licenses/LICENSE
--rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/anyio-4.3.0-pyhd8ed1ab_0/info/test/pyproject.toml
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/anyio-4.3.0-pyhd8ed1ab_0/site-packages/anyio-4.3.0.dist-info/LICENSE
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/asttokens-2.4.1-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/asttokens-2.4.1-pyhd8ed1ab_0/site-packages/asttokens-2.4.1.dist-info/LICENSE
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/attrs-23.2.0-pyh71513ae_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/attrs-23.2.0-pyh71513ae_0/site-packages/attrs-23.2.0.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/babel-2.14.0-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/babel-2.14.0-pyhd8ed1ab_0/site-packages/Babel-2.14.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/backports.tarfile-1.0.0-pyhd8ed1ab_1/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/backports.tarfile-1.0.0-pyhd8ed1ab_1/site-packages/backports.tarfile-1.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/brotli-1.1.0-hd590300_1/info/licenses/LICENSE
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/brotli-bin-1.1.0-hd590300_1/info/licenses/LICENSE
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/brotli-python-1.1.0-py311hb755f60_1/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/brotli-python-1.1.0-py311hb755f60_1/lib/python3.11/site-packages/Brotli-1.1.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/bzip2-1.0.8-hd590300_5/info/licenses/LICENSE
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/ca-certificates-2024.2.2-hbcca054_0/info/licenses/LICENSE
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/certifi-2024.2.2-pyhd8ed1ab_0/info/licenses/certifi/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/certifi-2024.2.2-pyhd8ed1ab_0/site-packages/certifi-2024.2.2.dist-info/LICENSE
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/cffi-1.16.0-py311hb3a22ac_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/cffi-1.16.0-py311hb3a22ac_0/lib/python3.11/site-packages/cffi-1.16.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/charset-normalizer-3.3.2-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/charset-normalizer-3.3.2-pyhd8ed1ab_0/site-packages/charset_normalizer-3.3.2.dist-info/LICENSE
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/comm-0.2.2-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/comm-0.2.2-pyhd8ed1ab_0/site-packages/comm-0.2.2.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/contourpy-1.2.1-py311h9547e67_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/contourpy-1.2.1-py311h9547e67_0/lib/python3.11/site-packages/contourpy-1.2.1.dist-info/LICENSE
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/cryptography-42.0.7-py311h4a61cc7_0/info/licenses/LICENSE
--rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/cryptography-42.0.7-py311h4a61cc7_0/info/test/pyproject.toml
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/cryptography-42.0.7-py311h4a61cc7_0/lib/python3.11/site-packages/cryptography-42.0.7.dist-info/LICENSE
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/cycler-0.12.1-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/cycler-0.12.1-pyhd8ed1ab_0/site-packages/cycler-0.12.1.dist-info/LICENSE
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/debugpy-1.8.1-py311hb755f60_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/debugpy-1.8.1-py311hb755f60_0/lib/python3.11/site-packages/debugpy/_vendored/pydevd/pydevd_plugins/extensions/README.md
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/debugpy-1.8.1-py311hb755f60_0/lib/python3.11/site-packages/debugpy-1.8.1.dist-info/LICENSE
--rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/exceptiongroup-1.2.0-pyhd8ed1ab_2/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/exceptiongroup-1.2.0-pyhd8ed1ab_2/site-packages/exceptiongroup-1.2.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/filelock-3.14.0-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/filelock-3.14.0-pyhd8ed1ab_0/site-packages/filelock-3.14.0.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/fonttools-4.51.0-py311h459d7ec_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/fonttools-4.51.0-py311h459d7ec_0/lib/python3.11/site-packages/fonttools-4.51.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/greenlet-3.0.3-py311hb755f60_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/greenlet-3.0.3-py311hb755f60_0/lib/python3.11/site-packages/greenlet-3.0.3.dist-info/LICENSE
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/h2-4.1.0-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/h2-4.1.0-pyhd8ed1ab_0/site-packages/h2-4.1.0.dist-info/LICENSE
--rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/hatch-1.10.0-pyhd8ed1ab_0/info/test/pyproject.toml
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/hpack-4.0.0-pyh9f0ad1d_0/info/licenses/LICENSE
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/hyperframe-6.0.1-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/hyperframe-6.0.1-pyhd8ed1ab_0/site-packages/hyperframe-6.0.1.dist-info/LICENSE
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/hyperlink-21.0.0-pyhd3deb0d_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/hyperlink-21.0.0-pyhd3deb0d_0/site-packages/hyperlink-21.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/importlib-metadata-7.1.0-pyha770c72_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/importlib-metadata-7.1.0-pyha770c72_0/site-packages/importlib_metadata-7.1.0.dist-info/LICENSE
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/importlib_metadata-7.1.0-hd8ed1ab_0/info/licenses/LICENSE
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/importlib_resources-6.4.0-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/importlib_resources-6.4.0-pyhd8ed1ab_0/site-packages/importlib_resources-6.4.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/iniconfig-2.0.0-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/iniconfig-2.0.0-pyhd8ed1ab_0/site-packages/iniconfig-2.0.0.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/ipykernel-6.29.3-pyhd33586a_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/ipykernel-6.29.3-pyhd33586a_0/site-packages/ipykernel-6.29.3.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/ipython-8.22.2-pyh707e725_0/info/licenses/LICENSE
--rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/ipython-8.22.2-pyh707e725_0/info/test/pyproject.toml
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/ipython-8.22.2-pyh707e725_0/site-packages/ipython-8.22.2.dist-info/LICENSE
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/jaraco.classes-3.4.0-pyhd8ed1ab_1/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/jaraco.classes-3.4.0-pyhd8ed1ab_1/site-packages/jaraco.classes-3.4.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/jaraco.context-5.3.0-pyhd8ed1ab_1/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/jaraco.context-5.3.0-pyhd8ed1ab_1/site-packages/jaraco.context-5.3.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/jaraco.functools-4.0.0-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/jaraco.functools-4.0.0-pyhd8ed1ab_0/site-packages/jaraco.functools-4.0.0.dist-info/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/jedi-0.19.1-pyhd8ed1ab_0/site-packages/jedi/third_party/typeshed/LICENSE
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/jeepney-0.8.0-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/jeepney-0.8.0-pyhd8ed1ab_0/site-packages/jeepney-0.8.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/jupyter-cache-1.0.0-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/jupyter-cache-1.0.0-pyhd8ed1ab_0/site-packages/jupyter_cache-1.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/jupyter_client-8.6.1-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/jupyter_client-8.6.1-pyhd8ed1ab_0/site-packages/jupyter_client-8.6.1.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/jupyter_core-5.7.2-py311h38be061_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/jupyter_core-5.7.2-py311h38be061_0/lib/python3.11/site-packages/jupyter_core-5.7.2.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/keyring-25.2.0-pyha804496_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/keyring-25.2.0-pyha804496_0/site-packages/keyring-25.2.0.dist-info/LICENSE
--rw-r--r--   0        0        0     3279 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/kiwisolver-1.4.5-py311h9547e67_1/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/kiwisolver-1.4.5-py311h9547e67_1/lib/python3.11/site-packages/kiwisolver-1.4.5.dist-info/LICENSE
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/lcms2-2.16-hb7c19ff_0/info/licenses/LICENSE
--rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/lerc-4.0.0-h27087fc_0/info/licenses/LICENSE
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/libbrotlicommon-1.1.0-hd590300_1/info/licenses/LICENSE
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/libbrotlidec-1.1.0-hd590300_1/info/licenses/LICENSE
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/libbrotlienc-1.1.0-hd590300_1/info/licenses/LICENSE
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/libev-4.33-hd590300_2/info/licenses/LICENSE
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/libffi-3.4.2-h7f98852_5/info/licenses/LICENSE
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/libgcc-ng-13.2.0-h77fa898_7/info/recipe/parent/LICENSE
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/libgfortran-ng-13.2.0-h69a702a_7/info/recipe/parent/LICENSE
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/libgfortran5-13.2.0-hca663fb_7/info/recipe/parent/LICENSE
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/libgomp-13.2.0-h77fa898_7/info/recipe/parent/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/libjpeg-turbo-3.0.0-hd590300_1/share/doc/libjpeg-turbo/README.md
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/libopenblas-0.3.27-pthreads_h413a1c8_0/info/licenses/LICENSE
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/libopenblas-0.3.27-pthreads_h413a1c8_0/info/licenses/lapack-netlib/LICENSE
--rw-r--r--   0        0        0     5345 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/libpng-1.6.43-h2797004_0/info/licenses/LICENSE
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/libsodium-1.0.18-h36c2ea0_1/info/licenses/LICENSE
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/libstdcxx-ng-13.2.0-hc0a3c3a_7/info/recipe/parent/LICENSE
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/markdown-it-py-3.0.0-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/markdown-it-py-3.0.0-pyhd8ed1ab_0/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/matplotlib-base-3.8.4-py311h54ef318_0/info/licenses/LICENSE/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/matplotlib-base-3.8.4-py311h54ef318_0/lib/python3.11/site-packages/matplotlib-3.8.4.dist-info/LICENSE
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/matplotlib-inline-0.1.7-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/matplotlib-inline-0.1.7-pyhd8ed1ab_0/site-packages/matplotlib_inline-0.1.7.dist-info/LICENSE
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/mdit-py-plugins-0.4.0-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/mdit-py-plugins-0.4.0-pyhd8ed1ab_0/site-packages/mdit_py_plugins/admon/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/mdit-py-plugins-0.4.0-pyhd8ed1ab_0/site-packages/mdit_py_plugins/container/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/mdit-py-plugins-0.4.0-pyhd8ed1ab_0/site-packages/mdit_py_plugins/container/README.md
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/mdit-py-plugins-0.4.0-pyhd8ed1ab_0/site-packages/mdit_py_plugins/deflist/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/mdit-py-plugins-0.4.0-pyhd8ed1ab_0/site-packages/mdit_py_plugins/deflist/README.md
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/mdit-py-plugins-0.4.0-pyhd8ed1ab_0/site-packages/mdit_py_plugins/footnote/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/mdit-py-plugins-0.4.0-pyhd8ed1ab_0/site-packages/mdit_py_plugins/front_matter/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/mdit-py-plugins-0.4.0-pyhd8ed1ab_0/site-packages/mdit_py_plugins/texmath/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/mdit-py-plugins-0.4.0-pyhd8ed1ab_0/site-packages/mdit_py_plugins/texmath/README.md
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/mdit-py-plugins-0.4.0-pyhd8ed1ab_0/site-packages/mdit_py_plugins-0.4.0.dist-info/LICENSE
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/mdurl-0.1.2-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/mdurl-0.1.2-pyhd8ed1ab_0/site-packages/mdurl-0.1.2.dist-info/LICENSE
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/more-itertools-10.2.0-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/more-itertools-10.2.0-pyhd8ed1ab_0/site-packages/more_itertools-10.2.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/mpmath-1.3.0-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/mpmath-1.3.0-pyhd8ed1ab_0/site-packages/mpmath-1.3.0.dist-info/LICENSE
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/mumps-include-5.7.1-ha770c72_0/info/licenses/LICENSE
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/mumps-seq-5.7.1-h6e8dedb_0/info/licenses/LICENSE
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/munkres-1.1.4-pyh9f0ad1d_0/info/test/test/README.md
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/myst-nb-1.1.0-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/myst-nb-1.1.0-pyhd8ed1ab_0/site-packages/myst_nb-1.1.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/myst-parser-3.0.1-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/myst-parser-3.0.1-pyhd8ed1ab_0/site-packages/myst_parser-3.0.1.dist-info/LICENSE
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/nbclient-0.10.0-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/nbclient-0.10.0-pyhd8ed1ab_0/site-packages/nbclient-0.10.0.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/nbformat-5.10.4-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/nbformat-5.10.4-pyhd8ed1ab_0/site-packages/nbformat-5.10.4.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/nest-asyncio-1.6.0-pyhd8ed1ab_0/info/licenses/LICENSE
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/nest-asyncio-1.6.0-pyhd8ed1ab_0/info/recipe/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/nest-asyncio-1.6.0-pyhd8ed1ab_0/site-packages/nest_asyncio-1.6.0.dist-info/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/numpy-1.26.4-py311h64a7726_0/lib/python3.11/site-packages/numpy/ma/LICENSE
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/openjpeg-2.5.2-h488ebb8_0/info/licenses/LICENSE
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/packaging-24.0-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/packaging-24.0-pyhd8ed1ab_0/site-packages/packaging-24.0.dist-info/LICENSE
--rw-r--r--   0        0        0    16726 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/pathspec-0.12.1-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/pathspec-0.12.1-pyhd8ed1ab_0/site-packages/pathspec-0.12.1.dist-info/LICENSE
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/pexpect-4.9.0-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/pexpect-4.9.0-pyhd8ed1ab_0/site-packages/pexpect-4.9.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/pickleshare-0.7.5-py_1003/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/pickleshare-0.7.5-py_1003/site-packages/pickleshare-0.7.5.dist-info/LICENSE
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/pillow-10.3.0-py311h18e6fac_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/pillow-10.3.0-py311h18e6fac_0/lib/python3.11/site-packages/pillow-10.3.0.dist-info/LICENSE
--rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_1/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_1/site-packages/pkgutil_resolve_name-1.3.10.dist-info/LICENSE
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/platformdirs-4.2.1-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/platformdirs-4.2.1-pyhd8ed1ab_0/site-packages/platformdirs-4.2.1.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/pluggy-1.5.0-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/pluggy-1.5.0-pyhd8ed1ab_0/site-packages/pluggy-1.5.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/prompt-toolkit-3.0.42-pyha770c72_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/prompt-toolkit-3.0.42-pyha770c72_0/site-packages/prompt_toolkit-3.0.42.dist-info/LICENSE
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/psutil-5.9.8-py311h459d7ec_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/psutil-5.9.8-py311h459d7ec_0/lib/python3.11/site-packages/psutil-5.9.8.dist-info/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/ptyprocess-0.7.0-pyhd3deb0d_0/site-packages/ptyprocess-0.7.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/pycparser-2.22-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/pycparser-2.22-pyhd8ed1ab_0/site-packages/pycparser-2.22.dist-info/LICENSE
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/pygments-2.18.0-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/pygments-2.18.0-pyhd8ed1ab_0/site-packages/pygments-2.18.0.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/pyparsing-3.1.2-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/pyparsing-3.1.2-pyhd8ed1ab_0/site-packages/pyparsing-3.1.2.dist-info/LICENSE
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/pysocks-1.7.1-pyha2e5f31_6/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/pysocks-1.7.1-pyha2e5f31_6/site-packages/PySocks-1.7.1.dist-info/LICENSE
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/pytest-8.2.0-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/pytest-8.2.0-pyhd8ed1ab_0/site-packages/pytest-8.2.0.dist-info/LICENSE
--rw-r--r--   0        0        0    13936 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/python-3.11.9-hb806964_0_cpython/info/licenses/LICENSE
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/python-3.11.9-hb806964_0_cpython/info/recipe/parent/patches/README.md
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/python-dateutil-2.9.0-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/python-dateutil-2.9.0-pyhd8ed1ab_0/site-packages/python_dateutil-2.9.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/python-fastjsonschema-2.19.1-pyhd8ed1ab_0/info/licenses/src/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/python-fastjsonschema-2.19.1-pyhd8ed1ab_0/site-packages/fastjsonschema-2.19.1.dist-info/LICENSE
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/python_abi-3.11-4_cp311/info/licenses/LICENSE
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/python_abi-3.11-4_cp311/info/recipe/LICENSE
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/pyyaml-6.0.1-py311h459d7ec_1/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/pyyaml-6.0.1-py311h459d7ec_1/lib/python3.11/site-packages/PyYAML-6.0.1.dist-info/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/pyzmq-26.0.3-py311h08a0b41_0/lib/python3.11/site-packages/zmq/backend/cffi/README.md
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/qsymm-1.4.0-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/qsymm-1.4.0-pyhd8ed1ab_0/site-packages/qsymm-1.4.0.dist-info/AUTHORS.md
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/qsymm-1.4.0-pyhd8ed1ab_0/site-packages/qsymm-1.4.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/referencing-0.35.1-pyhd8ed1ab_0/info/test/suite/LICENSE
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/referencing-0.35.1-pyhd8ed1ab_0/info/test/suite/README.md
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/referencing-0.35.1-pyhd8ed1ab_0/info/test/suite/pyproject.toml
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/requests-2.31.0-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/requests-2.31.0-pyhd8ed1ab_0/site-packages/requests-2.31.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/rich-13.7.1-pyhd8ed1ab_0/info/licenses/dist/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/rich-13.7.1-pyhd8ed1ab_0/site-packages/rich-13.7.1.dist-info/LICENSE
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/rpds-py-0.18.1-py311h5ecf98a_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/rpds-py-0.18.1-py311h5ecf98a_0/lib/python3.11/site-packages/rpds_py-0.18.1.dist-info/license_files/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/scipy-1.13.0-py311h517d4fd_1/lib/python3.11/site-packages/scipy/_lib/_uarray/LICENSE
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/secretstorage-3.3.3-py311h38be061_2/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/secretstorage-3.3.3-py311h38be061_2/lib/python3.11/site-packages/SecretStorage-3.3.3.dist-info/LICENSE
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/setuptools-69.5.1-pyhd8ed1ab_0/info/licenses/LICENSE
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/setuptools-scm-8.1.0-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/setuptools-scm-8.1.0-pyhd8ed1ab_0/site-packages/setuptools_scm-8.1.0.dist-info/LICENSE
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/shellingham-1.5.4-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/shellingham-1.5.4-pyhd8ed1ab_0/site-packages/shellingham-1.5.4.dist-info/LICENSE
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/six-1.16.0-pyh6c4a22f_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/six-1.16.0-pyh6c4a22f_0/site-packages/six-1.16.0.dist-info/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/sniffio-1.3.1-pyhd8ed1ab_0/site-packages/sniffio-1.3.1.dist-info/LICENSE
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/sphinx-copybutton-0.5.2-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/sphinx-copybutton-0.5.2-pyhd8ed1ab_0/site-packages/sphinx_copybutton-0.5.2.dist-info/LICENSE
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/sphinx-togglebutton-0.3.2-pyhd8ed1ab_0/info/licenses/LICENSE
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/sphinx-togglebutton-0.3.2-pyhd8ed1ab_0/info/recipe/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/sphinx-togglebutton-0.3.2-pyhd8ed1ab_0/site-packages/sphinx_togglebutton-0.3.2.dist-info/LICENSE
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/sphinxcontrib-applehelp-1.0.8-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/sphinxcontrib-applehelp-1.0.8-pyhd8ed1ab_0/site-packages/sphinxcontrib_applehelp-1.0.8.dist-info/LICENSE
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/sphinxcontrib-devhelp-1.0.6-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/sphinxcontrib-devhelp-1.0.6-pyhd8ed1ab_0/site-packages/sphinxcontrib_devhelp-1.0.6.dist-info/LICENSE
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/sphinxcontrib-htmlhelp-2.0.5-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/sphinxcontrib-htmlhelp-2.0.5-pyhd8ed1ab_0/site-packages/sphinxcontrib_htmlhelp-2.0.5.dist-info/LICENSE
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/sphinxcontrib-jsmath-1.0.1-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/sphinxcontrib-jsmath-1.0.1-pyhd8ed1ab_0/site-packages/sphinxcontrib_jsmath-1.0.1.dist-info/LICENSE
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/sphinxcontrib-qthelp-1.0.7-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/sphinxcontrib-qthelp-1.0.7-pyhd8ed1ab_0/site-packages/sphinxcontrib_qthelp-1.0.7.dist-info/LICENSE
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/sphinxcontrib-serializinghtml-1.1.10-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/sphinxcontrib-serializinghtml-1.1.10-pyhd8ed1ab_0/site-packages/sphinxcontrib_serializinghtml-1.1.10.dist-info/LICENSE
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/sqlalchemy-2.0.30-py311h331c9d8_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/sqlalchemy-2.0.30-py311h331c9d8_0/lib/python3.11/site-packages/SQLAlchemy-2.0.30.dist-info/LICENSE
--rw-r--r--   0        0        0     7885 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/sympy-1.12-pypyh9d50eac_103/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/sympy-1.12-pypyh9d50eac_103/site-packages/sympy-1.12.dist-info/LICENSE
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/tabulate-0.9.0-pyhd8ed1ab_1/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/tabulate-0.9.0-pyhd8ed1ab_1/site-packages/tabulate-0.9.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/tomli-2.0.1-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/tomli-2.0.1-pyhd8ed1ab_0/site-packages/tomli-2.0.1.dist-info/LICENSE
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/tomli-w-1.0.0-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/tomli-w-1.0.0-pyhd8ed1ab_0/site-packages/tomli_w-1.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/tomlkit-0.12.5-pyha770c72_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/tomlkit-0.12.5-pyha770c72_0/site-packages/tomlkit-0.12.5.dist-info/LICENSE
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/tornado-6.4-py311h459d7ec_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/tornado-6.4-py311h459d7ec_0/lib/python3.11/site-packages/tornado-6.4.dist-info/LICENSE
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/traitlets-5.14.3-pyhd8ed1ab_0/info/licenses/LICENSE
--rw-r--r--   0        0        0     7767 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/traitlets-5.14.3-pyhd8ed1ab_0/info/test/pyproject.toml
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/traitlets-5.14.3-pyhd8ed1ab_0/site-packages/traitlets-5.14.3.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/trove-classifiers-2024.4.10-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/trove-classifiers-2024.4.10-pyhd8ed1ab_0/site-packages/trove_classifiers-2024.4.10.dist-info/LICENSE
--rw-r--r--   0        0        0    13936 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/typing-extensions-4.11.0-hd8ed1ab_0/info/licenses/LICENSE
--rw-r--r--   0        0        0    13936 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/typing_extensions-4.11.0-pyha770c72_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/typing_extensions-4.11.0-pyha770c72_0/site-packages/typing_extensions-4.11.0.dist-info/LICENSE
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/tzdata-2024a-h0c530f3_0/info/licenses/LICENSE
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/virtualenv-20.26.1-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/virtualenv-20.26.1-pyhd8ed1ab_0/site-packages/virtualenv-20.26.1.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/wcwidth-0.2.13-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/wcwidth-0.2.13-pyhd8ed1ab_0/site-packages/wcwidth-0.2.13.dist-info/LICENSE
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/zeromq-4.3.5-h75354e8_3/info/licenses/LICENSE
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/zipp-3.17.0-pyhd8ed1ab_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/zipp-3.17.0-pyhd8ed1ab_0/site-packages/zipp-3.17.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/zstandard-0.19.0-py311hd4cff14_0/info/licenses/LICENSE
-hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/zstandard-0.19.0-py311hd4cff14_0/lib/python3.11/site-packages/zstandard-0.19.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 meanfi-1.0.0/micromamba/pkgs/zstd-1.5.6-ha6fb4c9_0/info/licenses/LICENSE
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 meanfi-1.0.0/.gitignore
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 meanfi-1.0.0/AUTHORS.md
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 meanfi-1.0.0/LICENSE
--rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 meanfi-1.0.0/README.md
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 meanfi-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 meanfi-1.0.0/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/docs/source/AUTHORS.md -> ../../AUTHORS.md
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 meanfi-1.1.0/meanfi/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 meanfi-1.1.0/meanfi/_version.py
+-rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 meanfi-1.1.0/meanfi/mf.py
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 meanfi-1.1.0/meanfi/model.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 meanfi-1.1.0/meanfi/observables.py
+-rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 meanfi-1.1.0/meanfi/solvers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/meanfi/kwant_helper/__init__.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 meanfi-1.1.0/meanfi/kwant_helper/kwant_examples.py
+-rw-r--r--   0        0        0     6703 2020-02-02 00:00:00.000000 meanfi-1.1.0/meanfi/kwant_helper/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/meanfi/params/__init__.py
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 meanfi-1.1.0/meanfi/params/rparams.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/meanfi/tb/__init__.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 meanfi-1.1.0/meanfi/tb/tb.py
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 meanfi-1.1.0/meanfi/tb/transforms.py
+-rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 meanfi-1.1.0/meanfi/tb/utils.py
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 meanfi-1.1.0/meanfi/tests/test_graphene.py
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 meanfi-1.1.0/meanfi/tests/test_hat.py
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 meanfi-1.1.0/meanfi/tests/test_hubbard.py
+-rw-r--r--   0        0        0     4403 2020-02-02 00:00:00.000000 meanfi-1.1.0/meanfi/tests/test_kwant.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 meanfi-1.1.0/meanfi/tests/test_params.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 meanfi-1.1.0/meanfi/tests/test_solvers.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 meanfi-1.1.0/meanfi/tests/test_tb.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 meanfi-1.1.0/meanfi/tests/test_zero_hint.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/Babel-2.14.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/Brotli-1.1.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/PySocks-1.7.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/PyYAML-6.0.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/SQLAlchemy-2.0.30.dist-info/LICENSE
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/SecretStorage-3.3.3.dist-info/LICENSE
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/a11y_pygments/a11y_dark/README.md
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/a11y_pygments/a11y_high_contrast_dark/README.md
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/a11y_pygments/a11y_high_contrast_light/README.md
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/a11y_pygments/a11y_light/README.md
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/a11y_pygments/blinds_dark/README.md
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/a11y_pygments/blinds_light/README.md
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/a11y_pygments/github_dark/README.md
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/a11y_pygments/github_dark_colorblind/README.md
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/a11y_pygments/github_dark_high_contrast/README.md
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/a11y_pygments/github_light/README.md
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/a11y_pygments/github_light_colorblind/README.md
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/a11y_pygments/github_light_high_contrast/README.md
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/a11y_pygments/gotthard_dark/README.md
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/a11y_pygments/gotthard_light/README.md
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/a11y_pygments/greative/README.md
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/a11y_pygments/pitaya_smoothie/README.md
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/accessible_pygments-0.0.5.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/anyio-4.3.0.dist-info/LICENSE
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/asttokens-2.4.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/attrs-23.2.0.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/backports.tarfile-1.0.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/beautifulsoup4-4.12.3.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/certifi-2024.2.2.dist-info/LICENSE
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/cffi-1.16.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/charset_normalizer-3.3.2.dist-info/LICENSE
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/comm-0.2.2.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/contourpy-1.2.1.dist-info/LICENSE
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/cryptography-42.0.7.dist-info/LICENSE
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/cycler-0.12.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/debugpy/_vendored/pydevd/pydevd_plugins/extensions/README.md
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/debugpy-1.8.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/exceptiongroup-1.2.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/fastjsonschema-2.19.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/filelock-3.14.0.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/fonttools-4.53.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/greenlet-3.0.3.dist-info/LICENSE
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/h2-4.1.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/hyperframe-6.0.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/hyperlink-21.0.0.dist-info/LICENSE
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/importlib_metadata-7.1.0.dist-info/LICENSE
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/importlib_resources-6.4.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/iniconfig-2.0.0.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/ipykernel-6.29.3.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/ipython-8.25.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/jaraco.classes-3.4.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/jaraco.context-5.3.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/jaraco.functools-4.0.0.dist-info/LICENSE
+-rw-r--r--   0        0        0    12658 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/jedi/third_party/typeshed/LICENSE
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/jeepney-0.8.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/jupyter_cache-1.0.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/jupyter_client-8.6.2.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/jupyter_core-5.7.2.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/keyring-25.2.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     3279 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/kiwisolver-1.4.5.dist-info/LICENSE
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/matplotlib-3.8.4.dist-info/LICENSE
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/matplotlib_inline-0.1.7.dist-info/LICENSE
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/admon/LICENSE
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/container/LICENSE
+-rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/container/README.md
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/deflist/LICENSE
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/deflist/README.md
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/footnote/LICENSE
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/front_matter/LICENSE
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/texmath/LICENSE
+-rw-r--r--   0        0        0     5191 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/texmath/README.md
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins-0.4.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdurl-0.1.2.dist-info/LICENSE
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/__init__.py
+-rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/mf.py
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/model.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/observables.py
+-rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/solvers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/kwant_helper/__init__.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/kwant_helper/kwant_examples.py
+-rw-r--r--   0        0        0     6703 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/kwant_helper/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/params/__init__.py
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/params/rparams.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/tb/__init__.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/tb/tb.py
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/tb/transforms.py
+-rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/tb/utils.py
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/tests/test_graphene.py
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/tests/test_hat.py
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/tests/test_hubbard.py
+-rw-r--r--   0        0        0     4403 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/tests/test_kwant.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/tests/test_params.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/tests/test_solvers.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/tests/test_tb.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/tests/test_zero_hint.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi-1.1.0.dist-info/licenses/AUTHORS.md
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi-1.1.0.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/more_itertools-10.2.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mpmath-1.3.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/myst_nb-1.1.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/myst_parser-3.0.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/nbclient-0.10.0.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/nbformat-5.10.4.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/nest_asyncio-1.6.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/numpy/ma/LICENSE
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/packaging-24.0.dist-info/LICENSE
+-rw-r--r--   0        0        0    16726 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pathspec-0.12.1.dist-info/LICENSE
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pexpect-4.9.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pickleshare-0.7.5.dist-info/LICENSE
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pillow-10.3.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pkgutil_resolve_name-1.3.10.dist-info/LICENSE
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/platformdirs-4.2.2.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pluggy-1.5.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/prompt_toolkit-3.0.42.dist-info/LICENSE
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/psutil-5.9.8.dist-info/LICENSE
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/ptyprocess-0.7.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pycparser-2.22.dist-info/LICENSE
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pydata_sphinx_theme-0.15.3.dist-info/LICENSE
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pygments-2.18.0.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pyparsing-3.1.2.dist-info/LICENSE
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pytest-8.2.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/python_dateutil-2.9.0.dist-info/LICENSE
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/qsymm-1.4.0.dist-info/AUTHORS.md
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/qsymm-1.4.0.dist-info/LICENSE
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/requests-2.32.3.dist-info/LICENSE
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/rich-13.7.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/rpds_py-0.18.1.dist-info/license_files/LICENSE
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/scipy/_lib/_uarray/LICENSE
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/setuptools_scm-8.1.0.dist-info/LICENSE
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/shellingham-1.5.4.dist-info/LICENSE
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/six-1.16.0.dist-info/LICENSE
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sniffio-1.3.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinx_book_theme/assets/translations/README.md
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinx_book_theme-1.1.2.dist-info/LICENSE
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinx_copybutton-0.5.2.dist-info/LICENSE
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinx_tippy-0.4.3.dist-info/LICENSE
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinx_togglebutton-0.3.2.dist-info/LICENSE
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinxcontrib_applehelp-1.0.8.dist-info/LICENSE
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinxcontrib_devhelp-1.0.6.dist-info/LICENSE
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinxcontrib_htmlhelp-2.0.5.dist-info/LICENSE
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinxcontrib_jsmath-1.0.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinxcontrib_qthelp-1.0.7.dist-info/LICENSE
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinxcontrib_serializinghtml-1.1.10.dist-info/LICENSE
+-rw-r--r--   0        0        0     7885 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sympy-1.12.dist-info/LICENSE
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/tabulate-0.9.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/tomli-2.0.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/tomli_w-1.0.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/tomlkit-0.12.5.dist-info/LICENSE
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/tornado-6.4.dist-info/LICENSE
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/traitlets-5.14.3.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/trove_classifiers-2024.5.22.dist-info/LICENSE
+-rw-r--r--   0        0        0    13936 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/typing_extensions-4.12.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/virtualenv-20.26.2.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/wcwidth-0.2.13.dist-info/LICENSE
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/zipp-3.17.0.dist-info/LICENSE
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/zmq/backend/cffi/README.md
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/zstandard-0.19.0.dist-info/LICENSE
+-rw-r--r--   0        0        0    16562 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/envs/meanfi-docs/share/doc/libjpeg-turbo/README.md
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/_openmp_mutex-4.5-2_gnu/info/licenses/LICENSE
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/_openmp_mutex-4.5-2_gnu/info/recipe/parent/LICENSE
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/anyio-4.3.0-pyhd8ed1ab_0/info/licenses/LICENSE
+-rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/anyio-4.3.0-pyhd8ed1ab_0/info/test/pyproject.toml
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/anyio-4.3.0-pyhd8ed1ab_0/site-packages/anyio-4.3.0.dist-info/LICENSE
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/asttokens-2.4.1-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/asttokens-2.4.1-pyhd8ed1ab_0/site-packages/asttokens-2.4.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/attrs-23.2.0-pyh71513ae_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/attrs-23.2.0-pyh71513ae_0/site-packages/attrs-23.2.0.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/babel-2.14.0-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/babel-2.14.0-pyhd8ed1ab_0/site-packages/Babel-2.14.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/backports.tarfile-1.0.0-pyhd8ed1ab_1/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/backports.tarfile-1.0.0-pyhd8ed1ab_1/site-packages/backports.tarfile-1.0.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/brotli-1.1.0-hd590300_1/info/licenses/LICENSE
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/brotli-bin-1.1.0-hd590300_1/info/licenses/LICENSE
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/brotli-python-1.1.0-py311hb755f60_1/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/brotli-python-1.1.0-py311hb755f60_1/lib/python3.11/site-packages/Brotli-1.1.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/bzip2-1.0.8-hd590300_5/info/licenses/LICENSE
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/ca-certificates-2024.6.2-hbcca054_0/info/licenses/LICENSE
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/certifi-2024.2.2-pyhd8ed1ab_0/info/licenses/certifi/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/certifi-2024.2.2-pyhd8ed1ab_0/site-packages/certifi-2024.2.2.dist-info/LICENSE
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/cffi-1.16.0-py311hb3a22ac_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/cffi-1.16.0-py311hb3a22ac_0/lib/python3.11/site-packages/cffi-1.16.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/charset-normalizer-3.3.2-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/charset-normalizer-3.3.2-pyhd8ed1ab_0/site-packages/charset_normalizer-3.3.2.dist-info/LICENSE
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/comm-0.2.2-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/comm-0.2.2-pyhd8ed1ab_0/site-packages/comm-0.2.2.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/contourpy-1.2.1-py311h9547e67_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/contourpy-1.2.1-py311h9547e67_0/lib/python3.11/site-packages/contourpy-1.2.1.dist-info/LICENSE
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/cryptography-42.0.7-py311h4a61cc7_0/info/licenses/LICENSE
+-rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/cryptography-42.0.7-py311h4a61cc7_0/info/test/pyproject.toml
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/cryptography-42.0.7-py311h4a61cc7_0/lib/python3.11/site-packages/cryptography-42.0.7.dist-info/LICENSE
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/cycler-0.12.1-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/cycler-0.12.1-pyhd8ed1ab_0/site-packages/cycler-0.12.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/debugpy-1.8.1-py311hb755f60_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/debugpy-1.8.1-py311hb755f60_0/lib/python3.11/site-packages/debugpy/_vendored/pydevd/pydevd_plugins/extensions/README.md
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/debugpy-1.8.1-py311hb755f60_0/lib/python3.11/site-packages/debugpy-1.8.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/exceptiongroup-1.2.0-pyhd8ed1ab_2/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/exceptiongroup-1.2.0-pyhd8ed1ab_2/site-packages/exceptiongroup-1.2.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/filelock-3.14.0-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/filelock-3.14.0-pyhd8ed1ab_0/site-packages/filelock-3.14.0.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/fonttools-4.53.0-py311h331c9d8_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/fonttools-4.53.0-py311h331c9d8_0/lib/python3.11/site-packages/fonttools-4.53.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/greenlet-3.0.3-py311hb755f60_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/greenlet-3.0.3-py311hb755f60_0/lib/python3.11/site-packages/greenlet-3.0.3.dist-info/LICENSE
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/h2-4.1.0-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/h2-4.1.0-pyhd8ed1ab_0/site-packages/h2-4.1.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/hatch-1.12.0-pyhd8ed1ab_0/info/test/pyproject.toml
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/hpack-4.0.0-pyh9f0ad1d_0/info/licenses/LICENSE
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/hyperframe-6.0.1-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/hyperframe-6.0.1-pyhd8ed1ab_0/site-packages/hyperframe-6.0.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/hyperlink-21.0.0-pyhd3deb0d_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/hyperlink-21.0.0-pyhd3deb0d_0/site-packages/hyperlink-21.0.0.dist-info/LICENSE
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/importlib-metadata-7.1.0-pyha770c72_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/importlib-metadata-7.1.0-pyha770c72_0/site-packages/importlib_metadata-7.1.0.dist-info/LICENSE
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/importlib_metadata-7.1.0-hd8ed1ab_0/info/licenses/LICENSE
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/importlib_resources-6.4.0-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/importlib_resources-6.4.0-pyhd8ed1ab_0/site-packages/importlib_resources-6.4.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/iniconfig-2.0.0-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/iniconfig-2.0.0-pyhd8ed1ab_0/site-packages/iniconfig-2.0.0.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/ipykernel-6.29.3-pyhd33586a_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/ipykernel-6.29.3-pyhd33586a_0/site-packages/ipykernel-6.29.3.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/ipython-8.25.0-pyh707e725_0/info/licenses/LICENSE
+-rw-r--r--   0        0        0    10223 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/ipython-8.25.0-pyh707e725_0/info/test/pyproject.toml
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/ipython-8.25.0-pyh707e725_0/site-packages/ipython-8.25.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/jaraco.classes-3.4.0-pyhd8ed1ab_1/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/jaraco.classes-3.4.0-pyhd8ed1ab_1/site-packages/jaraco.classes-3.4.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/jaraco.context-5.3.0-pyhd8ed1ab_1/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/jaraco.context-5.3.0-pyhd8ed1ab_1/site-packages/jaraco.context-5.3.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/jaraco.functools-4.0.0-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/jaraco.functools-4.0.0-pyhd8ed1ab_0/site-packages/jaraco.functools-4.0.0.dist-info/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/jedi-0.19.1-pyhd8ed1ab_0/site-packages/jedi/third_party/typeshed/LICENSE
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/jeepney-0.8.0-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/jeepney-0.8.0-pyhd8ed1ab_0/site-packages/jeepney-0.8.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/jupyter-cache-1.0.0-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/jupyter-cache-1.0.0-pyhd8ed1ab_0/site-packages/jupyter_cache-1.0.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/jupyter_client-8.6.2-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/jupyter_client-8.6.2-pyhd8ed1ab_0/site-packages/jupyter_client-8.6.2.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/jupyter_core-5.7.2-py311h38be061_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/jupyter_core-5.7.2-py311h38be061_0/lib/python3.11/site-packages/jupyter_core-5.7.2.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/keyring-25.2.1-pyha804496_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/keyring-25.2.1-pyha804496_0/site-packages/keyring-25.2.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     3279 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/kiwisolver-1.4.5-py311h9547e67_1/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/kiwisolver-1.4.5-py311h9547e67_1/lib/python3.11/site-packages/kiwisolver-1.4.5.dist-info/LICENSE
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/lcms2-2.16-hb7c19ff_0/info/licenses/LICENSE
+-rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/lerc-4.0.0-h27087fc_0/info/licenses/LICENSE
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/libbrotlicommon-1.1.0-hd590300_1/info/licenses/LICENSE
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/libbrotlidec-1.1.0-hd590300_1/info/licenses/LICENSE
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/libbrotlienc-1.1.0-hd590300_1/info/licenses/LICENSE
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/libev-4.33-hd590300_2/info/licenses/LICENSE
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/libffi-3.4.2-h7f98852_5/info/licenses/LICENSE
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/libgcc-ng-13.2.0-h77fa898_7/info/recipe/parent/LICENSE
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/libgfortran-ng-13.2.0-h69a702a_7/info/recipe/parent/LICENSE
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/libgfortran5-13.2.0-hca663fb_7/info/recipe/parent/LICENSE
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/libgomp-13.2.0-h77fa898_7/info/recipe/parent/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/libjpeg-turbo-3.0.0-hd590300_1/share/doc/libjpeg-turbo/README.md
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/libopenblas-0.3.27-pthreads_h413a1c8_0/info/licenses/LICENSE
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/libopenblas-0.3.27-pthreads_h413a1c8_0/info/licenses/lapack-netlib/LICENSE
+-rw-r--r--   0        0        0     5345 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/libpng-1.6.43-h2797004_0/info/licenses/LICENSE
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/libsodium-1.0.18-h36c2ea0_1/info/licenses/LICENSE
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/libstdcxx-ng-13.2.0-hc0a3c3a_7/info/recipe/parent/LICENSE
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/markdown-it-py-3.0.0-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/markdown-it-py-3.0.0-pyhd8ed1ab_0/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/matplotlib-base-3.8.4-py311ha4ca890_2/info/licenses/LICENSE/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/matplotlib-base-3.8.4-py311ha4ca890_2/lib/python3.11/site-packages/matplotlib-3.8.4.dist-info/LICENSE
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/matplotlib-inline-0.1.7-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/matplotlib-inline-0.1.7-pyhd8ed1ab_0/site-packages/matplotlib_inline-0.1.7.dist-info/LICENSE
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/mdit-py-plugins-0.4.1-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/mdit-py-plugins-0.4.1-pyhd8ed1ab_0/site-packages/mdit_py_plugins/admon/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/mdit-py-plugins-0.4.1-pyhd8ed1ab_0/site-packages/mdit_py_plugins/container/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/mdit-py-plugins-0.4.1-pyhd8ed1ab_0/site-packages/mdit_py_plugins/container/README.md
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/mdit-py-plugins-0.4.1-pyhd8ed1ab_0/site-packages/mdit_py_plugins/deflist/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/mdit-py-plugins-0.4.1-pyhd8ed1ab_0/site-packages/mdit_py_plugins/deflist/README.md
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/mdit-py-plugins-0.4.1-pyhd8ed1ab_0/site-packages/mdit_py_plugins/footnote/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/mdit-py-plugins-0.4.1-pyhd8ed1ab_0/site-packages/mdit_py_plugins/front_matter/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/mdit-py-plugins-0.4.1-pyhd8ed1ab_0/site-packages/mdit_py_plugins/texmath/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/mdit-py-plugins-0.4.1-pyhd8ed1ab_0/site-packages/mdit_py_plugins/texmath/README.md
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/mdit-py-plugins-0.4.1-pyhd8ed1ab_0/site-packages/mdit_py_plugins-0.4.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/mdurl-0.1.2-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/mdurl-0.1.2-pyhd8ed1ab_0/site-packages/mdurl-0.1.2.dist-info/LICENSE
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/more-itertools-10.2.0-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/more-itertools-10.2.0-pyhd8ed1ab_0/site-packages/more_itertools-10.2.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/mpmath-1.3.0-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/mpmath-1.3.0-pyhd8ed1ab_0/site-packages/mpmath-1.3.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/mumps-include-5.7.1-ha770c72_0/info/licenses/LICENSE
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/mumps-seq-5.7.1-h6e8dedb_0/info/licenses/LICENSE
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/munkres-1.1.4-pyh9f0ad1d_0/info/test/test/README.md
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/myst-nb-1.1.0-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/myst-nb-1.1.0-pyhd8ed1ab_0/site-packages/myst_nb-1.1.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/myst-parser-3.0.1-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/myst-parser-3.0.1-pyhd8ed1ab_0/site-packages/myst_parser-3.0.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/nbclient-0.10.0-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/nbclient-0.10.0-pyhd8ed1ab_0/site-packages/nbclient-0.10.0.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/nbformat-5.10.4-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/nbformat-5.10.4-pyhd8ed1ab_0/site-packages/nbformat-5.10.4.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/nest-asyncio-1.6.0-pyhd8ed1ab_0/info/licenses/LICENSE
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/nest-asyncio-1.6.0-pyhd8ed1ab_0/info/recipe/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/nest-asyncio-1.6.0-pyhd8ed1ab_0/site-packages/nest_asyncio-1.6.0.dist-info/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/numpy-1.26.4-py311h64a7726_0/lib/python3.11/site-packages/numpy/ma/LICENSE
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/openjpeg-2.5.2-h488ebb8_0/info/licenses/LICENSE
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/packaging-24.0-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/packaging-24.0-pyhd8ed1ab_0/site-packages/packaging-24.0.dist-info/LICENSE
+-rw-r--r--   0        0        0    16726 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/pathspec-0.12.1-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/pathspec-0.12.1-pyhd8ed1ab_0/site-packages/pathspec-0.12.1.dist-info/LICENSE
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/pexpect-4.9.0-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/pexpect-4.9.0-pyhd8ed1ab_0/site-packages/pexpect-4.9.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/pickleshare-0.7.5-py_1003/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/pickleshare-0.7.5-py_1003/site-packages/pickleshare-0.7.5.dist-info/LICENSE
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/pillow-10.3.0-py311h18e6fac_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/pillow-10.3.0-py311h18e6fac_0/lib/python3.11/site-packages/pillow-10.3.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_1/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_1/site-packages/pkgutil_resolve_name-1.3.10.dist-info/LICENSE
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/platformdirs-4.2.2-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/platformdirs-4.2.2-pyhd8ed1ab_0/site-packages/platformdirs-4.2.2.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/pluggy-1.5.0-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/pluggy-1.5.0-pyhd8ed1ab_0/site-packages/pluggy-1.5.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/prompt-toolkit-3.0.42-pyha770c72_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/prompt-toolkit-3.0.42-pyha770c72_0/site-packages/prompt_toolkit-3.0.42.dist-info/LICENSE
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/psutil-5.9.8-py311h459d7ec_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/psutil-5.9.8-py311h459d7ec_0/lib/python3.11/site-packages/psutil-5.9.8.dist-info/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/ptyprocess-0.7.0-pyhd3deb0d_0/site-packages/ptyprocess-0.7.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/pycparser-2.22-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/pycparser-2.22-pyhd8ed1ab_0/site-packages/pycparser-2.22.dist-info/LICENSE
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/pygments-2.18.0-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/pygments-2.18.0-pyhd8ed1ab_0/site-packages/pygments-2.18.0.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/pyparsing-3.1.2-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/pyparsing-3.1.2-pyhd8ed1ab_0/site-packages/pyparsing-3.1.2.dist-info/LICENSE
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/pysocks-1.7.1-pyha2e5f31_6/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/pysocks-1.7.1-pyha2e5f31_6/site-packages/PySocks-1.7.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/pytest-8.2.1-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/pytest-8.2.1-pyhd8ed1ab_0/site-packages/pytest-8.2.1.dist-info/LICENSE
+-rw-r--r--   0        0        0    13936 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/python-3.11.9-hb806964_0_cpython/info/licenses/LICENSE
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/python-3.11.9-hb806964_0_cpython/info/recipe/parent/patches/README.md
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/python-dateutil-2.9.0-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/python-dateutil-2.9.0-pyhd8ed1ab_0/site-packages/python_dateutil-2.9.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/python-fastjsonschema-2.19.1-pyhd8ed1ab_0/info/licenses/src/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/python-fastjsonschema-2.19.1-pyhd8ed1ab_0/site-packages/fastjsonschema-2.19.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/python_abi-3.11-4_cp311/info/licenses/LICENSE
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/python_abi-3.11-4_cp311/info/recipe/LICENSE
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/pyyaml-6.0.1-py311h459d7ec_1/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/pyyaml-6.0.1-py311h459d7ec_1/lib/python3.11/site-packages/PyYAML-6.0.1.dist-info/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/pyzmq-26.0.3-py311h08a0b41_0/lib/python3.11/site-packages/zmq/backend/cffi/README.md
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/qsymm-1.4.0-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/qsymm-1.4.0-pyhd8ed1ab_0/site-packages/qsymm-1.4.0.dist-info/AUTHORS.md
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/qsymm-1.4.0-pyhd8ed1ab_0/site-packages/qsymm-1.4.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/referencing-0.35.1-pyhd8ed1ab_0/info/test/suite/LICENSE
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/referencing-0.35.1-pyhd8ed1ab_0/info/test/suite/README.md
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/referencing-0.35.1-pyhd8ed1ab_0/info/test/suite/pyproject.toml
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/requests-2.32.3-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/requests-2.32.3-pyhd8ed1ab_0/site-packages/requests-2.32.3.dist-info/LICENSE
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/rich-13.7.1-pyhd8ed1ab_0/info/licenses/dist/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/rich-13.7.1-pyhd8ed1ab_0/site-packages/rich-13.7.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/rpds-py-0.18.1-py311h5ecf98a_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/rpds-py-0.18.1-py311h5ecf98a_0/lib/python3.11/site-packages/rpds_py-0.18.1.dist-info/license_files/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/scipy-1.13.1-py311h517d4fd_0/lib/python3.11/site-packages/scipy/_lib/_uarray/LICENSE
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/secretstorage-3.3.3-py311h38be061_2/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/secretstorage-3.3.3-py311h38be061_2/lib/python3.11/site-packages/SecretStorage-3.3.3.dist-info/LICENSE
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/setuptools-70.0.0-pyhd8ed1ab_0/info/licenses/LICENSE
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/setuptools-scm-8.1.0-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/setuptools-scm-8.1.0-pyhd8ed1ab_0/site-packages/setuptools_scm-8.1.0.dist-info/LICENSE
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/shellingham-1.5.4-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/shellingham-1.5.4-pyhd8ed1ab_0/site-packages/shellingham-1.5.4.dist-info/LICENSE
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/six-1.16.0-pyh6c4a22f_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/six-1.16.0-pyh6c4a22f_0/site-packages/six-1.16.0.dist-info/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/sniffio-1.3.1-pyhd8ed1ab_0/site-packages/sniffio-1.3.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/sphinx-copybutton-0.5.2-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/sphinx-copybutton-0.5.2-pyhd8ed1ab_0/site-packages/sphinx_copybutton-0.5.2.dist-info/LICENSE
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/sphinx-togglebutton-0.3.2-pyhd8ed1ab_0/info/licenses/LICENSE
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/sphinx-togglebutton-0.3.2-pyhd8ed1ab_0/info/recipe/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/sphinx-togglebutton-0.3.2-pyhd8ed1ab_0/site-packages/sphinx_togglebutton-0.3.2.dist-info/LICENSE
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/sphinxcontrib-applehelp-1.0.8-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/sphinxcontrib-applehelp-1.0.8-pyhd8ed1ab_0/site-packages/sphinxcontrib_applehelp-1.0.8.dist-info/LICENSE
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/sphinxcontrib-devhelp-1.0.6-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/sphinxcontrib-devhelp-1.0.6-pyhd8ed1ab_0/site-packages/sphinxcontrib_devhelp-1.0.6.dist-info/LICENSE
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/sphinxcontrib-htmlhelp-2.0.5-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/sphinxcontrib-htmlhelp-2.0.5-pyhd8ed1ab_0/site-packages/sphinxcontrib_htmlhelp-2.0.5.dist-info/LICENSE
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/sphinxcontrib-jsmath-1.0.1-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/sphinxcontrib-jsmath-1.0.1-pyhd8ed1ab_0/site-packages/sphinxcontrib_jsmath-1.0.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/sphinxcontrib-qthelp-1.0.7-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/sphinxcontrib-qthelp-1.0.7-pyhd8ed1ab_0/site-packages/sphinxcontrib_qthelp-1.0.7.dist-info/LICENSE
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/sphinxcontrib-serializinghtml-1.1.10-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/sphinxcontrib-serializinghtml-1.1.10-pyhd8ed1ab_0/site-packages/sphinxcontrib_serializinghtml-1.1.10.dist-info/LICENSE
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/sqlalchemy-2.0.30-py311h331c9d8_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/sqlalchemy-2.0.30-py311h331c9d8_0/lib/python3.11/site-packages/SQLAlchemy-2.0.30.dist-info/LICENSE
+-rw-r--r--   0        0        0     7885 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/sympy-1.12-pypyh9d50eac_103/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/sympy-1.12-pypyh9d50eac_103/site-packages/sympy-1.12.dist-info/LICENSE
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/tabulate-0.9.0-pyhd8ed1ab_1/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/tabulate-0.9.0-pyhd8ed1ab_1/site-packages/tabulate-0.9.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/tomli-2.0.1-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/tomli-2.0.1-pyhd8ed1ab_0/site-packages/tomli-2.0.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/tomli-w-1.0.0-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/tomli-w-1.0.0-pyhd8ed1ab_0/site-packages/tomli_w-1.0.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/tomlkit-0.12.5-pyha770c72_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/tomlkit-0.12.5-pyha770c72_0/site-packages/tomlkit-0.12.5.dist-info/LICENSE
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/tornado-6.4-py311h459d7ec_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/tornado-6.4-py311h459d7ec_0/lib/python3.11/site-packages/tornado-6.4.dist-info/LICENSE
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/traitlets-5.14.3-pyhd8ed1ab_0/info/licenses/LICENSE
+-rw-r--r--   0        0        0     7767 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/traitlets-5.14.3-pyhd8ed1ab_0/info/test/pyproject.toml
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/traitlets-5.14.3-pyhd8ed1ab_0/site-packages/traitlets-5.14.3.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/trove-classifiers-2024.5.22-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/trove-classifiers-2024.5.22-pyhd8ed1ab_0/site-packages/trove_classifiers-2024.5.22.dist-info/LICENSE
+-rw-r--r--   0        0        0    13936 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/typing-extensions-4.12.1-hd8ed1ab_0/info/licenses/LICENSE
+-rw-r--r--   0        0        0    13936 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/typing_extensions-4.12.1-pyha770c72_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/typing_extensions-4.12.1-pyha770c72_0/site-packages/typing_extensions-4.12.1.dist-info/LICENSE
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/tzdata-2024a-h0c530f3_0/info/licenses/LICENSE
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/virtualenv-20.26.2-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/virtualenv-20.26.2-pyhd8ed1ab_0/site-packages/virtualenv-20.26.2.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/wcwidth-0.2.13-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/wcwidth-0.2.13-pyhd8ed1ab_0/site-packages/wcwidth-0.2.13.dist-info/LICENSE
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/zeromq-4.3.5-h75354e8_4/info/licenses/LICENSE
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/zipp-3.17.0-pyhd8ed1ab_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/zipp-3.17.0-pyhd8ed1ab_0/site-packages/zipp-3.17.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/zstandard-0.19.0-py311hd4cff14_0/info/licenses/LICENSE
+hrw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/zstandard-0.19.0-py311hd4cff14_0/lib/python3.11/site-packages/zstandard-0.19.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 meanfi-1.1.0/micromamba/pkgs/zstd-1.5.6-ha6fb4c9_0/info/licenses/LICENSE
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 meanfi-1.1.0/.gitignore
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 meanfi-1.1.0/AUTHORS.md
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 meanfi-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 meanfi-1.1.0/README.md
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 meanfi-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 meanfi-1.1.0/PKG-INFO
```

### Comparing `meanfi-1.0.0/docs/build/html/_sources/AUTHORS.md` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi-1.1.0.dist-info/licenses/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/meanfi/__init__.py` & `meanfi-1.1.0/meanfi/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,26 +10,27 @@
     density_matrix,
     meanfield,
 )
 from .solvers import solver
 from .model import Model
 from .observables import expectation_value
 from .tb.tb import add_tb, scale_tb
-from .tb.transforms import tb_to_kgrid, kgrid_to_tb
+from .tb.transforms import tb_to_kgrid, kgrid_to_tb, tb_to_kfunc
 from .tb.utils import guess_tb, fermi_energy
 
 
 __all__ = [
     "solver",
     "Model",
     "expectation_value",
     "add_tb",
     "scale_tb",
     "guess_tb",
     "fermi_energy",
     "density_matrix",
     "meanfield",
     "tb_to_kgrid",
+    "tb_to_kfunc",
     "kgrid_to_tb",
     "__version__",
     "__version_tuple__",
 ]
```

### Comparing `meanfi-1.0.0/meanfi/mf.py` & `meanfi-1.1.0/meanfi/mf.py`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/meanfi/model.py` & `meanfi-1.1.0/meanfi/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -72,14 +72,33 @@
         self._ndim = len(_first_key)
         self._ndof = h_0[_first_key].shape[0]
         self._local_key = tuple(np.zeros((self._ndim,), dtype=int))
 
         _check_hermiticity(h_0)
         _check_hermiticity(h_int)
 
+    def density_matrix(self, rho: _tb_type, nk: int = 20) -> _tb_type:
+        """Computes the density matrix from a given initial density matrix.
+
+        Parameters
+        ----------
+        rho :
+            Initial density matrix tight-binding dictionary.
+        nk :
+            Number of k-points in a grid to sample the Brillouin zone along each dimension.
+            If the system is 0-dimensional (finite), this parameter is ignored.
+
+        Returns
+        -------
+        :
+            Density matrix tight-binding dictionary.
+        """
+        mf = meanfield(rho, self.h_int)
+        return density_matrix(add_tb(self.h_0, mf), self.filling, nk)[0]
+
     def mfield(self, mf: _tb_type, nk: int = 20) -> _tb_type:
         """Computes a new mean-field correction from a given one.
 
         Parameters
         ----------
         mf :
             Initial mean-field correction tight-binding dictionary.
```

### Comparing `meanfi-1.0.0/meanfi/observables.py` & `meanfi-1.1.0/meanfi/observables.py`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/meanfi/solvers.py` & `meanfi-1.1.0/meanfi/solvers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from functools import partial
 import numpy as np
 import scipy
 from typing import Optional, Callable
 
 from meanfi.params.rparams import rparams_to_tb, tb_to_rparams
 from meanfi.tb.tb import add_tb, _tb_type
+from meanfi.mf import density_matrix, meanfield
 from meanfi.model import Model
 from meanfi.tb.utils import fermi_energy
 
 
-def cost(mf_param: np.ndarray, model: Model, nk: int = 20) -> np.ndarray:
+def cost_mf(mf_param: np.ndarray, model: Model, nk: int = 20) -> np.ndarray:
     """Defines the cost function for root solver.
 
     The cost function is the difference between the computed and inputted mean-field.
 
     Parameters
     ----------
     mf_param :
@@ -33,22 +34,54 @@
     shape = model._ndof
     mf = rparams_to_tb(mf_param, list(model.h_int), shape)
     mf_new = model.mfield(mf, nk=nk)
     mf_params_new = tb_to_rparams(mf_new)
     return mf_params_new - mf_param
 
 
-def solver(
+def cost_density(rho_params: np.ndarray, model: Model, nk: int = 20) -> np.ndarray:
+    """Defines the cost function for root solver.
+
+    The cost function is the difference between the computed and inputted density matrix
+    reduced to the hoppings only present in the h_int.
+
+    Parameters
+    ----------
+    rho_params :
+        1D real array that parametrises the density matrix reduced to the
+        hoppings (keys) present in h_int.
+    Model :
+        Interacting tight-binding problem definition.
+    nk :
+        Number of k-points in a grid to sample the Brillouin zone along each dimension.
+        If the system is 0-dimensional (finite), this parameter is ignored.
+
+    Returns
+    -------
+    :
+        1D real array that is the difference between the computed and inputted
+        density matrix parametrisations reduced to the hoppings present in h_int.
+    """
+    shape = model._ndof
+    rho_reduced = rparams_to_tb(rho_params, list(model.h_int), shape)
+    rho_new = model.density_matrix(rho_reduced, nk=nk)
+    rho_reduced_new = {key: rho_new[key] for key in model.h_int}
+    rho_params_new = tb_to_rparams(rho_reduced_new)
+    return rho_params_new - rho_params
+
+
+def solver_mf(
     model: Model,
     mf_guess: np.ndarray,
     nk: int = 20,
     optimizer: Optional[Callable] = scipy.optimize.anderson,
     optimizer_kwargs: Optional[dict[str, str]] = {"M": 0},
 ) -> _tb_type:
-    """Solve for the mean-field correction through self-consistent root finding.
+    """Solve for the mean-field correction through self-consistent root finding
+    by finding the mean-field correction fixed point.
 
     Parameters
     ----------
     model :
         Interacting tight-binding problem definition.
     mf_guess :
         The initial guess for the mean-field correction in the tight-binding dictionary format.
@@ -64,13 +97,62 @@
     Returns
     -------
     :
         Mean-field correction solution in the tight-binding dictionary format.
     """
     shape = model._ndof
     mf_params = tb_to_rparams(mf_guess)
-    f = partial(cost, model=model, nk=nk)
+    f = partial(cost_mf, model=model, nk=nk)
     result = rparams_to_tb(
         optimizer(f, mf_params, **optimizer_kwargs), list(model.h_int), shape
     )
     fermi = fermi_energy(add_tb(model.h_0, result), model.filling, nk=nk)
     return add_tb(result, {model._local_key: -fermi * np.eye(model._ndof)})
+
+
+def solver_density(
+    model: Model,
+    mf_guess: _tb_type,
+    nk: int = 20,
+    optimizer: Optional[Callable] = scipy.optimize.anderson,
+    optimizer_kwargs: Optional[dict[str, str]] = {"M": 0, "line_search": "wolfe"},
+) -> _tb_type:
+    """Solve for the mean-field correction through self-consistent root finding
+    by finding the density matrix fixed point.
+
+    Parameters
+    ----------
+    model :
+        Interacting tight-binding problem definition.
+    mf_guess :
+        The initial guess for the mean-field correction in the tight-binding dictionary format.
+    nk :
+        Number of k-points in a grid to sample the Brillouin zone along each dimension.
+        If the system is 0-dimensional (finite), this parameter is ignored.
+    optimizer :
+        The solver used to solve the fixed point iteration.
+        Default uses `scipy.optimize.anderson`.
+    optimizer_kwargs :
+        The keyword arguments to pass to the optimizer.
+
+    Returns
+    -------
+    :
+        Mean-field correction solution in the tight-binding dictionary format.
+    """
+    shape = model._ndof
+    rho_guess = density_matrix(
+        add_tb(model.h_0, mf_guess), filling=model.filling, nk=nk
+    )[0]
+    rho_guess_reduced = {key: rho_guess[key] for key in model.h_int}
+
+    rho_params = tb_to_rparams(rho_guess_reduced)
+    f = partial(cost_density, model=model, nk=nk)
+    rho_result = rparams_to_tb(
+        optimizer(f, rho_params, **optimizer_kwargs), list(model.h_int), shape
+    )
+    mf_result = meanfield(rho_result, model.h_int)
+    fermi = fermi_energy(add_tb(model.h_0, mf_result), model.filling, nk=nk)
+    return add_tb(mf_result, {model._local_key: -fermi * np.eye(model._ndof)})
+
+
+solver = solver_density
```

### Comparing `meanfi-1.0.0/meanfi/kwant_helper/kwant_examples.py` & `meanfi-1.1.0/meanfi/kwant_helper/kwant_examples.py`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/meanfi/kwant_helper/utils.py` & `meanfi-1.1.0/meanfi/kwant_helper/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-import inspect
-from copy import copy
 from itertools import product
-from typing import Callable
+from typing import Callable, Optional
+import inspect
 
 import numpy as np
 from scipy.sparse import coo_array
 import kwant
+from kwant.builder import Site
 import kwant.lattice
 import kwant.builder
 
+
 from meanfi.tb.tb import _tb_type
 
 
 def builder_to_tb(
     builder: kwant.builder.Builder, params: dict = {}, return_data: bool = False
 ) -> _tb_type:
     """Construct a tight-binding dictionary from a `kwant.builder.Builder` system.
@@ -29,117 +30,153 @@
     Returns
     -------
     :
         Tight-binding dictionary that corresponds to the builder.
     :
         Data with sites and number of orbitals. Only if `return_data=True`.
     """
-    builder = copy(builder)
-    # Extract information from builder
-    dims = len(builder.symmetry.periods)
+    prim_vecs = builder.symmetry.periods
+    dims = len(prim_vecs)
+    sites_list = [*builder.sites()]
+    norbs_list = [site.family.norbs for site in builder.sites()]
+    norbs_list = [1 if norbs is None else norbs for norbs in norbs_list]
+
+    tb_norbs = sum(norbs_list)
+    tb_shape = (tb_norbs, tb_norbs)
     onsite_idx = tuple([0] * dims)
     h_0 = {}
-    sites_list = [*builder.sites()]
-    norbs_list = [site[0].norbs for site in builder.sites()]
-    positions_list = [site[0].pos for site in builder.sites()]
-    norbs_tot = sum(norbs_list)
-    # Extract onsite and hopping matrices.
-    # Based on `kwant.wraparound.wraparound`
-    # Onsite matrices
+
     for site, val in builder.site_value_pairs():
-        site = builder.symmetry.to_fd(site)
-        atom = sites_list.index(site)
-        row = np.sum(norbs_list[:atom]) + range(norbs_list[atom])
-        col = copy(row)
-        row, col = np.array([*product(row, col)]).T
-        try:
-            _params = {}
-            for arg in inspect.getfullargspec(val).args:
-                if arg in params:
-                    _params[arg] = params[arg]
-            val = val(site, **_params)
-            data = val.flatten()
-        except Exception:
-            data = val.flatten()
-        if onsite_idx in h_0:
-            h_0[onsite_idx] += coo_array(
-                (data, (row, col)), shape=(norbs_tot, norbs_tot)
-            ).toarray()
-        else:
-            h_0[onsite_idx] = coo_array(
-                (data, (row, col)), shape=(norbs_tot, norbs_tot)
-            ).toarray()
-    # Hopping matrices
-    for hop, val in builder.hopping_value_pairs():
-        a, b = hop
-        b_dom = builder.symmetry.which(b)
-        b_fd = builder.symmetry.to_fd(b)
-        atoms = np.array([sites_list.index(a), sites_list.index(b_fd)])
-        row, col = [
-            np.sum(norbs_list[: atoms[0]]) + range(norbs_list[atoms[0]]),
-            np.sum(norbs_list[: atoms[1]]) + range(norbs_list[atoms[1]]),
+        site_idx = sites_list.index(site)
+        tb_idx = np.sum(norbs_list[:site_idx]) + range(norbs_list[site_idx])
+        row, col = np.array([*product(tb_idx, tb_idx)]).T
+
+        if callable(val):
+            param_keys = inspect.getfullargspec(val).args[1:]
+            try:
+                val = val(site, *[params[key] for key in param_keys])
+            except KeyError as key:
+                raise KeyError(f"Parameter {key} not found in params.")
+
+        data = np.array(val).flatten()
+        onsite_value = coo_array((data, (row, col)), shape=tb_shape).toarray()
+
+        h_0[onsite_idx] = h_0.get(onsite_idx, 0) + onsite_value
+
+    for (site1, site2), val in builder.hopping_value_pairs():
+        site2_dom = builder.symmetry.which(site2)
+        site2_fd = builder.symmetry.to_fd(site2)
+
+        site1_idx, site2_idx = np.array(
+            [sites_list.index(site1), sites_list.index(site2_fd)]
+        )
+        tb_idx1, tb_idx2 = [
+            np.sum(norbs_list[:site1_idx]) + range(norbs_list[site1_idx]),
+            np.sum(norbs_list[:site2_idx]) + range(norbs_list[site2_idx]),
         ]
-        row, col = np.array([*product(row, col)]).T
-        try:
-            _params = {}
-            for arg in inspect.getfullargspec(val).args:
-                if arg in params:
-                    _params[arg] = params[arg]
-            val = val(a, b, **_params)
-            data = val.flatten()
-        except Exception:
-            data = val.flatten()
-        if tuple(b_dom) in h_0:
-            h_0[tuple(b_dom)] += coo_array(
-                (data, (row, col)), shape=(norbs_tot, norbs_tot)
-            ).toarray()
-            if np.linalg.norm(b_dom) == 0:
-                h_0[tuple(b_dom)] += (
-                    coo_array((data, (row, col)), shape=(norbs_tot, norbs_tot))
-                    .toarray()
-                    .T.conj()
-                )
-            else:
-                # Hopping vector in the opposite direction
-                h_0[tuple(-b_dom)] += (
-                    coo_array((data, (row, col)), shape=(norbs_tot, norbs_tot))
-                    .toarray()
-                    .T.conj()
-                )
-        else:
-            h_0[tuple(b_dom)] = coo_array(
-                (data, (row, col)), shape=(norbs_tot, norbs_tot)
-            ).toarray()
-            if np.linalg.norm(b_dom) == 0:
-                h_0[tuple(b_dom)] += (
-                    coo_array((data, (row, col)), shape=(norbs_tot, norbs_tot))
-                    .toarray()
-                    .T.conj()
-                )
-            else:
-                h_0[tuple(-b_dom)] = (
-                    coo_array((data, (row, col)), shape=(norbs_tot, norbs_tot))
-                    .toarray()
-                    .T.conj()
-                )
+        row, col = np.array([*product(tb_idx1, tb_idx2)]).T
+
+        if callable(val):
+            param_keys = inspect.getfullargspec(val).args[2:]
+            try:
+                val = val(site1, site2, *[params[key] for key in param_keys])
+            except KeyError as key:
+                raise KeyError(f"Parameter {key} not found in params.")
+
+        data = np.array(val).flatten()
+        hopping_value = coo_array((data, (row, col)), shape=tb_shape).toarray()
+
+        hop_key = tuple(site2_dom)
+        hop_key_back = tuple(-site2_dom)
+        h_0[hop_key] = h_0.get(hop_key, 0) + hopping_value
+        h_0[hop_key_back] = h_0.get(hop_key_back, 0) + hopping_value.T.conj()
 
     if return_data:
         data = {}
-        data["norbs"] = norbs_list
-        data["positions"] = positions_list
+        data["periods"] = prim_vecs
+        data["sites"] = sites_list
         return h_0, data
     else:
         return h_0
 
 
+def tb_to_builder(
+    h_0: _tb_type, sites_list: list[Site, ...], periods: np.ndarray
+) -> kwant.builder.Builder:
+    """
+    Construct a `kwant.builder.Builder` from a tight-binding dictionary.
+
+    Parameters
+    ----------
+    h_0 :
+        Tight-binding dictionary.
+    sites_list :
+        List of sites in the builder's unit cell.
+    periods :
+        2d array with periods of the translational symmetry.
+
+    Returns
+    -------
+    :
+        `kwant.builder.Builder` that corresponds to the tight-binding dictionary.
+    """
+
+    builder = kwant.Builder(kwant.TranslationalSymmetry(*periods))
+    onsite_idx = tuple([0] * len(list(h_0)[0]))
+
+    norbs_list = [site.family.norbs for site in sites_list]
+    norbs_list = [1 if norbs is None else norbs for norbs in norbs_list]
+
+    def site_to_tbIdxs(site):
+        site_idx = sites_list.index(site)
+        return (np.sum(norbs_list[:site_idx]) + range(norbs_list[site_idx])).astype(int)
+
+    # assemble the sites first
+    for site in sites_list:
+        tb_idxs = site_to_tbIdxs(site)
+        value = h_0[onsite_idx][
+            tb_idxs[0] : tb_idxs[-1] + 1, tb_idxs[0] : tb_idxs[-1] + 1
+        ]
+        builder[site] = value
+
+    # connect hoppings within the unit-cell
+    for site1, site2 in product(sites_list, sites_list):
+        if site1 == site2:
+            continue
+        tb_idxs1 = site_to_tbIdxs(site1)
+        tb_idxs2 = site_to_tbIdxs(site2)
+        value = h_0[onsite_idx][
+            tb_idxs1[0] : tb_idxs1[-1] + 1, tb_idxs2[0] : tb_idxs2[-1] + 1
+        ]
+        if np.all(value == 0):
+            continue
+        builder[(site1, site2)] = value
+
+    # connect hoppings between unit-cells
+    for key in h_0:
+        if key == onsite_idx:
+            continue
+        for site1, site2_fd in product(sites_list, sites_list):
+            site2 = builder.symmetry.act(key, site2_fd)
+            tb_idxs1 = site_to_tbIdxs(site1)
+            tb_idxs2 = site_to_tbIdxs(site2_fd)
+            value = h_0[key][
+                tb_idxs1[0] : tb_idxs1[-1] + 1, tb_idxs2[0] : tb_idxs2[-1] + 1
+            ]
+            if np.all(value == 0):
+                continue
+            builder[(site1, site2)] = value
+    return builder
+
+
 def build_interacting_syst(
     builder: kwant.builder.Builder,
     lattice: kwant.lattice.Polyatomic,
     func_onsite: Callable,
-    func_hop: Callable,
+    func_hop: Optional[Callable] = None,
     max_neighbor: int = 1,
 ) -> kwant.builder.Builder:
     """
     Construct an auxiliary `kwant` system that encodes the interactions.
 
     Parameters
     ----------
@@ -160,10 +197,11 @@
     :
         Auxiliary `kwant.builder.Builder` that encodes the interactions of the system.
     """
     int_builder = kwant.builder.Builder(
         kwant.lattice.TranslationalSymmetry(*builder.symmetry.periods)
     )
     int_builder[builder.sites()] = func_onsite
-    for neighbors in range(max_neighbor):
-        int_builder[lattice.neighbors(neighbors + 1)] = func_hop
+    if func_hop is not None:
+        for neighbors in range(max_neighbor):
+            int_builder[lattice.neighbors(neighbors + 1)] = func_hop
     return int_builder
```

### Comparing `meanfi-1.0.0/meanfi/params/param_transforms.py` & `meanfi-1.1.0/meanfi/tb/transforms.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,87 +1,107 @@
+import itertools
 import numpy as np
+from typing import Callable
+from scipy.fftpack import ifftn
 
 from meanfi.tb.tb import _tb_type
 
 
-def tb_to_flat(tb: _tb_type) -> np.ndarray:
-    """Parametrise a hermitian tight-binding dictionary by a flat complex vector.
+def tb_to_kgrid(tb: _tb_type, nk: int) -> np.ndarray:
+    """Evaluate a tight-binding dictionary on a k-space grid.
 
     Parameters
     ----------
     tb :
-        Hermitian tigh-binding dictionary
+        Tight-binding dictionary to evaluate on a k-space grid.
+    nk :
+        Number of k-points in a grid to sample the Brillouin zone along each dimension.
+        If the system is 0-dimensional (finite), this parameter is ignored.
 
     Returns
     -------
     :
-        1D complex array that parametrises the tight-binding dictionary.
+        Tight-binding dictionary evaluated on a k-space grid.
+        Has shape (nk, nk, ..., ndof, ndof), where ndof is number of internal degrees of freedom.
     """
-    if len(list(tb)[0]) == 0:
-        matrix = np.array(list(tb.values()))
-        matrix = matrix.reshape((matrix.shape[-2], matrix.shape[-1]))
-        return matrix[np.triu_indices(matrix.shape[-1])].flatten()
-    N = len(tb.keys()) // 2 + 1
-    sorted_vals = np.array(list(tb.values()))[np.lexsort(np.array(list(tb.keys())).T)]
-    return sorted_vals[:N].flatten()
-
-
-def flat_to_tb(
-    tb_param_complex: np.ndarray,
-    ndof: int,
-    tb_keys: list[tuple[None] | tuple[int, ...]],
-) -> _tb_type:
-    """Reverse operation to `tb_to_flat`.
+    ndim = len(list(tb)[0])
+    ks = np.linspace(-np.pi, np.pi, nk, endpoint=False)
+    ks = np.concatenate((ks[nk // 2 :], ks[: nk // 2]), axis=0)  # shift for ifft
+    kgrid = np.meshgrid(*([ks] * ndim), indexing="ij")
+
+    num_keys = len(list(tb.keys()))
+    tb_array = np.array(list(tb.values()))
+    keys = np.array(list(tb.keys()))
+
+    k_dependency = np.exp(-1j * np.tensordot(keys, kgrid, 1))[
+        (...,) + (np.newaxis,) * 2
+    ]
+    tb_array = tb_array.reshape([num_keys] + [1] * ndim + list(tb_array.shape[1:]))
+    return np.sum(tb_array * k_dependency, axis=0)
 
-    It takes a flat complex 1d array and return the tight-binding dictionary.
+
+def kgrid_to_tb(kgrid_array: np.ndarray) -> _tb_type:
+    """
+    Convert a k-space grid array to a tight-binding dictionary.
 
     Parameters
     ----------
-    tb_param_complex :
-        1d complex array that parametrises the tb model.
-    ndof :
-        Number internal degrees of freedom within the unit cell.
-    tb_keys :
-        List of keys of the tight-binding dictionary.
+    kgrid_array :
+        K-space grid array to convert to a tight-binding dictionary.
+        The array should be of shape (nk, nk, ..., ndof, ndof),
+        where ndof is number of internal degrees of freedom.
+    Returns
+    -------
+    :
+        Tight-binding dictionary.
+    """
+    ndim = len(kgrid_array.shape) - 2
+    return ifftn_to_tb(ifftn(kgrid_array, axes=np.arange(ndim)))
+
+
+def ifftn_to_tb(ifft_array: np.ndarray) -> _tb_type:
+    """
+    Convert the result of `scipy.fft.ifftn` to a tight-binding dictionary.
 
+    Parameters
+    ----------
+    ifft_array :
+        Result of `scipy.fft.ifftn` to convert to a tight-binding dictionary.
+        The input to `scipy.fft.ifftn` should be from `tb_to_khamvector`.
     Returns
     -------
-    tb :
-        tight-binding dictionary
+    :
+        Tight-binding dictionary.
     """
-    shape = (len(tb_keys), ndof, ndof)
-    if len(tb_keys[0]) == 0:
-        matrix = np.zeros((shape[-1], shape[-2]), dtype=complex)
-        matrix[np.triu_indices(shape[-1])] = tb_param_complex
-        matrix += matrix.conj().T
-        matrix[np.diag_indices(shape[-1])] /= 2
-        return {(): matrix}
-    matrix = np.zeros(shape, dtype=complex)
-    N = len(tb_keys) // 2 + 1
-    matrix[:N] = tb_param_complex.reshape(N, *shape[1:])
-    matrix[N:] = np.moveaxis(matrix[-(N + 1) :: -1], -1, -2).conj()
-
-    tb_keys = np.array(list(tb_keys))
-    sorted_keys = tb_keys[np.lexsort(tb_keys.T)]
-    tb = dict(zip(map(tuple, sorted_keys), matrix))
-    return tb
+    size = ifft_array.shape[:-2]
 
+    keys = [np.arange(-size[0] // 2 + 1, size[0] // 2) for i in range(len(size))]
+    keys = itertools.product(*keys)
+    return {tuple(k): ifft_array[tuple(k)] for k in keys}
 
-def complex_to_real(z: np.ndarray) -> np.ndarray:
-    """Split and concatenate real and imaginary parts of a complex array.
+
+def tb_to_kfunc(tb: _tb_type) -> Callable:
+    """
+    Fourier transforms a real-space tight-binding model to a k-space function.
 
     Parameters
     ----------
-    z :
-        Complex array.
+    tb :
+        Tight-binding dictionary.
 
     Returns
     -------
     :
-        Real array that concatenates the real and imaginary parts of the input array.
+        A function that takes a k-space vector and returns a complex np.array.
+
+    Notes
+    -----
+    Function doesn't work for zero dimensions.
     """
-    return np.concatenate((np.real(z), np.imag(z)))
 
+    def kfunc(k):
+        ham = 0
+        for vector in tb.keys():
+            ham += tb[vector] * np.exp(-1j * np.dot(k, np.array(vector, dtype=float)))
+        return ham
 
-def real_to_complex(z: np.ndarray) -> np.ndarray:
-    """Undo `complex_to_real`."""
-    return z[: len(z) // 2] + 1j * z[len(z) // 2 :]
+    return kfunc
```

### Comparing `meanfi-1.0.0/meanfi/tb/tb.py` & `meanfi-1.1.0/meanfi/tb/tb.py`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/meanfi/tb/transforms.py` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/tb/transforms.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import itertools
 import numpy as np
+from typing import Callable
 from scipy.fftpack import ifftn
 
 from meanfi.tb.tb import _tb_type
 
 
 def tb_to_kgrid(tb: _tb_type, nk: int) -> np.ndarray:
     """Evaluate a tight-binding dictionary on a k-space grid.
@@ -72,7 +73,35 @@
         Tight-binding dictionary.
     """
     size = ifft_array.shape[:-2]
 
     keys = [np.arange(-size[0] // 2 + 1, size[0] // 2) for i in range(len(size))]
     keys = itertools.product(*keys)
     return {tuple(k): ifft_array[tuple(k)] for k in keys}
+
+
+def tb_to_kfunc(tb: _tb_type) -> Callable:
+    """
+    Fourier transforms a real-space tight-binding model to a k-space function.
+
+    Parameters
+    ----------
+    tb :
+        Tight-binding dictionary.
+
+    Returns
+    -------
+    :
+        A function that takes a k-space vector and returns a complex np.array.
+
+    Notes
+    -----
+    Function doesn't work for zero dimensions.
+    """
+
+    def kfunc(k):
+        ham = 0
+        for vector in tb.keys():
+            ham += tb[vector] * np.exp(-1j * np.dot(k, np.array(vector, dtype=float)))
+        return ham
+
+    return kfunc
```

### Comparing `meanfi-1.0.0/meanfi/tb/utils.py` & `meanfi-1.1.0/meanfi/tb/utils.py`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/meanfi/tests/test_graphene.py` & `meanfi-1.1.0/meanfi/tests/test_graphene.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # %%
 import numpy as np
 import pytest
 
 from meanfi.kwant_helper import kwant_examples, utils
 from meanfi import (
     Model,
+    fermi_energy,
     solver,
     tb_to_kgrid,
     guess_tb,
     add_tb,
 )
 
 
@@ -74,15 +75,17 @@
     nk = 40
 
     h_int = utils.builder_to_tb(int_builder, params)
     guess = guess_tb(frozenset(h_int), len(list(h_0.values())[0]))
     model = Model(h_0, h_int, filling)
 
     mf_sol = solver(model, guess, nk=nk, optimizer_kwargs={"M": 0, "f_tol": 1e-8})
-    gap = compute_gap(add_tb(h_0, mf_sol), nk=200)
+    mf_full = add_tb(h_0, mf_sol)
+    EF = fermi_energy(mf_full, filling=filling, nk=nk)
+    gap = compute_gap(mf_full, fermi_energy=EF, nk=200)
 
     # Check if the gap is predicted correctly
     if gap > 0.1:
         gapped_predicted = True
     else:
         gapped_predicted = False
     assert (
```

### Comparing `meanfi-1.0.0/meanfi/tests/test_hat.py` & `meanfi-1.1.0/meanfi/tests/test_hat.py`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/meanfi/tests/test_hubbard.py` & `meanfi-1.1.0/meanfi/tests/test_hubbard.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # %%
 import numpy as np
 import pytest
 
 from meanfi.tests.test_graphene import compute_gap
 from meanfi import (
     Model,
+    fermi_energy,
     solver,
     guess_tb,
     add_tb,
 )
 
 repeat_number = 3
 
@@ -34,15 +35,17 @@
     for U in Us:
         h_int = {
             (0,): U * np.kron(np.eye(2), np.ones((2, 2))),
         }
         guess = guess_tb(frozenset(h_int), len(list(h_0.values())[0]))
         full_model = Model(h_0, h_int, filling=2)
         mf_sol = solver(full_model, guess, nk=nk)
-        _gap = compute_gap(add_tb(h_0, mf_sol), fermi_energy=0, nk=nk_dense)
+        mf_full = add_tb(h_0, mf_sol)
+        EF = fermi_energy(mf_full, filling=2, nk=nk)
+        _gap = compute_gap(mf_full, fermi_energy=EF, nk=nk_dense)
         gaps.append(_gap)
 
     fit_gap = np.polyfit(Us, np.array(gaps), 1)[0]
     assert np.abs(fit_gap - 1) < tol
 
 
 @pytest.mark.parametrize("seed", range(repeat_number))
```

### Comparing `meanfi-1.0.0/meanfi/tests/test_zero_hint.py` & `meanfi-1.1.0/meanfi/tests/test_zero_hint.py`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/Babel-2.14.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/Babel-2.14.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/Brotli-1.1.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/Brotli-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/PySocks-1.7.1.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/PySocks-1.7.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/PyYAML-6.0.1.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/PyYAML-6.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/SQLAlchemy-2.0.30.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/SQLAlchemy-2.0.30.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/SecretStorage-3.3.3.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/SecretStorage-3.3.3.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/accessible_pygments-0.0.4.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/accessible_pygments-0.0.5.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/anyio-4.3.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/anyio-4.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/asttokens-2.4.1.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/asttokens-2.4.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/attrs-23.2.0.dist-info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/attrs-23.2.0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/backports.tarfile-1.0.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/backports.tarfile-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/beautifulsoup4-4.12.3.dist-info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/beautifulsoup4-4.12.3.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/certifi-2024.2.2.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/certifi-2024.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/cffi-1.16.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/cffi-1.16.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/charset_normalizer-3.3.2.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/charset_normalizer-3.3.2.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/comm-0.2.2.dist-info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/comm-0.2.2.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/contourpy-1.2.1.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/contourpy-1.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/cycler-0.12.1.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/cycler-0.12.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/debugpy/_vendored/pydevd/pydevd_plugins/extensions/README.md` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/debugpy/_vendored/pydevd/pydevd_plugins/extensions/README.md`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/debugpy-1.8.1.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/debugpy-1.8.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/exceptiongroup-1.2.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/exceptiongroup-1.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/fastjsonschema-2.19.1.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/fastjsonschema-2.19.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/filelock-3.14.0.dist-info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/filelock-3.14.0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/fonttools-4.51.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/fonttools-4.53.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/greenlet-3.0.3.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/greenlet-3.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/h2-4.1.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/h2-4.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/hyperframe-6.0.1.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/hyperframe-6.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/hyperlink-21.0.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/hyperlink-21.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/importlib_metadata-7.1.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/importlib_metadata-7.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/importlib_resources-6.4.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/importlib_resources-6.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/iniconfig-2.0.0.dist-info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/iniconfig-2.0.0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/ipykernel-6.29.3.dist-info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/ipykernel-6.29.3.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/ipython-8.22.2.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/ipython-8.25.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/jaraco.classes-3.4.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/jaraco.classes-3.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/jaraco.context-5.3.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/jaraco.context-5.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/jaraco.functools-4.0.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/jaraco.functools-4.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/jedi/third_party/typeshed/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/jedi/third_party/typeshed/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/jeepney-0.8.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/jeepney-0.8.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/jupyter_cache-1.0.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/jupyter_cache-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/jupyter_client-8.6.1.dist-info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/jupyter_client-8.6.2.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/jupyter_core-5.7.2.dist-info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/jupyter_core-5.7.2.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/keyring-25.2.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/keyring-25.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/kiwisolver-1.4.5.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/kiwisolver-1.4.5.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/matplotlib-3.8.4.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/matplotlib-3.8.4.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/matplotlib_inline-0.1.7.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/matplotlib_inline-0.1.7.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/admon/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/admon/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/container/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/container/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/container/README.md` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/container/README.md`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/deflist/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/deflist/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/deflist/README.md` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/deflist/README.md`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/footnote/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/footnote/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/front_matter/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/front_matter/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/texmath/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/texmath/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/texmath/README.md` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins/texmath/README.md`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins-0.4.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdit_py_plugins-0.4.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdurl-0.1.2.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mdurl-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/__init__.py` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,26 +10,27 @@
     density_matrix,
     meanfield,
 )
 from .solvers import solver
 from .model import Model
 from .observables import expectation_value
 from .tb.tb import add_tb, scale_tb
-from .tb.transforms import tb_to_kgrid, kgrid_to_tb
+from .tb.transforms import tb_to_kgrid, kgrid_to_tb, tb_to_kfunc
 from .tb.utils import guess_tb, fermi_energy
 
 
 __all__ = [
     "solver",
     "Model",
     "expectation_value",
     "add_tb",
     "scale_tb",
     "guess_tb",
     "fermi_energy",
     "density_matrix",
     "meanfield",
     "tb_to_kgrid",
+    "tb_to_kfunc",
     "kgrid_to_tb",
     "__version__",
     "__version_tuple__",
 ]
```

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/mf.py` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/mf.py`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/model.py` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -72,14 +72,33 @@
         self._ndim = len(_first_key)
         self._ndof = h_0[_first_key].shape[0]
         self._local_key = tuple(np.zeros((self._ndim,), dtype=int))
 
         _check_hermiticity(h_0)
         _check_hermiticity(h_int)
 
+    def density_matrix(self, rho: _tb_type, nk: int = 20) -> _tb_type:
+        """Computes the density matrix from a given initial density matrix.
+
+        Parameters
+        ----------
+        rho :
+            Initial density matrix tight-binding dictionary.
+        nk :
+            Number of k-points in a grid to sample the Brillouin zone along each dimension.
+            If the system is 0-dimensional (finite), this parameter is ignored.
+
+        Returns
+        -------
+        :
+            Density matrix tight-binding dictionary.
+        """
+        mf = meanfield(rho, self.h_int)
+        return density_matrix(add_tb(self.h_0, mf), self.filling, nk)[0]
+
     def mfield(self, mf: _tb_type, nk: int = 20) -> _tb_type:
         """Computes a new mean-field correction from a given one.
 
         Parameters
         ----------
         mf :
             Initial mean-field correction tight-binding dictionary.
```

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/observables.py` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/observables.py`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/solvers.py` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/solvers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from functools import partial
 import numpy as np
 import scipy
 from typing import Optional, Callable
 
 from meanfi.params.rparams import rparams_to_tb, tb_to_rparams
 from meanfi.tb.tb import add_tb, _tb_type
+from meanfi.mf import density_matrix, meanfield
 from meanfi.model import Model
 from meanfi.tb.utils import fermi_energy
 
 
-def cost(mf_param: np.ndarray, model: Model, nk: int = 20) -> np.ndarray:
+def cost_mf(mf_param: np.ndarray, model: Model, nk: int = 20) -> np.ndarray:
     """Defines the cost function for root solver.
 
     The cost function is the difference between the computed and inputted mean-field.
 
     Parameters
     ----------
     mf_param :
@@ -33,22 +34,54 @@
     shape = model._ndof
     mf = rparams_to_tb(mf_param, list(model.h_int), shape)
     mf_new = model.mfield(mf, nk=nk)
     mf_params_new = tb_to_rparams(mf_new)
     return mf_params_new - mf_param
 
 
-def solver(
+def cost_density(rho_params: np.ndarray, model: Model, nk: int = 20) -> np.ndarray:
+    """Defines the cost function for root solver.
+
+    The cost function is the difference between the computed and inputted density matrix
+    reduced to the hoppings only present in the h_int.
+
+    Parameters
+    ----------
+    rho_params :
+        1D real array that parametrises the density matrix reduced to the
+        hoppings (keys) present in h_int.
+    Model :
+        Interacting tight-binding problem definition.
+    nk :
+        Number of k-points in a grid to sample the Brillouin zone along each dimension.
+        If the system is 0-dimensional (finite), this parameter is ignored.
+
+    Returns
+    -------
+    :
+        1D real array that is the difference between the computed and inputted
+        density matrix parametrisations reduced to the hoppings present in h_int.
+    """
+    shape = model._ndof
+    rho_reduced = rparams_to_tb(rho_params, list(model.h_int), shape)
+    rho_new = model.density_matrix(rho_reduced, nk=nk)
+    rho_reduced_new = {key: rho_new[key] for key in model.h_int}
+    rho_params_new = tb_to_rparams(rho_reduced_new)
+    return rho_params_new - rho_params
+
+
+def solver_mf(
     model: Model,
     mf_guess: np.ndarray,
     nk: int = 20,
     optimizer: Optional[Callable] = scipy.optimize.anderson,
     optimizer_kwargs: Optional[dict[str, str]] = {"M": 0},
 ) -> _tb_type:
-    """Solve for the mean-field correction through self-consistent root finding.
+    """Solve for the mean-field correction through self-consistent root finding
+    by finding the mean-field correction fixed point.
 
     Parameters
     ----------
     model :
         Interacting tight-binding problem definition.
     mf_guess :
         The initial guess for the mean-field correction in the tight-binding dictionary format.
@@ -64,13 +97,62 @@
     Returns
     -------
     :
         Mean-field correction solution in the tight-binding dictionary format.
     """
     shape = model._ndof
     mf_params = tb_to_rparams(mf_guess)
-    f = partial(cost, model=model, nk=nk)
+    f = partial(cost_mf, model=model, nk=nk)
     result = rparams_to_tb(
         optimizer(f, mf_params, **optimizer_kwargs), list(model.h_int), shape
     )
     fermi = fermi_energy(add_tb(model.h_0, result), model.filling, nk=nk)
     return add_tb(result, {model._local_key: -fermi * np.eye(model._ndof)})
+
+
+def solver_density(
+    model: Model,
+    mf_guess: _tb_type,
+    nk: int = 20,
+    optimizer: Optional[Callable] = scipy.optimize.anderson,
+    optimizer_kwargs: Optional[dict[str, str]] = {"M": 0, "line_search": "wolfe"},
+) -> _tb_type:
+    """Solve for the mean-field correction through self-consistent root finding
+    by finding the density matrix fixed point.
+
+    Parameters
+    ----------
+    model :
+        Interacting tight-binding problem definition.
+    mf_guess :
+        The initial guess for the mean-field correction in the tight-binding dictionary format.
+    nk :
+        Number of k-points in a grid to sample the Brillouin zone along each dimension.
+        If the system is 0-dimensional (finite), this parameter is ignored.
+    optimizer :
+        The solver used to solve the fixed point iteration.
+        Default uses `scipy.optimize.anderson`.
+    optimizer_kwargs :
+        The keyword arguments to pass to the optimizer.
+
+    Returns
+    -------
+    :
+        Mean-field correction solution in the tight-binding dictionary format.
+    """
+    shape = model._ndof
+    rho_guess = density_matrix(
+        add_tb(model.h_0, mf_guess), filling=model.filling, nk=nk
+    )[0]
+    rho_guess_reduced = {key: rho_guess[key] for key in model.h_int}
+
+    rho_params = tb_to_rparams(rho_guess_reduced)
+    f = partial(cost_density, model=model, nk=nk)
+    rho_result = rparams_to_tb(
+        optimizer(f, rho_params, **optimizer_kwargs), list(model.h_int), shape
+    )
+    mf_result = meanfield(rho_result, model.h_int)
+    fermi = fermi_energy(add_tb(model.h_0, mf_result), model.filling, nk=nk)
+    return add_tb(mf_result, {model._local_key: -fermi * np.eye(model._ndof)})
+
+
+solver = solver_density
```

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/kwant_helper/kwant_examples.py` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/kwant_helper/kwant_examples.py`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/kwant_helper/utils.py` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/kwant_helper/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-import inspect
-from copy import copy
 from itertools import product
-from typing import Callable
+from typing import Callable, Optional
+import inspect
 
 import numpy as np
 from scipy.sparse import coo_array
 import kwant
+from kwant.builder import Site
 import kwant.lattice
 import kwant.builder
 
+
 from meanfi.tb.tb import _tb_type
 
 
 def builder_to_tb(
     builder: kwant.builder.Builder, params: dict = {}, return_data: bool = False
 ) -> _tb_type:
     """Construct a tight-binding dictionary from a `kwant.builder.Builder` system.
@@ -29,117 +30,153 @@
     Returns
     -------
     :
         Tight-binding dictionary that corresponds to the builder.
     :
         Data with sites and number of orbitals. Only if `return_data=True`.
     """
-    builder = copy(builder)
-    # Extract information from builder
-    dims = len(builder.symmetry.periods)
+    prim_vecs = builder.symmetry.periods
+    dims = len(prim_vecs)
+    sites_list = [*builder.sites()]
+    norbs_list = [site.family.norbs for site in builder.sites()]
+    norbs_list = [1 if norbs is None else norbs for norbs in norbs_list]
+
+    tb_norbs = sum(norbs_list)
+    tb_shape = (tb_norbs, tb_norbs)
     onsite_idx = tuple([0] * dims)
     h_0 = {}
-    sites_list = [*builder.sites()]
-    norbs_list = [site[0].norbs for site in builder.sites()]
-    positions_list = [site[0].pos for site in builder.sites()]
-    norbs_tot = sum(norbs_list)
-    # Extract onsite and hopping matrices.
-    # Based on `kwant.wraparound.wraparound`
-    # Onsite matrices
+
     for site, val in builder.site_value_pairs():
-        site = builder.symmetry.to_fd(site)
-        atom = sites_list.index(site)
-        row = np.sum(norbs_list[:atom]) + range(norbs_list[atom])
-        col = copy(row)
-        row, col = np.array([*product(row, col)]).T
-        try:
-            _params = {}
-            for arg in inspect.getfullargspec(val).args:
-                if arg in params:
-                    _params[arg] = params[arg]
-            val = val(site, **_params)
-            data = val.flatten()
-        except Exception:
-            data = val.flatten()
-        if onsite_idx in h_0:
-            h_0[onsite_idx] += coo_array(
-                (data, (row, col)), shape=(norbs_tot, norbs_tot)
-            ).toarray()
-        else:
-            h_0[onsite_idx] = coo_array(
-                (data, (row, col)), shape=(norbs_tot, norbs_tot)
-            ).toarray()
-    # Hopping matrices
-    for hop, val in builder.hopping_value_pairs():
-        a, b = hop
-        b_dom = builder.symmetry.which(b)
-        b_fd = builder.symmetry.to_fd(b)
-        atoms = np.array([sites_list.index(a), sites_list.index(b_fd)])
-        row, col = [
-            np.sum(norbs_list[: atoms[0]]) + range(norbs_list[atoms[0]]),
-            np.sum(norbs_list[: atoms[1]]) + range(norbs_list[atoms[1]]),
+        site_idx = sites_list.index(site)
+        tb_idx = np.sum(norbs_list[:site_idx]) + range(norbs_list[site_idx])
+        row, col = np.array([*product(tb_idx, tb_idx)]).T
+
+        if callable(val):
+            param_keys = inspect.getfullargspec(val).args[1:]
+            try:
+                val = val(site, *[params[key] for key in param_keys])
+            except KeyError as key:
+                raise KeyError(f"Parameter {key} not found in params.")
+
+        data = np.array(val).flatten()
+        onsite_value = coo_array((data, (row, col)), shape=tb_shape).toarray()
+
+        h_0[onsite_idx] = h_0.get(onsite_idx, 0) + onsite_value
+
+    for (site1, site2), val in builder.hopping_value_pairs():
+        site2_dom = builder.symmetry.which(site2)
+        site2_fd = builder.symmetry.to_fd(site2)
+
+        site1_idx, site2_idx = np.array(
+            [sites_list.index(site1), sites_list.index(site2_fd)]
+        )
+        tb_idx1, tb_idx2 = [
+            np.sum(norbs_list[:site1_idx]) + range(norbs_list[site1_idx]),
+            np.sum(norbs_list[:site2_idx]) + range(norbs_list[site2_idx]),
         ]
-        row, col = np.array([*product(row, col)]).T
-        try:
-            _params = {}
-            for arg in inspect.getfullargspec(val).args:
-                if arg in params:
-                    _params[arg] = params[arg]
-            val = val(a, b, **_params)
-            data = val.flatten()
-        except Exception:
-            data = val.flatten()
-        if tuple(b_dom) in h_0:
-            h_0[tuple(b_dom)] += coo_array(
-                (data, (row, col)), shape=(norbs_tot, norbs_tot)
-            ).toarray()
-            if np.linalg.norm(b_dom) == 0:
-                h_0[tuple(b_dom)] += (
-                    coo_array((data, (row, col)), shape=(norbs_tot, norbs_tot))
-                    .toarray()
-                    .T.conj()
-                )
-            else:
-                # Hopping vector in the opposite direction
-                h_0[tuple(-b_dom)] += (
-                    coo_array((data, (row, col)), shape=(norbs_tot, norbs_tot))
-                    .toarray()
-                    .T.conj()
-                )
-        else:
-            h_0[tuple(b_dom)] = coo_array(
-                (data, (row, col)), shape=(norbs_tot, norbs_tot)
-            ).toarray()
-            if np.linalg.norm(b_dom) == 0:
-                h_0[tuple(b_dom)] += (
-                    coo_array((data, (row, col)), shape=(norbs_tot, norbs_tot))
-                    .toarray()
-                    .T.conj()
-                )
-            else:
-                h_0[tuple(-b_dom)] = (
-                    coo_array((data, (row, col)), shape=(norbs_tot, norbs_tot))
-                    .toarray()
-                    .T.conj()
-                )
+        row, col = np.array([*product(tb_idx1, tb_idx2)]).T
+
+        if callable(val):
+            param_keys = inspect.getfullargspec(val).args[2:]
+            try:
+                val = val(site1, site2, *[params[key] for key in param_keys])
+            except KeyError as key:
+                raise KeyError(f"Parameter {key} not found in params.")
+
+        data = np.array(val).flatten()
+        hopping_value = coo_array((data, (row, col)), shape=tb_shape).toarray()
+
+        hop_key = tuple(site2_dom)
+        hop_key_back = tuple(-site2_dom)
+        h_0[hop_key] = h_0.get(hop_key, 0) + hopping_value
+        h_0[hop_key_back] = h_0.get(hop_key_back, 0) + hopping_value.T.conj()
 
     if return_data:
         data = {}
-        data["norbs"] = norbs_list
-        data["positions"] = positions_list
+        data["periods"] = prim_vecs
+        data["sites"] = sites_list
         return h_0, data
     else:
         return h_0
 
 
+def tb_to_builder(
+    h_0: _tb_type, sites_list: list[Site, ...], periods: np.ndarray
+) -> kwant.builder.Builder:
+    """
+    Construct a `kwant.builder.Builder` from a tight-binding dictionary.
+
+    Parameters
+    ----------
+    h_0 :
+        Tight-binding dictionary.
+    sites_list :
+        List of sites in the builder's unit cell.
+    periods :
+        2d array with periods of the translational symmetry.
+
+    Returns
+    -------
+    :
+        `kwant.builder.Builder` that corresponds to the tight-binding dictionary.
+    """
+
+    builder = kwant.Builder(kwant.TranslationalSymmetry(*periods))
+    onsite_idx = tuple([0] * len(list(h_0)[0]))
+
+    norbs_list = [site.family.norbs for site in sites_list]
+    norbs_list = [1 if norbs is None else norbs for norbs in norbs_list]
+
+    def site_to_tbIdxs(site):
+        site_idx = sites_list.index(site)
+        return (np.sum(norbs_list[:site_idx]) + range(norbs_list[site_idx])).astype(int)
+
+    # assemble the sites first
+    for site in sites_list:
+        tb_idxs = site_to_tbIdxs(site)
+        value = h_0[onsite_idx][
+            tb_idxs[0] : tb_idxs[-1] + 1, tb_idxs[0] : tb_idxs[-1] + 1
+        ]
+        builder[site] = value
+
+    # connect hoppings within the unit-cell
+    for site1, site2 in product(sites_list, sites_list):
+        if site1 == site2:
+            continue
+        tb_idxs1 = site_to_tbIdxs(site1)
+        tb_idxs2 = site_to_tbIdxs(site2)
+        value = h_0[onsite_idx][
+            tb_idxs1[0] : tb_idxs1[-1] + 1, tb_idxs2[0] : tb_idxs2[-1] + 1
+        ]
+        if np.all(value == 0):
+            continue
+        builder[(site1, site2)] = value
+
+    # connect hoppings between unit-cells
+    for key in h_0:
+        if key == onsite_idx:
+            continue
+        for site1, site2_fd in product(sites_list, sites_list):
+            site2 = builder.symmetry.act(key, site2_fd)
+            tb_idxs1 = site_to_tbIdxs(site1)
+            tb_idxs2 = site_to_tbIdxs(site2_fd)
+            value = h_0[key][
+                tb_idxs1[0] : tb_idxs1[-1] + 1, tb_idxs2[0] : tb_idxs2[-1] + 1
+            ]
+            if np.all(value == 0):
+                continue
+            builder[(site1, site2)] = value
+    return builder
+
+
 def build_interacting_syst(
     builder: kwant.builder.Builder,
     lattice: kwant.lattice.Polyatomic,
     func_onsite: Callable,
-    func_hop: Callable,
+    func_hop: Optional[Callable] = None,
     max_neighbor: int = 1,
 ) -> kwant.builder.Builder:
     """
     Construct an auxiliary `kwant` system that encodes the interactions.
 
     Parameters
     ----------
@@ -160,10 +197,11 @@
     :
         Auxiliary `kwant.builder.Builder` that encodes the interactions of the system.
     """
     int_builder = kwant.builder.Builder(
         kwant.lattice.TranslationalSymmetry(*builder.symmetry.periods)
     )
     int_builder[builder.sites()] = func_onsite
-    for neighbors in range(max_neighbor):
-        int_builder[lattice.neighbors(neighbors + 1)] = func_hop
+    if func_hop is not None:
+        for neighbors in range(max_neighbor):
+            int_builder[lattice.neighbors(neighbors + 1)] = func_hop
     return int_builder
```

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/tb/tb.py` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/tb/tb.py`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/tb/utils.py` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/tb/utils.py`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/tests/test_graphene.py` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/tests/test_graphene.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # %%
 import numpy as np
 import pytest
 
 from meanfi.kwant_helper import kwant_examples, utils
 from meanfi import (
     Model,
+    fermi_energy,
     solver,
     tb_to_kgrid,
     guess_tb,
     add_tb,
 )
 
 
@@ -74,15 +75,17 @@
     nk = 40
 
     h_int = utils.builder_to_tb(int_builder, params)
     guess = guess_tb(frozenset(h_int), len(list(h_0.values())[0]))
     model = Model(h_0, h_int, filling)
 
     mf_sol = solver(model, guess, nk=nk, optimizer_kwargs={"M": 0, "f_tol": 1e-8})
-    gap = compute_gap(add_tb(h_0, mf_sol), nk=200)
+    mf_full = add_tb(h_0, mf_sol)
+    EF = fermi_energy(mf_full, filling=filling, nk=nk)
+    gap = compute_gap(mf_full, fermi_energy=EF, nk=200)
 
     # Check if the gap is predicted correctly
     if gap > 0.1:
         gapped_predicted = True
     else:
         gapped_predicted = False
     assert (
```

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/tests/test_hat.py` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/tests/test_hat.py`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/tests/test_hubbard.py` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/tests/test_hubbard.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # %%
 import numpy as np
 import pytest
 
 from meanfi.tests.test_graphene import compute_gap
 from meanfi import (
     Model,
+    fermi_energy,
     solver,
     guess_tb,
     add_tb,
 )
 
 repeat_number = 3
 
@@ -34,15 +35,17 @@
     for U in Us:
         h_int = {
             (0,): U * np.kron(np.eye(2), np.ones((2, 2))),
         }
         guess = guess_tb(frozenset(h_int), len(list(h_0.values())[0]))
         full_model = Model(h_0, h_int, filling=2)
         mf_sol = solver(full_model, guess, nk=nk)
-        _gap = compute_gap(add_tb(h_0, mf_sol), fermi_energy=0, nk=nk_dense)
+        mf_full = add_tb(h_0, mf_sol)
+        EF = fermi_energy(mf_full, filling=2, nk=nk)
+        _gap = compute_gap(mf_full, fermi_energy=EF, nk=nk_dense)
         gaps.append(_gap)
 
     fit_gap = np.polyfit(Us, np.array(gaps), 1)[0]
     assert np.abs(fit_gap - 1) < tol
 
 
 @pytest.mark.parametrize("seed", range(repeat_number))
```

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/tests/test_zero_hint.py` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi/tests/test_zero_hint.py`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi-1.0.0.dist-info/licenses/AUTHORS.md` & `meanfi-1.1.0/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi-1.0.0.dist-info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/meanfi-1.1.0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/more_itertools-10.2.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/more_itertools-10.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mpmath-1.3.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/mpmath-1.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/myst_nb-1.1.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/myst_nb-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/myst_parser-3.0.1.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/myst_parser-3.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/nbclient-0.10.0.dist-info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/nbclient-0.10.0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/nbformat-5.10.4.dist-info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/nbformat-5.10.4.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/nest_asyncio-1.6.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/nest_asyncio-1.6.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/numpy/ma/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/numpy/ma/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pathspec-0.12.1.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pathspec-0.12.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pexpect-4.9.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pexpect-4.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pickleshare-0.7.5.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pickleshare-0.7.5.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pillow-10.3.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pillow-10.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pkgutil_resolve_name-1.3.10.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pkgutil_resolve_name-1.3.10.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/platformdirs-4.2.1.dist-info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/platformdirs-4.2.2.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pluggy-1.5.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pluggy-1.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/prompt_toolkit-3.0.42.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/prompt_toolkit-3.0.42.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/psutil-5.9.8.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/psutil-5.9.8.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/ptyprocess-0.7.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/ptyprocess-0.7.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pycparser-2.22.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pycparser-2.22.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pydata_sphinx_theme-0.15.2.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pydata_sphinx_theme-0.15.3.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pygments-2.18.0.dist-info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pygments-2.18.0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pyparsing-3.1.2.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pyparsing-3.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pytest-8.2.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/pytest-8.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/python_dateutil-2.9.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/python_dateutil-2.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/qsymm-1.4.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/qsymm-1.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/requests-2.31.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/requests-2.32.3.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/rich-13.7.1.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/rich-13.7.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/rpds_py-0.18.1.dist-info/license_files/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/rpds_py-0.18.1.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/scipy/_lib/_uarray/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/scipy/_lib/_uarray/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/setuptools_scm-8.1.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/setuptools_scm-8.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/shellingham-1.5.4.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/shellingham-1.5.4.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/six-1.16.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/six-1.16.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinx_book_theme/assets/translations/README.md` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinx_book_theme/assets/translations/README.md`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinx_book_theme-1.1.2.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinx_book_theme-1.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinx_copybutton-0.5.2.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinx_copybutton-0.5.2.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinx_tippy-0.4.3.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinx_tippy-0.4.3.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinx_togglebutton-0.3.2.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinx_togglebutton-0.3.2.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinxcontrib_applehelp-1.0.8.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinxcontrib_applehelp-1.0.8.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinxcontrib_devhelp-1.0.6.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinxcontrib_devhelp-1.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinxcontrib_htmlhelp-2.0.5.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinxcontrib_htmlhelp-2.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinxcontrib_jsmath-1.0.1.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinxcontrib_jsmath-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinxcontrib_qthelp-1.0.7.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinxcontrib_qthelp-1.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinxcontrib_serializinghtml-1.1.10.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sphinxcontrib_serializinghtml-1.1.10.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sympy-1.12.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/sympy-1.12.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/tabulate-0.9.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/tabulate-0.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/tomli-2.0.1.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/tomli-2.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/tomli_w-1.0.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/tomli_w-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/tomlkit-0.12.5.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/tomlkit-0.12.5.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/tornado-6.4.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/tornado-6.4.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/traitlets-5.14.3.dist-info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/traitlets-5.14.3.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/trove_classifiers-2024.4.10.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/trove_classifiers-2024.5.22.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/typing_extensions-4.11.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/typing_extensions-4.12.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/virtualenv-20.26.1.dist-info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/virtualenv-20.26.2.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/wcwidth-0.2.13.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/wcwidth-0.2.13.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/zipp-3.17.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/zipp-3.17.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/zstandard-0.19.0.dist-info/LICENSE` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/lib/python3.1/site-packages/zstandard-0.19.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/envs/meanfi-docs/share/doc/libjpeg-turbo/README.md` & `meanfi-1.1.0/micromamba/envs/meanfi-docs/share/doc/libjpeg-turbo/README.md`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/_openmp_mutex-4.5-2_gnu/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/_openmp_mutex-4.5-2_gnu/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/_openmp_mutex-4.5-2_gnu/info/recipe/parent/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/_openmp_mutex-4.5-2_gnu/info/recipe/parent/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/anyio-4.3.0-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/anyio-4.3.0-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/anyio-4.3.0-pyhd8ed1ab_0/info/test/pyproject.toml` & `meanfi-1.1.0/micromamba/pkgs/anyio-4.3.0-pyhd8ed1ab_0/info/test/pyproject.toml`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/asttokens-2.4.1-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/asttokens-2.4.1-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/attrs-23.2.0-pyh71513ae_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/attrs-23.2.0-pyh71513ae_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/babel-2.14.0-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/babel-2.14.0-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/backports.tarfile-1.0.0-pyhd8ed1ab_1/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/backports.tarfile-1.0.0-pyhd8ed1ab_1/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/brotli-1.1.0-hd590300_1/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/brotli-1.1.0-hd590300_1/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/brotli-bin-1.1.0-hd590300_1/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/brotli-bin-1.1.0-hd590300_1/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/brotli-python-1.1.0-py311hb755f60_1/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/brotli-python-1.1.0-py311hb755f60_1/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/bzip2-1.0.8-hd590300_5/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/bzip2-1.0.8-hd590300_5/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/ca-certificates-2024.2.2-hbcca054_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/ca-certificates-2024.6.2-hbcca054_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/certifi-2024.2.2-pyhd8ed1ab_0/info/licenses/certifi/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/certifi-2024.2.2-pyhd8ed1ab_0/info/licenses/certifi/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/cffi-1.16.0-py311hb3a22ac_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/cffi-1.16.0-py311hb3a22ac_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/charset-normalizer-3.3.2-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/charset-normalizer-3.3.2-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/comm-0.2.2-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/comm-0.2.2-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/contourpy-1.2.1-py311h9547e67_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/contourpy-1.2.1-py311h9547e67_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/cryptography-42.0.7-py311h4a61cc7_0/info/test/pyproject.toml` & `meanfi-1.1.0/micromamba/pkgs/cryptography-42.0.7-py311h4a61cc7_0/info/test/pyproject.toml`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/cycler-0.12.1-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/cycler-0.12.1-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/debugpy-1.8.1-py311hb755f60_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/debugpy-1.8.1-py311hb755f60_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/exceptiongroup-1.2.0-pyhd8ed1ab_2/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/exceptiongroup-1.2.0-pyhd8ed1ab_2/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/filelock-3.14.0-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/filelock-3.14.0-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/fonttools-4.51.0-py311h459d7ec_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/fonttools-4.53.0-py311h331c9d8_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/greenlet-3.0.3-py311hb755f60_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/greenlet-3.0.3-py311hb755f60_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/h2-4.1.0-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/h2-4.1.0-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/hatch-1.10.0-pyhd8ed1ab_0/info/test/pyproject.toml` & `meanfi-1.1.0/micromamba/pkgs/hatch-1.12.0-pyhd8ed1ab_0/info/test/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,14 @@
   "pexpect~=4.8",
   "platformdirs>=2.5.0",
   "rich>=11.2.0",
   "shellingham>=1.4.0",
   "tomli-w>=1.0",
   "tomlkit>=0.11.1",
   "userpath~=1.7",
-  "uv>=0.1.35",
   "virtualenv>=20.26.1",
   "zstandard<1",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://hatch.pypa.io/latest/"
```

### Comparing `meanfi-1.0.0/micromamba/pkgs/hpack-4.0.0-pyh9f0ad1d_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/hpack-4.0.0-pyh9f0ad1d_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/hyperframe-6.0.1-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/hyperframe-6.0.1-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/hyperlink-21.0.0-pyhd3deb0d_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/hyperlink-21.0.0-pyhd3deb0d_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/importlib-metadata-7.1.0-pyha770c72_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/importlib-metadata-7.1.0-pyha770c72_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/importlib_metadata-7.1.0-hd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/importlib_metadata-7.1.0-hd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/importlib_resources-6.4.0-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/importlib_resources-6.4.0-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/iniconfig-2.0.0-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/iniconfig-2.0.0-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/ipykernel-6.29.3-pyhd33586a_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/ipykernel-6.29.3-pyhd33586a_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/ipython-8.22.2-pyh707e725_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/ipython-8.25.0-pyh707e725_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/jaraco.classes-3.4.0-pyhd8ed1ab_1/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/jaraco.classes-3.4.0-pyhd8ed1ab_1/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/jaraco.context-5.3.0-pyhd8ed1ab_1/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/jaraco.context-5.3.0-pyhd8ed1ab_1/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/jaraco.functools-4.0.0-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/jaraco.functools-4.0.0-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/jeepney-0.8.0-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/jeepney-0.8.0-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/jupyter-cache-1.0.0-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/jupyter-cache-1.0.0-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/jupyter_client-8.6.1-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/jupyter_client-8.6.2-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/jupyter_core-5.7.2-py311h38be061_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/jupyter_core-5.7.2-py311h38be061_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/keyring-25.2.0-pyha804496_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/keyring-25.2.1-pyha804496_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/kiwisolver-1.4.5-py311h9547e67_1/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/kiwisolver-1.4.5-py311h9547e67_1/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/lcms2-2.16-hb7c19ff_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/lcms2-2.16-hb7c19ff_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/lerc-4.0.0-h27087fc_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/lerc-4.0.0-h27087fc_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/libbrotlicommon-1.1.0-hd590300_1/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/libbrotlicommon-1.1.0-hd590300_1/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/libbrotlidec-1.1.0-hd590300_1/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/libbrotlidec-1.1.0-hd590300_1/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/libbrotlienc-1.1.0-hd590300_1/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/libbrotlienc-1.1.0-hd590300_1/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/libev-4.33-hd590300_2/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/libev-4.33-hd590300_2/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/libffi-3.4.2-h7f98852_5/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/libffi-3.4.2-h7f98852_5/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/libgcc-ng-13.2.0-h77fa898_7/info/recipe/parent/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/libgcc-ng-13.2.0-h77fa898_7/info/recipe/parent/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/libgfortran-ng-13.2.0-h69a702a_7/info/recipe/parent/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/libgfortran-ng-13.2.0-h69a702a_7/info/recipe/parent/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/libgfortran5-13.2.0-hca663fb_7/info/recipe/parent/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/libgfortran5-13.2.0-hca663fb_7/info/recipe/parent/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/libgomp-13.2.0-h77fa898_7/info/recipe/parent/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/libgomp-13.2.0-h77fa898_7/info/recipe/parent/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/libopenblas-0.3.27-pthreads_h413a1c8_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/libopenblas-0.3.27-pthreads_h413a1c8_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/libopenblas-0.3.27-pthreads_h413a1c8_0/info/licenses/lapack-netlib/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/libopenblas-0.3.27-pthreads_h413a1c8_0/info/licenses/lapack-netlib/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/libpng-1.6.43-h2797004_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/libpng-1.6.43-h2797004_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/libsodium-1.0.18-h36c2ea0_1/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/libsodium-1.0.18-h36c2ea0_1/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/libstdcxx-ng-13.2.0-hc0a3c3a_7/info/recipe/parent/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/libstdcxx-ng-13.2.0-hc0a3c3a_7/info/recipe/parent/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/markdown-it-py-3.0.0-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/markdown-it-py-3.0.0-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/matplotlib-base-3.8.4-py311h54ef318_0/info/licenses/LICENSE/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/matplotlib-base-3.8.4-py311ha4ca890_2/info/licenses/LICENSE/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/matplotlib-inline-0.1.7-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/matplotlib-inline-0.1.7-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/mdit-py-plugins-0.4.0-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/mdit-py-plugins-0.4.1-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/mdurl-0.1.2-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/mdurl-0.1.2-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/more-itertools-10.2.0-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/more-itertools-10.2.0-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/mpmath-1.3.0-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/mpmath-1.3.0-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/mumps-include-5.7.1-ha770c72_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/mumps-include-5.7.1-ha770c72_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/mumps-seq-5.7.1-h6e8dedb_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/mumps-seq-5.7.1-h6e8dedb_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/myst-nb-1.1.0-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/myst-nb-1.1.0-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/myst-parser-3.0.1-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/myst-parser-3.0.1-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/nbclient-0.10.0-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/nbclient-0.10.0-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/nbformat-5.10.4-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/nbformat-5.10.4-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/nest-asyncio-1.6.0-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/nest-asyncio-1.6.0-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/nest-asyncio-1.6.0-pyhd8ed1ab_0/info/recipe/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/nest-asyncio-1.6.0-pyhd8ed1ab_0/info/recipe/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/openjpeg-2.5.2-h488ebb8_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/openjpeg-2.5.2-h488ebb8_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/pathspec-0.12.1-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/pathspec-0.12.1-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/pexpect-4.9.0-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/pexpect-4.9.0-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/pickleshare-0.7.5-py_1003/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/pickleshare-0.7.5-py_1003/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/pillow-10.3.0-py311h18e6fac_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/pillow-10.3.0-py311h18e6fac_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_1/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_1/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/platformdirs-4.2.1-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/platformdirs-4.2.2-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/pluggy-1.5.0-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/pluggy-1.5.0-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/prompt-toolkit-3.0.42-pyha770c72_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/prompt-toolkit-3.0.42-pyha770c72_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/psutil-5.9.8-py311h459d7ec_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/psutil-5.9.8-py311h459d7ec_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/pycparser-2.22-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/pycparser-2.22-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/pygments-2.18.0-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/pygments-2.18.0-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/pyparsing-3.1.2-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/pyparsing-3.1.2-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/pysocks-1.7.1-pyha2e5f31_6/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/pysocks-1.7.1-pyha2e5f31_6/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/pytest-8.2.0-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/pytest-8.2.1-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/python-3.11.9-hb806964_0_cpython/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/python-3.11.9-hb806964_0_cpython/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/python-dateutil-2.9.0-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/python-dateutil-2.9.0-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/python-fastjsonschema-2.19.1-pyhd8ed1ab_0/info/licenses/src/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/python-fastjsonschema-2.19.1-pyhd8ed1ab_0/info/licenses/src/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/python_abi-3.11-4_cp311/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/python_abi-3.11-4_cp311/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/python_abi-3.11-4_cp311/info/recipe/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/python_abi-3.11-4_cp311/info/recipe/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/pyyaml-6.0.1-py311h459d7ec_1/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/pyyaml-6.0.1-py311h459d7ec_1/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/qsymm-1.4.0-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/qsymm-1.4.0-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/referencing-0.35.1-pyhd8ed1ab_0/info/test/suite/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/referencing-0.35.1-pyhd8ed1ab_0/info/test/suite/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/referencing-0.35.1-pyhd8ed1ab_0/info/test/suite/README.md` & `meanfi-1.1.0/micromamba/pkgs/referencing-0.35.1-pyhd8ed1ab_0/info/test/suite/README.md`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/referencing-0.35.1-pyhd8ed1ab_0/info/test/suite/pyproject.toml` & `meanfi-1.1.0/micromamba/pkgs/referencing-0.35.1-pyhd8ed1ab_0/info/test/suite/pyproject.toml`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/requests-2.31.0-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/requests-2.32.3-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/rich-13.7.1-pyhd8ed1ab_0/info/licenses/dist/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/rich-13.7.1-pyhd8ed1ab_0/info/licenses/dist/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/rpds-py-0.18.1-py311h5ecf98a_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/rpds-py-0.18.1-py311h5ecf98a_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/secretstorage-3.3.3-py311h38be061_2/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/secretstorage-3.3.3-py311h38be061_2/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/setuptools-69.5.1-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/setuptools-70.0.0-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/setuptools-scm-8.1.0-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/setuptools-scm-8.1.0-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/shellingham-1.5.4-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/shellingham-1.5.4-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/six-1.16.0-pyh6c4a22f_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/six-1.16.0-pyh6c4a22f_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/sphinx-copybutton-0.5.2-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/sphinx-copybutton-0.5.2-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/sphinx-togglebutton-0.3.2-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/sphinx-togglebutton-0.3.2-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/sphinx-togglebutton-0.3.2-pyhd8ed1ab_0/info/recipe/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/sphinx-togglebutton-0.3.2-pyhd8ed1ab_0/info/recipe/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/sphinxcontrib-applehelp-1.0.8-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/sphinxcontrib-applehelp-1.0.8-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/sphinxcontrib-devhelp-1.0.6-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/sphinxcontrib-devhelp-1.0.6-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/sphinxcontrib-htmlhelp-2.0.5-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/sphinxcontrib-htmlhelp-2.0.5-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/sphinxcontrib-jsmath-1.0.1-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/sphinxcontrib-jsmath-1.0.1-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/sphinxcontrib-qthelp-1.0.7-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/sphinxcontrib-qthelp-1.0.7-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/sphinxcontrib-serializinghtml-1.1.10-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/sphinxcontrib-serializinghtml-1.1.10-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/sqlalchemy-2.0.30-py311h331c9d8_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/sqlalchemy-2.0.30-py311h331c9d8_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/sympy-1.12-pypyh9d50eac_103/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/sympy-1.12-pypyh9d50eac_103/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/tabulate-0.9.0-pyhd8ed1ab_1/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/tabulate-0.9.0-pyhd8ed1ab_1/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/tomli-2.0.1-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/tomli-2.0.1-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/tomli-w-1.0.0-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/tomli-w-1.0.0-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/tomlkit-0.12.5-pyha770c72_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/tomlkit-0.12.5-pyha770c72_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/tornado-6.4-py311h459d7ec_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/tornado-6.4-py311h459d7ec_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/traitlets-5.14.3-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/traitlets-5.14.3-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/traitlets-5.14.3-pyhd8ed1ab_0/info/test/pyproject.toml` & `meanfi-1.1.0/micromamba/pkgs/traitlets-5.14.3-pyhd8ed1ab_0/info/test/pyproject.toml`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/trove-classifiers-2024.4.10-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/trove-classifiers-2024.5.22-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/typing-extensions-4.11.0-hd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/typing-extensions-4.12.1-hd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/typing_extensions-4.11.0-pyha770c72_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/typing_extensions-4.12.1-pyha770c72_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/virtualenv-20.26.1-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/virtualenv-20.26.2-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/wcwidth-0.2.13-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/wcwidth-0.2.13-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/zeromq-4.3.5-h75354e8_3/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/zeromq-4.3.5-h75354e8_4/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/zipp-3.17.0-pyhd8ed1ab_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/zipp-3.17.0-pyhd8ed1ab_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/zstandard-0.19.0-py311hd4cff14_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/zstandard-0.19.0-py311hd4cff14_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/micromamba/pkgs/zstd-1.5.6-ha6fb4c9_0/info/licenses/LICENSE` & `meanfi-1.1.0/micromamba/pkgs/zstd-1.5.6-ha6fb4c9_0/info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/LICENSE` & `meanfi-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meanfi-1.0.0/README.md` & `meanfi-1.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 `MeanFi` is a Python package that performs self-consistent Hartree-Fock calculations on tight-binding models.
 It aims to find the groundstate of a Hamiltonian with density-density interactions
 
 $$
 \hat{H} = \hat{H_0} + \hat{V} = \sum_{ij} h_{ij} c^\dagger_{i} c_{j} + \frac{1}{2} \sum_{ij} v_{ij} \hat{n}_i \hat{n}_j,
 $$
 
-and computes the mean-field correction $\hat{V}_{\text{MF}}$ which approximates the interaction term:
+and computes the mean-field correction $\hat{V}^{\text{MF}}$ which approximates the interaction term:
 
 $$
-\hat{V} \approx \hat{V}_{\text{MF}} = \sum_{ij} \tilde{v}_{ij} c^\dagger_{i} c_{j}.
+\hat{V} \approx \hat{V}^{\text{MF}} =\sum_{ij} \tilde{v}\_{ij} c_{i}^{\dagger} c_{j}.
 $$
 
-For more details, refer to the [theory overview](docs/source/documentation/mf_notes.md) and [algorithm description](docs/source/documentation/algorithm.md).
+For more details, refer to the [theory overview](https://meanfi.readthedocs.io/en/latest/documentation/mf_notes.html) and [algorithm description](https://meanfi.readthedocs.io/en/latest/documentation/algorithm.html).
 
 ## How to use `MeanFi`?
 
 The calculation of a mean-field Hamiltonian is a simple 3-step process:
 
 1. **Define**
 
@@ -47,15 +47,15 @@
 guess = meanfi.guess_tb(guess_hopping_keys, ndof)
 
 #Solve
 mf_correction = meanfi.solver(model, guess)
 h_mf = meanfi.add_tb(h_0, mf_correction)
 ```
 
-For more details and examples on how to use the package, we refer to the [tutorials](docs/source/tutorial/hubbard_1d.md).
+For more details and examples on how to use the package, we refer to the [tutorials](https://meanfi.readthedocs.io/en/latest/tutorial/hubbard_1d.html).
 
 ## Why `MeanFi`?
 
 Here is why you should use `MeanFi`:
 
 * Simple
 
@@ -71,16 +71,16 @@
     Introduces minimal overhead to the calculation of the mean-field Hamiltonian.
 
 
 ## What `MeanFi` doesn't do (yet)
 
 Here are some features that are not yet implemented but are planned for future releases:
 
-- **Superconductive order parameters**. Mean-field Hamiltonians do not include pairing terms.
-- **General interactions**. We allow only density-density interactions (e.g. Coulomb) which can be described by a second-order tensor.
+- **Superconducting order parameters**. Mean-field Hamiltonians do not include pairing terms.
+- **General interactions**. We allow only density-density interactions (e.g. Coulomb) which can be described by a rank two tensor.
 - **Temperature effects**. Density matrix calculations are done at zero temperature.
 
 ## Installation
 
 ```
 pip install meanfi
 ```
```

### Comparing `meanfi-1.0.0/pyproject.toml` & `meanfi-1.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -45,8 +45,8 @@
   "LICENSE",
   "pyproject.toml",
   "AUTHORS.md",
 ]
 
 [tool.codespell]
 skip = "*.ipynb"
-ignore-words-list = "multline, ket, bra, braket, nwo"
+ignore-words-list = "multline, ket, bra, braket, nwo, mater"
```

### Comparing `meanfi-1.0.0/PKG-INFO` & `meanfi-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: meanfi
-Version: 1.0.0
+Version: 1.1.0
 Summary: Package to perform self-consistent mean-field calculations on tight-binding systems
 Project-URL: Documentation, https://meanfi.readthedocs.io/en/latest/
 Project-URL: Repository, https://gitlab.kwant-project.org/qt/meanfi
 Project-URL: Bug Tracker, https://gitlab.kwant-project.org/qt/meanfi/-/issues
 Author: MeanFi developers
 License-File: AUTHORS.md
 License-File: LICENSE
@@ -28,21 +28,21 @@
 `MeanFi` is a Python package that performs self-consistent Hartree-Fock calculations on tight-binding models.
 It aims to find the groundstate of a Hamiltonian with density-density interactions
 
 $$
 \hat{H} = \hat{H_0} + \hat{V} = \sum_{ij} h_{ij} c^\dagger_{i} c_{j} + \frac{1}{2} \sum_{ij} v_{ij} \hat{n}_i \hat{n}_j,
 $$
 
-and computes the mean-field correction $\hat{V}_{\text{MF}}$ which approximates the interaction term:
+and computes the mean-field correction $\hat{V}^{\text{MF}}$ which approximates the interaction term:
 
 $$
-\hat{V} \approx \hat{V}_{\text{MF}} = \sum_{ij} \tilde{v}_{ij} c^\dagger_{i} c_{j}.
+\hat{V} \approx \hat{V}^{\text{MF}} =\sum_{ij} \tilde{v}\_{ij} c_{i}^{\dagger} c_{j}.
 $$
 
-For more details, refer to the [theory overview](docs/source/documentation/mf_notes.md) and [algorithm description](docs/source/documentation/algorithm.md).
+For more details, refer to the [theory overview](https://meanfi.readthedocs.io/en/latest/documentation/mf_notes.html) and [algorithm description](https://meanfi.readthedocs.io/en/latest/documentation/algorithm.html).
 
 ## How to use `MeanFi`?
 
 The calculation of a mean-field Hamiltonian is a simple 3-step process:
 
 1. **Define**
 
@@ -70,15 +70,15 @@
 guess = meanfi.guess_tb(guess_hopping_keys, ndof)
 
 #Solve
 mf_correction = meanfi.solver(model, guess)
 h_mf = meanfi.add_tb(h_0, mf_correction)
 ```
 
-For more details and examples on how to use the package, we refer to the [tutorials](docs/source/tutorial/hubbard_1d.md).
+For more details and examples on how to use the package, we refer to the [tutorials](https://meanfi.readthedocs.io/en/latest/tutorial/hubbard_1d.html).
 
 ## Why `MeanFi`?
 
 Here is why you should use `MeanFi`:
 
 * Simple
 
@@ -94,16 +94,16 @@
     Introduces minimal overhead to the calculation of the mean-field Hamiltonian.
 
 
 ## What `MeanFi` doesn't do (yet)
 
 Here are some features that are not yet implemented but are planned for future releases:
 
-- **Superconductive order parameters**. Mean-field Hamiltonians do not include pairing terms.
-- **General interactions**. We allow only density-density interactions (e.g. Coulomb) which can be described by a second-order tensor.
+- **Superconducting order parameters**. Mean-field Hamiltonians do not include pairing terms.
+- **General interactions**. We allow only density-density interactions (e.g. Coulomb) which can be described by a rank two tensor.
 - **Temperature effects**. Density matrix calculations are done at zero temperature.
 
 ## Installation
 
 ```
 pip install meanfi
 ```
```

