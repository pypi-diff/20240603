# Comparing `tmp/binomialbias-1.3.2.tar.gz` & `tmp/binomialbias-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binomialbias-1.3.2.tar", last modified: Fri Mar 15 15:35:01 2024, max compression
+gzip compressed data, was "binomialbias-1.3.3.tar", last modified: Mon Jun  3 09:21:20 2024, max compression
```

## Comparing `binomialbias-1.3.2.tar` & `binomialbias-1.3.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-03-15 15:35:01.568971 binomialbias-1.3.2/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    20849 2021-09-06 17:23:37.000000 binomialbias-1.3.2/LICENSE
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2600 2024-03-15 15:35:01.568971 binomialbias-1.3.2/PKG-INFO
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1768 2024-03-15 15:31:24.000000 binomialbias-1.3.2/README.md
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-03-15 15:35:01.568971 binomialbias-1.3.2/binomialbias/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       70 2023-07-23 02:56:45.000000 binomialbias-1.3.2/binomialbias/__init__.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    12583 2024-03-15 15:31:32.000000 binomialbias-1.3.2/binomialbias/app.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    14858 2023-09-15 14:39:54.000000 binomialbias-1.3.2/binomialbias/main.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       52 2024-03-15 15:31:43.000000 binomialbias-1.3.2/binomialbias/version.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-03-15 15:35:01.568971 binomialbias-1.3.2/binomialbias.egg-info/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2600 2024-03-15 15:35:01.000000 binomialbias-1.3.2/binomialbias.egg-info/PKG-INFO
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      356 2024-03-15 15:35:01.000000 binomialbias-1.3.2/binomialbias.egg-info/SOURCES.txt
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)        1 2024-03-15 15:35:01.000000 binomialbias-1.3.2/binomialbias.egg-info/dependency_links.txt
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       60 2024-03-15 15:35:01.000000 binomialbias-1.3.2/binomialbias.egg-info/requires.txt
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       13 2024-03-15 15:35:01.000000 binomialbias-1.3.2/binomialbias.egg-info/top_level.txt
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       38 2024-03-15 15:35:01.568971 binomialbias-1.3.2/setup.cfg
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1754 2023-09-12 07:08:24.000000 binomialbias-1.3.2/setup.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-03-15 15:35:01.568971 binomialbias-1.3.2/tests/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      606 2023-09-15 04:39:30.000000 binomialbias-1.3.2/tests/test_app.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      754 2023-09-15 14:39:54.000000 binomialbias-1.3.2/tests/test_plotting.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1684 2023-09-15 14:39:49.000000 binomialbias-1.3.2/tests/test_stats.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-06-03 09:21:20.142171 binomialbias-1.3.3/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    20849 2021-09-06 17:23:37.000000 binomialbias-1.3.3/LICENSE
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2600 2024-06-03 09:21:20.142171 binomialbias-1.3.3/PKG-INFO
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1768 2024-03-15 15:31:24.000000 binomialbias-1.3.3/README.md
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-06-03 09:21:20.142171 binomialbias-1.3.3/binomialbias/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       70 2023-07-23 02:56:45.000000 binomialbias-1.3.3/binomialbias/__init__.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    13131 2024-06-03 09:10:57.000000 binomialbias-1.3.3/binomialbias/app.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    15898 2024-06-03 09:10:57.000000 binomialbias-1.3.3/binomialbias/main.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       52 2024-06-03 09:10:57.000000 binomialbias-1.3.3/binomialbias/version.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-06-03 09:21:20.142171 binomialbias-1.3.3/binomialbias.egg-info/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2600 2024-06-03 09:21:20.000000 binomialbias-1.3.3/binomialbias.egg-info/PKG-INFO
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      356 2024-06-03 09:21:20.000000 binomialbias-1.3.3/binomialbias.egg-info/SOURCES.txt
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)        1 2024-06-03 09:21:20.000000 binomialbias-1.3.3/binomialbias.egg-info/dependency_links.txt
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       60 2024-06-03 09:21:20.000000 binomialbias-1.3.3/binomialbias.egg-info/requires.txt
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       13 2024-06-03 09:21:20.000000 binomialbias-1.3.3/binomialbias.egg-info/top_level.txt
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       38 2024-06-03 09:21:20.142171 binomialbias-1.3.3/setup.cfg
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1754 2023-09-12 07:08:24.000000 binomialbias-1.3.3/setup.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-06-03 09:21:20.142171 binomialbias-1.3.3/tests/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      606 2023-09-15 04:39:30.000000 binomialbias-1.3.3/tests/test_app.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      754 2023-09-15 14:39:54.000000 binomialbias-1.3.3/tests/test_plotting.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1684 2023-09-15 14:39:49.000000 binomialbias-1.3.3/tests/test_stats.py
```

### Comparing `binomialbias-1.3.2/LICENSE` & `binomialbias-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `binomialbias-1.3.2/PKG-INFO` & `binomialbias-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binomialbias
-Version: 1.3.2
+Version: 1.3.3
 Summary: Quantitative assessment of discrimination based on the binomial distribution
 Home-page: http://binomialbias.sciris.org
 Author: P.A. Robinson, C. C. Kerr
 Author-email: cliff@thekerrlab.com
 Keywords: binomial distribution,discrimination,bias,sexism,racism
 Platform: OS Independent
 Classifier: Environment :: Console
```

### Comparing `binomialbias-1.3.2/README.md` & `binomialbias-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `binomialbias-1.3.2/binomialbias/app.py` & `binomialbias-1.3.3/binomialbias/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,17 +67,17 @@
 
 def make_ui(*args, **kwargs):
 
     desc = '''
     <div>This webapp calculates bias and discrimination in appointment processes, based 
     on the binomial distribution. It is provided in support of the following paper:<br>
     <br>
-    <b>Quantitative assessment of discrimination in appointments to senior Australian university positions.</b>
-    Robinson PA, Kerr CC. <i>Under review (2023).</i><br>
-    <br>
+    <b>Quantitative measures of discrimination with application to appointment processes.</b>
+    Robinson PA, Kerr CC (2024). <i>PLoS ONE</i> <b>19</b>(3): e0299870. <a href="https://doi.org/10.1371/journal.pone.0299870">https://doi.org/10.1371/journal.pone.0299870</a>
+    <br><br>
     For more information, please see the <a href="https://github.com/thekerrlab/binomialbias">GitHub repository</a>,
     the <a href="http://binomialbiaspaper.sciris.org">paper</a>, or 
     <a href="mailto:cliff@thekerrlab.com">contact us</a>.<br>
     <br>
     </div>
     '''
     
@@ -154,16 +154,15 @@
                         ui.div(flexgap,
                             ui.input_checkbox("show_p", "Show plot", True),
                             ui.input_checkbox("show_s", "Show statistics", False),
                         )
                     ),
                     ui.div(
                         ui.panel_conditional("input.show_s",
-                            ui.h4('Statistics'),
-                            ui.output_table('stats_table'),
+                            ui.output_ui('stats_table'),
                         ),
                     ),
                     ui.output_text_verbatim('debug_text'), # Hidden unless debug = True above, but needed for reactivity
                 ),
             )
         ),
         title = 'BinomialBias',
@@ -189,14 +188,34 @@
 that 7 women would have been selected given a completely fair process is <i>P(n&le;n<sub>a</sub>)</i> = 0.135
 (compared to 0.588 had there been 10 women selected). We can also calculate that 
 the bias against women being selected for this committee is <i>B = 1.86</i>.<br>
 <br>
 Further information and examples are available in the manuscript.<br>
 ''')
 
+# Make statistics table
+def make_stats(hdict):
+    """ Get the HTML for rendering the statistics table """
+    header = '''
+<table class="dataframe table shiny-table w-auto">
+<thead><tr"><th>Parameter</th><th>Value</th></tr></thead>
+<tbody>
+'''
+    footer = '''
+</tbody>
+</table>
+'''
+    body = ''
+    for k,v in hdict.items():
+        body += f'<tr><td> {k} </td><td> {v} </td></tr>\n'
+        
+    tab = ui.HTML(sc.newlinejoin(header, body, footer))
+    return tab
+
+
 def server(input, output, session):
     """ The PyShiny server, which includes all the update logic """
     
     T2 = sc.timer() # For debugging
     g = make_globaldict()
     rerender = sh.reactive.Value(0)
     
@@ -312,21 +331,22 @@
         """ Plot the graphs """
         bb = make_bias()
         g.iter += 1
         fig = bb.plot(show=False, letters=False, wrap=True)
         return fig
     
     @output
-    @sh.render.table
+    @sh.render.ui
     @sh.reactive.event(rerender, ignore_none=False)
     def stats_table():
         """ Create a dataframe of the results """
         bb = make_bias()
-        df = bb.to_df(string=True)
-        return df
+        hdict = bb.to_html()
+        html = make_stats(hdict)
+        return html
     
     @output
     @sh.render.text
     def debug_text():
         """ Debugging -- which also happens to handle the reactivity! """
         import os
         u = get_ui()
```

### Comparing `binomialbias-1.3.2/binomialbias/main.py` & `binomialbias-1.3.3/binomialbias/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,38 @@
         if die:
             raise E
         else:
             num = np.nan
     return num
 
 
+def html_symbol(x, keep_var=False):
+    """ Append the mathematical symbol in HTML format to the text """
+    mapping = dict(
+        n             = '<i>n<sub>t</sub></i>',
+        expected      = '<i>n<sub>e</sub></i>',
+        actual        = '<i>n<sub>a</sub></i>',
+        f_expected    = '<i>f<sub>e</sub></i>',
+        f_actual      = '<i>f<sub>a</sub></i>',
+        expected_low  = '<i>E<sub>low</sub></i>',
+        expected_high = '<i>E<sub>high</sub></i>',
+        cum_prob      = '<i>P(n&lt;n<sub>a</sub>)</i>',
+        bias          = '<i>B</i>',
+        p_future      = '<i>P<sub>fut</sub></i>',
+    )
+    sym = mapping[x]
+    if sym:
+        if keep_var:
+            return f'{x} ({sym})'
+        else:
+            return sym
+    else:
+        return x
+
+
 class BinomialBias(sc.prettyobj):
     
     def __init__(self, n=20, n_e=10, n_a=7, f_e=None, f_a=None, one_sided=True,
                  display=False, plot=False, **kwargs):
         """
         Analysis for the paper "Quantitative assessment of discrimination in 
         appointments to senior Australian university positions" -
@@ -206,15 +230,23 @@
         """ Convert to a dataframe, optionally casting to string for correct s.f. """
         df = sc.dataframe.from_dict(self.results, orient='index')
         df = df.reset_index()
         df = df.rename(columns={'index':'Parameter', 0:'Value'})
         if string:
             df['Value'] = df['Value'].apply(lambda x: to_str(x))
         return df
-
+    
+    def to_html(self):
+        """ Convert results dictionary to an HTML-friendly version """
+        out = {}
+        for k,v in self.results.items():
+            new_k = html_symbol(k)
+            new_v = to_str(v)
+            out[new_k] = new_v
+        return out
 
     def plot(self, dist_color='cornflowerblue', cdf_color='darkblue', ci_color='k', letters=True, wrap=False,
              fig=None, barkw=None, figkw=None, layoutkw=None, textkw=None, max_bars=1000, show=True):
         """
         Plot the results of the bias calculation
         
         Args:
```

### Comparing `binomialbias-1.3.2/binomialbias.egg-info/PKG-INFO` & `binomialbias-1.3.3/binomialbias.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binomialbias
-Version: 1.3.2
+Version: 1.3.3
 Summary: Quantitative assessment of discrimination based on the binomial distribution
 Home-page: http://binomialbias.sciris.org
 Author: P.A. Robinson, C. C. Kerr
 Author-email: cliff@thekerrlab.com
 Keywords: binomial distribution,discrimination,bias,sexism,racism
 Platform: OS Independent
 Classifier: Environment :: Console
```

### Comparing `binomialbias-1.3.2/setup.py` & `binomialbias-1.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `binomialbias-1.3.2/tests/test_app.py` & `binomialbias-1.3.3/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `binomialbias-1.3.2/tests/test_plotting.py` & `binomialbias-1.3.3/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `binomialbias-1.3.2/tests/test_stats.py` & `binomialbias-1.3.3/tests/test_stats.py`

 * *Files identical despite different names*

