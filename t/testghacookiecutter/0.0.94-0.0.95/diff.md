# Comparing `tmp/testghacookiecutter-0.0.94-cp39-cp39-win_amd64.whl.zip` & `tmp/testghacookiecutter-0.0.95-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 55909 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat      253 b- defN 23-Jul-01 05:25 testghacookiecutter/__init__.py
--rw-rw-rw-  2.0 fat   104960 b- defN 23-Jul-01 05:25 testghacookiecutter/_testghacookiecutter.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      454 b- defN 23-Jul-01 05:19 testghacookiecutter/include/test-gha-cookiecutter/test-gha-cookiecutter.hpp
--rw-rw-rw-  2.0 fat     4273 b- defN 23-Jul-01 05:25 testghacookiecutter/lib/cmake/test-gha-cookiecutter/test-gha-cookiecutter-config.cmake
--rw-rw-rw-  2.0 fat      128 b- defN 23-Jul-01 05:25 testghacookiecutter-0.0.94.dist-info/COPYING.md
--rw-rw-rw-  2.0 fat     1093 b- defN 23-Jul-01 05:25 testghacookiecutter-0.0.94.dist-info/LICENSE.md
--rw-rw-rw-  2.0 fat     3595 b- defN 23-Jul-01 05:25 testghacookiecutter-0.0.94.dist-info/METADATA
--rw-rw-rw-  2.0 fat       94 b- defN 23-Jul-01 05:25 testghacookiecutter-0.0.94.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 23-Jul-01 05:25 testghacookiecutter-0.0.94.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1036 b- defN 23-Jul-01 05:25 testghacookiecutter-0.0.94.dist-info/RECORD
-10 files, 115906 bytes uncompressed, 54077 bytes compressed:  53.3%
+Zip file size: 55936 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat      253 b- defN 23-Aug-01 05:24 testghacookiecutter/__init__.py
+-rw-rw-rw-  2.0 fat   104960 b- defN 23-Aug-01 05:24 testghacookiecutter/_testghacookiecutter.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      454 b- defN 23-Aug-01 05:16 testghacookiecutter/include/test-gha-cookiecutter/test-gha-cookiecutter.hpp
+-rw-rw-rw-  2.0 fat     4273 b- defN 23-Aug-01 05:24 testghacookiecutter/lib/cmake/test-gha-cookiecutter/test-gha-cookiecutter-config.cmake
+-rw-rw-rw-  2.0 fat      128 b- defN 23-Aug-01 05:24 testghacookiecutter-0.0.95.dist-info/COPYING.md
+-rw-rw-rw-  2.0 fat     1093 b- defN 23-Aug-01 05:24 testghacookiecutter-0.0.95.dist-info/LICENSE.md
+-rw-rw-rw-  2.0 fat     3595 b- defN 23-Aug-01 05:24 testghacookiecutter-0.0.95.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       94 b- defN 23-Aug-01 05:24 testghacookiecutter-0.0.95.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 23-Aug-01 05:24 testghacookiecutter-0.0.95.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1036 b- defN 23-Aug-01 05:24 testghacookiecutter-0.0.95.dist-info/RECORD
+10 files, 115906 bytes uncompressed, 54104 bytes compressed:  53.3%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: testghacookiecutter/include/test-gha-cookiecutter/test-gha-cookiecutter.hpp
 Comment: 
 
 Filename: testghacookiecutter/lib/cmake/test-gha-cookiecutter/test-gha-cookiecutter-config.cmake
 Comment: 
 
-Filename: testghacookiecutter-0.0.94.dist-info/COPYING.md
+Filename: testghacookiecutter-0.0.95.dist-info/COPYING.md
 Comment: 
 
-Filename: testghacookiecutter-0.0.94.dist-info/LICENSE.md
+Filename: testghacookiecutter-0.0.95.dist-info/LICENSE.md
 Comment: 
 
-Filename: testghacookiecutter-0.0.94.dist-info/METADATA
+Filename: testghacookiecutter-0.0.95.dist-info/METADATA
 Comment: 
 
-Filename: testghacookiecutter-0.0.94.dist-info/WHEEL
+Filename: testghacookiecutter-0.0.95.dist-info/WHEEL
 Comment: 
 
-Filename: testghacookiecutter-0.0.94.dist-info/top_level.txt
+Filename: testghacookiecutter-0.0.95.dist-info/top_level.txt
 Comment: 
 
-Filename: testghacookiecutter-0.0.94.dist-info/RECORD
+Filename: testghacookiecutter-0.0.95.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## testghacookiecutter/lib/cmake/test-gha-cookiecutter/test-gha-cookiecutter-config.cmake

```diff
@@ -3,15 +3,15 @@
 if("${CMAKE_MAJOR_VERSION}.${CMAKE_MINOR_VERSION}" LESS 2.8)
    message(FATAL_ERROR "CMake >= 2.8.0 required")
 endif()
 if(CMAKE_VERSION VERSION_LESS "2.8.3")
    message(FATAL_ERROR "CMake >= 2.8.3 required")
 endif()
 cmake_policy(PUSH)
-cmake_policy(VERSION 2.8.3...3.24)
+cmake_policy(VERSION 2.8.3...3.25)
 #----------------------------------------------------------------
 # Generated CMake target import file.
 #----------------------------------------------------------------
 
 # Commands may need to know the format version.
 set(CMAKE_IMPORT_FILE_VERSION 1)
```

## Comparing `testghacookiecutter-0.0.94.dist-info/LICENSE.md` & `testghacookiecutter-0.0.95.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `testghacookiecutter-0.0.94.dist-info/METADATA` & `testghacookiecutter-0.0.95.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testghacookiecutter
-Version: 0.0.94
+Version: 0.0.95
 Summary: Add short description here
 Maintainer-email: Your Name <your@email.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
```

## Comparing `testghacookiecutter-0.0.94.dist-info/RECORD` & `testghacookiecutter-0.0.95.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 testghacookiecutter/__init__.py,sha256=OBqOctWq6djKLdCiXn_w9DPt5OUOfcnNV8bkboqyMCc,253
-testghacookiecutter/_testghacookiecutter.cp39-win_amd64.pyd,sha256=scy5g1L5vWTzBbDu_QLuXF9eKQSiRr5aVePvKZagg9U,104960
+testghacookiecutter/_testghacookiecutter.cp39-win_amd64.pyd,sha256=_mfRuXMB46GQGUnq4UdXgZ5w1jfFS9SOgBDtKwpzVvU,104960
 testghacookiecutter/include/test-gha-cookiecutter/test-gha-cookiecutter.hpp,sha256=xJI_XphGsAx1roIMsv5L-qTyHbEK2dK_kT_Ug88g0Kw,454
-testghacookiecutter/lib/cmake/test-gha-cookiecutter/test-gha-cookiecutter-config.cmake,sha256=7aiMkCIs-xUO-UL6foxEcgw7j64Lt9lw0dZPuoUSD4c,4273
-testghacookiecutter-0.0.94.dist-info/COPYING.md,sha256=JlKk83B_EtSemfyGM4n5PXcYasvk8X1srTz_VdkJDJ0,128
-testghacookiecutter-0.0.94.dist-info/LICENSE.md,sha256=scwZm1ncOOBqsAmrBbQz-jOpx5yJvouik7Q7sMdjlSg,1093
-testghacookiecutter-0.0.94.dist-info/METADATA,sha256=Q-K15h1idQ0FRflv7CWkjigHy2RjOyryDruR9MYlW80,3595
-testghacookiecutter-0.0.94.dist-info/WHEEL,sha256=aFh_uQusBybh-RCXOkSlg-ycdQBtqU_JDPyXfjBBBgs,94
-testghacookiecutter-0.0.94.dist-info/top_level.txt,sha256=IswgbSrIopzF6Lm7sluyuTfnHzFtW7dBRGigD5EsE00,20
-testghacookiecutter-0.0.94.dist-info/RECORD,,
+testghacookiecutter/lib/cmake/test-gha-cookiecutter/test-gha-cookiecutter-config.cmake,sha256=LqOJp-7TYM2wm1pmX2bdrrN33DU7uoSw40u-Dyeny4I,4273
+testghacookiecutter-0.0.95.dist-info/COPYING.md,sha256=JlKk83B_EtSemfyGM4n5PXcYasvk8X1srTz_VdkJDJ0,128
+testghacookiecutter-0.0.95.dist-info/LICENSE.md,sha256=scwZm1ncOOBqsAmrBbQz-jOpx5yJvouik7Q7sMdjlSg,1093
+testghacookiecutter-0.0.95.dist-info/METADATA,sha256=e-LAXhceh88PR6GENa7ldM_Edz49edZiiftE_O0SfIY,3595
+testghacookiecutter-0.0.95.dist-info/WHEEL,sha256=aFh_uQusBybh-RCXOkSlg-ycdQBtqU_JDPyXfjBBBgs,94
+testghacookiecutter-0.0.95.dist-info/top_level.txt,sha256=IswgbSrIopzF6Lm7sluyuTfnHzFtW7dBRGigD5EsE00,20
+testghacookiecutter-0.0.95.dist-info/RECORD,,
```

