# Comparing `tmp/pyrtz2-1.2.2.tar.gz` & `tmp/pyrtz2-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrtz2-1.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyrtz2-1.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyrtz2-1.2.2.tar` & `pyrtz2-1.2.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0       66 2024-04-02 19:47:59.285340 pyrtz2-1.2.2/.gitattributes
--rw-r--r--   0        0        0       37 2024-04-05 12:35:50.341792 pyrtz2-1.2.2/.gitignore
--rw-r--r--   0        0        0    33041 2024-04-02 20:07:11.768711 pyrtz2-1.2.2/LICENSE
--rw-r--r--   0        0        0      849 2024-05-28 19:32:22.605264 pyrtz2-1.2.2/README.md
--rw-r--r--   0        0        0   147249 2024-05-28 13:20:12.872947 pyrtz2-1.2.2/example/con050.PNG
--rw-r--r--   0        0        0   442996 2024-03-22 20:48:12.000000 pyrtz2-1.2.2/example/con050/jasYcon050cell37m0000.ibw
--rw-r--r--   0        0        0   922624 2024-03-22 20:48:22.000000 pyrtz2-1.2.2/example/con050/jasYcon050cell37m0001.tif
--rw-r--r--   0        0        0   453575 2024-03-22 20:48:52.000000 pyrtz2-1.2.2/example/con050/jasYcon050cell38m0000.ibw
--rw-r--r--   0        0        0   922624 2024-03-22 20:49:00.000000 pyrtz2-1.2.2/example/con050/jasYcon050cell38m0001.tif
--rw-r--r--   0        0        0   458723 2024-03-22 20:49:32.000000 pyrtz2-1.2.2/example/con050/jasYcon050cell39m0000.ibw
--rw-r--r--   0        0        0   922624 2024-03-22 20:49:38.000000 pyrtz2-1.2.2/example/con050/jasYcon050cell39m0001.tif
--rw-r--r--   0        0        0   435180 2024-03-22 20:50:14.000000 pyrtz2-1.2.2/example/con050/jasYcon050cell40m0000.ibw
--rw-r--r--   0        0        0   922624 2024-03-22 20:50:22.000000 pyrtz2-1.2.2/example/con050/jasYcon050cell40m0001.tif
--rw-r--r--   0        0        0   457660 2024-03-22 20:54:28.000000 pyrtz2-1.2.2/example/con050/jasYcon050cell42m0000.ibw
--rw-r--r--   0        0        0   922624 2024-03-22 20:54:36.000000 pyrtz2-1.2.2/example/con050/jasYcon050cell42m0001.tif
--rw-r--r--   0        0        0      202 2024-05-28 04:49:07.012252 pyrtz2-1.2.2/example/con050_cp_annotations.json
--rw-r--r--   0        0        0   337342 2024-05-28 05:18:15.173445 pyrtz2-1.2.2/example/con050_curves.pdf
--rw-r--r--   0        0        0     2741 2024-05-28 05:00:39.789633 pyrtz2-1.2.2/example/con050_fits.csv
--rw-r--r--   0        0        0     2814 2024-05-28 04:49:07.129790 pyrtz2-1.2.2/example/con050_im_annotations.json
--rw-r--r--   0        0        0      203 2024-05-28 04:49:07.063912 pyrtz2-1.2.2/example/con050_vd_annotations.json
--rw-r--r--   0        0        0       37 2024-04-05 12:53:39.905466 pyrtz2-1.2.2/example/test.py
--rw-r--r--   0        0        0      837 2024-05-22 01:14:58.847887 pyrtz2-1.2.2/pyproject.toml
--rw-r--r--   0        0        0       61 2024-05-28 19:33:14.063599 pyrtz2-1.2.2/pyrtz2/__init__.py
--rw-r--r--   0        0        0     2905 2024-05-12 14:31:18.502112 pyrtz2-1.2.2/pyrtz2/afm.py
--rw-r--r--   0        0        0      334 2024-05-23 04:49:31.358304 pyrtz2-1.2.2/pyrtz2/app.py
--rw-r--r--   0        0        0     1320 2024-03-29 18:30:21.132859 pyrtz2-1.2.2/pyrtz2/assets/style.css
--rw-r--r--   0        0        0     5108 2024-05-23 04:03:31.968397 pyrtz2-1.2.2/pyrtz2/asylum.py
--rw-r--r--   0        0        0    18167 2024-05-26 21:26:32.180350 pyrtz2-1.2.2/pyrtz2/curves.py
--rw-r--r--   0        0        0     4446 2024-05-23 21:11:51.382633 pyrtz2-1.2.2/pyrtz2/fit.py
--rw-r--r--   0        0        0        0 2024-04-03 01:57:24.101285 pyrtz2-1.2.2/pyrtz2/src/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.2.2/pyrtz2/src/components/__init__.py
--rw-r--r--   0        0        0     2461 2024-05-22 13:02:06.518745 pyrtz2-1.2.2/pyrtz2/src/components/annotator.py
--rw-r--r--   0        0        0     4851 2024-05-22 12:50:02.290868 pyrtz2-1.2.2/pyrtz2/src/components/contact_controls.py
--rw-r--r--   0        0        0     4115 2024-04-06 15:49:10.536249 pyrtz2-1.2.2/pyrtz2/src/components/curve_dropdown.py
--rw-r--r--   0        0        0     6326 2024-05-28 05:05:42.387835 pyrtz2-1.2.2/pyrtz2/src/components/downloader.py
--rw-r--r--   0        0        0     1796 2024-05-26 12:23:11.462175 pyrtz2-1.2.2/pyrtz2/src/components/experiment_loader.py
--rw-r--r--   0        0        0     3520 2024-05-26 21:30:53.840715 pyrtz2-1.2.2/pyrtz2/src/components/fig.py
--rw-r--r--   0        0        0     3251 2024-05-26 21:23:53.868511 pyrtz2-1.2.2/pyrtz2/src/components/fig_frame.py
--rw-r--r--   0        0        0     2192 2024-05-24 00:21:12.997723 pyrtz2-1.2.2/pyrtz2/src/components/fitter.py
--rw-r--r--   0        0        0     1294 2024-05-28 04:32:50.442531 pyrtz2-1.2.2/pyrtz2/src/components/ids.py
--rw-r--r--   0        0        0     8140 2024-05-28 19:01:29.143678 pyrtz2-1.2.2/pyrtz2/src/components/image.py
--rw-r--r--   0        0        0     3530 2024-05-28 04:32:50.846663 pyrtz2-1.2.2/pyrtz2/src/components/image_controls.py
--rw-r--r--   0        0        0     2493 2024-05-28 18:41:02.903094 pyrtz2-1.2.2/pyrtz2/src/components/image_frame.py
--rw-r--r--   0        0        0     1102 2024-05-26 18:40:42.770898 pyrtz2-1.2.2/pyrtz2/src/components/image_loader.py
--rw-r--r--   0        0        0     1509 2024-05-22 12:41:39.698771 pyrtz2-1.2.2/pyrtz2/src/components/layout.py
--rw-r--r--   0        0        0     3214 2024-05-23 03:44:27.840596 pyrtz2-1.2.2/pyrtz2/src/components/loader.py
--rw-r--r--   0        0        0     1211 2024-05-23 03:57:00.269489 pyrtz2-1.2.2/pyrtz2/src/components/toolbox.py
--rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.2.2/pyrtz2/src/utils/__init__.py
--rw-r--r--   0        0        0     2242 2024-05-28 05:00:03.989827 pyrtz2-1.2.2/pyrtz2/src/utils/processor.py
--rw-r--r--   0        0        0     2905 2024-05-27 16:39:21.314177 pyrtz2-1.2.2/pyrtz2/src/utils/utils.py
--rw-r--r--   0        0        0     1637 1970-01-01 00:00:00.000000 pyrtz2-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0       66 2024-04-02 19:47:59.285340 pyrtz2-1.2.3/.gitattributes
+-rw-r--r--   0        0        0       37 2024-04-05 12:35:50.341792 pyrtz2-1.2.3/.gitignore
+-rw-r--r--   0        0        0    33041 2024-04-02 20:07:11.768711 pyrtz2-1.2.3/LICENSE
+-rw-r--r--   0        0        0      849 2024-05-28 19:32:22.605264 pyrtz2-1.2.3/README.md
+-rw-r--r--   0        0        0   147249 2024-05-28 13:20:12.872947 pyrtz2-1.2.3/example/con050.PNG
+-rw-r--r--   0        0        0   442996 2024-03-22 20:48:12.000000 pyrtz2-1.2.3/example/con050/jasYcon050cell37m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:48:22.000000 pyrtz2-1.2.3/example/con050/jasYcon050cell37m0001.tif
+-rw-r--r--   0        0        0   453575 2024-03-22 20:48:52.000000 pyrtz2-1.2.3/example/con050/jasYcon050cell38m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:49:00.000000 pyrtz2-1.2.3/example/con050/jasYcon050cell38m0001.tif
+-rw-r--r--   0        0        0   458723 2024-03-22 20:49:32.000000 pyrtz2-1.2.3/example/con050/jasYcon050cell39m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:49:38.000000 pyrtz2-1.2.3/example/con050/jasYcon050cell39m0001.tif
+-rw-r--r--   0        0        0   435180 2024-03-22 20:50:14.000000 pyrtz2-1.2.3/example/con050/jasYcon050cell40m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:50:22.000000 pyrtz2-1.2.3/example/con050/jasYcon050cell40m0001.tif
+-rw-r--r--   0        0        0   457660 2024-03-22 20:54:28.000000 pyrtz2-1.2.3/example/con050/jasYcon050cell42m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:54:36.000000 pyrtz2-1.2.3/example/con050/jasYcon050cell42m0001.tif
+-rw-r--r--   0        0        0      202 2024-05-28 04:49:07.012252 pyrtz2-1.2.3/example/con050_cp_annotations.json
+-rw-r--r--   0        0        0   337342 2024-05-28 05:18:15.173445 pyrtz2-1.2.3/example/con050_curves.pdf
+-rw-r--r--   0        0        0     2741 2024-05-28 05:00:39.789633 pyrtz2-1.2.3/example/con050_fits.csv
+-rw-r--r--   0        0        0     2814 2024-05-28 04:49:07.129790 pyrtz2-1.2.3/example/con050_im_annotations.json
+-rw-r--r--   0        0        0      203 2024-05-28 04:49:07.063912 pyrtz2-1.2.3/example/con050_vd_annotations.json
+-rw-r--r--   0        0        0       37 2024-04-05 12:53:39.905466 pyrtz2-1.2.3/example/test.py
+-rw-r--r--   0        0        0      837 2024-05-22 01:14:58.847887 pyrtz2-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0       61 2024-06-03 04:25:33.600535 pyrtz2-1.2.3/pyrtz2/__init__.py
+-rw-r--r--   0        0        0     2905 2024-05-12 14:31:18.502112 pyrtz2-1.2.3/pyrtz2/afm.py
+-rw-r--r--   0        0        0      334 2024-05-23 04:49:31.358304 pyrtz2-1.2.3/pyrtz2/app.py
+-rw-r--r--   0        0        0     1320 2024-03-29 18:30:21.132859 pyrtz2-1.2.3/pyrtz2/assets/style.css
+-rw-r--r--   0        0        0     5108 2024-05-23 04:03:31.968397 pyrtz2-1.2.3/pyrtz2/asylum.py
+-rw-r--r--   0        0        0    18369 2024-06-03 04:25:17.842153 pyrtz2-1.2.3/pyrtz2/curves.py
+-rw-r--r--   0        0        0     4446 2024-05-23 21:11:51.382633 pyrtz2-1.2.3/pyrtz2/fit.py
+-rw-r--r--   0        0        0        0 2024-04-03 01:57:24.101285 pyrtz2-1.2.3/pyrtz2/src/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.2.3/pyrtz2/src/components/__init__.py
+-rw-r--r--   0        0        0     2461 2024-05-22 13:02:06.518745 pyrtz2-1.2.3/pyrtz2/src/components/annotator.py
+-rw-r--r--   0        0        0     4851 2024-05-22 12:50:02.290868 pyrtz2-1.2.3/pyrtz2/src/components/contact_controls.py
+-rw-r--r--   0        0        0     4115 2024-04-06 15:49:10.536249 pyrtz2-1.2.3/pyrtz2/src/components/curve_dropdown.py
+-rw-r--r--   0        0        0     6326 2024-05-28 05:05:42.387835 pyrtz2-1.2.3/pyrtz2/src/components/downloader.py
+-rw-r--r--   0        0        0     1796 2024-05-28 19:59:58.356675 pyrtz2-1.2.3/pyrtz2/src/components/experiment_loader.py
+-rw-r--r--   0        0        0     3520 2024-05-26 21:30:53.840715 pyrtz2-1.2.3/pyrtz2/src/components/fig.py
+-rw-r--r--   0        0        0     3251 2024-05-26 21:23:53.868511 pyrtz2-1.2.3/pyrtz2/src/components/fig_frame.py
+-rw-r--r--   0        0        0     2192 2024-05-24 00:21:12.997723 pyrtz2-1.2.3/pyrtz2/src/components/fitter.py
+-rw-r--r--   0        0        0     1294 2024-05-28 04:32:50.442531 pyrtz2-1.2.3/pyrtz2/src/components/ids.py
+-rw-r--r--   0        0        0     8140 2024-05-28 19:01:29.143678 pyrtz2-1.2.3/pyrtz2/src/components/image.py
+-rw-r--r--   0        0        0     3530 2024-05-28 04:32:50.846663 pyrtz2-1.2.3/pyrtz2/src/components/image_controls.py
+-rw-r--r--   0        0        0     2493 2024-05-28 18:41:02.903094 pyrtz2-1.2.3/pyrtz2/src/components/image_frame.py
+-rw-r--r--   0        0        0     1102 2024-05-26 18:40:42.770898 pyrtz2-1.2.3/pyrtz2/src/components/image_loader.py
+-rw-r--r--   0        0        0     1509 2024-05-22 12:41:39.698771 pyrtz2-1.2.3/pyrtz2/src/components/layout.py
+-rw-r--r--   0        0        0     3214 2024-05-23 03:44:27.840596 pyrtz2-1.2.3/pyrtz2/src/components/loader.py
+-rw-r--r--   0        0        0     1211 2024-05-23 03:57:00.269489 pyrtz2-1.2.3/pyrtz2/src/components/toolbox.py
+-rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.2.3/pyrtz2/src/utils/__init__.py
+-rw-r--r--   0        0        0     2242 2024-05-28 05:00:03.989827 pyrtz2-1.2.3/pyrtz2/src/utils/processor.py
+-rw-r--r--   0        0        0     2905 2024-05-27 16:39:21.314177 pyrtz2-1.2.3/pyrtz2/src/utils/utils.py
+-rw-r--r--   0        0        0     1637 1970-01-01 00:00:00.000000 pyrtz2-1.2.3/PKG-INFO
```

### Comparing `pyrtz2-1.2.2/LICENSE` & `pyrtz2-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/README.md` & `pyrtz2-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/example/con050.PNG` & `pyrtz2-1.2.3/example/con050.PNG`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/example/con050/jasYcon050cell37m0000.ibw` & `pyrtz2-1.2.3/example/con050/jasYcon050cell37m0000.ibw`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/example/con050/jasYcon050cell37m0001.tif` & `pyrtz2-1.2.3/example/con050/jasYcon050cell37m0001.tif`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/example/con050/jasYcon050cell38m0000.ibw` & `pyrtz2-1.2.3/example/con050/jasYcon050cell38m0000.ibw`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/example/con050/jasYcon050cell38m0001.tif` & `pyrtz2-1.2.3/example/con050/jasYcon050cell38m0001.tif`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/example/con050/jasYcon050cell39m0000.ibw` & `pyrtz2-1.2.3/example/con050/jasYcon050cell39m0000.ibw`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/example/con050/jasYcon050cell39m0001.tif` & `pyrtz2-1.2.3/example/con050/jasYcon050cell39m0001.tif`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/example/con050/jasYcon050cell40m0000.ibw` & `pyrtz2-1.2.3/example/con050/jasYcon050cell40m0000.ibw`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/example/con050/jasYcon050cell40m0001.tif` & `pyrtz2-1.2.3/example/con050/jasYcon050cell40m0001.tif`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/example/con050/jasYcon050cell42m0000.ibw` & `pyrtz2-1.2.3/example/con050/jasYcon050cell42m0000.ibw`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/example/con050/jasYcon050cell42m0001.tif` & `pyrtz2-1.2.3/example/con050/jasYcon050cell42m0001.tif`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/example/con050_curves.pdf` & `pyrtz2-1.2.3/example/con050_curves.pdf`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/example/con050_fits.csv` & `pyrtz2-1.2.3/example/con050_fits.csv`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/example/con050_im_annotations.json` & `pyrtz2-1.2.3/example/con050_im_annotations.json`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/pyproject.toml` & `pyrtz2-1.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/pyrtz2/afm.py` & `pyrtz2-1.2.3/pyrtz2/afm.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/pyrtz2/assets/style.css` & `pyrtz2-1.2.3/pyrtz2/assets/style.css`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/pyrtz2/asylum.py` & `pyrtz2-1.2.3/pyrtz2/asylum.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/pyrtz2/curves.py` & `pyrtz2-1.2.3/pyrtz2/curves.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,22 +31,24 @@
 
     _data: pd.DataFrame
     corrected: bool = False
     contact_index: int = 0
     contact_values: pd.Series | None = None
     max_ind: float
     max_f: float
+    t_ind: float
     vel_ind: float
     vel_z: float
     figs_data: dict[str, tuple[np.ndarray, np.ndarray]]
     fits_data: dict[str, tuple[np.ndarray, np.ndarray]]
     indent_param: list[float]
     indent_R2: float
     hertzian_param: list[float]
     hertzian_R2: float
+    t_dwell: float
     dwell_param: list[float]
     dwell_R2: float
     contact_fig: go.Figure
     dwell_fig: go.Figure
 
     def __init__(
             self,
@@ -60,15 +62,15 @@
 
         self.filename = filename
         self.data = data
         self.notes = notes
         self.invOLS = invOLS
         self.k = k
         self.dwell_range = dwell_range
-
+        self.t_dwell = float(notes['DwellTime'])
         self.backup_data()
 
     def backup_data(self) -> None:
         self._data = self.data.copy()
 
     def restore_data(self) -> None:
         self.data = self._data.copy()
@@ -267,14 +269,15 @@
     def get_fits_data(self, probe_diameter: float, ind: float | list[float]) -> None:
         indent = self.get_indent()
         indent_x_pred = indent['ind'].to_numpy()
         self.indent_param, self.indent_R2, indent_y_pred = self.fit_indent()
 
         self.max_ind = np.max(indent['ind'])
         self.max_f = np.max(indent['f'])
+        self.t_ind = np.max(indent['t'])
 
         if isinstance(ind, float):
             self.hertzian_param, self.hertzian_R2, hertzian_y_pred = self.fit_indent_until(
                 probe_diameter, ind)
             hertzian_x_pred = self.get_indent_until(ind)['ind'].to_numpy()
         elif isinstance(ind, list) and len(ind) == 2:
             self.hertzian_param, self.hertzian_R2, hertzian_y_pred = self.fit_indent_between(
@@ -386,26 +389,29 @@
         sleep(1)
         return fig
 
     def get_all_fits(self) -> dict:
         fit_results_dict = {
             'max_ind': self.max_ind,
             'max_f': self.max_f,
+            't_ind': self.t_ind,
 
             'vel_ind': self.vel_ind,
             'vel_z': self.vel_z,
 
             'indent_a': self.indent_param[0],
             'indent_b': self.indent_param[1],
             'indent_c': self.indent_param[2],
             'indent_R2': self.indent_R2,
 
             'Hertzian_E': self.hertzian_param[0],
             'Hertzian_R2': self.hertzian_R2,
 
+            't_dwell': self.t_dwell,
+
             'dwell_c': self.dwell_param[0],
             'dwell_tau1': self.dwell_param[1],
             'dwell_tau2': self.dwell_param[2],
             'dwell_tauMax': max(self.dwell_param[1], self.dwell_param[2]),
             'dwell_tauMin': min(self.dwell_param[1], self.dwell_param[2]),
             'dwell_yf': self.dwell_param[3],
             'dwell_R2': self.dwell_R2,
```

### Comparing `pyrtz2-1.2.2/pyrtz2/fit.py` & `pyrtz2-1.2.3/pyrtz2/fit.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/pyrtz2/src/components/annotator.py` & `pyrtz2-1.2.3/pyrtz2/src/components/annotator.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/pyrtz2/src/components/contact_controls.py` & `pyrtz2-1.2.3/pyrtz2/src/components/contact_controls.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/pyrtz2/src/components/curve_dropdown.py` & `pyrtz2-1.2.3/pyrtz2/src/components/curve_dropdown.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/pyrtz2/src/components/downloader.py` & `pyrtz2-1.2.3/pyrtz2/src/components/downloader.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/pyrtz2/src/components/experiment_loader.py` & `pyrtz2-1.2.3/pyrtz2/src/components/experiment_loader.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/pyrtz2/src/components/fig.py` & `pyrtz2-1.2.3/pyrtz2/src/components/fig.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/pyrtz2/src/components/fig_frame.py` & `pyrtz2-1.2.3/pyrtz2/src/components/fig_frame.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/pyrtz2/src/components/fitter.py` & `pyrtz2-1.2.3/pyrtz2/src/components/fitter.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/pyrtz2/src/components/ids.py` & `pyrtz2-1.2.3/pyrtz2/src/components/ids.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/pyrtz2/src/components/image.py` & `pyrtz2-1.2.3/pyrtz2/src/components/image.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/pyrtz2/src/components/image_controls.py` & `pyrtz2-1.2.3/pyrtz2/src/components/image_controls.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/pyrtz2/src/components/image_frame.py` & `pyrtz2-1.2.3/pyrtz2/src/components/image_frame.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/pyrtz2/src/components/image_loader.py` & `pyrtz2-1.2.3/pyrtz2/src/components/image_loader.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/pyrtz2/src/components/layout.py` & `pyrtz2-1.2.3/pyrtz2/src/components/layout.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/pyrtz2/src/components/loader.py` & `pyrtz2-1.2.3/pyrtz2/src/components/loader.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/pyrtz2/src/components/toolbox.py` & `pyrtz2-1.2.3/pyrtz2/src/components/toolbox.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/pyrtz2/src/utils/processor.py` & `pyrtz2-1.2.3/pyrtz2/src/utils/processor.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/pyrtz2/src/utils/utils.py` & `pyrtz2-1.2.3/pyrtz2/src/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.2/PKG-INFO` & `pyrtz2-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrtz2
-Version: 1.2.2
+Version: 1.2.3
 Summary: Force spectroscopy in Python
 Author-email: "Hoseyn A. Amiri" <aamirihoseyn@gmail.com>
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: dash
 Requires-Dist: dash-bootstrap-components
```

