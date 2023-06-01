# Comparing `tmp/reportlab-4.0.0.tar.gz` & `tmp/reportlab-4.0.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reportlab-4.0.0.tar", last modified: Thu May  4 10:31:54 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

