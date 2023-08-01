# Comparing `tmp/xarg-python-0.7.tar.gz` & `tmp/xarg_python-0.8-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarg-python-0.7.tar", last modified: Fri Jul 28 05:40:58 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

