# Comparing `tmp/hikari_arc-1.3.3.tar.gz` & `tmp/hikari_arc-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikari_arc-1.3.3.tar", last modified: Mon May 27 13:13:15 2024, max compression
+gzip compressed data, was "hikari_arc-1.3.4.tar", last modified: Sun Jun  2 22:47:17 2024, max compression
```

## Comparing `hikari_arc-1.3.3.tar` & `hikari_arc-1.3.4.tar`

### file list

```diff
@@ -1,92 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:13:15.210282 hikari_arc-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-05-27 13:13:15.210282 hikari_arc-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:13:15.194283 hikari_arc-1.3.3/arc/
--rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:13:15.198283 hikari_arc-1.3.3/arc/abc/
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/abc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54155 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/abc/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    28462 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/abc/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/abc/concurrency_limiting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/abc/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/abc/hookable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/abc/limiter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12981 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/abc/option.py
--rw-r--r--   0 runner    (1001) docker     (127)    19700 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/abc/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    17850 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:13:15.198283 hikari_arc-1.3.3/arc/command/
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5943 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/command/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:13:15.198283 hikari_arc-1.3.3/arc/command/option/
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/command/option/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/command/option/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/command/option/bool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/command/option/channel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:13:15.202283 hikari_arc-1.3.3/arc/command/option/custom/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/command/option/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/command/option/custom/color.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/command/option/custom/member.py
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/command/option/float.py
--rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/command/option/int.py
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/command/option/mentionable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/command/option/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/command/option/str.py
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/command/option/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    35491 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/command/slash.py
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/command/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:13:15.202283 hikari_arc-1.3.3/arc/context/
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/context/autocomplete.py
--rw-r--r--   0 runner    (1001) docker     (127)    39976 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/context/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:13:15.202283 hikari_arc-1.3.3/arc/ext/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/extension.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:13:15.202283 hikari_arc-1.3.3/arc/internal/
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/internal/about.py
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/internal/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/internal/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    13518 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/internal/sigparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    12589 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/internal/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/internal/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/internal/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/locale.py
--rw-r--r--   0 runner    (1001) docker     (127)     8622 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:13:15.202283 hikari_arc-1.3.3/arc/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12959 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/utils/concurrency_limiter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:13:15.206282 hikari_arc-1.3.3/arc/utils/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/utils/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5889 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/utils/hooks/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/utils/hooks/limiters.py
--rw-r--r--   0 runner    (1001) docker     (127)    14009 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/utils/loops.py
--rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/utils/ratelimiter.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/cron_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/doc_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:13:15.206282 hikari_arc-1.3.3/hikari_arc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-05-27 13:13:15.000000 hikari_arc-1.3.3/hikari_arc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-27 13:13:15.000000 hikari_arc-1.3.3/hikari_arc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 13:13:15.000000 hikari_arc-1.3.3/hikari_arc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 13:13:15.000000 hikari_arc-1.3.3/hikari_arc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-27 13:13:15.000000 hikari_arc-1.3.3/hikari_arc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-27 13:13:15.000000 hikari_arc-1.3.3/hikari_arc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/rest_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 13:13:15.210282 hikari_arc-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:13:15.206282 hikari_arc-1.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/tests/test_context_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/tests/test_di.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/tests/test_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/tests/test_sigparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/tests/test_slash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:17.108597 hikari_arc-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-06-02 22:47:17.108597 hikari_arc-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:17.096597 hikari_arc-1.3.4/arc/
+-rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:17.096597 hikari_arc-1.3.4/arc/abc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/abc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54108 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/abc/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28462 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/abc/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/abc/concurrency_limiting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/abc/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/abc/hookable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/abc/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12981 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/abc/option.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19700 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/abc/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17850 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:17.096597 hikari_arc-1.3.4/arc/command/
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5943 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/command/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:17.096597 hikari_arc-1.3.4/arc/command/option/
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/command/option/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/command/option/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/command/option/bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/command/option/channel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:17.100597 hikari_arc-1.3.4/arc/command/option/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/command/option/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/command/option/custom/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/command/option/custom/member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/command/option/float.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/command/option/int.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/command/option/mentionable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/command/option/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/command/option/str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/command/option/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35491 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/command/slash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/command/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:17.100597 hikari_arc-1.3.4/arc/context/
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/context/autocomplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39976 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/context/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:17.100597 hikari_arc-1.3.4/arc/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:17.100597 hikari_arc-1.3.4/arc/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/internal/about.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/internal/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/internal/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13518 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/internal/sigparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12589 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/internal/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/internal/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/internal/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/locale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8622 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:17.100597 hikari_arc-1.3.4/arc/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12959 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/utils/concurrency_limiter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:17.100597 hikari_arc-1.3.4/arc/utils/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/utils/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/utils/hooks/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/utils/hooks/limiters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14009 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/utils/loops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/arc/utils/ratelimiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/cron_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/doc_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:17.104597 hikari_arc-1.3.4/hikari_arc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-06-02 22:47:17.000000 hikari_arc-1.3.4/hikari_arc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-06-02 22:47:17.000000 hikari_arc-1.3.4/hikari_arc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 22:47:17.000000 hikari_arc-1.3.4/hikari_arc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 22:47:16.000000 hikari_arc-1.3.4/hikari_arc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-06-02 22:47:17.000000 hikari_arc-1.3.4/hikari_arc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-06-02 22:47:17.000000 hikari_arc-1.3.4/hikari_arc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/rest_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 22:47:17.108597 hikari_arc-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:17.104597 hikari_arc-1.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10226 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/tests/test_context_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/tests/test_di.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/tests/test_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/tests/test_sigparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-06-02 22:47:13.000000 hikari_arc-1.3.4/tests/test_slash.py
```

### Comparing `hikari_arc-1.3.3/LICENSE` & `hikari_arc-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/PKG-INFO` & `hikari_arc-1.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikari-arc
-Version: 1.3.3
+Version: 1.3.4
 Summary: A command handler for hikari with a focus on type-safety and correctness.
 Home-page: https://github.com/hypergonial/hikari-arc
 Author: hypergonial
 Author-email: git@hypergonial.com
 Maintainer: hypergonial
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,25 +24,25 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hikari>=2.0.0.dev122
 Requires-Dist: alluka<0.4,>=0.3.0
 Requires-Dist: attrs>=23.1
 Requires-Dist: colorama; sys_platform == "win32"
 Provides-Extra: docs
-Requires-Dist: mkdocs-material[imaging]~=9.5.24; extra == "docs"
+Requires-Dist: mkdocs-material[imaging]~=9.5.25; extra == "docs"
 Requires-Dist: mkdocs~=1.6.0; extra == "docs"
 Requires-Dist: mkdocstrings-python~=1.10.3; extra == "docs"
 Requires-Dist: black~=24.4.2; extra == "docs"
 Requires-Dist: griffe-inherited-docstrings~=1.0.0; extra == "docs"
 Requires-Dist: mkdocs-glightbox~=0.4.0; extra == "docs"
 Provides-Extra: dev
-Requires-Dist: ruff==0.4.5; extra == "dev"
-Requires-Dist: pyright==1.1.364; extra == "dev"
+Requires-Dist: ruff==0.4.6; extra == "dev"
+Requires-Dist: pyright==1.1.365; extra == "dev"
 Requires-Dist: nox==2024.4.15; extra == "dev"
-Requires-Dist: typing_extensions==4.11.0; extra == "dev"
+Requires-Dist: typing_extensions==4.12.0; extra == "dev"
 Requires-Dist: pytest==8.2.1; extra == "dev"
 Requires-Dist: pytest-asyncio==0.23.7; extra == "dev"
 Requires-Dist: slotscheck==0.19.0; extra == "dev"
 Provides-Extra: rest
 Requires-Dist: hikari[server]>=2.0.0.dev122; extra == "rest"
 Provides-Extra: cron
 Requires-Dist: croniter==2.0.5; extra == "cron"
```

### Comparing `hikari_arc-1.3.3/README.md` & `hikari_arc-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/__init__.py` & `hikari_arc-1.3.4/arc/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/__main__.py` & `hikari_arc-1.3.4/arc/__main__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/abc/__init__.py` & `hikari_arc-1.3.4/arc/abc/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/abc/client.py` & `hikari_arc-1.3.4/arc/abc/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -329,18 +329,18 @@
             if ctx.is_valid:
                 await ctx.respond("❌ Something went wrong. Please contact the bot developer.")
 
     async def _create_overriding_ctx_for_command(self, ctx: Context[te.Self]) -> alluka.OverridingContext:
         inj_ctx = alluka.OverridingContext.from_client(self.injector)
 
         for hook in self._injection_hooks:
-            if inspect.isawaitable(hook):
-                await hook(ctx, inj_ctx)  # type: ignore
-            else:
-                hook(ctx, inj_ctx)
+            res = hook(ctx, inj_ctx)
+
+            if inspect.isawaitable(res):
+                await res
         return inj_ctx
 
     def _provide_command_locale(self, request: CommandLocaleRequest) -> LocaleResponse:
         """Provide a locale for a command."""
         if self._command_locale_provider is None:
             return LocaleResponse(name=request.command.name, description=getattr(request.command, "description", None))
```

### Comparing `hikari_arc-1.3.3/arc/abc/command.py` & `hikari_arc-1.3.4/arc/abc/command.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/abc/concurrency_limiting.py` & `hikari_arc-1.3.4/arc/abc/concurrency_limiting.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/abc/error_handler.py` & `hikari_arc-1.3.4/arc/abc/error_handler.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/abc/hookable.py` & `hikari_arc-1.3.4/arc/abc/hookable.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/abc/limiter.py` & `hikari_arc-1.3.4/arc/abc/limiter.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/abc/option.py` & `hikari_arc-1.3.4/arc/abc/option.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/abc/plugin.py` & `hikari_arc-1.3.4/arc/abc/plugin.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/client.py` & `hikari_arc-1.3.4/arc/client.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/command/__init__.py` & `hikari_arc-1.3.4/arc/command/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/command/message.py` & `hikari_arc-1.3.4/arc/command/message.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/command/option/__init__.py` & `hikari_arc-1.3.4/arc/command/option/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/command/option/attachment.py` & `hikari_arc-1.3.4/arc/command/option/attachment.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/command/option/bool.py` & `hikari_arc-1.3.4/arc/command/option/bool.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/command/option/channel.py` & `hikari_arc-1.3.4/arc/command/option/channel.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/command/option/custom/color.py` & `hikari_arc-1.3.4/arc/command/option/custom/color.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/command/option/custom/member.py` & `hikari_arc-1.3.4/arc/command/option/custom/member.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/command/option/float.py` & `hikari_arc-1.3.4/arc/command/option/float.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/command/option/int.py` & `hikari_arc-1.3.4/arc/command/option/int.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/command/option/mentionable.py` & `hikari_arc-1.3.4/arc/command/option/mentionable.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/command/option/role.py` & `hikari_arc-1.3.4/arc/command/option/role.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/command/option/str.py` & `hikari_arc-1.3.4/arc/command/option/str.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/command/option/user.py` & `hikari_arc-1.3.4/arc/command/option/user.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/command/slash.py` & `hikari_arc-1.3.4/arc/command/slash.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/command/user.py` & `hikari_arc-1.3.4/arc/command/user.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/context/__init__.py` & `hikari_arc-1.3.4/arc/context/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/context/autocomplete.py` & `hikari_arc-1.3.4/arc/context/autocomplete.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/context/base.py` & `hikari_arc-1.3.4/arc/context/base.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/errors.py` & `hikari_arc-1.3.4/arc/errors.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/events.py` & `hikari_arc-1.3.4/arc/events.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/extension.py` & `hikari_arc-1.3.4/arc/extension.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/internal/__init__.py` & `hikari_arc-1.3.4/arc/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/internal/about.py` & `hikari_arc-1.3.4/arc/internal/about.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing as t
 
 __author__: t.Final[str] = "hypergonial"
 __author_email__: t.Final[str] = "git@hypergonial.com"
 __maintainer__: t.Final[str] = "hypergonial"
 __license__: t.Final[str] = "MIT"
 __url__: t.Final[str] = "https://github.com/hypergonial/hikari-arc"
-__version__: t.Final[str] = "1.3.3"
+__version__: t.Final[str] = "1.3.4"
 
 # MIT License
 #
 # Copyright (c) 2023-present hypergonial
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
```

### Comparing `hikari_arc-1.3.3/arc/internal/deprecation.py` & `hikari_arc-1.3.4/arc/internal/deprecation.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/internal/options.py` & `hikari_arc-1.3.4/arc/internal/options.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/internal/sigparse.py` & `hikari_arc-1.3.4/arc/internal/sigparse.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/internal/sync.py` & `hikari_arc-1.3.4/arc/internal/sync.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/internal/types.py` & `hikari_arc-1.3.4/arc/internal/types.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/internal/version.py` & `hikari_arc-1.3.4/arc/internal/version.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/locale.py` & `hikari_arc-1.3.4/arc/locale.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/plugin.py` & `hikari_arc-1.3.4/arc/plugin.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/utils/__init__.py` & `hikari_arc-1.3.4/arc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/utils/concurrency_limiter.py` & `hikari_arc-1.3.4/arc/utils/concurrency_limiter.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/utils/hooks/__init__.py` & `hikari_arc-1.3.4/arc/utils/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/utils/hooks/basic.py` & `hikari_arc-1.3.4/arc/utils/hooks/basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from __future__ import annotations
 
 import typing as t
 
 import hikari
 
 from arc.abc.hookable import HookResult
+from arc.context import Context  # noqa: TCH001 Needed for DI to work
 from arc.errors import (
     BotMissingPermissionsError,
     DMOnlyError,
     GuildOnlyError,
     InvokerMissingPermissionsError,
     NotOwnerError,
 )
 
-if t.TYPE_CHECKING:
-    from arc.context import Context
-
 
 def guild_only(ctx: Context[t.Any]) -> HookResult:
     """A pre-execution hook that aborts the execution of a command if it is invoked outside of a guild.
 
     Example
     --------
     ```py
```

### Comparing `hikari_arc-1.3.3/arc/utils/hooks/limiters.py` & `hikari_arc-1.3.4/arc/utils/hooks/limiters.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/utils/loops.py` & `hikari_arc-1.3.4/arc/utils/loops.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/arc/utils/ratelimiter.py` & `hikari_arc-1.3.4/arc/utils/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/hikari_arc.egg-info/PKG-INFO` & `hikari_arc-1.3.4/hikari_arc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikari-arc
-Version: 1.3.3
+Version: 1.3.4
 Summary: A command handler for hikari with a focus on type-safety and correctness.
 Home-page: https://github.com/hypergonial/hikari-arc
 Author: hypergonial
 Author-email: git@hypergonial.com
 Maintainer: hypergonial
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,25 +24,25 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hikari>=2.0.0.dev122
 Requires-Dist: alluka<0.4,>=0.3.0
 Requires-Dist: attrs>=23.1
 Requires-Dist: colorama; sys_platform == "win32"
 Provides-Extra: docs
-Requires-Dist: mkdocs-material[imaging]~=9.5.24; extra == "docs"
+Requires-Dist: mkdocs-material[imaging]~=9.5.25; extra == "docs"
 Requires-Dist: mkdocs~=1.6.0; extra == "docs"
 Requires-Dist: mkdocstrings-python~=1.10.3; extra == "docs"
 Requires-Dist: black~=24.4.2; extra == "docs"
 Requires-Dist: griffe-inherited-docstrings~=1.0.0; extra == "docs"
 Requires-Dist: mkdocs-glightbox~=0.4.0; extra == "docs"
 Provides-Extra: dev
-Requires-Dist: ruff==0.4.5; extra == "dev"
-Requires-Dist: pyright==1.1.364; extra == "dev"
+Requires-Dist: ruff==0.4.6; extra == "dev"
+Requires-Dist: pyright==1.1.365; extra == "dev"
 Requires-Dist: nox==2024.4.15; extra == "dev"
-Requires-Dist: typing_extensions==4.11.0; extra == "dev"
+Requires-Dist: typing_extensions==4.12.0; extra == "dev"
 Requires-Dist: pytest==8.2.1; extra == "dev"
 Requires-Dist: pytest-asyncio==0.23.7; extra == "dev"
 Requires-Dist: slotscheck==0.19.0; extra == "dev"
 Provides-Extra: rest
 Requires-Dist: hikari[server]>=2.0.0.dev122; extra == "rest"
 Provides-Extra: cron
 Requires-Dist: croniter==2.0.5; extra == "cron"
```

### Comparing `hikari_arc-1.3.3/hikari_arc.egg-info/SOURCES.txt` & `hikari_arc-1.3.4/hikari_arc.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -65,13 +65,14 @@
 hikari_arc.egg-info/PKG-INFO
 hikari_arc.egg-info/SOURCES.txt
 hikari_arc.egg-info/dependency_links.txt
 hikari_arc.egg-info/not-zip-safe
 hikari_arc.egg-info/requires.txt
 hikari_arc.egg-info/top_level.txt
 tests/test_client.py
+tests/test_command.py
 tests/test_context_command.py
 tests/test_di.py
 tests/test_inheritance.py
 tests/test_options.py
 tests/test_sigparse.py
 tests/test_slash.py
```

### Comparing `hikari_arc-1.3.3/pyproject.toml` & `hikari_arc-1.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/setup.py` & `hikari_arc-1.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/tests/test_client.py` & `hikari_arc-1.3.4/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/tests/test_context_command.py` & `hikari_arc-1.3.4/tests/test_context_command.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/tests/test_di.py` & `hikari_arc-1.3.4/tests/test_di.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/tests/test_inheritance.py` & `hikari_arc-1.3.4/tests/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/tests/test_options.py` & `hikari_arc-1.3.4/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/tests/test_sigparse.py` & `hikari_arc-1.3.4/tests/test_sigparse.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.3/tests/test_slash.py` & `hikari_arc-1.3.4/tests/test_slash.py`

 * *Files identical despite different names*

