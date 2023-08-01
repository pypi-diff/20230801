# Comparing `tmp/mypy-boto3-es-1.28.16.tar.gz` & `tmp/mypy_boto3_es-1.28.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-es-1.28.16.tar", last modified: Tue Aug  1 11:36:46 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

