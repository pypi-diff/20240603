# Comparing `tmp/kaiju_model-2.0.3-py3-none-any.whl.zip` & `tmp/kaiju_model-2.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 13147 bytes, number of entries: 12
--rw-r--r--  2.0 unx       94 b- defN 23-Jul-19 10:48 kaiju_model/__init__.py
--rw-r--r--  2.0 unx    21343 b- defN 23-Jul-19 10:48 kaiju_model/fields.py
--rw-r--r--  2.0 unx    18433 b- defN 23-Jul-19 10:48 kaiju_model/model.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 10:48 kaiju_model/grid/__init__.py
--rw-r--r--  2.0 unx      361 b- defN 23-Jul-19 10:48 kaiju_model/grid/base.py
--rw-r--r--  2.0 unx    10281 b- defN 23-Jul-19 10:48 kaiju_model/grid/constructor.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 10:48 kaiju_model/tests/__init__.py
--rw-rw-rw-  2.0 unx      610 b- defN 23-Jul-19 10:48 kaiju_model-2.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     2012 b- defN 23-Jul-19 10:48 kaiju_model-2.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-19 10:48 kaiju_model-2.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jul-19 10:48 kaiju_model-2.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      974 b- defN 23-Jul-19 10:48 kaiju_model-2.0.3.dist-info/RECORD
-12 files, 54212 bytes uncompressed, 11503 bytes compressed:  78.8%
+Zip file size: 13075 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       94 b- defN 24-Jun-03 13:54 kaiju_model/__init__.py
+-rw-r--r--  2.0 unx    20807 b- defN 24-Jun-03 13:43 kaiju_model/fields.py
+-rw-r--r--  2.0 unx    18529 b- defN 24-Jun-03 13:43 kaiju_model/model.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 13:43 kaiju_model/grid/__init__.py
+-rw-r--r--  2.0 unx      361 b- defN 24-Jun-03 13:43 kaiju_model/grid/base.py
+-rw-r--r--  2.0 unx    10281 b- defN 24-Jun-03 13:43 kaiju_model/grid/constructor.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 13:43 kaiju_model/tests/__init__.py
+-rw-r--r--  2.0 unx      610 b- defN 24-Jun-03 13:54 kaiju_model-2.2.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1968 b- defN 24-Jun-03 13:54 kaiju_model-2.2.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Jun-03 13:54 kaiju_model-2.2.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-Jun-03 13:54 kaiju_model-2.2.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      974 b- defN 24-Jun-03 13:54 kaiju_model-2.2.3.dist-info/RECORD
+12 files, 53728 bytes uncompressed, 11431 bytes compressed:  78.7%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: kaiju_model/grid/constructor.py
 Comment: 
 
 Filename: kaiju_model/tests/__init__.py
 Comment: 
 
-Filename: kaiju_model-2.0.3.dist-info/LICENSE
+Filename: kaiju_model-2.2.3.dist-info/LICENSE
 Comment: 
 
-Filename: kaiju_model-2.0.3.dist-info/METADATA
+Filename: kaiju_model-2.2.3.dist-info/METADATA
 Comment: 
 
-Filename: kaiju_model-2.0.3.dist-info/WHEEL
+Filename: kaiju_model-2.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: kaiju_model-2.0.3.dist-info/top_level.txt
+Filename: kaiju_model-2.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: kaiju_model-2.0.3.dist-info/RECORD
+Filename: kaiju_model-2.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kaiju_model/__init__.py

```diff
@@ -1,4 +1,4 @@
 __author__ = 'antonnidhoggr@me.com'
 __email__ = 'antonnidhoggr@me.com'
-__version__ = '2.0.3'
+__version__ = '2.2.3'
```

## kaiju_model/fields.py

```diff
@@ -40,33 +40,26 @@
         return cls._name
 
 
 class BaseField(abc.ABC, metaclass=_BaseFieldMeta):
     _name = None
 
     def __init__(
-        self,
-        required=False,
-        default=None,
-        disabled=False,
-        is_system=False,
-        group: str = None,
-        read_only=False,
-        grid_handler=None,
-        normalizer: Callable = None,
-        normalizer_es: Callable = None,
-        validator: Callable = None,
-        field_validator: Callable = None,
-        dependence: list = None,
-        nested=None,
-        label: str = None,
-        label_key: str = None,
-        helper_text: str = None,
-        helper_key: str = None,
-        view_condition: dict = None
+            self, required=False, default=None, disabled=False, is_system=False,
+            group: str = None,
+            read_only=False, grid_handler=None,
+            normalizer: Callable = None, normalizer_es: Callable = None,
+            validator: Callable = None, field_validator: Callable = None,
+            dependence: list = None,
+            nested: str = None,
+            label: str = None,
+            label_key: str = None,
+            helper_text: str = None,
+            helper_key: str = None,
+            view_condition: dict = None
     ):
         """
         :param required:
         :param default:
         :param disabled:
         :param read_only:
         :param grid_handler:
@@ -132,24 +125,24 @@
         pass
 
     def __iter__(self):
         return iter(self.repr().items())
 
     def repr(self):
         return {
-            'default': self.default,
-            'disabled': self.disabled,
-            'kind': self._name,
-            'required': self.required,
-            'dependence': self.dependence,
-            'label': self.label,
-            'label_key': self.label_key,
-            'view_condition': self.view_condition,
-            'helper_key': self.helper_key,
-            'helper_text': self.helper_text,
+            "default": self.default,
+            "disabled": self.disabled,
+            "kind": self._name,
+            "required": self.required,
+            "dependence": self.dependence,
+            "label": self.label,
+            "label_key": self.label_key,
+            "view_condition": self.view_condition,
+            "helper_key": self.helper_key,
+            "helper_text": self.helper_text,
         }
 
     @property
     def type(self):
         return self._name
 
     @staticmethod
@@ -161,54 +154,54 @@
     __slots__ = ('pattern', 'compiled', 'msg', '_repr')
 
     def __init__(self, pattern: str, msg: str = None):
         self.pattern = pattern
         self.compiled = re.compile(pattern)
         self.msg = msg
         self._repr = {
-            'pattern': self.pattern,
-            'msg': self.msg,
+            "pattern": self.pattern,
+            "msg": self.msg,
         }
 
     def __iter__(self):
         return iter(self.repr().items())
 
     def repr(self):
         return self._repr
 
 
 class StringField(BaseField):
-    _name = 'string'
+    _name = "string"
 
     def __init__(self, *args, regex=None, behavior=None, field_type=None, min: int = None, max: int = None,
                  **kwargs):
         super(StringField, self).__init__(*args, **kwargs)
         self.behavior = behavior
-        self.field_type = field_type  # 'password', 'email'
+        self.field_type = field_type  # "password", "email"
         self.min = min
         self.max = max
         if regex:
             self.regex = RegExp(*regex)
         else:
             self.regex = None
 
     def repr(self):
-        _r = super(StringField, self).repr()
+        _r = super().repr()
         _r.update({
-            'min': self.min,
-            'max': self.max,
+            "min": self.min,
+            "max": self.max,
         })
 
         if self.regex:
-            _r['regex'] = self.regex.repr()
+            _r["regex"] = self.regex.repr()
 
-        _r['behavior'] = self.behavior
+        _r["behavior"] = self.behavior
 
         if self.field_type:
-            _r['field_type'] = self.field_type
+            _r["field_type"] = self.field_type
 
         return _r
 
     @staticmethod
     def normalize(value, behavior=None, **_):
         try:
             if behavior == 'list':
@@ -219,58 +212,58 @@
 
             return str(value)
         except ValueError as exc:
             raise NormalizationError(str(exc))
 
 
 class TextField(StringField):
-    _name = 'text'
+    _name = "text"
 
     def __init__(self, *args, is_rich=None, **kwargs):
-        super(StringField, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self.is_rich = is_rich
 
     def repr(self):
-        _r = super(StringField, self).repr()
-        _r['is_rich'] = self.is_rich
+        _r = super().repr()
+        _r["is_rich"] = self.is_rich
         return _r
 
 
 class PasswordField(StringField):
-    _name = 'string'
+    _name = "string"
 
     def __init__(self, *args, new_password=False, **kwargs):
         super(StringField, self).__init__(*args, **kwargs)
         self.new_password = new_password  # field for new password or for old
 
     def repr(self):
         _r = super(StringField, self).repr()
-        _r['field_type'] = 'password'
-        _r['new_password'] = self.new_password
+        _r["field_type"] = "password"
+        _r["new_password"] = self.new_password
 
         return _r
 
 
 class BaseKeyField(StringField):
-    _name = 'key'
+    _name = "key"
 
 
 class BooleanField(BaseField):
-    _name = 'boolean'
+    _name = "boolean"
 
     @staticmethod
     def normalize(value, **_):
         try:
             return bool(value)
         except ValueError as exc:
             raise NormalizationError(str(exc))
 
 
 class IntegerField(BaseField):
-    _name = 'integer'
+    _name = "integer"
 
     def __init__(self, *args, negative_value=True, min: int = None, max: int = None, **kwargs):
         super(IntegerField, self).__init__(*args, **kwargs)
         self.negative_value = negative_value
         self.min = min
         self.max = max
 
@@ -279,35 +272,35 @@
         try:
             return int(value)
         except ValueError as exc:
             raise NormalizationError(str(exc))
 
     def repr(self):
         _repr = super(IntegerField, self).repr()
-        _repr['negative_value'] = self.negative_value
+        _repr["negative_value"] = self.negative_value
         _repr.update({
-            'min': self.min,
-            'max': self.max,
+            "min": self.min,
+            "max": self.max,
         })
         return _repr
 
 
 class DecimalField(IntegerField):
-    _name = 'decimal'
+    _name = "decimal"
 
     @staticmethod
     def normalize(value, **_):
         try:
             return decimal.Decimal(value)
         except (ValueError, decimal.InvalidOperation) as exc:
             raise NormalizationError(str(exc))
 
 
 class DateField(BaseField):
-    _name = 'date'
+    _name = "date"
 
     @staticmethod
     def normalize_base(value, **_):
         if isinstance(value, datetime.datetime):
             return value.date()
         elif isinstance(value, datetime.date):
             return value
@@ -329,15 +322,15 @@
 
     def __init__(self, *args, behavior=None, **kwargs):
         super(DateField, self).__init__(*args, **kwargs)
         self.behavior = behavior
 
     def repr(self):
         _r = super(DateField, self).repr()
-        _r['behavior'] = self.behavior
+        _r["behavior"] = self.behavior
 
         return _r
 
     def normalize(self, value, behavior=None, **_):
         try:
             if behavior == 'list':
                 if type(value) == list:
@@ -345,44 +338,47 @@
                     for _val in value:
                         res.append(self.normalize_base(_val))
                     return res
                 else:
                     return [self.normalize_base(value)]
             elif behavior == 'range':
                 if isinstance(value, dict):
-                    _min = value.get('min', None)
-                    _max = value.get('max', None)
-                    res = {'min': None, 'max': None}
+                    _min = value.get("min", None)
+                    _max = value.get("max", None)
+                    res = {
+                        "min": None,
+                        "max": None
+                    }
                     if _min:
-                        res['min'] = self.normalize_base(_min)
+                        res["min"] = self.normalize_base(_min)
                     if _max:
-                        res['max'] = self.normalize_base(_max)
+                        res["max"] = self.normalize_base(_max)
 
                 else:
                     return {
-                        'min': None,
-                        'max': None,
+                        "min": None,
+                        "max": None,
                     }
 
             return self.normalize_base(value)
         except ValueError as exc:
             raise NormalizationError(str(exc))
 
 
 class DateTimeField(BaseField):
-    _name = 'datetime'
+    _name = "datetime"
 
     def __init__(self, *args, behavior=None, **kwargs):
         super(DateTimeField, self).__init__(*args, **kwargs)
         self.behavior = behavior
 
     def repr(self):
         _r = super(DateTimeField, self).repr()
-        _r['behavior'] = self.behavior
-        _r['enable_time'] = True
+        _r["behavior"] = self.behavior
+        _r["enable_time"] = True
 
         return _r
 
     @staticmethod
     def normalize_base(value, **_):
         if isinstance(value, (datetime.datetime, datetime.date)):
             return value
@@ -400,26 +396,29 @@
                     for _val in value:
                         res.append(self.normalize_base(_val))
                     return res
                 else:
                     return [self.normalize_base(value)]
             elif behavior == 'range':
                 if isinstance(value, dict):
-                    _min = value.get('min', None)
-                    _max = value.get('max', None)
-                    res = {'min': None, 'max': None}
+                    _min = value.get("min", None)
+                    _max = value.get("max", None)
+                    res = {
+                        "min": None,
+                        "max": None
+                    }
                     if _min:
-                        res['min'] = self.normalize_base(_min)
+                        res["min"] = self.normalize_base(_min)
                     if _max:
-                        res['max'] = self.normalize_base(_max)
+                        res["max"] = self.normalize_base(_max)
 
                 else:
                     return {
-                        'min': None,
-                        'max': None,
+                        "min": None,
+                        "max": None,
                     }
 
             return self.normalize_base(value)
         except ValueError as exc:
             raise NormalizationError(str(exc))
 
     @staticmethod
@@ -430,111 +429,86 @@
             try:
                 return parser.parse(value, fuzzy=False).isoformat()
             except:
                 return value
 
 
 class SelectField(BaseField):
-    _name = 'select'
+    _name = "select"
 
-    def __init__(self, *args, options_handler=None, options_params=None, **kwargs):
-        super(SelectField, self).__init__(*args, **kwargs)
-        self.options_handler = options_handler
-        self.options_params = options_params
+    def __init__(self, options: list, *args, **kwargs):
+        """
+        options: [{"value": "1", "label": "Some label"}]
+        """
+        super().__init__(*args, **kwargs)
+        self.options = options
 
     @staticmethod
     def normalize(value, **_):
         return value
 
     def repr(self):
-        r = super(SelectField, self).repr()
-        r['options_handler'] = self.options_handler
-
-        if 'params' not in r:
-            r['params'] = self.options_params
-        else:
-            r['params'].update(**self.options_params)
-
+        r = super().repr()
+        r['options'] = self.options
         return r
 
 
 class MultiselectField(SelectField):
-    _name = 'multiselect'
+    _name = "multiselect"
 
     @staticmethod
     def normalize(value, **_):
         if isinstance(value, list):
             return value
 
         if not value:
             return []
 
         return [value]
 
-
 class TagField(MultiselectField):
-    _name = 'tag'
+    _name = "tag"
 
 
-class LookupSelectField(SelectField):
-    _name = 'lookup_select'
+class SelectAsyncField(BaseField):
+    _name = 'select_async'
+
+    def __init__(self, *args, options_handler=None, options_params=None, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.options_handler = options_handler
+        self.options_params = options_params
 
     @staticmethod
     def normalize(value, **_):
         return value
 
-
-class LookupMultiselectField(SelectField):
-    _name = 'lookup_multiselect'
-
-
-class ProductSelectField(SelectField):
-    _name = 'product_select'
-
-
-class ProductMultiselectField(SelectField):
-    _name = 'product_multiselect'
-
-
-class MetricField(BaseField):
-    _name = 'metric'
-
-    def __init__(self, *args, family=None, options_handler=None, **kwargs):
-        super(MetricField, self).__init__(*args, **kwargs)
-        self.family = family
-        self.options_handler = options_handler
-
     def repr(self):
-        r = super(MetricField, self).repr()
-        r['family'] = self.family
+        r = super().repr()
         r['options_handler'] = self.options_handler
+
+        if 'params' not in r:
+            r['params'] = self.options_params
+        else:
+            r['params'].update(**self.options_params)
+
         return r
 
-    # @staticmethod
-    # def normalize_es(value):
-    #     if isinstance(value, (datetime.datetime, datetime.date)):
-    #         return value.strftime('%Y-%m-%dT%H:%M:%S')
-    #     else:
-    #         return value
+
+class MultiSelectAsyncField(SelectAsyncField):
+    _name = 'multiselect_async'
 
     @staticmethod
     def normalize(value, **_):
-        if isinstance(value, dict):
-            if not value.get('value'):
-                return {}
+        if isinstance(value, list):
             return value
 
         if not value:
-            return {}
-
-        return value
-
+            return []
 
-class CurrencyField(MetricField):
-    _name = 'currency'
+        return [value]
 
 
 class VideoField(BaseField):
     _name = 'video'
 
     def __init__(self, limit=None, max_number_of_files=6, *args, **kwargs):
         super(VideoField, self).__init__(*args, **kwargs)
@@ -550,23 +524,23 @@
         return repr
 
 
 class DocumentField(BaseField):
     _name = 'document'
 
     def __init__(
-        self,
-        limit=None,
-        upload_path=None,
-        max_size_mb=1024,
-        auto_proceed=False,
-        allowed_types=None,
-        max_number_of_files=6,
-        *args,
-        **kwargs,
+            self,
+            limit=None,
+            upload_path=None,
+            max_size_mb=1024,
+            auto_proceed=False,
+            allowed_types=None,
+            max_number_of_files=6,
+            *args,
+            **kwargs,
     ):
         super(DocumentField, self).__init__(*args, **kwargs)
         self.limit = limit
         self.upload_path = upload_path
         self.max_size_mb = max_size_mb
         self.auto_proceed = auto_proceed
         self.allowed_types = allowed_types
@@ -705,15 +679,15 @@
 
 SimpleIdField = partial(
     StringField,
     read_only=True,
     required=True,
     validator=_f_empty_value,
     normalizer=normalizer_value,
-    regex=(r'^[a-z0-9_]+$', 'Regex.key'),
+    regex=(r'^[a-zA-Z0-9_]+$', 'Regex.key'),
 )
 
 IdField = partial(
     StringField,
     read_only=True,
     required=True,
     validator=_f_empty_value,
@@ -726,83 +700,83 @@
 )
 
 
 class MediaFileField(DocumentField):
     _name = 'media_file'
 
 
-class MediaMultiselectField(SelectField):
+class MediaMultiselectASyncField(SelectAsyncField):
     _name = 'media_multiselect'
 
     def compare(self, val1, val2):
         if val1 is not None:
             val1.sort()
 
         if val2 is not None:
             val2.sort()
 
         return val1 == val2
 
 
-class MediaField(SelectField):
+class MediaField(SelectAsyncField):
     _name = 'media'
 
     def compare(self, val1, val2):
         if val1 is not None:
             val1.sort()
 
         if val2 is not None:
             val2.sort()
 
         return val1 == val2
 
 
 class NestedField(BaseField):
-    _name = 'nested'
+    _name = "nested"
 
     def __init__(self, *args, **kwargs):
         self._fields = []
         self.init_fields(kwargs)
-        super(NestedField).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
     def init_fields(self, fields: dict):
         for k, field in list(fields.items()):
             if isinstance(field, BaseField):
                 fields.pop(k)
                 self._fields.append({
-                    'id': k,
+                    "id": k,
                     **field.repr()
                 })
 
     def repr(self):
         _r = super().repr()
-        _r['fields'] = self._fields
+        _r["fields"] = self._fields
         return _r
 
     @staticmethod
     def normalize(value, **_):
         # TODO NEED FIELD NOMALIZER
 
         return value
 
 
 class NestedListField(NestedField):
-    _name = 'nested_list'
+    _name = "nested_list"
 
     def normalize(self, value, **_):
         # TODO NEED FIELD NORMALIZER
         return value
 
 
 class TextBlock(BaseField):
-    _name = 'text_block'
+    _name = "text_block"
 
     def __init__(self, *args, text: str = None, text_key: str = None, **kwargs):
-        super(TextBlock).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self.text = text
         self.text_key = text_key
 
     def repr(self):
-        _r = super(TextBlock).repr()
-        _r['text'] = self.text
-        _r['text_key'] = self.text_key
+        _r = super().repr()
+        _r["text"] = self.text
+        _r["text_key"] = self.text_key
         return _r
```

## kaiju_model/model.py

```diff
@@ -330,23 +330,22 @@
         if type(exclude) is not set:
             exclude = set()
 
         base = {
             'id': FieldGroups.BASE.value,
             'fields': [
                 {'id': name, **field.repr(), **default_values.get(name, {})}
-                for name, field in cls._base_fields.items()
-                if not field.is_system and name not in exclude
+                for name, field in cls._base_fields.items() if not field.is_system and name not in exclude
             ]
         }
 
         optional = {}
 
         for name, field in cls._optional_fields.items():
-            if not field.is_system and name not in exclude:
+            if not field.is_system:
                 data = {'id': name, **field.repr(), **default_values.get(name, {})}
 
                 if field.group in optional:
                     optional[field.group].append(data)
                 else:
                     optional[field.group] = [data]
 
@@ -512,17 +511,24 @@
     @property
     def fields(self):
         """Returns attribute fields spec."""
 
         base = {
             'id': FieldGroups.BASE.value,
             'fields': [
-                {'id': name, "value": self.params.get(name), **field.repr(), **self.modify(name, field), "disabled": self._fields[name].read_only}
-                for name, field in self._base_fields.items() if not field.is_system
-            ]
+                {
+                    'id': name,
+                    'value': self.params.get(name),
+                    **field.repr(),
+                    **self.modify(name, field),
+                    'disabled': self._fields[name].read_only,
+                }
+                for name, field in self._base_fields.items()
+                if not field.is_system
+            ],
         }
 
         optional = {}
 
         for name, field in self._optional_fields.items():
             _modify = self.modify(name, field)
             if not _modify.get('is_system', field.is_system):
```

## Comparing `kaiju_model-2.0.3.dist-info/LICENSE` & `kaiju_model-2.2.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kaiju_model-2.0.3.dist-info/METADATA` & `kaiju_model-2.2.3.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: kaiju-model
-Version: 2.0.3
+Name: kaiju_model
+Version: 2.2.3
 Summary: Web interface related classes.
 Home-page: https://gitlab.com/kaiju-python/kaiju-model
 Author: antonnidhoggr@me.com
 Author-email: antonnidhoggr@me.com
 License: Apache Software License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
@@ -14,33 +14,33 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: python-dateutil (>=2.8.2)
-Requires-Dist: kaiju-tools (<3,>=2)
+Requires-Dist: python-dateutil >=2.8.2
+Requires-Dist: kaiju-tools <3,>=2
 Provides-Extra: dev
-Requires-Dist: bump2version (>=1.0) ; extra == 'dev'
-Requires-Dist: pyroma (>=4.1) ; extra == 'dev'
-Requires-Dist: bandit (>=1.7) ; extra == 'dev'
-Requires-Dist: black (>=22.12) ; extra == 'dev'
-Requires-Dist: flake8 (>=6.0) ; extra == 'dev'
+Requires-Dist: bump2version >=1.0 ; extra == 'dev'
+Requires-Dist: pyroma >=4.1 ; extra == 'dev'
+Requires-Dist: bandit >=1.7 ; extra == 'dev'
+Requires-Dist: black >=22.12 ; extra == 'dev'
+Requires-Dist: flake8 >=6.0 ; extra == 'dev'
 Requires-Dist: pyproject-flake8 ; extra == 'dev'
-Requires-Dist: pre-commit (>=3.1) ; extra == 'dev'
-Requires-Dist: pydocstyle (>=6.2) ; extra == 'dev'
-Requires-Dist: setup-cfg-fmt (>=2.2) ; extra == 'dev'
-Requires-Dist: restructuredtext-lint (>=1.4) ; extra == 'dev'
-Requires-Dist: tox (>=3.28) ; extra == 'dev'
-Requires-Dist: tox-pyenv (>=1.1) ; extra == 'dev'
-Requires-Dist: pip-tools (>=6.13) ; extra == 'dev'
-Requires-Dist: pyupgrade (>=3.4) ; extra == 'dev'
-Requires-Dist: towncrier (>=23.6) ; extra == 'dev'
+Requires-Dist: pre-commit >=3.1 ; extra == 'dev'
+Requires-Dist: pydocstyle >=6.2 ; extra == 'dev'
+Requires-Dist: setup-cfg-fmt >=2.2 ; extra == 'dev'
+Requires-Dist: restructuredtext-lint >=1.4 ; extra == 'dev'
+Requires-Dist: tox >=3.28 ; extra == 'dev'
+Requires-Dist: tox-pyenv >=1.1 ; extra == 'dev'
+Requires-Dist: pip-tools >=6.13 ; extra == 'dev'
+Requires-Dist: pyupgrade >=3.4 ; extra == 'dev'
+Requires-Dist: towncrier >=23.6 ; extra == 'dev'
 Provides-Extra: test
-Requires-Dist: pytest (>=7.2) ; extra == 'test'
-Requires-Dist: pytest-asyncio (>=0.20) ; extra == 'test'
-Requires-Dist: docker (>=6.0) ; extra == 'test'
-Requires-Dist: pytest-timeout (>=2.1) ; extra == 'test'
-Requires-Dist: pytest-aiohttp (>=1.0) ; extra == 'test'
-Requires-Dist: pytest-cov (>=4.1.0) ; extra == 'test'
+Requires-Dist: pytest >=7.2 ; extra == 'test'
+Requires-Dist: pytest-asyncio >=0.20 ; extra == 'test'
+Requires-Dist: docker >=6.0 ; extra == 'test'
+Requires-Dist: pytest-timeout >=2.1 ; extra == 'test'
+Requires-Dist: pytest-aiohttp >=1.0 ; extra == 'test'
+Requires-Dist: pytest-cov >=4.1.0 ; extra == 'test'
```

## Comparing `kaiju_model-2.0.3.dist-info/RECORD` & `kaiju_model-2.2.3.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-kaiju_model/__init__.py,sha256=S8fabmHBIhc1vIb1axXUW4ToBnCSxlUEF4875FIi47A,94
-kaiju_model/fields.py,sha256=NKcbM3EJGZdSZIMr2gkFQzIHJfHlgdiyIvZ5tg8Ov8M,21343
-kaiju_model/model.py,sha256=GjaXAC797LNrtVD-CXB6O7G2ng05fScrkf3E90SC5II,18433
+kaiju_model/__init__.py,sha256=NRoMrsSd8_VSSpb31AboocoTNpwo-yoai_m8Es3sR3Y,94
+kaiju_model/fields.py,sha256=mk-bZykzn-Qp0DQzrk9GE566XAJ05nyjOWCdrrRA22Q,20807
+kaiju_model/model.py,sha256=ca1ccILsSmpo8vBp-hOpOEjVRzfqeIt7MSJsnD3ngRg,18529
 kaiju_model/grid/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kaiju_model/grid/base.py,sha256=-RxkDq__VSR5w_yXCpa74LNAj-4BNr8NVheKae0rjUE,361
 kaiju_model/grid/constructor.py,sha256=e8m37QUuUxA_drXaFkXhtwBj7iVsQcoF2jr4t_H1WNY,10281
 kaiju_model/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-kaiju_model-2.0.3.dist-info/LICENSE,sha256=XIlN2qA8UqpBDA-PteoYP4hTU0qBW0G9PRB__khO2zc,610
-kaiju_model-2.0.3.dist-info/METADATA,sha256=9fjjTa7lgvl-ULiULKzp2NvzvKoClV0fxp9WEeiPgNo,2012
-kaiju_model-2.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-kaiju_model-2.0.3.dist-info/top_level.txt,sha256=3lm68s9XtN4zbuKIVlAbnzbqzxqSplKrNmLX6s2CD-Y,12
-kaiju_model-2.0.3.dist-info/RECORD,,
+kaiju_model-2.2.3.dist-info/LICENSE,sha256=XIlN2qA8UqpBDA-PteoYP4hTU0qBW0G9PRB__khO2zc,610
+kaiju_model-2.2.3.dist-info/METADATA,sha256=hnV2HkZJAZERsa_r61iKHqa6iJSWn7oPDQh5BEKKQZw,1968
+kaiju_model-2.2.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+kaiju_model-2.2.3.dist-info/top_level.txt,sha256=3lm68s9XtN4zbuKIVlAbnzbqzxqSplKrNmLX6s2CD-Y,12
+kaiju_model-2.2.3.dist-info/RECORD,,
```

