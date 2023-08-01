# Comparing `tmp/camSort-0.2.5.tar.gz` & `tmp/camSort-0.2.6-cp37-cp37m-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/camSort-0.2.5.tar", last modified: Tue Aug  1 08:55:40 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

