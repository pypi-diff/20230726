# Comparing `tmp/xmodits_py-0.2.4.tar.gz` & `tmp/xmodits_py-0.3.0.tar.gz`

## Comparing `xmodits_py-0.2.4.tar` & `xmodits_py-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0      846 1970-01-01 00:00:00.000000 xmodits_py-0.2.4/Cargo.toml
--rw-r--r--   0     1001      123     2794 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      775 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/.gitignore
--rw-r--r--   0     1001      123    42803 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/LICENSE
--rw-r--r--   0     1001      123     3380 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/README.md
--rw-r--r--   0     1001      123        0 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/examples/example_1.md
--rw-r--r--   0     1001      123      214 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/examples/example_1.py
--rw-r--r--   0     1001      123        0 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/examples/example_2.md
--rw-r--r--   0     1001      123      250 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/examples/example_2.py
--rw-r--r--   0     1001      123        0 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/examples/example_3.md
--rw-r--r--   0     1001      123      253 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/examples/example_3.py
--rw-r--r--   0     1001      123        0 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/examples/example_4.md
--rw-r--r--   0     1001      123      253 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/examples/example_4.py
--rw-r--r--   0     1001      123        0 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/examples/example_5.md
--rw-r--r--   0     1001      123      238 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/examples/example_5.py
--rw-r--r--   0     1001      123        0 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/examples/example_6.md
--rw-r--r--   0     1001      123      504 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/examples/example_6.py
--rw-r--r--   0     1001      123      638 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/pyproject.toml
--rw-r--r--   0     1001      123     1772 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/src/api.rs
--rw-r--r--   0     1001      123     2987 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/src/error.rs
--rw-r--r--   0     1001      123     1179 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/src/lib.rs
--rw-r--r--   0     1001      123    11664 2023-04-10 20:37:42.000000 xmodits_py-0.2.4/Cargo.lock
--rw-r--r--   0        0        0     3934 1970-01-01 00:00:00.000000 xmodits_py-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      808 1970-01-01 00:00:00.000000 xmodits_py-0.3.0/Cargo.toml
+-rw-r--r--   0     1001      123     2859 2023-07-26 17:59:34.000000 xmodits_py-0.3.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      775 2023-07-26 17:59:34.000000 xmodits_py-0.3.0/.gitignore
+-rw-r--r--   0     1001      123       27 2023-07-26 17:59:34.000000 xmodits_py-0.3.0/CHANGELOG.md
+-rw-r--r--   0     1001      123    42803 2023-07-26 17:59:34.000000 xmodits_py-0.3.0/LICENSE
+-rw-r--r--   0     1001      123     3380 2023-07-26 17:59:34.000000 xmodits_py-0.3.0/README.md
+-rw-r--r--   0     1001      123        0 2023-07-26 17:59:34.000000 xmodits_py-0.3.0/examples/example_1.md
+-rw-r--r--   0     1001      123      214 2023-07-26 17:59:34.000000 xmodits_py-0.3.0/examples/example_1.py
+-rw-r--r--   0     1001      123        0 2023-07-26 17:59:34.000000 xmodits_py-0.3.0/examples/example_2.md
+-rw-r--r--   0     1001      123      250 2023-07-26 17:59:34.000000 xmodits_py-0.3.0/examples/example_2.py
+-rw-r--r--   0     1001      123        0 2023-07-26 17:59:34.000000 xmodits_py-0.3.0/examples/example_3.md
+-rw-r--r--   0     1001      123      253 2023-07-26 17:59:34.000000 xmodits_py-0.3.0/examples/example_3.py
+-rw-r--r--   0     1001      123        0 2023-07-26 17:59:34.000000 xmodits_py-0.3.0/examples/example_4.md
+-rw-r--r--   0     1001      123      253 2023-07-26 17:59:34.000000 xmodits_py-0.3.0/examples/example_4.py
+-rw-r--r--   0     1001      123        0 2023-07-26 17:59:34.000000 xmodits_py-0.3.0/examples/example_5.md
+-rw-r--r--   0     1001      123      238 2023-07-26 17:59:34.000000 xmodits_py-0.3.0/examples/example_5.py
+-rw-r--r--   0     1001      123        0 2023-07-26 17:59:34.000000 xmodits_py-0.3.0/examples/example_6.md
+-rw-r--r--   0     1001      123      504 2023-07-26 17:59:34.000000 xmodits_py-0.3.0/examples/example_6.py
+-rw-r--r--   0     1001      123      636 2023-07-26 17:59:34.000000 xmodits_py-0.3.0/pyproject.toml
+-rw-r--r--   0     1001      123     2352 2023-07-26 17:59:34.000000 xmodits_py-0.3.0/src/api.rs
+-rw-r--r--   0     1001      123     3280 2023-07-26 17:59:34.000000 xmodits_py-0.3.0/src/error.rs
+-rw-r--r--   0     1001      123     1214 2023-07-26 17:59:34.000000 xmodits_py-0.3.0/src/lib.rs
+-rw-r--r--   0     1001      123    14511 2023-07-26 17:59:43.000000 xmodits_py-0.3.0/Cargo.lock
+-rw-r--r--   0        0        0     3934 1970-01-01 00:00:00.000000 xmodits_py-0.3.0/PKG-INFO
```

### Comparing `xmodits_py-0.2.4/Cargo.toml` & `xmodits_py-0.3.0/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [package]
 name = "xmodits_py"
 authors = ["B0ney - https://github.com/B0ney"]
 description = "Extract samples from tracker modules. Supports IT, XM, S3M, MOD, UMX, MPTM"
-version = "0.2.4"
+version = "0.3.0"
 edition = "2021"
 license = "LGPLv3"
 readme = "README.md"
 repository = "https://github.com/B0ney/xmodits-py"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "xmodits"
 crate-type = ["cdylib"]
 
-[dependencies]
-xmodits-lib = { git = "https://github.com/B0ney/xmodits-lib", rev = "2101418bda6a7069a889ffc2d3076d963776e3b2"}
+[dependencies.xmodits-lib]
+git = "https://github.com/B0ney/xmodits-lib"
+rev = "b72ca08"
 
 [dependencies.pyo3]
-version = "0.18.1"
+version = "0.19.1"
 features = ["extension-module", "abi3-py37", "anyhow"]
 
 [profile.release]
 strip = true
 opt-level = "s"     
 lto = true          # Enable Link Time Optimization
-codegen-units = 1   # Reduce number of codegen units to increase optimizations.
+codegen-units = 1   # Reduce number of codegen units to increase optimizations.
```

### Comparing `xmodits_py-0.2.4/.github/workflows/CI.yml` & `xmodits_py-0.3.0/.github/workflows/CI.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-# This file is autogenerated by maturin v0.14.15
+# This file is autogenerated by maturin v1.1.0
 # To update, run
 #
 #    maturin generate-ci github
 #
+name: CI
+
 on:
   push:
     branches:
       - main
       - master
     tags:
       - 'v*'
@@ -28,15 +30,15 @@
       - uses: actions/setup-python@v4
         with:
           python-version: '3.10'
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
-          args: --release --out dist
+          args: --release --out dist --find-interpreter
           sccache: 'true'
           manylinux: auto
       - name: Upload wheels
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
@@ -52,15 +54,15 @@
         with:
           python-version: '3.10'
           architecture: ${{ matrix.target }}
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
-          args: --release --out dist
+          args: --release --out dist --find-interpreter
           sccache: 'true'
       - name: Upload wheels
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
 
@@ -74,15 +76,15 @@
       - uses: actions/setup-python@v4
         with:
           python-version: '3.10'
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
-          args: --release --out dist
+          args: --release --out dist --find-interpreter
           sccache: 'true'
       - name: Upload wheels
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
```

### Comparing `xmodits_py-0.2.4/.gitignore` & `xmodits_py-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `xmodits_py-0.2.4/LICENSE` & `xmodits_py-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xmodits_py-0.2.4/README.md` & `xmodits_py-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `xmodits_py-0.2.4/pyproject.toml` & `xmodits_py-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["maturin>=0.14,<0.15"]
+requires = ["maturin>=1.1,<2.0"]
 build-backend = "maturin"
 
 [tool.maturin]
 # "extension-module" tells pyo3 we want to build an extension module (skips linking against libpython.so)
 features = ["pyo3/extension-module"]
 
 [project]
```

### Comparing `xmodits_py-0.2.4/src/api.rs` & `xmodits_py-0.3.0/src/api.rs`

 * *Files 18% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 use std::path::Path;
 use xmodits_lib::common::{extract, SUPPORTED_EXTENSIONS};
 use xmodits_lib::exporter::AudioFormat;
 use xmodits_lib::interface::ripper::Ripper;
 // use xmodits_lib::interface::Error as XmoditsError;
 use xmodits_lib::SampleNamer;
 
-pub fn rip<'a>(
+pub fn rip(
     path: &String,
     destination: String,
     index_raw: Option<bool>,
     index_padding: Option<usize>,
     index_only: Option<bool>,
     with_folder: Option<bool>,
     upper: Option<bool>,
     lower: Option<bool>,
     strict: Option<bool>,
+    format: Option<String>,
 ) -> Result<(), Error> {
     let strict = strict.unwrap_or(true);
     verify_extension(path, strict).map_err(Error::from)?;
 
     let default_namer = SampleNamer::default();
     let ripper = Ripper::new(
         SampleNamer {
@@ -31,15 +32,15 @@
                 .unwrap_or(default_namer.index_padding),
             index_raw: index_raw.unwrap_or_default(),
             lower: lower.unwrap_or_default(),
             upper: upper.unwrap_or_default(),
             ..default_namer
         }
         .into(),
-        AudioFormat::WAV.into(),
+        get_format(format)?.into(),
     );
 
     let self_contained = with_folder.unwrap_or_default();
 
     extract(path, &destination, &ripper, self_contained).map_err(Error::from)
 }
 
@@ -55,7 +56,25 @@
 
     if !SUPPORTED_EXTENSIONS.contains(&ext.as_ref()) {
         return Err(APIError::UnrecognizedFileExtension(ext));
     }
 
     Ok(())
 }
+
+fn get_format(format: Option<String>) -> Result<AudioFormat, APIError> {
+    let Some(format) = format else {
+        return Ok(AudioFormat::WAV);
+    };
+
+    let extension = format.to_lowercase();
+    let format = match extension.as_str() {
+        "wav" => AudioFormat::WAV,
+        "aiff" => AudioFormat::AIFF,
+        "8svx" => AudioFormat::IFF,
+        "its" => AudioFormat::ITS,
+        "s3i" => AudioFormat::S3I,
+        "raw" => AudioFormat::RAW,
+        _ => return Err(APIError::UnrecognizedFileExtension(extension)),
+    };
+    Ok(format)
+}
```

### Comparing `xmodits_py-0.2.4/src/error.rs` & `xmodits_py-0.3.0/src/error.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 use pyo3::exceptions::PyIOError;
 use pyo3::PyErr;
 use xmodits_lib::common::SUPPORTED_EXTENSIONS;
+use xmodits_lib::interface::errors::{ExtractionError, FailedExtraction};
 use xmodits_lib::interface::Error as XmoditsError;
 
 macro_rules! batch_create_exceptions {
     ($($EXCEPTION:ident) *) => {
         $(
             pyo3::create_exception!(xmodits, $EXCEPTION, pyo3::exceptions::PyException);
         )*
@@ -55,24 +56,31 @@
         Self::APIError(value)
     }
 }
 
 fn convert_xmodits(err: XmoditsError) -> PyErr {
     match err {
         XmoditsError::Io(e) => PyIOError::new_err(e.to_string()),
-        XmoditsError::PartialExtraction(e) => PartialExtraction::new_err(partial(e)),
-        XmoditsError::TotalExtraction(e) => TotalExtraction::new_err(total_failure(e)),
         XmoditsError::Extraction(e) => SampleExtraction::new_err(e),
         XmoditsError::UnsupportedModule(e) => UnsupportedFormat::new_err(e),
         XmoditsError::InvalidModule(e) => InvalidModule::new_err(e),
         XmoditsError::EmptyModule => EmptyModule::new_err(empty_module()),
         XmoditsError::AudioFormat(e) => AudioFormat::new_err(audio_format(e)),
         XmoditsError::BadSample { raw_index, .. } => {
             InvalidSample::new_err(invalid_sample(raw_index))
         }
+        XmoditsError::FailedRip(failed_extraction) => match failed_extraction {
+            FailedExtraction::Partial(partial_extraction) => {
+                PartialExtraction::new_err(partial(partial_extraction))
+            }
+            FailedExtraction::Total(total_extraction) => {
+                TotalExtraction::new_err(total_failure(total_extraction))
+            }
+        },
+
         XmoditsError::NoFormatFound => NoFormatFound::new_err(no_format_found()),
     }
 }
 
 pub fn convert_api(err: APIError) -> PyErr {
     match err {
         APIError::UnrecognizedFileExtension(ext) => {
@@ -97,14 +105,14 @@
     "Could not determine a valid format".into()
 }
 
 fn audio_format(error: String) -> String {
     format!("Could not export sample to desired format: {error}")
 }
 
-fn partial(_: Vec<XmoditsError>) -> String {
+fn partial(_: Vec<ExtractionError>) -> String {
     format!("Could not extract everything")
 }
 
-fn total_failure(_: Vec<XmoditsError>) -> String {
+fn total_failure(_: Vec<ExtractionError>) -> String {
     format!("Could not extract anything, the module might be corrupted")
 }
```

### Comparing `xmodits_py-0.2.4/src/lib.rs` & `xmodits_py-0.3.0/src/lib.rs`

 * *Files 9% similar despite different names*

```diff
@@ -9,27 +9,28 @@
     destination: String,          // Folder to put ripped samples
     index_raw: Option<bool>,      // Preserve sample number
     index_padding: Option<usize>, // Set sample number padding
     index_only: Option<bool>,     // Only name sample by their number
     with_folder: Option<bool>,    // Store ripped samples in a self-contained folder
     upper: Option<bool>,          // Name samples in upper case
     lower: Option<bool>,          // Name samples in lower case
-    strict: Option<bool>,         
-    // format: Option<String>,       // Format of exported samples
+    strict: Option<bool>,         // filter by extension
+    format: Option<String>,       // Format of exported samples
 ) -> PyResult<()> {
     api::rip(
         &path,
         destination,
         index_raw,
         index_padding,
         index_only,
         with_folder,
         upper,
         lower,
         strict,
+        format,
     )
     .map_err(PyErr::from)
 }
 
 /// XMODITS python library
 #[pymodule]
 fn xmodits(_py: Python, m: &PyModule) -> PyResult<()> {
```

### Comparing `xmodits_py-0.2.4/Cargo.lock` & `xmodits_py-0.3.0/Cargo.lock`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "anyhow"
-version = "1.0.70"
+version = "1.0.72"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7de8ce5e0f9f8d88245311066a578d72b7af3e7088f32783804676302df237e4"
+checksum = "3b13c32d80ecc7ab747b80c3784bce54ee8a7a0cc4fbda9bf4cda2cf6fe90854"
+
+[[package]]
+name = "ascii"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d92bec98840b8f03a5ff5413de5293bfcd8bf96467cf5452609f939ec6f5de16"
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
@@ -29,46 +35,165 @@
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "dasp"
+version = "0.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7381b67da416b639690ac77c73b86a7b5e64a29e31d1f75fb3b1102301ef355a"
+dependencies = [
+ "dasp_envelope",
+ "dasp_frame",
+ "dasp_interpolate",
+ "dasp_peak",
+ "dasp_ring_buffer",
+ "dasp_rms",
+ "dasp_sample",
+ "dasp_signal",
+ "dasp_slice",
+ "dasp_window",
+]
+
+[[package]]
+name = "dasp_envelope"
+version = "0.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8ec617ce7016f101a87fe85ed44180839744265fae73bb4aa43e7ece1b7668b6"
+dependencies = [
+ "dasp_frame",
+ "dasp_peak",
+ "dasp_ring_buffer",
+ "dasp_rms",
+ "dasp_sample",
+]
+
+[[package]]
+name = "dasp_frame"
+version = "0.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2a3937f5fe2135702897535c8d4a5553f8b116f76c1529088797f2eee7c5cd6"
+dependencies = [
+ "dasp_sample",
+]
+
+[[package]]
+name = "dasp_interpolate"
+version = "0.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7fc975a6563bb7ca7ec0a6c784ead49983a21c24835b0bc96eea11ee407c7486"
+dependencies = [
+ "dasp_frame",
+ "dasp_ring_buffer",
+ "dasp_sample",
+]
+
+[[package]]
+name = "dasp_peak"
+version = "0.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5cf88559d79c21f3d8523d91250c397f9a15b5fc72fbb3f87fdb0a37b79915bf"
+dependencies = [
+ "dasp_frame",
+ "dasp_sample",
+]
+
+[[package]]
+name = "dasp_ring_buffer"
+version = "0.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "07d79e19b89618a543c4adec9c5a347fe378a19041699b3278e616e387511ea1"
+
+[[package]]
+name = "dasp_rms"
+version = "0.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a6c5dcb30b7e5014486e2822537ea2beae50b19722ffe2ed7549ab03774575aa"
+dependencies = [
+ "dasp_frame",
+ "dasp_ring_buffer",
+ "dasp_sample",
+]
+
+[[package]]
+name = "dasp_sample"
+version = "0.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0c87e182de0887fd5361989c677c4e8f5000cd9491d6d563161a8f3a5519fc7f"
+
+[[package]]
+name = "dasp_signal"
+version = "0.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "aa1ab7d01689c6ed4eae3d38fe1cea08cba761573fbd2d592528d55b421077e7"
+dependencies = [
+ "dasp_envelope",
+ "dasp_frame",
+ "dasp_interpolate",
+ "dasp_peak",
+ "dasp_ring_buffer",
+ "dasp_rms",
+ "dasp_sample",
+ "dasp_window",
+]
+
+[[package]]
+name = "dasp_slice"
+version = "0.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4e1c7335d58e7baedafa516cb361360ff38d6f4d3f9d9d5ee2a2fc8e27178fa1"
+dependencies = [
+ "dasp_frame",
+ "dasp_sample",
+]
+
+[[package]]
+name = "dasp_window"
+version = "0.11.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "99ded7b88821d2ce4e8b842c9f1c86ac911891ab89443cc1de750cae764c5076"
+dependencies = [
+ "dasp_sample",
+]
+
+[[package]]
 name = "extended"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "af9673d8203fcb076b19dfd17e38b3d4ae9f44959416ea532ce72415a6020365"
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "libc"
-version = "0.2.141"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3304a64d199bb964be99741b7a14d26972741915b3649639149b2479bb46f4b5"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.8.0"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num-complex"
 version = "0.4.3"
@@ -86,73 +211,73 @@
 dependencies = [
  "autocfg",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.15"
+version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
+checksum = "f30b0abd723be7e2ffca1272140fac1a2f084c77ec3e123c192b66af1ee9e6c2"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.7"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-targets",
 ]
 
 [[package]]
 name = "primal-check"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9df7f93fd637f083201473dab4fee2db4c429d32e55e3299980ab3957ab916a0"
 dependencies = [
  "num-integer",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.56"
+version = "1.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
+checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.2"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cfb848f80438f926a9ebddf0a539ed6065434fd7aae03a89312a9821f81b8501"
+checksum = "ffb88ae05f306b4bfcde40ac4a51dc0b05936a9207a4b75b798c7729c4258a59"
 dependencies = [
  "anyhow",
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
@@ -160,78 +285,78 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.2"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "98a42e7f42e917ce6664c832d5eee481ad514c98250c49e0b03b20593e2c7ed0"
+checksum = "554db24f0b3c180a9c0b1268f91287ab3f17c162e15b54caaae5a6b3773396b0"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.2"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0707f0ab26826fe4ccd59b69106e9df5e12d097457c7b8f9c0fd1d2743eec4d"
+checksum = "922ede8759e8600ad4da3195ae41259654b9c55da4f7eec84a0ccc7d067a70a4"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.2"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978d18e61465ecd389e1f235ff5a467146dc4e3c3968b90d274fe73a5dd4a438"
+checksum = "8a5caec6a1dd355964a841fcbeeb1b89fe4146c87295573f94228911af3cc5a2"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.2"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e0e1128f85ce3fca66e435e08aa2089a2689c1c48ce97803e13f63124058462"
+checksum = "e0b78ccbb160db1556cdb6fd96c50334c5d4ec44dc5e0a968d0a1208fa0efa8b"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.26"
+version = "1.0.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
+checksum = "50f3b39ccfb720540debaa0164757101c08ecb8d326b15358ce76a62c7e85965"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "realfft"
-version = "3.2.0"
+version = "3.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93d6b8e8f0c6d2234aa58048d7290c60bf92cd36fd2888cd8331c66ad4f2e1d2"
+checksum = "953d9f7e5cdd80963547b456251296efc2626ed4e3cbf36c869d9564e0220571"
 dependencies = [
  "rustfft",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "rubato"
 version = "0.12.0"
@@ -257,23 +382,23 @@
  "strength_reduce",
  "transpose",
  "version_check",
 ]
 
 [[package]]
 name = "scopeguard"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
 name = "strength_reduce"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fe895eb47f22e2ddd4dabc02bce419d2e643c8e3b585c78158b349195bc24d82"
 
@@ -286,154 +411,147 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.13"
+version = "2.0.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c9da457c5285ac1f936ebd076af6dac17a61cfe7826f2076b4d015cf47bc8ec"
+checksum = "b60f673f44a8255b9c8c657daf66a596d435f2da81a555b06dc644d080ba45e0"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.6"
+version = "0.12.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+checksum = "1d2faeef5759ab89935255b1a4cd98e0baf99d1085e37d36599c625dac49ae8e"
 
 [[package]]
 name = "thiserror"
-version = "1.0.40"
+version = "1.0.44"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
+checksum = "611040a08a0439f8248d1990b111c95baa9c704c805fa1f62104b39655fd7f90"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.40"
+version = "1.0.44"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
+checksum = "090198534930841fab3a5d1bb637cde49e339654e606195f8d9c76eeb081dc96"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.13",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "transpose"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e6522d49d03727ffb138ae4cbc1283d3774f0d10aa7f9bf52e6784c45daf9b23"
 dependencies = [
  "num-integer",
  "strength_reduce",
 ]
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "301abaae475aa91687eb82514b328ab47a211a533026cb25fc3e519b86adfc3c"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
-name = "windows-sys"
-version = "0.45.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
-dependencies = [
- "windows-targets",
-]
-
-[[package]]
 name = "windows-targets"
-version = "0.42.2"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
 name = "xmodits-lib"
-version = "0.6.0"
-source = "git+https://github.com/B0ney/xmodits-lib?rev=2101418bda6a7069a889ffc2d3076d963776e3b2#2101418bda6a7069a889ffc2d3076d963776e3b2"
+version = "0.7.0"
+source = "git+https://github.com/B0ney/xmodits-lib?rev=b72ca08#b72ca0892d21d5aa4c19ee8752710253664eb00f"
 dependencies = [
+ "ascii",
  "bytemuck",
+ "dasp",
  "extended",
  "rubato",
  "thiserror",
 ]
 
 [[package]]
 name = "xmodits_py"
-version = "0.2.4"
+version = "0.3.0"
 dependencies = [
  "pyo3",
  "xmodits-lib",
 ]
```

### Comparing `xmodits_py-0.2.4/PKG-INFO` & `xmodits_py-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmodits_py
-Version: 0.2.4
+Version: 0.3.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Extract samples from tracker modules. Supports IT, XM, S3M, MOD, UMX, MPTM
 Author: B0ney - https://github.com/B0ney
 License: LGPLv3
```

