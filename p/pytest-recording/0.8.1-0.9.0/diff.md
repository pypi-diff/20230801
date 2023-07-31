# Comparing `tmp/pytest-recording-0.8.1.tar.gz` & `tmp/pytest_recording-0.9.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-recording-0.8.1.tar", last modified: Sat Jun 13 15:04:08 2020, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

