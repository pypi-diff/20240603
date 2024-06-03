# Comparing `tmp/delphai_fastapi-3.0.6.tar.gz` & `tmp/delphai_fastapi-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delphai_fastapi-3.0.6.tar", max compression
+gzip compressed data, was "delphai_fastapi-3.0.7.tar", max compression
```

## Comparing `delphai_fastapi-3.0.6.tar` & `delphai_fastapi-3.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       86 2024-05-31 11:03:38.595655 delphai_fastapi-3.0.6/delphai_fastapi/__init__.py
--rw-r--r--   0        0        0     2652 2024-05-31 11:03:38.595655 delphai_fastapi-3.0.6/delphai_fastapi/app.py
--rw-r--r--   0        0        0     5713 2024-05-31 11:03:38.595655 delphai_fastapi-3.0.6/delphai_fastapi/auth.py
--rw-r--r--   0        0        0        0 2024-05-31 11:03:38.595655 delphai_fastapi-3.0.6/delphai_fastapi/companies/__init__.py
--rw-r--r--   0        0        0     5582 2024-05-31 11:03:38.595655 delphai_fastapi-3.0.6/delphai_fastapi/companies/models.py
--rw-r--r--   0        0        0      375 2024-05-31 11:03:38.595655 delphai_fastapi-3.0.6/delphai_fastapi/decorators.py
--rw-r--r--   0        0        0        0 2024-05-31 11:03:38.595655 delphai_fastapi-3.0.6/delphai_fastapi/funding_rounds/__init__.py
--rw-r--r--   0        0        0     1623 2024-05-31 11:03:38.595655 delphai_fastapi-3.0.6/delphai_fastapi/funding_rounds/models.py
--rw-r--r--   0        0        0     1314 2024-05-31 11:03:38.595655 delphai_fastapi-3.0.6/delphai_fastapi/instrumentation.py
--rw-r--r--   0        0        0        0 2024-05-31 11:03:38.595655 delphai_fastapi-3.0.6/delphai_fastapi/job_posts/__init__.py
--rw-r--r--   0        0        0     3134 2024-05-31 11:03:38.599655 delphai_fastapi-3.0.6/delphai_fastapi/job_posts/models.py
--rw-r--r--   0        0        0     1386 2024-05-31 11:03:38.599655 delphai_fastapi-3.0.6/delphai_fastapi/models.py
--rw-r--r--   0        0        0        0 2024-05-31 11:03:38.599655 delphai_fastapi-3.0.6/delphai_fastapi/news_articles/__init__.py
--rw-r--r--   0        0        0     1120 2024-05-31 11:03:38.599655 delphai_fastapi-3.0.6/delphai_fastapi/news_articles/models.py
--rw-r--r--   0        0        0        0 2024-05-31 11:03:38.599655 delphai_fastapi-3.0.6/delphai_fastapi/projects/__init__.py
--rw-r--r--   0        0        0     1523 2024-05-31 11:03:38.599655 delphai_fastapi-3.0.6/delphai_fastapi/projects/models.py
--rw-r--r--   0        0        0      405 2024-05-31 11:03:38.599655 delphai_fastapi-3.0.6/delphai_fastapi/server.py
--rw-r--r--   0        0        0     3089 2024-05-31 11:03:38.599655 delphai_fastapi-3.0.6/delphai_fastapi/types.py
--rw-r--r--   0        0        0      590 2024-05-31 11:03:38.599655 delphai_fastapi-3.0.6/pyproject.toml
--rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 delphai_fastapi-3.0.6/PKG-INFO
+-rw-r--r--   0        0        0       86 2024-06-03 11:00:54.795224 delphai_fastapi-3.0.7/delphai_fastapi/__init__.py
+-rw-r--r--   0        0        0     2652 2024-06-03 11:00:54.795224 delphai_fastapi-3.0.7/delphai_fastapi/app.py
+-rw-r--r--   0        0        0     5713 2024-06-03 11:00:54.795224 delphai_fastapi-3.0.7/delphai_fastapi/auth.py
+-rw-r--r--   0        0        0        0 2024-06-03 11:00:54.795224 delphai_fastapi-3.0.7/delphai_fastapi/companies/__init__.py
+-rw-r--r--   0        0        0     5582 2024-06-03 11:00:54.795224 delphai_fastapi-3.0.7/delphai_fastapi/companies/models.py
+-rw-r--r--   0        0        0      375 2024-06-03 11:00:54.795224 delphai_fastapi-3.0.7/delphai_fastapi/decorators.py
+-rw-r--r--   0        0        0        0 2024-06-03 11:00:54.795224 delphai_fastapi-3.0.7/delphai_fastapi/funding_rounds/__init__.py
+-rw-r--r--   0        0        0     1623 2024-06-03 11:00:54.795224 delphai_fastapi-3.0.7/delphai_fastapi/funding_rounds/models.py
+-rw-r--r--   0        0        0     1314 2024-06-03 11:00:54.795224 delphai_fastapi-3.0.7/delphai_fastapi/instrumentation.py
+-rw-r--r--   0        0        0        0 2024-06-03 11:00:54.795224 delphai_fastapi-3.0.7/delphai_fastapi/job_posts/__init__.py
+-rw-r--r--   0        0        0     3201 2024-06-03 11:00:54.795224 delphai_fastapi-3.0.7/delphai_fastapi/job_posts/models.py
+-rw-r--r--   0        0        0     1386 2024-06-03 11:00:54.795224 delphai_fastapi-3.0.7/delphai_fastapi/models.py
+-rw-r--r--   0        0        0        0 2024-06-03 11:00:54.795224 delphai_fastapi-3.0.7/delphai_fastapi/news_articles/__init__.py
+-rw-r--r--   0        0        0     1120 2024-06-03 11:00:54.795224 delphai_fastapi-3.0.7/delphai_fastapi/news_articles/models.py
+-rw-r--r--   0        0        0        0 2024-06-03 11:00:54.795224 delphai_fastapi-3.0.7/delphai_fastapi/projects/__init__.py
+-rw-r--r--   0        0        0     1523 2024-06-03 11:00:54.795224 delphai_fastapi-3.0.7/delphai_fastapi/projects/models.py
+-rw-r--r--   0        0        0      405 2024-06-03 11:00:54.795224 delphai_fastapi-3.0.7/delphai_fastapi/server.py
+-rw-r--r--   0        0        0     3190 2024-06-03 11:00:54.795224 delphai_fastapi-3.0.7/delphai_fastapi/types.py
+-rw-r--r--   0        0        0      590 2024-06-03 11:00:54.795224 delphai_fastapi-3.0.7/pyproject.toml
+-rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 delphai_fastapi-3.0.7/PKG-INFO
```

### Comparing `delphai_fastapi-3.0.6/delphai_fastapi/app.py` & `delphai_fastapi-3.0.7/delphai_fastapi/app.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-3.0.6/delphai_fastapi/auth.py` & `delphai_fastapi-3.0.7/delphai_fastapi/auth.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-3.0.6/delphai_fastapi/companies/models.py` & `delphai_fastapi-3.0.7/delphai_fastapi/companies/models.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-3.0.6/delphai_fastapi/funding_rounds/models.py` & `delphai_fastapi-3.0.7/delphai_fastapi/funding_rounds/models.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-3.0.6/delphai_fastapi/instrumentation.py` & `delphai_fastapi-3.0.7/delphai_fastapi/instrumentation.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-3.0.6/delphai_fastapi/job_posts/models.py` & `delphai_fastapi-3.0.7/delphai_fastapi/job_posts/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 class AddJobPost(BaseJobPost):
     company_name: str = Field(
         ..., description="Name of the company posting the job post"
     )
     added_by: str = Field(
         ..., description="ID of the process or person this job post was added by"
     )
+    source: str = Field(..., description="Source of the job post")
     company_id: Optional[ObjectId] = Field(None, description="Internal company ID")
     original_description: Optional[str] = Field(
         None, description="Description in original language"
     )
     translated_description: Optional[str] = Field(
         None,
         description="Translated description in english. Only necessary if original language is not english",
```

### Comparing `delphai_fastapi-3.0.6/delphai_fastapi/models.py` & `delphai_fastapi-3.0.7/delphai_fastapi/models.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-3.0.6/delphai_fastapi/news_articles/models.py` & `delphai_fastapi-3.0.7/delphai_fastapi/news_articles/models.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-3.0.6/delphai_fastapi/projects/models.py` & `delphai_fastapi-3.0.7/delphai_fastapi/projects/models.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-3.0.6/delphai_fastapi/types.py` & `delphai_fastapi-3.0.7/delphai_fastapi/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,19 +15,22 @@
     ) -> CoreSchema:
         return core_schema.no_info_before_validator_function(
             cls.validate_objectid_string, handler(str)
         )
 
     @classmethod
     def validate_objectid_string(cls, v: Any) -> str:
-        if v is None:
-            raise InvalidId(
-                "None is not a valid ObjectId, it must be a 12-byte input or a 24-character hex string"
-            )
-        return str(BsonObjectId(v))
+        try:
+            if v is None:
+                raise InvalidId(
+                    "None is not a valid ObjectId, it must be a 12-byte input or a 24-character hex string"
+                )
+            return str(BsonObjectId(v))
+        except InvalidId as e:
+            raise ValueError(str(e))
 
     @classmethod
     def __get_pydantic_json_schema__(
         cls, core_schema: CoreSchema, handler: GetJsonSchemaHandler
     ) -> JsonSchemaValue:
         json_schema = handler(core_schema)
         json_schema = handler.resolve_ref_schema(json_schema)
```

### Comparing `delphai_fastapi-3.0.6/pyproject.toml` & `delphai_fastapi-3.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "delphai-fastapi"
-version = "3.0.6"
+version = "3.0.7"
 description = "Package for fastAPI models"
 authors = ["Berinike Tech <berinike@delphai.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 fastapi = "^0"
 pymongo = ">3"
```

### Comparing `delphai_fastapi-3.0.6/PKG-INFO` & `delphai_fastapi-3.0.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delphai-fastapi
-Version: 3.0.6
+Version: 3.0.7
 Summary: Package for fastAPI models
 Author: Berinike Tech
 Author-email: berinike@delphai.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

