# Comparing `tmp/physicsLab-1.3.0.1.tar.gz` & `tmp/physicsLab-1.3.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\physicsLab-1.3.0.1.tar", last modified: Sat Jul 29 08:55:00 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

