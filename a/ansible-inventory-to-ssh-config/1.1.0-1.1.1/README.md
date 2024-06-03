# Comparing `tmp/ansible-inventory-to-ssh-config-1.1.0.tar.gz` & `tmp/ansible_inventory_to_ssh_config-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-inventory-to-ssh-config-1.1.0.tar", last modified: Fri May 26 06:28:21 2023, max compression
+gzip compressed data, was "ansible_inventory_to_ssh_config-1.1.1.tar", last modified: Mon Jun  3 06:39:27 2024, max compression
```

## Comparing `ansible-inventory-to-ssh-config-1.1.0.tar` & `ansible_inventory_to_ssh_config-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,26 @@
-drwxr-xr-x   0 walter    (1000) walter    (1000)        0 2023-05-26 06:28:21.047472 ansible-inventory-to-ssh-config-1.1.0/
--rw-r--r--   0 walter    (1000) walter    (1000)     1062 2020-11-25 03:50:02.000000 ansible-inventory-to-ssh-config-1.1.0/LICENSE
--rw-r--r--   0 walter    (1000) walter    (1000)      289 2023-05-26 06:28:21.047472 ansible-inventory-to-ssh-config-1.1.0/PKG-INFO
--rw-r--r--   0 walter    (1000) walter    (1000)     2185 2023-05-26 06:21:45.000000 ansible-inventory-to-ssh-config-1.1.0/README.md
-drwxr-xr-x   0 walter    (1000) walter    (1000)        0 2023-05-26 06:28:21.047472 ansible-inventory-to-ssh-config-1.1.0/ansible_inventory_to_ssh_config.egg-info/
--rw-r--r--   0 walter    (1000) walter    (1000)      289 2023-05-26 06:28:20.000000 ansible-inventory-to-ssh-config-1.1.0/ansible_inventory_to_ssh_config.egg-info/PKG-INFO
--rw-r--r--   0 walter    (1000) walter    (1000)      386 2023-05-26 06:28:20.000000 ansible-inventory-to-ssh-config-1.1.0/ansible_inventory_to_ssh_config.egg-info/SOURCES.txt
--rw-r--r--   0 walter    (1000) walter    (1000)        1 2023-05-26 06:28:20.000000 ansible-inventory-to-ssh-config-1.1.0/ansible_inventory_to_ssh_config.egg-info/dependency_links.txt
--rw-r--r--   0 walter    (1000) walter    (1000)       88 2023-05-26 06:28:20.000000 ansible-inventory-to-ssh-config-1.1.0/ansible_inventory_to_ssh_config.egg-info/entry_points.txt
--rw-r--r--   0 walter    (1000) walter    (1000)       31 2023-05-26 06:28:20.000000 ansible-inventory-to-ssh-config-1.1.0/ansible_inventory_to_ssh_config.egg-info/requires.txt
--rw-r--r--   0 walter    (1000) walter    (1000)        4 2023-05-26 06:28:20.000000 ansible-inventory-to-ssh-config-1.1.0/ansible_inventory_to_ssh_config.egg-info/top_level.txt
--rw-r--r--   0 walter    (1000) walter    (1000)       38 2023-05-26 06:28:21.047472 ansible-inventory-to-ssh-config-1.1.0/setup.cfg
--rw-r--r--   0 walter    (1000) walter    (1000)      613 2023-05-26 06:18:52.000000 ansible-inventory-to-ssh-config-1.1.0/setup.py
-drwxr-xr-x   0 walter    (1000) walter    (1000)        0 2023-05-26 06:28:21.047472 ansible-inventory-to-ssh-config-1.1.0/src/
--rw-r--r--   0 walter    (1000) walter    (1000)        0 2021-01-06 08:54:25.000000 ansible-inventory-to-ssh-config-1.1.0/src/__init__.py
--rw-r--r--   0 walter    (1000) walter    (1000)     3652 2023-05-26 06:15:07.000000 ansible-inventory-to-ssh-config-1.1.0/src/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:39:27.737999 ansible_inventory_to_ssh_config-1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:39:27.729999 ansible_inventory_to_ssh_config-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:39:27.733999 ansible_inventory_to_ssh_config-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-06-03 06:39:22.000000 ansible_inventory_to_ssh_config-1.1.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-06-03 06:39:22.000000 ansible_inventory_to_ssh_config-1.1.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-06-03 06:39:22.000000 ansible_inventory_to_ssh_config-1.1.1/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-06-03 06:39:22.000000 ansible_inventory_to_ssh_config-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-06-03 06:39:22.000000 ansible_inventory_to_ssh_config-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-06-03 06:39:22.000000 ansible_inventory_to_ssh_config-1.1.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-06-03 06:39:27.733999 ansible_inventory_to_ssh_config-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-06-03 06:39:22.000000 ansible_inventory_to_ssh_config-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-06-03 06:39:22.000000 ansible_inventory_to_ssh_config-1.1.1/aitsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-06-03 06:39:22.000000 ansible_inventory_to_ssh_config-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-06-03 06:39:22.000000 ansible_inventory_to_ssh_config-1.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 06:39:27.737999 ansible_inventory_to_ssh_config-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:39:27.733999 ansible_inventory_to_ssh_config-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:39:27.733999 ansible_inventory_to_ssh_config-1.1.1/src/aitsc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 06:39:22.000000 ansible_inventory_to_ssh_config-1.1.1/src/aitsc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-06-03 06:39:22.000000 ansible_inventory_to_ssh_config-1.1.1/src/aitsc/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:39:27.733999 ansible_inventory_to_ssh_config-1.1.1/src/ansible_inventory_to_ssh_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-06-03 06:39:27.000000 ansible_inventory_to_ssh_config-1.1.1/src/ansible_inventory_to_ssh_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-06-03 06:39:27.000000 ansible_inventory_to_ssh_config-1.1.1/src/ansible_inventory_to_ssh_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 06:39:27.000000 ansible_inventory_to_ssh_config-1.1.1/src/ansible_inventory_to_ssh_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-06-03 06:39:27.000000 ansible_inventory_to_ssh_config-1.1.1/src/ansible_inventory_to_ssh_config.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-06-03 06:39:27.000000 ansible_inventory_to_ssh_config-1.1.1/src/ansible_inventory_to_ssh_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-03 06:39:27.000000 ansible_inventory_to_ssh_config-1.1.1/src/ansible_inventory_to_ssh_config.egg-info/top_level.txt
```

### Comparing `ansible-inventory-to-ssh-config-1.1.0/LICENSE` & `ansible_inventory_to_ssh_config-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-inventory-to-ssh-config-1.1.0/README.md` & `ansible_inventory_to_ssh_config-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ansible-inventory-to-ssh-config-1.1.0/src/main.py` & `ansible_inventory_to_ssh_config-1.1.1/src/aitsc/main.py`

 * *Files identical despite different names*

