# Comparing `tmp/HTSeq-2.0.3.tar.gz` & `tmp/HTSeq-2.0.4-cp310-cp310-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/io/wheelhouse/HTSeq-2.0.3.tar", last modified: Tue May 16 03:58:04 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

