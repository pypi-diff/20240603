# Comparing `tmp/abcli-9.62.1.tar.gz` & `tmp/abcli-9.63.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abcli-9.62.1.tar", last modified: Mon Jun  3 04:19:37 2024, max compression
+gzip compressed data, was "abcli-9.63.1.tar", last modified: Mon Jun  3 04:22:41 2024, max compression
```

## Comparing `abcli-9.62.1.tar` & `abcli-9.63.1.tar`

### file list

```diff
@@ -1,241 +1,241 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.156227 abcli-9.62.1/
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-26 21:47:30.000000 abcli-9.62.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     2168 2024-06-03 04:19:37.155465 abcli-9.62.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     1262 2024-06-03 04:19:20.000000 abcli-9.62.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.070815 abcli-9.62.1/abcli/
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.073294 abcli-9.62.1/abcli/.abcli/
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.076018 abcli-9.62.1/abcli/.abcli/abcli/
--rw-r--r--   0 kamangir   (502) staff       (20)      208 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/abcli/arg.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      140 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/abcli/bool.sh
--rwxr-xr-x   0 kamangir   (502) staff       (20)      176 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/abcli/file.sh
--rwxr-xr-x   0 kamangir   (502) staff       (20)      895 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/abcli/keyword.sh
--rwxr-xr-x   0 kamangir   (502) staff       (20)      972 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/abcli/list.sh
--rwxr-xr-x   0 kamangir   (502) staff       (20)      704 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/abcli/options.sh
--rwxr-xr-x   0 kamangir   (502) staff       (20)      826 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/abcli/string.sh
--rwxr-xr-x   0 kamangir   (502) staff       (20)     1732 2024-06-03 01:59:01.000000 abcli-9.62.1/abcli/.abcli/abcli.sh
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.078051 abcli-9.62.1/abcli/.abcli/bootstrap/
--rw-r--r--   0 kamangir   (502) staff       (20)     1440 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/bootstrap/dependencies.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      527 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/bootstrap/install.sh
--rwxr-xr-x   0 kamangir   (502) staff       (20)     3894 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/bootstrap/logging.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      580 2024-06-03 01:59:01.000000 abcli-9.62.1/abcli/.abcli/bootstrap/paths.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      998 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/bootstrap/source.sh
--rwxr-xr-x   0 kamangir   (502) staff       (20)     4291 2024-06-03 01:59:01.000000 abcli-9.62.1/abcli/.abcli/bootstrap/system.sh
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.081530 abcli-9.62.1/abcli/.abcli/modules/
--rw-r--r--   0 kamangir   (502) staff       (20)      417 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/modules/abcli.sh
--rwxr-xr-x   0 kamangir   (502) staff       (20)     1666 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/modules/download.sh
--rwxr-xr-x   0 kamangir   (502) staff       (20)     6596 2024-06-03 01:59:01.000000 abcli-9.62.1/abcli/.abcli/modules/env.sh
--rwxr-xr-x   0 kamangir   (502) staff       (20)     1077 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/modules/help.sh
--rwxr-xr-x   0 kamangir   (502) staff       (20)     2500 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/modules/host.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1345 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/modules/init.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      726 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/modules/initialize.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1574 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/modules/object.sh
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.082638 abcli-9.62.1/abcli/.abcli/modules/plugins/
--rw-r--r--   0 kamangir   (502) staff       (20)      976 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/modules/plugins/generic.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      753 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/modules/plugins/get.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      689 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/modules/plugins/install.sh
--rwxr-xr-x   0 kamangir   (502) staff       (20)      982 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/modules/plugins.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1262 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/modules/select.sh
--rwxr-xr-x   0 kamangir   (502) staff       (20)     5370 2024-06-03 01:59:01.000000 abcli-9.62.1/abcli/.abcli/modules/terraform.sh
--rwxr-xr-x   0 kamangir   (502) staff       (20)     2147 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/modules/upload.sh
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.103219 abcli-9.62.1/abcli/.abcli/plugins/
--rw-r--r--   0 kamangir   (502) staff       (20)     2007 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/GPU.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      796 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/actions.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1598 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/add.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1627 2024-06-02 21:13:49.000000 abcli-9.62.1/abcli/.abcli/plugins/alias.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      308 2024-06-02 21:15:05.000000 abcli-9.62.1/abcli/.abcli/plugins/badge.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      526 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/browse.sh
--rwxr-xr-x   0 kamangir   (502) staff       (20)     1855 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/cache.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1869 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/clone.sh
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.103670 abcli-9.62.1/abcli/.abcli/plugins/conda/
--rw-r--r--   0 kamangir   (502) staff       (20)     1414 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/conda/create.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1981 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/conda.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1010 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/eval.sh
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.108432 abcli-9.62.1/abcli/.abcli/plugins/git/
--rw-r--r--   0 kamangir   (502) staff       (20)      321 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/git/browse.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     3314 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/git/clone.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      644 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/git/create_branch.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      294 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/git/get_repo_name.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      347 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/git/increment_version.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1015 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/git/pull.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1514 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/git/push.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1305 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/git/review.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      492 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/git/status.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      624 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/git/utils.sh
--rwxr-xr-x   0 kamangir   (502) staff       (20)     5016 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/git.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      447 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/graphics.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     2630 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/huggingface.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1394 2024-05-31 02:43:14.000000 abcli-9.62.1/abcli/.abcli/plugins/install.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     6335 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/instance.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1602 2024-05-31 04:37:38.000000 abcli-9.62.1/abcli/.abcli/plugins/latex.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      853 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/list.sh
--rwxr-xr-x   0 kamangir   (502) staff       (20)     2232 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/message.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     3044 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/metadata.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      767 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/open.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1207 2024-05-31 02:43:14.000000 abcli-9.62.1/abcli/.abcli/plugins/papertrail.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      488 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/pause.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      459 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/pip.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     2304 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/publish.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1179 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/pylint.sh
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.110021 abcli-9.62.1/abcli/.abcli/plugins/pypi/
--rw-r--r--   0 kamangir   (502) staff       (20)      665 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/pypi/browse.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1500 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/pypi/build.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      315 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/pypi/install.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      620 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/pypi.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1109 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/pytest.sh
--rwxr-xr-x   0 kamangir   (502) staff       (20)     2536 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/relations.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      473 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/repeat.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      850 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/scp.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      920 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/screen.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     9957 2024-06-03 01:59:01.000000 abcli-9.62.1/abcli/.abcli/plugins/seed.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     3284 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/session.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      384 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/sleep.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     3317 2024-06-03 01:59:01.000000 abcli-9.62.1/abcli/.abcli/plugins/ssh.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     2594 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/storage.sh
--rwxr-xr-x   0 kamangir   (502) staff       (20)     2691 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/tags.sh
--rwxr-xr-x   0 kamangir   (502) staff       (20)     1690 2024-06-03 04:09:40.000000 abcli-9.62.1/abcli/.abcli/plugins/terminal.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     3168 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/test.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      587 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/watch.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1461 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/plugins/wifi.sh
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.114066 abcli-9.62.1/abcli/.abcli/tests/
--rw-r--r--   0 kamangir   (502) staff       (20)     3956 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/tests/abcli_clarify_object.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      223 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/tests/env.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      704 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/tests/keyword.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      178 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/tests/list.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      953 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/tests/list_functions.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      448 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/tests/log_list.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1602 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/tests/metadata.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     3069 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/tests/options.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1700 2024-05-26 21:47:33.000000 abcli-9.62.1/abcli/.abcli/tests/plugins.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      150 2024-05-28 01:33:08.000000 abcli-9.62.1/abcli/.abcli/tests/version.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      339 2024-06-03 04:19:31.000000 abcli-9.62.1/abcli/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      237 2024-05-28 01:01:55.000000 abcli-9.62.1/abcli/__main__.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.114465 abcli-9.62.1/abcli/assets/
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.115337 abcli-9.62.1/abcli/assets/aws/
--rw-r--r--   0 kamangir   (502) staff       (20)       56 2024-06-03 01:59:01.000000 abcli-9.62.1/abcli/assets/aws/ec2_bash_profile
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.118510 abcli-9.62.1/abcli/assets/env/
--rw-r--r--   0 kamangir   (502) staff       (20)      224 2024-06-03 01:59:01.000000 abcli-9.62.1/abcli/assets/env/area550.env
--rw-r--r--   0 kamangir   (502) staff       (20)      149 2024-06-03 01:59:01.000000 abcli-9.62.1/abcli/assets/env/candle.env
--rw-r--r--   0 kamangir   (502) staff       (20)      148 2024-06-03 01:59:01.000000 abcli-9.62.1/abcli/assets/env/dec82.env
--rw-r--r--   0 kamangir   (502) staff       (20)      160 2024-06-03 01:59:01.000000 abcli-9.62.1/abcli/assets/env/dec82q.env
--rw-r--r--   0 kamangir   (502) staff       (20)       55 2024-06-03 01:59:01.000000 abcli-9.62.1/abcli/assets/env/eye.env
--rw-r--r--   0 kamangir   (502) staff       (20)      341 2024-06-03 01:59:01.000000 abcli-9.62.1/abcli/assets/env/may26.env
--rw-r--r--   0 kamangir   (502) staff       (20)      124 2024-06-03 01:59:01.000000 abcli-9.62.1/abcli/assets/env/mirror.env
--rw-r--r--   0 kamangir   (502) staff       (20)      153 2024-06-03 01:59:01.000000 abcli-9.62.1/abcli/assets/env/nurah.env
--rw-r--r--   0 kamangir   (502) staff       (20)      138 2024-06-03 01:59:01.000000 abcli-9.62.1/abcli/assets/env/portal.env
--rw-r--r--   0 kamangir   (502) staff       (20)       83 2024-06-03 01:59:01.000000 abcli-9.62.1/abcli/assets/env/thermal.env
--rw-r--r--   0 kamangir   (502) staff       (20)      147 2024-06-03 01:59:01.000000 abcli-9.62.1/abcli/assets/env/unicorn.env
--rw-r--r--   0 kamangir   (502) staff       (20)      155 2024-06-03 01:59:01.000000 abcli-9.62.1/abcli/assets/env/worker.env
--rw-r--r--   0 kamangir   (502) staff       (20)   575810 2024-06-03 01:59:01.000000 abcli-9.62.1/abcli/assets/marquee.png
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.119006 abcli-9.62.1/abcli/assets/script/
--rw-r--r--   0 kamangir   (502) staff       (20)      222 2024-06-03 01:59:01.000000 abcli-9.62.1/abcli/assets/script/script.py
--rw-r--r--   0 kamangir   (502) staff       (20)      105 2024-06-03 01:59:01.000000 abcli-9.62.1/abcli/assets/script/script.sh
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.120183 abcli-9.62.1/abcli/bash/
--rw-r--r--   0 kamangir   (502) staff       (20)        0 2022-08-19 04:11:13.000000 abcli-9.62.1/abcli/bash/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       96 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/bash/colors.py
--rw-r--r--   0 kamangir   (502) staff       (20)      598 2024-02-18 05:10:50.000000 abcli-9.62.1/abcli/bash/help.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2309 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/bash/list.py
--rw-r--r--   0 kamangir   (502) staff       (20)      777 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/bash/logging.py
--rw-r--r--   0 kamangir   (502) staff       (20)      784 2024-06-03 01:14:54.000000 abcli-9.62.1/abcli/config.env
--rw-r--r--   0 kamangir   (502) staff       (20)      537 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/elapsed_timer.py
--rw-r--r--   0 kamangir   (502) staff       (20)     5294 2024-06-03 01:59:01.000000 abcli-9.62.1/abcli/env.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.121996 abcli-9.62.1/abcli/file/
--rw-r--r--   0 kamangir   (502) staff       (20)      109 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/file/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      996 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/file/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      570 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/file/classes.py
--rw-r--r--   0 kamangir   (502) staff       (20)     9177 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/file/functions.py
--rw-r--r--   0 kamangir   (502) staff       (20)     6315 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/file/load.py
--rw-r--r--   0 kamangir   (502) staff       (20)     7303 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/file/save.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.123837 abcli-9.62.1/abcli/keywords/
--rw-r--r--   0 kamangir   (502) staff       (20)       84 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/keywords/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      897 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/keywords/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      236 2022-08-20 04:12:52.000000 abcli-9.62.1/abcli/keywords/functions.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1407 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/keywords/keywords.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1353 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/logger.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.125830 abcli-9.62.1/abcli/modules/
--rw-r--r--   0 kamangir   (502) staff       (20)       23 2022-08-28 06:57:23.000000 abcli-9.62.1/abcli/modules/__init__.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.127125 abcli-9.62.1/abcli/modules/host/
--rw-r--r--   0 kamangir   (502) staff       (20)       90 2022-09-21 00:58:39.000000 abcli-9.62.1/abcli/modules/host/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2523 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/modules/host/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     5416 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/modules/host/functions.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2025 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/modules/objects.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.128064 abcli-9.62.1/abcli/options/
--rw-r--r--   0 kamangir   (502) staff       (20)       53 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/options/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1751 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/options/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2826 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/options/classes.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.129087 abcli-9.62.1/abcli/path/
--rw-r--r--   0 kamangir   (502) staff       (20)       68 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/path/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       10 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/path/consts.py
--rw-r--r--   0 kamangir   (502) staff       (20)     5254 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/path/functions.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.131477 abcli-9.62.1/abcli/plugins/
--rw-r--r--   0 kamangir   (502) staff       (20)       49 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/plugins/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1651 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/plugins/__main__.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.132604 abcli-9.62.1/abcli/plugins/cache/
--rw-r--r--   0 kamangir   (502) staff       (20)       55 2022-08-20 04:12:52.000000 abcli-9.62.1/abcli/plugins/cache/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1646 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/plugins/cache/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     4705 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/plugins/cache/functions.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1265 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/plugins/functions.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.133891 abcli-9.62.1/abcli/plugins/git/
--rw-r--r--   0 kamangir   (502) staff       (20)       26 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/plugins/git/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      696 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/plugins/git/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1716 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/plugins/git/version.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.135068 abcli-9.62.1/abcli/plugins/gpu/
--rw-r--r--   0 kamangir   (502) staff       (20)       52 2022-08-20 04:12:52.000000 abcli-9.62.1/abcli/plugins/gpu/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      499 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/plugins/gpu/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      590 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/plugins/gpu/functions.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.138032 abcli-9.62.1/abcli/plugins/graphics/
--rw-r--r--   0 kamangir   (502) staff       (20)      124 2022-09-25 02:29:01.000000 abcli-9.62.1/abcli/plugins/graphics/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1462 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/plugins/graphics/constants.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1740 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/plugins/graphics/gif.py
--rw-r--r--   0 kamangir   (502) staff       (20)      431 2022-08-14 18:15:57.000000 abcli-9.62.1/abcli/plugins/graphics/image.py
--rw-r--r--   0 kamangir   (502) staff       (20)     3591 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/plugins/graphics/signature.py
--rw-r--r--   0 kamangir   (502) staff       (20)     6641 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/plugins/graphics/text.py
--rw-r--r--   0 kamangir   (502) staff       (20)      953 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/plugins/markdown.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.139650 abcli-9.62.1/abcli/plugins/metadata/
--rw-r--r--   0 kamangir   (502) staff       (20)       58 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/plugins/metadata/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2109 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/plugins/metadata/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2231 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/plugins/metadata/functions.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.141008 abcli-9.62.1/abcli/plugins/relations/
--rw-r--r--   0 kamangir   (502) staff       (20)       59 2022-08-20 04:12:52.000000 abcli-9.62.1/abcli/plugins/relations/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2102 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/plugins/relations/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     5157 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/plugins/relations/functions.py
--rw-r--r--   0 kamangir   (502) staff       (20)      705 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/plugins/seed.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.142345 abcli-9.62.1/abcli/plugins/storage/
--rw-r--r--   0 kamangir   (502) staff       (20)       83 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/plugins/storage/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2248 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/plugins/storage/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     8063 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/plugins/storage/classes.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.143844 abcli-9.62.1/abcli/plugins/tags/
--rw-r--r--   0 kamangir   (502) staff       (20)       55 2022-08-20 04:12:52.000000 abcli-9.62.1/abcli/plugins/tags/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2219 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/plugins/tags/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     5991 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/plugins/tags/functions.py
--rw-r--r--   0 kamangir   (502) staff       (20)      344 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/plugins/testing.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1313 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/plugins/video.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.146833 abcli-9.62.1/abcli/string/
--rw-r--r--   0 kamangir   (502) staff       (20)      244 2024-02-18 05:23:47.000000 abcli-9.62.1/abcli/string/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1138 2024-02-18 05:23:40.000000 abcli-9.62.1/abcli/string/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      216 2024-02-18 05:23:45.000000 abcli-9.62.1/abcli/string/constants.py
--rw-r--r--   0 kamangir   (502) staff       (20)    11283 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/string/functions.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.147799 abcli-9.62.1/abcli/table/
--rw-r--r--   0 kamangir   (502) staff       (20)       45 2022-08-20 04:12:52.000000 abcli-9.62.1/abcli/table/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     4541 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/table/classes.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.153595 abcli-9.62.1/abcli/tests/
--rw-r--r--   0 kamangir   (502) staff       (20)        0 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/tests/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       69 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/tests/test_abcli.py
--rw-r--r--   0 kamangir   (502) staff       (20)      264 2024-06-03 01:59:01.000000 abcli-9.62.1/abcli/tests/test_env.py
--rw-r--r--   0 kamangir   (502) staff       (20)      410 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/tests/test_modules_objects.py
--rw-r--r--   0 kamangir   (502) staff       (20)     3194 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/tests/test_options.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1400 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/tests/test_plugins.py
--rw-r--r--   0 kamangir   (502) staff       (20)      634 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/tests/test_plugins_graphics_gif_generate_animated_gif.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1037 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/tests/test_plugins_graphics_signature.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2831 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/tests/test_plugins_metadata.py
--rw-r--r--   0 kamangir   (502) staff       (20)      777 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/tests/test_plugins_testing.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2199 2024-05-26 21:47:30.000000 abcli-9.62.1/abcli/timer.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:19:37.154393 abcli-9.62.1/abcli.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     2168 2024-06-03 04:19:37.000000 abcli-9.62.1/abcli.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     5965 2024-06-03 04:19:37.000000 abcli-9.62.1/abcli.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-06-03 04:19:37.000000 abcli-9.62.1/abcli.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      125 2024-06-03 04:19:37.000000 abcli-9.62.1/abcli.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        6 2024-06-03 04:19:37.000000 abcli-9.62.1/abcli.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-26 21:47:30.000000 abcli-9.62.1/pyproject.toml
--rw-r--r--   0 kamangir   (502) staff       (20)      124 2024-05-26 21:47:30.000000 abcli-9.62.1/requirements.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-06-03 04:19:37.156375 abcli-9.62.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      943 2024-06-03 01:59:01.000000 abcli-9.62.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.249685 abcli-9.63.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-26 21:47:30.000000 abcli-9.63.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     2168 2024-06-03 04:22:41.248862 abcli-9.63.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     1262 2024-06-03 04:20:32.000000 abcli-9.63.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.173040 abcli-9.63.1/abcli/
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.175490 abcli-9.63.1/abcli/.abcli/
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.177816 abcli-9.63.1/abcli/.abcli/abcli/
+-rw-r--r--   0 kamangir   (502) staff       (20)      208 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/abcli/arg.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      140 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/abcli/bool.sh
+-rwxr-xr-x   0 kamangir   (502) staff       (20)      176 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/abcli/file.sh
+-rwxr-xr-x   0 kamangir   (502) staff       (20)      895 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/abcli/keyword.sh
+-rwxr-xr-x   0 kamangir   (502) staff       (20)      972 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/abcli/list.sh
+-rwxr-xr-x   0 kamangir   (502) staff       (20)      704 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/abcli/options.sh
+-rwxr-xr-x   0 kamangir   (502) staff       (20)      826 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/abcli/string.sh
+-rwxr-xr-x   0 kamangir   (502) staff       (20)     1732 2024-06-03 01:59:01.000000 abcli-9.63.1/abcli/.abcli/abcli.sh
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.179503 abcli-9.63.1/abcli/.abcli/bootstrap/
+-rw-r--r--   0 kamangir   (502) staff       (20)     1440 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/bootstrap/dependencies.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      527 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/bootstrap/install.sh
+-rwxr-xr-x   0 kamangir   (502) staff       (20)     3894 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/bootstrap/logging.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      580 2024-06-03 01:59:01.000000 abcli-9.63.1/abcli/.abcli/bootstrap/paths.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      998 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/bootstrap/source.sh
+-rwxr-xr-x   0 kamangir   (502) staff       (20)     4291 2024-06-03 01:59:01.000000 abcli-9.63.1/abcli/.abcli/bootstrap/system.sh
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.183489 abcli-9.63.1/abcli/.abcli/modules/
+-rw-r--r--   0 kamangir   (502) staff       (20)      417 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/modules/abcli.sh
+-rwxr-xr-x   0 kamangir   (502) staff       (20)     1666 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/modules/download.sh
+-rwxr-xr-x   0 kamangir   (502) staff       (20)     6596 2024-06-03 01:59:01.000000 abcli-9.63.1/abcli/.abcli/modules/env.sh
+-rwxr-xr-x   0 kamangir   (502) staff       (20)     1077 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/modules/help.sh
+-rwxr-xr-x   0 kamangir   (502) staff       (20)     2500 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/modules/host.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1345 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/modules/init.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      726 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/modules/initialize.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1574 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/modules/object.sh
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.184506 abcli-9.63.1/abcli/.abcli/modules/plugins/
+-rw-r--r--   0 kamangir   (502) staff       (20)      976 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/modules/plugins/generic.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      753 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/modules/plugins/get.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      689 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/modules/plugins/install.sh
+-rwxr-xr-x   0 kamangir   (502) staff       (20)      982 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/modules/plugins.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1262 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/modules/select.sh
+-rwxr-xr-x   0 kamangir   (502) staff       (20)     5370 2024-06-03 01:59:01.000000 abcli-9.63.1/abcli/.abcli/modules/terraform.sh
+-rwxr-xr-x   0 kamangir   (502) staff       (20)     2147 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/modules/upload.sh
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.203215 abcli-9.63.1/abcli/.abcli/plugins/
+-rw-r--r--   0 kamangir   (502) staff       (20)     2007 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/GPU.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      796 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/actions.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1598 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/add.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1627 2024-06-02 21:13:49.000000 abcli-9.63.1/abcli/.abcli/plugins/alias.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      308 2024-06-02 21:15:05.000000 abcli-9.63.1/abcli/.abcli/plugins/badge.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      526 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/browse.sh
+-rwxr-xr-x   0 kamangir   (502) staff       (20)     1855 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/cache.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1869 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/clone.sh
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.203857 abcli-9.63.1/abcli/.abcli/plugins/conda/
+-rw-r--r--   0 kamangir   (502) staff       (20)     1414 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/conda/create.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1981 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/conda.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1010 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/eval.sh
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.207493 abcli-9.63.1/abcli/.abcli/plugins/git/
+-rw-r--r--   0 kamangir   (502) staff       (20)      321 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/git/browse.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     3314 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/git/clone.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      644 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/git/create_branch.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      294 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/git/get_repo_name.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      347 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/git/increment_version.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1015 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/git/pull.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1514 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/git/push.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1305 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/git/review.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      492 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/git/status.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      624 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/git/utils.sh
+-rwxr-xr-x   0 kamangir   (502) staff       (20)     5016 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/git.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      447 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/graphics.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     2630 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/huggingface.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1394 2024-05-31 02:43:14.000000 abcli-9.63.1/abcli/.abcli/plugins/install.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     6335 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/instance.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1602 2024-05-31 04:37:38.000000 abcli-9.63.1/abcli/.abcli/plugins/latex.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      853 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/list.sh
+-rwxr-xr-x   0 kamangir   (502) staff       (20)     2232 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/message.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     3044 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/metadata.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      767 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/open.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1207 2024-05-31 02:43:14.000000 abcli-9.63.1/abcli/.abcli/plugins/papertrail.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      488 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/pause.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      459 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/pip.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     2304 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/publish.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1179 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/pylint.sh
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.208571 abcli-9.63.1/abcli/.abcli/plugins/pypi/
+-rw-r--r--   0 kamangir   (502) staff       (20)      665 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/pypi/browse.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1500 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/pypi/build.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      315 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/pypi/install.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      620 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/pypi.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1109 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/pytest.sh
+-rwxr-xr-x   0 kamangir   (502) staff       (20)     2536 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/relations.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      473 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/repeat.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      850 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/scp.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      920 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/screen.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     9957 2024-06-03 01:59:01.000000 abcli-9.63.1/abcli/.abcli/plugins/seed.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     3284 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/session.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      384 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/sleep.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     3317 2024-06-03 01:59:01.000000 abcli-9.63.1/abcli/.abcli/plugins/ssh.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     2594 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/storage.sh
+-rwxr-xr-x   0 kamangir   (502) staff       (20)     2691 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/tags.sh
+-rwxr-xr-x   0 kamangir   (502) staff       (20)     1690 2024-06-03 04:09:40.000000 abcli-9.63.1/abcli/.abcli/plugins/terminal.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     3168 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/test.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      587 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/watch.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1461 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/plugins/wifi.sh
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.212421 abcli-9.63.1/abcli/.abcli/tests/
+-rw-r--r--   0 kamangir   (502) staff       (20)     3956 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/tests/abcli_clarify_object.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      223 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/tests/env.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      704 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/tests/keyword.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      178 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/tests/list.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      953 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/tests/list_functions.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      448 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/tests/log_list.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1602 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/tests/metadata.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     3069 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/tests/options.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1700 2024-05-26 21:47:33.000000 abcli-9.63.1/abcli/.abcli/tests/plugins.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      150 2024-05-28 01:33:08.000000 abcli-9.63.1/abcli/.abcli/tests/version.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      339 2024-06-03 04:22:36.000000 abcli-9.63.1/abcli/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      237 2024-05-28 01:01:55.000000 abcli-9.63.1/abcli/__main__.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.212906 abcli-9.63.1/abcli/assets/
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.216560 abcli-9.63.1/abcli/assets/aws/
+-rw-r--r--   0 kamangir   (502) staff       (20)       56 2024-06-03 01:59:01.000000 abcli-9.63.1/abcli/assets/aws/ec2_bash_profile
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.220304 abcli-9.63.1/abcli/assets/env/
+-rw-r--r--   0 kamangir   (502) staff       (20)      224 2024-06-03 01:59:01.000000 abcli-9.63.1/abcli/assets/env/area550.env
+-rw-r--r--   0 kamangir   (502) staff       (20)      149 2024-06-03 01:59:01.000000 abcli-9.63.1/abcli/assets/env/candle.env
+-rw-r--r--   0 kamangir   (502) staff       (20)      148 2024-06-03 01:59:01.000000 abcli-9.63.1/abcli/assets/env/dec82.env
+-rw-r--r--   0 kamangir   (502) staff       (20)      160 2024-06-03 01:59:01.000000 abcli-9.63.1/abcli/assets/env/dec82q.env
+-rw-r--r--   0 kamangir   (502) staff       (20)       55 2024-06-03 01:59:01.000000 abcli-9.63.1/abcli/assets/env/eye.env
+-rw-r--r--   0 kamangir   (502) staff       (20)      341 2024-06-03 01:59:01.000000 abcli-9.63.1/abcli/assets/env/may26.env
+-rw-r--r--   0 kamangir   (502) staff       (20)      124 2024-06-03 01:59:01.000000 abcli-9.63.1/abcli/assets/env/mirror.env
+-rw-r--r--   0 kamangir   (502) staff       (20)      153 2024-06-03 01:59:01.000000 abcli-9.63.1/abcli/assets/env/nurah.env
+-rw-r--r--   0 kamangir   (502) staff       (20)      138 2024-06-03 01:59:01.000000 abcli-9.63.1/abcli/assets/env/portal.env
+-rw-r--r--   0 kamangir   (502) staff       (20)       83 2024-06-03 01:59:01.000000 abcli-9.63.1/abcli/assets/env/thermal.env
+-rw-r--r--   0 kamangir   (502) staff       (20)      147 2024-06-03 01:59:01.000000 abcli-9.63.1/abcli/assets/env/unicorn.env
+-rw-r--r--   0 kamangir   (502) staff       (20)      155 2024-06-03 01:59:01.000000 abcli-9.63.1/abcli/assets/env/worker.env
+-rw-r--r--   0 kamangir   (502) staff       (20)  2192018 2024-06-03 04:21:12.000000 abcli-9.63.1/abcli/assets/marquee.png
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.220878 abcli-9.63.1/abcli/assets/script/
+-rw-r--r--   0 kamangir   (502) staff       (20)      222 2024-06-03 01:59:01.000000 abcli-9.63.1/abcli/assets/script/script.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      105 2024-06-03 01:59:01.000000 abcli-9.63.1/abcli/assets/script/script.sh
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.222056 abcli-9.63.1/abcli/bash/
+-rw-r--r--   0 kamangir   (502) staff       (20)        0 2022-08-19 04:11:13.000000 abcli-9.63.1/abcli/bash/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       96 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/bash/colors.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      598 2024-02-18 05:10:50.000000 abcli-9.63.1/abcli/bash/help.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2309 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/bash/list.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      777 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/bash/logging.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      784 2024-06-03 01:14:54.000000 abcli-9.63.1/abcli/config.env
+-rw-r--r--   0 kamangir   (502) staff       (20)      537 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/elapsed_timer.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     5294 2024-06-03 01:59:01.000000 abcli-9.63.1/abcli/env.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.223630 abcli-9.63.1/abcli/file/
+-rw-r--r--   0 kamangir   (502) staff       (20)      109 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/file/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      996 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/file/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      570 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/file/classes.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     9177 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/file/functions.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     6315 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/file/load.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     7303 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/file/save.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.224657 abcli-9.63.1/abcli/keywords/
+-rw-r--r--   0 kamangir   (502) staff       (20)       84 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/keywords/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      897 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/keywords/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      236 2022-08-20 04:12:52.000000 abcli-9.63.1/abcli/keywords/functions.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1407 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/keywords/keywords.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1353 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/logger.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.225280 abcli-9.63.1/abcli/modules/
+-rw-r--r--   0 kamangir   (502) staff       (20)       23 2022-08-28 06:57:23.000000 abcli-9.63.1/abcli/modules/__init__.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.226445 abcli-9.63.1/abcli/modules/host/
+-rw-r--r--   0 kamangir   (502) staff       (20)       90 2022-09-21 00:58:39.000000 abcli-9.63.1/abcli/modules/host/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2523 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/modules/host/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     5416 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/modules/host/functions.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2025 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/modules/objects.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.227302 abcli-9.63.1/abcli/options/
+-rw-r--r--   0 kamangir   (502) staff       (20)       53 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/options/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1751 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/options/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2826 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/options/classes.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.228149 abcli-9.63.1/abcli/path/
+-rw-r--r--   0 kamangir   (502) staff       (20)       68 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/path/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       10 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/path/consts.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     5254 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/path/functions.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.229824 abcli-9.63.1/abcli/plugins/
+-rw-r--r--   0 kamangir   (502) staff       (20)       49 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/plugins/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1651 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/plugins/__main__.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.230619 abcli-9.63.1/abcli/plugins/cache/
+-rw-r--r--   0 kamangir   (502) staff       (20)       55 2022-08-20 04:12:52.000000 abcli-9.63.1/abcli/plugins/cache/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1646 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/plugins/cache/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     4705 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/plugins/cache/functions.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1265 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/plugins/functions.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.231464 abcli-9.63.1/abcli/plugins/git/
+-rw-r--r--   0 kamangir   (502) staff       (20)       26 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/plugins/git/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      696 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/plugins/git/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1716 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/plugins/git/version.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.232250 abcli-9.63.1/abcli/plugins/gpu/
+-rw-r--r--   0 kamangir   (502) staff       (20)       52 2022-08-20 04:12:52.000000 abcli-9.63.1/abcli/plugins/gpu/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      499 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/plugins/gpu/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      590 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/plugins/gpu/functions.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.233817 abcli-9.63.1/abcli/plugins/graphics/
+-rw-r--r--   0 kamangir   (502) staff       (20)      124 2022-09-25 02:29:01.000000 abcli-9.63.1/abcli/plugins/graphics/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1462 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/plugins/graphics/constants.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1740 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/plugins/graphics/gif.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      431 2022-08-14 18:15:57.000000 abcli-9.63.1/abcli/plugins/graphics/image.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     3591 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/plugins/graphics/signature.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     6641 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/plugins/graphics/text.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      953 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/plugins/markdown.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.234567 abcli-9.63.1/abcli/plugins/metadata/
+-rw-r--r--   0 kamangir   (502) staff       (20)       58 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/plugins/metadata/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2109 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/plugins/metadata/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2231 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/plugins/metadata/functions.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.235767 abcli-9.63.1/abcli/plugins/relations/
+-rw-r--r--   0 kamangir   (502) staff       (20)       59 2022-08-20 04:12:52.000000 abcli-9.63.1/abcli/plugins/relations/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2102 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/plugins/relations/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     5157 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/plugins/relations/functions.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      705 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/plugins/seed.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.237054 abcli-9.63.1/abcli/plugins/storage/
+-rw-r--r--   0 kamangir   (502) staff       (20)       83 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/plugins/storage/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2248 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/plugins/storage/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     8063 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/plugins/storage/classes.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.238764 abcli-9.63.1/abcli/plugins/tags/
+-rw-r--r--   0 kamangir   (502) staff       (20)       55 2022-08-20 04:12:52.000000 abcli-9.63.1/abcli/plugins/tags/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2219 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/plugins/tags/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     5991 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/plugins/tags/functions.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      344 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/plugins/testing.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1313 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/plugins/video.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.240963 abcli-9.63.1/abcli/string/
+-rw-r--r--   0 kamangir   (502) staff       (20)      244 2024-02-18 05:23:47.000000 abcli-9.63.1/abcli/string/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1138 2024-02-18 05:23:40.000000 abcli-9.63.1/abcli/string/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      216 2024-02-18 05:23:45.000000 abcli-9.63.1/abcli/string/constants.py
+-rw-r--r--   0 kamangir   (502) staff       (20)    11283 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/string/functions.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.242059 abcli-9.63.1/abcli/table/
+-rw-r--r--   0 kamangir   (502) staff       (20)       45 2022-08-20 04:12:52.000000 abcli-9.63.1/abcli/table/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     4541 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/table/classes.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.247222 abcli-9.63.1/abcli/tests/
+-rw-r--r--   0 kamangir   (502) staff       (20)        0 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/tests/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       69 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/tests/test_abcli.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      264 2024-06-03 01:59:01.000000 abcli-9.63.1/abcli/tests/test_env.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      410 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/tests/test_modules_objects.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     3194 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/tests/test_options.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1400 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/tests/test_plugins.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      634 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/tests/test_plugins_graphics_gif_generate_animated_gif.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1037 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/tests/test_plugins_graphics_signature.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2831 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/tests/test_plugins_metadata.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      777 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/tests/test_plugins_testing.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2199 2024-05-26 21:47:30.000000 abcli-9.63.1/abcli/timer.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 04:22:41.247990 abcli-9.63.1/abcli.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     2168 2024-06-03 04:22:41.000000 abcli-9.63.1/abcli.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     5965 2024-06-03 04:22:41.000000 abcli-9.63.1/abcli.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-06-03 04:22:41.000000 abcli-9.63.1/abcli.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      125 2024-06-03 04:22:41.000000 abcli-9.63.1/abcli.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        6 2024-06-03 04:22:41.000000 abcli-9.63.1/abcli.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-26 21:47:30.000000 abcli-9.63.1/pyproject.toml
+-rw-r--r--   0 kamangir   (502) staff       (20)      124 2024-05-26 21:47:30.000000 abcli-9.63.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-06-03 04:22:41.249871 abcli-9.63.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      943 2024-06-03 01:59:01.000000 abcli-9.63.1/setup.py
```

### Comparing `abcli-9.62.1/PKG-INFO` & `abcli-9.63.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abcli
-Version: 9.62.1
+Version: 9.63.1
 Summary: 🚀 a language to speak AI.
 Home-page: https://github.com/kamangir/awesome-bash-cli
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
@@ -23,20 +23,20 @@
 Requires-Dist: pylint
 Requires-Dist: pytest
 Requires-Dist: python-dotenv[cli]
 Requires-Dist: tqdm
 
 # awesome bash cli (abcli/abc)
 
+`abcli` 🚀 is an implementation of [🔻 giza](https://github.com/kamangir/giza) and the library behind [these projects](https://github.com/kamangir/kamangir).
+
 ![image](https://raw.githubusercontent.com/kamangir/awesome-bash-cli/current/abcli/assets/marquee.png)
 
 [![PyPI version](https://img.shields.io/pypi/v/abcli.svg)](https://pypi.org/project/abcli/)
 
-`abcli` 🚀 is an implementation of [🔻 giza](https://github.com/kamangir/giza) and the library behind [these projects](https://github.com/kamangir/kamangir).
-
 To install `abcli`, type in,
 
 ```bash
 pip install abcli
 ```
 
 or follow these (not-too-update) instructions for custom environments:
```

### Comparing `abcli-9.62.1/README.md` & `abcli-9.63.1/README.md`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # awesome bash cli (abcli/abc)
 
+`abcli` 🚀 is an implementation of [🔻 giza](https://github.com/kamangir/giza) and the library behind [these projects](https://github.com/kamangir/kamangir).
+
 ![image](./abcli/assets/marquee.png)
 
 [![PyPI version](https://img.shields.io/pypi/v/abcli.svg)](https://pypi.org/project/abcli/)
 
-`abcli` 🚀 is an implementation of [🔻 giza](https://github.com/kamangir/giza) and the library behind [these projects](https://github.com/kamangir/kamangir).
-
 To install `abcli`, type in,
 
 ```bash
 pip install abcli
 ```
 
 or follow these (not-too-update) instructions for custom environments:
```

### Comparing `abcli-9.62.1/abcli/.abcli/abcli/keyword.sh` & `abcli-9.63.1/abcli/.abcli/abcli/keyword.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/abcli/list.sh` & `abcli-9.63.1/abcli/.abcli/abcli/list.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/abcli/options.sh` & `abcli-9.63.1/abcli/.abcli/abcli/options.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/abcli/string.sh` & `abcli-9.63.1/abcli/.abcli/abcli/string.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/abcli.sh` & `abcli-9.63.1/abcli/.abcli/abcli.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/bootstrap/dependencies.sh` & `abcli-9.63.1/abcli/.abcli/bootstrap/dependencies.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/bootstrap/install.sh` & `abcli-9.63.1/abcli/.abcli/bootstrap/install.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/bootstrap/logging.sh` & `abcli-9.63.1/abcli/.abcli/bootstrap/logging.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/bootstrap/paths.sh` & `abcli-9.63.1/abcli/.abcli/bootstrap/paths.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/bootstrap/source.sh` & `abcli-9.63.1/abcli/.abcli/bootstrap/source.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/bootstrap/system.sh` & `abcli-9.63.1/abcli/.abcli/bootstrap/system.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/modules/download.sh` & `abcli-9.63.1/abcli/.abcli/modules/download.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/modules/env.sh` & `abcli-9.63.1/abcli/.abcli/modules/env.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/modules/help.sh` & `abcli-9.63.1/abcli/.abcli/modules/help.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/modules/host.sh` & `abcli-9.63.1/abcli/.abcli/modules/host.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/modules/init.sh` & `abcli-9.63.1/abcli/.abcli/modules/init.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/modules/initialize.sh` & `abcli-9.63.1/abcli/.abcli/modules/initialize.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/modules/object.sh` & `abcli-9.63.1/abcli/.abcli/modules/object.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/modules/plugins/generic.sh` & `abcli-9.63.1/abcli/.abcli/modules/plugins/generic.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/modules/plugins/get.sh` & `abcli-9.63.1/abcli/.abcli/modules/plugins/get.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/modules/plugins/install.sh` & `abcli-9.63.1/abcli/.abcli/modules/plugins/install.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/modules/plugins.sh` & `abcli-9.63.1/abcli/.abcli/modules/plugins.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/modules/select.sh` & `abcli-9.63.1/abcli/.abcli/modules/select.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/modules/terraform.sh` & `abcli-9.63.1/abcli/.abcli/modules/terraform.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/modules/upload.sh` & `abcli-9.63.1/abcli/.abcli/modules/upload.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/GPU.sh` & `abcli-9.63.1/abcli/.abcli/plugins/GPU.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/actions.sh` & `abcli-9.63.1/abcli/.abcli/plugins/actions.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/add.sh` & `abcli-9.63.1/abcli/.abcli/plugins/add.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/alias.sh` & `abcli-9.63.1/abcli/.abcli/plugins/alias.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/browse.sh` & `abcli-9.63.1/abcli/.abcli/plugins/browse.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/cache.sh` & `abcli-9.63.1/abcli/.abcli/plugins/cache.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/clone.sh` & `abcli-9.63.1/abcli/.abcli/plugins/clone.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/conda/create.sh` & `abcli-9.63.1/abcli/.abcli/plugins/conda/create.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/conda.sh` & `abcli-9.63.1/abcli/.abcli/plugins/conda.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/eval.sh` & `abcli-9.63.1/abcli/.abcli/plugins/eval.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/git/clone.sh` & `abcli-9.63.1/abcli/.abcli/plugins/git/clone.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/git/create_branch.sh` & `abcli-9.63.1/abcli/.abcli/plugins/git/create_branch.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/git/pull.sh` & `abcli-9.63.1/abcli/.abcli/plugins/git/pull.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/git/push.sh` & `abcli-9.63.1/abcli/.abcli/plugins/git/push.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/git/review.sh` & `abcli-9.63.1/abcli/.abcli/plugins/git/review.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/git/utils.sh` & `abcli-9.63.1/abcli/.abcli/plugins/git/utils.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/git.sh` & `abcli-9.63.1/abcli/.abcli/plugins/git.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/huggingface.sh` & `abcli-9.63.1/abcli/.abcli/plugins/huggingface.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/install.sh` & `abcli-9.63.1/abcli/.abcli/plugins/install.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/instance.sh` & `abcli-9.63.1/abcli/.abcli/plugins/instance.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/latex.sh` & `abcli-9.63.1/abcli/.abcli/plugins/latex.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/list.sh` & `abcli-9.63.1/abcli/.abcli/plugins/list.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/message.sh` & `abcli-9.63.1/abcli/.abcli/plugins/message.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/metadata.sh` & `abcli-9.63.1/abcli/.abcli/plugins/metadata.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/open.sh` & `abcli-9.63.1/abcli/.abcli/plugins/open.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/papertrail.sh` & `abcli-9.63.1/abcli/.abcli/plugins/papertrail.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/publish.sh` & `abcli-9.63.1/abcli/.abcli/plugins/publish.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/pylint.sh` & `abcli-9.63.1/abcli/.abcli/plugins/pylint.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/pypi/browse.sh` & `abcli-9.63.1/abcli/.abcli/plugins/pypi/browse.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/pypi/build.sh` & `abcli-9.63.1/abcli/.abcli/plugins/pypi/build.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/pypi.sh` & `abcli-9.63.1/abcli/.abcli/plugins/pypi.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/pytest.sh` & `abcli-9.63.1/abcli/.abcli/plugins/pytest.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/relations.sh` & `abcli-9.63.1/abcli/.abcli/plugins/relations.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/scp.sh` & `abcli-9.63.1/abcli/.abcli/plugins/scp.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/screen.sh` & `abcli-9.63.1/abcli/.abcli/plugins/screen.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/seed.sh` & `abcli-9.63.1/abcli/.abcli/plugins/seed.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/session.sh` & `abcli-9.63.1/abcli/.abcli/plugins/session.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/ssh.sh` & `abcli-9.63.1/abcli/.abcli/plugins/ssh.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/storage.sh` & `abcli-9.63.1/abcli/.abcli/plugins/storage.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/tags.sh` & `abcli-9.63.1/abcli/.abcli/plugins/tags.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/terminal.sh` & `abcli-9.63.1/abcli/.abcli/plugins/terminal.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/test.sh` & `abcli-9.63.1/abcli/.abcli/plugins/test.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/watch.sh` & `abcli-9.63.1/abcli/.abcli/plugins/watch.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/plugins/wifi.sh` & `abcli-9.63.1/abcli/.abcli/plugins/wifi.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/tests/abcli_clarify_object.sh` & `abcli-9.63.1/abcli/.abcli/tests/abcli_clarify_object.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/tests/keyword.sh` & `abcli-9.63.1/abcli/.abcli/tests/keyword.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/tests/list_functions.sh` & `abcli-9.63.1/abcli/.abcli/tests/list_functions.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/tests/metadata.sh` & `abcli-9.63.1/abcli/.abcli/tests/metadata.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/tests/options.sh` & `abcli-9.63.1/abcli/.abcli/tests/options.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/.abcli/tests/plugins.sh` & `abcli-9.63.1/abcli/.abcli/tests/plugins.sh`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/bash/help.py` & `abcli-9.63.1/abcli/bash/help.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/bash/list.py` & `abcli-9.63.1/abcli/bash/list.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/bash/logging.py` & `abcli-9.63.1/abcli/bash/logging.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/config.env` & `abcli-9.63.1/abcli/config.env`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/elapsed_timer.py` & `abcli-9.63.1/abcli/elapsed_timer.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/env.py` & `abcli-9.63.1/abcli/env.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/file/__main__.py` & `abcli-9.63.1/abcli/file/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/file/classes.py` & `abcli-9.63.1/abcli/file/classes.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/file/functions.py` & `abcli-9.63.1/abcli/file/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/file/load.py` & `abcli-9.63.1/abcli/file/load.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/file/save.py` & `abcli-9.63.1/abcli/file/save.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/keywords/__main__.py` & `abcli-9.63.1/abcli/keywords/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/keywords/keywords.py` & `abcli-9.63.1/abcli/keywords/keywords.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/logger.py` & `abcli-9.63.1/abcli/logger.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/modules/host/__main__.py` & `abcli-9.63.1/abcli/modules/host/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/modules/host/functions.py` & `abcli-9.63.1/abcli/modules/host/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/modules/objects.py` & `abcli-9.63.1/abcli/modules/objects.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/options/__main__.py` & `abcli-9.63.1/abcli/options/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/options/classes.py` & `abcli-9.63.1/abcli/options/classes.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/path/functions.py` & `abcli-9.63.1/abcli/path/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/plugins/__main__.py` & `abcli-9.63.1/abcli/plugins/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/plugins/cache/__main__.py` & `abcli-9.63.1/abcli/plugins/cache/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/plugins/cache/functions.py` & `abcli-9.63.1/abcli/plugins/cache/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/plugins/functions.py` & `abcli-9.63.1/abcli/plugins/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/plugins/git/__main__.py` & `abcli-9.63.1/abcli/plugins/git/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/plugins/git/version.py` & `abcli-9.63.1/abcli/plugins/git/version.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/plugins/gpu/functions.py` & `abcli-9.63.1/abcli/plugins/gpu/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/plugins/graphics/constants.py` & `abcli-9.63.1/abcli/plugins/graphics/constants.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/plugins/graphics/gif.py` & `abcli-9.63.1/abcli/plugins/graphics/gif.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/plugins/graphics/signature.py` & `abcli-9.63.1/abcli/plugins/graphics/signature.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/plugins/graphics/text.py` & `abcli-9.63.1/abcli/plugins/graphics/text.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/plugins/markdown.py` & `abcli-9.63.1/abcli/plugins/markdown.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/plugins/metadata/__main__.py` & `abcli-9.63.1/abcli/plugins/metadata/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/plugins/metadata/functions.py` & `abcli-9.63.1/abcli/plugins/metadata/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/plugins/relations/__main__.py` & `abcli-9.63.1/abcli/plugins/relations/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/plugins/relations/functions.py` & `abcli-9.63.1/abcli/plugins/relations/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/plugins/seed.py` & `abcli-9.63.1/abcli/plugins/seed.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/plugins/storage/__main__.py` & `abcli-9.63.1/abcli/plugins/storage/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/plugins/storage/classes.py` & `abcli-9.63.1/abcli/plugins/storage/classes.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/plugins/tags/__main__.py` & `abcli-9.63.1/abcli/plugins/tags/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/plugins/tags/functions.py` & `abcli-9.63.1/abcli/plugins/tags/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/plugins/video.py` & `abcli-9.63.1/abcli/plugins/video.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/string/__main__.py` & `abcli-9.63.1/abcli/string/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/string/functions.py` & `abcli-9.63.1/abcli/string/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/table/classes.py` & `abcli-9.63.1/abcli/table/classes.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/tests/test_options.py` & `abcli-9.63.1/abcli/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/tests/test_plugins.py` & `abcli-9.63.1/abcli/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/tests/test_plugins_graphics_gif_generate_animated_gif.py` & `abcli-9.63.1/abcli/tests/test_plugins_graphics_gif_generate_animated_gif.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/tests/test_plugins_graphics_signature.py` & `abcli-9.63.1/abcli/tests/test_plugins_graphics_signature.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/tests/test_plugins_metadata.py` & `abcli-9.63.1/abcli/tests/test_plugins_metadata.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/tests/test_plugins_testing.py` & `abcli-9.63.1/abcli/tests/test_plugins_testing.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli/timer.py` & `abcli-9.63.1/abcli/timer.py`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/abcli.egg-info/PKG-INFO` & `abcli-9.63.1/abcli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abcli
-Version: 9.62.1
+Version: 9.63.1
 Summary: 🚀 a language to speak AI.
 Home-page: https://github.com/kamangir/awesome-bash-cli
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
@@ -23,20 +23,20 @@
 Requires-Dist: pylint
 Requires-Dist: pytest
 Requires-Dist: python-dotenv[cli]
 Requires-Dist: tqdm
 
 # awesome bash cli (abcli/abc)
 
+`abcli` 🚀 is an implementation of [🔻 giza](https://github.com/kamangir/giza) and the library behind [these projects](https://github.com/kamangir/kamangir).
+
 ![image](https://raw.githubusercontent.com/kamangir/awesome-bash-cli/current/abcli/assets/marquee.png)
 
 [![PyPI version](https://img.shields.io/pypi/v/abcli.svg)](https://pypi.org/project/abcli/)
 
-`abcli` 🚀 is an implementation of [🔻 giza](https://github.com/kamangir/giza) and the library behind [these projects](https://github.com/kamangir/kamangir).
-
 To install `abcli`, type in,
 
 ```bash
 pip install abcli
 ```
 
 or follow these (not-too-update) instructions for custom environments:
```

### Comparing `abcli-9.62.1/abcli.egg-info/SOURCES.txt` & `abcli-9.63.1/abcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `abcli-9.62.1/setup.py` & `abcli-9.63.1/setup.py`

 * *Files identical despite different names*

