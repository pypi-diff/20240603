# Comparing `tmp/thermolib-0.3.1.tar.gz` & `tmp/thermolib-0.3.2.tar.gz`

## Comparing `thermolib-0.3.1.tar` & `thermolib-0.3.2.tar`

### file list

```diff
@@ -1,45 +1,49 @@
--rw-r--r--   0        0        0      655 1970-01-01 00:00:00.000000 thermolib-0.3.1/Cargo.toml
--rw-r--r--   0        0        0       22 2024-03-13 13:32:17.000000 thermolib-0.3.1/.gitignore
--rw-r--r--   0        0        0   121546 2024-05-27 08:23:40.000000 thermolib-0.3.1/Cargo.lock
--rw-r--r--   0        0        0     1082 2024-02-20 03:32:56.000000 thermolib-0.3.1/LICENSE
--rw-r--r--   0        0        0      167 2024-02-20 03:32:56.000000 thermolib-0.3.1/README.md
--rw-r--r--   0        0        0       76 2024-05-22 09:31:41.000000 thermolib-0.3.1/build.rs
--rw-r--r--   0        0        0     6045 2024-05-27 08:19:27.000000 thermolib-0.3.1/res/22DimethylButane.json
--rw-r--r--   0        0        0     5756 2024-05-27 08:19:27.000000 thermolib-0.3.1/res/23DimethylButane.json
--rw-r--r--   0        0        0     6154 2024-05-27 08:19:27.000000 thermolib-0.3.1/res/3MethylPentane.json
--rw-r--r--   0        0        0     5573 2024-05-27 08:19:27.000000 thermolib-0.3.1/res/C4F10.json
--rw-r--r--   0        0        0     5584 2024-05-27 08:19:27.000000 thermolib-0.3.1/res/C5F12.json
--rw-r--r--   0        0        0     5594 2024-05-27 08:19:27.000000 thermolib-0.3.1/res/C6F14.json
--rw-r--r--   0        0        0     6177 2024-04-10 07:36:35.000000 thermolib-0.3.1/res/SO2.json
--rw-r--r--   0        0        0       85 2024-05-27 08:19:27.000000 thermolib-0.3.1/src/bin/thermo.rs
--rw-r--r--   0        0        0      138 2024-05-27 08:19:27.000000 thermolib-0.3.1/src/bin/thermo.slint
--rw-r--r--   0        0        0     6284 2024-05-27 08:19:27.000000 thermolib-0.3.1/src/core/core_traits.rs
--rw-r--r--   0        0        0    27734 2024-05-27 08:19:27.000000 thermolib-0.3.1/src/core/generic_a.rs
--rw-r--r--   0        0        0      729 2024-05-27 08:19:27.000000 thermolib-0.3.1/src/core/ideal_cv.rs
--rw-r--r--   0        0        0     6171 2024-05-27 08:19:27.000000 thermolib-0.3.1/src/core/readme.md
--rw-r--r--   0        0        0      894 2024-05-21 12:58:36.000000 thermolib-0.3.1/src/core/tlerr.rs
--rw-r--r--   0        0        0      259 2024-05-27 08:19:27.000000 thermolib-0.3.1/src/core.rs
--rw-r--r--   0        0        0     7673 2024-05-24 13:17:30.000000 thermolib-0.3.1/src/helmholtz/alpha.rs
--rw-r--r--   0        0        0     4854 2024-05-27 08:19:27.000000 thermolib-0.3.1/src/helmholtz/alpha_i.rs
--rw-r--r--   0        0        0     8049 2024-05-27 08:19:27.000000 thermolib-0.3.1/src/helmholtz/alpha_r.rs
--rw-r--r--   0        0        0     2959 2024-05-27 08:19:27.000000 thermolib-0.3.1/src/helmholtz/anc_equ.rs
--rw-r--r--   0        0        0      250 2024-04-03 11:57:39.000000 thermolib-0.3.1/src/helmholtz.rs
--rw-r--r--   0        0        0      471 2024-05-22 09:31:41.000000 thermolib-0.3.1/src/lib.rs
--rw-r--r--   0        0        0     1425 2024-05-27 08:19:27.000000 thermolib-0.3.1/src/pc_saft/alpha.rs
--rw-r--r--   0        0        0     7501 2024-05-27 08:19:27.000000 thermolib-0.3.1/src/pc_saft/alpha_r.rs
--rw-r--r--   0        0        0    31367 2024-05-27 08:19:27.000000 thermolib-0.3.1/src/pc_saft/disp.rs
--rw-r--r--   0        0        0    20494 2024-05-27 08:19:27.000000 thermolib-0.3.1/src/pc_saft/hc.rs
--rw-r--r--   0        0        0      248 2024-05-22 09:31:41.000000 thermolib-0.3.1/src/pc_saft.rs
--rw-r--r--   0        0        0     1939 2024-05-22 07:46:25.000000 thermolib-0.3.1/src/pr/density_pr.rs
--rw-r--r--   0        0        0     9587 2024-05-27 08:19:27.000000 thermolib-0.3.1/src/pr/pr_pure.rs
--rw-r--r--   0        0        0      155 2024-05-22 09:31:41.000000 thermolib-0.3.1/src/pr.rs
--rw-r--r--   0        0        0    10013 2024-05-27 08:19:27.000000 thermolib-0.3.1/src/python.rs
--rw-r--r--   0        0        0      550 2024-05-27 08:19:27.000000 thermolib-0.3.1/tests/find_json.rs
--rw-r--r--   0        0        0     2020 2024-05-27 08:19:27.000000 thermolib-0.3.1/tests/internals/mod.rs
--rw-r--r--   0        0        0      406 2024-05-22 08:33:46.000000 thermolib-0.3.1/tests/main.cpp
--rw-r--r--   0        0        0      747 2024-05-27 08:19:27.000000 thermolib-0.3.1/tests/main.py
--rw-r--r--   0        0        0   118429 2024-05-22 08:34:33.000000 thermolib-0.3.1/tests/pcsaft.cpp
--rw-r--r--   0        0        0     5416 2024-05-21 11:39:49.000000 thermolib-0.3.1/tests/pcsaft.h
--rw-r--r--   0        0        0     8006 2024-05-27 08:19:27.000000 thermolib-0.3.1/tests/test_fluid.rs
--rw-r--r--   0        0        0      406 2024-03-27 02:49:30.000000 thermolib-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      669 1970-01-01 00:00:00.000000 thermolib-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      655 1970-01-01 00:00:00.000000 thermolib-0.3.2/Cargo.toml
+-rw-r--r--   0        0        0       22 2024-03-13 13:32:17.000000 thermolib-0.3.2/.gitignore
+-rw-r--r--   0        0        0   121546 2024-06-03 07:20:11.000000 thermolib-0.3.2/Cargo.lock
+-rw-r--r--   0        0        0     1082 2024-02-20 03:32:56.000000 thermolib-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1795 2024-06-03 07:18:45.000000 thermolib-0.3.2/README.md
+-rw-r--r--   0        0        0       76 2024-05-22 09:31:41.000000 thermolib-0.3.2/build.rs
+-rw-r--r--   0        0        0     6045 2024-05-27 08:19:27.000000 thermolib-0.3.2/res/22DimethylButane.json
+-rw-r--r--   0        0        0     5756 2024-05-27 08:19:27.000000 thermolib-0.3.2/res/23DimethylButane.json
+-rw-r--r--   0        0        0     6154 2024-05-27 08:19:27.000000 thermolib-0.3.2/res/3MethylPentane.json
+-rw-r--r--   0        0        0     5573 2024-05-27 08:19:27.000000 thermolib-0.3.2/res/C4F10.json
+-rw-r--r--   0        0        0     5584 2024-05-27 08:19:27.000000 thermolib-0.3.2/res/C5F12.json
+-rw-r--r--   0        0        0     5594 2024-05-27 08:19:27.000000 thermolib-0.3.2/res/C6F14.json
+-rw-r--r--   0        0        0     6177 2024-06-01 09:16:20.000000 thermolib-0.3.2/res/SO2.json
+-rw-r--r--   0        0        0       85 2024-05-27 08:19:27.000000 thermolib-0.3.2/src/bin/thermo.rs
+-rw-r--r--   0        0        0      138 2024-05-27 08:19:27.000000 thermolib-0.3.2/src/bin/thermo.slint
+-rw-r--r--   0        0        0     1342 2024-06-03 07:18:45.000000 thermolib-0.3.2/src/core/core_traits.md
+-rw-r--r--   0        0        0     6405 2024-06-03 07:18:45.000000 thermolib-0.3.2/src/core/core_traits.rs
+-rw-r--r--   0        0        0     4906 2024-06-03 07:18:45.000000 thermolib-0.3.2/src/core/generic_a.md
+-rw-r--r--   0        0        0    29225 2024-06-03 07:18:45.000000 thermolib-0.3.2/src/core/generic_a.rs
+-rw-r--r--   0        0        0     2231 2024-06-03 07:18:45.000000 thermolib-0.3.2/src/core/ideal_cv.md
+-rw-r--r--   0        0        0     4548 2024-06-03 07:18:45.000000 thermolib-0.3.2/src/core/ideal_cv.rs
+-rw-r--r--   0        0        0      894 2024-05-21 12:58:36.000000 thermolib-0.3.2/src/core/tlerr.rs
+-rw-r--r--   0        0        0      259 2024-05-27 08:19:27.000000 thermolib-0.3.2/src/core.rs
+-rw-r--r--   0        0        0     7668 2024-06-03 07:18:45.000000 thermolib-0.3.2/src/helmholtz/alpha.rs
+-rw-r--r--   0        0        0     4950 2024-06-03 07:18:45.000000 thermolib-0.3.2/src/helmholtz/alpha_i.rs
+-rw-r--r--   0        0        0     8310 2024-06-03 07:18:45.000000 thermolib-0.3.2/src/helmholtz/alpha_r.rs
+-rw-r--r--   0        0        0     2959 2024-05-27 08:19:27.000000 thermolib-0.3.2/src/helmholtz/anc_equ.rs
+-rw-r--r--   0        0        0      250 2024-04-03 11:57:39.000000 thermolib-0.3.2/src/helmholtz.rs
+-rw-r--r--   0        0        0      480 2024-06-03 07:18:45.000000 thermolib-0.3.2/src/lib.rs
+-rw-r--r--   0        0        0     1441 2024-06-03 07:18:45.000000 thermolib-0.3.2/src/pc_saft/alpha.rs
+-rw-r--r--   0        0        0     7607 2024-06-03 07:18:45.000000 thermolib-0.3.2/src/pc_saft/alpha_r.rs
+-rw-r--r--   0        0        0    31367 2024-05-30 03:12:06.000000 thermolib-0.3.2/src/pc_saft/disp.rs
+-rw-r--r--   0        0        0    20494 2024-05-27 08:19:27.000000 thermolib-0.3.2/src/pc_saft/hc.rs
+-rw-r--r--   0        0        0      248 2024-05-30 03:11:49.000000 thermolib-0.3.2/src/pc_saft.rs
+-rw-r--r--   0        0        0     1939 2024-06-03 07:18:45.000000 thermolib-0.3.2/src/pr/density.rs
+-rw-r--r--   0        0        0     6423 2024-06-03 07:18:45.000000 thermolib-0.3.2/src/pr/pr_a.rs
+-rw-r--r--   0        0        0     1901 2024-06-03 07:18:45.000000 thermolib-0.3.2/src/pr/pr_ar.md
+-rw-r--r--   0        0        0     5235 2024-06-03 07:18:45.000000 thermolib-0.3.2/src/pr/pr_ar.rs
+-rw-r--r--   0        0        0      184 2024-06-03 07:18:45.000000 thermolib-0.3.2/src/pr.rs
+-rw-r--r--   0        0        0    15576 2024-06-03 07:18:45.000000 thermolib-0.3.2/src/python.rs
+-rw-r--r--   0        0        0      550 2024-05-27 08:19:27.000000 thermolib-0.3.2/tests/find_json.rs
+-rw-r--r--   0        0        0     2020 2024-05-27 08:19:27.000000 thermolib-0.3.2/tests/internals/mod.rs
+-rw-r--r--   0        0        0      406 2024-05-22 08:33:46.000000 thermolib-0.3.2/tests/main.cpp
+-rw-r--r--   0        0        0      747 2024-05-27 08:19:27.000000 thermolib-0.3.2/tests/main.py
+-rw-r--r--   0        0        0   118429 2024-05-22 08:34:33.000000 thermolib-0.3.2/tests/pcsaft.cpp
+-rw-r--r--   0        0        0     5416 2024-05-21 11:39:49.000000 thermolib-0.3.2/tests/pcsaft.h
+-rw-r--r--   0        0        0     8006 2024-05-27 08:19:27.000000 thermolib-0.3.2/tests/test_fluid.rs
+-rw-r--r--   0        0        0      406 2024-03-27 02:49:30.000000 thermolib-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2297 1970-01-01 00:00:00.000000 thermolib-0.3.2/PKG-INFO
```

### Comparing `thermolib-0.3.1/Cargo.toml` & `thermolib-0.3.2/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "thermolib"
 build = "build.rs"
-version = "0.3.1"
+version = "0.3.2"
 edition = "2021"
 license = "MIT"
 repository = "https://github.com/shaw-yu2020/thermolib"
 description = "An open-source library for the calculation of fluid properties"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `thermolib-0.3.1/Cargo.lock` & `thermolib-0.3.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -3620,15 +3620,15 @@
 name = "text-size"
 version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f18aa187839b2bdb1ad2fa35ead8c4c2976b64e4363c386d45ac0f7ee85c9233"
 
 [[package]]
 name = "thermolib"
-version = "0.3.1"
+version = "0.3.2"
 dependencies = [
  "anyhow",
  "pyo3",
  "serde",
  "serde_json",
  "slint",
  "slint-build",
```

### Comparing `thermolib-0.3.1/LICENSE` & `thermolib-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `thermolib-0.3.1/res/22DimethylButane.json` & `thermolib-0.3.2/res/22DimethylButane.json`

 * *Files identical despite different names*

### Comparing `thermolib-0.3.1/res/23DimethylButane.json` & `thermolib-0.3.2/res/23DimethylButane.json`

 * *Files identical despite different names*

### Comparing `thermolib-0.3.1/res/3MethylPentane.json` & `thermolib-0.3.2/res/3MethylPentane.json`

 * *Files identical despite different names*

### Comparing `thermolib-0.3.1/res/C4F10.json` & `thermolib-0.3.2/res/C4F10.json`

 * *Files identical despite different names*

### Comparing `thermolib-0.3.1/res/C5F12.json` & `thermolib-0.3.2/res/C5F12.json`

 * *Files identical despite different names*

### Comparing `thermolib-0.3.1/res/C6F14.json` & `thermolib-0.3.2/res/C6F14.json`

 * *Files identical despite different names*

### Comparing `thermolib-0.3.1/res/SO2.json` & `thermolib-0.3.2/res/SO2.json`

 * *Files identical despite different names*

### Comparing `thermolib-0.3.1/src/core/core_traits.rs` & `thermolib-0.3.2/src/core/core_traits.rs`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,16 @@
     /// > $$T^2\left(\frac{\partial^2a^i}{\partial T^2}\right)_D$$  
     /// > fn iT2D1(&self, _T:f64) -> f64; Equal to = $0$  
     /// > fn iT2D2(&self, _T:f64) -> f64; Equal to = $0$  
     fn iT2(&self, _T: f64) -> f64 {
         println!("no implementation for CalcAi::iT2(), return 0.0");
         0.0
     }
+    /// Used for trait::Setting
+    fn set_R(&mut self, R: f64);
 }
 /// Partial derivatives of residual part of fundumental helmholtz equation of state.  
 /// Equal to $$ T^(dT) * D^(dD) * Ar_DT(dT)_DD(dD) $$
 #[allow(non_snake_case)]
 pub trait CalcAr {
     /// > fn rT0D0(&self, _T: f64, _D: f64) -> f64; Equal to =  
     /// > $$a^r\left(T,D\right)$$  
@@ -63,26 +65,28 @@
     }
     /// > fn rT2D0(&self, _T: f64, _D: f64) -> f64; Equal to =  
     /// > $$T^2\left(\frac{\partial^2a^r}{\partial T^2}\right)_D$$  
     fn rT2D0(&self, _T: f64, _D: f64) -> f64 {
         println!("no implementation for CalcAr::rT2D0(), return 0.0");
         0.0
     }
+    /// Used for trait::Setting
+    fn set_RM(&mut self, R: f64, M: f64);
 }
 /// Settings for fundumental helmholtz equation of state.
 #[allow(non_snake_case)]
 pub trait Setting {
     fn set_mass_unit(&mut self);
     fn set_molar_unit(&mut self);
 }
 /// Flash calculation of fundumental helmholtz equation of state.
 #[allow(non_snake_case)]
 pub trait Flash {
     /// Temperature and Density UNCHECKED
-    fn td_unchecked(&mut self, _T: f64, _D: f64) -> anyhow::Result<()>;
+    fn td_unchecked(&mut self, _T: f64, _D: f64);
     /// Critical point
     fn c_flash(&mut self) -> anyhow::Result<()>;
     /// Temperature of saturated state
     fn t_flash(&mut self, _Ts: f64) -> anyhow::Result<()>;
     /// Temperature and Density
     fn td_flash(&mut self, _T: f64, _D: f64) -> anyhow::Result<()>;
     /// Temperature and Pressure
@@ -91,14 +95,16 @@
 /// Get thermodynamic properties of corresponding fluid phase.
 #[allow(non_snake_case)]
 pub trait Prop {
     /// Temperature
     fn T(&self) -> anyhow::Result<f64>;
     /// Density
     fn D(&self) -> anyhow::Result<f64>;
+    /// compressibility factor
+    fn Z(&mut self) -> anyhow::Result<f64>;
     /// pressure
     fn p(&mut self) -> anyhow::Result<f64>;
     fn Dp_DT_D(&mut self) -> anyhow::Result<f64>;
     fn Dp_DD_T(&mut self) -> anyhow::Result<f64>;
     /// isochoric heat capacity
     fn cv(&mut self) -> anyhow::Result<f64>;
     /// isobaric heat capacity
@@ -122,16 +128,14 @@
     fn a(&mut self) -> anyhow::Result<f64>;
     fn a_res(&mut self) -> anyhow::Result<f64>;
     /// gibbs energy
     fn g(&mut self) -> anyhow::Result<f64>;
     fn Dg_DT_D(&mut self) -> anyhow::Result<f64>;
     fn Dg_DD_T(&mut self) -> anyhow::Result<f64>;
     fn g_res(&mut self) -> anyhow::Result<f64>;
-    /// compressibility factor
-    fn Z(&mut self) -> anyhow::Result<f64>;
     /// second virial coefficient
     fn B(&mut self) -> anyhow::Result<f64>;
     /// third virial coefficient
     fn C(&mut self) -> anyhow::Result<f64>;
     /// isothermal expansion coefficient
     fn k_T(&mut self) -> anyhow::Result<f64>;
     /// isentropic expansion coefficient
```

### Comparing `thermolib-0.3.1/src/core/generic_a.rs` & `thermolib-0.3.2/src/core/generic_a.rs`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #[allow(non_snake_case)]
 #[derive(Serialize, Deserialize, Debug, Clone)]
 pub struct GenericA<I: CalcAi, R: CalcAr> {
     ai: I,
     ar: R,
     R: f64,
     M: f64,
-    #[serde(skip, default = "default_phase")]
+    #[serde(skip, default)]
     phase: Phase,
     #[serde(skip, default)]
     aT0D0: Cache,
     #[serde(skip, default)]
     aT0D1: Cache,
     #[serde(skip, default)]
     aT0D2: Cache,
@@ -41,54 +41,82 @@
     #[serde(skip, default)]
     aT1D1: Cache,
     #[serde(skip, default)]
     aT2D0: Cache,
     #[serde(skip, default)]
     aT0D0_sub_aT1D0: Cache,
 }
-fn default_phase() -> Phase {
-    Phase::One { T: 1.0, D: 1.0 }
+impl Default for Phase {
+    fn default() -> Self {
+        Phase::One { T: 1.0, D: 1.0 }
+    }
 }
 #[allow(non_snake_case)]
 impl<I: CalcAi, R: CalcAr> GenericA<I, R> {
     pub fn new(ai: I, ar: R, M: f64) -> Self {
         GenericA {
             ai,
             ar,
             M,
             R: 8.314462618,
-            phase: default_phase(),
+            phase: Phase::default(),
             aT0D0: Cache::default(),
             aT0D1: Cache::default(),
             aT0D2: Cache::default(),
             aT1D0: Cache::default(),
             aT1D1: Cache::default(),
             aT2D0: Cache::default(),
             aT0D0_sub_aT1D0: Cache::default(),
         }
     }
 }
 /// Get internal fields of generic struct
 #[allow(non_snake_case)]
-impl<I: CalcAi, R: CalcAr> GenericA<I, R> {
-    pub fn mut_ref_ai(&mut self) -> &mut I {
-        &mut self.ai
+impl<I: CalcAi + Clone, R: CalcAr + Clone> GenericA<I, R> {
+    pub fn set_ai<A: CalcAi>(&self, ai: A) -> GenericA<A, R> {
+        GenericA::<A, R> {
+            ai,
+            R: self.R,
+            M: self.M,
+            ar: self.ar.clone(),
+            phase: Phase::default(),
+            aT0D0: Cache::default(),
+            aT0D1: Cache::default(),
+            aT0D2: Cache::default(),
+            aT1D0: Cache::default(),
+            aT1D1: Cache::default(),
+            aT2D0: Cache::default(),
+            aT0D0_sub_aT1D0: Cache::default(),
+        }
     }
-    pub fn mut_ref_ar(&mut self) -> &mut R {
-        &mut self.ar
+    pub fn set_ar<A: CalcAr>(&self, ar: A) -> GenericA<I, A> {
+        GenericA::<I, A> {
+            ar,
+            R: self.R,
+            M: self.M,
+            ai: self.ai.clone(),
+            phase: Phase::default(),
+            aT0D0: Cache::default(),
+            aT0D1: Cache::default(),
+            aT0D2: Cache::default(),
+            aT1D0: Cache::default(),
+            aT1D1: Cache::default(),
+            aT2D0: Cache::default(),
+            aT0D0_sub_aT1D0: Cache::default(),
+        }
     }
     pub fn ref_ar(&self) -> &R {
         &self.ar
     }
-    pub fn ref_phase(&self) -> &Phase {
-        &self.phase
-    }
     pub fn set_phase(&mut self, phase: Phase) {
         self.phase = phase;
     }
+    pub fn phase(&self) -> Phase {
+        self.phase.clone()
+    }
     pub fn R(&self) -> f64 {
         self.R
     }
 }
 /// Calculate partial derivatives of fundumental helmholtz equation of state.  
 /// Equal to $$ T^(dT) * D^(dD) * A_DT(dT)_DD(dD) $$  
 /// Used to calculate thermodynamic properties.  
@@ -97,85 +125,104 @@
     /// > fn aT0D0(&self, T: f64, D: f64) -> f64; Equal to
     /// > $$a\left(T,D\right)
     /// > =a^i\left(T,D\right)
     /// > +a^r\left(T,D\right)
     /// > =iT0(T)+RT\ln D+rT0D0(T,D)$$
     fn aT0D0(&mut self, T: f64, D: f64) -> f64 {
         if self.aT0D0.T != T || self.aT0D0.D != D {
+            self.aT0D0.T = T;
+            self.aT0D0.D = D;
             self.aT0D0.value = self.ai.iT0(T) + self.R * T * D.ln() + self.ar.rT0D0(T, D);
         }
         self.aT0D0.value
     }
     /// > fn aT0D1(&self, T: f64, D: f64) -> f64; Equal to
     /// > $$D\left(\frac{\partial a}{\partial D}\right)_T
     /// > =D\left(\frac{\partial a^i}{\partial D}\right)_T
     /// > +D\left(\frac{\partial a^r}{\partial D}\right)_T
     /// > =RT+rT0D1(T,D)$$
     fn aT0D1(&mut self, T: f64, D: f64) -> f64 {
         if self.aT0D1.T != T || self.aT0D1.D != D {
+            self.aT0D1.T = T;
+            self.aT0D1.D = D;
             self.aT0D1.value = self.R * T + self.ar.rT0D1(T, D);
         }
         self.aT0D1.value
     }
     /// > fn aT0D2(&self, T: f64, D: f64) -> f64; Equal to
     /// > $$D^2\left(\frac{\partial^2a}{\partial D^2}\right)_T
     /// > =D^2\left(\frac{\partial^2a^i}{\partial D^2}\right)_T
     /// > +D^2\left(\frac{\partial^2a^r}{\partial D^2}\right)_T
     /// > =-RT+rT0D2(T,D)$$
     fn aT0D2(&mut self, T: f64, D: f64) -> f64 {
         if self.aT0D2.T != T || self.aT0D2.D != D {
+            self.aT0D2.T = T;
+            self.aT0D2.D = D;
             self.aT0D2.value = -self.R * T + self.ar.rT0D2(T, D);
         }
         self.aT0D2.value
     }
     /// > fn aT1D0(&self, T: f64, D: f64) -> f64; Equal to
     /// > $$T\left(\frac{\partial a}{\partial T}\right)_D
     /// > =T\left(\frac{\partial a^i}{\partial T}\right)_D
     /// > +T\left(\frac{\partial a^r}{\partial T}\right)_D
     /// > =iT1(T)+RT\ln D+rT1D0(T,D)$$
     fn aT1D0(&mut self, T: f64, D: f64) -> f64 {
         if self.aT1D0.T != T || self.aT1D0.D != D {
+            self.aT1D0.T = T;
+            self.aT1D0.D = D;
             self.aT1D0.value = self.ai.iT1(T) + self.R * T * D.ln() + self.ar.rT1D0(T, D);
         }
         self.aT1D0.value
     }
     /// > fn aT1D1(&self, T: f64, D: f64) -> f64; Equal to
     /// > $$TD\left(\frac{\partial^2a}{\partial T\partial D}\right)
     /// > =TD\left(\frac{\partial^2a^i}{\partial T\partial D}\right)
     /// > +TD\left(\frac{\partial^2a^r}{\partial T\partial D}\right)
     /// > =RT+rT1D1(T,D)$$
     fn aT1D1(&mut self, T: f64, D: f64) -> f64 {
         if self.aT1D1.T != T || self.aT1D1.D != D {
+            self.aT1D1.T = T;
+            self.aT1D1.D = D;
             self.aT1D1.value = self.R * T + self.ar.rT1D1(T, D)
         }
         self.aT1D1.value
     }
     /// > fn aT2D0(&self, T: f64, D: f64) -> f64; Equal to
     /// > $$T^2\left(\frac{\partial^2a}{\partial T^2}\right)_D
     /// > =T^2\left(\frac{\partial^2a^i}{\partial T^2}\right)_D
     /// > +T^2\left(\frac{\partial^2a^r}{\partial T^2}\right)_D
     /// > =iT2(T)+rT2D0(T,D)$$
     fn aT2D0(&mut self, T: f64, D: f64) -> f64 {
         if self.aT2D0.T != T || self.aT2D0.D != D {
+            self.aT2D0.T = T;
+            self.aT2D0.D = D;
             self.aT2D0.value = self.ai.iT2(T) + self.ar.rT2D0(T, D);
         }
         self.aT2D0.value
     }
     /// shit-code
     fn aT0D0_sub_aT1D0(&mut self, T: f64, D: f64) -> f64 {
         if self.aT0D0_sub_aT1D0.T != T || self.aT0D0_sub_aT1D0.D != D {
+            self.aT0D0_sub_aT1D0.T = T;
+            self.aT0D0_sub_aT1D0.D = D;
             self.aT0D0_sub_aT1D0.value =
                 self.ai.iT0(T) + self.ar.rT0D0(T, D) - self.ai.iT1(T) - self.ar.rT1D0(T, D);
         }
         self.aT0D0_sub_aT1D0.value
     }
 }
 /// Calculate thermodynamic properties of fundumental helmholtz equation of state.
 #[allow(non_snake_case)]
 impl<I: CalcAi, R: CalcAr> GenericA<I, R> {
+    /// > $$Z
+    /// > =\frac{1}{RT}D\left(\frac{\partial a}{\partial D}\right)_T$$
+    fn Z(&mut self, T: f64, D: f64) -> f64 {
+        self.aT0D1(T, D) / self.R / T
+    }
     /// > $$p
     /// > =D^2\left(\frac{\partial a}{\partial D}\right)_T$$
     fn p(&mut self, T: f64, D: f64) -> f64 {
         D * self.aT0D1(T, D)
     }
     /// > $$Dp\\_DT\\_D=\left(\frac{\partial p}{\partial T}\right)_D
     /// > =D^2\left(\frac{\partial^2a}{\partial D\partial T}\right)$$
@@ -305,19 +352,14 @@
     }
     /// > $$g\\_res
     /// > =a^r\left(T,D\right)
     /// > +D\left(\frac{\partial a^r}{\partial D}\right)_T$$
     fn g_res(&mut self, T: f64, D: f64) -> f64 {
         self.ar.rT0D0(T, D) + self.ar.rT0D1(T, D)
     }
-    /// > $$Z
-    /// > =\frac{1}{RT}D\left(\frac{\partial a}{\partial D}\right)_T$$
-    fn Z(&mut self, T: f64, D: f64) -> f64 {
-        self.aT0D1(T, D) / self.R() / T
-    }
     /// > $$B
     /// > =\frac{1}{RT}\left(\frac{\partial a^r}{\partial D}\right)_T$$
     fn B(&mut self, T: f64, _D: f64) -> f64 {
         let D = 1E-16;
         self.ar.rT0D1(T, D) / D / self.R / T
     }
     /// > $$C
@@ -354,28 +396,31 @@
 /// Settings for fundumental helmholtz equation of state.
 #[allow(non_snake_case)]
 impl<I: CalcAi, R: CalcAr> Setting for GenericA<I, R> {
     fn set_mass_unit(&mut self) {
         if self.R < 10.0 {
             self.R /= self.M;
         }
+        self.ai.set_R(self.R);
+        self.ar.set_RM(self.R, self.M);
     }
     fn set_molar_unit(&mut self) {
         if self.R > 10.0 {
             self.R *= self.M;
         }
+        self.ai.set_R(self.R);
+        self.ar.set_RM(self.R, self.M);
     }
 }
 /// Flash calculation of fundumental helmholtz equation of state.
 #[allow(non_snake_case)]
 impl<I: CalcAi, R: CalcAr> Flash for GenericA<I, R> {
     /// Temperature and Density UNCHECKED
-    fn td_unchecked(&mut self, T: f64, D: f64) -> anyhow::Result<()> {
+    fn td_unchecked(&mut self, T: f64, D: f64) {
         self.phase = Phase::One { T, D };
-        Ok(())
     }
     /// Critical point
     fn c_flash(&mut self) -> anyhow::Result<()> {
         Err(anyhow!(TlErr::NoImplementation))
     }
     /// Temperature of saturated state
     fn t_flash(&mut self, Ts: f64) -> anyhow::Result<()> {
@@ -531,14 +576,20 @@
     }
     fn D(&self) -> anyhow::Result<f64> {
         match self.phase {
             Phase::One { D, .. } => Ok(D),
             Phase::Two { .. } => Err(anyhow!(TlErr::NotInTwoPhase)),
         }
     }
+    fn Z(&mut self) -> anyhow::Result<f64> {
+        match self.phase {
+            Phase::One { T, D } => Ok(self.Z(T, D)),
+            Phase::Two { .. } => Err(anyhow!(TlErr::NotInTwoPhase)),
+        }
+    }
     fn p(&mut self) -> anyhow::Result<f64> {
         match self.phase {
             Phase::One { T, D } => Ok(self.p(T, D)),
             Phase::Two { .. } => Err(anyhow!(TlErr::NotInTwoPhase)),
         }
     }
     fn Dp_DT_D(&mut self) -> anyhow::Result<f64> {
@@ -663,20 +714,14 @@
     }
     fn g_res(&mut self) -> anyhow::Result<f64> {
         match self.phase {
             Phase::One { T, D } => Ok(self.g_res(T, D)),
             Phase::Two { .. } => Err(anyhow!(TlErr::NotInTwoPhase)),
         }
     }
-    fn Z(&mut self) -> anyhow::Result<f64> {
-        match self.phase {
-            Phase::One { T, D } => Ok(self.Z(T, D)),
-            Phase::Two { .. } => Err(anyhow!(TlErr::NotInTwoPhase)),
-        }
-    }
     fn B(&mut self) -> anyhow::Result<f64> {
         match self.phase {
             Phase::One { T, D } => Ok(self.B(T, D)),
             Phase::Two { .. } => Err(anyhow!(TlErr::NotInTwoPhase)),
         }
     }
     fn C(&mut self) -> anyhow::Result<f64> {
```

### Comparing `thermolib-0.3.1/src/core/tlerr.rs` & `thermolib-0.3.2/src/core/tlerr.rs`

 * *Files identical despite different names*

### Comparing `thermolib-0.3.1/src/helmholtz/alpha.rs` & `thermolib-0.3.2/src/helmholtz/alpha.rs`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
             || D >= 1.05 * self.ref_ar().rhols(T)
         {
             self.set_phase(Phase::One { T, D });
             Ok(()) // one phase
         } else if let Err(why) = self.t_flash(T) {
             Err(why) // Self::t_flash diverge
         } else {
-            match *self.ref_phase() {
+            match self.phase() {
                 Phase::Two { Dg, Dl, .. } => {
                     if D < Dg || D > Dl {
                         self.set_phase(Phase::One { T, D });
                         Ok(()) // one phase
                     } else {
                         self.set_phase(Phase::Two {
                             Ts: T,
```

### Comparing `thermolib-0.3.1/src/helmholtz/alpha_i.rs` & `thermolib-0.3.2/src/helmholtz/alpha_i.rs`

 * *Files 1% similar despite different names*

```diff
@@ -137,8 +137,12 @@
             + self
                 .pe_terms
                 .iter()
                 .map(|term| term.calc_2(T, self.Tc))
                 .sum::<f64>();
         self.R * T * tau2_alpha0_dtau2
     }
+    /// Used for trait::Setting
+    fn set_R(&mut self, R: f64) {
+        self.R = R;
+    }
 }
```

### Comparing `thermolib-0.3.1/src/helmholtz/alpha_r.rs` & `thermolib-0.3.2/src/helmholtz/alpha_r.rs`

 * *Files 1% similar despite different names*

```diff
@@ -226,8 +226,18 @@
     /// > $$T^2\left(\frac{\partial^2a^r}{\partial T^2}\right)_D$$  
     fn rT2D0(&self, T: f64, D: f64) -> f64 {
         (self.R * T)
             * self
                 .alphar
                 .calc_dtau_ddelta((2, 0), self.Tc / T, D / self.Dc)
     }
+    /// Used for trait::Setting
+    fn set_RM(&mut self, R: f64, M: f64) {
+        self.R = R;
+        if self.R < 10.0 && R > 10.0 {
+            self.Dc /= M;
+        }
+        if self.R > 10.0 && R < 10.0 {
+            self.Dc *= M;
+        }
+    }
 }
```

### Comparing `thermolib-0.3.1/src/helmholtz/anc_equ.rs` & `thermolib-0.3.2/src/helmholtz/anc_equ.rs`

 * *Files identical despite different names*

### Comparing `thermolib-0.3.1/src/pc_saft/alpha.rs` & `thermolib-0.3.2/src/pc_saft/alpha.rs`

 * *Files 6% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 use crate::core::{GenericA, IdealCv};
 /// PC-SAFT equation of state
 pub type Alpha = GenericA<IdealCv, AlphaR>;
 /// Methods of PC-SAFT equation of state
 #[allow(non_snake_case)]
 impl Alpha {
     pub fn new_pc_saft(m: f64, sigma: f64, epsilon: f64, M: f64) -> Self {
-        Self::new(IdealCv {}, AlphaR::new(m, sigma, epsilon, M), M)
+        Self::new(IdealCv::default(), AlphaR::new(m, sigma, epsilon, M), M)
     }
 }
 /// unit test
 #[cfg(test)]
 mod tests {
     use super::*;
     use crate::{Flash, Prop};
     #[test]
     #[allow(non_snake_case)]
     fn test_pc_saft_alpha() {
         let mut pc_saft = Alpha::new(
-            IdealCv {},
+            IdealCv::default(),
             AlphaR::new(1.6069, 3.5206, 191.42, 30.07),
             30.07,
         ); // parameters for ethane
         let T = 300.0; // K
         let D = 1000.0; // mol/m3
         if let Err(_) = pc_saft.td_flash(T, D) {
             panic!("td_flash failed at T = {} K and D = {} mol/m3", T, D);
```

### Comparing `thermolib-0.3.1/src/pc_saft/alpha_r.rs` & `thermolib-0.3.2/src/pc_saft/alpha_r.rs`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,18 @@
         let D = self.change_density(D);
         (self.R * T)
             * (2.0 * self.disp.calc_rT1D0(T, D)
                 + self.disp.calc_rT2D0(T, D)
                 + 2.0 * self.hc.calc_rT1D0(T, D)
                 + self.hc.calc_rT2D0(T, D))
     }
+    /// Used for trait::Setting
+    fn set_RM(&mut self, R: f64, _M: f64) {
+        self.R = R;
+    }
 }
 /// unit test
 #[cfg(test)]
 mod tests {
     use super::*;
     #[test]
     #[allow(non_snake_case)]
```

### Comparing `thermolib-0.3.1/src/pc_saft/disp.rs` & `thermolib-0.3.2/src/pc_saft/disp.rs`

 * *Files identical despite different names*

### Comparing `thermolib-0.3.1/src/pc_saft/hc.rs` & `thermolib-0.3.2/src/pc_saft/hc.rs`

 * *Files identical despite different names*

### Comparing `thermolib-0.3.1/src/pr/density_pr.rs` & `thermolib-0.3.2/src/pr/density.rs`

 * *Files identical despite different names*

### Comparing `thermolib-0.3.1/tests/find_json.rs` & `thermolib-0.3.2/tests/find_json.rs`

 * *Files identical despite different names*

### Comparing `thermolib-0.3.1/tests/internals/mod.rs` & `thermolib-0.3.2/tests/internals/mod.rs`

 * *Files identical despite different names*

### Comparing `thermolib-0.3.1/tests/main.py` & `thermolib-0.3.2/tests/main.py`

 * *Files identical despite different names*

### Comparing `thermolib-0.3.1/tests/pcsaft.cpp` & `thermolib-0.3.2/tests/pcsaft.cpp`

 * *Files identical despite different names*

### Comparing `thermolib-0.3.1/tests/pcsaft.h` & `thermolib-0.3.2/tests/pcsaft.h`

 * *Files identical despite different names*

### Comparing `thermolib-0.3.1/tests/test_fluid.rs` & `thermolib-0.3.2/tests/test_fluid.rs`

 * *Files identical despite different names*

