# Comparing `tmp/bikeshare_model-1.0.0-py3-none-any.whl.zip` & `tmp/bikeshare_model-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,22 @@
-Zip file size: 306201 bytes, number of entries: 19
--rw-rw-r--  2.0 unx        5 b- defN 23-Jul-31 23:47 bikeshare_model/VERSION
+Zip file size: 3741865 bytes, number of entries: 20
+-rw-rw-r--  2.0 unx        5 b- defN 23-Aug-01 00:09 bikeshare_model/VERSION
 -rw-r--r--  2.0 unx      307 b- defN 23-Jun-21 08:52 bikeshare_model/__init__.py
 -rw-rw-r--  2.0 unx     1948 b- defN 23-May-25 02:27 bikeshare_model/config.yml
 -rw-r--r--  2.0 unx     2715 b- defN 23-Jun-21 08:52 bikeshare_model/pipeline.py
 -rw-r--r--  2.0 unx     1851 b- defN 23-Jul-05 18:41 bikeshare_model/predict.py
 -rw-r--r--  2.0 unx     1450 b- defN 23-Jun-21 08:52 bikeshare_model/train_pipeline.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-21 13:27 bikeshare_model/config/__init__.py
 -rw-r--r--  2.0 unx     2820 b- defN 23-Jun-21 08:53 bikeshare_model/config/core.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-21 13:27 bikeshare_model/datasets/__init__.py
 -rw-rw-r--  2.0 unx  1598454 b- defN 23-May-22 10:38 bikeshare_model/datasets/bike-rental-dataset.csv
 -rw-r--r--  2.0 unx        2 b- defN 23-May-21 13:27 bikeshare_model/processing/__init__.py
 -rw-r--r--  2.0 unx     2972 b- defN 23-Jun-21 08:53 bikeshare_model/processing/data_manager.py
 -rw-r--r--  2.0 unx     5280 b- defN 23-Jun-04 01:13 bikeshare_model/processing/features.py
 -rw-r--r--  2.0 unx     1403 b- defN 23-Jun-04 01:43 bikeshare_model/processing/validation.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-21 13:27 bikeshare_model/trained_models/__init__.py
--rw-r--r--  2.0 unx     1078 b- defN 23-Jul-31 23:53 bikeshare_model-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-31 23:53 bikeshare_model-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jul-31 23:53 bikeshare_model-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1682 b- defN 23-Jul-31 23:53 bikeshare_model-1.0.0.dist-info/RECORD
-19 files, 1622075 bytes uncompressed, 303395 bytes compressed:  81.3%
+-rw-r--r--  2.0 unx 12920234 b- defN 23-Aug-01 00:23 bikeshare_model/trained_models/bikeshare__model_output_v1.0.1.pkl
+-rw-r--r--  2.0 unx     1137 b- defN 23-Aug-01 00:28 bikeshare_model-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-01 00:28 bikeshare_model-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Aug-01 00:28 bikeshare_model-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1808 b- defN 23-Aug-01 00:28 bikeshare_model-1.0.1.dist-info/RECORD
+20 files, 14542494 bytes uncompressed, 3738853 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -39,20 +39,23 @@
 
 Filename: bikeshare_model/processing/validation.py
 Comment: 
 
 Filename: bikeshare_model/trained_models/__init__.py
 Comment: 
 
-Filename: bikeshare_model-1.0.0.dist-info/METADATA
+Filename: bikeshare_model/trained_models/bikeshare__model_output_v1.0.1.pkl
 Comment: 
 
-Filename: bikeshare_model-1.0.0.dist-info/WHEEL
+Filename: bikeshare_model-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: bikeshare_model-1.0.0.dist-info/top_level.txt
+Filename: bikeshare_model-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: bikeshare_model-1.0.0.dist-info/RECORD
+Filename: bikeshare_model-1.0.1.dist-info/top_level.txt
+Comment: 
+
+Filename: bikeshare_model-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bikeshare_model/VERSION

```diff
@@ -1 +1 @@
-1.0.0
+1.0.1
```

## Comparing `bikeshare_model-1.0.0.dist-info/METADATA` & `bikeshare_model-1.0.1.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: bikeshare-model
-Version: 1.0.0
+Version: 1.0.1
 Summary: Bikeshare dataset regression model package 
+Home-page: UNKNOWN
 Author: Ajay Kumar Singh
 Author-email: ajaytevatia@gmail.com
 License: BSD-3
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -20,9 +22,11 @@
 Requires-Dist: numpy (==1.24.0)
 Requires-Dist: pandas (==1.5.3)
 Requires-Dist: pydantic (==1.10.10)
 Requires-Dist: scikit-learn (==1.3.0)
 Requires-Dist: strictyaml (==1.6.2)
 Requires-Dist: ruamel.yaml (==0.17.32)
 Requires-Dist: joblib (==1.3.1)
+Requires-Dist: wheel
 
 Bikeshare dataset regression model package 
+
```

## Comparing `bikeshare_model-1.0.0.dist-info/RECORD` & `bikeshare_model-1.0.1.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-bikeshare_model/VERSION,sha256=klIfw8vZZL3J9YSpkbif3apXVO0cyW1tQkRTOGacEwU,5
+bikeshare_model/VERSION,sha256=1R5uyUBYVUqEVYpbQC7m71_fVFXjXJAv7aYc2odSlDo,5
 bikeshare_model/__init__.py,sha256=JgyMhOr15b4vkuO7b3ik4h467eYl4CP_NlLAM88vs_8,307
 bikeshare_model/config.yml,sha256=fd42grpC0KZp5XKfmxyaSV6NkuU9I3F_0uqUsnBLAGw,1948
 bikeshare_model/pipeline.py,sha256=7Mg7hswgR0Z5c3XDoQu_0auZF4gi-NnJ9G19HEqByKI,2715
 bikeshare_model/predict.py,sha256=KuLoOJ9p_iSNjZ8WhGbthOr01lUEV24frCni1gGDNiw,1851
 bikeshare_model/train_pipeline.py,sha256=HGiB1rpKwiC40xkw__STaKGVrUAPP7wdY-OkF3Q9nhI,1450
 bikeshare_model/config/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 bikeshare_model/config/core.py,sha256=1j-SYM_P_5ng4ZoP0EAwgrqCGir1uPCGJiREtml92ag,2820
 bikeshare_model/datasets/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 bikeshare_model/datasets/bike-rental-dataset.csv,sha256=NyQ2F3BOHwh6JMkESfZL5hIrnecqwNFWQf4_uihALx4,1598454
 bikeshare_model/processing/__init__.py,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
 bikeshare_model/processing/data_manager.py,sha256=PzAoNxgYMFnk6D0OHfJGgodpGFzu6PHA4OezEKJXFZM,2972
 bikeshare_model/processing/features.py,sha256=rSTDgQxiwN_ssXjbA0p5o_6yVPq4-wz7NlwgAdEwFuA,5280
 bikeshare_model/processing/validation.py,sha256=ZYSk-v7OAZqMxhsNU6slsA5m412ZatDwSBjDRDio50I,1403
 bikeshare_model/trained_models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-bikeshare_model-1.0.0.dist-info/METADATA,sha256=YrdpFYDmdXclbDbApdn8i-oZriHcK0Pt8XSVkmvasbg,1078
-bikeshare_model-1.0.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-bikeshare_model-1.0.0.dist-info/top_level.txt,sha256=ZKIHSbGTS6ZE2aLhfpCV8HFAqGuZmXzRWQVz-N03wPI,16
-bikeshare_model-1.0.0.dist-info/RECORD,,
+bikeshare_model/trained_models/bikeshare__model_output_v1.0.1.pkl,sha256=sZ0qTjugrMbnc7zLHu5zjrLCs0p1rweCG8dhArSSQ8Q,12920234
+bikeshare_model-1.0.1.dist-info/METADATA,sha256=4eaKFMZeVOnIVCDCDhAn1H8M2jXS69pS6N6A5yF8Aw4,1137
+bikeshare_model-1.0.1.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+bikeshare_model-1.0.1.dist-info/top_level.txt,sha256=ZKIHSbGTS6ZE2aLhfpCV8HFAqGuZmXzRWQVz-N03wPI,16
+bikeshare_model-1.0.1.dist-info/RECORD,,
```

