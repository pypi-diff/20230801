# Comparing `tmp/botocore-a-la-carte-entityresolution-1.31.15.tar.gz` & `tmp/botocore_a_la_carte_entityresolution-1.31.16-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-entityresolution-1.31.15.tar", last modified: Sat Jul 29 01:14:03 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

