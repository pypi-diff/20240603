# Comparing `tmp/linerate-1.0.0.tar.gz` & `tmp/linerate-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linerate-1.0.0.tar", max compression
+gzip compressed data, was "linerate-1.0.1.tar", max compression
```

## Comparing `linerate-1.0.0.tar` & `linerate-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1059 2024-04-08 11:36:41.365230 linerate-1.0.0/LICENSE
--rw-r--r--   0        0        0     3324 2024-04-08 11:36:41.365230 linerate-1.0.0/README.md
--rw-r--r--   0        0        0      221 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/__init__.py
--rw-r--r--   0        0        0      464 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/equations/__init__.py
--rw-r--r--   0        0        0      148 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/equations/cigre601/__init__.py
--rw-r--r--   0        0        0    22018 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/equations/cigre601/convective_cooling.py
--rw-r--r--   0        0        0        0 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/equations/cigre601/py.typed
--rw-r--r--   0        0        0     7634 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/equations/cigre601/solar_heating.py
--rw-r--r--   0        0        0      147 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/equations/ieee738/__init__.py
--rw-r--r--   0        0        0    11546 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/equations/ieee738/convective_cooling.py
--rw-r--r--   0        0        0        0 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/equations/ieee738/py.typed
--rw-r--r--   0        0        0     4559 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/equations/ieee738/solar_heating.py
--rw-r--r--   0        0        0     5969 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/equations/joule_heating.py
--rw-r--r--   0        0        0      331 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/equations/math.py
--rw-r--r--   0        0        0        0 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/equations/py.typed
--rw-r--r--   0        0        0     1351 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/equations/radiative_cooling.py
--rw-r--r--   0        0        0     7276 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/equations/solar_angles.py
--rw-r--r--   0        0        0    21848 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/model.py
--rw-r--r--   0        0        0        0 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/py.typed
--rw-r--r--   0        0        0     5754 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/solver.py
--rw-r--r--   0        0        0     6697 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/types.py
--rw-r--r--   0        0        0     1476 2024-04-08 11:36:41.369230 linerate-1.0.0/linerate/units.py
--rw-r--r--   0        0        0     2227 2024-04-08 11:37:30.785199 linerate-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4060 1970-01-01 00:00:00.000000 linerate-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-06-03 09:57:16.162075 linerate-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3324 2024-06-03 09:57:16.162075 linerate-1.0.1/README.md
+-rw-r--r--   0        0        0      221 2024-06-03 09:57:16.166075 linerate-1.0.1/linerate/__init__.py
+-rw-r--r--   0        0        0      464 2024-06-03 09:57:16.166075 linerate-1.0.1/linerate/equations/__init__.py
+-rw-r--r--   0        0        0      148 2024-06-03 09:57:16.166075 linerate-1.0.1/linerate/equations/cigre601/__init__.py
+-rw-r--r--   0        0        0    22018 2024-06-03 09:57:16.166075 linerate-1.0.1/linerate/equations/cigre601/convective_cooling.py
+-rw-r--r--   0        0        0        0 2024-06-03 09:57:16.166075 linerate-1.0.1/linerate/equations/cigre601/py.typed
+-rw-r--r--   0        0        0     7634 2024-06-03 09:57:16.166075 linerate-1.0.1/linerate/equations/cigre601/solar_heating.py
+-rw-r--r--   0        0        0      147 2024-06-03 09:57:16.166075 linerate-1.0.1/linerate/equations/ieee738/__init__.py
+-rw-r--r--   0        0        0    11546 2024-06-03 09:57:16.166075 linerate-1.0.1/linerate/equations/ieee738/convective_cooling.py
+-rw-r--r--   0        0        0        0 2024-06-03 09:57:16.166075 linerate-1.0.1/linerate/equations/ieee738/py.typed
+-rw-r--r--   0        0        0     4559 2024-06-03 09:57:16.166075 linerate-1.0.1/linerate/equations/ieee738/solar_heating.py
+-rw-r--r--   0        0        0     5969 2024-06-03 09:57:16.166075 linerate-1.0.1/linerate/equations/joule_heating.py
+-rw-r--r--   0        0        0      331 2024-06-03 09:57:16.166075 linerate-1.0.1/linerate/equations/math.py
+-rw-r--r--   0        0        0        0 2024-06-03 09:57:16.166075 linerate-1.0.1/linerate/equations/py.typed
+-rw-r--r--   0        0        0     1351 2024-06-03 09:57:16.166075 linerate-1.0.1/linerate/equations/radiative_cooling.py
+-rw-r--r--   0        0        0     7631 2024-06-03 09:57:16.166075 linerate-1.0.1/linerate/equations/solar_angles.py
+-rw-r--r--   0        0        0    21890 2024-06-03 09:57:16.166075 linerate-1.0.1/linerate/model.py
+-rw-r--r--   0        0        0        0 2024-06-03 09:57:16.166075 linerate-1.0.1/linerate/py.typed
+-rw-r--r--   0        0        0     5754 2024-06-03 09:57:16.166075 linerate-1.0.1/linerate/solver.py
+-rw-r--r--   0        0        0     6697 2024-06-03 09:57:16.166075 linerate-1.0.1/linerate/types.py
+-rw-r--r--   0        0        0     1476 2024-06-03 09:57:16.166075 linerate-1.0.1/linerate/units.py
+-rw-r--r--   0        0        0     2227 2024-06-03 09:58:04.342474 linerate-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4060 1970-01-01 00:00:00.000000 linerate-1.0.1/PKG-INFO
```

### Comparing `linerate-1.0.0/LICENSE` & `linerate-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `linerate-1.0.0/README.md` & `linerate-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `linerate-1.0.0/linerate/equations/cigre601/convective_cooling.py` & `linerate-1.0.1/linerate/equations/cigre601/convective_cooling.py`

 * *Files identical despite different names*

### Comparing `linerate-1.0.0/linerate/equations/cigre601/solar_heating.py` & `linerate-1.0.1/linerate/equations/cigre601/solar_heating.py`

 * *Files identical despite different names*

### Comparing `linerate-1.0.0/linerate/equations/ieee738/convective_cooling.py` & `linerate-1.0.1/linerate/equations/ieee738/convective_cooling.py`

 * *Files identical despite different names*

### Comparing `linerate-1.0.0/linerate/equations/ieee738/solar_heating.py` & `linerate-1.0.1/linerate/equations/ieee738/solar_heating.py`

 * *Files identical despite different names*

### Comparing `linerate-1.0.0/linerate/equations/joule_heating.py` & `linerate-1.0.1/linerate/equations/joule_heating.py`

 * *Files identical despite different names*

### Comparing `linerate-1.0.0/linerate/equations/radiative_cooling.py` & `linerate-1.0.1/linerate/equations/radiative_cooling.py`

 * *Files identical despite different names*

### Comparing `linerate-1.0.0/linerate/equations/solar_angles.py` & `linerate-1.0.1/linerate/equations/solar_angles.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,40 +20,46 @@
 def _get_minute_of_hour(when: Date) -> Unitless:
     HourResolutionType = np.datetime64(1, "h")
     MinuteResolutionType = np.datetime64(1, "m")
 
     return (when.astype(MinuteResolutionType) - when.astype(HourResolutionType)).astype(float)
 
 
-def compute_hour_angle_relative_to_noon(when: Date) -> Radian:
+def compute_hour_angle_relative_to_noon(when: Date, longitude: Degrees) -> Radian:
     r"""Compute the hour angle.
 
     Described in the text on p. 18 of :cite:p:`ieee738`. The hour angle is the number of hours
     from noon times 15^\circ. This means that the hour angle for 11:00 is -15^\circ, and the
     hour angle for 14:00 is 30^\circ.
 
     This function converts the hour angle to radians by multiplying it by \frac{\pi}{12},
     which is the same as 15^\circ.
 
     The hour angle is used when calculating the solar altitude.
+    This function does not take into account the difference between apparent/actual
+    and mean solar time, which means that the result may be up to 15 minutes from the
+    correct hour angle.
 
     Parameters
     ----------
     when:
         The time and date.
 
     Returns
     -------
     Union[float, float64, ndarray[Any, dtype[float64]]]
         :math:'\omega~\left[\text{radian}\right]`. The hour angle relative to noon.
     """
-    hour = _get_hour_of_day(when)
-    minute = _get_minute_of_hour(when)
+    utc_hour = _get_hour_of_day(when)
+    utc_minute = _get_minute_of_hour(when)
     pi = np.pi
-    return (-12 + hour + minute / 60) * (pi / 12)  # pi/12 is 15 degrees
+    # We add longitude/15 since 15 degrees of longitude increases solar hour by 1
+    return np.mod((-12 + utc_hour + utc_minute / 60 + longitude / 15), 24) * (
+        pi / 12
+    )  # pi/12 is 15 degrees
 
 
 def compute_solar_declination(
     when: Date,
 ) -> Radian:
     r"""Compute the solar declination
```

### Comparing `linerate-1.0.0/linerate/model.py` & `linerate-1.0.1/linerate/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -335,15 +335,15 @@
         F = self.span.ground_albedo
         phi = self.span.latitude
         gamma_c = self.span.conductor_azimuth
         y = self.span.conductor_altitude
         N_s = self.weather.clearness_ratio
         D = self.span.conductor.conductor_diameter
 
-        omega = solar_angles.compute_hour_angle_relative_to_noon(self.time)
+        omega = solar_angles.compute_hour_angle_relative_to_noon(self.time, self.span.longitude)
         delta = solar_angles.compute_solar_declination(self.time)
         sin_H_s = solar_angles.compute_sin_solar_altitude(phi, delta, omega)
         chi = solar_angles.compute_solar_azimuth_variable(phi, delta, omega)
         C = solar_angles.compute_solar_azimuth_constant(chi, omega)
         gamma_s = solar_angles.compute_solar_azimuth(C, chi)  # Z_c in IEEE
         cos_eta = solar_angles.compute_cos_solar_effective_incidence_angle(
             sin_H_s, gamma_s, gamma_c
@@ -487,15 +487,15 @@
     ) -> WattPerMeter:
         alpha_s = self.span.conductor.solar_absorptivity  # alpha in IEEE
         phi = self.span.latitude  # Lat in IEEE
         gamma_c = self.span.conductor_azimuth  # Z_l i IEEE
         y = self.span.conductor_altitude  # H_e in IEEE
         D = self.span.conductor.conductor_diameter  # D_0 in IEEE
 
-        omega = solar_angles.compute_hour_angle_relative_to_noon(self.time)
+        omega = solar_angles.compute_hour_angle_relative_to_noon(self.time, self.span.longitude)
         delta = solar_angles.compute_solar_declination(self.time)
         sin_H_c = solar_angles.compute_sin_solar_altitude(phi, delta, omega)
         Q_s = ieee738.solar_heating.compute_total_heat_flux_density(sin_H_c, True)
         K_solar = ieee738.solar_heating.compute_solar_altitude_correction_factor(y)
         Q_se = ieee738.solar_heating.compute_elevation_correction_factor(K_solar, Q_s)
         chi = solar_angles.compute_solar_azimuth_variable(phi, delta, omega)
         C = solar_angles.compute_solar_azimuth_constant(chi, omega)
```

### Comparing `linerate-1.0.0/linerate/solver.py` & `linerate-1.0.1/linerate/solver.py`

 * *Files identical despite different names*

### Comparing `linerate-1.0.0/linerate/types.py` & `linerate-1.0.1/linerate/types.py`

 * *Files identical despite different names*

### Comparing `linerate-1.0.0/linerate/units.py` & `linerate-1.0.1/linerate/units.py`

 * *Files identical despite different names*

### Comparing `linerate-1.0.0/pyproject.toml` & `linerate-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "linerate"
-version = "1.0.0"
+version = "1.0.1"
 description = "Library for computing line ampacity ratings for overhead lines"
 authors = ["Statnett Datascience <Datascience.Drift@Statnett.no>", "Yngve Mardal Moe <yngve.m.moe@gmail.com>"]
 repository = "https://github.com/statnett/linerate.git"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
```

### Comparing `linerate-1.0.0/PKG-INFO` & `linerate-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linerate
-Version: 1.0.0
+Version: 1.0.1
 Summary: Library for computing line ampacity ratings for overhead lines
 Home-page: https://github.com/statnett/linerate.git
 Author: Statnett Datascience
 Author-email: Datascience.Drift@Statnett.no
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

