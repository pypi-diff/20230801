# Comparing `tmp/fpzip-1.2.1.tar.gz` & `tmp/fpzip-1.2.2-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpzip-1.2.1.tar", last modified: Tue May  2 18:25:32 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

