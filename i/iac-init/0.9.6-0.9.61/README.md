# Comparing `tmp/iac_init-0.9.6.tar.gz` & `tmp/iac_init-0.9.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iac_init-0.9.6.tar", max compression
+gzip compressed data, was "iac_init-0.9.61.tar", max compression
```

## Comparing `iac_init-0.9.6.tar` & `iac_init-0.9.61.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0    16295 2024-06-03 05:17:44.928325 iac_init-0.9.6/LICENSE
--rw-r--r--   0        0        0     1622 2024-06-03 05:17:44.928325 iac_init-0.9.6/README.md
--rw-r--r--   0        0        0      392 2024-06-03 05:17:44.928325 iac_init-0.9.6/iac_init/__init__.py
--rw-r--r--   0        0        0      162 2024-06-03 05:17:44.928325 iac_init-0.9.6/iac_init/__main__.py
--rw-r--r--   0        0        0    13223 2024-06-03 05:17:44.928325 iac_init-0.9.6/iac_init/cli/main.py
--rw-r--r--   0        0        0      228 2024-06-03 05:17:44.928325 iac_init-0.9.6/iac_init/cli/options.py
--rw-r--r--   0        0        0     1775 2024-06-03 05:17:44.928325 iac_init-0.9.6/iac_init/conf/__init__.py
--rw-r--r--   0        0        0     1104 2024-06-03 05:17:44.928325 iac_init-0.9.6/iac_init/conf/global_settings.py
--rw-r--r--   0        0        0     1585 2024-06-03 05:17:44.928325 iac_init-0.9.6/iac_init/scripts/ansible_tool.py
--rw-r--r--   0        0        0     2756 2024-06-03 05:17:44.928325 iac_init-0.9.6/iac_init/scripts/apic_connecton_tool.py
--rw-r--r--   0        0        0     7793 2024-06-03 05:17:44.928325 iac_init-0.9.6/iac_init/scripts/cimc_precheck_tool.py
--rw-r--r--   0        0        0      438 2024-06-03 05:17:44.928325 iac_init-0.9.6/iac_init/scripts/logging_tool.py
--rw-r--r--   0        0        0      443 2024-06-03 05:17:44.928325 iac_init-0.9.6/iac_init/scripts/ssh_tool.py
--rw-r--r--   0        0        0     1744 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/scripts/telnet_tool.py
--rw-r--r--   0        0        0      415 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/scripts/thread_tool.py
--rw-r--r--   0        0        0     3778 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
--rw-r--r--   0        0        0     5040 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
--rw-r--r--   0        0        0     1860 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
--rw-r--r--   0        0        0     6989 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
--rw-r--r--   0        0        0     1370 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
--rw-r--r--   0        0        0        0 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
--rw-r--r--   0        0        0     5598 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
--rw-r--r--   0        0        0     1516 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
--rw-r--r--   0        0        0     1607 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
--rw-r--r--   0        0        0     1553 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
--rw-r--r--   0        0        0      790 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
--rw-r--r--   0        0        0      197 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
--rw-r--r--   0        0        0      194 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
--rw-r--r--   0        0        0        0 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/02-discover_apic/apic_discovery/files/.gitkeep
--rw-r--r--   0        0        0     1557 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
--rw-r--r--   0        0        0     3527 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2
--rw-r--r--   0        0        0     3585 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2
--rw-r--r--   0        0        0     1656 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2
--rw-r--r--   0        0        0        0 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/02-discover_apic/apic_discovery/vars/.gitkeep
--rw-r--r--   0        0        0      181 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
--rw-r--r--   0        0        0      388 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/03-nac_tasks/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/03-nac_tasks/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/03-nac_tasks/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/03-nac_tasks/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/03-nac_tasks/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/03-nac_tasks/inventory.yaml.j2
--rw-r--r--   0        0        0      101 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/utils/exceptions.py
--rw-r--r--   0        0        0     4924 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/utils/functional.py
--rw-r--r--   0        0        0    14779 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/validator.py
--rw-r--r--   0        0        0     5139 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/yaml_conf/yaml.py
--rw-r--r--   0        0        0     5430 2024-06-03 05:17:44.936325 iac_init-0.9.6/iac_init/yaml_conf/yaml_writer.py
--rw-r--r--   0        0        0     1666 2024-06-03 05:17:44.936325 iac_init-0.9.6/pyproject.toml
--rw-r--r--   0        0        0     2505 1970-01-01 00:00:00.000000 iac_init-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0    16295 2024-06-03 05:39:17.296067 iac_init-0.9.61/LICENSE
+-rw-r--r--   0        0        0     1622 2024-06-03 05:39:17.296067 iac_init-0.9.61/README.md
+-rw-r--r--   0        0        0      392 2024-06-03 05:39:17.296067 iac_init-0.9.61/iac_init/__init__.py
+-rw-r--r--   0        0        0      162 2024-06-03 05:39:17.296067 iac_init-0.9.61/iac_init/__main__.py
+-rw-r--r--   0        0        0    13237 2024-06-03 05:39:17.296067 iac_init-0.9.61/iac_init/cli/main.py
+-rw-r--r--   0        0        0      228 2024-06-03 05:39:17.296067 iac_init-0.9.61/iac_init/cli/options.py
+-rw-r--r--   0        0        0     1775 2024-06-03 05:39:17.296067 iac_init-0.9.61/iac_init/conf/__init__.py
+-rw-r--r--   0        0        0     1105 2024-06-03 05:39:17.296067 iac_init-0.9.61/iac_init/conf/global_settings.py
+-rw-r--r--   0        0        0     1585 2024-06-03 05:39:17.296067 iac_init-0.9.61/iac_init/scripts/ansible_tool.py
+-rw-r--r--   0        0        0     2712 2024-06-03 05:39:17.296067 iac_init-0.9.61/iac_init/scripts/apic_connecton_tool.py
+-rw-r--r--   0        0        0     7748 2024-06-03 05:39:17.296067 iac_init-0.9.61/iac_init/scripts/cimc_precheck_tool.py
+-rw-r--r--   0        0        0      439 2024-06-03 05:39:17.296067 iac_init-0.9.61/iac_init/scripts/logging_tool.py
+-rw-r--r--   0        0        0      443 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/scripts/ssh_tool.py
+-rw-r--r--   0        0        0     1699 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/scripts/telnet_tool.py
+-rw-r--r--   0        0        0      416 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/scripts/thread_tool.py
+-rw-r--r--   0        0        0     3778 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
+-rw-r--r--   0        0        0     5040 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
+-rw-r--r--   0        0        0     1860 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     6989 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
+-rw-r--r--   0        0        0     1370 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0        0 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
+-rw-r--r--   0        0        0     5598 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     1516 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
+-rw-r--r--   0        0        0     1607 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
+-rw-r--r--   0        0        0     1553 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
+-rw-r--r--   0        0        0      790 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0      197 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
+-rw-r--r--   0        0        0      194 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
+-rw-r--r--   0        0        0        0 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/templates/02-discover_apic/apic_discovery/files/.gitkeep
+-rw-r--r--   0        0        0     1557 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
+-rw-r--r--   0        0        0     3527 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2
+-rw-r--r--   0        0        0     3585 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2
+-rw-r--r--   0        0        0     1656 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/templates/02-discover_apic/apic_discovery/vars/.gitkeep
+-rw-r--r--   0        0        0      181 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
+-rw-r--r--   0        0        0      388 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/templates/03-nac_tasks/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/templates/03-nac_tasks/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/templates/03-nac_tasks/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/templates/03-nac_tasks/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/templates/03-nac_tasks/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/templates/03-nac_tasks/inventory.yaml.j2
+-rw-r--r--   0        0        0      101 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/utils/exceptions.py
+-rw-r--r--   0        0        0     4924 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/utils/functional.py
+-rw-r--r--   0        0        0    14779 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/validator.py
+-rw-r--r--   0        0        0     5104 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/yaml_conf/yaml.py
+-rw-r--r--   0        0        0     5396 2024-06-03 05:39:17.300067 iac_init-0.9.61/iac_init/yaml_conf/yaml_writer.py
+-rw-r--r--   0        0        0     1667 2024-06-03 05:39:17.304067 iac_init-0.9.61/pyproject.toml
+-rw-r--r--   0        0        0     2506 1970-01-01 00:00:00.000000 iac_init-0.9.61/PKG-INFO
```

### Comparing `iac_init-0.9.6/LICENSE` & `iac_init-0.9.61/LICENSE`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.6/README.md` & `iac_init-0.9.61/README.md`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.6/iac_init/cli/main.py` & `iac_init-0.9.61/iac_init/cli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,16 @@
     option_choice = click.prompt(
         click.style(option_prompt, fg='green'),
         type=validator.validate_choices)
     if not option_choice:
         exit()
 
     # Type "yes" or "no" to confirm
-    option_prompt = "\nAre you sure to proceed with following option(s)?\n{}\n"\
+    option_prompt = "\nAre you sure to proceed with following option(s)?" \
+                    "\n{}\n" \
         .format("\n".join([f"[{i}]  {settings.DEFAULT_USER_OPTIONS[int(i)-1]}"
                            for i in option_choice]))
     option_proceed = click.prompt(
         click.style(option_prompt, fg='green'),
         type=click.Choice(['yes', 'no'], case_sensitive=False)
     )
     validator._validate_bool(option_proceed)
@@ -348,18 +349,18 @@
                     exit()
 
             except Exception as e:
                 msg = "Run Step 3 NaC ansible-playbook" \
                       " failed.\nDetail: {}".format(e)
                 logger.error(msg)
                 exit()
-            
-            logger.info("Processing step {} completed.".format(option))
 
+            logger.info("Processing step {} completed.".format(option))
 
     logger.info(f"Option(s): {option_choice} had been completed!")
 
+
 def exit() -> None:
     if error_handler.fired:
         sys.exit(1)
     else:
         sys.exit(0)
```

### Comparing `iac_init-0.9.6/iac_init/conf/__init__.py` & `iac_init-0.9.61/iac_init/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.6/iac_init/conf/global_settings.py` & `iac_init-0.9.61/iac_init/conf/global_settings.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -38,8 +38,8 @@
 ANSIBLE_STEP = [
     'wipe_apic',
     'wipe_switch',
     'setup_apic',
     'aac_validate',
     'aac_deploy',
     'aac_test'
-]
+]
```

### Comparing `iac_init-0.9.6/iac_init/scripts/ansible_tool.py` & `iac_init-0.9.61/iac_init/scripts/ansible_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.6/iac_init/scripts/apic_connecton_tool.py` & `iac_init-0.9.61/iac_init/scripts/apic_connecton_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # -*- coding: utf-8 -*-
 
 # Copyright: (c) 2024, Wang Xiao <xiawang3@cisco.com>
 
 import requests
-import os
 import json
 import urllib3
-from iac_init.conf import settings
 from iac_init.scripts.logging_tool import setup_logging
 
 logger = setup_logging()
 
 urllib3.disable_warnings(
     urllib3.exceptions.InsecureRequestWarning
 )
@@ -46,14 +44,15 @@
         else:
             return False
     except Exception as e:
         msg = "{}".format(e)
         logger.error(msg)
         return False
 
+
 # Rudy: discuss AAA domain later
 def apic_login(APIC_IP, APIC_USERNAME, APIC_PASSWORD):
     try:
         apic_login_url = f"https://{APIC_IP}/api/aaaLogin.json"
         headers = {
             'accept': 'application/json',
             'Content-Type': 'application/json',
```

### Comparing `iac_init-0.9.6/iac_init/scripts/cimc_precheck_tool.py` & `iac_init-0.9.61/iac_init/scripts/cimc_precheck_tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # -*- coding: utf-8 -*-
 
 # Copyright: (c) 2024, Rudy Lei <shlei@cisco.com>
 
-import os
 import re
 import urllib3
 import requests
 import xml.etree.ElementTree as ET
 
-from iac_init.conf import settings
 from iac_init.scripts.logging_tool import setup_logging
 
 logger = setup_logging()
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
```

### Comparing `iac_init-0.9.6/iac_init/scripts/telnet_tool.py` & `iac_init-0.9.61/iac_init/scripts/telnet_tool.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # -*- coding: utf-8 -*-
 
 # Copyright: (c) 2024, Wang Xiao <xiawang3@cisco.com>
 
-import os
 import time
 import telnetlib
 
-from iac_init.conf import settings
 from iac_init.scripts.logging_tool import setup_logging
 
 logger = setup_logging()
 
 
 class TelnetClient:
     def __init__(
```

### Comparing `iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh` & `iac_init-0.9.61/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64` & `iac_init-0.9.61/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml` & `iac_init-0.9.61/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2` & `iac_init-0.9.61/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2` & `iac_init-0.9.61/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml` & `iac_init-0.9.61/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2` & `iac_init-0.9.61/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2` & `iac_init-0.9.61/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2` & `iac_init-0.9.61/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2` & `iac_init-0.9.61/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.6/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml` & `iac_init-0.9.61/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.6/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2` & `iac_init-0.9.61/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.6/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2` & `iac_init-0.9.61/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.6/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2` & `iac_init-0.9.61/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.6/iac_init/utils/functional.py` & `iac_init-0.9.61/iac_init/utils/functional.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.6/iac_init/validator.py` & `iac_init-0.9.61/iac_init/validator.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.6/iac_init/yaml_conf/yaml.py` & `iac_init-0.9.61/iac_init/yaml_conf/yaml.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 import os
 import subprocess
 import importlib.util
 from typing import Any, Dict, List
 
 from ruamel import yaml
-from iac_init.conf import settings
 from iac_init.scripts.logging_tool import setup_logging
 
 logger = setup_logging()
 
 
 class VaultTag(yaml.YAMLObject):
     yaml_tag = "!vault"
```

### Comparing `iac_init-0.9.6/iac_init/yaml_conf/yaml_writer.py` & `iac_init-0.9.61/iac_init/yaml_conf/yaml_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 import os
 import pathlib
 import shutil
 
 from . import yaml
 from typing import Any, Dict, List
 from jinja2 import ChainableUndefined, Environment, FileSystemLoader
-from iac_init.conf import settings
 from iac_init.scripts.logging_tool import setup_logging
 
 logger = setup_logging()
 
+
 class YamlWriter:
     def __init__(
         self,
         data_paths: List[str],
     ) -> None:
         logger.info("Loading YAML files from {}".format(data_paths[0]))
         self.data = yaml.load_yaml_files(data_paths)
```

### Comparing `iac_init-0.9.6/pyproject.toml` & `iac_init-0.9.61/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iac-init"
-version = "0.9.6"
+version = "0.9.61"
 description = ""
 authors = ["Wang Xiao <xiawang3@cisco.com>", "Rudy Lei <shlei@cisco.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 iac-init = "iac_init.cli.main:main"
```

### Comparing `iac_init-0.9.6/PKG-INFO` & `iac_init-0.9.61/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iac-init
-Version: 0.9.6
+Version: 0.9.61
 Summary: 
 Author: Wang Xiao
 Author-email: xiawang3@cisco.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

