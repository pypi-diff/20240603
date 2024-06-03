# Comparing `tmp/amisui-0.1.4.tar.gz` & `tmp/amisui-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amisui-0.1.4.tar", last modified: Thu Mar 14 12:26:38 2024, max compression
+gzip compressed data, was "amisui-0.1.5.tar", last modified: Mon Jun  3 14:23:54 2024, max compression
```

## Comparing `amisui-0.1.4.tar` & `amisui-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11358 2024-03-14 12:26:20.737538 amisui-0.1.4/LICENSE
--rw-r--r--   0        0        0     1327 2024-03-14 12:26:20.737538 amisui-0.1.4/README.md
--rw-r--r--   0        0        0      475 2024-03-14 12:26:38.753529 amisui-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      249 2024-03-14 12:26:20.737538 amisui-0.1.4/src/amisui/__init__.py
--rw-r--r--   0        0        0   179558 2024-03-14 12:26:20.737538 amisui-0.1.4/src/amisui/components.py
--rw-r--r--   0        0        0      103 2024-03-14 12:26:20.737538 amisui-0.1.4/src/amisui/config.py
--rw-r--r--   0        0        0     1287 2024-03-14 12:26:20.737538 amisui-0.1.4/src/amisui/constants.py
--rw-r--r--   0        0        0     7006 2024-03-14 12:26:20.737538 amisui-0.1.4/src/amisui/templates/app.jinja2
--rw-r--r--   0        0        0     1555 2024-03-14 12:26:20.737538 amisui-0.1.4/src/amisui/templates/page.jinja2
--rw-r--r--   0        0        0     5918 2024-03-14 12:26:20.737538 amisui-0.1.4/src/amisui/types.py
--rw-r--r--   0        0        0        0 2024-03-14 12:26:20.737538 amisui-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0      381 2024-03-14 12:26:20.737538 amisui-0.1.4/tests/test.py
--rw-r--r--   0        0        0     1607 1970-01-01 00:00:00.000000 amisui-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-06-03 14:23:39.736894 amisui-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1327 2024-06-03 14:23:39.736894 amisui-0.1.5/README.md
+-rw-r--r--   0        0        0      475 2024-06-03 14:23:54.636719 amisui-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      249 2024-06-03 14:23:39.736894 amisui-0.1.5/src/amisui/__init__.py
+-rw-r--r--   0        0        0   179558 2024-06-03 14:23:39.736894 amisui-0.1.5/src/amisui/components.py
+-rw-r--r--   0        0        0      103 2024-06-03 14:23:39.736894 amisui-0.1.5/src/amisui/config.py
+-rw-r--r--   0        0        0     1287 2024-06-03 14:23:39.736894 amisui-0.1.5/src/amisui/constants.py
+-rw-r--r--   0        0        0     7006 2024-06-03 14:23:39.736894 amisui-0.1.5/src/amisui/templates/app.jinja2
+-rw-r--r--   0        0        0     1555 2024-06-03 14:23:39.736894 amisui-0.1.5/src/amisui/templates/page.jinja2
+-rw-r--r--   0        0        0     5731 2024-06-03 14:23:39.736894 amisui-0.1.5/src/amisui/types.py
+-rw-r--r--   0        0        0        0 2024-06-03 14:23:39.736894 amisui-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0      381 2024-06-03 14:23:39.736894 amisui-0.1.5/tests/test.py
+-rw-r--r--   0        0        0     1607 1970-01-01 00:00:00.000000 amisui-0.1.5/PKG-INFO
```

### Comparing `amisui-0.1.4/LICENSE` & `amisui-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `amisui-0.1.4/README.md` & `amisui-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `amisui-0.1.4/src/amisui/components.py` & `amisui-0.1.5/src/amisui/components.py`

 * *Files identical despite different names*

### Comparing `amisui-0.1.4/src/amisui/constants.py` & `amisui-0.1.5/src/amisui/constants.py`

 * *Files identical despite different names*

### Comparing `amisui-0.1.4/src/amisui/templates/app.jinja2` & `amisui-0.1.5/src/amisui/templates/app.jinja2`

 * *Files identical despite different names*

### Comparing `amisui-0.1.4/src/amisui/templates/page.jinja2` & `amisui-0.1.5/src/amisui/templates/page.jinja2`

 * *Files identical despite different names*

### Comparing `amisui-0.1.4/src/amisui/types.py` & `amisui-0.1.5/src/amisui/types.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,24 +9,20 @@
 Expression = str
 Template = Union[str, "Tpl", dict]
 SchemaNode = Union[Template, "AmisNode", List["AmisNode"], dict]
 OptionsNode = Union[List[dict], List[str]]
 
 
 class BaseAmisModel(BaseModel):
-    class Config:
-        extra = Extra.allow
-        json_loads = json.loads
-        json_dumps = json.dumps
 
     def to_json(self):
-        return self.json(exclude_none=True, by_alias=True, ensure_ascii=False, indent=4)
+        return self.model_dump_json()
 
     def to_dict(self):
-        return self.dict(exclude_none=True, by_alias=True)
+        return self.model_dump()
 
     def update_from_dict(self, kwargs: Dict[str, Any]):
         for k, v in kwargs.items():
             setattr(self, k, v)
         return self
 
     def update_from_kwargs(self, **kwargs):
```

### Comparing `amisui-0.1.4/PKG-INFO` & `amisui-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: amisui
-Version: 0.1.4
+Version: 0.1.5
 Summary: Default template for PDM package
 Author-Email: luxuncang <luxuncang@qq.com>
 License: Apache-2.0
 Requires-Python: >3.7
-Requires-Dist: pydantic==1.10.14
+Requires-Dist: pydantic>=1.10.14
 Requires-Dist: jinja2>=3.1.3
 Description-Content-Type: text/markdown
 
 ## amis-python
 <p align="center">
     <a href="https://cdn.jsdelivr.net/gh/CMHopeSunshine/amis-python@master/LICENSE"><img src="https://img.shields.io/github/license/CMHopeSunshine/amis-python" alt="license"></a>
     <img src="https://img.shields.io/badge/Python-3.8+-yellow" alt="python">
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: amisui Version: 0.1.4 Summary: Default template for
+Metadata-Version: 2.1 Name: amisui Version: 0.1.5 Summary: Default template for
 PDM package Author-Email: luxuncang
 qq.com> License: Apache-2.0 Requires-Python: >3.7 Requires-Dist:
-pydantic==1.10.14 Requires-Dist: jinja2>=3.1.3 Description-Content-Type: text/
+pydantic>=1.10.14 Requires-Dist: jinja2>=3.1.3 Description-Content-Type: text/
 markdown ## amis-python
                           _[_l_i_c_e_n_s_e_][python][version]
 åºäº [ç¾åº¦amis](https://github.com/baidu/amis) åç«¯æ¡æ¶çpython
 pydanticæ¨¡åå°è£ã ç±äº[åçæ¬](https://github.com/amisadmin/
 fastapi_amis_admin/tree/master/fastapi_amis_admin/
 amis)ç¼ºå°å¤§éamisæ°çæ¬çç»ä»¶æéç½®ï¼å æ­¤æ¬é¡¹ç®å¨å¶çæ¬çåºç¡ä¸è¿è¡äºæ©åã
 ç¸æ¯fastapi-amis-adminççæ¬ï¼ -
```

