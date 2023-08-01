# Comparing `tmp/abstract_gui-0.0.54.0.tar.gz` & `tmp/abstract_gui-0.0.54.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_gui-0.0.54.0.tar", last modified: Mon Jul 31 08:20:35 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

