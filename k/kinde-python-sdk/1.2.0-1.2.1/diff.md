# Comparing `tmp/kinde-python-sdk-1.2.0.tar.gz` & `tmp/kinde_python_sdk-1.2.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kinde-python-sdk-1.2.0.tar", last modified: Thu May 25 05:25:32 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

