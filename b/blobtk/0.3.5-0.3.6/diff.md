# Comparing `tmp/blobtk-0.3.5.tar.gz` & `tmp/blobtk-0.3.6.tar.gz`

## Comparing `blobtk-0.3.5.tar` & `blobtk-0.3.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1410 1970-01-01 00:00:00.000000 blobtk-0.3.5/Cargo.toml
--rw-r--r--   0      501       20    60602 2023-05-22 15:31:33.000000 blobtk-0.3.5/Cargo.lock
--rw-r--r--   0      501       20      313 2023-05-22 15:31:33.000000 blobtk-0.3.5/pyproject.toml
--rw-r--r--   0      501       20     9018 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/bam.rs
--rw-r--r--   0      501       20    20229 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/blobdir.rs
--rw-r--r--   0      501       20     8857 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/cli.rs
--rw-r--r--   0      501       20      541 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/depth.rs
--rw-r--r--   0      501       20      723 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/error.rs
--rw-r--r--   0      501       20     1855 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/fasta.rs
--rw-r--r--   0      501       20     6177 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/fastq.rs
--rw-r--r--   0      501       20     1416 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/filter.rs
--rw-r--r--   0      501       20     2738 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/io.rs
--rw-r--r--   0      501       20      824 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/lib.rs
--rw-r--r--   0      501       20      650 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/main.rs
--rw-r--r--   0      501       20     4174 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/plot/axis.rs
--rw-r--r--   0      501       20    22851 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/plot/blob.rs
--rw-r--r--   0      501       20     5567 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/plot/category.rs
--rw-r--r--   0      501       20     5730 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/plot/chart.rs
--rw-r--r--   0      501       20    38069 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/plot/component.rs
--rw-r--r--   0      501       20     5835 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/plot/cumulative.rs
--rw-r--r--   0      501       20     4422 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/plot/data.rs
--rw-r--r--   0      501       20    30467 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/plot/snail.rs
--rw-r--r--   0      501       20     1020 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/plot/style.rs
--rw-r--r--   0      501       20    12399 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/plot.rs
--rw-r--r--   0      501       20     3172 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/python/depth.rs
--rw-r--r--   0      501       20     3518 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/python/filter.rs
--rw-r--r--   0      501       20     1879 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/python/utils.rs
--rw-r--r--   0      501       20      491 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/python.rs
--rw-r--r--   0      501       20     4497 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/taxonomy.rs
--rw-r--r--   0      501       20     8053 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/utils.rs
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 blobtk-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1568 1970-01-01 00:00:00.000000 blobtk-0.3.6/Cargo.toml
+-rw-r--r--   0     1001      123    60602 2023-06-01 12:42:15.000000 blobtk-0.3.6/Cargo.lock
+-rw-r--r--   0     1001      123      313 2023-06-01 12:42:15.000000 blobtk-0.3.6/pyproject.toml
+-rw-r--r--   0     1001      123     9018 2023-06-01 12:42:15.000000 blobtk-0.3.6/src/bam.rs
+-rw-r--r--   0     1001      123    20229 2023-06-01 12:42:15.000000 blobtk-0.3.6/src/blobdir.rs
+-rw-r--r--   0     1001      123     8857 2023-06-01 12:42:15.000000 blobtk-0.3.6/src/cli.rs
+-rw-r--r--   0     1001      123      541 2023-06-01 12:42:15.000000 blobtk-0.3.6/src/depth.rs
+-rw-r--r--   0     1001      123      723 2023-06-01 12:42:15.000000 blobtk-0.3.6/src/error.rs
+-rw-r--r--   0     1001      123     1855 2023-06-01 12:42:15.000000 blobtk-0.3.6/src/fasta.rs
+-rw-r--r--   0     1001      123     6177 2023-06-01 12:42:15.000000 blobtk-0.3.6/src/fastq.rs
+-rw-r--r--   0     1001      123     1416 2023-06-01 12:42:15.000000 blobtk-0.3.6/src/filter.rs
+-rw-r--r--   0     1001      123     2738 2023-06-01 12:42:15.000000 blobtk-0.3.6/src/io.rs
+-rw-r--r--   0     1001      123      824 2023-06-01 12:42:15.000000 blobtk-0.3.6/src/lib.rs
+-rw-r--r--   0     1001      123      650 2023-06-01 12:42:15.000000 blobtk-0.3.6/src/main.rs
+-rw-r--r--   0     1001      123     4174 2023-06-01 12:42:15.000000 blobtk-0.3.6/src/plot/axis.rs
+-rw-r--r--   0     1001      123    22851 2023-06-01 12:42:15.000000 blobtk-0.3.6/src/plot/blob.rs
+-rw-r--r--   0     1001      123     5567 2023-06-01 12:42:15.000000 blobtk-0.3.6/src/plot/category.rs
+-rw-r--r--   0     1001      123     5730 2023-06-01 12:42:15.000000 blobtk-0.3.6/src/plot/chart.rs
+-rw-r--r--   0     1001      123    38069 2023-06-01 12:42:15.000000 blobtk-0.3.6/src/plot/component.rs
+-rw-r--r--   0     1001      123     5835 2023-06-01 12:42:15.000000 blobtk-0.3.6/src/plot/cumulative.rs
+-rw-r--r--   0     1001      123     4422 2023-06-01 12:42:15.000000 blobtk-0.3.6/src/plot/data.rs
+-rw-r--r--   0     1001      123    30467 2023-06-01 12:42:15.000000 blobtk-0.3.6/src/plot/snail.rs
+-rw-r--r--   0     1001      123     1020 2023-06-01 12:42:15.000000 blobtk-0.3.6/src/plot/style.rs
+-rw-r--r--   0     1001      123    12399 2023-06-01 12:42:15.000000 blobtk-0.3.6/src/plot.rs
+-rw-r--r--   0     1001      123     3172 2023-06-01 12:42:15.000000 blobtk-0.3.6/src/python/depth.rs
+-rw-r--r--   0     1001      123     3518 2023-06-01 12:42:15.000000 blobtk-0.3.6/src/python/filter.rs
+-rw-r--r--   0     1001      123     1879 2023-06-01 12:42:15.000000 blobtk-0.3.6/src/python/utils.rs
+-rw-r--r--   0     1001      123      491 2023-06-01 12:42:15.000000 blobtk-0.3.6/src/python.rs
+-rw-r--r--   0     1001      123     4497 2023-06-01 12:42:15.000000 blobtk-0.3.6/src/taxonomy.rs
+-rw-r--r--   0     1001      123     8053 2023-06-01 12:42:15.000000 blobtk-0.3.6/src/utils.rs
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 blobtk-0.3.6/PKG-INFO
```

### Comparing `blobtk-0.3.5/Cargo.toml` & `blobtk-0.3.6/Cargo.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "blobtk"
-version = "0.3.5"
+version = "0.3.6"
 edition = "2021"
 authors = [
     "Rich Challis <rc28@sanger.ac.uk>",
 ]
 license = "MIT"
 description = "Core utilities for BlobToolKit."
 homepage = "https://github.com/blobtoolkit/blobtk"
@@ -25,14 +25,21 @@
 
 [profile.release]
 strip = true
 lto = true
 codegen-units = 1
 panic = "abort"
 
+[target.x86_64-unknown-linux-gnu]
+rustflags = ["-C", "target-feature=+crt-static"]
+
+[aarch64-apple-darwin]
+rustflags = ["-C", "target-feature=+crt-static"]
+
+
 [dependencies]
 anyhow = "1.0.71"
 atty = "0.2.14"
 clap = { version = "4.0.29", features = [ "derive" ]}
 clap-num = "1.0.2"
 colorous = "1.0.10"
 coord_transforms = "1.4.0"
```

### Comparing `blobtk-0.3.5/Cargo.lock` & `blobtk-0.3.6/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "blobtk"
-version = "0.3.5"
+version = "0.3.6"
 dependencies = [
  "anyhow",
  "atty",
  "clap",
  "clap-num",
  "colorous",
  "coord_transforms",
```

### Comparing `blobtk-0.3.5/src/bam.rs` & `blobtk-0.3.6/src/bam.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.5/src/blobdir.rs` & `blobtk-0.3.6/src/blobdir.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.5/src/cli.rs` & `blobtk-0.3.6/src/cli.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.5/src/depth.rs` & `blobtk-0.3.6/src/depth.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.5/src/error.rs` & `blobtk-0.3.6/src/error.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.5/src/fasta.rs` & `blobtk-0.3.6/src/fasta.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.5/src/fastq.rs` & `blobtk-0.3.6/src/fastq.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.5/src/filter.rs` & `blobtk-0.3.6/src/filter.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.5/src/io.rs` & `blobtk-0.3.6/src/io.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.5/src/lib.rs` & `blobtk-0.3.6/src/lib.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.5/src/main.rs` & `blobtk-0.3.6/src/main.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.5/src/plot/axis.rs` & `blobtk-0.3.6/src/plot/axis.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.5/src/plot/blob.rs` & `blobtk-0.3.6/src/plot/blob.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.5/src/plot/category.rs` & `blobtk-0.3.6/src/plot/category.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.5/src/plot/chart.rs` & `blobtk-0.3.6/src/plot/chart.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.5/src/plot/component.rs` & `blobtk-0.3.6/src/plot/component.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.5/src/plot/cumulative.rs` & `blobtk-0.3.6/src/plot/cumulative.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.5/src/plot/data.rs` & `blobtk-0.3.6/src/plot/data.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.5/src/plot/snail.rs` & `blobtk-0.3.6/src/plot/snail.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.5/src/plot/style.rs` & `blobtk-0.3.6/src/plot/style.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.5/src/plot.rs` & `blobtk-0.3.6/src/plot.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.5/src/python/depth.rs` & `blobtk-0.3.6/src/python/depth.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.5/src/python/filter.rs` & `blobtk-0.3.6/src/python/filter.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.5/src/python/utils.rs` & `blobtk-0.3.6/src/python/utils.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.5/src/taxonomy.rs` & `blobtk-0.3.6/src/taxonomy.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.5/src/utils.rs` & `blobtk-0.3.6/src/utils.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.5/PKG-INFO` & `blobtk-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blobtk
-Version: 0.3.5
+Version: 0.3.6
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Core utilities for BlobToolKit.
 Keywords: bioinformatics,blobtoolkit,genome,genomics
 Home-Page: https://github.com/blobtoolkit/blobtk
 Author: Rich Challis <rc28@sanger.ac.uk>
```

