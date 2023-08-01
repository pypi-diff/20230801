# Comparing `tmp/alchql-3.4.2.30112519.tar.gz` & `tmp/alchql-3.4.2.30112526-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alchql-3.4.2.30112519.tar", last modified: Tue Aug  1 10:12:20 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

