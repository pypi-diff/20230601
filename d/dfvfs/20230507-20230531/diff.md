# Comparing `tmp/dfvfs-20230507.tar.gz` & `tmp/dfvfs-20230531-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfvfs-20230507.tar", last modified: Sun May  7 16:50:11 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

