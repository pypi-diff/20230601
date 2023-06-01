# Comparing `tmp/Indago-0.4.4.tar.gz` & `tmp/Indago-0.4.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Indago-0.4.4.tar", last modified: Wed Mar  1 13:01:36 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

