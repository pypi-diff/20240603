# Comparing `tmp/jupyter_bokeh-4.0.4.tar.gz` & `tmp/jupyter_bokeh-4.0.5.tar.gz`

## Comparing `jupyter_bokeh-4.0.4.tar` & `jupyter_bokeh-4.0.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/.eslintignore
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/.eslintrc.js
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/.yarnrc.yml
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/DEVGUIDE.md
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/MANIFEST.in
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/install.json
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/jupyter_bokeh.json
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/package.json
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/setup.cfg
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/setup.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/tsconfig.json
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/webpack.config.js
--rw-r--r--   0        0        0   202074 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/yarn.lock
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/conda.recipe/meta.yaml
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/examples/jupyter_interactors.ipynb
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/examples/jupyter_sliders.ipynb
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/examples/jupyter_widgets.ipynb
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/examples/notebook_comms.ipynb
--rw-r--r--   0        0        0     3836 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/examples/server_embed.ipynb
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/examples/static_plot.ipynb
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/jupyter_bokeh/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/jupyter_bokeh/_version.py
--rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/jupyter_bokeh/widgets.py
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/jupyter_bokeh/labextension/package.json
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/jupyter_bokeh/labextension/static/25.a1f00326924633b92ed3.js
--rw-r--r--   0        0        0   171237 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/jupyter_bokeh/labextension/static/7.2d4b977066efef2921dc.js
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/jupyter_bokeh/labextension/static/7.2d4b977066efef2921dc.js.LICENSE.txt
--rw-r--r--   0        0        0     6317 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/jupyter_bokeh/labextension/static/824.a3a1e45ab4137dbaadb5.js
--rw-r--r--   0        0        0     7455 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/jupyter_bokeh/labextension/static/remoteEntry.352adabd3ad00a55dce4.js
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/jupyter_bokeh/labextension/static/style.js
--rw-r--r--   0        0        0    10017 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/jupyter_bokeh/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/jupyter_bokeh/nbextension/extension.js
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/jupyter_bokeh/nbextension/index.js.LICENSE.txt
--rwxr-xr-x   0        0        0      409 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/scripts/deploy.sh
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/src/extension.ts
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/src/index.ts
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/src/manager.ts
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/src/metadata.d.ts
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/src/plugin.ts
--rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/src/renderer.ts
--rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/src/widgets.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/style/index.js
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/.gitignore
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/LICENSE.txt
--rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/README.md
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/pyproject.toml
--rw-r--r--   0        0        0     7119 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/PKG-INFO
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/.eslintignore
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/.eslintrc.js
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/.yarnrc.yml
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/DEVGUIDE.md
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/MANIFEST.in
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/install.json
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/jupyter_bokeh.json
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/package.json
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/setup.cfg
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/setup.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/tsconfig.json
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/webpack.config.js
+-rw-r--r--   0        0        0   202074 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/yarn.lock
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/conda.recipe/meta.yaml
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/examples/jupyter_interactors.ipynb
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/examples/jupyter_sliders.ipynb
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/examples/jupyter_widgets.ipynb
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/examples/notebook_comms.ipynb
+-rw-r--r--   0        0        0     3836 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/examples/server_embed.ipynb
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/examples/static_plot.ipynb
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/jupyter_bokeh/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/jupyter_bokeh/_version.py
+-rw-r--r--   0        0        0     6290 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/jupyter_bokeh/widgets.py
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/jupyter_bokeh/labextension/package.json
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/jupyter_bokeh/labextension/static/25.a1f00326924633b92ed3.js
+-rw-r--r--   0        0        0   171237 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/jupyter_bokeh/labextension/static/7.2d4b977066efef2921dc.js
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/jupyter_bokeh/labextension/static/7.2d4b977066efef2921dc.js.LICENSE.txt
+-rw-r--r--   0        0        0     6317 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/jupyter_bokeh/labextension/static/824.85f07f87f0792b25f70b.js
+-rw-r--r--   0        0        0     7455 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/jupyter_bokeh/labextension/static/remoteEntry.46e48fc13a737187eb1c.js
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/jupyter_bokeh/labextension/static/style.js
+-rw-r--r--   0        0        0    10017 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/jupyter_bokeh/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/jupyter_bokeh/nbextension/extension.js
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/jupyter_bokeh/nbextension/index.js.LICENSE.txt
+-rwxr-xr-x   0        0        0      409 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/scripts/deploy.sh
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/src/extension.ts
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/src/index.ts
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/src/manager.ts
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/src/metadata.d.ts
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/src/plugin.ts
+-rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/src/renderer.ts
+-rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/src/widgets.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/style/index.js
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/.gitignore
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/LICENSE.txt
+-rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/README.md
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/pyproject.toml
+-rw-r--r--   0        0        0     7119 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.5/PKG-INFO
```

### Comparing `jupyter_bokeh-4.0.4/.eslintrc.js` & `jupyter_bokeh-4.0.5/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.4/package.json` & `jupyter_bokeh-4.0.5/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'4.0.5'"}*

```diff
@@ -83,9 +83,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "4.0.4"
+    "version": "4.0.5"
 }
```

### Comparing `jupyter_bokeh-4.0.4/tsconfig.json` & `jupyter_bokeh-4.0.5/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.4/webpack.config.js` & `jupyter_bokeh-4.0.5/webpack.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.4/yarn.lock` & `jupyter_bokeh-4.0.5/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.4/conda.recipe/meta.yaml` & `jupyter_bokeh-4.0.5/conda.recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.4/examples/jupyter_interactors.ipynb` & `jupyter_bokeh-4.0.5/examples/jupyter_interactors.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.4/examples/jupyter_sliders.ipynb` & `jupyter_bokeh-4.0.5/examples/jupyter_sliders.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.4/examples/jupyter_widgets.ipynb` & `jupyter_bokeh-4.0.5/examples/jupyter_widgets.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.4/examples/notebook_comms.ipynb` & `jupyter_bokeh-4.0.5/examples/notebook_comms.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.4/examples/server_embed.ipynb` & `jupyter_bokeh-4.0.5/examples/server_embed.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.4/examples/static_plot.ipynb` & `jupyter_bokeh-4.0.5/examples/static_plot.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.4/jupyter_bokeh/__init__.py` & `jupyter_bokeh-4.0.5/jupyter_bokeh/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.4/jupyter_bokeh/widgets.py` & `jupyter_bokeh-4.0.5/jupyter_bokeh/widgets.py`

 * *Files 8% similar despite different names*

```diff
@@ -147,23 +147,23 @@
             new = descriptor.property.prepare_value(model, descriptor.name, new)
             old = descriptor._get(model)
             descriptor._set(model, old, new, setter=setter)
 
             for cb in model._callbacks.get(attr, []):
                 cb(attr, old, new)
         elif kind == "ColumnsStreamed":
-            model = content["model"]
-            data = content["data"]
-            rollover = content["rollover"]
+            model = event["model"]
+            data = event["data"]
+            rollover = event["rollover"]
 
             assert isinstance(model, ColumnDataSource)
             model._stream(data, rollover, setter=setter)
         elif kind == "ColumnsPatched":
-            model = content["model"]
-            patches = content["data"]
+            model = event["model"]
+            patches = event["patches"]
 
             assert isinstance(model, ColumnDataSource)
             model.patch(patches, setter=setter)
         elif kind == "MessageSent":
             msg_type = event["msg_type"]
             msg_data = event["msg_data"]
             if msg_type == "bokeh_event":
```

### Comparing `jupyter_bokeh-4.0.4/jupyter_bokeh/labextension/package.json` & `jupyter_bokeh-4.0.5/jupyter_bokeh/labextension/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9755291005291005%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.46e48fc13a737187eb1c.js'}}",*

 * * "'version'": "'4.0.5'"}*

```diff
@@ -36,15 +36,15 @@
         "{dist,lib}/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/bokeh/jupyter_bokeh",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.352adabd3ad00a55dce4.js",
+            "load": "static/remoteEntry.46e48fc13a737187eb1c.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyter_bokeh/labextension"
     },
     "keywords": [
         "jupyter",
@@ -88,9 +88,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "4.0.4"
+    "version": "4.0.5"
 }
```

### Comparing `jupyter_bokeh-4.0.4/jupyter_bokeh/labextension/static/25.a1f00326924633b92ed3.js` & `jupyter_bokeh-4.0.5/jupyter_bokeh/labextension/static/25.a1f00326924633b92ed3.js`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.4/jupyter_bokeh/labextension/static/7.2d4b977066efef2921dc.js` & `jupyter_bokeh-4.0.5/jupyter_bokeh/labextension/static/7.2d4b977066efef2921dc.js`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.4/jupyter_bokeh/labextension/static/824.a3a1e45ab4137dbaadb5.js` & `jupyter_bokeh-4.0.5/jupyter_bokeh/labextension/static/824.85f07f87f0792b25f70b.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -230,12 +230,12 @@
                 },
                 autoStart: !0
             }
         },
         2288: (e, t) => {
             Object.assign(t, {
                 name: "@bokeh/jupyter_bokeh",
-                version: "4.0.4"
+                version: "4.0.5"
             })
         }
     }
 ]);
```

### Comparing `jupyter_bokeh-4.0.4/jupyter_bokeh/labextension/static/remoteEntry.352adabd3ad00a55dce4.js` & `jupyter_bokeh-4.0.5/jupyter_bokeh/labextension/static/remoteEntry.46e48fc13a737187eb1c.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, o, n, a, i, u, l, s, f, d, c, p, h, b, v, m, g, y, w = {
+    var e, r, t, o, n, a, i, u, l, s, d, f, c, p, h, b, v, m, g, y, w = {
             55: (e, r, t) => {
                 var o = {
                         "./index": () => Promise.all([t.e(256), t.e(824)]).then((() => () => t(9824))),
                         "./extension": () => Promise.all([t.e(256), t.e(824)]).then((() => () => t(9824))),
                         "./style": () => t.e(25).then((() => () => t(4025)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(o, e) ? o[e]() : Promise.resolve().then((() => {
@@ -48,51 +48,51 @@
             get: r[t]
         })
     }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
         7: "2d4b977066efef2921dc",
         25: "a1f00326924633b92ed3",
         256: "3673b9e8accbe04f1c8a",
         805: "5070eeb32117fc99ba19",
-        824: "a3a1e45ab4137dbaadb5"
+        824: "85f07f87f0792b25f70b"
     } [e] + ".js?v=" + {
         7: "2d4b977066efef2921dc",
         25: "a1f00326924633b92ed3",
         256: "3673b9e8accbe04f1c8a",
         805: "5070eeb32117fc99ba19",
-        824: "a3a1e45ab4137dbaadb5"
+        824: "85f07f87f0792b25f70b"
     } [e], j.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), j.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@bokeh/jupyter_bokeh:", j.l = (t, o, n, a) => {
         if (e[t]) e[t].push(o);
         else {
             var i, u;
             if (void 0 !== n)
                 for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
-                    var f = l[s];
-                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + n) {
-                        i = f;
+                    var d = l[s];
+                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + n) {
+                        i = d;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, j.nc && i.setAttribute("nonce", j.nc), i.setAttribute("data-webpack", r + n), i.src = t), e[t] = [o];
-            var d = (r, o) => {
+            var f = (r, o) => {
                     i.onerror = i.onload = null, clearTimeout(c);
                     var n = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), n && n.forEach((e => e(o))), r) return r(o)
                 },
-                c = setTimeout(d.bind(null, void 0, {
+                c = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, j.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -114,15 +114,15 @@
                         (!u || !u.loaded && (!o != !u.eager ? o : i > u.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!o
                         })
                     },
                     l = [];
-                return "default" === t && (u("@bokeh/jupyter_bokeh", "4.0.4", (() => Promise.all([j.e(256), j.e(824)]).then((() => () => j(9824))))), u("@jupyter-widgets/base", "6.0.7", (() => Promise.all([j.e(7), j.e(805), j.e(256)]).then((() => () => j(4007)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("@bokeh/jupyter_bokeh", "4.0.5", (() => Promise.all([j.e(256), j.e(824)]).then((() => () => j(9824))))), u("@jupyter-widgets/base", "6.0.7", (() => Promise.all([j.e(7), j.e(805), j.e(256)]).then((() => () => j(4007)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -172,33 +172,33 @@
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var o = e[0],
                 n = o < 0;
             n && (o = -o - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var s, f, d = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !l || ("u" == d ? u > o && !n : "" == d != n);
-                if ("u" == f) {
-                    if (!l || "u" != d) return !1
+                var s, d, f = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (d = (typeof(s = r[i]))[0])) return !l || ("u" == f ? u > o && !n : "" == f != n);
+                if ("u" == d) {
+                    if (!l || "u" != f) return !1
                 } else if (l)
-                    if (d == f)
+                    if (f == d)
                         if (u <= o) {
                             if (s != e[u]) return !1
                         } else {
                             if (n ? s > e[u] : s < e[u]) return !1;
                             s != e[u] && (l = !1)
                         }
-                else if ("s" != d && "n" != d) {
+                else if ("s" != f && "n" != f) {
                     if (n || u <= o) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= o || f < d != n) return !1;
+                    if (u <= o || d < f != n) return !1;
                     l = !1
-                } else "s" != d && "n" != d && (l = !1, u--)
+                } else "s" != f && "n" != f && (l = !1, u--)
             }
         }
         var c = [],
             p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
@@ -209,25 +209,25 @@
         if (!t || !j.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && o(e, r) ? r : e), 0)
     }, l = (e, r, t, o) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(o) + ")", s = (e, r, t, o) => {
         var n = u(e, t);
-        return a(o, n) || d(l(e, t, n, o)), c(e[t][n])
-    }, f = (e, r, t) => {
+        return a(o, n) || f(l(e, t, n, o)), c(e[t][n])
+    }, d = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !a(t, r) || e && !o(e, r) ? e : r), 0)) && n[r]
-    }, d = e => {
+    }, f = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, o, n) {
         var a = j.I(r);
         return a && a.then ? a.then(e.bind(e, r, j.S[r], t, o, n)) : e(r, j.S[r], t, o, n)
     })(((e, r, t, o) => (i(e, t), s(r, 0, t, o)))), b = p(((e, r, t, o, n) => {
-        var a = r && j.o(r, t) && f(r, t, o);
+        var a = r && j.o(r, t) && d(r, t, o);
         return a ? c(a) : n()
     })), v = {}, m = {
         5256: () => h("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
         1803: () => b("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 5],
             [1, 4],
             [1, 3],
```

### Comparing `jupyter_bokeh-4.0.4/jupyter_bokeh/labextension/static/third-party-licenses.json` & `jupyter_bokeh-4.0.5/jupyter_bokeh/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.4/jupyter_bokeh/nbextension/index.js.LICENSE.txt` & `jupyter_bokeh-4.0.5/jupyter_bokeh/nbextension/index.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.4/src/manager.ts` & `jupyter_bokeh-4.0.5/src/manager.ts`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.4/src/plugin.ts` & `jupyter_bokeh-4.0.5/src/plugin.ts`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.4/src/renderer.ts` & `jupyter_bokeh-4.0.5/src/renderer.ts`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.4/src/widgets.ts` & `jupyter_bokeh-4.0.5/src/widgets.ts`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.4/LICENSE.txt` & `jupyter_bokeh-4.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.4/README.md` & `jupyter_bokeh-4.0.5/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.4/pyproject.toml` & `jupyter_bokeh-4.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.4/PKG-INFO` & `jupyter_bokeh-4.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_bokeh
-Version: 4.0.4
+Version: 4.0.5
 Summary: A Jupyter extension for rendering Bokeh content.
 Project-URL: Homepage, https://github.com/bokeh/jupyter_bokeh
 Project-URL: Bug Tracker, https://github.com/bokeh/jupyter_bokeh/issues
 Project-URL: Repository, https://github.com/bokeh/jupyter_bokeh.git
 Author-email: Bokeh team <info@bokeh.org>
 License: Copyright (c) 2012 - 2020, Anaconda, Inc., and Bokeh Contributors
         All rights reserved.
```

