# Comparing `tmp/iac_init-0.9.3.tar.gz` & `tmp/iac_init-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iac_init-0.9.3.tar", max compression
+gzip compressed data, was "iac_init-0.9.4.tar", max compression
```

## Comparing `iac_init-0.9.3.tar` & `iac_init-0.9.4.tar`

### file list

```diff
@@ -1,49 +1,50 @@
--rw-r--r--   0        0        0    16295 2024-05-31 04:54:50.890772 iac_init-0.9.3/LICENSE
--rw-r--r--   0        0        0     1622 2024-05-31 04:54:50.890772 iac_init-0.9.3/README.md
--rw-r--r--   0        0        0      392 2024-05-31 04:54:50.890772 iac_init-0.9.3/iac_init/__init__.py
--rw-r--r--   0        0        0      162 2024-05-31 04:54:50.890772 iac_init-0.9.3/iac_init/__main__.py
--rw-r--r--   0        0        0    13430 2024-05-31 04:54:50.890772 iac_init-0.9.3/iac_init/cli/main.py
--rw-r--r--   0        0        0      228 2024-05-31 04:54:50.890772 iac_init-0.9.3/iac_init/cli/options.py
--rw-r--r--   0        0        0     1829 2024-05-31 04:54:50.890772 iac_init-0.9.3/iac_init/conf/__init__.py
--rw-r--r--   0        0        0     1199 2024-05-31 04:54:50.890772 iac_init-0.9.3/iac_init/conf/global_settings.py
--rw-r--r--   0        0        0     1585 2024-05-31 04:54:50.890772 iac_init-0.9.3/iac_init/scripts/ansible_tool.py
--rw-r--r--   0        0        0     2921 2024-05-31 04:54:50.890772 iac_init-0.9.3/iac_init/scripts/apic_connecton_tool.py
--rw-r--r--   0        0        0     7958 2024-05-31 04:54:50.894772 iac_init-0.9.3/iac_init/scripts/cimc_precheck_tool.py
--rw-r--r--   0        0        0      443 2024-05-31 04:54:50.894772 iac_init-0.9.3/iac_init/scripts/ssh_tool.py
--rw-r--r--   0        0        0     1908 2024-05-31 04:54:50.894772 iac_init-0.9.3/iac_init/scripts/telnet_tool.py
--rw-r--r--   0        0        0      415 2024-05-31 04:54:50.894772 iac_init-0.9.3/iac_init/scripts/thread_tool.py
--rw-r--r--   0        0        0     3778 2024-05-31 04:54:50.894772 iac_init-0.9.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
--rw-r--r--   0        0        0     5040 2024-05-31 04:54:50.894772 iac_init-0.9.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
--rw-r--r--   0        0        0     1860 2024-05-31 04:54:50.894772 iac_init-0.9.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
--rw-r--r--   0        0        0     6989 2024-05-31 04:54:50.894772 iac_init-0.9.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
--rw-r--r--   0        0        0     1370 2024-05-31 04:54:50.894772 iac_init-0.9.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-31 04:54:50.894772 iac_init-0.9.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
--rw-r--r--   0        0        0        0 2024-05-31 04:54:50.894772 iac_init-0.9.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
--rw-r--r--   0        0        0     5598 2024-05-31 04:54:50.894772 iac_init-0.9.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
--rw-r--r--   0        0        0     1516 2024-05-31 04:54:50.898772 iac_init-0.9.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
--rw-r--r--   0        0        0     1607 2024-05-31 04:54:50.898772 iac_init-0.9.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
--rw-r--r--   0        0        0     1553 2024-05-31 04:54:50.898772 iac_init-0.9.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
--rw-r--r--   0        0        0      790 2024-05-31 04:54:50.898772 iac_init-0.9.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-31 04:54:50.898772 iac_init-0.9.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
--rw-r--r--   0        0        0      197 2024-05-31 04:54:50.898772 iac_init-0.9.3/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
--rw-r--r--   0        0        0      194 2024-05-31 04:54:50.898772 iac_init-0.9.3/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
--rw-r--r--   0        0        0        0 2024-05-31 04:54:50.898772 iac_init-0.9.3/iac_init/templates/02-discover_apic/apic_discovery/files/.gitkeep
--rw-r--r--   0        0        0     1557 2024-05-31 04:54:50.898772 iac_init-0.9.3/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
--rw-r--r--   0        0        0     3527 2024-05-31 04:54:50.898772 iac_init-0.9.3/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2
--rw-r--r--   0        0        0     3585 2024-05-31 04:54:50.898772 iac_init-0.9.3/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2
--rw-r--r--   0        0        0     1656 2024-05-31 04:54:50.898772 iac_init-0.9.3/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-31 04:54:50.898772 iac_init-0.9.3/iac_init/templates/02-discover_apic/apic_discovery/vars/.gitkeep
--rw-r--r--   0        0        0      181 2024-05-31 04:54:50.898772 iac_init-0.9.3/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
--rw-r--r--   0        0        0      388 2024-05-31 04:54:50.898772 iac_init-0.9.3/iac_init/templates/03-nac_tasks/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-31 04:54:50.898772 iac_init-0.9.3/iac_init/templates/03-nac_tasks/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-31 04:54:50.898772 iac_init-0.9.3/iac_init/templates/03-nac_tasks/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-31 04:54:50.898772 iac_init-0.9.3/iac_init/templates/03-nac_tasks/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-31 04:54:50.898772 iac_init-0.9.3/iac_init/templates/03-nac_tasks/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-31 04:54:50.898772 iac_init-0.9.3/iac_init/templates/03-nac_tasks/inventory.yaml.j2
--rw-r--r--   0        0        0      101 2024-05-31 04:54:50.898772 iac_init-0.9.3/iac_init/utils/exceptions.py
--rw-r--r--   0        0        0     4924 2024-05-31 04:54:50.898772 iac_init-0.9.3/iac_init/utils/functional.py
--rw-r--r--   0        0        0    15022 2024-05-31 04:54:50.898772 iac_init-0.9.3/iac_init/validator.py
--rw-r--r--   0        0        0     5304 2024-05-31 04:54:50.898772 iac_init-0.9.3/iac_init/yaml_conf/yaml.py
--rw-r--r--   0        0        0     5586 2024-05-31 04:54:50.898772 iac_init-0.9.3/iac_init/yaml_conf/yaml_writer.py
--rw-r--r--   0        0        0     1666 2024-05-31 04:54:50.898772 iac_init-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     2505 1970-01-01 00:00:00.000000 iac_init-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0    16295 2024-06-03 03:14:02.320320 iac_init-0.9.4/LICENSE
+-rw-r--r--   0        0        0     1622 2024-06-03 03:14:02.320320 iac_init-0.9.4/README.md
+-rw-r--r--   0        0        0      392 2024-06-03 03:14:02.320320 iac_init-0.9.4/iac_init/__init__.py
+-rw-r--r--   0        0        0      162 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/__main__.py
+-rw-r--r--   0        0        0    13498 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/cli/main.py
+-rw-r--r--   0        0        0      228 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/cli/options.py
+-rw-r--r--   0        0        0     1829 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/conf/__init__.py
+-rw-r--r--   0        0        0     1203 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/conf/global_settings.py
+-rw-r--r--   0        0        0     1585 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/scripts/ansible_tool.py
+-rw-r--r--   0        0        0     2756 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/scripts/apic_connecton_tool.py
+-rw-r--r--   0        0        0     7793 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/scripts/cimc_precheck_tool.py
+-rw-r--r--   0        0        0      327 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/scripts/logging_tool.py
+-rw-r--r--   0        0        0      443 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/scripts/ssh_tool.py
+-rw-r--r--   0        0        0     1745 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/scripts/telnet_tool.py
+-rw-r--r--   0        0        0      415 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/scripts/thread_tool.py
+-rw-r--r--   0        0        0     3778 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
+-rw-r--r--   0        0        0     5040 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
+-rw-r--r--   0        0        0     1860 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     6989 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
+-rw-r--r--   0        0        0     1370 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0        0 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
+-rw-r--r--   0        0        0     5598 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     1516 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
+-rw-r--r--   0        0        0     1607 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
+-rw-r--r--   0        0        0     1553 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
+-rw-r--r--   0        0        0      790 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0      197 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
+-rw-r--r--   0        0        0      194 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
+-rw-r--r--   0        0        0        0 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/templates/02-discover_apic/apic_discovery/files/.gitkeep
+-rw-r--r--   0        0        0     1557 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
+-rw-r--r--   0        0        0     3527 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2
+-rw-r--r--   0        0        0     3585 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2
+-rw-r--r--   0        0        0     1656 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/templates/02-discover_apic/apic_discovery/vars/.gitkeep
+-rw-r--r--   0        0        0      181 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
+-rw-r--r--   0        0        0      388 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/templates/03-nac_tasks/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/templates/03-nac_tasks/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/templates/03-nac_tasks/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/templates/03-nac_tasks/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/templates/03-nac_tasks/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/templates/03-nac_tasks/inventory.yaml.j2
+-rw-r--r--   0        0        0      101 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/utils/exceptions.py
+-rw-r--r--   0        0        0     4924 2024-06-03 03:14:02.324320 iac_init-0.9.4/iac_init/utils/functional.py
+-rw-r--r--   0        0        0    14874 2024-06-03 03:14:02.328320 iac_init-0.9.4/iac_init/validator.py
+-rw-r--r--   0        0        0     5304 2024-06-03 03:14:02.328320 iac_init-0.9.4/iac_init/yaml_conf/yaml.py
+-rw-r--r--   0        0        0     5586 2024-06-03 03:14:02.328320 iac_init-0.9.4/iac_init/yaml_conf/yaml_writer.py
+-rw-r--r--   0        0        0     1666 2024-06-03 03:14:02.328320 iac_init-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     2505 1970-01-01 00:00:00.000000 iac_init-0.9.4/PKG-INFO
```

### Comparing `iac_init-0.9.3/LICENSE` & `iac_init-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.3/README.md` & `iac_init-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.3/iac_init/cli/main.py` & `iac_init-0.9.4/iac_init/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 import sys
 import click
 import shutil
 import errorhandler
 import iac_init.validator
 
 from . import options
-from loguru import logger
 from iac_init.conf import settings
 from iac_init.yaml_conf import yaml_writer
 from iac_init.scripts.thread_tool import MyThread
 from iac_init.scripts.ansible_tool import ansible_deploy_function
+from iac_init.scripts.logging_tool import setup_logging
 
 error_handler = errorhandler.ErrorHandler()
 
 
 @click.command(context_settings=dict(help_option_names=["-h", "--help"]))
 @click.version_option(iac_init.__version__)
 @options.yaml_dir_path
@@ -27,23 +27,15 @@
 ) -> None:
     """A CLI tool to bootstrap and configure ACI fabric using ACI as Code."""
     output = settings.OUTPUT_BASE_DIR
 
     if os.path.exists(output) and os.path.isdir(output):
         shutil.rmtree(output)
 
-    logger.add(
-        sink=os.path.join(
-            settings.OUTPUT_BASE_DIR,
-            'iac_init_log',
-            'iac_init_main.log'
-        ),
-        format='{time:YYYY-MM-DD HH:mm:ss} | {level} | {message}',
-        encoding='utf-8'
-    )
+    logger = setup_logging()
 
     validator = iac_init.validator.Validator(data, output)
 
     # Type single number or multiple numbers (1,2...)
     option_prompt = "Select single or multiple option(s) " \
                     "to init ACI Fabric:\n{}\nExample: (1,2,..)"\
         .format("\n".join([f"[{i + 1}]  {option}" for i, option
@@ -81,19 +73,19 @@
             )
             if not yaml_path:
                 exit()
             error = validator.validate_cimc_precheck()
             if error:
                 exit()
             # Rudy: If only 1, this might not need to check
-            option_yaml_path = validator.validate_yaml_exist(
-                settings.DATA_PATH[int(option)-1]
-            )
-            if not option_yaml_path:
-                exit()
+            # option_yaml_path = validator.validate_yaml_exist(
+            #     settings.DATA_PATH[int(option)-1]
+            # )
+            # if not option_yaml_path:
+            #     exit()
             try:
                 writer = yaml_writer.YamlWriter([yaml_path])
                 writer.write(settings.TEMPLATE_DIR[int(option) - 1], output)
                 logger.info("Generate step {} working directory in {} successfully."
                             .format(option, output))
 
                 dir_path = os.path.join(
@@ -140,24 +132,24 @@
                     "playbook_aci_switch_init.yaml"
                 )
 
                 thread1 = MyThread(
                     target=ansible_deploy_function,
                     args=(
                         playbook_dir_apic,
-                        settings.ANSIBLE_STEP[3],
+                        settings.ANSIBLE_STEP[0],
                         option,
                         None,
                         True)
                 )
                 thread2 = MyThread(
                     target=ansible_deploy_function,
                     args=(
                         playbook_dir_switch,
-                        settings.ANSIBLE_STEP[4],
+                        settings.ANSIBLE_STEP[1],
                         option,
                         None,
                         True)
                 )
 
                 logger.info("ACI fabric bootstrap in progress, "
                             "check APIC/switch logs for detail.")
@@ -166,14 +158,15 @@
                 thread2.start()
 
                 thread1.join()
                 thread2.join()
 
                 if thread1.get_result() and thread2.get_result():
                     logger.info("ACI fabric bootstrap is successfully.")
+                    logger.info("Processing step {} is completed.".format(option))
                 else:
                     logger.error(
                         "ACI fabric bootstrap failed, "
                         "check APIC/switch logs for detail."
                     )
                     exit()
 
@@ -188,19 +181,19 @@
                 settings.DEFAULT_DATA_PATH
             )
             if not yaml_path:
                 exit()
             error = validator.validate_cimc_precheck()
             if error:
                 exit()
-            option_yaml_path = validator.validate_yaml_exist(
-                settings.DATA_PATH[int(option)-1]
-            )
-            if not option_yaml_path:
-                exit()
+            # option_yaml_path = validator.validate_yaml_exist(
+            #     settings.DATA_PATH[int(option)-1]
+            # )
+            # if not option_yaml_path:
+            #     exit()
             try:
                 writer = yaml_writer.YamlWriter([yaml_path])
                 writer.write(settings.TEMPLATE_DIR[int(option)-1], output)
                 logger.info(
                     "Generate step {} working directory in {} successfully."
                     .format(option, output)
                 )
@@ -230,20 +223,21 @@
                     output,
                     os.path.basename(settings.TEMPLATE_DIR[int(option)-1]),
                     "playbook_apic_discovery.yaml"
                 )
 
                 run_result = ansible_deploy_function(
                     playbook_dir=playbook_dir,
-                    step_name=settings.ANSIBLE_STEP[5],
+                    step_name=settings.ANSIBLE_STEP[2],
                     option=option,
                     quiet=False
                 )
                 if run_result:
                     logger.info("APIC init successfully.")
+                    logger.info("Processing step {} is completed.".format(option))
                 else:
                     logger.error("APIC init failed!")
                     exit()
 
             except Exception as e:
                 msg = "Run Step 2 APIC init ansible-playbook" \
                       " failed.\nDetail: {}".format(e)
@@ -256,15 +250,15 @@
                 exit()
             yaml_path = validator.validate_yaml_exist(
                 settings.DEFAULT_DATA_PATH
             )
             if not yaml_path:
                 exit()
             option_yaml_path = validator.validate_yaml_dir_exist(
-                settings.DATA_PATH[int(option)-1]
+                settings.DATA_PATH
             )
             if not option_yaml_path:
                 exit()
             try:
                 writer = yaml_writer.YamlWriter([yaml_path])
                 writer.write(
                     settings.TEMPLATE_DIR[int(option)-1],
@@ -327,49 +321,51 @@
                     os.path.basename(settings.TEMPLATE_DIR[int(option)-1]),
                     'aac_ansible',
                     "apic_test.yaml"
                 )
 
                 validate_result = ansible_deploy_function(
                     playbook_dir=playbook_dir_validate,
-                    step_name=settings.ANSIBLE_STEP[0],
+                    step_name=settings.ANSIBLE_STEP[3],
                     inventory_path=inventory_path,
                     option=option,
                     quiet=False)
 
                 if not validate_result:
                     exit()
 
                 deploy_result = ansible_deploy_function(
                     playbook_dir=playbook_dir_deploy,
-                    step_name=settings.ANSIBLE_STEP[1],
+                    step_name=settings.ANSIBLE_STEP[4],
                     inventory_path=inventory_path,
                     option=option,
                     quiet=False
                 )
 
                 if not deploy_result:
                     exit()
 
                 test_result = ansible_deploy_function(
                     playbook_dir=playbook_dir_test,
-                    step_name=settings.ANSIBLE_STEP[2],
+                    step_name=settings.ANSIBLE_STEP[5],
                     inventory_path=inventory_path,
                     option=option,
                     quiet=False
                 )
 
                 if not test_result:
                     exit()
 
             except Exception as e:
                 msg = "Run Step 3 NaC ansible-playbook" \
                       " failed.\nDetail: {}".format(e)
                 logger.error(msg)
                 exit()
+            
+            logger.info("Processing step {} is completed.".format(option))
 
 
 def exit() -> None:
     if error_handler.fired:
         sys.exit(1)
     else:
         sys.exit(0)
```

### Comparing `iac_init-0.9.3/iac_init/conf/__init__.py` & `iac_init-0.9.4/iac_init/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.3/iac_init/conf/global_settings.py` & `iac_init-0.9.4/iac_init/conf/global_settings.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,20 +13,21 @@
     "Wipe and boot APIC/switch to particular version(APIC + Switch)",
     "APIC initial setup(Single Pod)",
     "Init ACI Fabric via NaC(Network as Code)"
 ]
 
 
 DEFAULT_DATA_PATH = "00-global_policy.yml"
+DATA_PATH = "nac_data"
 
-DATA_PATH = [
-    "00-global_policy.yml",
-    "00-global_policy.yml",
-    "nac_data",
-]
+# DATA_PATH = [
+#     "00-global_policy.yml",
+#     "00-global_policy.yml",
+#     "nac_data",
+# ]
 
 TEMPLATE_DIR = [
     os.path.join(BASE_DIR, "templates", "01-wipe_aci_fabric"),
     os.path.join(BASE_DIR, "templates", "02-discover_apic"),
     os.path.join(BASE_DIR, "templates", "03-nac_tasks"),
 ]
 
@@ -35,16 +36,16 @@
     os.path.join(OUTPUT_BASE_DIR, "02-discover_apic"),
     os.path.join(OUTPUT_BASE_DIR, "03-nac_tasks"),
 ]
 
 os.environ["iac_init_option_1"] = OUTPUT_DIR[0]
 os.environ["iac_init_option_2"] = OUTPUT_DIR[1]
 
-# Rudy: sync the step name later
+
 ANSIBLE_STEP = [
-    'iac-validate',
-    'deploy',
-    'iac-test',
     'wipe_apic',
     'wipe_switch',
-    'apic_setup'
-]
+    'setup_apic',
+    'aac_validate',
+    'aac_deploy',
+    'aac_test'
+]
```

### Comparing `iac_init-0.9.3/iac_init/scripts/ansible_tool.py` & `iac_init-0.9.4/iac_init/scripts/ansible_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.3/iac_init/scripts/apic_connecton_tool.py` & `iac_init-0.9.4/iac_init/scripts/apic_connecton_tool.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,27 +2,18 @@
 
 # Copyright: (c) 2024, Wang Xiao <xiawang3@cisco.com>
 
 import requests
 import os
 import json
 import urllib3
-from loguru import logger
 from iac_init.conf import settings
+from iac_init.scripts.logging_tool import setup_logging
 
-# Rudy: need to check log setting
-logger.add(
-    sink=os.path.join(
-        settings.OUTPUT_BASE_DIR,
-        'iac_init_log',
-        'iac_init_main.log'
-    ),
-    format="{time} {level} {message}",
-    level="INFO"
-)
+logger = setup_logging()
 
 urllib3.disable_warnings(
     urllib3.exceptions.InsecureRequestWarning
 )
 
 
 def get_health_status(APIC_IP, token):
```

### Comparing `iac_init-0.9.3/iac_init/scripts/cimc_precheck_tool.py` & `iac_init-0.9.4/iac_init/scripts/cimc_precheck_tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,27 +4,18 @@
 
 import os
 import re
 import urllib3
 import requests
 import xml.etree.ElementTree as ET
 
-from loguru import logger
 from iac_init.conf import settings
+from iac_init.scripts.logging_tool import setup_logging
 
-# Rudy: need to check log setting
-logger.add(
-    sink=os.path.join(
-        settings.OUTPUT_BASE_DIR,
-        'iac_init_log',
-        'iac_init_main.log'
-    ),
-    format="{time} {level} {message}",
-    level="INFO"
-)
+logger = setup_logging()
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 
 def cimc_api(CIMC_IP, data):
     try:
         cimc_url = f"https://{CIMC_IP}/nuova"
```

### Comparing `iac_init-0.9.3/iac_init/scripts/telnet_tool.py` & `iac_init-0.9.4/iac_init/scripts/telnet_tool.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 # -*- coding: utf-8 -*-
 
 # Copyright: (c) 2024, Wang Xiao <xiawang3@cisco.com>
 
 import os
 import time
 import telnetlib
-from loguru import logger
+
 from iac_init.conf import settings
+from iac_init.scripts.logging_tool import setup_logging
+
 
-# Rudy: need to check log setting
-logger.add(
-    sink=os.path.join(
-        settings.OUTPUT_BASE_DIR,
-        'iac_init_log',
-        'iac_init_main.log'
-    ),
-    format="{time} {level} {message}",
-    level="INFO"
-)
+logger = setup_logging()
 
 
 class TelnetClient:
     def __init__(
             self,
             telnet_ip,
             telnet_port,
```

### Comparing `iac_init-0.9.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh` & `iac_init-0.9.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64` & `iac_init-0.9.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml` & `iac_init-0.9.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2` & `iac_init-0.9.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2` & `iac_init-0.9.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml` & `iac_init-0.9.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2` & `iac_init-0.9.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2` & `iac_init-0.9.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2` & `iac_init-0.9.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2` & `iac_init-0.9.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.3/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml` & `iac_init-0.9.4/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.3/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2` & `iac_init-0.9.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.3/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2` & `iac_init-0.9.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.3/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2` & `iac_init-0.9.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.3/iac_init/utils/functional.py` & `iac_init-0.9.4/iac_init/utils/functional.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.3/iac_init/validator.py` & `iac_init-0.9.4/iac_init/validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,25 @@
 # Copyright: (c) 2024, Wang Xiao <xiawang3@cisco.com>
 
 import os
 import re
 import time
 from ruamel import yaml
 
-from loguru import logger
 from typing import Any, Dict, List, Optional
 
 from iac_init.conf import settings
 from iac_init.yaml_conf.yaml import load_yaml_files
 from iac_init.scripts.ssh_tool import check_ssh_connection
 from iac_init.scripts.apic_connecton_tool import apic_login
 from iac_init.scripts.cimc_precheck_tool import cimc_precheck
 from iac_init.scripts.telnet_tool import TelnetClient
+from iac_init.scripts.logging_tool import setup_logging
 
-logger.add(sink=os.path.join(settings.OUTPUT_BASE_DIR,
-           'iac_init_log', 'iac_init_main.log'),
-           format='{time:YYYY-MM-DD HH:mm:ss} | {level} | {message}',
-           encoding='utf-8')
+logger = setup_logging()
 
 
 class Validator:
     def __init__(self, data_path: str, output: str):
         self.data: Optional[Dict[str, Any]] = None
         self.data_path = data_path
         self.output = output
```

### Comparing `iac_init-0.9.3/iac_init/yaml_conf/yaml.py` & `iac_init-0.9.4/iac_init/yaml_conf/yaml.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.3/iac_init/yaml_conf/yaml_writer.py` & `iac_init-0.9.4/iac_init/yaml_conf/yaml_writer.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.3/pyproject.toml` & `iac_init-0.9.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iac-init"
-version = "0.9.3"
+version = "0.9.4"
 description = ""
 authors = ["Wang Xiao <xiawang3@cisco.com>", "Rudy Lei <shlei@cisco.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 iac-init = "iac_init.cli.main:main"
```

### Comparing `iac_init-0.9.3/PKG-INFO` & `iac_init-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iac-init
-Version: 0.9.3
+Version: 0.9.4
 Summary: 
 Author: Wang Xiao
 Author-email: xiawang3@cisco.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

