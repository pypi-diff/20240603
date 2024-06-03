# Comparing `tmp/iac_init-0.9.62.tar.gz` & `tmp/iac_init-0.9.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iac_init-0.9.62.tar", max compression
+gzip compressed data, was "iac_init-0.9.63.tar", max compression
```

## Comparing `iac_init-0.9.62.tar` & `iac_init-0.9.63.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0    16295 2024-06-03 05:51:48.153941 iac_init-0.9.62/LICENSE
--rw-r--r--   0        0        0     1622 2024-06-03 05:51:48.153941 iac_init-0.9.62/README.md
--rw-r--r--   0        0        0      392 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/__init__.py
--rw-r--r--   0        0        0      162 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/__main__.py
--rw-r--r--   0        0        0    13355 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/cli/main.py
--rw-r--r--   0        0        0      228 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/cli/options.py
--rw-r--r--   0        0        0     1931 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/conf/__init__.py
--rw-r--r--   0        0        0     1105 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/conf/global_settings.py
--rw-r--r--   0        0        0     1585 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/scripts/ansible_tool.py
--rw-r--r--   0        0        0     2712 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/scripts/apic_connecton_tool.py
--rw-r--r--   0        0        0     7748 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/scripts/cimc_precheck_tool.py
--rw-r--r--   0        0        0      439 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/scripts/logging_tool.py
--rw-r--r--   0        0        0      443 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/scripts/ssh_tool.py
--rw-r--r--   0        0        0     1768 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/scripts/telnet_tool.py
--rw-r--r--   0        0        0      416 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/scripts/thread_tool.py
--rw-r--r--   0        0        0     3778 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
--rw-r--r--   0        0        0     5040 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
--rw-r--r--   0        0        0     1860 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
--rw-r--r--   0        0        0     6989 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
--rw-r--r--   0        0        0     1370 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
--rw-r--r--   0        0        0        0 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
--rw-r--r--   0        0        0     5598 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
--rw-r--r--   0        0        0     1516 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
--rw-r--r--   0        0        0     1607 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
--rw-r--r--   0        0        0     1553 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
--rw-r--r--   0        0        0      790 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
--rw-r--r--   0        0        0      197 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
--rw-r--r--   0        0        0      194 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
--rw-r--r--   0        0        0        0 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/templates/02-discover_apic/apic_discovery/files/.gitkeep
--rw-r--r--   0        0        0     1557 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
--rw-r--r--   0        0        0     3527 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2
--rw-r--r--   0        0        0     3585 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2
--rw-r--r--   0        0        0     1656 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2
--rw-r--r--   0        0        0        0 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/templates/02-discover_apic/apic_discovery/vars/.gitkeep
--rw-r--r--   0        0        0      181 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
--rw-r--r--   0        0        0      388 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/templates/03-nac_tasks/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/templates/03-nac_tasks/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/templates/03-nac_tasks/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/templates/03-nac_tasks/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/templates/03-nac_tasks/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-06-03 05:51:48.153941 iac_init-0.9.62/iac_init/templates/03-nac_tasks/inventory.yaml.j2
--rw-r--r--   0        0        0      101 2024-06-03 05:51:48.157941 iac_init-0.9.62/iac_init/utils/exceptions.py
--rw-r--r--   0        0        0     4924 2024-06-03 05:51:48.157941 iac_init-0.9.62/iac_init/utils/functional.py
--rw-r--r--   0        0        0    14848 2024-06-03 05:51:48.157941 iac_init-0.9.62/iac_init/validator.py
--rw-r--r--   0        0        0     5104 2024-06-03 05:51:48.157941 iac_init-0.9.62/iac_init/yaml_conf/yaml.py
--rw-r--r--   0        0        0     5396 2024-06-03 05:51:48.157941 iac_init-0.9.62/iac_init/yaml_conf/yaml_writer.py
--rw-r--r--   0        0        0     1667 2024-06-03 05:51:48.157941 iac_init-0.9.62/pyproject.toml
--rw-r--r--   0        0        0     2506 1970-01-01 00:00:00.000000 iac_init-0.9.62/PKG-INFO
+-rw-r--r--   0        0        0    16295 2024-06-03 05:54:49.634122 iac_init-0.9.63/LICENSE
+-rw-r--r--   0        0        0     1622 2024-06-03 05:54:49.634122 iac_init-0.9.63/README.md
+-rw-r--r--   0        0        0      392 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/__init__.py
+-rw-r--r--   0        0        0      162 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/__main__.py
+-rw-r--r--   0        0        0    13211 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/cli/main.py
+-rw-r--r--   0        0        0      228 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/cli/options.py
+-rw-r--r--   0        0        0     1816 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/conf/__init__.py
+-rw-r--r--   0        0        0     1105 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/conf/global_settings.py
+-rw-r--r--   0        0        0     1585 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/scripts/ansible_tool.py
+-rw-r--r--   0        0        0     2712 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/scripts/apic_connecton_tool.py
+-rw-r--r--   0        0        0     7748 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/scripts/cimc_precheck_tool.py
+-rw-r--r--   0        0        0      439 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/scripts/logging_tool.py
+-rw-r--r--   0        0        0      443 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/scripts/ssh_tool.py
+-rw-r--r--   0        0        0     1768 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/scripts/telnet_tool.py
+-rw-r--r--   0        0        0      416 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/scripts/thread_tool.py
+-rw-r--r--   0        0        0     3778 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
+-rw-r--r--   0        0        0     5040 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
+-rw-r--r--   0        0        0     1860 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     6989 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
+-rw-r--r--   0        0        0     1370 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0        0 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
+-rw-r--r--   0        0        0     5598 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     1516 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
+-rw-r--r--   0        0        0     1607 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
+-rw-r--r--   0        0        0     1553 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
+-rw-r--r--   0        0        0      790 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0      197 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
+-rw-r--r--   0        0        0      194 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
+-rw-r--r--   0        0        0        0 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/templates/02-discover_apic/apic_discovery/files/.gitkeep
+-rw-r--r--   0        0        0     1557 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
+-rw-r--r--   0        0        0     3527 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2
+-rw-r--r--   0        0        0     3585 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2
+-rw-r--r--   0        0        0     1656 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/templates/02-discover_apic/apic_discovery/vars/.gitkeep
+-rw-r--r--   0        0        0      181 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
+-rw-r--r--   0        0        0      388 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/templates/03-nac_tasks/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/templates/03-nac_tasks/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-06-03 05:54:49.634122 iac_init-0.9.63/iac_init/templates/03-nac_tasks/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-06-03 05:54:49.638122 iac_init-0.9.63/iac_init/templates/03-nac_tasks/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-06-03 05:54:49.638122 iac_init-0.9.63/iac_init/templates/03-nac_tasks/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-06-03 05:54:49.638122 iac_init-0.9.63/iac_init/templates/03-nac_tasks/inventory.yaml.j2
+-rw-r--r--   0        0        0      101 2024-06-03 05:54:49.638122 iac_init-0.9.63/iac_init/utils/exceptions.py
+-rw-r--r--   0        0        0     4924 2024-06-03 05:54:49.638122 iac_init-0.9.63/iac_init/utils/functional.py
+-rw-r--r--   0        0        0    14848 2024-06-03 05:54:49.638122 iac_init-0.9.63/iac_init/validator.py
+-rw-r--r--   0        0        0     5104 2024-06-03 05:54:49.638122 iac_init-0.9.63/iac_init/yaml_conf/yaml.py
+-rw-r--r--   0        0        0     5396 2024-06-03 05:54:49.638122 iac_init-0.9.63/iac_init/yaml_conf/yaml_writer.py
+-rw-r--r--   0        0        0     1667 2024-06-03 05:54:49.638122 iac_init-0.9.63/pyproject.toml
+-rw-r--r--   0        0        0     2506 1970-01-01 00:00:00.000000 iac_init-0.9.63/PKG-INFO
```

### Comparing `iac_init-0.9.62/LICENSE` & `iac_init-0.9.63/LICENSE`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.62/README.md` & `iac_init-0.9.63/README.md`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.62/iac_init/cli/main.py` & `iac_init-0.9.63/iac_init/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,17 +79,15 @@
                 exit()
             error = validator.validate_cimc_precheck()
             if error:
                 exit()
             try:
                 writer = yaml_writer.YamlWriter([yaml_path])
                 writer.write(settings.TEMPLATE_DIR[int(option) - 1], output)
-                # logger.info("Generate step {} working directory in {} successfully."
-                #             .format(option, output))
-                logger.info(f"Generate step {option} working directory" \
+                logger.info(f"Generate step {option} working directory"
                             f"in {output} successfully")
 
                 dir_path = os.path.join(
                     output,
                     os.path.basename(settings.TEMPLATE_DIR[int(option)-1]),
                     'aci_switch_reimage',
                     'vars'
```

### Comparing `iac_init-0.9.62/iac_init/conf/__init__.py` & `iac_init-0.9.63/iac_init/conf/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     def __getattr__(self, name):
         """Return the value of a setting and cache it in self.__dict__."""
         _wrapped = None
         if (_wrapped := self._wrapped) is empty:
             self._setup(name)
             _wrapped = self._wrapped
         # val = getattr(self._wrapped, name)
-        # add fix: ./iac_init/conf/__init__.py:31:13: F841 local variable '_wrapped' is assigned to but never used
         val = getattr(_wrapped, name)
         self.__dict__[name] = val
         return val
 
     def __setattr__(self, name, value):
         """
         Set the value of setting. Clear all cached values if _wrapped changes
```

### Comparing `iac_init-0.9.62/iac_init/conf/global_settings.py` & `iac_init-0.9.63/iac_init/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.62/iac_init/scripts/ansible_tool.py` & `iac_init-0.9.63/iac_init/scripts/ansible_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.62/iac_init/scripts/apic_connecton_tool.py` & `iac_init-0.9.63/iac_init/scripts/apic_connecton_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.62/iac_init/scripts/cimc_precheck_tool.py` & `iac_init-0.9.63/iac_init/scripts/cimc_precheck_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.62/iac_init/scripts/telnet_tool.py` & `iac_init-0.9.63/iac_init/scripts/telnet_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.62/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh` & `iac_init-0.9.63/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.62/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64` & `iac_init-0.9.63/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.62/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml` & `iac_init-0.9.63/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.62/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2` & `iac_init-0.9.63/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.62/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2` & `iac_init-0.9.63/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.62/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml` & `iac_init-0.9.63/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.62/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2` & `iac_init-0.9.63/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.62/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2` & `iac_init-0.9.63/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.62/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2` & `iac_init-0.9.63/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.62/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2` & `iac_init-0.9.63/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.62/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml` & `iac_init-0.9.63/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.62/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2` & `iac_init-0.9.63/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.62/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2` & `iac_init-0.9.63/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.62/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2` & `iac_init-0.9.63/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.62/iac_init/utils/functional.py` & `iac_init-0.9.63/iac_init/utils/functional.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.62/iac_init/validator.py` & `iac_init-0.9.63/iac_init/validator.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.62/iac_init/yaml_conf/yaml.py` & `iac_init-0.9.63/iac_init/yaml_conf/yaml.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.62/iac_init/yaml_conf/yaml_writer.py` & `iac_init-0.9.63/iac_init/yaml_conf/yaml_writer.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.62/pyproject.toml` & `iac_init-0.9.63/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iac-init"
-version = "0.9.62"
+version = "0.9.63"
 description = ""
 authors = ["Wang Xiao <xiawang3@cisco.com>", "Rudy Lei <shlei@cisco.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 iac-init = "iac_init.cli.main:main"
```

### Comparing `iac_init-0.9.62/PKG-INFO` & `iac_init-0.9.63/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iac-init
-Version: 0.9.62
+Version: 0.9.63
 Summary: 
 Author: Wang Xiao
 Author-email: xiawang3@cisco.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

