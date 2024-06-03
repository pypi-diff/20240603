# Comparing `tmp/pynboard-0.0.3.tar.gz` & `tmp/pynboard-0.0.5.tar.gz`

## Comparing `pynboard-0.0.3.tar` & `pynboard-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 pynboard-0.0.3/requirements.txt
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 pynboard-0.0.3/.idea/.gitignore
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 pynboard-0.0.3/.idea/misc.xml
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 pynboard-0.0.3/.idea/modules.xml
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 pynboard-0.0.3/.idea/pynboard.iml
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pynboard-0.0.3/.idea/vcs.xml
--rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 pynboard-0.0.3/.idea/workspace.xml
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 pynboard-0.0.3/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pynboard-0.0.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pynboard-0.0.3/examples/scratch_00.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 pynboard-0.0.3/src/pynboard/__init__.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 pynboard-0.0.3/src/pynboard/actions.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 pynboard-0.0.3/src/pynboard/core.py
--rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 pynboard-0.0.3/src/pynboard/html_buffer.py
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 pynboard-0.0.3/src/pynboard/utils.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pynboard-0.0.3/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pynboard-0.0.3/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pynboard-0.0.3/README.md
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pynboard-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 pynboard-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 pynboard-0.0.5/requirements.txt
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 pynboard-0.0.5/.idea/.gitignore
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 pynboard-0.0.5/.idea/misc.xml
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 pynboard-0.0.5/.idea/modules.xml
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 pynboard-0.0.5/.idea/pynboard.iml
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pynboard-0.0.5/.idea/vcs.xml
+-rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 pynboard-0.0.5/.idea/workspace.xml
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 pynboard-0.0.5/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pynboard-0.0.5/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pynboard-0.0.5/examples/scratch_00.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 pynboard-0.0.5/src/pynboard/__init__.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 pynboard-0.0.5/src/pynboard/actions.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 pynboard-0.0.5/src/pynboard/core.py
+-rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 pynboard-0.0.5/src/pynboard/html_buffer.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 pynboard-0.0.5/src/pynboard/utils.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pynboard-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pynboard-0.0.5/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pynboard-0.0.5/README.md
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 pynboard-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 pynboard-0.0.5/PKG-INFO
```

### Comparing `pynboard-0.0.3/.idea/workspace.xml` & `pynboard-0.0.5/.idea/workspace.xml`

 * *Files 0% similar despite different names*

#### Comparing `pynboard-0.0.3/.idea/workspace.xml` & `pynboard-0.0.5/.idea/workspace.xml`

```diff
@@ -69,15 +69,15 @@
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="8e3ec5eb-ecea-4929-9532-604c6ae2131c" name="Changes" comment=""/>
       <created>1717348824739</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1717348824739</updated>
-      <workItem from="1717348826484" duration="6615000"/>
+      <workItem from="1717348826484" duration="7541000"/>
     </task>
     <task id="LOCAL-00001" summary="pynboard">
       <option name="closed" value="true"/>
       <created>1717348938104</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
```

### Comparing `pynboard-0.0.3/.idea/inspectionProfiles/Project_Default.xml` & `pynboard-0.0.5/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `pynboard-0.0.3/examples/scratch_00.py` & `pynboard-0.0.5/examples/scratch_00.py`

 * *Files identical despite different names*

### Comparing `pynboard-0.0.3/src/pynboard/__init__.py` & `pynboard-0.0.5/src/pynboard/__init__.py`

 * *Files identical despite different names*

### Comparing `pynboard-0.0.3/src/pynboard/actions.py` & `pynboard-0.0.5/src/pynboard/actions.py`

 * *Files identical despite different names*

### Comparing `pynboard-0.0.3/src/pynboard/core.py` & `pynboard-0.0.5/src/pynboard/core.py`

 * *Files identical despite different names*

### Comparing `pynboard-0.0.3/src/pynboard/html_buffer.py` & `pynboard-0.0.5/src/pynboard/html_buffer.py`

 * *Files identical despite different names*

### Comparing `pynboard-0.0.3/LICENSE` & `pynboard-0.0.5/LICENSE`

 * *Files identical despite different names*

