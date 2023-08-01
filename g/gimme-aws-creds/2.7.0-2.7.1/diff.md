# Comparing `tmp/gimme aws creds-2.7.0.tar.gz` & `tmp/gimme_aws_creds-2.7.1-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gimme aws creds-2.7.0.tar", last modified: Thu Jun 22 16:25:25 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

