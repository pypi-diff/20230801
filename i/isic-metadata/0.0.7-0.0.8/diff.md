# Comparing `tmp/isic-metadata-0.0.7.tar.gz` & `tmp/isic-metadata-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isic-metadata-0.0.7.tar", last modified: Wed Jul  5 15:56:44 2023, max compression
+gzip compressed data, was "isic-metadata-0.0.8.tar", last modified: Tue Aug  1 21:05:29 2023, max compression
```

## Comparing `isic-metadata-0.0.7.tar` & `isic-metadata-0.0.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:56:44.250575 isic-metadata-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-05 15:56:19.000000 isic-metadata-0.0.7/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-05 15:56:19.000000 isic-metadata-0.0.7/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:56:44.234575 isic-metadata-0.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:56:44.242575 isic-metadata-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-05 15:56:19.000000 isic-metadata-0.0.7/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-05 15:56:19.000000 isic-metadata-0.0.7/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-05 15:56:19.000000 isic-metadata-0.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-05 15:56:19.000000 isic-metadata-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-05 15:56:44.250575 isic-metadata-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-05 15:56:19.000000 isic-metadata-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:56:44.246575 isic-metadata-0.0.7/isic_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-07-05 15:56:19.000000 isic-metadata-0.0.7/isic_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-07-05 15:56:19.000000 isic-metadata-0.0.7/isic_metadata/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-07-05 15:56:19.000000 isic-metadata-0.0.7/isic_metadata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-05 15:56:19.000000 isic-metadata-0.0.7/isic_metadata/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 15:56:19.000000 isic-metadata-0.0.7/isic_metadata/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:56:44.246575 isic-metadata-0.0.7/isic_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-05 15:56:44.000000 isic-metadata-0.0.7/isic_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-05 15:56:44.000000 isic-metadata-0.0.7/isic_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 15:56:44.000000 isic-metadata-0.0.7/isic_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-05 15:56:44.000000 isic-metadata-0.0.7/isic_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-05 15:56:44.000000 isic-metadata-0.0.7/isic_metadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-05 15:56:19.000000 isic-metadata-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 15:56:44.250575 isic-metadata-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-05 15:56:19.000000 isic-metadata-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:56:44.246575 isic-metadata-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-05 15:56:19.000000 isic-metadata-0.0.7/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-05 15:56:19.000000 isic-metadata-0.0.7/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-05 15:56:19.000000 isic-metadata-0.0.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:05:29.424707 isic-metadata-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-01 21:05:02.000000 isic-metadata-0.0.8/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-01 21:05:02.000000 isic-metadata-0.0.8/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:05:29.416706 isic-metadata-0.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:05:29.420706 isic-metadata-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-01 21:05:02.000000 isic-metadata-0.0.8/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-01 21:05:02.000000 isic-metadata-0.0.8/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-08-01 21:05:02.000000 isic-metadata-0.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 21:05:02.000000 isic-metadata-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-01 21:05:29.424707 isic-metadata-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-01 21:05:02.000000 isic-metadata-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:05:29.420706 isic-metadata-0.0.8/isic_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-08-01 21:05:02.000000 isic-metadata-0.0.8/isic_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-08-01 21:05:02.000000 isic-metadata-0.0.8/isic_metadata/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-08-01 21:05:02.000000 isic-metadata-0.0.8/isic_metadata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-08-01 21:05:02.000000 isic-metadata-0.0.8/isic_metadata/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 21:05:02.000000 isic-metadata-0.0.8/isic_metadata/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:05:29.420706 isic-metadata-0.0.8/isic_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-01 21:05:29.000000 isic-metadata-0.0.8/isic_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-01 21:05:29.000000 isic-metadata-0.0.8/isic_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 21:05:29.000000 isic-metadata-0.0.8/isic_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 21:05:29.000000 isic-metadata-0.0.8/isic_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-01 21:05:29.000000 isic-metadata-0.0.8/isic_metadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-08-01 21:05:02.000000 isic-metadata-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 21:05:29.424707 isic-metadata-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-01 21:05:02.000000 isic-metadata-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:05:29.420706 isic-metadata-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-08-01 21:05:02.000000 isic-metadata-0.0.8/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-01 21:05:02.000000 isic-metadata-0.0.8/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-08-01 21:05:02.000000 isic-metadata-0.0.8/tox.ini
```

### Comparing `isic-metadata-0.0.7/.github/workflows/ci.yml` & `isic-metadata-0.0.8/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `isic-metadata-0.0.7/.github/workflows/release.yml` & `isic-metadata-0.0.8/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `isic-metadata-0.0.7/.gitignore` & `isic-metadata-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `isic-metadata-0.0.7/LICENSE` & `isic-metadata-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `isic-metadata-0.0.7/PKG-INFO` & `isic-metadata-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isic-metadata
-Version: 0.0.7
+Version: 0.0.8
 Home-page: https://github.com/ImageMarkup/isic-metadata
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/ImageMarkup/isic-metadata/issues
 Project-URL: Source, https://github.com/ImageMarkup/isic-metadata
 Keywords: requests
```

### Comparing `isic-metadata-0.0.7/isic_metadata/__init__.py` & `isic-metadata-0.0.8/isic_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `isic-metadata-0.0.7/isic_metadata/fields.py` & `isic-metadata-0.0.8/isic_metadata/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,16 +180,18 @@
         if value not in NevusTypeEnum._value2member_map_:
             raise ValueError(f"Invalid nevus type of: {value}.")
         return value
 
 
 class ImageTypeEnum(str, Enum):
     dermoscopic = "dermoscopic"
-    clinical = "clinical"
-    overview = "overview"
+    clinical_close_up = "clinical: close-up"
+    clinical_overview = "clinical: overview"
+    tbp_tile_close_up = "TBP tile: close-up"
+    tbp_tile_overview = "TBP tile: overview"
 
 
 class ImageType(BaseStr):
     @classmethod
     def validate(cls, value: str) -> str | None:
         if value not in ImageTypeEnum._value2member_map_:
             raise ValueError(f"Invalid image type of: {value}.")
```

### Comparing `isic-metadata-0.0.7/isic_metadata/metadata.py` & `isic-metadata-0.0.8/isic_metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `isic-metadata-0.0.7/isic_metadata/utils.py` & `isic-metadata-0.0.8/isic_metadata/utils.py`

 * *Files identical despite different names*

### Comparing `isic-metadata-0.0.7/isic_metadata.egg-info/PKG-INFO` & `isic-metadata-0.0.8/isic_metadata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isic-metadata
-Version: 0.0.7
+Version: 0.0.8
 Home-page: https://github.com/ImageMarkup/isic-metadata
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/ImageMarkup/isic-metadata/issues
 Project-URL: Source, https://github.com/ImageMarkup/isic-metadata
 Keywords: requests
```

### Comparing `isic-metadata-0.0.7/pyproject.toml` & `isic-metadata-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `isic-metadata-0.0.7/setup.py` & `isic-metadata-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `isic-metadata-0.0.7/tests/test_fields.py` & `isic-metadata-0.0.8/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `isic-metadata-0.0.7/tests/test_utils.py` & `isic-metadata-0.0.8/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `isic-metadata-0.0.7/tox.ini` & `isic-metadata-0.0.8/tox.ini`

 * *Files identical despite different names*

