# Comparing `tmp/ipyslides-3.9.9.tar.gz` & `tmp/ipyslides-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyslides-3.9.9.tar", last modified: Sat Jun  1 21:05:20 2024, max compression
+gzip compressed data, was "ipyslides-4.0.0.tar", last modified: Sun Jun  2 18:37:53 2024, max compression
```

## Comparing `ipyslides-3.9.9.tar` & `ipyslides-4.0.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 21:05:20.586967 ipyslides-3.9.9/
--rw-rw-rw-   0        0        0     1090 2023-02-22 21:18:51.000000 ipyslides-3.9.9/LICENSE
--rw-rw-rw-   0        0        0     5273 2024-06-01 21:05:20.583478 ipyslides-3.9.9/PKG-INFO
--rw-rw-rw-   0        0        0     4384 2024-06-01 21:03:10.000000 ipyslides-3.9.9/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 21:05:20.483573 ipyslides-3.9.9/ipyslides/
--rw-rw-rw-   0        0        0      394 2024-03-14 11:52:17.000000 ipyslides-3.9.9/ipyslides/__init__.py
--rw-rw-rw-   0        0        0       25 2024-06-01 20:52:13.000000 ipyslides-3.9.9/ipyslides/__version__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 21:05:20.576357 ipyslides-3.9.9/ipyslides/_base/
--rw-rw-rw-   0        0        0      283 2023-02-22 21:18:52.000000 ipyslides-3.9.9/ipyslides/_base/__init__.py
--rw-rw-rw-   0        0        0    40933 2024-06-01 20:56:10.000000 ipyslides-3.9.9/ipyslides/_base/_layout_css.py
--rw-rw-rw-   0        0        0     6170 2024-05-28 17:17:01.000000 ipyslides-3.9.9/ipyslides/_base/_widgets.py
--rw-rw-rw-   0        0        0    32648 2024-06-01 20:54:40.000000 ipyslides-3.9.9/ipyslides/_base/base.py
--rw-rw-rw-   0        0        0     7555 2024-05-29 17:23:33.000000 ipyslides-3.9.9/ipyslides/_base/export_html.py
--rw-rw-rw-   0        0        0     6606 2024-05-10 05:07:47.000000 ipyslides-3.9.9/ipyslides/_base/export_template.py
--rw-rw-rw-   0        0        0    12175 2024-05-10 05:35:36.000000 ipyslides-3.9.9/ipyslides/_base/icons.py
--rw-rw-rw-   0        0        0     7689 2024-05-30 18:07:59.000000 ipyslides-3.9.9/ipyslides/_base/intro.py
-drwxrwxrwx   0        0        0        0 2024-06-01 21:05:20.578362 ipyslides-3.9.9/ipyslides/_base/js/
--rw-rw-rw-   0        0        0    11354 2024-05-30 18:06:53.000000 ipyslides-3.9.9/ipyslides/_base/js/interaction.js
--rw-rw-rw-   0        0        0     1874 2024-05-28 17:40:55.000000 ipyslides-3.9.9/ipyslides/_base/js/notes.js
--rw-rw-rw-   0        0        0     3563 2024-05-18 22:39:26.000000 ipyslides-3.9.9/ipyslides/_base/navigation.py
--rw-rw-rw-   0        0        0     2616 2024-06-01 18:25:46.000000 ipyslides-3.9.9/ipyslides/_base/notes.py
--rw-rw-rw-   0        0        0    11995 2024-06-01 20:27:13.000000 ipyslides-3.9.9/ipyslides/_base/screenshot.py
--rw-rw-rw-   0        0        0    23214 2024-06-01 19:11:51.000000 ipyslides-3.9.9/ipyslides/_base/settings.py
--rw-rw-rw-   0        0        0    27096 2024-06-01 20:01:52.000000 ipyslides-3.9.9/ipyslides/_base/slide.py
--rw-rw-rw-   0        0        0    28407 2024-05-19 17:34:36.000000 ipyslides-3.9.9/ipyslides/_base/styles.py
--rw-rw-rw-   0        0        0    16171 2024-06-01 20:22:44.000000 ipyslides-3.9.9/ipyslides/_base/widgets.py
--rw-rw-rw-   0        0        0    12534 2024-06-01 20:52:21.000000 ipyslides-3.9.9/ipyslides/_demo.py
--rw-rw-rw-   0        0        0    46692 2024-06-01 20:07:57.000000 ipyslides-3.9.9/ipyslides/core.py
--rw-rw-rw-   0        0        0    18527 2024-05-08 17:02:50.000000 ipyslides-3.9.9/ipyslides/formatters.py
--rw-rw-rw-   0        0        0     8776 2024-06-01 18:12:25.000000 ipyslides-3.9.9/ipyslides/source.py
--rw-rw-rw-   0        0        0    29785 2024-06-01 20:26:23.000000 ipyslides-3.9.9/ipyslides/utils.py
--rw-rw-rw-   0        0        0    14549 2024-06-01 18:28:02.000000 ipyslides-3.9.9/ipyslides/writer.py
--rw-rw-rw-   0        0        0    28897 2024-06-01 18:27:10.000000 ipyslides-3.9.9/ipyslides/xmd.py
-drwxrwxrwx   0        0        0        0 2024-06-01 21:05:20.548353 ipyslides-3.9.9/ipyslides.egg-info/
--rw-rw-rw-   0        0        0     5273 2024-06-01 21:05:19.000000 ipyslides-3.9.9/ipyslides.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      854 2024-06-01 21:05:19.000000 ipyslides-3.9.9/ipyslides.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 21:05:19.000000 ipyslides-3.9.9/ipyslides.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      134 2024-06-01 21:05:19.000000 ipyslides-3.9.9/ipyslides.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-06-01 21:05:19.000000 ipyslides-3.9.9/ipyslides.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 21:05:20.586967 ipyslides-3.9.9/setup.cfg
--rw-rw-rw-   0        0        0     3730 2023-12-09 17:54:29.000000 ipyslides-3.9.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 18:37:53.592254 ipyslides-4.0.0/
+-rw-rw-rw-   0        0        0     1090 2023-02-22 21:18:51.000000 ipyslides-4.0.0/LICENSE
+-rw-rw-rw-   0        0        0     5273 2024-06-02 18:37:53.590789 ipyslides-4.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4384 2024-06-01 21:03:10.000000 ipyslides-4.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 18:37:53.522675 ipyslides-4.0.0/ipyslides/
+-rw-rw-rw-   0        0        0      394 2024-03-14 11:52:17.000000 ipyslides-4.0.0/ipyslides/__init__.py
+-rw-rw-rw-   0        0        0       25 2024-06-02 18:36:49.000000 ipyslides-4.0.0/ipyslides/__version__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 18:37:53.585742 ipyslides-4.0.0/ipyslides/_base/
+-rw-rw-rw-   0        0        0      283 2023-02-22 21:18:52.000000 ipyslides-4.0.0/ipyslides/_base/__init__.py
+-rw-rw-rw-   0        0        0    41124 2024-06-02 05:16:29.000000 ipyslides-4.0.0/ipyslides/_base/_layout_css.py
+-rw-rw-rw-   0        0        0     6170 2024-05-28 17:17:01.000000 ipyslides-4.0.0/ipyslides/_base/_widgets.py
+-rw-rw-rw-   0        0        0    32676 2024-06-02 18:25:17.000000 ipyslides-4.0.0/ipyslides/_base/base.py
+-rw-rw-rw-   0        0        0     7555 2024-05-29 17:23:33.000000 ipyslides-4.0.0/ipyslides/_base/export_html.py
+-rw-rw-rw-   0        0        0     6606 2024-05-10 05:07:47.000000 ipyslides-4.0.0/ipyslides/_base/export_template.py
+-rw-rw-rw-   0        0        0    12175 2024-05-10 05:35:36.000000 ipyslides-4.0.0/ipyslides/_base/icons.py
+-rw-rw-rw-   0        0        0     7689 2024-05-30 18:07:59.000000 ipyslides-4.0.0/ipyslides/_base/intro.py
+drwxrwxrwx   0        0        0        0 2024-06-02 18:37:53.588741 ipyslides-4.0.0/ipyslides/_base/js/
+-rw-rw-rw-   0        0        0    11354 2024-05-30 18:06:53.000000 ipyslides-4.0.0/ipyslides/_base/js/interaction.js
+-rw-rw-rw-   0        0        0     1874 2024-05-28 17:40:55.000000 ipyslides-4.0.0/ipyslides/_base/js/notes.js
+-rw-rw-rw-   0        0        0     3563 2024-05-18 22:39:26.000000 ipyslides-4.0.0/ipyslides/_base/navigation.py
+-rw-rw-rw-   0        0        0     2616 2024-06-01 18:25:46.000000 ipyslides-4.0.0/ipyslides/_base/notes.py
+-rw-rw-rw-   0        0        0    11978 2024-06-02 05:10:04.000000 ipyslides-4.0.0/ipyslides/_base/screenshot.py
+-rw-rw-rw-   0        0        0    23214 2024-06-01 19:11:51.000000 ipyslides-4.0.0/ipyslides/_base/settings.py
+-rw-rw-rw-   0        0        0    27096 2024-06-02 00:18:00.000000 ipyslides-4.0.0/ipyslides/_base/slide.py
+-rw-rw-rw-   0        0        0    28334 2024-06-02 17:43:42.000000 ipyslides-4.0.0/ipyslides/_base/styles.py
+-rw-rw-rw-   0        0        0    16171 2024-06-01 20:22:44.000000 ipyslides-4.0.0/ipyslides/_base/widgets.py
+-rw-rw-rw-   0        0        0    12531 2024-06-02 18:36:04.000000 ipyslides-4.0.0/ipyslides/_demo.py
+-rw-rw-rw-   0        0        0    46692 2024-06-02 02:28:07.000000 ipyslides-4.0.0/ipyslides/core.py
+-rw-rw-rw-   0        0        0    18778 2024-06-02 18:11:36.000000 ipyslides-4.0.0/ipyslides/formatters.py
+-rw-rw-rw-   0        0        0     8776 2024-06-01 18:12:25.000000 ipyslides-4.0.0/ipyslides/source.py
+-rw-rw-rw-   0        0        0    30968 2024-06-02 18:33:07.000000 ipyslides-4.0.0/ipyslides/utils.py
+-rw-rw-rw-   0        0        0    14549 2024-06-01 18:28:02.000000 ipyslides-4.0.0/ipyslides/writer.py
+-rw-rw-rw-   0        0        0    29435 2024-06-02 17:40:34.000000 ipyslides-4.0.0/ipyslides/xmd.py
+drwxrwxrwx   0        0        0        0 2024-06-02 18:37:53.560744 ipyslides-4.0.0/ipyslides.egg-info/
+-rw-rw-rw-   0        0        0     5273 2024-06-02 18:37:53.000000 ipyslides-4.0.0/ipyslides.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      854 2024-06-02 18:37:53.000000 ipyslides-4.0.0/ipyslides.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 18:37:53.000000 ipyslides-4.0.0/ipyslides.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      134 2024-06-02 18:37:53.000000 ipyslides-4.0.0/ipyslides.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-06-02 18:37:53.000000 ipyslides-4.0.0/ipyslides.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 18:37:53.592254 ipyslides-4.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     3730 2023-12-09 17:54:29.000000 ipyslides-4.0.0/setup.py
```

### Comparing `ipyslides-3.9.9/LICENSE` & `ipyslides-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.9/PKG-INFO` & `ipyslides-4.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyslides
-Version: 3.9.9
+Version: 4.0.0
 Summary: Live rich content slides in jupyter notebook
 Home-page: https://github.com/massgh/ipyslides
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyslides/issues
 Keywords: Jupyter,Widgets,IPython
```

### Comparing `ipyslides-3.9.9/README.md` & `ipyslides-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.9/ipyslides/_base/_layout_css.py` & `ipyslides-4.0.0/ipyslides/_base/_layout_css.py`

 * *Files 0% similar despite different names*

```diff
@@ -537,14 +537,18 @@
             ".CropBox": {
                 "z-index": "15 !important", # above others
                 ".CropHtml img": {
                     "border": "1px dashed red",
                     "padding": "0 !important",
                     "margin-bottom": "0 !important",
                     "box-sizing":"border-box"},
+                ".CropHtml figure": { # override inline margin
+                    "margin-inline": "0 !important",
+                    "margin-block": "0 !important",
+                },
             },
             ".Draw-Widget": {
                 "backdrop-filter": "blur(50px)",
                 "margin": 0,
                 "z-index": 6,
                 "overflow": "hidden !important",
                 "transition": "height 200ms",
```

### Comparing `ipyslides-3.9.9/ipyslides/_base/_widgets.py` & `ipyslides-4.0.0/ipyslides/_base/_widgets.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.9/ipyslides/_base/base.py` & `ipyslides-4.0.0/ipyslides/_base/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     @property
     def uid(self):
         "Unique CCS class for slides."
         return self._uid
     
     @property
     def css_styles(self):
-        """CSS styles for markdown or `classed` command."""
+        """CSS styles for markdown or `styled` command."""
         # self.html will be added from Chid class
         return self.raw('''
         Use any or combinations of these styles in className argument of writing functions:
         ------------------------------------------------------------------------------------
          className          | Formatting Style                                              
         ====================================================================================
          'text-[value]'     | [value] should be one of tiny, small, big, large, huge.
@@ -444,15 +444,15 @@
         
         with self.next_slide(), self.code.context():
             self.write(self.fmt('`{self.version!r}` `{self.xmd_syntax}`'))
             
         with self.next_slide():
             self.write('## Adding Content')
             self.write('Besides functions below, you can add content to slides with `%%xmd`,`%xmd` as well.\n{.note .info}')
-            self.write([self.classed(self.doc(self.write,'Slides'),'block-green'), self.doc(self.parse,'Slides'),self.doc(self.clip_image,'Slides')])
+            self.write([self.styled(self.doc(self.write,'Slides'),'block-green'), self.doc(self.parse,'Slides'),self.doc(self.clip_image,'Slides')])
         
         with self.next_slide():
             self.write('## Adding Speaker Notes')
             (skipper := self.goto_button('Skip to Dynamic Content')).display()
             self.write([f'You can use alert`notes\`notes content\`` in markdown.\n{{.note .success}}\n',
                        'This is experimental feature, and may not work as expected.\n{.note-error .error}'])
             self.doc(self.notes,'Slides.notes', members = True, itself = False).display()
@@ -460,25 +460,25 @@
         with self.next_slide():
             self.write('## Displaying Source Code')
             self.doc(self.code,'Slides.code', members = True, itself = False).display()
         
         self.next_from_markdown('section`?Layout and color[yellow,black]`Theme` Settings?` toc`### Contents`')
         
         with self.next_slide(): 
-            self.write('## Layout and Theme Settings')
+            self.styled('## Layout and Theme Settings', 'info', border='1px solid red').display()
             self.doc(self.settings,'Slides.settings', members=True,itself = False).display()
                 
         with self.next_slide():
             self.write('## Useful Functions for Rich Content section`?Useful Functions for alert`Rich Content`?`')
             self.doc(self.clip_image,'Slides').display()
             self.run_doc(self.alt,'Slides')
             
             members = sorted((
-                'alert block bokeh2html bullets classed format_html fmt color cols details doc sub sup '
-                'today error enable_zoom format_css highlight html iframe image keep_format notify plt2html '
+                'alert block bokeh2html bullets styled inline format_html fmt color cols details doc sub sup '
+                'today error zoomable format_css highlight html iframe image keep_format notify plt2html '
                 'raw rows set_dir sig textbox suppress_output suppress_stdout svg vspace'
             ).split())
             self.doc(self, 'Slides', members = members, itself = False).display()
 
         with self.next_slide():
             self.write('''
                 ## Citations and Sections
@@ -544,27 +544,26 @@
             self.doc(self.extender,'Slides.extender', members = True, itself = False).display()
         
         with self.next_slide():
             self.write('''
             ## Focus on what matters
             - There is a zoom button on top bar which enables zooming of certain elements. This can be toggled by `Z` key.
             - Most of supported elements are zoomable by default like images, matplotlib, bokeh, PIL image, altair plotly, dataframe, etc.
-            - You can also enable zooming for an object/widget by wrapping it inside `Slide.enable_zoom` function conveniently.
+            - You can also enable zooming for an object/widget by wrapping it inside `Slide.zoomable` function conveniently.
             - You can also enable by manully adding `zoom-self`, `zoom-child` classes to an element. To prevent zooming under as `zoom-child` class, use `no-zoom` class.
             
             ::: zoom-self block-red
                 ### Focus on Me 😎
                 - If zoom button is enabled, you can hover here to zoom in this part!
                 - You can also zoom in this part by pressing `Z` key while mouse is over this part.
             ''')
         with self.next_slide():
-            self.write('''
-                ## SVG Icons
-                Icons that apprear on buttons inslides (and their rotations) available to use in your slides as well.
-                ''')
+            self.inline('## SVG Icons',
+                'Icons that apprear on buttons inslides (and their rotations) available to use in your slides as well'
+            ).display()
             self.write(' '.join([f'`{k}`: ' + self.icon(k,color='crimson').svg for k in self.icon.available]))
             
             with self.code.context():
                 import ipywidgets as ipw
                 btn = ipw.Button(description='Chevron-Down',icon='plus').add_class('MyIcon') # Any free font awesome icon, but class is important to overwrite icon     
                 self.write(btn)
                 self.format_css({'.MyIcon .fa.fa-plus': self.icon('chevron',color='crimson', size='1.5em',rotation=90).css}).display() # Overwrite icon with your own
```

### Comparing `ipyslides-3.9.9/ipyslides/_base/export_html.py` & `ipyslides-4.0.0/ipyslides/_base/export_html.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.9/ipyslides/_base/export_template.py` & `ipyslides-4.0.0/ipyslides/_base/export_template.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.9/ipyslides/_base/icons.py` & `ipyslides-4.0.0/ipyslides/_base/icons.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.9/ipyslides/_base/intro.py` & `ipyslides-4.0.0/ipyslides/_base/intro.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.9/ipyslides/_base/js/interaction.js` & `ipyslides-4.0.0/ipyslides/_base/js/interaction.js`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.9/ipyslides/_base/js/notes.js` & `ipyslides-4.0.0/ipyslides/_base/js/notes.js`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.9/ipyslides/_base/navigation.py` & `ipyslides-4.0.0/ipyslides/_base/navigation.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.9/ipyslides/_base/notes.py` & `ipyslides-4.0.0/ipyslides/_base/notes.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.9/ipyslides/_base/screenshot.py` & `ipyslides-4.0.0/ipyslides/_base/screenshot.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             self.btn_crop.description = 'Set Crop Bounding Box'
 
     def _crop_image(self, change):
         if self._cimage is not None:
             x1,x2 = self.widgets.sliders.crop_w.value
             y2,y1 = [self.widgets.sliders.crop_h.max - v for v in self.widgets.sliders.crop_h.value]
             self._crop_bbox = [x1,y1,x2,y2]
-            self.widgets.htmls.crop.value = image(self._cimage.crop([x1,y1,x2,y2]), as_figure=False, width='100%').value
+            self.widgets.htmls.crop.value = image(self._cimage.crop([x1,y1,x2,y2]), width='100%').value
 
     @contextmanager
     def capture_mode(self, *additional_widgets_to_hide):
         """Hide some widgets and while capturing a screenshot, show them back again.
         You can provide additional widgets to hide while capturing as well."""
         hide_widgets = [self.widgets.controls, # now other buttons are inside Menu-Box which gets hidden 
                         self.widgets.htmls.toast,
```

### Comparing `ipyslides-3.9.9/ipyslides/_base/settings.py` & `ipyslides-4.0.0/ipyslides/_base/settings.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.9/ipyslides/_base/slide.py` & `ipyslides-4.0.0/ipyslides/_base/slide.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.9/ipyslides/_base/styles.py` & `ipyslides-4.0.0/ipyslides/_base/styles.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,14 @@
                 'color':'var(--heading-color)',
                 'text-align':'center' if centered else 'left',
                 'margin-block': '0.2em 0.3em !important', # Closer to the text of its own scope
                 'line-height':'1.5em',
                 'overflow':'hidden', # Firefox 
                 'mjx-c, .MathJax span': {"color":"var(--heading-color)",}, # MathJax span is for export
             },
-            'h1:first-of-type': {'margin-block-start':'0em !important',},
             'h1': {'font-size':'2.2em'},
             'h2': {'font-size':'1.7em'},
             'h3': {'font-size':'1.5em'},
             'h4': {'font-size':'1.2em'},
             'h5': {'font-size':'1em'},
             'table': {
                 'border-collapse':'collapse !important',
@@ -403,15 +402,15 @@
                     'align-items':'center !important',
                     'justify-content':'center !important',
                 },
             },
             'figcaption': {
                 'font-size':'0.8em !important',
                 'line-height':'1em !important',
-                'padding-top':'0.2em !important',
+                'padding':'0.5em 1.5em !important',
             },
             '.columns':{
                 'width':'100%',
                 'max-width':'100%',
                 'display':'inline-flex',
                 'flex-direction':'row',
                 'column-gap':'0.2em',
```

### Comparing `ipyslides-3.9.9/ipyslides/_base/widgets.py` & `ipyslides-4.0.0/ipyslides/_base/widgets.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.9/ipyslides/_demo.py` & `ipyslides-4.0.0/ipyslides/_demo.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         slides.write(f'alert`I was added at end by a given proxy, see the how it was done at the end of the slides`')
 
 
     slides.next_from_markdown(f"""
     section`Adding informative TOC` 
     ```toc ### Contents
     vspace`2` This is summary for current section created using block syntax of toc. See `Slides.xmd_syntax` for details.
-                                       
+                                    
     - Item 1
     - Item 2
 
     $$ E = mc^2 $$                        
     ```
                                        
     ```markdown
```

### Comparing `ipyslides-3.9.9/ipyslides/core.py` & `ipyslides-4.0.0/ipyslides/core.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.9/ipyslides/formatters.py` & `ipyslides-4.0.0/ipyslides/formatters.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,35 +43,42 @@
         return self._repr_html_()
     
     def as_widget(self, click_pointer=False):
         "Returns HtmlWidget with same data."
         return HtmlWidget(self.value, click_pointer=click_pointer)
         
 
-def plt2html(plt_fig = None,transparent=True,caption=None):
+def plt2html(plt_fig = None,transparent=True,width = '95%', caption=None):
     """Write matplotib figure as HTML string to use in `ipyslide.utils.write`.
     **Parameters**
     
     - plt_fig    : Matplotlib's figure instance, auto picks as well.
     - transparent: True of False for fig background.
+    - width      : CSS style width.
     - caption    : Caption for figure.
     """
     # First line is to remove depedency on matplotlib if not used
     plt = sys.modules.get('matplotlib.pyplot', __import__('matplotlib.pyplot'))
     _fig = plt_fig or plt.gcf()
     plot_bytes = BytesIO()
     _fig.savefig(plot_bytes,format='svg',transparent = transparent)
     _fig.clf() # Clear image to avoid other display
     plt.close() #AVoids throwing text outside figure
-    svg = '<svg' + plot_bytes.getvalue().decode('utf-8').split('<svg')[1]
-    cap = f'<figcaption class="no-zoom">{caption}</figcaption>' if caption else ''
+    width = f'width:{width}px;' if isinstance(width,int) else f'width:{width};'
+    svg = f'<svg style="{width}"' + plot_bytes.getvalue().decode('utf-8').split('<svg')[1]
+    
+    cap = ''
+    if caption:
+        from .xmd import _fig_caption # avoid circular import and only on demenad
+        cap = _fig_caption(caption)
+
     return XTML(f"<figure class='zoom-child'>{svg + cap}</figure>")
 
-def _plt2htmlstr(plt_fig=None,transparent=True,caption=None):
-    return plt2html(plt_fig=plt_fig,transparent=transparent,caption=caption).value
+def _plt2htmlstr(plt_fig=None,transparent=True,width="95%", caption=None):
+    return plt2html(plt_fig=plt_fig,transparent=transparent,width=width, caption=caption).value
 
 
 def bokeh2html(bokeh_fig,title=""):
     """Write bokeh figure as HTML string to use in `ipyslide.utils.write`.
     **Parameters**
     
     - bokeh_fig : Bokeh figure instance.
```

### Comparing `ipyslides-3.9.9/ipyslides/source.py` & `ipyslides-4.0.0/ipyslides/source.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.9/ipyslides/utils.py` & `ipyslides-4.0.0/ipyslides/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-_attrs = ['alt','alert', 'block', 'bullets', 'classed', 'color', 'cols', 'error', 'suppress_output','suppress_stdout','details', 'set_dir', 'textbox', 'vspace', 'center',
-            'image','svg','iframe', 'format_html','format_css','keep_format', 'run_doc',
-            'raw', 'rows', 'enable_zoom','html','sig','doc','code','today','sub','sup','get_child_dir','get_notebook_dir','is_jupyter_session','inside_jupyter_notebook']
+_attrs = ['alt','alert', 'block', 'bullets', 'color', 'cols', 'error', 'suppress_output','suppress_stdout','details', 'set_dir', 'textbox', 'hspace', 'vspace', 'center',
+            'image','svg','iframe', 'inline', 'format_html','format_css','keep_format', 'run_doc',
+            'raw', 'rows', 'zoomable','html','sig','styled', 'doc','code','today','sub','sup','get_child_dir','get_notebook_dir','is_jupyter_session','inside_jupyter_notebook']
 
 _attrs.extend([f'block_{c}' for c in 'red green blue cyan magenta yellow gray'.split()])
 __all__ = sorted(_attrs)
 
 import os, re
 import datetime
 import inspect
@@ -15,16 +15,17 @@
 
 from IPython import get_ipython
 from IPython.display import SVG, IFrame
 from IPython.core.display import Image, display
 import ipywidgets as ipw
 
 from .formatters import XTML, fix_ipy_image, htmlize
-from .xmd import get_unique_css_class, capture_content, raw, error # raw error for export from here
+from .xmd import _fig_caption, get_unique_css_class, capture_content, parse, raw, error # raw error for export from here
 from .writer import Writer, AltForWidget
+from ._base._widgets import HtmlWidget
 
 def is_jupyter_session():
      "Return True if code is executed inside jupyter session even while being imported."
      shell = get_ipython()
      if shell.__class__.__name__ in ("ZMQInteractiveShell","Shell"):
          return True # Verify Jupyter and Colab
      else:
@@ -334,84 +335,96 @@
     "Check if data is a PIL Image or numpy array"
     if data.__repr__().startswith('<PIL'):
         im_bytes = BytesIO()
         data.save(im_bytes,data.format if data.format else 'PNG',quality=95) #Save image to BytesIO in format of given image
         return im_bytes.getvalue()
     return data # if not return back data
 
-_fig_style_inline = "margin-block:0.5em;margin-inline:0.5em" # its 40px by defualt, ruins space, not working in CSS outside
+_fig_style_inline = "margin-block:0.25em;margin-inline:0.25em" # its 40px by defualt, ruins space, not working in CSS outside
 
-def image(data=None,width='95%',caption=None, as_figure = True, **kwargs):
+def image(data=None,width='95%',caption=None, **kwargs):
     """Displays PNG/JPEG files or image data etc, `kwrags` are passed to IPython.display.Image. 
     You can provide following to `data` parameter:
         
     - An opened PIL image. Useful for image operations and then direct writing to slides. 
     - A file path to image file.
     - A url to image file.
     - A str/bytes object containing image data.  
     - A str like "clip:image.png" will load an image saved using `Slides.clip_image('image.png')`. 
-
-    If `as_figure = False` caption is not used.
     """
     if isinstance(width,int):
         width = f'{width}px'
     
     if isinstance(data, str) and data.startswith("clip:"):
         data = get_child_dir(".ipyslides-assets", "clips", create = True) / data[5:] # strip clip by index, don't strip other characters
         if not data.exists():
             raise FileNotFoundError(f"File: {data!r} does not exist!")
     
     _data = _check_pil_image(data) #Check if data is a PIL Image or return data
     img = fix_ipy_image(Image(data = _data,**kwargs),width=width) # gievs XTML object
+    return html('figure', img.value + _fig_caption(caption), className='zoom-child', style = _fig_style_inline)  
 
-    if not as_figure:
-        return img
-    
-    cap = f'<figcaption class="no-zoom">{caption}</figcaption>' if caption else ''
-    return html('figure', img.value + cap, className='zoom-child', style = _fig_style_inline)  
-
-def svg(data=None,width = '95%',caption=None, as_figure=True, **kwargs):
+def svg(data=None,width = '95%',caption=None, **kwargs):
     """Display svg file or svg string/bytes with additional customizations. 
     `kwrags` are passed to IPython.display.SVG. You can provide url/string/bytes/filepath for svg.
-    
-    If `as_figure = False` caption is not used.
     """
     svg = SVG(data=data, **kwargs)._repr_svg_()
-    
-    if not as_figure:
-        return XTML(svg)
-    
-    cap = f'<figcaption class="no-zoom">{caption}</figcaption>' if caption else ''
     style = f'width:{width}px;' if isinstance(width,int) else f'width:{width};' + _fig_style_inline
-    return html('figure', svg + cap, className='zoom-child', style=style) 
+    return html('figure', svg + _fig_caption(caption), className='zoom-child', style=style) 
 
 
 def iframe(src, width='100%',height='auto',**kwargs):
     "Display `src` in an iframe. `kwrags` are passed to IPython.display.IFrame"
     f = IFrame(src,width,height, **kwargs)
     return XTML(f._repr_html_())
+    
+    
+def styled(obj, className=None, **css_inline_props):
+    """Add a class to a given object, whether a widget or html/IPYthon object.
+    CSS inline style properties should be given with names including '-' replaced with '_' but values should not.
+    Only a subset of inline properties take effect if obj is a widget.
+
+    ::: note-tip
+        Objects other than widgets will be wrapped in a 'div' tag. Use `html` function if you need more flexibility.
+    """
+    kwargs = {k.replace('_','-'):v for k,v in css_inline_props.items()}
+    style = ''.join(f"{k}:{v};" for k,v in kwargs.items())
+    klass = className if isinstance(className, str) else ''
 
-def enable_zoom(obj):
-    "Wraps a given obj in a parent with 'zoom-child' class or add 'zoom-self' to widget, whether a widget or html/IPYthon object"
     if isinstance(obj,ipw.DOMWidget):
-        return obj.add_class('zoom-self')
+        if hasattr(obj, 'layout'):
+            for k,v in kwargs.items():
+                setattr(obj.layout, k, v)
+        return obj.add_class(klass)
+    elif isinstance(obj, (str, bytes)):
+        return XTML(f'<div class="{klass}" style="{style}">{parse(obj, True)}</div>')
     else:
-        return classed(obj, 'zoom-child')
+        return XTML(f'<div class="{klass}" style="{style}">{htmlize(obj)}</div>')
     
-def classed(obj, className):
-    "Add a class to a given object, whether a widget or html/IPYthon object and pass to `write` command."
-    if not isinstance(className,str):
-        raise TypeError('className must be a string!')
-    if isinstance(obj,(str,bytes)):
-        raise TypeError('Cannnot add class to strings/bytes! Use `::: className [indented block on new line]` pattern in markdown instead.')
+def inline(*objs, **flex_box_props):
+    "Align objs in a horizontal flexbox. This is alternative to columns. Widgets are supported!"
+    children = [obj if isinstance(obj, ipw.DOMWidget) else parse(obj, True) if isinstance(obj, (str, bytes)) else htmlize(obj) for obj in objs]
+    kwargs = {'gap':'0.5em', **flex_box_props, 'display':'inline-flex', 'flex_direction': 'row'} # don't let change flex itslef
+    
+    if any(isinstance(child, ipw.DOMWidget) for child in children):
+        return alt(
+            styled(ipw.HBox([
+                child if isinstance(child, ipw.DOMWidget) else HtmlWidget(child) for child in children
+            ]), **kwargs), 
+        lambda w: '\n'.join(child.value if isinstance(child, (ipw.HTML, HtmlWidget)) else ''  for child in w.children)
+        )
     
+    return styled('\n'.join(children), **kwargs)
+
+def zoomable(obj):
+    "Wraps a given obj in a parent with 'zoom-child' class or add 'zoom-self' to widget, whether a widget or html/IPYthon object"
     if isinstance(obj,ipw.DOMWidget):
-        return obj.add_class(className)
+        return obj.add_class('zoom-self')
     else:
-        return XTML(f'<div class="{className}">{htmlize(obj)}</div>')
+        return styled(obj, 'zoom-child')
 
 def center(obj):
     "Align a given object at center horizontally, whether a widget or html/IPYthon object"
     if isinstance(obj,ipw.DOMWidget):
         return ipw.Box([obj]).add_class('align-center') # needs to wrap in another for cenering
     else:
         return XTML(f'<div class="align-center">{htmlize(obj)}</div>')
@@ -470,15 +483,19 @@
         
     tag_in =  f'<{tag} {attrs}>' if attrs else f'<{tag}>' # space is must after tag, strip attrs spaces
     return XTML(f'{tag_in}{content}</{tag}>')
 
 def vspace(em = 1):
     "Returns html node with given height in `em`."
     return html('div',style=f'height:{em}em;')
- 
+
+def hspace(em = 1):
+    "Returns html node with given height in `em`."
+    return html('div',style=f'width:{em}em;')
+
 def textbox(text, **css_props):
     """Formats text in a box for writing e.g. inline refrences. `css_props` are applied to box and `-` should be `_` like `font-size` -> `font_size`. 
     `text` is not parsed to general markdown i.e. only bold italic etc. applied, so if need markdown, parse it to html before. You can have common CSS for all textboxes using class `text-box`."""
     css_props = {'display':'inline-block','white-space': 'pre', **css_props} # very important to apply text styles in order
     # white-space:pre preserves whitspacing, text will be viewed as written. 
     _style = ' '.join([f"{key.replace('_','-')}:{value};" for key,value in css_props.items()])
     return XTML(f"<span class='text-box' style = {_style!r}>{text}</span>")  # markdown="span" will avoid inner parsing
```

### Comparing `ipyslides-3.9.9/ipyslides/writer.py` & `ipyslides-4.0.0/ipyslides/writer.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.9/ipyslides/xmd.py` & `ipyslides-4.0.0/ipyslides/xmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,27 +83,31 @@
 
 
 extender = PyMarkdown_Extender()
 del PyMarkdown_Extender
 
 _special_funcs = {
     "vspace": "number in units of em",
+    "hspace": "number in units of em",
     "alert": "text",
     "color": "text",
-    "image": "path/src or clip:filename",
-    "raw": "text",
-    "svg": "path/src",
-    "iframe": "src",
     "sub": "text",
     "sup": "text",
     "today": "fmt like %b-%d-%Y",
     "textbox": "text",  # Anything above this can be enclosed in a textbox
+    "image": "path/src or clip:filename",
+    "raw": "text",
+    "svg": "path/src",
+    "iframe": "src",
     "details": "text",
-    "center": "text or \`{variable}\`",
-}  # align-center should be at end of all
+    "inline": "keep objects inline",
+    "styled": "style objects with CSS classes and inline styles",
+    "zoomable": "zoom a block of html when hovered",
+    "center": "text or \`{variable}\`", # should be last
+}
 
 _code_ = """
 ```python run
 {app} = get_slides_instance()
 {block}
 ```
 """
@@ -154,29 +158,31 @@
         builtins.print = rprint # replace temporarily
         with capture_output(stdout=stdout, stderr=stderr,display=display) as cap:
             yield cap # pass capturedIO at top
     finally: # only need finally, errors are automatically thrown
         builtins.print = bprint
 
 
-def resolve_objs_on_slide(slide_instance, text_chunk):
+def resolve_objs_on_slide(xmd_instance, slide_instance, text_chunk):
     "Resolve objects in text_chunk corrsponding to slide such as cite, notes, etc."
     # notes`This is a note for current slide`
     all_matches = re.findall(
         r"notes\`(.*?)\`", text_chunk, flags=re.DOTALL | re.MULTILINE
     )
     for match in all_matches:
         slide_instance.notes.insert(match)
         text_chunk = text_chunk.replace(f"notes`{match}`", "", 1)
 
     # cite`key` should be after citations`key`, so that available for writing there if any
     all_matches = re.findall(r"cite\`(.*?)\`", text_chunk, flags=re.DOTALL)
     for match in all_matches:
         key = match.strip()
-        text_chunk = text_chunk.replace(f"cite`{match}`", slide_instance._cite(key), 1)
+        xmd_key = f"PrivateXmdVar{len(xmd_instance._vars)}X"
+        xmd_instance._vars[xmd_key] = slide_instance._cite(key) # need to store to avoid conflict with img[]`` etc.
+        text_chunk = text_chunk.replace(f"cite`{match}`", xmd_key , 1)
     
     # section`This is section title`
     all_matches = re.findall(
         r"section\`(.*?)\`", text_chunk, flags=re.DOTALL | re.MULTILINE
     )
     for match in all_matches:
         slide_instance.section(match)  # This will be attached to the running slide
@@ -359,15 +365,15 @@
         xmd = re.sub("\\\`", "&#96;", xmd)  # Escape backticks
         xmd = self._resolve_nested(
             xmd
         )  # Resolve nested objects in form func`?text?` to func`html_repr`
 
         if self._slides and self._slides.this: # under building slide
             xmd = resolve_objs_on_slide(
-                self._slides, xmd
+                self, self._slides, xmd
             )  # Resolve objects in xmd related to current slide
 
 
         # After resolve_objs_on_slide, xmd can have code blocks which may not be passed from suitable context
         if (r"\n```python run" in xmd) and self._returns: # Do not match nested blocks, r"" is important
             raise RuntimeError(
                 "Cannot execute code in current context, use Slides.parse(..., returns = False) for complete parsing!"
@@ -546,15 +552,15 @@
                 _func = getattr(utils, func)
                 _out = (_func(match) if match else _func()).value # If no argument, use default
                 html_output = html_output.replace(f"{func}`{match}`", handle_var(_out), 1)
 
         # Replace functions with arguments
         for func in _special_funcs.keys():
             all_matches = re.findall(
-                rf"{func}\[(.*?)\]\`(.*?)\`",
+                rf"{func}\[(.*?)\]\`(.*?)\`", # three or one backticks
                 html_output,
                 flags=re.DOTALL | re.MULTILINE,
             )
             for match in all_matches:
                 arg0 = match[1].strip()
                 args = [
                     v.replace("__COM__", ",")
@@ -671,7 +677,10 @@
 
     Returns an xtr object which delays formatting until it is intercepted by markdown parser.
     """
     if isinstance(text, str): # depth belowshoul be 2 to go where fmt will run
         return xtr(text).with_ns(_get_ns(text, 2, **kwargs)) # should return as string to be parsed
     else: # should not allow anything else because it will cause issues in Makrdown formatting
         return TypeError(f"fmt expects a str, got {type(text)}!")
+    
+def _fig_caption(text): # need here to use in many modules
+    return f'<figcaption class="no-zoom">{parse(text,True)}</figcaption>' if text else ''
```

### Comparing `ipyslides-3.9.9/ipyslides.egg-info/PKG-INFO` & `ipyslides-4.0.0/ipyslides.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyslides
-Version: 3.9.9
+Version: 4.0.0
 Summary: Live rich content slides in jupyter notebook
 Home-page: https://github.com/massgh/ipyslides
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyslides/issues
 Keywords: Jupyter,Widgets,IPython
```

### Comparing `ipyslides-3.9.9/ipyslides.egg-info/SOURCES.txt` & `ipyslides-4.0.0/ipyslides.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.9/setup.py` & `ipyslides-4.0.0/setup.py`

 * *Files identical despite different names*

