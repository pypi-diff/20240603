# Comparing `tmp/hebill-3.0.0.tar.gz` & `tmp/hebill-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hebill-3.0.0.tar", last modified: Mon Jun  3 08:03:13 2024, max compression
+gzip compressed data, was "hebill-3.1.0.tar", last modified: Mon Jun  3 08:25:35 2024, max compression
```

## Comparing `hebill-3.0.0.tar` & `hebill-3.1.0.tar`

### file list

```diff
@@ -1,249 +1,258 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.147227 hebill-3.0.0/
--rw-rw-rw-   0        0        0      347 2024-06-03 08:03:13.146187 hebill-3.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:12.943859 hebill-3.0.0/hebill/
--rw-rw-rw-   0        0        0      300 2024-06-03 08:03:12.000000 hebill-3.0.0/hebill/__constants__.py
--rw-rw-rw-   0        0        0       30 2024-06-01 07:48:37.000000 hebill-3.0.0/hebill/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:12.951282 hebill-3.0.0/hebill/digital/
--rw-rw-rw-   0        0        0       27 2024-06-01 08:59:10.000000 hebill-3.0.0/hebill/digital/__init__.py
--rw-rw-rw-   0        0        0     1143 2024-06-03 07:01:14.000000 hebill-3.0.0/hebill/digital/constants.py
--rw-rw-rw-   0        0        0    13401 2024-06-03 07:32:05.000000 hebill-3.0.0/hebill/digital/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:12.954436 hebill-3.0.0/hebill/html/
--rw-rw-rw-   0        0        0      164 2024-06-01 07:41:05.000000 hebill-3.0.0/hebill/html/README.MD
--rw-rw-rw-   0        0        0       25 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/__constants__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:12.955739 hebill-3.0.0/hebill/html/__extensions__/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/__extensions__/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:12.958104 hebill-3.0.0/hebill/html/__extensions__/toggle/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/__extensions__/toggle/__init__.py
--rw-rw-rw-   0        0        0      804 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/__extensions__/toggle/core.py
--rw-rw-rw-   0        0        0      125 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:12.959255 hebill-3.0.0/hebill/html/__templates__/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/__templates__/__init__.py
--rw-rw-rw-   0        0        0      516 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/__templates__/styles.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:12.960565 hebill-3.0.0/hebill/html/components/
--rw-rw-rw-   0        0        0      245 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:12.965839 hebill-3.0.0/hebill/html/components/__utilities__/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/__utilities__/__init__.py
--rw-rw-rw-   0        0        0     3585 2024-06-01 07:41:05.000000 hebill-3.0.0/hebill/html/components/__utilities__/align.py
--rw-rw-rw-   0        0        0     3375 2024-06-01 07:41:05.000000 hebill-3.0.0/hebill/html/components/__utilities__/align_self.py
--rw-rw-rw-   0        0        0     2567 2024-06-01 07:41:05.000000 hebill-3.0.0/hebill/html/components/__utilities__/direction.py
--rw-rw-rw-   0        0        0      659 2024-06-01 07:41:05.000000 hebill-3.0.0/hebill/html/components/__utilities__/fill.py
--rw-rw-rw-   0        0        0     1211 2024-06-01 07:41:05.000000 hebill-3.0.0/hebill/html/components/__utilities__/flex.py
--rw-rw-rw-   0        0        0     4673 2024-06-01 07:41:05.000000 hebill-3.0.0/hebill/html/components/__utilities__/justify.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:12.968840 hebill-3.0.0/hebill/html/components/alert/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/alert/__init__.py
--rw-rw-rw-   0        0        0      874 2024-06-01 07:41:05.000000 hebill-3.0.0/hebill/html/components/alert/color.py
--rw-rw-rw-   0        0        0      394 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/alert/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:12.970838 hebill-3.0.0/hebill/html/components/breadcrumb/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/breadcrumb/__init__.py
--rw-rw-rw-   0        0        0      790 2024-06-01 07:41:05.000000 hebill-3.0.0/hebill/html/components/breadcrumb/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:12.974923 hebill-3.0.0/hebill/html/components/button/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/button/__init__.py
--rw-rw-rw-   0        0        0      842 2024-06-01 07:41:05.000000 hebill-3.0.0/hebill/html/components/button/color.py
--rw-rw-rw-   0        0        0      970 2024-06-01 07:41:04.000000 hebill-3.0.0/hebill/html/components/button/color_outline.py
--rw-rw-rw-   0        0        0      866 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/button/core.py
--rw-rw-rw-   0        0        0      304 2024-06-01 07:41:05.000000 hebill-3.0.0/hebill/html/components/button/size.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:12.977898 hebill-3.0.0/hebill/html/components/container/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/container/__init__.py
--rw-rw-rw-   0        0        0      375 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/container/core.py
--rw-rw-rw-   0        0        0      845 2024-06-01 07:41:05.000000 hebill-3.0.0/hebill/html/components/container/size.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:12.979599 hebill-3.0.0/hebill/html/components/html/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/html/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:12.981867 hebill-3.0.0/hebill/html/components/html/body/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/html/body/__init__.py
--rw-rw-rw-   0        0        0      977 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/html/body/core.py
--rw-rw-rw-   0        0        0     2822 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/html/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:12.983057 hebill-3.0.0/hebill/html/components/html/head/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/html/head/__init__.py
--rw-rw-rw-   0        0        0      660 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/html/head/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:12.985193 hebill-3.0.0/hebill/html/components/html/head/title/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/html/head/title/__init__.py
--rw-rw-rw-   0        0        0      106 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/html/head/title/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:12.987294 hebill-3.0.0/hebill/html/components/html/libraries/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/html/libraries/__init__.py
--rw-rw-rw-   0        0        0      448 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/html/libraries/libraries.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:12.988356 hebill-3.0.0/hebill/html/components/navbar/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/navbar/__init__.py
--rw-rw-rw-   0        0        0      777 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/navbar/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:12.990582 hebill-3.0.0/hebill/html/components/navbar/menus/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/navbar/menus/__init__.py
--rw-rw-rw-   0        0        0      350 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/navbar/menus/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:12.993235 hebill-3.0.0/hebill/html/components/pagination/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/pagination/__init__.py
--rw-rw-rw-   0        0        0      857 2024-06-01 07:41:04.000000 hebill-3.0.0/hebill/html/components/pagination/core.py
--rw-rw-rw-   0        0        0      332 2024-06-01 07:41:05.000000 hebill-3.0.0/hebill/html/components/pagination/size.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:12.995355 hebill-3.0.0/hebill/html/components/table/
--rw-rw-rw-   0        0        0      190 2024-06-01 07:41:05.000000 hebill-3.0.0/hebill/html/components/table/README.MD
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/table/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:12.997307 hebill-3.0.0/hebill/html/components/table/__templates__/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/table/__templates__/__init__.py
--rw-rw-rw-   0        0        0      875 2024-06-01 07:41:05.000000 hebill-3.0.0/hebill/html/components/table/__templates__/color.py
--rw-rw-rw-   0        0        0     2402 2024-06-01 07:41:05.000000 hebill-3.0.0/hebill/html/components/table/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:12.999352 hebill-3.0.0/hebill/html/components/table/tbody/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/table/tbody/__init__.py
--rw-rw-rw-   0        0        0     1079 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/table/tbody/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.000352 hebill-3.0.0/hebill/html/components/table/tbody/tr/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/table/tbody/tr/__init__.py
--rw-rw-rw-   0        0        0      896 2024-06-01 07:41:04.000000 hebill-3.0.0/hebill/html/components/table/tbody/tr/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.002422 hebill-3.0.0/hebill/html/components/table/tbody/tr/td/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/table/tbody/tr/td/__init__.py
--rw-rw-rw-   0        0        0      165 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/table/tbody/tr/td/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.004430 hebill-3.0.0/hebill/html/components/table/thead/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/table/thead/__init__.py
--rw-rw-rw-   0        0        0     1079 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/table/thead/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.005627 hebill-3.0.0/hebill/html/components/table/thead/tr/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/table/thead/tr/__init__.py
--rw-rw-rw-   0        0        0      889 2024-06-01 07:41:04.000000 hebill-3.0.0/hebill/html/components/table/thead/tr/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.007863 hebill-3.0.0/hebill/html/components/table/thead/tr/th/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/table/thead/tr/th/__init__.py
--rw-rw-rw-   0        0        0      165 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/components/table/thead/tr/th/core.py
--rw-rw-rw-   0        0        0      966 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.008864 hebill-3.0.0/hebill/html/nodes/
--rw-rw-rw-   0        0        0      186 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/nodes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.012174 hebill-3.0.0/hebill/html/nodes/code/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/nodes/code/__init__.py
--rw-rw-rw-   0        0        0      271 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/nodes/code/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.013794 hebill-3.0.0/hebill/html/nodes/comment/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/nodes/comment/__init__.py
--rw-rw-rw-   0        0        0      512 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/nodes/comment/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.015871 hebill-3.0.0/hebill/html/nodes/content/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/nodes/content/__init__.py
--rw-rw-rw-   0        0        0      497 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/nodes/content/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.017996 hebill-3.0.0/hebill/html/nodes/group/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/nodes/group/__init__.py
--rw-rw-rw-   0        0        0     1242 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/nodes/group/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.020950 hebill-3.0.0/hebill/html/nodes/group/create/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/nodes/group/create/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.023487 hebill-3.0.0/hebill/html/nodes/group/create/components/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/nodes/group/create/components/__init__.py
--rw-rw-rw-   0        0        0      757 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/nodes/group/create/components/core.py
--rw-rw-rw-   0        0        0      752 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/nodes/group/create/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.025591 hebill-3.0.0/hebill/html/nodes/group/create/nodes/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/nodes/group/create/nodes/__init__.py
--rw-rw-rw-   0        0        0      648 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/nodes/group/create/nodes/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.028827 hebill-3.0.0/hebill/html/nodes/group/create/tags/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/nodes/group/create/tags/__init__.py
--rw-rw-rw-   0        0        0     3097 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/nodes/group/create/tags/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.030831 hebill-3.0.0/hebill/html/nodes/node/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/nodes/node/__init__.py
--rw-rw-rw-   0        0        0     1222 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/nodes/node/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.033348 hebill-3.0.0/hebill/html/nodes/tag/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/nodes/tag/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.036560 hebill-3.0.0/hebill/html/nodes/tag/attributes/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/nodes/tag/attributes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.039137 hebill-3.0.0/hebill/html/nodes/tag/attributes/classes/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/nodes/tag/attributes/classes/__init__.py
--rw-rw-rw-   0        0        0     1264 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/nodes/tag/attributes/classes/core.py
--rw-rw-rw-   0        0        0     1959 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/nodes/tag/attributes/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.041643 hebill-3.0.0/hebill/html/nodes/tag/attributes/styles/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/nodes/tag/attributes/styles/__init__.py
--rw-rw-rw-   0        0        0     1100 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/nodes/tag/attributes/styles/core.py
--rw-rw-rw-   0        0        0     1223 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/nodes/tag/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.043058 hebill-3.0.0/hebill/html/tags/
--rw-rw-rw-   0        0        0      781 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.045116 hebill-3.0.0/hebill/html/tags/a/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/a/__init__.py
--rw-rw-rw-   0        0        0      268 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/a/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.047273 hebill-3.0.0/hebill/html/tags/body/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/body/__init__.py
--rw-rw-rw-   0        0        0      165 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/body/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.049196 hebill-3.0.0/hebill/html/tags/button/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/button/__init__.py
--rw-rw-rw-   0        0        0      227 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/button/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.051719 hebill-3.0.0/hebill/html/tags/div/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/div/__init__.py
--rw-rw-rw-   0        0        0      221 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/div/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.054718 hebill-3.0.0/hebill/html/tags/h1/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/h1/__init__.py
--rw-rw-rw-   0        0        0      161 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/h1/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.059776 hebill-3.0.0/hebill/html/tags/h2/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/h2/__init__.py
--rw-rw-rw-   0        0        0      161 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/h2/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.064100 hebill-3.0.0/hebill/html/tags/h3/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/h3/__init__.py
--rw-rw-rw-   0        0        0      161 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/h3/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.067118 hebill-3.0.0/hebill/html/tags/h4/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/h4/__init__.py
--rw-rw-rw-   0        0        0      161 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/h4/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.071736 hebill-3.0.0/hebill/html/tags/h5/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/h5/__init__.py
--rw-rw-rw-   0        0        0      161 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/h5/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.074686 hebill-3.0.0/hebill/html/tags/h6/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/h6/__init__.py
--rw-rw-rw-   0        0        0      161 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/h6/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.077905 hebill-3.0.0/hebill/html/tags/head/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/head/__init__.py
--rw-rw-rw-   0        0        0      123 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/head/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.079413 hebill-3.0.0/hebill/html/tags/html/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/html/__init__.py
--rw-rw-rw-   0        0        0      303 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/html/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.081422 hebill-3.0.0/hebill/html/tags/input_text/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/input_text/__init__.py
--rw-rw-rw-   0        0        0      487 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/input_text/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.083423 hebill-3.0.0/hebill/html/tags/li/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/li/__init__.py
--rw-rw-rw-   0        0        0      161 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/li/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.087312 hebill-3.0.0/hebill/html/tags/link/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/link/__init__.py
--rw-rw-rw-   0        0        0      212 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/link/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.088963 hebill-3.0.0/hebill/html/tags/meta/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/meta/__init__.py
--rw-rw-rw-   0        0        0      432 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/meta/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.091468 hebill-3.0.0/hebill/html/tags/nav/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/nav/__init__.py
--rw-rw-rw-   0        0        0      121 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/nav/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.093990 hebill-3.0.0/hebill/html/tags/ol/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/ol/__init__.py
--rw-rw-rw-   0        0        0      119 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/ol/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.097003 hebill-3.0.0/hebill/html/tags/script/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/script/__init__.py
--rw-rw-rw-   0        0        0      215 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/script/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.099521 hebill-3.0.0/hebill/html/tags/span/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/span/__init__.py
--rw-rw-rw-   0        0        0      223 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/span/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.101524 hebill-3.0.0/hebill/html/tags/table/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/table/__init__.py
--rw-rw-rw-   0        0        0      125 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/table/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.103549 hebill-3.0.0/hebill/html/tags/tbody/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/tbody/__init__.py
--rw-rw-rw-   0        0        0      125 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/tbody/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.106074 hebill-3.0.0/hebill/html/tags/td/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/td/__init__.py
--rw-rw-rw-   0        0        0      169 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/td/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.108160 hebill-3.0.0/hebill/html/tags/th/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/th/__init__.py
--rw-rw-rw-   0        0        0      169 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/th/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.111219 hebill-3.0.0/hebill/html/tags/thead/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/thead/__init__.py
--rw-rw-rw-   0        0        0      125 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/thead/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.113319 hebill-3.0.0/hebill/html/tags/title/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/title/__init__.py
--rw-rw-rw-   0        0        0      437 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/title/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.117049 hebill-3.0.0/hebill/html/tags/tr/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/tr/__init__.py
--rw-rw-rw-   0        0        0      127 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/tr/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.125173 hebill-3.0.0/hebill/html/tags/ul/
--rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/ul/__init__.py
--rw-rw-rw-   0        0        0      119 2024-05-27 03:13:03.000000 hebill-3.0.0/hebill/html/tags/ul/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.133465 hebill-3.0.0/hebill/pypi/
--rw-rw-rw-   0        0        0     1410 2024-06-01 06:46:51.000000 hebill-3.0.0/hebill/pypi/README.MD
--rw-rw-rw-   0        0        0       25 2024-06-01 06:46:51.000000 hebill-3.0.0/hebill/pypi/__constants__.py
--rw-rw-rw-   0        0        0       24 2024-06-01 06:46:51.000000 hebill-3.0.0/hebill/pypi/__init__.py
--rw-rw-rw-   0        0        0     9694 2024-06-03 07:58:58.000000 hebill-3.0.0/hebill/pypi/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.138734 hebill-3.0.0/hebill/string/
--rw-rw-rw-   0        0        0       67 2024-06-01 08:59:10.000000 hebill-3.0.0/hebill/string/__init__.py
--rw-rw-rw-   0        0        0     1000 2024-06-03 07:22:41.000000 hebill-3.0.0/hebill/string/core.py
--rw-rw-rw-   0        0        0      377 2024-06-01 08:56:44.000000 hebill-3.0.0/hebill/string/string_random.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.143867 hebill-3.0.0/hebill/terminal/
--rw-rw-rw-   0        0        0       28 2024-06-01 06:46:51.000000 hebill-3.0.0/hebill/terminal/__init__.py
--rw-rw-rw-   0        0        0     1618 2024-06-01 06:46:51.000000 hebill-3.0.0/hebill/terminal/color.py
--rw-rw-rw-   0        0        0      134 2024-06-03 07:13:46.000000 hebill-3.0.0/hebill/terminal/color_back.py
--rw-rw-rw-   0        0        0      142 2024-06-03 07:13:46.000000 hebill-3.0.0/hebill/terminal/color_fore.py
--rw-rw-rw-   0        0        0     1002 2024-06-03 07:17:01.000000 hebill-3.0.0/hebill/terminal/core.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:03:13.144908 hebill-3.0.0/hebill.egg-info/
--rw-rw-rw-   0        0        0      347 2024-06-03 08:03:12.000000 hebill-3.0.0/hebill.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6239 2024-06-03 08:03:12.000000 hebill-3.0.0/hebill.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 08:03:12.000000 hebill-3.0.0/hebill.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-06-03 08:03:12.000000 hebill-3.0.0/hebill.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-06-03 08:03:12.000000 hebill-3.0.0/hebill.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      462 2024-06-03 08:03:12.000000 hebill-3.0.0/pack_upload_setup.py
--rw-rw-rw-   0        0        0       42 2024-06-03 08:03:13.147527 hebill-3.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.919229 hebill-3.1.0/
+-rw-rw-rw-   0        0        0      359 2024-06-03 08:25:35.918236 hebill-3.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.749649 hebill-3.1.0/hebill/
+-rw-rw-rw-   0        0        0      300 2024-06-03 08:25:35.000000 hebill-3.1.0/hebill/__constants__.py
+-rw-rw-rw-   0        0        0       30 2024-06-01 07:48:37.000000 hebill-3.1.0/hebill/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.758127 hebill-3.1.0/hebill/digital/
+-rw-rw-rw-   0        0        0       27 2024-06-01 08:59:10.000000 hebill-3.1.0/hebill/digital/__init__.py
+-rw-rw-rw-   0        0        0     1143 2024-06-03 07:01:14.000000 hebill-3.1.0/hebill/digital/constants.py
+-rw-rw-rw-   0        0        0    13401 2024-06-03 07:32:05.000000 hebill-3.1.0/hebill/digital/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.763068 hebill-3.1.0/hebill/html/
+-rw-rw-rw-   0        0        0      164 2024-06-01 07:41:05.000000 hebill-3.1.0/hebill/html/README.MD
+-rw-rw-rw-   0        0        0       25 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/__constants__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.764220 hebill-3.1.0/hebill/html/__extensions__/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/__extensions__/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.766454 hebill-3.1.0/hebill/html/__extensions__/toggle/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/__extensions__/toggle/__init__.py
+-rw-rw-rw-   0        0        0      804 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/__extensions__/toggle/core.py
+-rw-rw-rw-   0        0        0      125 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.768462 hebill-3.1.0/hebill/html/__templates__/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/__templates__/__init__.py
+-rw-rw-rw-   0        0        0      516 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/__templates__/styles.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.770472 hebill-3.1.0/hebill/html/components/
+-rw-rw-rw-   0        0        0      245 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.777123 hebill-3.1.0/hebill/html/components/__utilities__/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/__utilities__/__init__.py
+-rw-rw-rw-   0        0        0     3585 2024-06-01 07:41:05.000000 hebill-3.1.0/hebill/html/components/__utilities__/align.py
+-rw-rw-rw-   0        0        0     3375 2024-06-01 07:41:05.000000 hebill-3.1.0/hebill/html/components/__utilities__/align_self.py
+-rw-rw-rw-   0        0        0     2567 2024-06-01 07:41:05.000000 hebill-3.1.0/hebill/html/components/__utilities__/direction.py
+-rw-rw-rw-   0        0        0      659 2024-06-01 07:41:05.000000 hebill-3.1.0/hebill/html/components/__utilities__/fill.py
+-rw-rw-rw-   0        0        0     1211 2024-06-01 07:41:05.000000 hebill-3.1.0/hebill/html/components/__utilities__/flex.py
+-rw-rw-rw-   0        0        0     4673 2024-06-01 07:41:05.000000 hebill-3.1.0/hebill/html/components/__utilities__/justify.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.779552 hebill-3.1.0/hebill/html/components/alert/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/alert/__init__.py
+-rw-rw-rw-   0        0        0      874 2024-06-01 07:41:05.000000 hebill-3.1.0/hebill/html/components/alert/color.py
+-rw-rw-rw-   0        0        0      394 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/alert/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.781358 hebill-3.1.0/hebill/html/components/breadcrumb/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/breadcrumb/__init__.py
+-rw-rw-rw-   0        0        0      790 2024-06-01 07:41:05.000000 hebill-3.1.0/hebill/html/components/breadcrumb/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.785830 hebill-3.1.0/hebill/html/components/button/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/button/__init__.py
+-rw-rw-rw-   0        0        0      842 2024-06-01 07:41:05.000000 hebill-3.1.0/hebill/html/components/button/color.py
+-rw-rw-rw-   0        0        0      970 2024-06-01 07:41:04.000000 hebill-3.1.0/hebill/html/components/button/color_outline.py
+-rw-rw-rw-   0        0        0      866 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/button/core.py
+-rw-rw-rw-   0        0        0      304 2024-06-01 07:41:05.000000 hebill-3.1.0/hebill/html/components/button/size.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.788629 hebill-3.1.0/hebill/html/components/container/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/container/__init__.py
+-rw-rw-rw-   0        0        0      375 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/container/core.py
+-rw-rw-rw-   0        0        0      845 2024-06-01 07:41:05.000000 hebill-3.1.0/hebill/html/components/container/size.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.789931 hebill-3.1.0/hebill/html/components/html/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/html/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.792546 hebill-3.1.0/hebill/html/components/html/body/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/html/body/__init__.py
+-rw-rw-rw-   0        0        0      977 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/html/body/core.py
+-rw-rw-rw-   0        0        0     2822 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/html/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.793576 hebill-3.1.0/hebill/html/components/html/head/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/html/head/__init__.py
+-rw-rw-rw-   0        0        0      660 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/html/head/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.796029 hebill-3.1.0/hebill/html/components/html/head/title/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/html/head/title/__init__.py
+-rw-rw-rw-   0        0        0      106 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/html/head/title/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.797121 hebill-3.1.0/hebill/html/components/html/libraries/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/html/libraries/__init__.py
+-rw-rw-rw-   0        0        0      448 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/html/libraries/libraries.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.799135 hebill-3.1.0/hebill/html/components/navbar/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/navbar/__init__.py
+-rw-rw-rw-   0        0        0      777 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/navbar/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.801287 hebill-3.1.0/hebill/html/components/navbar/menus/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/navbar/menus/__init__.py
+-rw-rw-rw-   0        0        0      350 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/navbar/menus/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.803731 hebill-3.1.0/hebill/html/components/pagination/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/pagination/__init__.py
+-rw-rw-rw-   0        0        0      857 2024-06-01 07:41:04.000000 hebill-3.1.0/hebill/html/components/pagination/core.py
+-rw-rw-rw-   0        0        0      332 2024-06-01 07:41:05.000000 hebill-3.1.0/hebill/html/components/pagination/size.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.807268 hebill-3.1.0/hebill/html/components/table/
+-rw-rw-rw-   0        0        0      190 2024-06-01 07:41:05.000000 hebill-3.1.0/hebill/html/components/table/README.MD
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/table/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.808297 hebill-3.1.0/hebill/html/components/table/__templates__/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/table/__templates__/__init__.py
+-rw-rw-rw-   0        0        0      875 2024-06-01 07:41:05.000000 hebill-3.1.0/hebill/html/components/table/__templates__/color.py
+-rw-rw-rw-   0        0        0     2402 2024-06-01 07:41:05.000000 hebill-3.1.0/hebill/html/components/table/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.810529 hebill-3.1.0/hebill/html/components/table/tbody/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/table/tbody/__init__.py
+-rw-rw-rw-   0        0        0     1079 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/table/tbody/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.812194 hebill-3.1.0/hebill/html/components/table/tbody/tr/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/table/tbody/tr/__init__.py
+-rw-rw-rw-   0        0        0      896 2024-06-01 07:41:04.000000 hebill-3.1.0/hebill/html/components/table/tbody/tr/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.814244 hebill-3.1.0/hebill/html/components/table/tbody/tr/td/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/table/tbody/tr/td/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/table/tbody/tr/td/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.816245 hebill-3.1.0/hebill/html/components/table/thead/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/table/thead/__init__.py
+-rw-rw-rw-   0        0        0     1079 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/table/thead/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.817766 hebill-3.1.0/hebill/html/components/table/thead/tr/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/table/thead/tr/__init__.py
+-rw-rw-rw-   0        0        0      889 2024-06-01 07:41:04.000000 hebill-3.1.0/hebill/html/components/table/thead/tr/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.819880 hebill-3.1.0/hebill/html/components/table/thead/tr/th/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/table/thead/tr/th/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/components/table/thead/tr/th/core.py
+-rw-rw-rw-   0        0        0      966 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.821056 hebill-3.1.0/hebill/html/nodes/
+-rw-rw-rw-   0        0        0      186 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/nodes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.823075 hebill-3.1.0/hebill/html/nodes/code/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/nodes/code/__init__.py
+-rw-rw-rw-   0        0        0      271 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/nodes/code/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.824072 hebill-3.1.0/hebill/html/nodes/comment/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/nodes/comment/__init__.py
+-rw-rw-rw-   0        0        0      512 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/nodes/comment/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.826064 hebill-3.1.0/hebill/html/nodes/content/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/nodes/content/__init__.py
+-rw-rw-rw-   0        0        0      497 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/nodes/content/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.827585 hebill-3.1.0/hebill/html/nodes/group/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/nodes/group/__init__.py
+-rw-rw-rw-   0        0        0     1242 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/nodes/group/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.829835 hebill-3.1.0/hebill/html/nodes/group/create/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/nodes/group/create/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.830845 hebill-3.1.0/hebill/html/nodes/group/create/components/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/nodes/group/create/components/__init__.py
+-rw-rw-rw-   0        0        0      757 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/nodes/group/create/components/core.py
+-rw-rw-rw-   0        0        0      752 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/nodes/group/create/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.833465 hebill-3.1.0/hebill/html/nodes/group/create/nodes/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/nodes/group/create/nodes/__init__.py
+-rw-rw-rw-   0        0        0      648 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/nodes/group/create/nodes/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.835663 hebill-3.1.0/hebill/html/nodes/group/create/tags/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/nodes/group/create/tags/__init__.py
+-rw-rw-rw-   0        0        0     3097 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/nodes/group/create/tags/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.837663 hebill-3.1.0/hebill/html/nodes/node/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/nodes/node/__init__.py
+-rw-rw-rw-   0        0        0     1222 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/nodes/node/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.839667 hebill-3.1.0/hebill/html/nodes/tag/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/nodes/tag/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.841128 hebill-3.1.0/hebill/html/nodes/tag/attributes/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/nodes/tag/attributes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.843659 hebill-3.1.0/hebill/html/nodes/tag/attributes/classes/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/nodes/tag/attributes/classes/__init__.py
+-rw-rw-rw-   0        0        0     1264 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/nodes/tag/attributes/classes/core.py
+-rw-rw-rw-   0        0        0     1959 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/nodes/tag/attributes/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.845242 hebill-3.1.0/hebill/html/nodes/tag/attributes/styles/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/nodes/tag/attributes/styles/__init__.py
+-rw-rw-rw-   0        0        0     1100 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/nodes/tag/attributes/styles/core.py
+-rw-rw-rw-   0        0        0     1223 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/nodes/tag/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.846179 hebill-3.1.0/hebill/html/tags/
+-rw-rw-rw-   0        0        0      781 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.848185 hebill-3.1.0/hebill/html/tags/a/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/a/__init__.py
+-rw-rw-rw-   0        0        0      268 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/a/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.850195 hebill-3.1.0/hebill/html/tags/body/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/body/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/body/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.852408 hebill-3.1.0/hebill/html/tags/button/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/button/__init__.py
+-rw-rw-rw-   0        0        0      227 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/button/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.853839 hebill-3.1.0/hebill/html/tags/div/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/div/__init__.py
+-rw-rw-rw-   0        0        0      221 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/div/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.855359 hebill-3.1.0/hebill/html/tags/h1/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/h1/__init__.py
+-rw-rw-rw-   0        0        0      161 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/h1/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.857852 hebill-3.1.0/hebill/html/tags/h2/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/h2/__init__.py
+-rw-rw-rw-   0        0        0      161 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/h2/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.858976 hebill-3.1.0/hebill/html/tags/h3/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/h3/__init__.py
+-rw-rw-rw-   0        0        0      161 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/h3/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.860985 hebill-3.1.0/hebill/html/tags/h4/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/h4/__init__.py
+-rw-rw-rw-   0        0        0      161 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/h4/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.862501 hebill-3.1.0/hebill/html/tags/h5/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/h5/__init__.py
+-rw-rw-rw-   0        0        0      161 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/h5/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.864610 hebill-3.1.0/hebill/html/tags/h6/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/h6/__init__.py
+-rw-rw-rw-   0        0        0      161 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/h6/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.867158 hebill-3.1.0/hebill/html/tags/head/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/head/__init__.py
+-rw-rw-rw-   0        0        0      123 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/head/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.869171 hebill-3.1.0/hebill/html/tags/html/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/html/__init__.py
+-rw-rw-rw-   0        0        0      303 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/html/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.871282 hebill-3.1.0/hebill/html/tags/input_text/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/input_text/__init__.py
+-rw-rw-rw-   0        0        0      487 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/input_text/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.873722 hebill-3.1.0/hebill/html/tags/li/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/li/__init__.py
+-rw-rw-rw-   0        0        0      161 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/li/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.874745 hebill-3.1.0/hebill/html/tags/link/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/link/__init__.py
+-rw-rw-rw-   0        0        0      212 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/link/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.877070 hebill-3.1.0/hebill/html/tags/meta/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/meta/__init__.py
+-rw-rw-rw-   0        0        0      432 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/meta/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.879113 hebill-3.1.0/hebill/html/tags/nav/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/nav/__init__.py
+-rw-rw-rw-   0        0        0      121 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/nav/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.881625 hebill-3.1.0/hebill/html/tags/ol/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/ol/__init__.py
+-rw-rw-rw-   0        0        0      119 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/ol/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.882647 hebill-3.1.0/hebill/html/tags/script/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/script/__init__.py
+-rw-rw-rw-   0        0        0      215 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/script/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.885146 hebill-3.1.0/hebill/html/tags/span/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/span/__init__.py
+-rw-rw-rw-   0        0        0      223 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/span/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.886659 hebill-3.1.0/hebill/html/tags/table/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/table/__init__.py
+-rw-rw-rw-   0        0        0      125 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/table/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.888666 hebill-3.1.0/hebill/html/tags/tbody/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/tbody/__init__.py
+-rw-rw-rw-   0        0        0      125 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/tbody/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.890956 hebill-3.1.0/hebill/html/tags/td/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/td/__init__.py
+-rw-rw-rw-   0        0        0      169 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/td/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.891969 hebill-3.1.0/hebill/html/tags/th/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/th/__init__.py
+-rw-rw-rw-   0        0        0      169 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/th/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.894041 hebill-3.1.0/hebill/html/tags/thead/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/thead/__init__.py
+-rw-rw-rw-   0        0        0      125 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/thead/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.896371 hebill-3.1.0/hebill/html/tags/title/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/title/__init__.py
+-rw-rw-rw-   0        0        0      437 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/title/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.897399 hebill-3.1.0/hebill/html/tags/tr/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/tr/__init__.py
+-rw-rw-rw-   0        0        0      127 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/tr/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.899231 hebill-3.1.0/hebill/html/tags/ul/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/ul/__init__.py
+-rw-rw-rw-   0        0        0      119 2024-05-27 03:13:03.000000 hebill-3.1.0/hebill/html/tags/ul/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.900238 hebill-3.1.0/hebill/image/
+-rw-rw-rw-   0        0        0      653 2024-06-01 06:46:51.000000 hebill-3.1.0/hebill/image/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.902841 hebill-3.1.0/hebill/image/png/
+-rw-rw-rw-   0        0        0        0 2024-06-01 06:46:51.000000 hebill-3.1.0/hebill/image/png/__init__.py
+-rw-rw-rw-   0        0        0    60832 2024-06-01 06:46:51.000000 hebill-3.1.0/hebill/image/png/constants.py
+-rw-rw-rw-   0        0        0     5804 2024-06-01 06:46:51.000000 hebill-3.1.0/hebill/image/png/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.904887 hebill-3.1.0/hebill/math/
+-rw-rw-rw-   0        0        0       24 2024-06-01 06:46:51.000000 hebill-3.1.0/hebill/math/__init__.py
+-rw-rw-rw-   0        0        0     1707 2024-06-01 06:46:51.000000 hebill-3.1.0/hebill/math/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.908480 hebill-3.1.0/hebill/pypi/
+-rw-rw-rw-   0        0        0     1410 2024-06-01 06:46:51.000000 hebill-3.1.0/hebill/pypi/README.MD
+-rw-rw-rw-   0        0        0       25 2024-06-01 06:46:51.000000 hebill-3.1.0/hebill/pypi/__constants__.py
+-rw-rw-rw-   0        0        0       24 2024-06-01 06:46:51.000000 hebill-3.1.0/hebill/pypi/__init__.py
+-rw-rw-rw-   0        0        0     9694 2024-06-03 07:58:58.000000 hebill-3.1.0/hebill/pypi/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.910659 hebill-3.1.0/hebill/string/
+-rw-rw-rw-   0        0        0       67 2024-06-01 08:59:10.000000 hebill-3.1.0/hebill/string/__init__.py
+-rw-rw-rw-   0        0        0     1000 2024-06-03 07:22:41.000000 hebill-3.1.0/hebill/string/core.py
+-rw-rw-rw-   0        0        0      377 2024-06-01 08:56:44.000000 hebill-3.1.0/hebill/string/string_random.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.915071 hebill-3.1.0/hebill/terminal/
+-rw-rw-rw-   0        0        0       28 2024-06-01 06:46:51.000000 hebill-3.1.0/hebill/terminal/__init__.py
+-rw-rw-rw-   0        0        0     1618 2024-06-01 06:46:51.000000 hebill-3.1.0/hebill/terminal/color.py
+-rw-rw-rw-   0        0        0      134 2024-06-03 07:13:46.000000 hebill-3.1.0/hebill/terminal/color_back.py
+-rw-rw-rw-   0        0        0      142 2024-06-03 07:13:46.000000 hebill-3.1.0/hebill/terminal/color_fore.py
+-rw-rw-rw-   0        0        0     1002 2024-06-03 07:17:01.000000 hebill-3.1.0/hebill/terminal/core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:25:35.917219 hebill-3.1.0/hebill.egg-info/
+-rw-rw-rw-   0        0        0      359 2024-06-03 08:25:35.000000 hebill-3.1.0/hebill.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6392 2024-06-03 08:25:35.000000 hebill-3.1.0/hebill.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 08:25:35.000000 hebill-3.1.0/hebill.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-06-03 08:25:35.000000 hebill-3.1.0/hebill.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-06-03 08:25:35.000000 hebill-3.1.0/hebill.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      543 2024-06-03 08:25:35.000000 hebill-3.1.0/pack_upload_setup.py
+-rw-rw-rw-   0        0        0       42 2024-06-03 08:25:35.919229 hebill-3.1.0/setup.cfg
```

### Comparing `hebill-3.0.0/hebill/digital/constants.py` & `hebill-3.1.0/hebill/digital/constants.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/digital/core.py` & `hebill-3.1.0/hebill/digital/core.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/__extensions__/toggle/core.py` & `hebill-3.1.0/hebill/html/__extensions__/toggle/core.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/__templates__/styles.py` & `hebill-3.1.0/hebill/html/__templates__/styles.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/components/__utilities__/align.py` & `hebill-3.1.0/hebill/html/components/__utilities__/align.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/components/__utilities__/align_self.py` & `hebill-3.1.0/hebill/html/components/__utilities__/align_self.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/components/__utilities__/direction.py` & `hebill-3.1.0/hebill/html/components/__utilities__/direction.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/components/__utilities__/fill.py` & `hebill-3.1.0/hebill/html/components/__utilities__/fill.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/components/__utilities__/flex.py` & `hebill-3.1.0/hebill/html/components/__utilities__/flex.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/components/__utilities__/justify.py` & `hebill-3.1.0/hebill/html/components/__utilities__/justify.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/components/alert/color.py` & `hebill-3.1.0/hebill/html/components/alert/color.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/components/breadcrumb/core.py` & `hebill-3.1.0/hebill/html/components/breadcrumb/core.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/components/button/color.py` & `hebill-3.1.0/hebill/html/components/button/color.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/components/button/color_outline.py` & `hebill-3.1.0/hebill/html/components/button/color_outline.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/components/button/core.py` & `hebill-3.1.0/hebill/html/components/button/core.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/components/container/size.py` & `hebill-3.1.0/hebill/html/components/container/size.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/components/html/body/core.py` & `hebill-3.1.0/hebill/html/components/html/body/core.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/components/html/core.py` & `hebill-3.1.0/hebill/html/components/html/core.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/components/html/head/core.py` & `hebill-3.1.0/hebill/html/components/html/head/core.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/components/navbar/core.py` & `hebill-3.1.0/hebill/html/components/navbar/core.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/components/pagination/core.py` & `hebill-3.1.0/hebill/html/components/pagination/core.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/components/table/__templates__/color.py` & `hebill-3.1.0/hebill/html/components/table/__templates__/color.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/components/table/core.py` & `hebill-3.1.0/hebill/html/components/table/core.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/components/table/tbody/core.py` & `hebill-3.1.0/hebill/html/components/table/tbody/core.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/components/table/tbody/tr/core.py` & `hebill-3.1.0/hebill/html/components/table/tbody/tr/core.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/components/table/thead/core.py` & `hebill-3.1.0/hebill/html/components/table/thead/core.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/components/table/thead/tr/core.py` & `hebill-3.1.0/hebill/html/components/table/thead/tr/core.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/core.py` & `hebill-3.1.0/hebill/html/core.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/nodes/comment/core.py` & `hebill-3.1.0/hebill/html/nodes/comment/core.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/nodes/group/core.py` & `hebill-3.1.0/hebill/html/nodes/group/core.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/nodes/group/create/components/core.py` & `hebill-3.1.0/hebill/html/nodes/group/create/components/core.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/nodes/group/create/core.py` & `hebill-3.1.0/hebill/html/nodes/group/create/core.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/nodes/group/create/nodes/core.py` & `hebill-3.1.0/hebill/html/nodes/group/create/nodes/core.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/nodes/group/create/tags/core.py` & `hebill-3.1.0/hebill/html/nodes/group/create/tags/core.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/nodes/node/core.py` & `hebill-3.1.0/hebill/html/nodes/node/core.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/nodes/tag/attributes/classes/core.py` & `hebill-3.1.0/hebill/html/nodes/tag/attributes/classes/core.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/nodes/tag/attributes/core.py` & `hebill-3.1.0/hebill/html/nodes/tag/attributes/core.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/nodes/tag/attributes/styles/core.py` & `hebill-3.1.0/hebill/html/nodes/tag/attributes/styles/core.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/nodes/tag/core.py` & `hebill-3.1.0/hebill/html/nodes/tag/core.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/html/tags/__init__.py` & `hebill-3.1.0/hebill/html/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/pypi/README.MD` & `hebill-3.1.0/hebill/pypi/README.MD`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/pypi/core.py` & `hebill-3.1.0/hebill/pypi/core.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/string/core.py` & `hebill-3.1.0/hebill/string/core.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/terminal/color.py` & `hebill-3.1.0/hebill/terminal/color.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill/terminal/core.py` & `hebill-3.1.0/hebill/terminal/core.py`

 * *Files identical despite different names*

### Comparing `hebill-3.0.0/hebill.egg-info/SOURCES.txt` & `hebill-3.1.0/hebill.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -153,14 +153,20 @@
 hebill/html/tags/thead/core.py
 hebill/html/tags/title/__init__.py
 hebill/html/tags/title/core.py
 hebill/html/tags/tr/__init__.py
 hebill/html/tags/tr/core.py
 hebill/html/tags/ul/__init__.py
 hebill/html/tags/ul/core.py
+hebill/image/__init__.py
+hebill/image/png/__init__.py
+hebill/image/png/constants.py
+hebill/image/png/core.py
+hebill/math/__init__.py
+hebill/math/core.py
 hebill/pypi/README.MD
 hebill/pypi/__constants__.py
 hebill/pypi/__init__.py
 hebill/pypi/core.py
 hebill/string/__init__.py
 hebill/string/core.py
 hebill/string/string_random.py
```

