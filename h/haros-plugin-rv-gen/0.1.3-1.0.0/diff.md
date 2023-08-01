# Comparing `tmp/haros-plugin-rv-gen-0.1.3.tar.gz` & `tmp/haros_plugin_rv_gen-1.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/haros-plugin-rv-gen-0.1.3.tar", last modified: Thu Aug 12 09:09:04 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

