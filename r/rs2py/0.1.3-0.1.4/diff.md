# Comparing `tmp/rs2py-0.1.3.tar.gz` & `tmp/rs2py-0.1.4.tar.gz`

## Comparing `rs2py-0.1.3.tar` & `rs2py-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      303 1970-01-01 00:00:00.000000 rs2py-0.1.3/Cargo.toml
--rw-r--r--   0     1001      121     1464 2022-07-08 11:01:13.000000 rs2py-0.1.3/.github/workflows/CI.yml
--rw-r--r--   0     1001      121      686 2022-07-08 11:01:13.000000 rs2py-0.1.3/.gitignore
--rw-r--r--   0     1001      121       36 2022-07-08 11:01:13.000000 rs2py-0.1.3/README.md
--rw-r--r--   0     1001      121      561 2022-07-08 11:01:13.000000 rs2py-0.1.3/pyproject.toml
--rwxr-xr-x   0     1001      121      741 2022-07-08 11:01:38.000000 rs2py-0.1.3/run-maturin-action.sh
--rw-r--r--   0     1001      121    36905 2022-07-08 11:01:13.000000 rs2py-0.1.3/src/lib.rs
--rw-r--r--   0     1001      121        0 2022-07-08 11:01:13.000000 rs2py-0.1.3/tests/__init__.py
--rw-r--r--   0     1001      121      178 2022-07-08 11:01:13.000000 rs2py-0.1.3/tests/test_utils.py
--rw-r--r--   0        0        0      525 1970-01-01 00:00:00.000000 rs2py-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      316 1970-01-01 00:00:00.000000 rs2py-0.1.4/Cargo.toml
+-rw-r--r--   0     1001      123     2750 2023-06-01 14:14:01.000000 rs2py-0.1.4/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      686 2023-06-01 14:14:01.000000 rs2py-0.1.4/.gitignore
+-rw-r--r--   0     1001      123       36 2023-06-01 14:14:01.000000 rs2py-0.1.4/README.md
+-rw-r--r--   0     1001      123      716 2023-06-01 14:14:01.000000 rs2py-0.1.4/pyproject.toml
+-rw-r--r--   0     1001      123    37363 2023-06-01 14:14:01.000000 rs2py-0.1.4/src/lib.rs
+-rw-r--r--   0     1001      123        0 2023-06-01 14:14:01.000000 rs2py-0.1.4/tests/__init__.py
+-rw-r--r--   0     1001      123      506 2023-06-01 14:14:01.000000 rs2py-0.1.4/tests/test_utils.py
+-rw-r--r--   0     1001      123     6845 2023-06-01 14:14:01.000000 rs2py-0.1.4/Cargo.lock
+-rw-r--r--   0        0        0      525 1970-01-01 00:00:00.000000 rs2py-0.1.4/PKG-INFO
```

### Comparing `rs2py-0.1.3/.gitignore` & `rs2py-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `rs2py-0.1.3/src/lib.rs` & `rs2py-0.1.4/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 use pyo3::prelude::*;
 
-use std::collections::HashMap;
 use lazy_static::lazy_static;
-
+use std::collections::HashMap;
 
 static IX: [f64; 4999] = [
     0.01, 0.02, 0.03, 0.04, 0.05, 0.06, 0.07, 0.08, 0.09, 0.1, 0.11, 0.12, 0.13, 0.14, 0.15, 0.16,
     0.17, 0.18, 0.19, 0.2, 0.21, 0.22, 0.23, 0.24, 0.25, 0.26, 0.27, 0.28, 0.29, 0.3, 0.31, 0.32,
     0.33, 0.34, 0.35, 0.36, 0.37, 0.38, 0.39, 0.4, 0.41, 0.42, 0.43, 0.44, 0.45, 0.46, 0.47, 0.48,
     0.49, 0.5, 0.51, 0.52, 0.53, 0.54, 0.55, 0.56, 0.57, 0.58, 0.59, 0.6, 0.61, 0.62, 0.63, 0.64,
     0.65, 0.66, 0.67, 0.68, 0.69, 0.7, 0.71, 0.72, 0.73, 0.74, 0.75, 0.76, 0.77, 0.78, 0.79, 0.8,
@@ -381,31 +380,42 @@
         for (i, v) in IX.iter().enumerate() {
             ixmap.insert((v * 100.) as i64, i as i64);
         }
         ixmap
     };
 }
 
-
 /// Formats the sum of two numbers as string.
 #[pyfunction]
 fn get_price_tick_move(a: f64, b: i64) -> f64 {
     let idx: &i64 = IXMAP.get(&((a * 100.) as i64)).unwrap();
     IX[(idx + b) as usize]
 }
 
 #[pyfunction]
 fn get_price_between_tick(a: f64, b: f64) -> i64 {
     let a_idx: &i64 = IXMAP.get(&((a * 100.) as i64)).unwrap();
     let b_idx: &i64 = IXMAP.get(&((b * 100.) as i64)).unwrap();
     b_idx - a_idx
 }
 
-
+#[pyfunction]
+fn get_price_between_ticks(a: f64, b: f64) -> Vec<f64> {
+    let a_idx: i64 = *IXMAP.get(&((a * 100.) as i64)).unwrap();
+    let b_idx: i64 = *IXMAP.get(&((b * 100.) as i64)).unwrap();
+    if b_idx > a_idx {
+        IX[a_idx as usize..=b_idx as usize].to_vec()
+    } else {
+        let mut v = IX[b_idx as usize..=a_idx as usize].to_vec();
+        v.reverse();
+        v
+    }
+}
 
 /// A Python module implemented in Rust.
 #[pymodule]
 fn rs2py(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(get_price_tick_move, m)?)?;
     m.add_function(wrap_pyfunction!(get_price_between_tick, m)?)?;
+    m.add_function(wrap_pyfunction!(get_price_between_ticks, m)?)?;
     Ok(())
 }
```

### Comparing `rs2py-0.1.3/PKG-INFO` & `rs2py-0.1.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rs2py
-Version: 0.1.3
+Version: 0.1.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Rust Extention for Python
 Keywords: rust,python,utils
 Author: YVictor
 Author-email: yvictor3141@gmail.com
```

