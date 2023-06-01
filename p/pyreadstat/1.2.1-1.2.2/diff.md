# Comparing `tmp/pyreadstat-1.2.1.tar.gz` & `tmp/pyreadstat-1.2.2-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreadstat-1.2.1.tar", last modified: Wed Feb 22 11:52:10 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

