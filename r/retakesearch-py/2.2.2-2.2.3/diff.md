# Comparing `tmp/retakesearch-py-2.2.2.tar.gz` & `tmp/retakesearch_py-2.2.3-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retakesearch-py-2.2.2.tar", last modified: Mon Jul 31 22:54:28 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

