# Comparing `tmp/iac_init-0.9.52.tar.gz` & `tmp/iac_init-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iac_init-0.9.52.tar", max compression
+gzip compressed data, was "iac_init-0.9.6.tar", max compression
```

## Comparing `iac_init-0.9.52.tar` & `iac_init-0.9.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0    16295 2024-06-03 03:34:57.409356 iac_init-0.9.52/LICENSE
--rw-r--r--   0        0        0     1622 2024-06-03 03:34:57.409356 iac_init-0.9.52/README.md
--rw-r--r--   0        0        0      392 2024-06-03 03:34:57.409356 iac_init-0.9.52/iac_init/__init__.py
--rw-r--r--   0        0        0      162 2024-06-03 03:34:57.409356 iac_init-0.9.52/iac_init/__main__.py
--rw-r--r--   0        0        0    13477 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/cli/main.py
--rw-r--r--   0        0        0      228 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/cli/options.py
--rw-r--r--   0        0        0     1829 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/conf/__init__.py
--rw-r--r--   0        0        0     1203 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/conf/global_settings.py
--rw-r--r--   0        0        0     1585 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/scripts/ansible_tool.py
--rw-r--r--   0        0        0     2756 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/scripts/apic_connecton_tool.py
--rw-r--r--   0        0        0     7793 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/scripts/cimc_precheck_tool.py
--rw-r--r--   0        0        0      379 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/scripts/logging_tool.py
--rw-r--r--   0        0        0      443 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/scripts/ssh_tool.py
--rw-r--r--   0        0        0     1745 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/scripts/telnet_tool.py
--rw-r--r--   0        0        0      415 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/scripts/thread_tool.py
--rw-r--r--   0        0        0     3778 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
--rw-r--r--   0        0        0     5040 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
--rw-r--r--   0        0        0     1860 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
--rw-r--r--   0        0        0     6989 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
--rw-r--r--   0        0        0     1370 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
--rw-r--r--   0        0        0        0 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
--rw-r--r--   0        0        0     5598 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
--rw-r--r--   0        0        0     1516 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
--rw-r--r--   0        0        0     1607 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
--rw-r--r--   0        0        0     1553 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
--rw-r--r--   0        0        0      790 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
--rw-r--r--   0        0        0      197 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
--rw-r--r--   0        0        0      194 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
--rw-r--r--   0        0        0        0 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/templates/02-discover_apic/apic_discovery/files/.gitkeep
--rw-r--r--   0        0        0     1557 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
--rw-r--r--   0        0        0     3527 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2
--rw-r--r--   0        0        0     3585 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2
--rw-r--r--   0        0        0     1656 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2
--rw-r--r--   0        0        0        0 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/templates/02-discover_apic/apic_discovery/vars/.gitkeep
--rw-r--r--   0        0        0      181 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
--rw-r--r--   0        0        0      388 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/templates/03-nac_tasks/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/templates/03-nac_tasks/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/templates/03-nac_tasks/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/templates/03-nac_tasks/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/templates/03-nac_tasks/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/templates/03-nac_tasks/inventory.yaml.j2
--rw-r--r--   0        0        0      101 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/utils/exceptions.py
--rw-r--r--   0        0        0     4924 2024-06-03 03:34:57.413356 iac_init-0.9.52/iac_init/utils/functional.py
--rw-r--r--   0        0        0    14874 2024-06-03 03:34:57.417356 iac_init-0.9.52/iac_init/validator.py
--rw-r--r--   0        0        0     5304 2024-06-03 03:34:57.417356 iac_init-0.9.52/iac_init/yaml_conf/yaml.py
--rw-r--r--   0        0        0     5586 2024-06-03 03:34:57.417356 iac_init-0.9.52/iac_init/yaml_conf/yaml_writer.py
--rw-r--r--   0        0        0     1667 2024-06-03 03:34:57.417356 iac_init-0.9.52/pyproject.toml
--rw-r--r--   0        0        0     2506 1970-01-01 00:00:00.000000 iac_init-0.9.52/PKG-INFO
+-rw-r--r--   0        0        0    16295 2024-06-03 05:17:44.928325 iac_init-0.9.6/LICENSE
+-rw-r--r--   0        0        0     1622 2024-06-03 05:17:44.928325 iac_init-0.9.6/README.md
+-rw-r--r--   0        0        0      392 2024-06-03 05:17:44.928325 iac_init-0.9.6/iac_init/__init__.py
+-rw-r--r--   0        0        0      162 2024-06-03 05:17:44.928325 iac_init-0.9.6/iac_init/__main__.py
+-rw-r--r--   0        0        0    13223 2024-06-03 05:17:44.928325 iac_init-0.9.6/iac_init/cli/main.py
+-rw-r--r--   0        0        0      228 2024-06-03 05:17:44.928325 iac_init-0.9.6/iac_init/cli/options.py
+-rw-r--r--   0        0        0     1775 2024-06-03 05:17:44.928325 iac_init-0.9.6/iac_init/conf/__init__.py
+-rw-r--r--   0        0        0     1104 2024-06-03 05:17:44.928325 iac_init-0.9.6/iac_init/conf/global_settings.py
+-rw-r--r--   0        0        0     1585 2024-06-03 05:17:44.928325 iac_init-0.9.6/iac_init/scripts/ansible_tool.py
+-rw-r--r--   0        0        0     2756 2024-06-03 05:17:44.928325 iac_init-0.9.6/iac_init/scripts/apic_connecton_tool.py
+-rw-r--r--   0        0        0     7793 2024-06-03 05:17:44.928325 iac_init-0.9.6/iac_init/scripts/cimc_precheck_tool.py
+-rw-r--r--   0        0        0      438 2024-06-03 05:17:44.928325 iac_init-0.9.6/iac_init/scripts/logging_tool.py
+-rw-r--r--   0        0        0      443 2024-06-03 05:17:44.928325 iac_init-0.9.6/iac_init/scripts/ssh_tool.py
+-rw-r--r--   0        0        0     1744 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/scripts/telnet_tool.py
+-rw-r--r--   0        0        0      415 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/scripts/thread_tool.py
+-rw-r--r--   0        0        0     3778 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
+-rw-r--r--   0        0        0     5040 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
+-rw-r--r--   0        0        0     1860 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     6989 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
+-rw-r--r--   0        0        0     1370 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0        0 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
+-rw-r--r--   0        0        0     5598 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     1516 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
+-rw-r--r--   0        0        0     1607 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
+-rw-r--r--   0        0        0     1553 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
+-rw-r--r--   0        0        0      790 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0      197 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
+-rw-r--r--   0        0        0      194 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
+-rw-r--r--   0        0        0        0 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/02-discover_apic/apic_discovery/files/.gitkeep
+-rw-r--r--   0        0        0     1557 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
+-rw-r--r--   0        0        0     3527 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2
+-rw-r--r--   0        0        0     3585 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2
+-rw-r--r--   0        0        0     1656 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/02-discover_apic/apic_discovery/vars/.gitkeep
+-rw-r--r--   0        0        0      181 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
+-rw-r--r--   0        0        0      388 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/03-nac_tasks/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/03-nac_tasks/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/03-nac_tasks/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/03-nac_tasks/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/03-nac_tasks/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/templates/03-nac_tasks/inventory.yaml.j2
+-rw-r--r--   0        0        0      101 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/utils/exceptions.py
+-rw-r--r--   0        0        0     4924 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/utils/functional.py
+-rw-r--r--   0        0        0    14779 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/validator.py
+-rw-r--r--   0        0        0     5139 2024-06-03 05:17:44.932325 iac_init-0.9.6/iac_init/yaml_conf/yaml.py
+-rw-r--r--   0        0        0     5430 2024-06-03 05:17:44.936325 iac_init-0.9.6/iac_init/yaml_conf/yaml_writer.py
+-rw-r--r--   0        0        0     1666 2024-06-03 05:17:44.936325 iac_init-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0     2505 1970-01-01 00:00:00.000000 iac_init-0.9.6/PKG-INFO
```

### Comparing `iac_init-0.9.52/LICENSE` & `iac_init-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.52/README.md` & `iac_init-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.52/iac_init/cli/main.py` & `iac_init-0.9.6/iac_init/cli/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,16 @@
     output = settings.OUTPUT_BASE_DIR
 
     if os.path.exists(output) and os.path.isdir(output):
         shutil.rmtree(output)
 
     logger = setup_logging()
 
+    logger.info("Start to process aac-init tool!")
+
     validator = iac_init.validator.Validator(data, output)
 
     # Type single number or multiple numbers (1,2...)
     option_prompt = "Select single or multiple option(s) " \
                     "to init ACI Fabric:\n{}\nExample: (1,2,..)"\
         .format("\n".join([f"[{i + 1}]  {option}" for i, option
                            in enumerate(settings.DEFAULT_USER_OPTIONS)]))
@@ -54,17 +56,18 @@
         click.style(option_prompt, fg='green'),
         type=click.Choice(['yes', 'no'], case_sensitive=False)
     )
     validator._validate_bool(option_proceed)
 
     error = validator._wrapped()
     if error:
-        logger.error("Option(s) validated failed, exiting...")
+        logger.error(f"Option(s): {option_choice} validated failed, exiting...")
         exit()
     logger.info("Option(s) validated.")
+    logger.info(f"Option(s): {option_choice} had been selected!")
 
     for option in option_choice:
         logger.info("Start processing step {}.".format(option))
         if int(option) in [1]:
             error = validator.validate_ssh_telnet_connection()
             if error:
                 exit()
@@ -72,20 +75,14 @@
                 settings.DEFAULT_DATA_PATH
             )
             if not yaml_path:
                 exit()
             error = validator.validate_cimc_precheck()
             if error:
                 exit()
-            # Rudy: If only 1, this might not need to check
-            # option_yaml_path = validator.validate_yaml_exist(
-            #     settings.DATA_PATH[int(option)-1]
-            # )
-            # if not option_yaml_path:
-            #     exit()
             try:
                 writer = yaml_writer.YamlWriter([yaml_path])
                 writer.write(settings.TEMPLATE_DIR[int(option) - 1], output)
                 logger.info("Generate step {} working directory in {} successfully."
                             .format(option, output))
 
                 dir_path = os.path.join(
@@ -158,15 +155,15 @@
                 thread2.start()
 
                 thread1.join()
                 thread2.join()
 
                 if thread1.get_result() and thread2.get_result():
                     logger.info("ACI fabric bootstrap is successfully.")
-                    logger.info("Processing step {} is completed.".format(option))
+                    logger.info("Processing step {} completed.".format(option))
                 else:
                     logger.error(
                         "ACI fabric bootstrap failed, "
                         "check APIC/switch logs for detail."
                     )
                     exit()
 
@@ -181,19 +178,14 @@
                 settings.DEFAULT_DATA_PATH
             )
             if not yaml_path:
                 exit()
             error = validator.validate_cimc_precheck()
             if error:
                 exit()
-            # option_yaml_path = validator.validate_yaml_exist(
-            #     settings.DATA_PATH[int(option)-1]
-            # )
-            # if not option_yaml_path:
-            #     exit()
             try:
                 writer = yaml_writer.YamlWriter([yaml_path])
                 writer.write(settings.TEMPLATE_DIR[int(option)-1], output)
                 logger.info(
                     "Generate step {} working directory in {} successfully."
                     .format(option, output)
                 )
@@ -228,22 +220,22 @@
                 run_result = ansible_deploy_function(
                     playbook_dir=playbook_dir,
                     step_name=settings.ANSIBLE_STEP[2],
                     option=option,
                     quiet=False
                 )
                 if run_result:
-                    logger.info("APIC init successfully.")
-                    logger.info("Processing step {} is completed.".format(option))
+                    logger.info("APIC setup successfully.")
+                    logger.info("Processing step {} completed.".format(option))
                 else:
-                    logger.error("APIC init failed!")
+                    logger.error("APIC setup failed!")
                     exit()
 
             except Exception as e:
-                msg = "Run Step 2 APIC init ansible-playbook" \
+                msg = "Run Step 2 APIC setup ansible-playbook" \
                       " failed.\nDetail: {}".format(e)
                 logger.error(msg)
                 exit()
 
         elif int(option) in [3]:
             error = validator.validate_apic_aaa_connection()
             if error:
@@ -357,15 +349,17 @@
 
             except Exception as e:
                 msg = "Run Step 3 NaC ansible-playbook" \
                       " failed.\nDetail: {}".format(e)
                 logger.error(msg)
                 exit()
             
-            logger.info("Processing step {} is completed.".format(option))
+            logger.info("Processing step {} completed.".format(option))
+
 
+    logger.info(f"Option(s): {option_choice} had been completed!")
 
 def exit() -> None:
     if error_handler.fired:
         sys.exit(1)
     else:
         sys.exit(0)
```

### Comparing `iac_init-0.9.52/iac_init/conf/__init__.py` & `iac_init-0.9.6/iac_init/conf/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 # -*- coding: utf-8 -*-
 
 # Copyright: (c) 2024, Wang Xiao <xiawang3@cisco.com>
 
 from iac_init.conf import global_settings
 from iac_init.utils.functional import LazyObject, empty
 
-# ENVIRONMENT_VARIABLE = "IAC_INIT_SETTINGS_MODULE"
-
-
 class SettingsReference(str):
     """
     String subclass which references a current settings value. It's treated as
     the value in memory but serializes to a settings.NAME attribute reference.
     """
 
     def __new__(self, value, setting_name):
```

### Comparing `iac_init-0.9.52/iac_init/conf/global_settings.py` & `iac_init-0.9.6/iac_init/conf/global_settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,20 +15,14 @@
     "Init ACI Fabric via NaC(Network as Code)"
 ]
 
 
 DEFAULT_DATA_PATH = "00-global_policy.yml"
 DATA_PATH = "nac_data"
 
-# DATA_PATH = [
-#     "00-global_policy.yml",
-#     "00-global_policy.yml",
-#     "nac_data",
-# ]
-
 TEMPLATE_DIR = [
     os.path.join(BASE_DIR, "templates", "01-wipe_aci_fabric"),
     os.path.join(BASE_DIR, "templates", "02-discover_apic"),
     os.path.join(BASE_DIR, "templates", "03-nac_tasks"),
 ]
 
 OUTPUT_DIR = [
```

### Comparing `iac_init-0.9.52/iac_init/scripts/ansible_tool.py` & `iac_init-0.9.6/iac_init/scripts/ansible_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.52/iac_init/scripts/apic_connecton_tool.py` & `iac_init-0.9.6/iac_init/scripts/apic_connecton_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.52/iac_init/scripts/cimc_precheck_tool.py` & `iac_init-0.9.6/iac_init/scripts/cimc_precheck_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.52/iac_init/scripts/telnet_tool.py` & `iac_init-0.9.6/iac_init/scripts/telnet_tool.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import os
 import time
 import telnetlib
 
 from iac_init.conf import settings
 from iac_init.scripts.logging_tool import setup_logging
 
-
 logger = setup_logging()
 
 
 class TelnetClient:
     def __init__(
             self,
             telnet_ip,
```

### Comparing `iac_init-0.9.52/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh` & `iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.52/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64` & `iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.52/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml` & `iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.52/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2` & `iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.52/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2` & `iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.52/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml` & `iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.52/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2` & `iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.52/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2` & `iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.52/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2` & `iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.52/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2` & `iac_init-0.9.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.52/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml` & `iac_init-0.9.6/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.52/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2` & `iac_init-0.9.6/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.52/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2` & `iac_init-0.9.6/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.52/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2` & `iac_init-0.9.6/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.52/iac_init/utils/functional.py` & `iac_init-0.9.6/iac_init/utils/functional.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.52/iac_init/validator.py` & `iac_init-0.9.6/iac_init/validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -313,16 +313,14 @@
                 logger.error(msg)
                 self.errors.append(msg)
                 return
         self.choices = sorted(choices, key=lambda x: int(x))
         self.options = value
         return self.choices
 
-    # This function is used for option 1 and 2.
-    # Rudy: seems this is used for all options
     def validate_yaml_exist(self, yamlfile):
         for dir, _, files in os.walk(self.data_path):
             for filename in files:
                 if yamlfile == filename:
                     self.yaml_path = os.path.join(dir, filename)
         if self.yaml_path:
             msg = "YAML file {} validated successfully.".format(yamlfile)
```

### Comparing `iac_init-0.9.52/iac_init/yaml_conf/yaml.py` & `iac_init-0.9.6/iac_init/yaml_conf/yaml.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,27 +4,18 @@
 
 import os
 import subprocess
 import importlib.util
 from typing import Any, Dict, List
 
 from ruamel import yaml
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
 
 
 class VaultTag(yaml.YAMLObject):
     yaml_tag = "!vault"
 
     def __init__(self, v: str):
         self.value = v
```

### Comparing `iac_init-0.9.52/iac_init/yaml_conf/yaml_writer.py` & `iac_init-0.9.6/iac_init/yaml_conf/yaml_writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,27 +4,20 @@
 
 import json
 import os
 import pathlib
 import shutil
 
 from . import yaml
-from loguru import logger
 from typing import Any, Dict, List
 from jinja2 import ChainableUndefined, Environment, FileSystemLoader
 from iac_init.conf import settings
+from iac_init.scripts.logging_tool import setup_logging
 
-# Rudy: need to check log setting
-logger.add(
-    sink=os.path.join(
-        settings.OUTPUT_BASE_DIR,
-        'iac_init_log',
-        'iac_init_main.log'),
-    format="{time} {level} {message}", level="INFO")
-
+logger = setup_logging()
 
 class YamlWriter:
     def __init__(
         self,
         data_paths: List[str],
     ) -> None:
         logger.info("Loading YAML files from {}".format(data_paths[0]))
```

### Comparing `iac_init-0.9.52/pyproject.toml` & `iac_init-0.9.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iac-init"
-version = "0.9.52"
+version = "0.9.6"
 description = ""
 authors = ["Wang Xiao <xiawang3@cisco.com>", "Rudy Lei <shlei@cisco.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 iac-init = "iac_init.cli.main:main"
```

### Comparing `iac_init-0.9.52/PKG-INFO` & `iac_init-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iac-init
-Version: 0.9.52
+Version: 0.9.6
 Summary: 
 Author: Wang Xiao
 Author-email: xiawang3@cisco.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

