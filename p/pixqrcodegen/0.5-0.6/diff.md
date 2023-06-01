# Comparing `tmp/pixqrcodegen-0.5.tar.gz` & `tmp/pixqrcodegen-0.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixqrcodegen-0.5.tar", last modified: Sun Sep 18 18:40:26 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

