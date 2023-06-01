# Comparing `tmp/efshape-0.1.1.tar.gz` & `tmp/efshape-1.0.0-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efshape-0.1.1.tar", last modified: Thu Apr 27 10:56:21 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

