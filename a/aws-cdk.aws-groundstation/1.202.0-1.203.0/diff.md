# Comparing `tmp/aws-cdk.aws-groundstation-1.202.0.tar.gz` & `tmp/aws_cdk.aws_groundstation-1.203.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src306747024/src/packages/@aws-cdk/aws-groundstation/dist/python/aws-cdk.aws-groundstation-1.202.0.tar", last modified: Fri May 19 23:13:12 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

