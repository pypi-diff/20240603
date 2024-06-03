# Comparing `tmp/feincms3-5.0a1.tar.gz` & `tmp/feincms3-5.0a2.tar.gz`

## Comparing `feincms3-5.0a1.tar` & `feincms3-5.0a2.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/__init__.py
--rw-r--r--   0        0        0    22857 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/admin.py
--rw-r--r--   0        0        0    23996 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/applications.py
--rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/cleanse.py
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/embedding.py
--rw-r--r--   0        0        0     6057 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/inline_ckeditor.py
--rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/mixins.py
--rw-r--r--   0        0        0     9935 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/pages.py
--rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/regions.py
--rw-r--r--   0        0        0    13486 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/renderer.py
--rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/shortcuts.py
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/utils.py
--rw-r--r--   0        0        0     6228 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     8609 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9293 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7904 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     8912 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/plugins/__init__.py
--rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/plugins/external.py
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/plugins/html.py
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/plugins/image.py
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/plugins/old_richtext.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/plugins/richtext.py
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/plugins/snippet.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/root/__init__.py
--rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/root/middleware.py
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/root/passthru.py
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/static/feincms3/admin.css
--rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/static/feincms3/admin.js
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/static/feincms3/inline-ckeditor-contents.css
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/static/feincms3/inline-ckeditor.css
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/static/feincms3/inline-ckeditor.js
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/static/feincms3/plugin-ckeditor.css
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/static/feincms3/static-path-style.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/templatetags/__init__.py
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/templatetags/feincms3.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 feincms3-5.0a1/.gitignore
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 feincms3-5.0a1/LICENSE
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 feincms3-5.0a1/README.rst
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 feincms3-5.0a1/pyproject.toml
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 feincms3-5.0a1/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/__init__.py
+-rw-r--r--   0        0        0    22936 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/admin.py
+-rw-r--r--   0        0        0    23996 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/applications.py
+-rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/cleanse.py
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/embedding.py
+-rw-r--r--   0        0        0     6057 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/inline_ckeditor.py
+-rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/mixins.py
+-rw-r--r--   0        0        0    10066 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/pages.py
+-rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/regions.py
+-rw-r--r--   0        0        0    13486 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/renderer.py
+-rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/shortcuts.py
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/utils.py
+-rw-r--r--   0        0        0     6222 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     8603 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9293 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7904 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     8912 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/plugins/__init__.py
+-rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/plugins/external.py
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/plugins/html.py
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/plugins/image.py
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/plugins/old_richtext.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/plugins/richtext.py
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/plugins/snippet.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/root/__init__.py
+-rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/root/middleware.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/root/passthru.py
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/static/feincms3/admin.css
+-rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/static/feincms3/admin.js
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/static/feincms3/inline-ckeditor-contents.css
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/static/feincms3/inline-ckeditor.css
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/static/feincms3/inline-ckeditor.js
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/static/feincms3/move-form.css
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/static/feincms3/plugin-ckeditor.css
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/static/feincms3/static-path-style.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/templatetags/__init__.py
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 feincms3-5.0a2/feincms3/templatetags/feincms3.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 feincms3-5.0a2/.gitignore
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 feincms3-5.0a2/LICENSE
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 feincms3-5.0a2/README.rst
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 feincms3-5.0a2/pyproject.toml
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 feincms3-5.0a2/PKG-INFO
```

### Comparing `feincms3-5.0a1/feincms3/admin.py` & `feincms3-5.0a2/feincms3/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,18 +277,18 @@
         move = self.cleaned_data["move"]
         relative_to = self.cleaned_data["relative_to"]
         position = self.cleaned_data["position"]
 
         print(self.cleaned_data)
 
         if position in {"first-child", "last-child"}:
-            move.parent = relative_to
+            move._set_parent(relative_to)
             siblings_qs = relative_to.children
         else:
-            move.parent = relative_to.parent
+            move._set_parent(relative_to.parent)
             siblings_qs = relative_to.__class__._default_manager.filter(
                 parent=relative_to.parent
             )
 
         try:
             # All fields of model are not in this form
             move.full_clean(exclude=[f.name for f in move._meta.get_fields()])
@@ -337,14 +337,17 @@
     """
     Allows making the node the left or right sibling or the first or last
     child of another node.
 
     Requires the node to be moved as ``obj`` keyword argument.
     """
 
+    class Media:
+        css = {"screen": ["feincms3/move-form.css"]}
+
     def __init__(self, *args, **kwargs):
         self.instance = kwargs.pop("obj")
         self.modeladmin = kwargs.pop("modeladmin")
         self.request = kwargs.pop("request")
         self.model = self.instance.__class__
 
         super().__init__(*args, **kwargs)
```

### Comparing `feincms3-5.0a1/feincms3/applications.py` & `feincms3-5.0a2/feincms3/applications.py`

 * *Files identical despite different names*

### Comparing `feincms3-5.0a1/feincms3/cleanse.py` & `feincms3-5.0a2/feincms3/cleanse.py`

 * *Files identical despite different names*

### Comparing `feincms3-5.0a1/feincms3/embedding.py` & `feincms3-5.0a2/feincms3/embedding.py`

 * *Files identical despite different names*

### Comparing `feincms3-5.0a1/feincms3/inline_ckeditor.py` & `feincms3-5.0a2/feincms3/inline_ckeditor.py`

 * *Files identical despite different names*

### Comparing `feincms3-5.0a1/feincms3/mixins.py` & `feincms3-5.0a2/feincms3/mixins.py`

 * *Files identical despite different names*

### Comparing `feincms3-5.0a1/feincms3/pages.py` & `feincms3-5.0a2/feincms3/pages.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,14 +142,18 @@
 
             # Descendants of inactive nodes cannot be active themselves:
             if not node.parent.is_active:
                 node.is_active = False
             nodes[node.id] = node
         return nodes
 
+    def _set_parent(self, parent):
+        # Hook used in feincms3-sites and feincms3-language-sites
+        self.parent = parent
+
     def _clash_candidates(self):
         # Hook used in feincms3-sites and feincms3-language-sites
         return self.__class__._default_manager
 
     def _path_clash_candidates(self):
         return self._clash_candidates().exclude(
             Q(pk__in=self.descendants(), static_path=False) | Q(pk=self.pk)
```

### Comparing `feincms3-5.0a1/feincms3/regions.py` & `feincms3-5.0a2/feincms3/regions.py`

 * *Files identical despite different names*

### Comparing `feincms3-5.0a1/feincms3/renderer.py` & `feincms3-5.0a2/feincms3/renderer.py`

 * *Files identical despite different names*

### Comparing `feincms3-5.0a1/feincms3/shortcuts.py` & `feincms3-5.0a2/feincms3/shortcuts.py`

 * *Files identical despite different names*

### Comparing `feincms3-5.0a1/feincms3/utils.py` & `feincms3-5.0a2/feincms3/utils.py`

 * *Files identical despite different names*

### Comparing `feincms3-5.0a1/feincms3/locale/de/LC_MESSAGES/django.mo` & `feincms3-5.0a2/feincms3/locale/de/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -72,15 +72,15 @@
 "Verschieben ist nicht möglich weil es keine gültigen Zielorte gibt. "
 "Vielleicht den einzigen Wurzelknoten gewählt?"
 
 msgid "New location"
 msgstr "Neuer Ort"
 
 msgid "Node '{}' has been moved to its new position."
-msgstr "'%(node)s' wurde zur neuen Position verschoben."
+msgstr "'{}' wurde zur neuen Position verschoben."
 
 msgid ""
 "Objects in the primary language cannot be the translation of another object."
 msgstr ""
 "Objekte in der primären Sprache können nicht eine Übersetzung eines anderen "
 "Objektes sein."
```

### Comparing `feincms3-5.0a1/feincms3/locale/de/LC_MESSAGES/django.po` & `feincms3-5.0a2/feincms3/locale/de/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
 #: admin.py:296
 msgid "Error while validating the new position of '{}'."
 msgstr "Fehler beim Validieren der neuen Position von '{}'."
 
 #: admin.py:327
 msgid "Node '{}' has been moved to its new position."
-msgstr "'%(node)s' wurde zur neuen Position verschoben."
+msgstr "'{}' wurde zur neuen Position verschoben."
 
 #: admin.py:352
 msgid "New location"
 msgstr "Neuer Ort"
 
 #: admin.py:360
 msgid ""
```

### Comparing `feincms3-5.0a1/feincms3/locale/en/LC_MESSAGES/django.po` & `feincms3-5.0a2/feincms3/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3-5.0a1/feincms3/locale/fr/LC_MESSAGES/django.mo` & `feincms3-5.0a2/feincms3/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3-5.0a1/feincms3/locale/fr/LC_MESSAGES/django.po` & `feincms3-5.0a2/feincms3/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3-5.0a1/feincms3/locale/it/LC_MESSAGES/django.mo` & `feincms3-5.0a2/feincms3/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3-5.0a1/feincms3/locale/it/LC_MESSAGES/django.po` & `feincms3-5.0a2/feincms3/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3-5.0a1/feincms3/locale/nb_NO/LC_MESSAGES/django.mo` & `feincms3-5.0a2/feincms3/locale/nb_NO/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3-5.0a1/feincms3/locale/nb_NO/LC_MESSAGES/django.po` & `feincms3-5.0a2/feincms3/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3-5.0a1/feincms3/plugins/__init__.py` & `feincms3-5.0a2/feincms3/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `feincms3-5.0a1/feincms3/plugins/external.py` & `feincms3-5.0a2/feincms3/plugins/external.py`

 * *Files identical despite different names*

### Comparing `feincms3-5.0a1/feincms3/plugins/html.py` & `feincms3-5.0a2/feincms3/plugins/html.py`

 * *Files identical despite different names*

### Comparing `feincms3-5.0a1/feincms3/plugins/image.py` & `feincms3-5.0a2/feincms3/plugins/image.py`

 * *Files identical despite different names*

### Comparing `feincms3-5.0a1/feincms3/plugins/old_richtext.py` & `feincms3-5.0a2/feincms3/plugins/old_richtext.py`

 * *Files identical despite different names*

### Comparing `feincms3-5.0a1/feincms3/plugins/richtext.py` & `feincms3-5.0a2/feincms3/plugins/richtext.py`

 * *Files identical despite different names*

### Comparing `feincms3-5.0a1/feincms3/plugins/snippet.py` & `feincms3-5.0a2/feincms3/plugins/snippet.py`

 * *Files identical despite different names*

### Comparing `feincms3-5.0a1/feincms3/root/middleware.py` & `feincms3-5.0a2/feincms3/root/middleware.py`

 * *Files identical despite different names*

### Comparing `feincms3-5.0a1/feincms3/root/passthru.py` & `feincms3-5.0a2/feincms3/root/passthru.py`

 * *Files identical despite different names*

### Comparing `feincms3-5.0a1/feincms3/static/feincms3/admin.css` & `feincms3-5.0a2/feincms3/static/feincms3/admin.css`

 * *Files identical despite different names*

### Comparing `feincms3-5.0a1/feincms3/static/feincms3/admin.js` & `feincms3-5.0a2/feincms3/static/feincms3/admin.js`

 * *Files identical despite different names*

### Comparing `feincms3-5.0a1/feincms3/static/feincms3/inline-ckeditor.css` & `feincms3-5.0a2/feincms3/static/feincms3/inline-ckeditor.css`

 * *Files identical despite different names*

### Comparing `feincms3-5.0a1/feincms3/static/feincms3/inline-ckeditor.js` & `feincms3-5.0a2/feincms3/static/feincms3/inline-ckeditor.js`

 * *Files identical despite different names*

### Comparing `feincms3-5.0a1/feincms3/static/feincms3/static-path-style.js` & `feincms3-5.0a2/feincms3/static/feincms3/static-path-style.js`

 * *Files identical despite different names*

### Comparing `feincms3-5.0a1/feincms3/templatetags/feincms3.py` & `feincms3-5.0a2/feincms3/templatetags/feincms3.py`

 * *Files identical despite different names*

### Comparing `feincms3-5.0a1/LICENSE` & `feincms3-5.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `feincms3-5.0a1/README.rst` & `feincms3-5.0a2/README.rst`

 * *Files identical despite different names*

### Comparing `feincms3-5.0a1/pyproject.toml` & `feincms3-5.0a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `feincms3-5.0a1/PKG-INFO` & `feincms3-5.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: feincms3
-Version: 5.0a1
+Version: 5.0a2
 Summary: CMS-building toolkit for Django
 Project-URL: Homepage, https://github.com/matthiask/feincms3/
 Author-email: Matthias Kestenholz <mk@feinheit.ch>
 License: BSD-3-Clause
 License-File: LICENSE
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

