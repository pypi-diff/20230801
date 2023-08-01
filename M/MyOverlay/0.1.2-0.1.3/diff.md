# Comparing `tmp/MyOverlay-0.1.2.tar.gz` & `tmp/MyOverlay-0.1.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MyOverlay-0.1.2.tar", last modified: Tue Aug  1 09:05:09 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

