# Comparing `tmp/photcalib-0.2.tar.gz` & `tmp/photcalib-0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "photcalib-0.2.tar", last modified: Tue Aug  1 14:11:47 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

