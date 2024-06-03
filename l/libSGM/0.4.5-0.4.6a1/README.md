# Comparing `tmp/libSGM-0.4.5.tar.gz` & `tmp/libsgm-0.4.6a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libSGM-0.4.5.tar", last modified: Tue Jan 30 14:19:49 2024, max compression
+gzip compressed data, was "libsgm-0.4.6a1.tar", last modified: Mon Jun  3 09:12:57 2024, max compression
```

## Comparing `libSGM-0.4.5.tar` & `libsgm-0.4.6a1.tar`

### file list

```diff
@@ -1,131 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:19:49.318613 libSGM-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-01-30 14:19:04.000000 libSGM-0.4.5/.codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:19:49.294613 libSGM-0.4.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:19:49.302613 libSGM-0.4.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-01-30 14:19:04.000000 libSGM-0.4.5/.github/workflows/libsgm_ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-01-30 14:19:04.000000 libSGM-0.4.5/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:19:49.302613 libSGM-0.4.5/.gitlab/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-01-30 14:19:04.000000 libSGM-0.4.5/.gitlab/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:19:49.302613 libSGM-0.4.5/.gitlab/issue_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-01-30 14:19:04.000000 libSGM-0.4.5/.gitlab/issue_templates/Bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-01-30 14:19:04.000000 libSGM-0.4.5/.gitlab/issue_templates/Proposition.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:19:49.302613 libSGM-0.4.5/.gitlab/merge_request_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-01-30 14:19:04.000000 libSGM-0.4.5/.gitlab/merge_request_templates/MR.md
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-01-30 14:19:04.000000 libSGM-0.4.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    16057 2024-01-30 14:19:04.000000 libSGM-0.4.5/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-01-30 14:19:04.000000 libSGM-0.4.5/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-01-30 14:19:04.000000 libSGM-0.4.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-01-30 14:19:04.000000 libSGM-0.4.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-01-30 14:19:04.000000 libSGM-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-01-30 14:19:04.000000 libSGM-0.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-01-30 14:19:04.000000 libSGM-0.4.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-01-30 14:19:04.000000 libSGM-0.4.5/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-01-30 14:19:49.318613 libSGM-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-01-30 14:19:04.000000 libSGM-0.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:19:49.302613 libSGM-0.4.5/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-01-30 14:19:04.000000 libSGM-0.4.5/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-01-30 14:19:04.000000 libSGM-0.4.5/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:19:49.302613 libSGM-0.4.5/doc/source/
--rw-r--r--   0 runner    (1001) docker     (127)   108587 2024-01-30 14:19:04.000000 libSGM-0.4.5/doc/source/Doxyfile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:19:49.302613 libSGM-0.4.5/doc/source/api_reference/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:19:49.302613 libSGM-0.4.5/doc/source/api_reference/libsgm_python/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-01-30 14:19:04.000000 libSGM-0.4.5/doc/source/api_reference/libsgm_python/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:19:49.302613 libSGM-0.4.5/doc/source/api_reference/libsgm_python/lr_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-01-30 14:19:04.000000 libSGM-0.4.5/doc/source/api_reference/libsgm_python/lr_manager/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:19:49.302613 libSGM-0.4.5/doc/source/api_reference/libsgm_python/sgm_python/
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-01-30 14:19:04.000000 libSGM-0.4.5/doc/source/api_reference/libsgm_python/sgm_python/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:19:49.302613 libSGM-0.4.5/doc/source/api_reference/libsgm_python/sgm_python_parall/
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-01-30 14:19:04.000000 libSGM-0.4.5/doc/source/api_reference/libsgm_python/sgm_python_parall/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-01-30 14:19:04.000000 libSGM-0.4.5/doc/source/api_reference/sgm_wrapper.rst
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-01-30 14:19:04.000000 libSGM-0.4.5/doc/source/api_reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-01-30 14:19:04.000000 libSGM-0.4.5/doc/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:19:49.306613 libSGM-0.4.5/doc/source/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-01-30 14:19:04.000000 libSGM-0.4.5/doc/source/developer_guide/before_coding.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-01-30 14:19:04.000000 libSGM-0.4.5/doc/source/developer_guide/lr_manager.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-01-30 14:19:04.000000 libSGM-0.4.5/doc/source/developer_guide/memory_optimization.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-01-30 14:19:04.000000 libSGM-0.4.5/doc/source/developer_guide/piecewise_optimization.rst
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-01-30 14:19:04.000000 libSGM-0.4.5/doc/source/developer_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:19:49.306613 libSGM-0.4.5/doc/source/getting_started/
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-01-30 14:19:04.000000 libSGM-0.4.5/doc/source/getting_started/example.rst
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-01-30 14:19:04.000000 libSGM-0.4.5/doc/source/getting_started/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-01-30 14:19:04.000000 libSGM-0.4.5/doc/source/getting_started/quick_overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-01-30 14:19:04.000000 libSGM-0.4.5/doc/source/getting_started.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:19:49.306613 libSGM-0.4.5/doc/source/images/
--rw-r--r--   0 runner    (1001) docker     (127)    19203 2024-01-30 14:19:04.000000 libSGM-0.4.5/doc/source/images/lr_manager.png
--rw-r--r--   0 runner    (1001) docker     (127)     8005 2024-01-30 14:19:04.000000 libSGM-0.4.5/doc/source/images/piecewise_optimization.png
--rw-r--r--   0 runner    (1001) docker     (127)    26826 2024-01-30 14:19:04.000000 libSGM-0.4.5/doc/source/images/sgm_memory_optim.png
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-01-30 14:19:04.000000 libSGM-0.4.5/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-30 14:19:04.000000 libSGM-0.4.5/doc/source/user_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:19:49.318613 libSGM-0.4.5/libSGM.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-01-30 14:19:49.000000 libSGM-0.4.5/libSGM.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-01-30 14:19:49.000000 libSGM-0.4.5/libSGM.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 14:19:49.000000 libSGM-0.4.5/libSGM.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-01-30 14:19:49.000000 libSGM-0.4.5/libSGM.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 14:19:29.000000 libSGM-0.4.5/libSGM.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-01-30 14:19:49.000000 libSGM-0.4.5/libSGM.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-30 14:19:49.000000 libSGM-0.4.5/libSGM.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:19:49.306613 libSGM-0.4.5/libsgm_python/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:19:04.000000 libSGM-0.4.5/libsgm_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-01-30 14:19:04.000000 libSGM-0.4.5/libsgm_python/lr_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-01-30 14:19:04.000000 libSGM-0.4.5/libsgm_python/sgm_python.py
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-01-30 14:19:04.000000 libSGM-0.4.5/libsgm_python/sgm_python_parall.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-01-30 14:19:04.000000 libSGM-0.4.5/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-01-30 14:19:04.000000 libSGM-0.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-01-30 14:19:49.318613 libSGM-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-01-30 14:19:04.000000 libSGM-0.4.5/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-01-30 14:19:04.000000 libSGM-0.4.5/sonar-project.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:19:49.310613 libSGM-0.4.5/sources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:19:49.310613 libSGM-0.4.5/sources/lib/
--rw-r--r--   0 runner    (1001) docker     (127)    30468 2024-01-30 14:19:04.000000 libSGM-0.4.5/sources/lib/sgm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13310 2024-01-30 14:19:04.000000 libSGM-0.4.5/sources/lib/sgm.hpp
--rw-r--r--   0 runner    (1001) docker     (127)  1044601 2024-01-30 14:19:04.000000 libSGM-0.4.5/sources/sgm_wrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8443 2024-01-30 14:19:04.000000 libSGM-0.4.5/sources/sgm_wrapper.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:19:49.310613 libSGM-0.4.5/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    69319 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/functions_unittest.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:19:49.298613 libSGM-0.4.5/test/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:19:49.310613 libSGM-0.4.5/test/include/gtest/
--rw-r--r--   0 runner    (1001) docker     (127)    14343 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/include/gtest/gtest-death-test.h
--rw-r--r--   0 runner    (1001) docker     (127)    26991 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/include/gtest/gtest-matchers.h
--rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/include/gtest/gtest-message.h
--rw-r--r--   0 runner    (1001) docker     (127)    22183 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/include/gtest/gtest-param-test.h
--rw-r--r--   0 runner    (1001) docker     (127)    34029 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/include/gtest/gtest-printers.h
--rw-r--r--   0 runner    (1001) docker     (127)    10097 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/include/gtest/gtest-spi.h
--rw-r--r--   0 runner    (1001) docker     (127)     6793 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/include/gtest/gtest-test-part.h
--rw-r--r--   0 runner    (1001) docker     (127)    15395 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/include/gtest/gtest-typed-test.h
--rw-r--r--   0 runner    (1001) docker     (127)    93571 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/include/gtest/gtest.h
--rw-r--r--   0 runner    (1001) docker     (127)    14850 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/include/gtest/gtest_pred_impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/include/gtest/gtest_prod.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:19:49.314613 libSGM-0.4.5/test/include/gtest/internal/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:19:49.314613 libSGM-0.4.5/test/include/gtest/internal/custom/
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/include/gtest/internal/custom/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/include/gtest/internal/custom/gtest-port.h
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/include/gtest/internal/custom/gtest-printers.h
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/include/gtest/internal/custom/gtest.h
--rw-r--r--   0 runner    (1001) docker     (127)    13436 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/include/gtest/internal/gtest-death-test-internal.h
--rw-r--r--   0 runner    (1001) docker     (127)     9752 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/include/gtest/internal/gtest-filepath.h
--rw-r--r--   0 runner    (1001) docker     (127)    53813 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/include/gtest/internal/gtest-internal.h
--rw-r--r--   0 runner    (1001) docker     (127)    33066 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/include/gtest/internal/gtest-param-util.h
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/include/gtest/internal/gtest-port-arch.h
--rw-r--r--   0 runner    (1001) docker     (127)    79624 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/include/gtest/internal/gtest-port.h
--rw-r--r--   0 runner    (1001) docker     (127)     7005 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/include/gtest/internal/gtest-string.h
--rw-r--r--   0 runner    (1001) docker     (127)   186064 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/include/gtest/internal/gtest-type-util.h
--rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/include/gtest/internal/gtest-type-util.h.pump
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:19:49.314613 libSGM-0.4.5/test/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/src/gtest-all.cc
--rw-r--r--   0 runner    (1001) docker     (127)    62175 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/src/gtest-death-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)    14240 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/src/gtest-filepath.cc
--rw-r--r--   0 runner    (1001) docker     (127)    46926 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/src/gtest-internal-inl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/src/gtest-matchers.cc
--rw-r--r--   0 runner    (1001) docker     (127)    46449 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/src/gtest-port.cc
--rw-r--r--   0 runner    (1001) docker     (127)    14711 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/src/gtest-printers.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/src/gtest-test-part.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/src/gtest-typed-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)   225917 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/src/gtest.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/src/gtest_main.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:19:49.318613 libSGM-0.4.5/test/test_libsgm_python/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/test_libsgm_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/test_libsgm_python/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/test_libsgm_python/disable_test_sgm_python_parall.py
--rw-r--r--   0 runner    (1001) docker     (127)    23839 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/test_libsgm_python/test_lr_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-01-30 14:19:04.000000 libSGM-0.4.5/test/test_libsgm_python/test_sgm_python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:12:57.246233 libsgm-0.4.6a1/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/.codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:12:57.214233 libsgm-0.4.6a1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:12:57.222233 libsgm-0.4.6a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/.github/workflows/libsgm_ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:12:57.222233 libsgm-0.4.6a1/.gitlab/
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/.gitlab/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:12:57.222233 libsgm-0.4.6a1/.gitlab/issue_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/.gitlab/issue_templates/Bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/.gitlab/issue_templates/Proposition.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:12:57.222233 libsgm-0.4.6a1/.gitlab/merge_request_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/.gitlab/merge_request_templates/MR.md
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    16057 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-06-03 09:12:57.246233 libsgm-0.4.6a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:12:57.222233 libsgm-0.4.6a1/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)   108584 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/doc/Doxyfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:12:57.226233 libsgm-0.4.6a1/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:12:57.226233 libsgm-0.4.6a1/doc/source/api_reference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:12:57.226233 libsgm-0.4.6a1/doc/source/api_reference/libsgm_python/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/doc/source/api_reference/libsgm_python/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:12:57.226233 libsgm-0.4.6a1/doc/source/api_reference/libsgm_python/lr_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/doc/source/api_reference/libsgm_python/lr_manager/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:12:57.226233 libsgm-0.4.6a1/doc/source/api_reference/libsgm_python/sgm_python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/doc/source/api_reference/libsgm_python/sgm_python/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:12:57.226233 libsgm-0.4.6a1/doc/source/api_reference/libsgm_python/sgm_python_parall/
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/doc/source/api_reference/libsgm_python/sgm_python_parall/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/doc/source/api_reference/sgm_wrapper.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/doc/source/api_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/doc/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:12:57.226233 libsgm-0.4.6a1/doc/source/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/doc/source/developer_guide/before_coding.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/doc/source/developer_guide/lr_manager.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/doc/source/developer_guide/memory_optimization.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/doc/source/developer_guide/piecewise_optimization.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/doc/source/developer_guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:12:57.226233 libsgm-0.4.6a1/doc/source/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/doc/source/getting_started/example.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/doc/source/getting_started/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/doc/source/getting_started/quick_overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/doc/source/getting_started.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:12:57.230233 libsgm-0.4.6a1/doc/source/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    19203 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/doc/source/images/lr_manager.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8005 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/doc/source/images/piecewise_optimization.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26826 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/doc/source/images/sgm_memory_optim.png
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/doc/source/user_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-06-03 09:12:57.246233 libsgm-0.4.6a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/sonar-project.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:12:57.218233 libsgm-0.4.6a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:12:57.230233 libsgm-0.4.6a1/src/libSGM/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:12:57.230233 libsgm-0.4.6a1/src/libSGM/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)    30496 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/src/libSGM/lib/sgm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13473 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/src/libSGM/lib/sgm.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)  1044601 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/src/libSGM/sgm_wrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8443 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/src/libSGM/sgm_wrapper.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:12:57.242233 libsgm-0.4.6a1/src/libSGM.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-06-03 09:12:57.000000 libsgm-0.4.6a1/src/libSGM.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-06-03 09:12:57.000000 libsgm-0.4.6a1/src/libSGM.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:12:57.000000 libsgm-0.4.6a1/src/libSGM.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-03 09:12:57.000000 libsgm-0.4.6a1/src/libSGM.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:12:19.000000 libsgm-0.4.6a1/src/libSGM.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-06-03 09:12:57.000000 libsgm-0.4.6a1/src/libSGM.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-06-03 09:12:57.000000 libsgm-0.4.6a1/src/libSGM.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:12:57.234233 libsgm-0.4.6a1/src/libsgm_python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/src/libsgm_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/src/libsgm_python/lr_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/src/libsgm_python/sgm_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/src/libsgm_python/sgm_python_parall.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:12:57.234233 libsgm-0.4.6a1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69322 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/functions_unittest.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:12:57.218233 libsgm-0.4.6a1/test/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:12:57.234233 libsgm-0.4.6a1/test/include/gtest/
+-rw-r--r--   0 runner    (1001) docker     (127)    14343 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/include/gtest/gtest-death-test.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26991 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/include/gtest/gtest-matchers.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/include/gtest/gtest-message.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22183 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/include/gtest/gtest-param-test.h
+-rw-r--r--   0 runner    (1001) docker     (127)    34029 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/include/gtest/gtest-printers.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10097 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/include/gtest/gtest-spi.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6793 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/include/gtest/gtest-test-part.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15395 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/include/gtest/gtest-typed-test.h
+-rw-r--r--   0 runner    (1001) docker     (127)    93571 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/include/gtest/gtest.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14850 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/include/gtest/gtest_pred_impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/include/gtest/gtest_prod.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:12:57.238233 libsgm-0.4.6a1/test/include/gtest/internal/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:12:57.238233 libsgm-0.4.6a1/test/include/gtest/internal/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/include/gtest/internal/custom/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/include/gtest/internal/custom/gtest-port.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/include/gtest/internal/custom/gtest-printers.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/include/gtest/internal/custom/gtest.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13436 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/include/gtest/internal/gtest-death-test-internal.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9752 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/include/gtest/internal/gtest-filepath.h
+-rw-r--r--   0 runner    (1001) docker     (127)    53813 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/include/gtest/internal/gtest-internal.h
+-rw-r--r--   0 runner    (1001) docker     (127)    33066 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/include/gtest/internal/gtest-param-util.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/include/gtest/internal/gtest-port-arch.h
+-rw-r--r--   0 runner    (1001) docker     (127)    79624 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/include/gtest/internal/gtest-port.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7005 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/include/gtest/internal/gtest-string.h
+-rw-r--r--   0 runner    (1001) docker     (127)   186064 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/include/gtest/internal/gtest-type-util.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/include/gtest/internal/gtest-type-util.h.pump
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:12:57.242233 libsgm-0.4.6a1/test/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/src/gtest-all.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    62175 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/src/gtest-death-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    14240 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/src/gtest-filepath.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    46926 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/src/gtest-internal-inl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/src/gtest-matchers.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    46449 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/src/gtest-port.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    14711 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/src/gtest-printers.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/src/gtest-test-part.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/src/gtest-typed-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)   225917 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/src/gtest.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/src/gtest_main.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:12:57.242233 libsgm-0.4.6a1/test/test_libsgm_python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/test_libsgm_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/test_libsgm_python/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/test_libsgm_python/disable_test_sgm_python_parall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23839 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/test_libsgm_python/test_lr_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-06-03 09:11:53.000000 libsgm-0.4.6a1/test/test_libsgm_python/test_sgm_python.py
```

### Comparing `libSGM-0.4.5/.github/workflows/libsgm_ci.yml` & `libsgm-0.4.6a1/.github/workflows/libsgm_ci.yml`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/.gitlab/README.md` & `libsgm-0.4.6a1/.gitlab/README.md`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/.gitlab/merge_request_templates/MR.md` & `libsgm-0.4.6a1/.gitlab/merge_request_templates/MR.md`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/.pre-commit-config.yaml` & `libsgm-0.4.6a1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/.pylintrc` & `libsgm-0.4.6a1/.pylintrc`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/AUTHORS.md` & `libsgm-0.4.6a1/AUTHORS.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # Credits
 
-Copyright (c) 2023 Centre National d'Etudes Spatiales (CNES).
+Copyright (c) 2024 Centre National d'Etudes Spatiales (CNES).
 
 Pandora_libsgm is licensed under permissive Apache 2 license (See LICENSE file).
 The copyright is kept CNES only for long term maintenance ease.
 
 See CONTRIBUTING.md for more details on Contributor License Agreement.
 
 This file keeps track of authors contributions.
 
 ## Development Lead
 
 * Emmanuelle Sarrazin <emmanuelle.sarrazin@cnes.fr>
 * Natalia Jimenez <natalia.jimenez-diaz@csgroup.eu>
 * Alice de Bardonnèche-Richard <alice.de-bardonneche-richard@csgroup.eu>
+* Marie Leconte <marie.leconte@csgroup.eu>
+* Philippe Mallet-Ladeira <philippe.mallet-ladeira@csgroup.eu>
 
 ## Contributors
 
 * Veronique Defonte <veronique.defonte@csgroup.eu>
 * Quentin Fardet <quentin.fardet@csgroup.eu>
 * Mannaïg L'Haridon <mannaig.lharidon@csgroup.eu>
 * Julien Michel <Julien.Michel@cnes.fr>
```

### Comparing `libSGM-0.4.5/CHANGELOG.md` & `libsgm-0.4.6a1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+## 0.4.6a1 (June 2024)
+
+### Changed
+- Update the setup.py file to install with the -e option. [#68]
+
 ## 0.4.5 (January 2024)
 
 ### Changed
 
 - Update of the minimal version for python. [#78]
 - Update of the minimal version for python in github workflow. [#79]
```

### Comparing `libSGM-0.4.5/LICENSE` & `libsgm-0.4.6a1/LICENSE`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/Makefile` & `libsgm-0.4.6a1/Makefile`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2020 Centre National d'Etudes Spatiales (CNES).
+# Copyright (c) 2024 Centre National d'Etudes Spatiales (CNES).
 #
 # This file is part of LIBSGM
 #
 #     https://github.com/CNES/Pandora_libsgm
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -18,22 +18,22 @@
 # limitations under the License.
 #
 # Variables for compilation
 CC=gcc
 CFLAGS=-Wall -ansi -pedantic -Wextra -g -fdiagnostics-show-option -o2
 CXX=g++
 # Project's variables
-SOURCES=sources/lib/sgm.cpp
+SOURCES=src/libSGM/lib/sgm.cpp
 EXEC=sgm
 
 # Points to the root of Google Test, relative to where this file is.
 GTEST_DIR=./test
 
 # Where to find user code.
-SRC_DIR=./sources/lib
+SRC_DIR=./src/libSGM/lib
 TEST_DIR=./test
 
 # Flags passed to the preprocessor.
 # Set Google Test's header directory as a system directory, such that
 # the compiler doesn't generate warnings in Google Test headers.
 CPPFLAGS += -isystem $(GTEST_DIR)/include
```

### Comparing `libSGM-0.4.5/NOTICE` & `libsgm-0.4.6a1/NOTICE`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/PKG-INFO` & `libsgm-0.4.6a1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: libSGM
-Version: 0.4.5
+Version: 0.4.6a1
 Summary: libSGM is a CNES version of H.Hirschmuller Semi-Global Matching
 Home-page: https://github.com/CNES/Pandora_libsgm
 Author: CNES
 Author-email: myriam.cournet@cnes.fr
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.22; python_version > "3.7"
 Requires-Dist: numpy; python_version < "3.8"
 Requires-Dist: numba>=0.55.2; python_version > "3.7"
 Requires-Dist: numba>=0.47.0; python_version < "3.8"
+Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx_rtd_theme; extra == "docs"
+Requires-Dist: sphinx_autoapi; extra == "docs"
+Requires-Dist: breathe; extra == "docs"
+Requires-Dist: exhale; extra == "docs"
 Provides-Extra: dev
-Requires-Dist: sphinx; extra == "dev"
-Requires-Dist: sphinx_rtd_theme; extra == "dev"
-Requires-Dist: sphinx_autoapi; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: black; extra == "dev"
 
@@ -63,14 +66,24 @@
 from libSGM import sgm_wrapper
 ...
 cost_volumes_out = sgm_wrapper.sgm_api(cost_volume_in, p1, p2, directions, invalid_value, False, False)
 ```
 
 Let's see [pandora_plugin_LibSGM](https://github.com/CNES/pandora_plugin_libsgm) for real life exemple.
 
+## Documentation
+
+To build documentation, `doxygen` must be installed on your system.
+
+Then install dependencies with `pip install .[doc]`.
+
+Go in `doc` and run `make html` to generate html documentation.
+
+You can serve generated documentation locally with `make serve` and open your webbrowser at [https://0.0.0.0:8000/](https://0.0.0.0:8000/).
+
 ## Related
 
 [Pandora](https://github.com/CNES/Pandora) - A stereo matching framework  
 [Plugin_LibSGM](https://github.com/CNES/pandora_plugin_libsgm) - Stereo Matching Algorithm plugin for Pandora  
 
 ## References
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: libSGM Version: 0.4.5 Summary: libSGM is a CNES
+Metadata-Version: 2.1 Name: libSGM Version: 0.4.6a1 Summary: libSGM is a CNES
 version of H.Hirschmuller Semi-Global Matching Home-page: https://github.com/
 CNES/Pandora_libsgm Author: CNES Author-email: myriam.cournet@cnes.fr License:
 Apache License 2.0 Requires-Python: >=3.8 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: numpy>=1.22; python_version >
 "3.7" Requires-Dist: numpy; python_version < "3.8" Requires-Dist:
 numba>=0.55.2; python_version > "3.7" Requires-Dist: numba>=0.47.0;
-python_version < "3.8" Provides-Extra: dev Requires-Dist: sphinx; extra ==
-"dev" Requires-Dist: sphinx_rtd_theme; extra == "dev" Requires-Dist:
-sphinx_autoapi; extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-
-Dist: pytest-cov; extra == "dev" Requires-Dist: pylint; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev" Requires-Dist: mypy; extra == "dev"
-Requires-Dist: black; extra == "dev"
+python_version < "3.8" Provides-Extra: docs Requires-Dist: sphinx; extra ==
+"docs" Requires-Dist: sphinx_rtd_theme; extra == "docs" Requires-Dist:
+sphinx_autoapi; extra == "docs" Requires-Dist: breathe; extra == "docs"
+Requires-Dist: exhale; extra == "docs" Provides-Extra: dev Requires-Dist:
+pytest; extra == "dev" Requires-Dist: pytest-cov; extra == "dev" Requires-Dist:
+pylint; extra == "dev" Requires-Dist: pre-commit; extra == "dev" Requires-Dist:
+mypy; extra == "dev" Requires-Dist: black; extra == "dev"
                              ************ lliibbSSGGMM ************
                     ****** SSeemmii--GGlloobbaall MMaattcchhiinngg aallggoorriitthhmm.. ******
    _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_C_N_E_S_/_P_a_n_d_o_r_a___l_i_b_S_G_M_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_l_i_b_s_g_m___c_i_._y_m_l_/
   _b_a_d_g_e_._s_v_g_?_b_r_a_n_c_h_=_m_a_s_t_e_r_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_C_N_E_S_/_P_a_n_d_o_r_a___l_i_b_S_G_M_/_b_r_a_n_c_h_/
 _m_a_s_t_e_r_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_O_Z_C_Y_I_8_4_3_J_H_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-
                             _A_p_a_c_h_e_%_2_0_2_._0_-_b_l_u_e_._s_v_g_]
            _O_v_e_r_v_i_e_w â¢ _I_n_s_t_a_l_l â¢ _U_s_a_g_e â¢ _R_e_l_a_t_e_d â¢ _R_e_f_e_r_e_n_c_e_s
@@ -23,25 +24,29 @@
 [Hirschmuller, 2008]](#1.), [[Ernst, Ines & HirschmÃ¼ller, 2008]](#2.) and [
 [HirschmÃ¼ller, Buder & Ernst, 2012]](#3.). ## Install **libsgm** is available
 on Pypi and can be installed by: ```bash pip install numpy pip install libsgm
 ``` ## Usage libSGM must be used as a package : ```python from libSGM import
 sgm_wrapper ... cost_volumes_out = sgm_wrapper.sgm_api(cost_volume_in, p1, p2,
 directions, invalid_value, False, False) ``` Let's see [pandora_plugin_LibSGM]
 (https://github.com/CNES/pandora_plugin_libsgm) for real life exemple. ##
-Related [Pandora](https://github.com/CNES/Pandora) - A stereo matching
-framework [Plugin_LibSGM](https://github.com/CNES/pandora_plugin_libsgm) -
-Stereo Matching Algorithm plugin for Pandora ## References Please cite the
-following paper when using libsgm: *Cournet, M., Sarrazin, E., Dumas, L.,
-Michel, J., Guinet, J., Youssefi, D., Defonte, V., Fardet, Q., 2020. Ground-
-truth generation and disparity estimation for optical satellite imagery. ISPRS
-- International Archives of the Photogrammetry, Remote Sensing and Spatial
-Information Sciences.* [Hirschmuller, 2008] *H. Hirschmuller, "Stereo
-Processing by Semiglobal Matching and Mutual Information," in IEEE Transactions
-on Pattern Analysis and Machine Intelligence, vol. 30, no. 2, pp. 328-341, Feb.
-2008. doi: 10.1109/TPAMI.2007.1166* [Ernst, Ines & HirschmÃ¼ller, 2008] *Ernst,
-Ines & HirschmÃ¼ller, Heiko. (2008). Mutual Information Based Semi-Global
-Stereo Matching on the GPU. Proceedings of the International Symposium on
-Visual Computing. 5358. 10.1007/978-3-540-89639-5_22.* [HirschmÃ¼ller, Buder &
-Ernst, 2012] *HirschmÃ¼ller, Heiko & Buder, Maximilian & Ernst, Ines. (2012).
-Memory Efficient Semi-Global Matching. ISPRS Annals of Photogrammetry, Remote
-Sensing and Spatial Information Sciences. I-3. 10.5194/isprsannals-I-3-371-
-2012.*
+Documentation To build documentation, `doxygen` must be installed on your
+system. Then install dependencies with `pip install .[doc]`. Go in `doc` and
+run `make html` to generate html documentation. You can serve generated
+documentation locally with `make serve` and open your webbrowser at [https://
+0.0.0.0:8000/](https://0.0.0.0:8000/). ## Related [Pandora](https://github.com/
+CNES/Pandora) - A stereo matching framework [Plugin_LibSGM](https://github.com/
+CNES/pandora_plugin_libsgm) - Stereo Matching Algorithm plugin for Pandora ##
+References Please cite the following paper when using libsgm: *Cournet, M.,
+Sarrazin, E., Dumas, L., Michel, J., Guinet, J., Youssefi, D., Defonte, V.,
+Fardet, Q., 2020. Ground-truth generation and disparity estimation for optical
+satellite imagery. ISPRS - International Archives of the Photogrammetry, Remote
+Sensing and Spatial Information Sciences.* [Hirschmuller, 2008] *H.
+Hirschmuller, "Stereo Processing by Semiglobal Matching and Mutual
+Information," in IEEE Transactions on Pattern Analysis and Machine
+Intelligence, vol. 30, no. 2, pp. 328-341, Feb. 2008. doi: 10.1109/
+TPAMI.2007.1166* [Ernst, Ines & HirschmÃ¼ller, 2008] *Ernst, Ines &
+HirschmÃ¼ller, Heiko. (2008). Mutual Information Based Semi-Global Stereo
+Matching on the GPU. Proceedings of the International Symposium on Visual
+Computing. 5358. 10.1007/978-3-540-89639-5_22.* [HirschmÃ¼ller, Buder & Ernst,
+2012] *HirschmÃ¼ller, Heiko & Buder, Maximilian & Ernst, Ines. (2012). Memory
+Efficient Semi-Global Matching. ISPRS Annals of Photogrammetry, Remote Sensing
+and Spatial Information Sciences. I-3. 10.5194/isprsannals-I-3-371-2012.*
```

### Comparing `libSGM-0.4.5/README.md` & `libsgm-0.4.6a1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -37,14 +37,24 @@
 from libSGM import sgm_wrapper
 ...
 cost_volumes_out = sgm_wrapper.sgm_api(cost_volume_in, p1, p2, directions, invalid_value, False, False)
 ```
 
 Let's see [pandora_plugin_LibSGM](https://github.com/CNES/pandora_plugin_libsgm) for real life exemple.
 
+## Documentation
+
+To build documentation, `doxygen` must be installed on your system.
+
+Then install dependencies with `pip install .[doc]`.
+
+Go in `doc` and run `make html` to generate html documentation.
+
+You can serve generated documentation locally with `make serve` and open your webbrowser at [https://0.0.0.0:8000/](https://0.0.0.0:8000/).
+
 ## Related
 
 [Pandora](https://github.com/CNES/Pandora) - A stereo matching framework  
 [Plugin_LibSGM](https://github.com/CNES/pandora_plugin_libsgm) - Stereo Matching Algorithm plugin for Pandora  
 
 ## References
```

#### html2text {}

```diff
@@ -10,25 +10,29 @@
 [Hirschmuller, 2008]](#1.), [[Ernst, Ines & HirschmÃ¼ller, 2008]](#2.) and [
 [HirschmÃ¼ller, Buder & Ernst, 2012]](#3.). ## Install **libsgm** is available
 on Pypi and can be installed by: ```bash pip install numpy pip install libsgm
 ``` ## Usage libSGM must be used as a package : ```python from libSGM import
 sgm_wrapper ... cost_volumes_out = sgm_wrapper.sgm_api(cost_volume_in, p1, p2,
 directions, invalid_value, False, False) ``` Let's see [pandora_plugin_LibSGM]
 (https://github.com/CNES/pandora_plugin_libsgm) for real life exemple. ##
-Related [Pandora](https://github.com/CNES/Pandora) - A stereo matching
-framework [Plugin_LibSGM](https://github.com/CNES/pandora_plugin_libsgm) -
-Stereo Matching Algorithm plugin for Pandora ## References Please cite the
-following paper when using libsgm: *Cournet, M., Sarrazin, E., Dumas, L.,
-Michel, J., Guinet, J., Youssefi, D., Defonte, V., Fardet, Q., 2020. Ground-
-truth generation and disparity estimation for optical satellite imagery. ISPRS
-- International Archives of the Photogrammetry, Remote Sensing and Spatial
-Information Sciences.* [Hirschmuller, 2008] *H. Hirschmuller, "Stereo
-Processing by Semiglobal Matching and Mutual Information," in IEEE Transactions
-on Pattern Analysis and Machine Intelligence, vol. 30, no. 2, pp. 328-341, Feb.
-2008. doi: 10.1109/TPAMI.2007.1166* [Ernst, Ines & HirschmÃ¼ller, 2008] *Ernst,
-Ines & HirschmÃ¼ller, Heiko. (2008). Mutual Information Based Semi-Global
-Stereo Matching on the GPU. Proceedings of the International Symposium on
-Visual Computing. 5358. 10.1007/978-3-540-89639-5_22.* [HirschmÃ¼ller, Buder &
-Ernst, 2012] *HirschmÃ¼ller, Heiko & Buder, Maximilian & Ernst, Ines. (2012).
-Memory Efficient Semi-Global Matching. ISPRS Annals of Photogrammetry, Remote
-Sensing and Spatial Information Sciences. I-3. 10.5194/isprsannals-I-3-371-
-2012.*
+Documentation To build documentation, `doxygen` must be installed on your
+system. Then install dependencies with `pip install .[doc]`. Go in `doc` and
+run `make html` to generate html documentation. You can serve generated
+documentation locally with `make serve` and open your webbrowser at [https://
+0.0.0.0:8000/](https://0.0.0.0:8000/). ## Related [Pandora](https://github.com/
+CNES/Pandora) - A stereo matching framework [Plugin_LibSGM](https://github.com/
+CNES/pandora_plugin_libsgm) - Stereo Matching Algorithm plugin for Pandora ##
+References Please cite the following paper when using libsgm: *Cournet, M.,
+Sarrazin, E., Dumas, L., Michel, J., Guinet, J., Youssefi, D., Defonte, V.,
+Fardet, Q., 2020. Ground-truth generation and disparity estimation for optical
+satellite imagery. ISPRS - International Archives of the Photogrammetry, Remote
+Sensing and Spatial Information Sciences.* [Hirschmuller, 2008] *H.
+Hirschmuller, "Stereo Processing by Semiglobal Matching and Mutual
+Information," in IEEE Transactions on Pattern Analysis and Machine
+Intelligence, vol. 30, no. 2, pp. 328-341, Feb. 2008. doi: 10.1109/
+TPAMI.2007.1166* [Ernst, Ines & HirschmÃ¼ller, 2008] *Ernst, Ines &
+HirschmÃ¼ller, Heiko. (2008). Mutual Information Based Semi-Global Stereo
+Matching on the GPU. Proceedings of the International Symposium on Visual
+Computing. 5358. 10.1007/978-3-540-89639-5_22.* [HirschmÃ¼ller, Buder & Ernst,
+2012] *HirschmÃ¼ller, Heiko & Buder, Maximilian & Ernst, Ines. (2012). Memory
+Efficient Semi-Global Matching. ISPRS Annals of Photogrammetry, Remote Sensing
+and Spatial Information Sciences. I-3. 10.5194/isprsannals-I-3-371-2012.*
```

### Comparing `libSGM-0.4.5/doc/Makefile` & `libsgm-0.4.6a1/doc/Makefile`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2020 Centre National d'Etudes Spatiales (CNES).
+# Copyright (c) 2024 Centre National d'Etudes Spatiales (CNES).
 #
 # This file is part of LIBSGM
 #
 #     https://github.com/CNES/Pandora_libsgm
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -28,18 +28,24 @@
 SOURCEDIR     = source
 BUILDDIR      = build
 
 # Put it first so that "make" without argument is like "make help".
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
-.PHONY: help Makefile clean
+.PHONY: help Makefile doxygen serve clean
+
+doxygen:
+	doxygen Doxyfile
+
+serve:
+	python -m http.server --directory build/html
 
 # Catch-all target: route all unknown targets to Sphinx using the new
 # "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
-%: Makefile
+%: Makefile doxygen
 	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
 clean:
 	rm -rf doxyoutput/ build/ 
 	@$(SPHINXBUILD) -M clean "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `libSGM-0.4.5/doc/make.bat` & `libsgm-0.4.6a1/doc/make.bat`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ::
-:: Copyright (c) 2020 Centre National d'Etudes Spatiales (CNES).
+:: Copyright (c) 2024 Centre National d'Etudes Spatiales (CNES).
 ::
 :: This file is part of LIBSGM
 ::
 ::     https://github.com/CNES/Pandora_libsgm
 ::
 :: Licensed under the Apache License, Version 2.0 (the "License");
 :: you may not use this file except in compliance with the License.
```

### Comparing `libSGM-0.4.5/doc/source/Doxyfile` & `libsgm-0.4.6a1/doc/Doxyfile`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 PROJECT_LOGO           =
 
 # The OUTPUT_DIRECTORY tag is used to specify the (relative or absolute) path
 # into which the generated documentation will be written. If a relative path is
 # entered, it will be relative to the location where doxygen was started. If
 # left blank the current directory will be used.
 
-OUTPUT_DIRECTORY       = ../doxyoutput/
+OUTPUT_DIRECTORY       = doxyoutput/
 
 # If the CREATE_SUBDIRS tag is set to YES then doxygen will create 4096 sub-
 # directories (in 2 levels) under the output directory of each output format and
 # will distribute the generated files over these directories. Enabling this
 # option can be useful when feeding doxygen a huge amount of source files, where
 # putting all generated files in the same directory would otherwise causes
 # performance problems for the file system.
@@ -786,15 +786,15 @@
 
 # The INPUT tag is used to specify the files and/or directories that contain
 # documented source files. You may enter file names like myfile.cpp or
 # directories like /usr/src/myproject. Separate the files or directories with
 # spaces. See also FILE_PATTERNS and EXTENSION_MAPPING
 # Note: If this tag is empty the current directory is searched.
 
-INPUT                  = ../../sources/lib/
+INPUT                  = ../src/libSGM/lib/
 
 # This tag can be used to specify the character encoding of the source files
 # that doxygen parses. Internally doxygen uses the UTF-8 encoding. Doxygen uses
 # libiconv (or the iconv built into libc) for the transcoding. See the libiconv
 # documentation (see: http://www.gnu.org/software/libiconv) for the list of
 # possible encodings.
 # The default value is: UTF-8.
```

### Comparing `libSGM-0.4.5/doc/source/api_reference/libsgm_python/lr_manager/index.rst` & `libsgm-0.4.6a1/doc/source/api_reference/libsgm_python/lr_manager/index.rst`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/doc/source/api_reference/libsgm_python/sgm_python/index.rst` & `libsgm-0.4.6a1/doc/source/api_reference/libsgm_python/sgm_python/index.rst`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/doc/source/api_reference/libsgm_python/sgm_python_parall/index.rst` & `libsgm-0.4.6a1/doc/source/api_reference/libsgm_python/sgm_python_parall/index.rst`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/doc/source/conf.py` & `libsgm-0.4.6a1/doc/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # pylint: skip-file
-# Copyright (c) 2020 Centre National d'Etudes Spatiales (CNES).
+# Copyright (c) 2024 Centre National d'Etudes Spatiales (CNES).
 #
 # This file is part of LIBSGM
 #
 #     https://github.com/CNES/Pandora_libsgm
 #
 # Licensed under the Apache License, Version 2.0 (the 'License');
 # you may not use this file except in compliance with the License.
@@ -33,15 +33,15 @@
 # import sys
 # sys.path.insert(0, os.path.abspath('.'))
 
 
 # -- Project information -----------------------------------------------------
 
 project = "libSGM"
-copyright = "2020, CNES"
+copyright = "2024, CNES"
 author = "CNES"
 
 # The full version, including alpha/beta/rc tags
 release = "1.A"
 
 
 # -- General configuration ---------------------------------------------------
@@ -66,15 +66,15 @@
 exhale_args = {
     # These arguments are required
     "containmentFolder": "./api_reference/",
     "rootFileName": "library_root.rst",
     "rootFileTitle": "Library C++ API",
     "doxygenStripFromPath": "..",
     "exhaleExecutesDoxygen": True,
-    "exhaleDoxygenStdin": "INPUT =../../sources/lib/sgm.hpp",
+    "exhaleDoxygenStdin": "INPUT =../../src/libSGM/lib/sgm.hpp",
 }
 
 # Tell sphinx what the primary language being documented is.
 primary_domain = "cpp"
 
 # Tell sphinx what the pygments highlight language should be.
 highlight_language = "cpp"
```

### Comparing `libSGM-0.4.5/doc/source/developer_guide/before_coding.rst` & `libsgm-0.4.6a1/doc/source/developer_guide/before_coding.rst`

 * *Files 26% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 =============
 
 Thinks and tips to know before coding
 
 About cython
 ------------
 
-We have decided to distribute the generated .c files as well as our Cython sources.
+We have decided to distribute the generated .cpp files as well as our Cython sources.
 So, without Cython, one can install libsgm package. 
 
-This means that developers have to maintain the generated .c files. It can be done automatically, by Cython compilation.
-To generate them, make sur Cython is installed and use the following command
+This means that developers have to maintain the generated .cpp files. It can be done automatically, by Cython compilation.
+To generate them, make sur Cython is installed and use the following command in `src/libSGM`:
 
 .. sourcecode:: text
 
-    $ python setup.py build_ext
+    $ cython --cplus sgm_wrapper.pyx
 
 
 Unit testing
 ------------
 
 `Google test framework <https://github.com/google/googletest>`__ is used on this project.
 Don't forget to write and maintain unit tests.
```

### Comparing `libSGM-0.4.5/doc/source/developer_guide/lr_manager.rst` & `libsgm-0.4.6a1/doc/source/developer_guide/lr_manager.rst`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/doc/source/developer_guide/memory_optimization.rst` & `libsgm-0.4.6a1/doc/source/developer_guide/memory_optimization.rst`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/doc/source/developer_guide/piecewise_optimization.rst` & `libsgm-0.4.6a1/doc/source/developer_guide/piecewise_optimization.rst`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/doc/source/getting_started/example.rst` & `libsgm-0.4.6a1/doc/source/getting_started/example.rst`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/doc/source/getting_started/installation.rst` & `libsgm-0.4.6a1/doc/source/getting_started/installation.rst`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/doc/source/images/lr_manager.png` & `libsgm-0.4.6a1/doc/source/images/lr_manager.png`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/doc/source/images/piecewise_optimization.png` & `libsgm-0.4.6a1/doc/source/images/piecewise_optimization.png`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/doc/source/images/sgm_memory_optim.png` & `libsgm-0.4.6a1/doc/source/images/sgm_memory_optim.png`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/libSGM.egg-info/PKG-INFO` & `libsgm-0.4.6a1/src/libSGM.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: libSGM
-Version: 0.4.5
+Version: 0.4.6a1
 Summary: libSGM is a CNES version of H.Hirschmuller Semi-Global Matching
 Home-page: https://github.com/CNES/Pandora_libsgm
 Author: CNES
 Author-email: myriam.cournet@cnes.fr
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.22; python_version > "3.7"
 Requires-Dist: numpy; python_version < "3.8"
 Requires-Dist: numba>=0.55.2; python_version > "3.7"
 Requires-Dist: numba>=0.47.0; python_version < "3.8"
+Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx_rtd_theme; extra == "docs"
+Requires-Dist: sphinx_autoapi; extra == "docs"
+Requires-Dist: breathe; extra == "docs"
+Requires-Dist: exhale; extra == "docs"
 Provides-Extra: dev
-Requires-Dist: sphinx; extra == "dev"
-Requires-Dist: sphinx_rtd_theme; extra == "dev"
-Requires-Dist: sphinx_autoapi; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: black; extra == "dev"
 
@@ -63,14 +66,24 @@
 from libSGM import sgm_wrapper
 ...
 cost_volumes_out = sgm_wrapper.sgm_api(cost_volume_in, p1, p2, directions, invalid_value, False, False)
 ```
 
 Let's see [pandora_plugin_LibSGM](https://github.com/CNES/pandora_plugin_libsgm) for real life exemple.
 
+## Documentation
+
+To build documentation, `doxygen` must be installed on your system.
+
+Then install dependencies with `pip install .[doc]`.
+
+Go in `doc` and run `make html` to generate html documentation.
+
+You can serve generated documentation locally with `make serve` and open your webbrowser at [https://0.0.0.0:8000/](https://0.0.0.0:8000/).
+
 ## Related
 
 [Pandora](https://github.com/CNES/Pandora) - A stereo matching framework  
 [Plugin_LibSGM](https://github.com/CNES/pandora_plugin_libsgm) - Stereo Matching Algorithm plugin for Pandora  
 
 ## References
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: libSGM Version: 0.4.5 Summary: libSGM is a CNES
+Metadata-Version: 2.1 Name: libSGM Version: 0.4.6a1 Summary: libSGM is a CNES
 version of H.Hirschmuller Semi-Global Matching Home-page: https://github.com/
 CNES/Pandora_libsgm Author: CNES Author-email: myriam.cournet@cnes.fr License:
 Apache License 2.0 Requires-Python: >=3.8 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: numpy>=1.22; python_version >
 "3.7" Requires-Dist: numpy; python_version < "3.8" Requires-Dist:
 numba>=0.55.2; python_version > "3.7" Requires-Dist: numba>=0.47.0;
-python_version < "3.8" Provides-Extra: dev Requires-Dist: sphinx; extra ==
-"dev" Requires-Dist: sphinx_rtd_theme; extra == "dev" Requires-Dist:
-sphinx_autoapi; extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-
-Dist: pytest-cov; extra == "dev" Requires-Dist: pylint; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev" Requires-Dist: mypy; extra == "dev"
-Requires-Dist: black; extra == "dev"
+python_version < "3.8" Provides-Extra: docs Requires-Dist: sphinx; extra ==
+"docs" Requires-Dist: sphinx_rtd_theme; extra == "docs" Requires-Dist:
+sphinx_autoapi; extra == "docs" Requires-Dist: breathe; extra == "docs"
+Requires-Dist: exhale; extra == "docs" Provides-Extra: dev Requires-Dist:
+pytest; extra == "dev" Requires-Dist: pytest-cov; extra == "dev" Requires-Dist:
+pylint; extra == "dev" Requires-Dist: pre-commit; extra == "dev" Requires-Dist:
+mypy; extra == "dev" Requires-Dist: black; extra == "dev"
                              ************ lliibbSSGGMM ************
                     ****** SSeemmii--GGlloobbaall MMaattcchhiinngg aallggoorriitthhmm.. ******
    _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_C_N_E_S_/_P_a_n_d_o_r_a___l_i_b_S_G_M_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_l_i_b_s_g_m___c_i_._y_m_l_/
   _b_a_d_g_e_._s_v_g_?_b_r_a_n_c_h_=_m_a_s_t_e_r_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_C_N_E_S_/_P_a_n_d_o_r_a___l_i_b_S_G_M_/_b_r_a_n_c_h_/
 _m_a_s_t_e_r_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_O_Z_C_Y_I_8_4_3_J_H_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-
                             _A_p_a_c_h_e_%_2_0_2_._0_-_b_l_u_e_._s_v_g_]
            _O_v_e_r_v_i_e_w â¢ _I_n_s_t_a_l_l â¢ _U_s_a_g_e â¢ _R_e_l_a_t_e_d â¢ _R_e_f_e_r_e_n_c_e_s
@@ -23,25 +24,29 @@
 [Hirschmuller, 2008]](#1.), [[Ernst, Ines & HirschmÃ¼ller, 2008]](#2.) and [
 [HirschmÃ¼ller, Buder & Ernst, 2012]](#3.). ## Install **libsgm** is available
 on Pypi and can be installed by: ```bash pip install numpy pip install libsgm
 ``` ## Usage libSGM must be used as a package : ```python from libSGM import
 sgm_wrapper ... cost_volumes_out = sgm_wrapper.sgm_api(cost_volume_in, p1, p2,
 directions, invalid_value, False, False) ``` Let's see [pandora_plugin_LibSGM]
 (https://github.com/CNES/pandora_plugin_libsgm) for real life exemple. ##
-Related [Pandora](https://github.com/CNES/Pandora) - A stereo matching
-framework [Plugin_LibSGM](https://github.com/CNES/pandora_plugin_libsgm) -
-Stereo Matching Algorithm plugin for Pandora ## References Please cite the
-following paper when using libsgm: *Cournet, M., Sarrazin, E., Dumas, L.,
-Michel, J., Guinet, J., Youssefi, D., Defonte, V., Fardet, Q., 2020. Ground-
-truth generation and disparity estimation for optical satellite imagery. ISPRS
-- International Archives of the Photogrammetry, Remote Sensing and Spatial
-Information Sciences.* [Hirschmuller, 2008] *H. Hirschmuller, "Stereo
-Processing by Semiglobal Matching and Mutual Information," in IEEE Transactions
-on Pattern Analysis and Machine Intelligence, vol. 30, no. 2, pp. 328-341, Feb.
-2008. doi: 10.1109/TPAMI.2007.1166* [Ernst, Ines & HirschmÃ¼ller, 2008] *Ernst,
-Ines & HirschmÃ¼ller, Heiko. (2008). Mutual Information Based Semi-Global
-Stereo Matching on the GPU. Proceedings of the International Symposium on
-Visual Computing. 5358. 10.1007/978-3-540-89639-5_22.* [HirschmÃ¼ller, Buder &
-Ernst, 2012] *HirschmÃ¼ller, Heiko & Buder, Maximilian & Ernst, Ines. (2012).
-Memory Efficient Semi-Global Matching. ISPRS Annals of Photogrammetry, Remote
-Sensing and Spatial Information Sciences. I-3. 10.5194/isprsannals-I-3-371-
-2012.*
+Documentation To build documentation, `doxygen` must be installed on your
+system. Then install dependencies with `pip install .[doc]`. Go in `doc` and
+run `make html` to generate html documentation. You can serve generated
+documentation locally with `make serve` and open your webbrowser at [https://
+0.0.0.0:8000/](https://0.0.0.0:8000/). ## Related [Pandora](https://github.com/
+CNES/Pandora) - A stereo matching framework [Plugin_LibSGM](https://github.com/
+CNES/pandora_plugin_libsgm) - Stereo Matching Algorithm plugin for Pandora ##
+References Please cite the following paper when using libsgm: *Cournet, M.,
+Sarrazin, E., Dumas, L., Michel, J., Guinet, J., Youssefi, D., Defonte, V.,
+Fardet, Q., 2020. Ground-truth generation and disparity estimation for optical
+satellite imagery. ISPRS - International Archives of the Photogrammetry, Remote
+Sensing and Spatial Information Sciences.* [Hirschmuller, 2008] *H.
+Hirschmuller, "Stereo Processing by Semiglobal Matching and Mutual
+Information," in IEEE Transactions on Pattern Analysis and Machine
+Intelligence, vol. 30, no. 2, pp. 328-341, Feb. 2008. doi: 10.1109/
+TPAMI.2007.1166* [Ernst, Ines & HirschmÃ¼ller, 2008] *Ernst, Ines &
+HirschmÃ¼ller, Heiko. (2008). Mutual Information Based Semi-Global Stereo
+Matching on the GPU. Proceedings of the International Symposium on Visual
+Computing. 5358. 10.1007/978-3-540-89639-5_22.* [HirschmÃ¼ller, Buder & Ernst,
+2012] *HirschmÃ¼ller, Heiko & Buder, Maximilian & Ernst, Ines. (2012). Memory
+Efficient Semi-Global Matching. ISPRS Annals of Photogrammetry, Remote Sensing
+and Spatial Information Sciences. I-3. 10.5194/isprsannals-I-3-371-2012.*
```

### Comparing `libSGM-0.4.5/libSGM.egg-info/SOURCES.txt` & `libsgm-0.4.6a1/src/libSGM.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 setup.py
 sonar-project.properties
 .github/workflows/libsgm_ci.yml
 .gitlab/README.md
 .gitlab/issue_templates/Bug.md
 .gitlab/issue_templates/Proposition.md
 .gitlab/merge_request_templates/MR.md
+doc/Doxyfile
 doc/Makefile
 doc/make.bat
-doc/source/Doxyfile
 doc/source/api_reference.rst
 doc/source/conf.py
 doc/source/developer_guide.rst
 doc/source/getting_started.rst
 doc/source/index.rst
 doc/source/user_guide.rst
 doc/source/api_reference/sgm_wrapper.rst
@@ -40,29 +40,29 @@
 doc/source/developer_guide/piecewise_optimization.rst
 doc/source/getting_started/example.rst
 doc/source/getting_started/installation.rst
 doc/source/getting_started/quick_overview.rst
 doc/source/images/lr_manager.png
 doc/source/images/piecewise_optimization.png
 doc/source/images/sgm_memory_optim.png
-libSGM.egg-info/PKG-INFO
-libSGM.egg-info/SOURCES.txt
-libSGM.egg-info/dependency_links.txt
-libSGM.egg-info/entry_points.txt
-libSGM.egg-info/not-zip-safe
-libSGM.egg-info/requires.txt
-libSGM.egg-info/top_level.txt
-libsgm_python/__init__.py
-libsgm_python/lr_manager.py
-libsgm_python/sgm_python.py
-libsgm_python/sgm_python_parall.py
-sources/sgm_wrapper.cpp
-sources/sgm_wrapper.pyx
-sources/lib/sgm.cpp
-sources/lib/sgm.hpp
+src/libSGM/sgm_wrapper.cpp
+src/libSGM/sgm_wrapper.pyx
+src/libSGM.egg-info/PKG-INFO
+src/libSGM.egg-info/SOURCES.txt
+src/libSGM.egg-info/dependency_links.txt
+src/libSGM.egg-info/entry_points.txt
+src/libSGM.egg-info/not-zip-safe
+src/libSGM.egg-info/requires.txt
+src/libSGM.egg-info/top_level.txt
+src/libSGM/lib/sgm.cpp
+src/libSGM/lib/sgm.hpp
+src/libsgm_python/__init__.py
+src/libsgm_python/lr_manager.py
+src/libsgm_python/sgm_python.py
+src/libsgm_python/sgm_python_parall.py
 test/__init__.py
 test/functions_unittest.cpp
 test/include/gtest/gtest-death-test.h
 test/include/gtest/gtest-matchers.h
 test/include/gtest/gtest-message.h
 test/include/gtest/gtest-param-test.h
 test/include/gtest/gtest-printers.h
```

### Comparing `libSGM-0.4.5/libsgm_python/lr_manager.py` & `libsgm-0.4.6a1/src/libsgm_python/lr_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pylint:disable=fixme
 #!/usr/bin/env python
 # coding: utf8
 #
-# Copyright (c) 2020 Centre National d'Etudes Spatiales (CNES).
+# Copyright (c) 2024 Centre National d'Etudes Spatiales (CNES).
 #
 # This file is part of LIBSGM
 #
 #     https://github.com/CNES/Pandora_libsgm
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `libSGM-0.4.5/libsgm_python/sgm_python.py` & `libsgm-0.4.6a1/src/libsgm_python/sgm_python.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # coding: utf8
 #
-# Copyright (c) 2020 Centre National d'Etudes Spatiales (CNES).
+# Copyright (c) 2024 Centre National d'Etudes Spatiales (CNES).
 #
 # This file is part of LIBSGM
 #
 #     https://github.com/CNES/Pandora_libsgm
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `libSGM-0.4.5/libsgm_python/sgm_python_parall.py` & `libsgm-0.4.6a1/src/libsgm_python/sgm_python_parall.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # coding: utf8
 #
-# Copyright (c) 2020 Centre National d'Etudes Spatiales (CNES).
+# Copyright (c) 2024 Centre National d'Etudes Spatiales (CNES).
 #
 # This file is part of LIBSGM
 #
 #     https://github.com/CNES/Pandora_libsgm
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `libSGM-0.4.5/mypy.ini` & `libsgm-0.4.6a1/mypy.ini`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/setup.cfg` & `libsgm-0.4.6a1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -7,34 +7,40 @@
 url = https://github.com/CNES/Pandora_libsgm
 license = Apache License 2.0
 license_file = LICENSE
 
 [options]
 python_requires = >=3.8
 setup_requires = 
-	setuptools>=65.5
+	setuptools>=69.1
 	setuptools_scm[toml]>=6.2 # Following https://pypi.org/project/setuptools-scm/
 install_requires = 
 	numpy>=1.22;python_version>'3.7'
 	numpy;python_version<'3.8'
 	numba>=0.55.2;python_version>'3.7'
 	numba>=0.47.0;python_version<'3.8'
 package_dir = 
-	. = libsgm
+	=src
 packages = find:
 
+[options.packages.find]
+where = src
+
 [options.entry_points]
 libsgm = 
 	python_libsgm = libsgm_python.sgm_python:run_sgm
 
 [options.extras_require]
-dev = 
+docs = 
 	sphinx
 	sphinx_rtd_theme
 	sphinx_autoapi
+	breathe
+	exhale
+dev = 
 	pytest
 	pytest-cov
 	pylint
 	pre-commit
 	mypy
 	black
```

### Comparing `libSGM-0.4.5/sonar-project.properties` & `libsgm-0.4.6a1/sonar-project.properties`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 sonar.projectKey=outilscommuns:correlateurchaine3D:libsgm
 
 # project metadata
 sonar.projectName=LibSGM
 sonar.projectVersion=0.1
 
 # path to source directories (required)
-sonar.sources=sources
+sonar.sources=src
+
+# Files to exclude from analysis
+sonar.exclusions = src/libSGM/sgm_wrapper.cpp
 
 # path to test source directories (optional)
 sonar.tests=test
 
 
 # properties related to C language
 ## GCC
```

### Comparing `libSGM-0.4.5/sources/lib/sgm.cpp` & `libsgm-0.4.6a1/src/libSGM/lib/sgm.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
- * Copyright (c) 2020 Centre National d'Etudes Spatiales (CNES).
+ * Copyright (c) 2024 Centre National d'Etudes Spatiales (CNES).
  *
  * This file is part of LIBSGM
  *
  *     https://github.com/CNES/Pandora_libsgm
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
@@ -215,21 +215,21 @@
     float reset7;
 
 
     int overcounting_factor;
 
     if (overcounting)
     {
-	// Factor to correct the overcounting: number of directions [8] - 1
-	overcounting_factor = 7;
+        // Factor to correct the overcounting: number of directions [8] - 1
+        overcounting_factor = 7;
     }
     else
     {
-	// Factor to not correct the over-counting
-	overcounting_factor = 0;
+        // Factor to not correct the over-counting
+        overcounting_factor = 0;
     }
 
     for (int row = nb_rows-1; row >= 0; row --)
     {
         for (int col = nb_cols-1; col >= 0; col --)
         {
             //right->left
```

### Comparing `libSGM-0.4.5/sources/lib/sgm.hpp` & `libsgm-0.4.6a1/src/libSGM/lib/sgm.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
- * Copyright (c) 2020 Centre National d'Etudes Spatiales (CNES).
+ * Copyright (c) 2024 Centre National d'Etudes Spatiales (CNES).
  *
  * This file is part of LIBSGM
  *
  *     https://github.com/CNES/Pandora_libsgm
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
@@ -20,32 +20,35 @@
 
 #include <stdint.h>
 
 /**
 * Structure to represent Aggregated Cost Volume and the positions of minimum costs along each direction
 */
 struct CostVolumes{
-    float * cost_volume;
-    int * cost_volume_min;
+    float * cost_volume; /**< Aggregated Cost Volume */
+    int * cost_volume_min; /**< positions of minimum costs along each direction */
 };
 
 
 /**
 * Structure to represent coordinates of previous point path
 */
 
 struct Direction{
     int drow; /**< row coordinate */
     int dcol; /**< col coordinate */
 };
 
+/**
+* Structure to represent Penalty
+*/
 template<typename T>
 struct Penalty{
-    T P1;
-    T P2;
+    T P1; /**< Penalty 1 */
+    T P2; /**< Penalty 2 */
 };
 
 /*!
  *  \brief  Compute aggregated cost volume
  *   Compute aggregated cost volume following
  *   Semi-Global algorithm by Hirschmuller
  *
```

### Comparing `libSGM-0.4.5/sources/sgm_wrapper.cpp` & `libsgm-0.4.6a1/src/libSGM/sgm_wrapper.cpp`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/sources/sgm_wrapper.pyx` & `libsgm-0.4.6a1/src/libSGM/sgm_wrapper.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # coding: utf8
 #
-# Copyright (c) 2020 Centre National d'Etudes Spatiales (CNES).
+# Copyright (c) 2024 Centre National d'Etudes Spatiales (CNES).
 #
 # This file is part of LIBSGM
 #
 #     https://github.com/CNES/Pandora_libsgm
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `libSGM-0.4.5/test/functions_unittest.cpp` & `libsgm-0.4.6a1/test/functions_unittest.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
- * Copyright (c) 2020 Centre National d'Etudes Spatiales (CNES).
+ * Copyright (c) 2024 Centre National d'Etudes Spatiales (CNES).
  *
  * This file is part of LIBSGM
  *
  *     https://github.com/CNES/Pandora_libsgm
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
@@ -15,15 +15,15 @@
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
 
 #include "gtest/gtest.h"
-#include "../../sources/lib/sgm.hpp"
+#include "../../src/libSGM/lib/sgm.hpp"
 
 
 //Global Test of sgm function: aggregation value from 8 directions on a middle point of cost volume
 //with invalid middle point and without over-counting correction
 
 TEST(sgmTest, TestMiddleValueInvalid){
```

### Comparing `libSGM-0.4.5/test/include/gtest/gtest-death-test.h` & `libsgm-0.4.6a1/test/include/gtest/gtest-death-test.h`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/test/include/gtest/gtest-matchers.h` & `libsgm-0.4.6a1/test/include/gtest/gtest-matchers.h`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/test/include/gtest/gtest-message.h` & `libsgm-0.4.6a1/test/include/gtest/gtest-message.h`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/test/include/gtest/gtest-param-test.h` & `libsgm-0.4.6a1/test/include/gtest/gtest-param-test.h`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/test/include/gtest/gtest-printers.h` & `libsgm-0.4.6a1/test/include/gtest/gtest-printers.h`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/test/include/gtest/gtest-spi.h` & `libsgm-0.4.6a1/test/include/gtest/gtest-spi.h`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/test/include/gtest/gtest-test-part.h` & `libsgm-0.4.6a1/test/include/gtest/gtest-test-part.h`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/test/include/gtest/gtest-typed-test.h` & `libsgm-0.4.6a1/test/include/gtest/gtest-typed-test.h`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/test/include/gtest/gtest.h` & `libsgm-0.4.6a1/test/include/gtest/gtest.h`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/test/include/gtest/gtest_pred_impl.h` & `libsgm-0.4.6a1/test/include/gtest/gtest_pred_impl.h`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/test/include/gtest/gtest_prod.h` & `libsgm-0.4.6a1/test/include/gtest/gtest_prod.h`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/test/include/gtest/internal/custom/README.md` & `libsgm-0.4.6a1/test/include/gtest/internal/custom/README.md`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/test/include/gtest/internal/custom/gtest-port.h` & `libsgm-0.4.6a1/test/include/gtest/internal/custom/gtest-port.h`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/test/include/gtest/internal/custom/gtest-printers.h` & `libsgm-0.4.6a1/test/include/gtest/internal/custom/gtest-printers.h`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/test/include/gtest/internal/custom/gtest.h` & `libsgm-0.4.6a1/test/include/gtest/internal/custom/gtest.h`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/test/include/gtest/internal/gtest-death-test-internal.h` & `libsgm-0.4.6a1/test/include/gtest/internal/gtest-death-test-internal.h`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/test/include/gtest/internal/gtest-filepath.h` & `libsgm-0.4.6a1/test/include/gtest/internal/gtest-filepath.h`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/test/include/gtest/internal/gtest-internal.h` & `libsgm-0.4.6a1/test/include/gtest/internal/gtest-internal.h`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/test/include/gtest/internal/gtest-param-util.h` & `libsgm-0.4.6a1/test/include/gtest/internal/gtest-param-util.h`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/test/include/gtest/internal/gtest-port-arch.h` & `libsgm-0.4.6a1/test/include/gtest/internal/gtest-port-arch.h`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/test/include/gtest/internal/gtest-port.h` & `libsgm-0.4.6a1/test/include/gtest/internal/gtest-port.h`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/test/include/gtest/internal/gtest-string.h` & `libsgm-0.4.6a1/test/include/gtest/internal/gtest-string.h`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/test/include/gtest/internal/gtest-type-util.h` & `libsgm-0.4.6a1/test/include/gtest/internal/gtest-type-util.h`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/test/include/gtest/internal/gtest-type-util.h.pump` & `libsgm-0.4.6a1/test/include/gtest/internal/gtest-type-util.h.pump`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/test/src/gtest-all.cc` & `libsgm-0.4.6a1/test/src/gtest-all.cc`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/test/src/gtest-death-test.cc` & `libsgm-0.4.6a1/test/src/gtest-death-test.cc`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/test/src/gtest-filepath.cc` & `libsgm-0.4.6a1/test/src/gtest-filepath.cc`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/test/src/gtest-internal-inl.h` & `libsgm-0.4.6a1/test/src/gtest-internal-inl.h`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/test/src/gtest-matchers.cc` & `libsgm-0.4.6a1/test/src/gtest-matchers.cc`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/test/src/gtest-port.cc` & `libsgm-0.4.6a1/test/src/gtest-port.cc`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/test/src/gtest-printers.cc` & `libsgm-0.4.6a1/test/src/gtest-printers.cc`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/test/src/gtest-test-part.cc` & `libsgm-0.4.6a1/test/src/gtest-test-part.cc`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/test/src/gtest-typed-test.cc` & `libsgm-0.4.6a1/test/src/gtest-typed-test.cc`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/test/src/gtest.cc` & `libsgm-0.4.6a1/test/src/gtest.cc`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/test/src/gtest_main.cc` & `libsgm-0.4.6a1/test/src/gtest_main.cc`

 * *Files identical despite different names*

### Comparing `libSGM-0.4.5/test/test_libsgm_python/common.py` & `libsgm-0.4.6a1/test/test_libsgm_python/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # coding: utf8
 #
-# Copyright (c) 2020 Centre National d'Etudes Spatiales (CNES).
+# Copyright (c) 2024 Centre National d'Etudes Spatiales (CNES).
 #
 # This file is part of LIBSGM
 #
 #     https://github.com/CNES/Pandora_libsgm
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `libSGM-0.4.5/test/test_libsgm_python/disable_test_sgm_python_parall.py` & `libsgm-0.4.6a1/test/test_libsgm_python/disable_test_sgm_python_parall.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # coding: utf8
 #
-# Copyright (c) 2020 Centre National d'Etudes Spatiales (CNES).
+# Copyright (c) 2024 Centre National d'Etudes Spatiales (CNES).
 #
 # This file is part of LIBSGM
 #
 #     https://github.com/CNES/Pandora_libsgm
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `libSGM-0.4.5/test/test_libsgm_python/test_lr_manager.py` & `libsgm-0.4.6a1/test/test_libsgm_python/test_lr_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pylint:disable = not-callable
 #!/usr/bin/env python
 # coding: utf8
 #
-# Copyright (c) 2020 Centre National d'Etudes Spatiales (CNES).
+# Copyright (c) 2024 Centre National d'Etudes Spatiales (CNES).
 #
 # This file is part of LIBSGM
 #
 #     https://github.com/CNES/Pandora_libsgm
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `libSGM-0.4.5/test/test_libsgm_python/test_sgm_python.py` & `libsgm-0.4.6a1/test/test_libsgm_python/test_sgm_python.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # coding: utf8
 #
-# Copyright (c) 2020 Centre National d'Etudes Spatiales (CNES).
+# Copyright (c) 2024 Centre National d'Etudes Spatiales (CNES).
 #
 # This file is part of LIBSGM
 #
 #     https://github.com/CNES/Pandora_libsgm
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

