# Comparing `tmp/passwordless-client-0.1.0.tar.gz` & `tmp/passwordless_client-0.1.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passwordless-client-0.1.0.tar", last modified: Mon Jul 31 17:10:01 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

