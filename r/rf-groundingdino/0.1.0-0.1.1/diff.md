# Comparing `tmp/rf_groundingdino-0.1.0.tar.gz` & `tmp/rf_groundingdino-0.1.1-cp39-cp39-manylinux_2_17_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rf_groundingdino-0.1.0.tar", last modified: Thu May 25 17:48:33 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

