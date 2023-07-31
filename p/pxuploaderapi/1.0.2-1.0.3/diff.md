# Comparing `tmp/pxuploaderapi-1.0.2.tar.gz` & `tmp/pxuploaderapi-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pxuploaderapi-1.0.2.tar", last modified: Fri Jul 28 16:34:18 2023, max compression
+gzip compressed data, was "pxuploaderapi-1.0.3.tar", last modified: Mon Jul 31 22:16:11 2023, max compression
```

## Comparing `pxuploaderapi-1.0.2.tar` & `pxuploaderapi-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 16:34:18.221849 pxuploaderapi-1.0.2/
--rw-rw-rw-   0        0        0      333 2023-07-28 16:34:18.221849 pxuploaderapi-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      108 2023-07-06 23:26:11.000000 pxuploaderapi-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      523 2023-07-28 16:34:18.221849 pxuploaderapi-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-28 16:34:18.221849 pxuploaderapi-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-28 16:34:18.221849 pxuploaderapi-1.0.2/src/pxuploaderapi/
--rw-rw-rw-   0        0        0      867 2023-07-28 16:20:26.000000 pxuploaderapi-1.0.2/src/pxuploaderapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 16:34:18.221849 pxuploaderapi-1.0.2/src/pxuploaderapi.egg-info/
--rw-rw-rw-   0        0        0      333 2023-07-28 16:34:18.000000 pxuploaderapi-1.0.2/src/pxuploaderapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-07-28 16:34:18.000000 pxuploaderapi-1.0.2/src/pxuploaderapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 16:34:18.000000 pxuploaderapi-1.0.2/src/pxuploaderapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-28 16:34:18.000000 pxuploaderapi-1.0.2/src/pxuploaderapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 22:16:11.892197 pxuploaderapi-1.0.3/
+-rw-rw-rw-   0        0        0      333 2023-07-31 22:16:11.892197 pxuploaderapi-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      108 2023-07-06 23:26:11.000000 pxuploaderapi-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      523 2023-07-31 22:16:11.892197 pxuploaderapi-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-31 22:16:11.876577 pxuploaderapi-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-31 22:16:11.892197 pxuploaderapi-1.0.3/src/pxuploaderapi/
+-rw-rw-rw-   0        0        0      954 2023-07-31 22:14:15.000000 pxuploaderapi-1.0.3/src/pxuploaderapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 22:16:11.892197 pxuploaderapi-1.0.3/src/pxuploaderapi.egg-info/
+-rw-rw-rw-   0        0        0      333 2023-07-31 22:16:11.000000 pxuploaderapi-1.0.3/src/pxuploaderapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-07-31 22:16:11.000000 pxuploaderapi-1.0.3/src/pxuploaderapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 22:16:11.000000 pxuploaderapi-1.0.3/src/pxuploaderapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-31 22:16:11.000000 pxuploaderapi-1.0.3/src/pxuploaderapi.egg-info/top_level.txt
```

### Comparing `pxuploaderapi-1.0.2/setup.cfg` & `pxuploaderapi-1.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7875 706c 6f61 6465 7261 7069   = pxuploaderapi
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 302e  ..version = 1.0.
-00000030: 320d 0a61 7574 686f 7220 3d20 506f 756e  2..author = Poun
+00000030: 330d 0a61 7574 686f 7220 3d20 506f 756e  3..author = Poun
 00000040: 6465 7820 4173 736f 6369 6174 6573 2043  dex Associates C
 00000050: 6f72 706f 7261 7469 6f6e 0d0a 6175 7468  orporation..auth
 00000060: 6f72 5f65 6d61 696c 203d 2069 7440 706f  or_email = it@po
 00000070: 756e 6465 782e 636f 6d0d 0a64 6573 6372  undex.com..descr
 00000080: 6970 7469 6f6e 203d 200d 0a6c 6f6e 675f  iption = ..long_
 00000090: 6465 7363 7269 7074 696f 6e20 3d20 0d0a  description = ..
 000000a0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
```

### Comparing `pxuploaderapi-1.0.2/src/pxuploaderapi/__init__.py` & `pxuploaderapi-1.0.3/src/pxuploaderapi/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 
     def getName(self) -> str:
         return self.getUploader()["name"]
     
     def getUUID(self) -> str:
         return self.getUploader()["uuid"]
     
+    def getTesting(self) -> bool:
+        return self.getUploader()["testing"]
+    
     def getFields(self) -> dict:
         return self.getUploader()["fields"]
 
     def getUploader(self) -> dict:
         return self.uploader_dict
     
     def getTestOptions(self) -> dict:
```

