# Comparing `tmp/digital-sport-0.2.0.tar.gz` & `tmp/digital_sport-0.2.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digital-sport-0.2.0.tar", last modified: Tue Aug  1 11:55:22 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

