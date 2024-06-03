# Comparing `tmp/polars_cli-0.7.0.tar.gz` & `tmp/polars_cli-0.8.0.tar.gz`

## Comparing `polars_cli-0.7.0.tar` & `polars_cli-0.8.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 polars_cli-0.7.0/Cargo.toml
--rw-r--r--   0     1001      127       43 2024-03-07 10:02:00.000000 polars_cli-0.7.0/.github/CODEOWNERS
--rw-r--r--   0     1001      127     3368 2024-03-07 10:02:00.000000 polars_cli-0.7.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0     1001      127       18 2024-03-07 10:02:00.000000 polars_cli-0.7.0/.github/FUNDING.yml
--rw-r--r--   0     1001      127     1473 2024-03-07 10:02:00.000000 polars_cli-0.7.0/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0     1001      127      525 2024-03-07 10:02:00.000000 polars_cli-0.7.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0     1001      127      380 2024-03-07 10:02:00.000000 polars_cli-0.7.0/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0     1001      127      297 2024-03-07 10:02:00.000000 polars_cli-0.7.0/.github/dependabot.yml
--rw-r--r--   0     1001      127     1369 2024-03-07 10:02:00.000000 polars_cli-0.7.0/.github/release-drafter.yml
--rw-r--r--   0     1001      127     1979 2024-03-07 10:02:00.000000 polars_cli-0.7.0/.github/workflows/bump-versions.yml
--rw-r--r--   0     1001      127     1107 2024-03-07 10:02:00.000000 polars_cli-0.7.0/.github/workflows/lint.yml
--rw-r--r--   0     1001      127      384 2024-03-07 10:02:00.000000 polars_cli-0.7.0/.github/workflows/pr-labeler.yml
--rw-r--r--   0     1001      127      674 2024-03-07 10:02:00.000000 polars_cli-0.7.0/.github/workflows/release-drafter.yml
--rw-r--r--   0     1001      127     8053 2024-03-07 10:02:00.000000 polars_cli-0.7.0/.github/workflows/release.yml
--rw-r--r--   0     1001      127     2982 2024-03-07 10:02:00.000000 polars_cli-0.7.0/.gitignore
--rw-r--r--   0     1001      127    63874 2024-03-07 10:02:00.000000 polars_cli-0.7.0/Cargo.lock
--rw-r--r--   0     1001      127     1056 2024-03-07 10:02:00.000000 polars_cli-0.7.0/LICENSE
--rw-r--r--   0     1001      127     3368 2024-03-07 10:02:00.000000 polars_cli-0.7.0/README.md
--rw-r--r--   0     1001      127      205 2024-03-07 10:02:00.000000 polars_cli-0.7.0/dprint.json
--rw-r--r--   0     1001      127      457 2024-03-07 10:02:00.000000 polars_cli-0.7.0/examples/datasets/foods.csv
--rw-r--r--   0     1001      127        0 2024-03-07 10:02:00.000000 polars_cli-0.7.0/python/polars-cli/__init__.py
--rw-r--r--   0     1001      127     1050 2024-03-07 10:02:00.000000 polars_cli-0.7.0/python/polars-cli/__main__.py
--rw-r--r--   0     1001      127       43 2024-03-07 10:02:00.000000 polars_cli-0.7.0/rust-toolchain.toml
--rw-r--r--   0     1001      127      100 2024-03-07 10:02:00.000000 polars_cli-0.7.0/rustfmt.toml
--rw-r--r--   0     1001      127     4583 2024-03-07 10:02:00.000000 polars_cli-0.7.0/src/highlighter.rs
--rw-r--r--   0     1001      127     6646 2024-03-07 10:02:00.000000 polars_cli-0.7.0/src/interactive.rs
--rw-r--r--   0     1001      127     5414 2024-03-07 10:02:00.000000 polars_cli-0.7.0/src/main.rs
--rw-r--r--   0     1001      127     1044 2024-03-07 10:02:00.000000 polars_cli-0.7.0/src/prompt.rs
--rw-r--r--   0     1001      127     1302 2024-03-07 10:02:00.000000 polars_cli-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     4628 1970-01-01 00:00:00.000000 polars_cli-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 polars_cli-0.8.0/Cargo.toml
+-rw-r--r--   0     1001      127       43 2024-06-03 07:17:36.000000 polars_cli-0.8.0/.github/CODEOWNERS
+-rw-r--r--   0     1001      127     3368 2024-06-03 07:17:36.000000 polars_cli-0.8.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0     1001      127       18 2024-06-03 07:17:36.000000 polars_cli-0.8.0/.github/FUNDING.yml
+-rw-r--r--   0     1001      127     1473 2024-06-03 07:17:36.000000 polars_cli-0.8.0/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0     1001      127      525 2024-06-03 07:17:36.000000 polars_cli-0.8.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0     1001      127      380 2024-06-03 07:17:36.000000 polars_cli-0.8.0/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0     1001      127      297 2024-06-03 07:17:36.000000 polars_cli-0.8.0/.github/dependabot.yml
+-rw-r--r--   0     1001      127     1369 2024-06-03 07:17:36.000000 polars_cli-0.8.0/.github/release-drafter.yml
+-rw-r--r--   0     1001      127     1979 2024-06-03 07:17:36.000000 polars_cli-0.8.0/.github/workflows/bump-versions.yml
+-rw-r--r--   0     1001      127     1107 2024-06-03 07:17:36.000000 polars_cli-0.8.0/.github/workflows/lint.yml
+-rw-r--r--   0     1001      127      384 2024-06-03 07:17:36.000000 polars_cli-0.8.0/.github/workflows/pr-labeler.yml
+-rw-r--r--   0     1001      127      674 2024-06-03 07:17:36.000000 polars_cli-0.8.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0     1001      127     8112 2024-06-03 07:17:36.000000 polars_cli-0.8.0/.github/workflows/release.yml
+-rw-r--r--   0     1001      127     2982 2024-06-03 07:17:36.000000 polars_cli-0.8.0/.gitignore
+-rw-r--r--   0     1001      127    65640 2024-06-03 07:17:36.000000 polars_cli-0.8.0/Cargo.lock
+-rw-r--r--   0     1001      127     1056 2024-06-03 07:17:36.000000 polars_cli-0.8.0/LICENSE
+-rw-r--r--   0     1001      127     3368 2024-06-03 07:17:36.000000 polars_cli-0.8.0/README.md
+-rw-r--r--   0     1001      127      205 2024-06-03 07:17:36.000000 polars_cli-0.8.0/dprint.json
+-rw-r--r--   0     1001      127      457 2024-06-03 07:17:36.000000 polars_cli-0.8.0/examples/datasets/foods.csv
+-rw-r--r--   0     1001      127        0 2024-06-03 07:17:36.000000 polars_cli-0.8.0/python/polars-cli/__init__.py
+-rw-r--r--   0     1001      127     1050 2024-06-03 07:17:36.000000 polars_cli-0.8.0/python/polars-cli/__main__.py
+-rw-r--r--   0     1001      127       43 2024-06-03 07:17:36.000000 polars_cli-0.8.0/rust-toolchain.toml
+-rw-r--r--   0     1001      127      100 2024-06-03 07:17:36.000000 polars_cli-0.8.0/rustfmt.toml
+-rw-r--r--   0     1001      127     4583 2024-06-03 07:17:36.000000 polars_cli-0.8.0/src/highlighter.rs
+-rw-r--r--   0     1001      127     6646 2024-06-03 07:17:36.000000 polars_cli-0.8.0/src/interactive.rs
+-rw-r--r--   0     1001      127     5521 2024-06-03 07:17:36.000000 polars_cli-0.8.0/src/main.rs
+-rw-r--r--   0     1001      127     1044 2024-06-03 07:17:36.000000 polars_cli-0.8.0/src/prompt.rs
+-rw-r--r--   0     1001      127     1302 2024-06-03 07:17:36.000000 polars_cli-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     4628 1970-01-01 00:00:00.000000 polars_cli-0.8.0/PKG-INFO
```

### Comparing `polars_cli-0.7.0/Cargo.toml` & `polars_cli-0.8.0/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "polars-cli"
-version = "0.7.0"
+version = "0.8.0"
 edition = "2021"
 license = "MIT"
 repository = "https://github.com/pola-rs/polars-cli"
 description = "CLI interface for running SQL queries with Polars as backend"
 
 [[bin]]
 name = "polars"
@@ -12,21 +12,21 @@
 
 [dependencies]
 atty = { version = "0.2" }
 ciborium = { version = "0.2" }
 clap = { version = "4", features = ["derive", "cargo"] }
 nu-ansi-term = { version = "0.50", optional = true }
 once_cell = { version = "1" }
-reedline = { version = "0.30" }
+reedline = { version = "0.32" }
 serde = { version = "1", features = ["derive"] }
-sqlparser = { version = "0.44" }
+sqlparser = { version = "0.47" }
 tmp_env = { version = "0.1" }
 
 [dependencies.polars]
-version = "0.38"
+version = "0.40"
 features = ["lazy", "sql", "dtype-full", "serde-lazy"]
 
 [target.'cfg(target_os = "linux")'.dependencies]
 jemallocator = { version = "0.5", features = ["disable_initial_exec_tls"] }
 
 [features]
 default = ["highlight", "parquet", "json", "ipc"]
```

### Comparing `polars_cli-0.7.0/.github/CODE_OF_CONDUCT.md` & `polars_cli-0.8.0/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `polars_cli-0.7.0/.github/ISSUE_TEMPLATE/bug_report.yml` & `polars_cli-0.8.0/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `polars_cli-0.7.0/.github/ISSUE_TEMPLATE/config.yml` & `polars_cli-0.8.0/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `polars_cli-0.7.0/.github/release-drafter.yml` & `polars_cli-0.8.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `polars_cli-0.7.0/.github/workflows/bump-versions.yml` & `polars_cli-0.8.0/.github/workflows/bump-versions.yml`

 * *Files identical despite different names*

### Comparing `polars_cli-0.7.0/.github/workflows/lint.yml` & `polars_cli-0.8.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `polars_cli-0.7.0/.github/workflows/release-drafter.yml` & `polars_cli-0.8.0/.github/workflows/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `polars_cli-0.7.0/.github/workflows/release.yml` & `polars_cli-0.8.0/.github/workflows/release.yml`

 * *Files 4% similar despite different names*

```diff
@@ -150,15 +150,16 @@
           target: ${{ steps.target.outputs.target }}
           args: >
             --release
             --out dist
           manylinux: '2_28'
 
       - name: Test wheel
-        if: matrix.arch == 'x86_64'
+        # Only test wheels that match the runner architecture for now
+        if: (matrix.arch == 'x86_64' && matrix.os != 'macos-latest') || (matrix.arch == 'aarch64' && matrix.os == 'macos-latest')
         run: |
           pip install dist/*.whl --force-reinstall
           polars --version
           python -m polars-cli --version
 
       - name: Upload wheel
         uses: actions/upload-artifact@v4
@@ -195,16 +196,15 @@
         with:
           pattern: dist-*
           path: dist
           merge-multiple: true
 
       - name: Publish to PyPI
         if: inputs.dry-run == false
-        # Pinned to commit to circumvent an issue with the v1.8.12 release
-        uses: pypa/gh-action-pypi-publish@aec4e82833d00547d2c8e4744a0d08766a02629a
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
           skip-existing: true
           verbose: true
 
   publish-to-crates-io:
     needs: [create-sdist, build-wheels]
     environment:
```

### Comparing `polars_cli-0.7.0/.gitignore` & `polars_cli-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `polars_cli-0.7.0/Cargo.lock` & `polars_cli-0.8.0/Cargo.lock`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "addr2line"
-version = "0.21.0"
+version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a30b2e23b9e17a9f90641c7ab1549cd9b44f296d3ccbf309d2863cfe398a0cb"
+checksum = "6e4503c46a5c0c7844e948c9a4d6acd9f50cccb4de1c48eb9e291ea17470c678"
 dependencies = [
  "gimli",
 ]
 
 [[package]]
 name = "adler"
 version = "1.0.2"
@@ -28,17 +28,17 @@
  "once_cell",
  "version_check",
  "zerocopy",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "1.1.2"
+version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2969dcb958b36655471fc61f7e416fa76033bdd4bfed0678d8fee1e2d07a1f0"
+checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "alloc-no-stdlib"
 version = "2.0.4"
@@ -52,17 +52,17 @@
 checksum = "94fb8275041c72129eb51b7d0322c29b8387a0386127718b096429201a5d6ece"
 dependencies = [
  "alloc-no-stdlib",
 ]
 
 [[package]]
 name = "allocator-api2"
-version = "0.2.16"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0942ffc6dcaadf03badf6e6a2d0228460359d5e34b57ccdc720b7382dfbd5ec5"
+checksum = "5c6cb57a04249c6480766f7f7cef5467412af1490f8d1e243141daddada3264f"
 
 [[package]]
 name = "android-tzdata"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
 
@@ -73,55 +73,56 @@
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "anstream"
-version = "0.6.13"
+version = "0.6.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d96bd03f33fe50a863e394ee9718a706f988b9079b20c3784fb726e7678b62fb"
+checksum = "418c75fa768af9c03be99d17643f93f79bbba589895012a80e3452a19ddda15b"
 dependencies = [
  "anstyle",
  "anstyle-parse",
  "anstyle-query",
  "anstyle-wincon",
  "colorchoice",
+ "is_terminal_polyfill",
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle"
-version = "1.0.6"
+version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8901269c6307e8d93993578286ac0edf7f195079ffff5ebdeea6a59ffb7e36bc"
+checksum = "038dfcf04a5feb68e9c60b21c9625a54c2c0616e79b72b0fd87075a056ae1d1b"
 
 [[package]]
 name = "anstyle-parse"
-version = "0.2.3"
+version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c75ac65da39e5fe5ab759307499ddad880d724eed2f6ce5b5e8a26f4f387928c"
+checksum = "c03a11a9034d92058ceb6ee011ce58af4a9bf61491aa7e1e59ecd24bd40d22d4"
 dependencies = [
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle-query"
-version = "1.0.2"
+version = "1.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e28923312444cdd728e4738b3f9c9cac739500909bb3d3c94b43551b16517648"
+checksum = "a64c907d4e79225ac72e2a354c9ce84d50ebb4586dee56c82b3ee73004f537f5"
 dependencies = [
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "anstyle-wincon"
-version = "3.0.2"
+version = "3.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1cd54b81ec8d6180e24654d0b371ad22fc3dd083b6ff8ba325b72e00c87660a7"
+checksum = "61a38449feb7068f52bb06c12759005cf459ee52bb4adc1d5a7c4322d716fb19"
 dependencies = [
  "anstyle",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "argminmax"
@@ -153,26 +154,26 @@
 name = "async-stream-impl"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "16e62a023e7c117e27523144c5d2459f4397fcc3cab0085af8e2224f643a0193"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "async-trait"
-version = "0.1.77"
+version = "0.1.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c980ee35e870bd1a4d2c8294d4c04d0499e67bca1e4b5cefcc693c2fa00caea9"
+checksum = "c6fa2087f2753a7da8cc1c0dbfcf89579dd57458e36769de5ac750b4671737ca"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "atoi"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f28d99ec8bfea296261ca1af174f24225171fea9664ba9003cbebee704810528"
@@ -195,134 +196,129 @@
  "hermit-abi 0.1.19",
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "backtrace"
-version = "0.3.69"
+version = "0.3.72"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2089b7e3f35b9dd2d0ed921ead4f6d318c27680d4a5bd167b3ee120edb105837"
+checksum = "17c6a35df3749d2e8bb1b7b21a976d82b15548788d2735b9d82f329268f71a11"
 dependencies = [
  "addr2line",
  "cc",
  "cfg-if",
  "libc",
  "miniz_oxide",
  "object",
  "rustc-demangle",
 ]
 
 [[package]]
 name = "base64"
-version = "0.21.7"
+version = "0.22.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
+checksum = "72b3254f16251a8381aa12e40e3c4d2f0199f8c6508fbecb9d91f575e0fbb8c6"
 
 [[package]]
 name = "bitflags"
-version = "1.3.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
-
-[[package]]
-name = "bitflags"
-version = "2.4.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed570934406eb16438a4e976b1b4500774099c13b8cb96eec99f620f05090ddf"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "brotli"
-version = "3.4.0"
+version = "5.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "516074a47ef4bce09577a3b379392300159ce5b1ba2e501ff1c819950066100f"
+checksum = "19483b140a7ac7174d34b5a581b406c64f84da5409d3e09cf4fff604f9270e67"
 dependencies = [
  "alloc-no-stdlib",
  "alloc-stdlib",
  "brotli-decompressor",
 ]
 
 [[package]]
 name = "brotli-decompressor"
-version = "2.5.1"
+version = "4.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4e2e4afe60d7dd600fdd3de8d0f08c2b7ec039712e3b6137ff98b7004e82de4f"
+checksum = "9a45bd2e4095a8b518033b128020dd4a55aab1c0a381ba4404a472630f4bc362"
 dependencies = [
  "alloc-no-stdlib",
  "alloc-stdlib",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.15.3"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ea184aa71bb362a1157c896979544cc23974e08fd265f29ea96b59f0b4a555b"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "bytemuck"
-version = "1.14.3"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2ef034f05691a48569bd920a96c81b9d91bbad1ab5ac7c4616c1f6ef36cb79f"
+checksum = "78834c15cb5d5efe3452d58b1e8ba890dd62d21907f867f383358198e56ebca5"
 dependencies = [
  "bytemuck_derive",
 ]
 
 [[package]]
 name = "bytemuck_derive"
-version = "1.5.0"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "965ab7eb5f8f97d2a083c799f3a1b994fc397b2fe2da5d1da1626ce15a39f2b1"
+checksum = "1ee891b04274a59bd38b412188e24b849617b2e45a0fd8d057deb63e7403761b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "bytes"
-version = "1.5.0"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2bd12c1caf447e69cd4528f47f94d203fd2582878ecb9e9465484c4148a8223"
+checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
-version = "1.0.89"
+version = "1.0.98"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0ba8f7aaa012f30d5b2861462f6708eccd49c3c39863fe083a308035f63d723"
+checksum = "41c270e7540d725e65ac7f1b212ac8ce349719624d7bcff99f8e2e488e8cf03f"
 dependencies = [
  "jobserver",
  "libc",
+ "once_cell",
 ]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.35"
+version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8eaf5903dcbc0a39312feb77df2ff4c76387d591b9fc7b04a238dcf8bb62639a"
+checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "num-traits",
  "serde",
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "chrono-tz"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d59ae0466b83e838b81a54256c39d5d7c20b9d7daa10510a242d9b75abd5936e"
@@ -368,17 +364,17 @@
 dependencies = [
  "ciborium-io",
  "half",
 ]
 
 [[package]]
 name = "clap"
-version = "4.5.2"
+version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b230ab84b0ffdf890d5a10abdbc8b83ae1c4918275daea1ab8801f71536b2651"
+checksum = "90bc066a67923782aa8515dbaea16946c5bcc5addbd668bb80af688e53e548a0"
 dependencies = [
  "clap_builder",
  "clap_derive",
 ]
 
 [[package]]
 name = "clap_builder"
@@ -390,41 +386,41 @@
  "anstyle",
  "clap_lex",
  "strsim",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "4.5.0"
+version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "307bc0538d5f0f83b8248db3087aa92fe504e4691294d0c96c0eabc33f47ba47"
+checksum = "528131438037fd55894f62d6e9f068b8f45ac57ffa77517819645d10aed04f64"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "98cc8fbded0c607b7ba9dd60cd98df59af97e84d24e49c8557331cfc26d301ce"
 
 [[package]]
 name = "colorchoice"
-version = "1.0.0"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
+checksum = "0b6a852b24ab71dffc585bcb46eaf7959d175cb865a7152e35b348d1b2960422"
 
 [[package]]
 name = "comfy-table"
-version = "7.1.0"
+version = "7.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7c64043d6c7b7a4c58e39e7efccfdea7b93d885a795d0c054a69dbbf4dd52686"
+checksum = "b34115915337defe99b2aff5c2ce6771e5fbc4079f4b506301f5cf394c8452f7"
 dependencies = [
  "crossterm",
  "strum",
  "strum_macros",
  "unicode-width",
 ]
 
@@ -432,26 +428,26 @@
 name = "core-foundation-sys"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
 
 [[package]]
 name = "crc32fast"
-version = "1.4.0"
+version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b3855a8a784b474f333699ef2bbca9db2c4a1f6d9088a90a2d25b1eb53111eaa"
+checksum = "a97769d94ddab943e4510d138150169a2758b5ef3eb191a9ee688de3e23ef7b3"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "crossbeam-channel"
-version = "0.5.12"
+version = "0.5.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ab3db02a9c5b5121e1e42fbdb1aeb65f5e02624cc58c43f2884c6ccac0b82f95"
+checksum = "33480d6946193aa8033910124896ca395333cae7e2d1113d1fef6c3272217df2"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-deque"
 version = "0.8.5"
@@ -478,25 +474,25 @@
 checksum = "df0346b5d5e76ac2fe4e327c5fd1118d6be7c51dfb18f9b7922923f287471e35"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.19"
+version = "0.8.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
+checksum = "22ec99545bb0ed0ea7bb9b8e1e9122ea386ff8a48c0922e43f36d45ab09e0e80"
 
 [[package]]
 name = "crossterm"
 version = "0.27.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f476fe445d41c9e991fd07515a6f463074b782242ccf4a5b7b1d1012e70824df"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags",
  "crossterm_winapi",
  "libc",
  "mio",
  "parking_lot",
  "serde",
  "signal-hook",
  "signal-hook-mio",
@@ -522,41 +518,44 @@
 name = "dyn-clone"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0d6ef0072f8a535281e4876be788938b528e9a1d43900b82c2569af7da799125"
 
 [[package]]
 name = "either"
-version = "1.10.0"
+version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
+checksum = "3dca9240753cf90908d7e4aac30f630662b02aebaa1b58a3cadabdb23385b58b"
+dependencies = [
+ "serde",
+]
 
 [[package]]
 name = "enum_dispatch"
-version = "0.3.12"
+version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f33313078bb8d4d05a2733a94ac4c2d8a0df9a2b84424ebf4f33bfc224a890e"
+checksum = "aa18ce2bc66555b3218614519ac839ddb759a7d6720732f979ef8d13be147ecd"
 dependencies = [
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
 name = "errno"
-version = "0.3.8"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
+checksum = "534c5cf6194dfab3db3242765c03bbe257cf92f22b38f6bc0c58d59108a820ba"
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "ethnum"
@@ -574,28 +573,28 @@
 name = "fast-float"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95765f67b4b18863968b4a1bd5bb576f732b29a4a28c7cd84c09fa3e2875f33c"
 
 [[package]]
 name = "fd-lock"
-version = "3.0.13"
+version = "4.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ef033ed5e9bad94e55838ca0ca906db0e043f517adda0c8b79c7a8c66c93c1b5"
+checksum = "7e5768da2206272c81ef0b5e951a41862938a6070da63bcea197899942d3b947"
 dependencies = [
  "cfg-if",
  "rustix",
- "windows-sys 0.48.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "flate2"
-version = "1.0.28"
+version = "1.0.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46303f565772937ffe1d394a4fac6f411c6013172fadde9dcdb1e147a086940e"
+checksum = "5f54427cfd1c7829e2a139fcefea601bf088ebca651d2bf53ebc600eac295dae"
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "float-cmp"
@@ -664,15 +663,15 @@
 name = "futures-macro"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
@@ -699,42 +698,42 @@
  "pin-project-lite",
  "pin-utils",
  "slab",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.12"
+version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+checksum = "c4567c8db10ae91089c99af84c68c38da3ec2f087c3f82960bcdbf3656b6f4d7"
 dependencies = [
  "cfg-if",
  "js-sys",
  "libc",
  "wasi",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "gimli"
-version = "0.28.1"
+version = "0.29.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
+checksum = "40ecd4077b5ae9fd2e9e169b102c6c330d0605168eb0e8bf79952b256dbefffd"
 
 [[package]]
 name = "glob"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
 name = "half"
-version = "2.4.0"
+version = "2.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5eceaaeec696539ddaf7b333340f1af35a5aa87ae3e4f3ead0532f72affab2e"
+checksum = "6dd08c532ae367adf81c312a4580bc67f1d0fe8bc9c460520283f4c0ff277888"
 dependencies = [
  "cfg-if",
  "crunchy",
 ]
 
 [[package]]
 name = "halfbrown"
@@ -744,28 +743,29 @@
 dependencies = [
  "hashbrown",
  "serde",
 ]
 
 [[package]]
 name = "hashbrown"
-version = "0.14.3"
+version = "0.14.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
+checksum = "e5274423e17b7c9fc20b6e7e208532f9b19825d82dfd615708b70edd83df41f1"
 dependencies = [
  "ahash",
  "allocator-api2",
  "rayon",
+ "serde",
 ]
 
 [[package]]
 name = "heck"
-version = "0.4.1"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
+checksum = "2304e00983f87ffb38b55b444b5e3b60a884b5d30c0fca7d82fe33449bbe55ea"
 
 [[package]]
 name = "hermit-abi"
 version = "0.1.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
 dependencies = [
@@ -814,37 +814,43 @@
 checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "indexmap"
-version = "2.2.5"
+version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b0b929d511467233429c45a44ac1dcaa21ba0f5ba11e4879e6ed28ddb4f9df4"
+checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
  "hashbrown",
  "serde",
 ]
 
 [[package]]
+name = "is_terminal_polyfill"
+version = "1.70.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f8478577c03552c21db0e2724ffb8986a5ce7af88107e6be5d2ee6e158c12800"
+
+[[package]]
 name = "itertools"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "itoap"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9028f49264629065d057f340a86acb84867925865f73bbf8d47b4d149a7e88b8"
 
@@ -866,17 +872,17 @@
 dependencies = [
  "jemalloc-sys",
  "libc",
 ]
 
 [[package]]
 name = "jobserver"
-version = "0.1.28"
+version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ab46a6e9526ddef3ae7f787c06f0f2600639ba80ea3eade3d8e670a2230f51d6"
+checksum = "d2b099aaa34a9751c5bf0878add70444e1ed2dd73f347be99003d4577277de6e"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "js-sys"
 version = "0.3.69"
@@ -959,35 +965,35 @@
 dependencies = [
  "lexical-util",
  "static_assertions",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.155"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "97b3888a4aecf77e811145cadf6eef5901f4782c53886191b2f693f24761847c"
 
 [[package]]
 name = "libm"
 version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.4.13"
+version = "0.4.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
+checksum = "78b3ae25bc7c8c38cec158d1f2757ee79e9b3740fbc7ccf0e59e4b08d793fa89"
 
 [[package]]
 name = "lock_api"
-version = "0.4.11"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
@@ -1013,32 +1019,32 @@
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
 name = "memchr"
-version = "2.7.1"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memmap2"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f49388d20533534cd19360ad3d6a7dadc885944aa802ba3995040c5ec11288c6"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "miniz_oxide"
-version = "0.7.2"
+version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
+checksum = "87dfd01fe195c66b572b37921ad8803d010623c0aca821bea2302239d155cdae"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mio"
 version = "0.8.11"
@@ -1049,27 +1055,27 @@
  "log",
  "wasi",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "multiversion"
-version = "0.7.3"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2c7b9d7fe61760ce5ea19532ead98541f6b4c495d87247aff9826445cf6872a"
+checksum = "c4851161a11d3ad0bf9402d90ffc3967bf231768bfd7aeb61755ad06dbf1a142"
 dependencies = [
  "multiversion-macros",
  "target-features",
 ]
 
 [[package]]
 name = "multiversion-macros"
-version = "0.7.3"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26a83d8500ed06d68877e9de1dde76c1dbb83885dcdbda4ef44ccbc3fbda2ac8"
+checksum = "79a74ddee9e0c27d2578323c13905793e91622148f138ba29738f9dddb835e90"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
  "target-features",
 ]
 
@@ -1098,17 +1104,17 @@
 checksum = "dd2800e1520bdc966782168a627aa5d1ad92e33b984bf7c7615d31280c83ff14"
 dependencies = [
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.18"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
+checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
 name = "num_cpus"
@@ -1118,65 +1124,65 @@
 dependencies = [
  "hermit-abi 0.3.9",
  "libc",
 ]
 
 [[package]]
 name = "object"
-version = "0.32.2"
+version = "0.35.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a6a622008b6e321afc04970976f62ee297fdbaa6f95318ca343e3eebb9648441"
+checksum = "b8ec7ab813848ba4522158d5517a6093db1ded27575b070f4177b8d12b41db5e"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "f1bf18183cf54e8d6059647fc3063646a1801cf30896933ec2311622cc4b9a27"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.9"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-targets 0.48.5",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "parquet-format-safe"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1131c54b167dd4e4799ce762e1ab01549ebb94d5bdd13e6ec1b467491c378e1f"
 dependencies = [
  "async-trait",
  "futures",
 ]
 
 [[package]]
 name = "parse-zoneinfo"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c705f256449c60da65e11ff6626e0c16a0a0b96aaa348de61376b249bc340f41"
+checksum = "1f2a05b18d44e2957b88f96ba460715e295bc1d7510468a2f3d3b44535d26c24"
 dependencies = [
  "regex",
 ]
 
 [[package]]
 name = "percent-encoding"
 version = "2.3.1"
@@ -1219,17 +1225,17 @@
 checksum = "90fcb95eef784c2ac79119d1dd819e162b5da872ce6f3c3abe1e8ca1c082f72b"
 dependencies = [
  "siphasher",
 ]
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.13"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
+checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
@@ -1246,17 +1252,17 @@
 checksum = "fc1691dd09e82f428ce8d6310bd6d5da2557c82ff17694d2a32cad7242aea89f"
 dependencies = [
  "array-init-cursor",
 ]
 
 [[package]]
 name = "polars"
-version = "0.38.1"
+version = "0.40.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3a26ef94cfedd5915da990a0b4740cca17b5854bd44a8e8c741fe732c02aac37"
+checksum = "e148396dca5496566880fa19374f3f789a29db94e3eb458afac1497b4bac5442"
 dependencies = [
  "getrandom",
  "polars-arrow",
  "polars-core",
  "polars-error",
  "polars-io",
  "polars-lazy",
@@ -1266,17 +1272,17 @@
  "polars-time",
  "polars-utils",
  "version_check",
 ]
 
 [[package]]
 name = "polars-arrow"
-version = "0.38.1"
+version = "0.40.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "48e71d30a9fa503bc3baaff3b4c48f08d402c442a50ea7fb9d475ce7b575425a"
+checksum = "1cb5e11cd0752ae022fa6ca3afa50a14b0301b7ce53c0135828fbb0f4fa8303e"
 dependencies = [
  "ahash",
  "atoi",
  "atoi_simd",
  "bytemuck",
  "chrono",
  "chrono-tz",
@@ -1313,53 +1319,53 @@
 dependencies = [
  "planus",
  "serde",
 ]
 
 [[package]]
 name = "polars-cli"
-version = "0.7.0"
+version = "0.8.0"
 dependencies = [
  "atty",
  "ciborium",
  "clap",
  "jemallocator",
  "nu-ansi-term",
  "once_cell",
  "polars",
  "reedline",
  "serde",
- "sqlparser 0.44.0",
+ "sqlparser 0.47.0",
  "tmp_env",
 ]
 
 [[package]]
 name = "polars-compute"
-version = "0.38.1"
+version = "0.40.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26342dea46502e8a3322f484062869c2fa49185d512bce4fb44f350b559b4eae"
+checksum = "89fc4578f826234cdecb782952aa9c479dc49373f81694a7b439c70b6f609ba0"
 dependencies = [
  "bytemuck",
  "either",
  "num-traits",
  "polars-arrow",
  "polars-error",
  "polars-utils",
  "strength_reduce",
  "version_check",
 ]
 
 [[package]]
 name = "polars-core"
-version = "0.38.1"
+version = "0.40.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99e0885a8f1bd1f4d928f5eaa852825bf647b6b5e21e171b6af838f77b6565f3"
+checksum = "e490c6bace1366a558feea33d1846f749a8ca90bd72a6748752bc65bb4710b2a"
 dependencies = [
  "ahash",
- "bitflags 2.4.2",
+ "bitflags",
  "bytemuck",
  "chrono",
  "chrono-tz",
  "comfy-table",
  "either",
  "hashbrown",
  "indexmap",
@@ -1379,29 +1385,49 @@
  "thiserror",
  "version_check",
  "xxhash-rust",
 ]
 
 [[package]]
 name = "polars-error"
-version = "0.38.1"
+version = "0.40.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d259d905c17d8e8b2de1eadc94dc4186bf1d325f1be81b4087afea22a6f753d6"
+checksum = "08888f58e61599b00f5ea0c2ccdc796b54b9859559cc0d4582733509451fa01a"
 dependencies = [
  "polars-arrow-format",
  "regex",
  "simdutf8",
  "thiserror",
 ]
 
 [[package]]
+name = "polars-expr"
+version = "0.40.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4173591920fe56ad55af025f92eb0d08421ca85705c326a640c43856094e3484"
+dependencies = [
+ "ahash",
+ "bitflags",
+ "once_cell",
+ "polars-arrow",
+ "polars-core",
+ "polars-io",
+ "polars-ops",
+ "polars-plan",
+ "polars-time",
+ "polars-utils",
+ "rayon",
+ "smartstring",
+]
+
+[[package]]
 name = "polars-io"
-version = "0.38.1"
+version = "0.40.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "45f694b918ba2ee7e6f13e8415598f94009c390a9e61c95e6b9c26c8fe1a1a54"
+checksum = "5842896aea46d975b425d63f156f412aed3cfde4c257b64fb1f43ceea288074e"
 dependencies = [
  "ahash",
  "async-trait",
  "atoi_simd",
  "bytes",
  "chrono",
  "fast-float",
@@ -1430,17 +1456,17 @@
  "smartstring",
  "tokio",
  "tokio-util",
 ]
 
 [[package]]
 name = "polars-json"
-version = "0.38.1"
+version = "0.40.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd7c4d33540a22cd49ccb9b4da77999604ba986707d4568be57fde2f719954ae"
+checksum = "160cbad0145b93ac6a88639aadfa6f7d7c769d05a8674f9b7e895b398cae9901"
 dependencies = [
  "ahash",
  "chrono",
  "fallible-streaming-iterator",
  "hashbrown",
  "indexmap",
  "itoa",
@@ -1451,41 +1477,42 @@
  "ryu",
  "simd-json",
  "streaming-iterator",
 ]
 
 [[package]]
 name = "polars-lazy"
-version = "0.38.1"
+version = "0.40.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "56e3b40272d24142bcecb2979b19ec8d8c1a14036cb3cea09ce8fb8a4a43bcde"
+checksum = "e805ea2ebbc6b7749b0afb31b7fc5d32b42b57ba29b984549d43d3a16114c4a5"
 dependencies = [
  "ahash",
- "bitflags 2.4.2",
+ "bitflags",
  "glob",
  "once_cell",
  "polars-arrow",
  "polars-core",
+ "polars-expr",
  "polars-io",
  "polars-json",
  "polars-ops",
  "polars-pipe",
  "polars-plan",
  "polars-time",
  "polars-utils",
  "rayon",
  "smartstring",
  "version_check",
 ]
 
 [[package]]
 name = "polars-ops"
-version = "0.38.1"
+version = "0.40.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cd5bad61c2fa1977eb65bb719f12d4f68b908edf1106b91b3ab9615f9df8843e"
+checksum = "7b0aed7e169c81b98457641cf82b251f52239a668916c2e683abd1f38df00d58"
 dependencies = [
  "ahash",
  "argminmax",
  "base64",
  "bytemuck",
  "chrono",
  "chrono-tz",
@@ -1509,17 +1536,17 @@
  "smartstring",
  "unicode-reverse",
  "version_check",
 ]
 
 [[package]]
 name = "polars-parquet"
-version = "0.38.1"
+version = "0.40.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "06d84fb9b005a19ca523406df371d9329466ae87df48922d0d3d8955072502a4"
+checksum = "c70670a9e51cac66d0e77fd20b5cc957dbcf9f2660d410633862bb72f846d5b8"
 dependencies = [
  "ahash",
  "async-stream",
  "base64",
  "brotli",
  "ethnum",
  "flate2",
@@ -1535,101 +1562,107 @@
  "snap",
  "streaming-decompression",
  "zstd",
 ]
 
 [[package]]
 name = "polars-pipe"
-version = "0.38.1"
+version = "0.40.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "58097bef7208a5b833c4d832d948026854917b4a219d55ab1779eb36b59fac0f"
+checksum = "0a40ae1b3c74ee07e2d1f7cbf56c5d6e15969e45d9b6f0903bd2acaf783ba436"
 dependencies = [
  "crossbeam-channel",
  "crossbeam-queue",
  "enum_dispatch",
  "hashbrown",
  "num-traits",
  "polars-arrow",
  "polars-compute",
  "polars-core",
+ "polars-expr",
  "polars-io",
  "polars-ops",
  "polars-plan",
  "polars-row",
  "polars-utils",
  "rayon",
  "smartstring",
  "uuid",
  "version_check",
 ]
 
 [[package]]
 name = "polars-plan"
-version = "0.38.1"
+version = "0.40.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "56493c0e13aaccfcae59985db34da30cd4893e57edc9715d8688c96d7e911d47"
+checksum = "8daa3541ae7e9af311a4389bc2b21f83349c34c723cc67fa524cdefdaa172d90"
 dependencies = [
  "ahash",
  "bytemuck",
  "chrono-tz",
+ "either",
+ "hashbrown",
  "once_cell",
  "percent-encoding",
  "polars-arrow",
  "polars-core",
  "polars-io",
  "polars-json",
  "polars-ops",
  "polars-parquet",
  "polars-time",
  "polars-utils",
  "rayon",
+ "recursive",
  "regex",
  "serde",
  "smartstring",
  "strum_macros",
  "version_check",
 ]
 
 [[package]]
 name = "polars-row"
-version = "0.38.1"
+version = "0.40.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7def6f9fc14fbfc0550bad615a757f3e1d86c00983c5ff23166fcdf205438d51"
+checksum = "deb285f2f3a65b00dd06bef16bb9f712dbb5478f941dab5cf74f9f016d382e40"
 dependencies = [
  "bytemuck",
  "polars-arrow",
  "polars-error",
  "polars-utils",
 ]
 
 [[package]]
 name = "polars-sql"
-version = "0.38.1"
+version = "0.40.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f9d7de9dca8170a20b6c4cb7bafaf724abe88e807646bc3c2e98f13a34a7c4c"
+checksum = "a724f699d194cb02c25124d3832f7d4d77f387f1a89ee42f6b9e88ec561d4ad9"
 dependencies = [
  "hex",
+ "once_cell",
  "polars-arrow",
  "polars-core",
  "polars-error",
  "polars-lazy",
  "polars-plan",
  "rand",
  "serde",
  "serde_json",
  "sqlparser 0.39.0",
 ]
 
 [[package]]
 name = "polars-time"
-version = "0.38.1"
+version = "0.40.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "162c815c3cb0f859da40f056c8a0a9c4247900e1275702ae399192ea60acac2a"
+checksum = "87ebec238d8b6200d9f0c3ce411c8441e950bd5a7df7806b8172d06c1d5a4b97"
 dependencies = [
  "atoi",
+ "bytemuck",
  "chrono",
  "chrono-tz",
  "now",
  "once_cell",
  "polars-arrow",
  "polars-core",
  "polars-error",
@@ -1638,52 +1671,62 @@
  "regex",
  "serde",
  "smartstring",
 ]
 
 [[package]]
 name = "polars-utils"
-version = "0.38.1"
+version = "0.40.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7fca7938ee789314ac92a0bf6c1c4e5eaeb5e428241df2519fd70f21dba49194"
+checksum = "34e1a907c63abf71e5f21467e2e4ff748896c28196746f631c6c25512ec6102c"
 dependencies = [
  "ahash",
  "bytemuck",
  "hashbrown",
  "indexmap",
  "num-traits",
  "once_cell",
  "polars-error",
  "raw-cpuid",
  "rayon",
  "smartstring",
+ "stacker",
  "sysinfo",
  "version_check",
 ]
 
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.78"
+version = "1.0.85"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
+checksum = "22244ce15aa966053a896d1accb3a6e68469b97c7f33f284b99f0d576879fc23"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
+name = "psm"
+version = "0.1.21"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5787f7cda34e3033a72192c018bc5883100330f362ef279a8cbccfce8bb4e874"
+dependencies = [
+ "cc",
+]
+
+[[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -1722,26 +1765,26 @@
 dependencies = [
  "num-traits",
  "rand",
 ]
 
 [[package]]
 name = "raw-cpuid"
-version = "11.0.1"
+version = "11.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d86a7c4638d42c44551f4791a20e687dbb4c3de1f33c43dd71e355cd429def1"
+checksum = "e29830cbb1290e404f24c73af91c5d8d631ce7e128691e9477556b540cd01ecd"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags",
 ]
 
 [[package]]
 name = "rayon"
-version = "1.9.0"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e4963ed1bc86e4f3ee217022bd855b297cef07fb9eac5dfa1f788b220b49b3bd"
+checksum = "b418a60154510ca1a002a752ca9714984e21e4241e804d32555251faf8b78ffa"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
@@ -1750,27 +1793,47 @@
 checksum = "1465873a3dfdaa8ae7cb14b4383657caab0b3e8a0aa9ae8e04b044854c8dfce2"
 dependencies = [
  "crossbeam-deque",
  "crossbeam-utils",
 ]
 
 [[package]]
+name = "recursive"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0786a43debb760f491b1bc0269fe5e84155353c67482b9e60d0cfb596054b43e"
+dependencies = [
+ "recursive-proc-macro-impl",
+ "stacker",
+]
+
+[[package]]
+name = "recursive-proc-macro-impl"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "76009fbe0614077fc1a2ce255e3a1881a2e3a3527097d5dc6d8212c585e7e38b"
+dependencies = [
+ "quote",
+ "syn 2.0.66",
+]
+
+[[package]]
 name = "redox_syscall"
-version = "0.4.1"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags",
 ]
 
 [[package]]
 name = "reedline"
-version = "0.30.0"
+version = "0.32.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "413a9fa6a5d8c937d3ae1e975bfb6a918bb0b6cdfae6a10416218c837a31b8fc"
+checksum = "abf59e4c97b5049ba96b052cdb652368305a2eddcbce9bf1c16f9d003139eeea"
 dependencies = [
  "chrono",
  "crossterm",
  "fd-lock",
  "itertools",
  "nu-ansi-term",
  "serde",
@@ -1780,37 +1843,37 @@
  "thiserror",
  "unicode-segmentation",
  "unicode-width",
 ]
 
 [[package]]
 name = "ref-cast"
-version = "1.0.22"
+version = "1.0.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c4846d4c50d1721b1a3bef8af76924eef20d5e723647333798c1b519b3a9473f"
+checksum = "ccf0a6f84d5f1d581da8b41b47ec8600871962f2a528115b542b362d4b744931"
 dependencies = [
  "ref-cast-impl",
 ]
 
 [[package]]
 name = "ref-cast-impl"
-version = "1.0.22"
+version = "1.0.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5fddb4f8d99b0a2ebafc65a87a69a7b9875e4b1ae1f00db265d300ef7f28bccc"
+checksum = "bcc303e793d3734489387d205e9b186fac9c6cfacedd98cbb2e8a5943595f3e6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "regex"
-version = "1.10.3"
+version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b62dbe01f0b06f9d8dc7d49e05a0785f153b00b2c227856282f671e0318c9b15"
+checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-automata",
  "regex-syntax",
 ]
 
@@ -1823,48 +1886,48 @@
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "rustc-demangle"
-version = "0.1.23"
+version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
+checksum = "719b953e2095829ee67db738b3bfa9fa368c94900df327b3f07fe6e794d2fe1f"
 
 [[package]]
 name = "rustix"
-version = "0.38.31"
+version = "0.38.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ea3e1a662af26cd7a3ba09c0297a31af215563ecf42817c98df621387f4e949"
+checksum = "70dc5ec042f7a43c4a73241207cecc9873a06d45debb38b329f8541d85c2730f"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags",
  "errno",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "rustversion"
-version = "1.0.14"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ffc183a10b4478d04cbbbfc96d0873219d962dd5accaff2ffbd4ceb7df837f4"
+checksum = "955d28af4278de8121b7ebeb796b6a45735dc01436d898801014aced2773a3d6"
 
 [[package]]
 name = "ryu"
-version = "1.0.17"
+version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
+checksum = "f3cb5ba0dc43242ce17de99c180e96db90b235b8a9fdc9543c96d2209116bd9f"
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
@@ -1872,37 +1935,37 @@
 name = "seq-macro"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3f0bf26fd526d2a95683cd0f87bf103b8539e2ca1ef48ce002d67aad59aa0b4"
 
 [[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.203"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "7253ab4de971e72fb7be983802300c30b5a7f0c2e56fab8abfc6a214307c0094"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.203"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "500cbc0ebeb6f46627f50f3f5811ccf6bf00643be300b4c3eabc0ef55dc5b5ba"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.114"
+version = "1.0.117"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5f09b1bd632ef549eaa9f60a1f8de742bdbc698e6cee2095fc84dde5f549ae0"
+checksum = "455182ea6142b14f93f4bc5320a2b31c1f266b66a4a5c858b013302a5d8cbfc3"
 dependencies = [
  "indexmap",
  "itoa",
  "ryu",
  "serde",
 ]
 
@@ -1925,26 +1988,26 @@
  "libc",
  "mio",
  "signal-hook",
 ]
 
 [[package]]
 name = "signal-hook-registry"
-version = "1.4.1"
+version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
+checksum = "a9e9e0b4211b72e7b8b6e85c807d36c212bdb33ea8587f7569562a84df5465b1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "simd-json"
-version = "0.13.8"
+version = "0.13.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2faf8f101b9bc484337a6a6b0409cf76c139f2fb70a9e3aee6b6774be7bfbf76"
+checksum = "570c430b3d902ea083097e853263ae782dfe40857d93db019a12356c8e8143fa"
 dependencies = [
  "ahash",
  "getrandom",
  "halfbrown",
  "lexical-core",
  "once_cell",
  "ref-cast",
@@ -1973,17 +2036,17 @@
 checksum = "8f92a496fb766b417c996b9c5e57daf2f7ad3b0bebe1ccfca4856390e3d3bb67"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.13.1"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "smartstring"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fb72c633efbaa2dd666986505016c32c3044395ceaf881518399d2f4127ee29"
 dependencies = [
@@ -1997,17 +2060,17 @@
 name = "snap"
 version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1b6b67fb9a61334225b5b790716f609cd58395f895b3fe8b328786812a40bc3b"
 
 [[package]]
 name = "socket2"
-version = "0.5.6"
+version = "0.5.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05ffd9c0a93b7543e062e759284fcf5f5e3b098501104bfbdde4d404db792871"
+checksum = "ce305eb0b4296696835b71df73eb912e0f1ffd2556a501fcede6e0c50349191c"
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "sqlparser"
@@ -2016,22 +2079,35 @@
 checksum = "743b4dc2cbde11890ccb254a8fc9d537fa41b36da00de2a1c5e9848c9bc42bd7"
 dependencies = [
  "log",
 ]
 
 [[package]]
 name = "sqlparser"
-version = "0.44.0"
+version = "0.47.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aaf9c7ff146298ffda83a200f8d5084f08dcee1edfc135fcc1d646a45d50ffd6"
+checksum = "295e9930cd7a97e58ca2a070541a3ca502b17f5d1fa7157376d0fabd85324f25"
 dependencies = [
  "log",
 ]
 
 [[package]]
+name = "stacker"
+version = "0.1.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c886bd4480155fd3ef527d45e9ac8dd7118a898a46530b7b94c3e21866259fce"
+dependencies = [
+ "cc",
+ "cfg-if",
+ "libc",
+ "psm",
+ "winapi",
+]
+
+[[package]]
 name = "static_assertions"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
 
 [[package]]
 name = "streaming-decompression"
@@ -2061,35 +2137,35 @@
 checksum = "55ff8ef943b384c414f54aefa961dd2bd853add74ec75e7ac74cf91dba62bcfa"
 dependencies = [
  "vte",
 ]
 
 [[package]]
 name = "strsim"
-version = "0.11.0"
+version = "0.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ee073c9e4cd00e28217186dbe12796d692868f432bf2e97ee73bed0c56dfa01"
+checksum = "7da8b5736845d9f2fcb837ea5d9e2628564b3b043a70948a3f0b778838c5fb4f"
 
 [[package]]
 name = "strum"
-version = "0.25.0"
+version = "0.26.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "290d54ea6f91c969195bdbcd7442c8c2a2ba87da8bf60a7ee86a235d4bc1e125"
+checksum = "5d8cec3501a5194c432b2b7976db6b7d10ec95c253208b45f83f7136aa985e29"
 
 [[package]]
 name = "strum_macros"
-version = "0.25.3"
+version = "0.26.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23dc1fa9ac9c169a78ba62f0b841814b7abae11bdd047b9c58f893439e309ea0"
+checksum = "f7993a8e3a9e88a00351486baae9522c91b123a088f76469e5bd5cc17198ea87"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "rustversion",
- "syn 2.0.52",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
@@ -2097,93 +2173,93 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.52"
+version = "2.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b699d15b36d1f02c3e7c69f8ffef53de37aefae075d8488d4ba1a7788d574a07"
+checksum = "c42f3f41a2de00b01c0aaad383c5a45241efc8b2d1eda5661812fda5f3cdcff5"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "sysinfo"
-version = "0.30.7"
+version = "0.30.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c385888ef380a852a16209afc8cfad22795dd8873d69c9a14d2e2088f118d18"
+checksum = "732ffa00f53e6b2af46208fba5718d9662a421049204e156328b66791ffa15ae"
 dependencies = [
  "cfg-if",
  "core-foundation-sys",
  "libc",
  "ntapi",
  "once_cell",
  "windows",
 ]
 
 [[package]]
 name = "target-features"
-version = "0.1.5"
+version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cfb5fa503293557c5158bd215fdc225695e567a77e453f5d4452a50a193969bd"
+checksum = "c1bbb9f3c5c463a01705937a24fdabc5047929ac764b2d5b9cf681c1f5041ed5"
 
 [[package]]
 name = "thiserror"
-version = "1.0.57"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e45bcbe8ed29775f228095caf2cd67af7a4ccf756ebff23a306bf3e8b47b24b"
+checksum = "c546c80d6be4bc6a00c0f01730c08df82eaa7a7a61f11d656526506112cc1709"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.57"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a953cb265bef375dae3de6663da4d3804eee9682ea80d8e2542529b73c531c81"
+checksum = "46c3384250002a6d5af4d114f2845d37b57521033f30d5c3f46c4d70e1197533"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "tmp_env"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a56eb9e5a28c3c4f0a6aa8ea70a8ad2d6c53e4bf364571ce78f57945b6766843"
 dependencies = [
  "rand",
 ]
 
 [[package]]
 name = "tokio"
-version = "1.36.0"
+version = "1.38.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "61285f6515fa018fb2d1e46eb21223fff441ee8db5d0f1435e8ab4f5cdb80931"
+checksum = "ba4f4a02a7a80d6f274636f0aa95c7e383b912d41fe721a31f29e29698585a4a"
 dependencies = [
  "backtrace",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "pin-project-lite",
  "socket2",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "tokio-util"
-version = "0.7.10"
+version = "0.7.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5419f34732d9eb6ee4c3578b7989078579b7f039cbbb9ca2c4da015749371e15"
+checksum = "9cf6b47b3771c49ac75ad09a6162f53ad4b8088b76ac60e8ec1455b31a189fe1"
 dependencies = [
  "bytes",
  "futures-core",
  "futures-sink",
  "pin-project-lite",
  "tokio",
 ]
@@ -2192,44 +2268,44 @@
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unicode-reverse"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0bea5dacebb0d2d0a69a6700a05b59b3908bf801bf563a49bd27a1b60122962c"
+checksum = "4b6f4888ebc23094adfb574fdca9fdc891826287a6397d2cd28802ffd6f20c76"
 dependencies = [
  "unicode-segmentation",
 ]
 
 [[package]]
 name = "unicode-segmentation"
 version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d4c87d22b6e3f4a18d4d40ef354e97c90fcb14dd91d7dc0aa9d8a1172ebf7202"
 
 [[package]]
 name = "unicode-width"
-version = "0.1.11"
+version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e51733f11c9c4f72aa0c160008246859e340b00807569a0da0e7a1079b27ba85"
+checksum = "68f5e5f3158ecfd4b8ff6fe086db7c8467a2dfdac97fe420f2b7c4aa97af66d6"
 
 [[package]]
 name = "utf8parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
 name = "uuid"
-version = "1.7.0"
+version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f00cc9702ca12d3c81455259621e676d0f7251cec66a21e98fe2e9a37db93b2a"
+checksum = "a183cf7feeba97b4dd1c0d46788634f6221d87fa961b305bed08c851829efcc0"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "value-trait"
 version = "0.8.1"
@@ -2291,15 +2367,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.66",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2313,15 +2389,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.66",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
@@ -2353,24 +2429,24 @@
 [[package]]
 name = "windows"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e48a53791691ab099e5e2ad123536d0fff50652600abaf43bbf952894110d0be"
 dependencies = [
  "windows-core",
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-core"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
@@ -2380,15 +2456,15 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -2400,157 +2476,164 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.4",
- "windows_aarch64_msvc 0.52.4",
- "windows_i686_gnu 0.52.4",
- "windows_i686_msvc 0.52.4",
- "windows_x86_64_gnu 0.52.4",
- "windows_x86_64_gnullvm 0.52.4",
- "windows_x86_64_msvc 0.52.4",
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.4"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "xxhash-rust"
 version = "0.8.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "927da81e25be1e1a2901d59b81b37dd2efd1fc9c9345a55007f09bf5a2d3ee03"
 
 [[package]]
 name = "zerocopy"
-version = "0.7.32"
+version = "0.7.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "74d4d3961e53fa4c9a25a8637fc2bfaf2595b3d3ae34875568a5cf64787716be"
+checksum = "ae87e3fcd617500e5d106f0380cf7b77f3c6092aae37191433159dda23cfb087"
 dependencies = [
  "zerocopy-derive",
 ]
 
 [[package]]
 name = "zerocopy-derive"
-version = "0.7.32"
+version = "0.7.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
+checksum = "15e934569e47891f7d9411f1a451d947a60e000ab3bd24fbb970f000387d1b3b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "zstd"
-version = "0.13.0"
+version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bffb3309596d527cfcba7dfc6ed6052f1d39dfbd7c867aa2e865e4a449c10110"
+checksum = "2d789b1514203a1120ad2429eae43a7bd32b90976a7bb8a05f7ec02fa88cc23a"
 dependencies = [
  "zstd-safe",
 ]
 
 [[package]]
 name = "zstd-safe"
-version = "7.0.0"
+version = "7.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "43747c7422e2924c11144d5229878b98180ef8b06cca4ab5af37afc8a8d8ea3e"
+checksum = "1cd99b45c6bc03a018c8b8a86025678c87e55526064e38f9df301989dce7ec0a"
 dependencies = [
  "zstd-sys",
 ]
 
 [[package]]
 name = "zstd-sys"
-version = "2.0.9+zstd.1.5.5"
+version = "2.0.10+zstd.1.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e16efa8a874a0481a574084d34cc26fdb3b99627480f785888deb6386506656"
+checksum = "c253a4914af5bafc8fa8c86ee400827e83cf6ec01195ec1f1ed8441bf00d65aa"
 dependencies = [
  "cc",
  "pkg-config",
 ]
```

### Comparing `polars_cli-0.7.0/LICENSE` & `polars_cli-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_cli-0.7.0/README.md` & `polars_cli-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `polars_cli-0.7.0/python/polars-cli/__main__.py` & `polars_cli-0.8.0/python/polars-cli/__main__.py`

 * *Files identical despite different names*

### Comparing `polars_cli-0.7.0/src/highlighter.rs` & `polars_cli-0.8.0/src/highlighter.rs`

 * *Files identical despite different names*

### Comparing `polars_cli-0.7.0/src/interactive.rs` & `polars_cli-0.8.0/src/interactive.rs`

 * *Files identical despite different names*

### Comparing `polars_cli-0.7.0/src/main.rs` & `polars_cli-0.8.0/src/main.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 #[cfg(feature = "highlight")]
 mod highlighter;
 mod interactive;
 mod prompt;
 
 #[cfg(target_os = "linux")]
 use jemallocator::Jemalloc;
-use polars::prelude::*;
+use polars::prelude::{
+    CsvWriter, DslPlan, IdxSize, IpcWriter, JsonWriter, ParquetWriter, PlHashMap, PlIndexMap,
+    SerWriter,
+};
 use serde::{Deserialize, Serialize};
 
 #[global_allocator]
 #[cfg(target_os = "linux")]
 static ALLOC: Jemalloc = Jemalloc;
 
 use std::io::{self, BufRead};
@@ -110,15 +113,15 @@
             _ => Err(format!("Invalid output mode: {}", s)),
         }
     }
 }
 
 #[derive(Serialize, Deserialize)]
 struct SerializableContext {
-    table_map: PlIndexMap<String, LogicalPlan>,
+    table_map: PlIndexMap<String, DslPlan>,
     tables: Vec<String>,
 }
 
 impl From<&'_ mut SQLContext> for SerializableContext {
     fn from(ctx: &mut SQLContext) -> Self {
         let table_map = ctx
             .clone()
```

### Comparing `polars_cli-0.7.0/src/prompt.rs` & `polars_cli-0.8.0/src/prompt.rs`

 * *Files identical despite different names*

### Comparing `polars_cli-0.7.0/pyproject.toml` & `polars_cli-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polars_cli-0.7.0/PKG-INFO` & `polars_cli-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: polars-cli
-Version: 0.7.0
+Version: 0.8.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

