# Comparing `tmp/mrgrain.cdk-esbuild-4.2.0.tar.gz` & `tmp/mrgrain.cdk-esbuild-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrgrain.cdk-esbuild-4.2.0.tar", last modified: Wed Jul 26 23:52:47 2023, max compression
+gzip compressed data, was "mrgrain.cdk-esbuild-4.2.1.tar", last modified: Tue Aug  1 05:05:11 2023, max compression
```

## Comparing `mrgrain.cdk-esbuild-4.2.0.tar` & `mrgrain.cdk-esbuild-4.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:52:47.230481 mrgrain.cdk-esbuild-4.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-26 23:52:34.000000 mrgrain.cdk-esbuild-4.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-26 23:52:34.000000 mrgrain.cdk-esbuild-4.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19637 2023-07-26 23:52:47.230481 mrgrain.cdk-esbuild-4.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18679 2023-07-26 23:52:34.000000 mrgrain.cdk-esbuild-4.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-26 23:52:34.000000 mrgrain.cdk-esbuild-4.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 23:52:47.230481 mrgrain.cdk-esbuild-4.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-26 23:52:34.000000 mrgrain.cdk-esbuild-4.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:52:47.226481 mrgrain.cdk-esbuild-4.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:52:47.226481 mrgrain.cdk-esbuild-4.2.0/src/mrgrain/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:52:47.230481 mrgrain.cdk-esbuild-4.2.0/src/mrgrain/cdk_esbuild/
--rw-r--r--   0 runner    (1001) docker     (123)   411762 2023-07-26 23:52:34.000000 mrgrain.cdk-esbuild-4.2.0/src/mrgrain/cdk_esbuild/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:52:47.230481 mrgrain.cdk-esbuild-4.2.0/src/mrgrain/cdk_esbuild/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-26 23:52:34.000000 mrgrain.cdk-esbuild-4.2.0/src/mrgrain/cdk_esbuild/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    82716 2023-07-26 23:52:34.000000 mrgrain.cdk-esbuild-4.2.0/src/mrgrain/cdk_esbuild/_jsii/cdk-esbuild@4.2.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 23:52:34.000000 mrgrain.cdk-esbuild-4.2.0/src/mrgrain/cdk_esbuild/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:52:47.226481 mrgrain.cdk-esbuild-4.2.0/src/mrgrain.cdk_esbuild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19637 2023-07-26 23:52:47.000000 mrgrain.cdk-esbuild-4.2.0/src/mrgrain.cdk_esbuild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-26 23:52:47.000000 mrgrain.cdk-esbuild-4.2.0/src/mrgrain.cdk_esbuild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 23:52:47.000000 mrgrain.cdk-esbuild-4.2.0/src/mrgrain.cdk_esbuild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-26 23:52:47.000000 mrgrain.cdk-esbuild-4.2.0/src/mrgrain.cdk_esbuild.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-26 23:52:47.000000 mrgrain.cdk-esbuild-4.2.0/src/mrgrain.cdk_esbuild.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:05:11.403932 mrgrain.cdk-esbuild-4.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-01 05:04:59.000000 mrgrain.cdk-esbuild-4.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 05:04:59.000000 mrgrain.cdk-esbuild-4.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19637 2023-08-01 05:05:11.403932 mrgrain.cdk-esbuild-4.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18679 2023-08-01 05:04:59.000000 mrgrain.cdk-esbuild-4.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-01 05:04:59.000000 mrgrain.cdk-esbuild-4.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 05:05:11.403932 mrgrain.cdk-esbuild-4.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-08-01 05:04:59.000000 mrgrain.cdk-esbuild-4.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:05:11.403932 mrgrain.cdk-esbuild-4.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:05:11.403932 mrgrain.cdk-esbuild-4.2.1/src/mrgrain/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:05:11.403932 mrgrain.cdk-esbuild-4.2.1/src/mrgrain/cdk_esbuild/
+-rw-r--r--   0 runner    (1001) docker     (123)   411762 2023-08-01 05:04:59.000000 mrgrain.cdk-esbuild-4.2.1/src/mrgrain/cdk_esbuild/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:05:11.403932 mrgrain.cdk-esbuild-4.2.1/src/mrgrain/cdk_esbuild/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-01 05:04:59.000000 mrgrain.cdk-esbuild-4.2.1/src/mrgrain/cdk_esbuild/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82718 2023-08-01 05:04:59.000000 mrgrain.cdk-esbuild-4.2.1/src/mrgrain/cdk_esbuild/_jsii/cdk-esbuild@4.2.1.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 05:04:59.000000 mrgrain.cdk-esbuild-4.2.1/src/mrgrain/cdk_esbuild/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:05:11.403932 mrgrain.cdk-esbuild-4.2.1/src/mrgrain.cdk_esbuild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19637 2023-08-01 05:05:11.000000 mrgrain.cdk-esbuild-4.2.1/src/mrgrain.cdk_esbuild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-08-01 05:05:11.000000 mrgrain.cdk-esbuild-4.2.1/src/mrgrain.cdk_esbuild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 05:05:11.000000 mrgrain.cdk-esbuild-4.2.1/src/mrgrain.cdk_esbuild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-01 05:05:11.000000 mrgrain.cdk-esbuild-4.2.1/src/mrgrain.cdk_esbuild.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 05:05:11.000000 mrgrain.cdk-esbuild-4.2.1/src/mrgrain.cdk_esbuild.egg-info/top_level.txt
```

### Comparing `mrgrain.cdk-esbuild-4.2.0/LICENSE` & `mrgrain.cdk-esbuild-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mrgrain.cdk-esbuild-4.2.0/PKG-INFO` & `mrgrain.cdk-esbuild-4.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrgrain.cdk-esbuild
-Version: 4.2.0
+Version: 4.2.1
 Summary: CDK constructs for esbuild, an extremely fast JavaScript bundler
 Home-page: https://github.com/mrgrain/cdk-esbuild
 Author: Moritz Kornher<mail@moritzkornher.de>
 License: MIT
 Project-URL: Source, https://github.com/mrgrain/cdk-esbuild
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `mrgrain.cdk-esbuild-4.2.0/README.md` & `mrgrain.cdk-esbuild-4.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mrgrain.cdk-esbuild-4.2.0/setup.py` & `mrgrain.cdk-esbuild-4.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "mrgrain.cdk-esbuild",
-    "version": "4.2.0",
+    "version": "4.2.1",
     "description": "CDK constructs for esbuild, an extremely fast JavaScript bundler",
     "license": "MIT",
     "url": "https://github.com/mrgrain/cdk-esbuild",
     "long_description_content_type": "text/markdown",
     "author": "Moritz Kornher<mail@moritzkornher.de>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "mrgrain.cdk_esbuild",
         "mrgrain.cdk_esbuild._jsii"
     ],
     "package_data": {
         "mrgrain.cdk_esbuild._jsii": [
-            "cdk-esbuild@4.2.0.jsii.tgz"
+            "cdk-esbuild@4.2.1.jsii.tgz"
         ],
         "mrgrain.cdk_esbuild": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `mrgrain.cdk-esbuild-4.2.0/src/mrgrain/cdk_esbuild/__init__.py` & `mrgrain.cdk-esbuild-4.2.1/src/mrgrain/cdk_esbuild/__init__.py`

 * *Files identical despite different names*

### Comparing `mrgrain.cdk-esbuild-4.2.0/src/mrgrain/cdk_esbuild/_jsii/cdk-esbuild@4.2.0.jsii.tgz` & `mrgrain.cdk-esbuild-4.2.1/src/mrgrain/cdk_esbuild/_jsii/cdk-esbuild@4.2.1.jsii.tgz`

 * *Files 26% similar despite different names*

#### Comparing `cdk-esbuild@4.2.0.jsii.tgz-content` & `cdk-esbuild@4.2.1.jsii.tgz-content`

##### package/.jsii

###### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'fingerprint'": "'9JhWk6ogoHLEAegIf8ctPB0NYktgUv89QIV9DVFKoV4='", "'version'": "'4.2.1'"}*

```diff
@@ -2915,15 +2915,15 @@
             }
         }
     },
     "description": "CDK constructs for esbuild, an extremely fast JavaScript bundler",
     "docs": {
         "stability": "stable"
     },
-    "fingerprint": "e1/txMLZnofT5l/mmAWHfcTB3nhQrekjiUHbhZ/TaUc=",
+    "fingerprint": "9JhWk6ogoHLEAegIf8ctPB0NYktgUv89QIV9DVFKoV4=",
     "homepage": "https://github.com/mrgrain/cdk-esbuild",
     "jsiiVersion": "1.85.0 (build 08ee592)",
     "keywords": [
         "aws-cdk",
         "bundler",
         "cdk",
         "constructs",
@@ -7533,9 +7533,9 @@
                         "primitive": "string"
                     }
                 }
             ],
             "symbolId": "src/source:TypeScriptSourceProps"
         }
     },
-    "version": "4.2.0"
+    "version": "4.2.1"
 }
```

##### package/lib/asset.js

###### js-beautify {}

```diff
@@ -59,38 +59,38 @@
         });
     }
 }
 exports.EsbuildAsset = EsbuildAsset;
 _a = JSII_RTTI_SYMBOL_1;
 EsbuildAsset[_a] = {
     fqn: "@mrgrain/cdk-esbuild.EsbuildAsset",
-    version: "4.2.0"
+    version: "4.2.1"
 };
 /**
  * Bundles the entry points and creates a CDK asset which is uploaded to the bootstrapped CDK S3 bucket during deployment.
  *
  * The asset can be used by other constructs.
  *
  * @stability stable
  */
 class JavaScriptAsset extends EsbuildAsset {}
 exports.JavaScriptAsset = JavaScriptAsset;
 _b = JSII_RTTI_SYMBOL_1;
 JavaScriptAsset[_b] = {
     fqn: "@mrgrain/cdk-esbuild.JavaScriptAsset",
-    version: "4.2.0"
+    version: "4.2.1"
 };
 /**
  * Bundles the entry points and creates a CDK asset which is uploaded to the bootstrapped CDK S3 bucket during deployment.
  *
  * The asset can be used by other constructs.
  *
  * @stability stable
  */
 class TypeScriptAsset extends EsbuildAsset {}
 exports.TypeScriptAsset = TypeScriptAsset;
 _c = JSII_RTTI_SYMBOL_1;
 TypeScriptAsset[_c] = {
     fqn: "@mrgrain/cdk-esbuild.TypeScriptAsset",
-    version: "4.2.0"
+    version: "4.2.1"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiYXNzZXQuanMiLCJzb3VyY2VSb290IjoiIiwic291cmNlcyI6WyIuLi9zcmMvYXNzZXQudHMiXSwibmFtZXMiOltdLCJtYXBwaW5ncyI6Ijs7Ozs7QUFBQSwrQkFBNEM7QUFDNUMsNkNBQTRDO0FBQzVDLDZEQUE2RDtBQUM3RCwyQ0FBNkM7QUFDN0MsdUNBQXNFO0FBeUN0RTs7Ozs7O0dBTUc7QUFDSCxNQUFhLFlBQXVDLFNBQVEscUJBQU87SUFDakU7O09BRUc7SUFDSCxZQUNFLEtBQWdCLEVBQ2hCLEVBQVUsRUFDVixLQUFZO1FBRVosTUFBTSxFQUNKLFNBQVMsRUFDVCxZQUFZLEVBQUUsT0FBTyxHQUFHLEVBQUUsR0FDM0IsR0FBRyxLQUFLLENBQUM7UUFDVixNQUFNLFdBQVcsR0FDZixPQUFPLEtBQUssQ0FBQyxXQUFXLEtBQUssUUFBUSxDQUFDLENBQUMsQ0FBQyxDQUFDLEtBQUssQ0FBQyxXQUFXLENBQUMsQ0FBQyxDQUFDLENBQUMsS0FBSyxDQUFDLFdBQVcsQ0FBQztRQUVsRixNQUFNLElBQUksR0FBRyxLQUFLLENBQUMsSUFBSSxDQUFDLElBQUksR0FBRyxpQkFBSSxDQUFDLFFBQVEsR0FBRyxFQUFFLENBQUM7UUFFbEQsTUFBTSxhQUFhLEdBQUcsT0FBTyxDQUFDLGFBQWEsSUFBSSxPQUFPLENBQUMsR0FBRyxFQUFFLENBQUM7UUFFN0QsTUFBTSwyQkFBMkIsR0FBRyxDQUFDLFVBQWtCLEVBQVUsRUFBRTtZQUNqRSxJQUFJLENBQUMsaUJBQVUsQ0FBQyxVQUFVLENBQUMsRUFBRTtnQkFDM0IsT0FBTyxVQUFVLENBQUM7YUFDbkI7WUFFRCxNQUFNLGtCQUFrQixHQUFHLGVBQVEsQ0FBQyxhQUFhLEVBQUUsVUFBVSxDQUFDLENBQUM7WUFDL0QsSUFBSSxrQkFBa0IsQ0FBQyxVQUFVLENBQUMsSUFBSSxDQUFDLElBQUksaUJBQVUsQ0FBQyxrQkFBa0IsQ0FBQyxFQUFFO2dCQUN6RSxNQUFNLElBQUksS0FBSyxDQUNiLEdBQUcsSUFBSSxtSkFBbUosQ0FDM0osQ0FBQzthQUNIO1lBRUQsT0FBTyxrQkFBa0IsQ0FBQztRQUM1QixDQUFDLENBQUM7UUFFRixNQUFNLG1CQUFtQixHQUN2QixLQUFLLENBQUMsT0FBTyxDQUFDLFdBQVcsQ0FBQyxDQUFDLENBQUM7WUFDMUIsV0FBVyxDQUFDLEdBQUcsQ0FBQywyQkFBMkIsQ0FBQyxDQUFDLENBQUM7WUFDOUMsTUFBTSxDQUFDLFdBQVcsQ0FDaEIsTUFBTSxDQUFDLE9BQU8sQ0FBQyxXQUFXLENBQUM7aUJBQ3hCLEdBQUcsQ0FBQyxDQUFDLENBQUMsR0FBRyxFQUFFLFVBQVUsQ0FBQyxFQUFFLEVBQUUsQ0FBQyxDQUFDLENBQUMsR0FBRyxFQUFFLDJCQUEyQixDQUFDLFVBQVUsQ0FBQyxDQUFDLENBQUMsQ0FDM0UsQ0FDSixDQUFDO1FBR04sTUFBTSxZQUFZLEdBQUc7WUFDbkIsTUFBTSxFQUFFLElBQUk7WUFDWixHQUFHLE9BQU87WUFDVixhQUFhO1NBQ2QsQ0FBQztRQUVGLEtBQUssQ0FBQyxLQUFLLEVBQUUsRUFBRSxFQUFFO1lBQ2YsSUFBSSxFQUFFLGFBQWE7WUFDbkIsU0FBUztZQUNULGFBQWEsRUFBRSxTQUFTLENBQUMsQ0FBQyxDQUFDLDJCQUFhLENBQUMsTUFBTSxDQUFDLENBQUMsQ0FBQywyQkFBYSxDQUFDLE1BQU07WUFDdEUsUUFBUSxFQUFFLElBQUksd0JBQWMsQ0FDMUIsbUJBQW1CLEVBQ25CO2dCQUNFLEdBQUcsS0FBSztnQkFDUixZQUFZO2FBQ2IsQ0FDRjtTQUNGLENBQUMsQ0FBQztJQUNMLENBQUM7O0FBL0RILG9DQWdFQzs7O0FBRUQ7Ozs7OztHQU1HO0FBQ0gsTUFBYSxlQUFnQixTQUFRLFlBQWtDOztBQUF2RSwwQ0FBMEU7OztBQUUxRTs7Ozs7O0dBTUc7QUFDSCxNQUFhLGVBQWdCLFNBQVEsWUFBa0M7O0FBQXZFLDBDQUEwRSIsInNvdXJjZXNDb250ZW50IjpbImltcG9ydCB7IGlzQWJzb2x1dGUsIHJlbGF0aXZlIH0gZnJvbSAncGF0aCc7XG5pbXBvcnQgeyBBc3NldEhhc2hUeXBlIH0gZnJvbSAnYXdzLWNkay1saWInO1xuaW1wb3J0IHsgQXNzZXQgYXMgUzNBc3NldCB9IGZyb20gJ2F3cy1jZGstbGliL2F3cy1zMy1hc3NldHMnO1xuaW1wb3J0IHsgQ29uc3RydWN0LCBOb2RlIH0gZnJvbSAnY29uc3RydWN0cyc7XG5pbXBvcnQgeyBFc2J1aWxkQnVuZGxlciwgQnVuZGxlclByb3BzLCBFbnRyeVBvaW50cyB9IGZyb20gJy4vYnVuZGxlcic7XG5cbi8qKlxuICogQGludGVybmFsXG4gKi9cbmV4cG9ydCBpbnRlcmZhY2UgQXNzZXRCYXNlUHJvcHMgZXh0ZW5kcyBCdW5kbGVyUHJvcHMge1xuICAvKipcbiAgICogQSBoYXNoIG9mIHRoaXMgYXNzZXQsIHdoaWNoIGlzIGF2YWlsYWJsZSBhdCBjb25zdHJ1Y3Rpb24gdGltZS5cbiAgICpcbiAgICogQXMgdGhpcyBpcyBhIHBsYWluIHN0cmluZywgaXQgY2FuIGJlIHVzZWQgaW4gY29uc3RydWN0IElEcyBpbiBvcmRlciB0byBlbmZvcmNlIGNyZWF0aW9uIG9mIGEgbmV3IHJlc291cmNlIHdoZW4gdGhlIGNvbnRlbnQgaGFzaCBoYXMgY2hhbmdlZC5cbiAgICpcbiAgICogRGVmYXVsdHMgdG8gYSBoYXNoIG9mIGFsbCBmaWxlcyBpbiB0aGUgcmVzdWx0aW5nIGJ1bmRsZS5cbiAgICpcbiAgICogQHN0YWJpbGl0eSBzdGFibGVcbiAgICovXG4gIHJlYWRvbmx5IGFzc2V0SGFzaD86IHN0cmluZztcbn1cblxuZXhwb3J0IGludGVyZmFjZSBBc3NldFByb3BzIGV4dGVuZHMgQXNzZXRCYXNlUHJvcHMge1xuICAvKipcbiAgICogQSBwYXRoIG9yIGxpc3Qgb3IgbWFwIG9mIHBhdGhzIHRvIHRoZSBlbnRyeSBwb2ludHMgb2YgeW91ciBjb2RlLlxuICAgKlxuICAgKiBSZWxhdGl2ZSBwYXRocyBhcmUgYnkgZGVmYXVsdCByZXNvbHZlZCBmcm9tIHRoZSBjdXJyZW50IHdvcmtpbmcgZGlyZWN0b3J5LlxuICAgKiBUbyBjaGFuZ2UgdGhlIHdvcmtpbmcgZGlyZWN0b3J5LCBzZWUgYGJ1aWxkT3B0aW9ucy5hYnNXb3JraW5nRGlyYC5cbiAgICpcbiAgICogQWJzb2x1dGUgcGF0aHMgY2FuIGJlIHVzZWQgaWYgZmlsZXMgYXJlIHBhcnQgb2YgdGhlIHdvcmtpbmcgZGlyZWN0b3J5LlxuICAgKlxuICAgKiBFeGFtcGxlczpcbiAgICogIC0gYCdzcmMvaW5kZXgudHMnYFxuICAgKiAgLSBgcmVxdWlyZS5yZXNvbHZlKCcuL2xhbWJkYScpYFxuICAgKiAgLSBgWydzcmMvaW5kZXgudHMnLCAnc3JjL3V0aWwudHMnXWBcbiAgICogIC0gYHtvbmU6ICdzcmMvdHdvLnRzJywgdHdvOiAnc3JjL29uZS50cyd9YFxuICAgKlxuICAgKiBAc3RhYmlsaXR5IHN0YWJsZVxuICAgKi9cbiAgcmVhZG9ubHkgZW50cnlQb2ludHM6IEVudHJ5UG9pbnRzO1xufVxuXG50eXBlIEphdmFTY3JpcHRBc3NldFByb3BzID0gQXNzZXRQcm9wcztcbnR5cGUgVHlwZVNjcmlwdEFzc2V0UHJvcHMgPSBBc3NldFByb3BzO1xuXG4vKipcbiAqIFJlcHJlc2VudHMgYSBnZW5lcmljIGVzYnVpbGQgYXNzZXQuXG4gKlxuICogWW91IHNob3VsZCBhbHdheXMgdXNlIGBUeXBlU2NyaXB0QXNzZXRgIG9yIGBKYXZhU2NyaXB0QXNzZXRgLlxuICpcbiAqIEBzdGFiaWxpdHkgZXhwZXJpbWVudGFsXG4gKi9cbmV4cG9ydCBjbGFzcyBFc2J1aWxkQXNzZXQ8UHJvcHMgZXh0ZW5kcyBBc3NldFByb3BzPiBleHRlbmRzIFMzQXNzZXQge1xuICAvKipcbiAgICogQHN0YWJpbGl0eSBzdGFibGVcbiAgICovXG4gIHB1YmxpYyBjb25zdHJ1Y3RvcihcbiAgICBzY29wZTogQ29uc3RydWN0LFxuICAgIGlkOiBzdHJpbmcsXG4gICAgcHJvcHM6IFByb3BzLFxuICApIHtcbiAgICBjb25zdCB7XG4gICAgICBhc3NldEhhc2gsXG4gICAgICBidWlsZE9wdGlvbnM6IG9wdGlvbnMgPSB7fSxcbiAgICB9ID0gcHJvcHM7XG4gICAgY29uc3QgZW50cnlQb2ludHM6IHN0cmluZ1tdIHwgUmVjb3JkPHN0cmluZywgc3RyaW5nPiA9XG4gICAgICB0eXBlb2YgcHJvcHMuZW50cnlQb2ludHMgPT09ICdzdHJpbmcnID8gW3Byb3BzLmVudHJ5UG9pbnRzXSA6IHByb3BzLmVudHJ5UG9pbnRzO1xuXG4gICAgY29uc3QgbmFtZSA9IHNjb3BlLm5vZGUucGF0aCArIE5vZGUuUEFUSF9TRVAgKyBpZDtcblxuICAgIGNvbnN0IGFic1dvcmtpbmdEaXIgPSBvcHRpb25zLmFic1dvcmtpbmdEaXIgPz8gcHJvY2Vzcy5jd2QoKTtcblxuICAgIGNvbnN0IGZvcmNlUmVsYXRpdmVFbnRyeXBvaW50UGF0aCA9IChlbnRyeVBvaW50OiBzdHJpbmcpOiBzdHJpbmcgPT4ge1xuICAgICAgaWYgKCFpc0Fic29sdXRlKGVudHJ5UG9pbnQpKSB7XG4gICAgICAgIHJldHVybiBlbnRyeVBvaW50O1xuICAgICAgfVxuXG4gICAgICBjb25zdCByZWxhdGl2ZUVudHJ5UG9pbnQgPSByZWxhdGl2ZShhYnNXb3JraW5nRGlyLCBlbnRyeVBvaW50KTtcbiAgICAgIGlmIChyZWxhdGl2ZUVudHJ5UG9pbnQuc3RhcnRzV2l0aCgnLi4nKSB8fCBpc0Fic29sdXRlKHJlbGF0aXZlRW50cnlQb2ludCkpIHtcbiAgICAgICAgdGhyb3cgbmV3IEVycm9yKFxuICAgICAgICAgIGAke25hbWV9OiBFbnRyeSBwb2ludHMgbXVzdCBiZSBwYXJ0IG9mIHRoZSB3b3JraW5nIGRpcmVjdG9yeS4gU2VlIFxcYGJ1aWxkT3B0aW9ucy5hYnNXb3JraW5nRGlyXFxgIHRvIHNldCBhIHdvcmtpbmcgZGlyZWN0b3J5IGRpZmZlcmVudCB0byB0aGUgY3VycmVudCBvbmUuYCxcbiAgICAgICAgKTtcbiAgICAgIH1cblxuICAgICAgcmV0dXJuIHJlbGF0aXZlRW50cnlQb2ludDtcbiAgICB9O1xuXG4gICAgY29uc3QgcmVsYXRpdmVFbnRyeVBvaW50cyA9XG4gICAgICBBcnJheS5pc0FycmF5KGVudHJ5UG9pbnRzKSA/XG4gICAgICAgIGVudHJ5UG9pbnRzLm1hcChmb3JjZVJlbGF0aXZlRW50cnlwb2ludFBhdGgpIDpcbiAgICAgICAgT2JqZWN0LmZyb21FbnRyaWVzKFxuICAgICAgICAgIE9iamVjdC5lbnRyaWVzKGVudHJ5UG9pbnRzKVxuICAgICAgICAgICAgLm1hcCgoW291dCwgZW50cnlQb2ludF0pID0+IChbb3V0LCBmb3JjZVJlbGF0aXZlRW50cnlwb2ludFBhdGgoZW50cnlQb2ludCldKSxcbiAgICAgICAgICAgICksXG4gICAgICAgICk7XG5cblxuICAgIGNvbnN0IGJ1aWxkT3B0aW9ucyA9IHtcbiAgICAgIGJ1bmRsZTogdHJ1ZSxcbiAgICAgIC4uLm9wdGlvbnMsXG4gICAgICBhYnNXb3JraW5nRGlyLFxuICAgIH07XG5cbiAgICBzdXBlcihzY29wZSwgaWQsIHtcbiAgICAgIHBhdGg6IGFic1dvcmtpbmdEaXIsXG4gICAgICBhc3NldEhhc2gsXG4gICAgICBhc3NldEhhc2hUeXBlOiBhc3NldEhhc2ggPyBBc3NldEhhc2hUeXBlLkNVU1RPTSA6IEFzc2V0SGFzaFR5cGUuT1VUUFVULFxuICAgICAgYnVuZGxpbmc6IG5ldyBFc2J1aWxkQnVuZGxlcihcbiAgICAgICAgcmVsYXRpdmVFbnRyeVBvaW50cyxcbiAgICAgICAge1xuICAgICAgICAgIC4uLnByb3BzLFxuICAgICAgICAgIGJ1aWxkT3B0aW9ucyxcbiAgICAgICAgfSxcbiAgICAgICksXG4gICAgfSk7XG4gIH1cbn1cblxuLyoqXG4gKiBCdW5kbGVzIHRoZSBlbnRyeSBwb2ludHMgYW5kIGNyZWF0ZXMgYSBDREsgYXNzZXQgd2hpY2ggaXMgdXBsb2FkZWQgdG8gdGhlIGJvb3RzdHJhcHBlZCBDREsgUzMgYnVja2V0IGR1cmluZyBkZXBsb3ltZW50LlxuICpcbiAqIFRoZSBhc3NldCBjYW4gYmUgdXNlZCBieSBvdGhlciBjb25zdHJ1Y3RzLlxuICpcbiAqIEBzdGFiaWxpdHkgc3RhYmxlXG4gKi9cbmV4cG9ydCBjbGFzcyBKYXZhU2NyaXB0QXNzZXQgZXh0ZW5kcyBFc2J1aWxkQXNzZXQ8SmF2YVNjcmlwdEFzc2V0UHJvcHM+IHt9XG5cbi8qKlxuICogQnVuZGxlcyB0aGUgZW50cnkgcG9pbnRzIGFuZCBjcmVhdGVzIGEgQ0RLIGFzc2V0IHdoaWNoIGlzIHVwbG9hZGVkIHRvIHRoZSBib290c3RyYXBwZWQgQ0RLIFMzIGJ1Y2tldCBkdXJpbmcgZGVwbG95bWVudC5cbiAqXG4gKiBUaGUgYXNzZXQgY2FuIGJlIHVzZWQgYnkgb3RoZXIgY29uc3RydWN0cy5cbiAqXG4gKiBAc3RhYmlsaXR5IHN0YWJsZVxuICovXG5leHBvcnQgY2xhc3MgVHlwZVNjcmlwdEFzc2V0IGV4dGVuZHMgRXNidWlsZEFzc2V0PFR5cGVTY3JpcHRBc3NldFByb3BzPiB7fVxuIl19
```

##### package/lib/bundler.js

###### js-beautify {}

```diff
@@ -141,10 +141,10 @@
         };
     }
 }
 exports.EsbuildBundler = EsbuildBundler;
 _a = JSII_RTTI_SYMBOL_1;
 EsbuildBundler[_a] = {
     fqn: "@mrgrain/cdk-esbuild.EsbuildBundler",
-    version: "4.2.0"
+    version: "4.2.1"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiYnVuZGxlci5qcyIsInNvdXJjZVJvb3QiOiIiLCJzb3VyY2VzIjpbIi4uL3NyYy9idW5kbGVyLnRzIl0sIm5hbWVzIjpbXSwibWFwcGluZ3MiOiI7Ozs7O0FBQUEsMkJBQW1EO0FBQ25ELCtCQUE2RTtBQUM3RSw2Q0FLcUI7QUFFckIsMkNBQWlEO0FBQ2pELHlDQUE2RDtBQWdGN0Q7Ozs7O0dBS0c7QUFDSCxNQUFhLGNBQWM7SUFlekI7O09BRUc7SUFDSDtJQUNFOzs7Ozs7Ozs7Ozs7Ozs7T0FlRztJQUNhLFdBQXdCO0lBRXhDOzs7O09BSUc7SUFDYSxLQUFtQjtRQVBuQixnQkFBVyxHQUFYLFdBQVcsQ0FBYTtRQU94QixVQUFLLEdBQUwsS0FBSyxDQUFjO1FBbENyQzs7OztXQUlHO1FBQ2EsVUFBSyxHQUFHLHlCQUFXLENBQUMsWUFBWSxDQUFDLFNBQVMsQ0FBQyxDQUFDO1FBK0IxRCxJQUFJLEtBQUssRUFBRSxZQUFZLEVBQUUsT0FBTyxJQUFJLEtBQUssRUFBRSxZQUFZLEVBQUUsTUFBTSxFQUFFO1lBQy9ELE1BQU0sSUFBSSxLQUFLLENBQUMsd0NBQXdDLENBQUMsQ0FBQztTQUMzRDtRQUNELElBQUksQ0FBQyxLQUFLLEdBQUc7WUFDWCxTQUFTLEVBQUUsQ0FBQyxTQUFpQixFQUFFLFFBQXlCLEVBQVcsRUFBRTtnQkFFbkUsSUFBSSxJQUFJLENBQUMsS0FBSyxDQUFDLE9BQU8sRUFBRTtvQkFDdEIsTUFBTSxPQUFPLEdBQUcsSUFBSSxDQUFDLGNBQWMsQ0FBQyxJQUFJLENBQUMsS0FBSyxDQUFDLE9BQU8sQ0FBQyxDQUFDO29CQUV4RCxPQUFPLENBQUMsT0FBTyxDQUFDLENBQUMsQ0FBQyxJQUFJLEVBQUUsR0FBRyxDQUFDLEVBQUUsRUFBRTt3QkFDOUIsTUFBTSxNQUFNLEdBQUcsY0FBTyxDQUNwQixJQUFJLENBQUMsS0FBSyxFQUFFLFlBQVksRUFBRSxhQUFhLElBQUksT0FBTyxDQUFDLEdBQUcsRUFBRSxFQUN4RCxHQUFHLENBQ0osQ0FBQzt3QkFDRixNQUFNLE9BQU8sR0FBRyxjQUFPLENBQUMsU0FBUyxFQUFFLElBQUksQ0FBQyxDQUFDO3dCQUV6QyxNQUFNLFlBQVksR0FBRyxlQUFRLENBQUMsU0FBUyxFQUFFLE9BQU8sQ0FBQyxDQUFDO3dCQUNsRCxJQUFJLFlBQVksQ0FBQyxVQUFVLENBQUMsSUFBSSxDQUFDLElBQUksaUJBQVUsQ0FBQyxZQUFZLENBQUMsRUFBRTs0QkFDN0QsTUFBTSxJQUFJLEtBQUssQ0FBQyxvRkFBb0YsQ0FBQyxDQUFDO3lCQUN2Rzt3QkFFRCxJQUFJLGVBQVUsQ0FBQyxPQUFPLENBQUMsRUFBRTs0QkFDdkIsV0FBTSxDQUFDLE9BQU8sRUFBRSxFQUFFLFNBQVMsRUFBRSxJQUFJLEVBQUUsS0FBSyxFQUFFLElBQUksRUFBRSxDQUFDLENBQUM7eUJBQ25EO3dCQUNELGNBQVMsQ0FBQyxPQUFPLEVBQUUsRUFBRSxTQUFTLEVBQUUsSUFBSSxFQUFFLENBQUMsQ0FBQzt3QkFDeEMsd0JBQVUsQ0FBQyxhQUFhLENBQUMsTUFBTSxFQUFFLE9BQU8sQ0FBQyxDQUFDO29CQUM1QyxDQUFDLENBQUMsQ0FBQztpQkFDSjtnQkFFRCxJQUFJO29CQUNGLE1BQU0sUUFBUSxHQUFHLEtBQUssQ0FBQyxhQUFhLElBQUksMEJBQWUsQ0FBQyxvQkFBb0IsRUFBRSxDQUFDO29CQUUvRSxRQUFRLENBQUMsU0FBUyxDQUFDO3dCQUNqQixXQUFXLEVBQUUsT0FBTyxXQUFXLEtBQUssUUFBUSxDQUFDLENBQUMsQ0FBQyxDQUFDLFdBQVcsQ0FBQyxDQUFDLENBQUMsQ0FBQyxXQUFXO3dCQUMxRSxLQUFLLEVBQUUsT0FBTyxDQUFDLEdBQUcsQ0FBQyxRQUFRLENBQUMsQ0FBQyxDQUFDLE9BQU8sQ0FBQyxPQUFPLENBQUMsR0FBRyxDQUFDLFFBQVEsQ0FBQyxDQUFDLENBQUMsQ0FBQyxTQUFTO3dCQUN2RSxHQUFHLENBQUMsSUFBSSxDQUFDLEtBQUssRUFBRSxZQUFZLElBQUksRUFBRSxDQUFDO3dCQUNuQyxHQUFHLElBQUksQ0FBQyxnQkFBZ0IsQ0FBQyxTQUFTLEVBQUUsRUFBRSxTQUFTLEVBQVQsZ0JBQVMsRUFBRSxJQUFJLEVBQUosV0FBSSxFQUFFLENBQUM7cUJBQ3pELENBQUMsQ0FBQztpQkFDSjtnQkFBQyxPQUFPLEtBQUssRUFBRTtvQkFDZCxJQUFJLHNCQUFjLENBQUMsS0FBSyxDQUFDLEVBQUU7d0JBQ3pCLE1BQU0sSUFBSSxLQUFLLENBQUMsNEJBQTRCLFdBQVcsRUFBRSxDQUFDLENBQUM7cUJBQzVEO29CQUNELE1BQU0sS0FBSyxDQUFDO2lCQUNiO2dCQUVELE9BQU8sSUFBSSxDQUFDO1lBQ2QsQ0FBQztTQUNGLENBQUM7SUFDSixDQUFDO0lBRU8sY0FBYyxDQUFDLE9BQWdDO1FBQ3JELGtCQUFrQjtRQUNsQixJQUFJLENBQUMsT0FBTyxFQUFFO1lBQ1osT0FBTyxFQUFFLENBQUM7U0FDWDtRQUVELGtCQUFrQjtRQUNsQixJQUFJLEtBQUssQ0FBQyxPQUFPLENBQUMsT0FBTyxDQUFDLEVBQUU7WUFDMUIsT0FBTyxPQUFPLENBQUMsR0FBRyxDQUFDLENBQUMsR0FBVyxFQUFFLEVBQUUsQ0FBQyxDQUFDLEdBQUcsRUFBRSxHQUFHLENBQUMsQ0FBQyxDQUFDO1NBQ2pEO1FBRUQsUUFBUTtRQUNSLElBQ0UsT0FBTyxPQUFPLEtBQUssUUFBUTtZQUMzQixDQUFDLEtBQUssQ0FBQyxPQUFPLENBQUMsT0FBTyxDQUFDO1lBQ3ZCLE9BQU8sS0FBSyxJQUFJLEVBQ2hCO1lBQ0EsT0FBTyxNQUFNO2lCQUNWLE9BQU8sQ0FBQyxPQUFPLENBQUM7aUJBQ2hCLE9BQU8sQ0FBQyxDQUFDLENBQUMsSUFBSSxFQUFFLE9BQU8sQ0FBQyxFQUFFLEVBQUU7Z0JBQzNCLElBQUksS0FBSyxDQUFDLE9BQU8sQ0FBQyxPQUFPLENBQUMsRUFBRTtvQkFDMUIsT0FBTyxPQUFPLENBQUMsR0FBRyxDQUFDLENBQUMsR0FBRyxFQUFFLEVBQUUsQ0FBQyxDQUFDLElBQUksRUFBRSxHQUFHLENBQUMsQ0FBNEIsQ0FBQztpQkFDckU7Z0JBRUQsT0FBTyxDQUFDLENBQUMsSUFBSSxFQUFFLE9BQU8sQ0FBQyxDQUFDLENBQUM7WUFDM0IsQ0FBQyxDQUFDLENBQUM7U0FDTjtRQUVELGtCQUFrQjtRQUNsQixPQUFPLENBQUMsQ0FBQyxHQUFHLEVBQUUsT0FBaUIsQ0FBQyxDQUFDLENBQUM7SUFDcEMsQ0FBQztJQUVPLGdCQUFnQixDQUN0QixZQUFvQixFQUNwQixPQUFpRCxZQUFLO1FBRXRELElBQUksSUFBSSxDQUFDLEtBQUssRUFBRSxZQUFZLEVBQUUsT0FBTyxFQUFFO1lBQ3JDLE9BQU87Z0JBQ0wsTUFBTSxFQUFFLFNBQVM7Z0JBQ2pCLE9BQU8sRUFBRSxJQUFJLENBQUMsU0FBUyxDQUNyQixJQUFJLENBQUMsSUFBSSxDQUNQLEdBQUksQ0FBQyxZQUFZLEVBQUUsSUFBSSxDQUFDLEtBQUssRUFBRSxZQUFZLEVBQUUsT0FBTyxDQUFDLENBQUMsTUFBTSxDQUMxRCxPQUFPLENBQ0ssQ0FDZixDQUNGO2FBQ0YsQ0FBQztTQUNIO1FBRUQsT0FBTztZQUNMLE1BQU0sRUFBRSxJQUFJLENBQUMsU0FBUyxDQUNwQixJQUFJLENBQUMsSUFBSSxDQUNQLEdBQUksQ0FBQyxZQUFZLEVBQUUsSUFBSSxDQUFDLEtBQUssRUFBRSxZQUFZLEVBQUUsTUFBTSxDQUFDLENBQUMsTUFBTSxDQUN6RCxPQUFPLENBQ0ssQ0FDZixDQUNGO1lBQ0QsT0FBTyxFQUFFLFNBQVM7U0FDbkIsQ0FBQztJQUNKLENBQUM7O0FBekpILHdDQTBKQyIsInNvdXJjZXNDb250ZW50IjpbImltcG9ydCB7IGV4aXN0c1N5bmMsIG1rZGlyU3luYywgcm1TeW5jIH0gZnJvbSAnZnMnO1xuaW1wb3J0IHsgam9pbiwgbm9ybWFsaXplLCByZWxhdGl2ZSwgcmVzb2x2ZSwgcG9zaXgsIGlzQWJzb2x1dGUgfSBmcm9tICdwYXRoJztcbmltcG9ydCB7XG4gIEJ1bmRsaW5nT3B0aW9ucyxcbiAgRG9ja2VySW1hZ2UsXG4gIEZpbGVTeXN0ZW0sXG4gIElMb2NhbEJ1bmRsaW5nLFxufSBmcm9tICdhd3MtY2RrLWxpYic7XG5pbXBvcnQgeyBCdWlsZE9wdGlvbnMgfSBmcm9tICcuL2VzYnVpbGQtdHlwZXMnO1xuaW1wb3J0IHsgaXNFc2J1aWxkRXJyb3IgfSBmcm9tICcuL3ByaXZhdGUvdXRpbHMnO1xuaW1wb3J0IHsgRXNidWlsZFByb3ZpZGVyLCBJQnVpbGRQcm92aWRlciB9IGZyb20gJy4vcHJvdmlkZXInO1xuXG4vKipcbiAqIEEgcGF0aCBvciBsaXN0IG9yIG1hcCBvZiBwYXRocyB0byB0aGUgZW50cnkgcG9pbnRzIG9mIHlvdXIgY29kZS5cbiAqXG4gKiBSZWxhdGl2ZSBwYXRocyBhcmUgYnkgZGVmYXVsdCByZXNvbHZlZCBmcm9tIHRoZSBjdXJyZW50IHdvcmtpbmcgZGlyZWN0b3J5LlxuICogVG8gY2hhbmdlIHRoZSB3b3JraW5nIGRpcmVjdG9yeSwgc2VlIGBidWlsZE9wdGlvbnMuYWJzV29ya2luZ0RpcmAuXG4gKlxuICogQWJzb2x1dGUgcGF0aHMgY2FuIGJlIHVzZWQgaWYgZmlsZXMgYXJlIHBhcnQgb2YgdGhlIHdvcmtpbmcgZGlyZWN0b3J5LlxuICpcbiAqIEV4YW1wbGVzOlxuICogIC0gYCdzcmMvaW5kZXgudHMnYFxuICogIC0gYHJlcXVpcmUucmVzb2x2ZSgnLi9sYW1iZGEnKWBcbiAqICAtIGBbJ3NyYy9pbmRleC50cycsICdzcmMvdXRpbC50cyddYFxuICogIC0gYHtvbmU6ICdzcmMvdHdvLnRzJywgdHdvOiAnc3JjL29uZS50cyd9YFxuICpcbiAqIEBzdGFiaWxpdHkgc3RhYmxlXG4gKi9cbmV4cG9ydCB0eXBlIEVudHJ5UG9pbnRzID0gc3RyaW5nIHwgc3RyaW5nW10gfCBSZWNvcmQ8c3RyaW5nLCBzdHJpbmc+O1xuXG4vKipcbiAqIEBzdGFiaWxpdHkgc3RhYmxlXG4gKi9cbmV4cG9ydCBpbnRlcmZhY2UgQnVuZGxlclByb3BzIHtcbiAgLyoqXG4gICAqIEJ1aWxkIG9wdGlvbnMgcGFzc2VkIG9uIHRvIGVzYnVpbGQuIFBsZWFzZSByZWZlciB0byB0aGUgZXNidWlsZCBCdWlsZCBBUEkgZG9jcyBmb3IgZGV0YWlscy5cbiAgICpcbiAgICogKiBgYnVpbGRPcHRpb25zLm91dGRpcjogc3RyaW5nYFxuICAgKiBUaGUgYWN0dWFsIHBhdGggZm9yIHRoZSBvdXRwdXQgZGlyZWN0b3J5IGlzIGRlZmluZWQgYnkgQ0RLLiBIb3dldmVyIHNldHRpbmcgdGhpcyBvcHRpb24gYWxsb3dzIHRvIHdyaXRlIGZpbGVzIGludG8gYSBzdWJkaXJlY3RvcnkuIFxcXG4gICAqIEZvciBleGFtcGxlIGB7IG91dGRpcjogJ2pzJyB9YCB3aWxsIGNyZWF0ZSBhbiBhc3NldCB3aXRoIGEgc2luZ2xlIGRpcmVjdG9yeSBjYWxsZWQgYGpzYCwgd2hpY2ggY29udGFpbnMgYWxsIGJ1aWx0IGZpbGVzLiBUaGlzIGFwcHJvYWNoIGNhbiBiZSB1c2VmdWwgZm9yIHN0YXRpYyB3ZWJzaXRlIGRlcGxveW1lbnRzLCB3aGVyZSBKYXZhU2NyaXB0IGNvZGUgc2hvdWxkIGJlIHBsYWNlZCBpbnRvIGEgc3ViZGlyZWN0b3J5LiBcXFxuICAgKiAqQ2Fubm90IGJlIHVzZWQgdG9nZXRoZXIgd2l0aCBgb3V0ZmlsZWAqLlxuICAgKiAqIGBidWlsZE9wdGlvbnMub3V0ZmlsZTogc3RyaW5nYFxuICAgKiBSZWxhdGl2ZSBwYXRoIHRvIGEgZmlsZSBpbnNpZGUgdGhlIENESyBhc3NldCBvdXRwdXQgZGlyZWN0b3J5LlxuICAgKiBGb3IgZXhhbXBsZSBgeyBvdXRmaWxlOiAnanMvaW5kZXguanMnIH1gIHdpbGwgY3JlYXRlIGFuIGFzc2V0IHdpdGggYSBzaW5nbGUgZGlyZWN0b3J5IGNhbGxlZCBganNgLCB3aGljaCBjb250YWlucyBhIHNpbmdsZSBmaWxlIGBpbmRleC5qc2AuIFRoaXMgY2FuIGJlIHVzZWZ1bCB0byByZW5hbWUgdGhlIGVudHJ5IHBvaW50LiBcXFxuICAgKiAqQ2Fubm90IGJlIHVzZWQgd2l0aCBtdWx0aXBsZSBlbnRyeVBvaW50cyBvciB0b2dldGhlciB3aXRoIGBvdXRkaXJgLipcbiAgICogKiBgYnVpbGRPcHRpb25zLmFic1dvcmtpbmdEaXI6IHN0cmluZ2BcbiAgICogQWJzb2x1dGUgcGF0aCB0byB0aGUgW2VzYnVpbGQgd29ya2luZyBkaXJlY3RvcnldKGh0dHBzOi8vZXNidWlsZC5naXRodWIuaW8vYXBpLyN3b3JraW5nLWRpcmVjdG9yeSkgYW5kIGRlZmF1bHRzIHRvIHRoZSBbY3VycmVudCB3b3JraW5nIGRpcmVjdG9yeV0oaHR0cHM6Ly9lbi53aWtpcGVkaWEub3JnL3dpa2kvV29ya2luZ19kaXJlY3RvcnkpLiBcXFxuICAgKiBJZiBwYXRocyBjYW5ub3QgYmUgZm91bmQsIGEgZ29vZCBzdGFydGluZyBwb2ludCBpcyB0byBsb29rIGF0IHRoZSBjb25jYXRlbmF0aW9uIG9mIGBhYnNXb3JraW5nRGlyICsgZW50cnlQb2ludGAuIEl0IG11c3QgYWx3YXlzIGJlIGEgdmFsaWQgYWJzb2x1dGUgcGF0aCBwb2ludGluZyB0byB0aGUgZW50cnkgcG9pbnQuIFdoZW4gbmVlZGVkLCB0aGUgcHJvYmFibHkgZWFzaWVzdCB3YXkgdG8gc2V0IGFic1dvcmtpbmdEaXIgaXMgdG8gdXNlIGEgY29tYmluYXRpb24gb2YgYHJlc29sdmVgIGFuZCBgX19kaXJuYW1lYCAoc2VlIFwiTGlicmFyeSBhdXRob3JzXCIgc2VjdGlvbiBpbiB0aGUgZG9jdW1lbnRhdGlvbikuXG4gICAqXG4gICAqIEBzZWUgaHR0cHM6Ly9lc2J1aWxkLmdpdGh1Yi5pby9hcGkvI2J1aWxkLWFwaVxuICAgKiBAc3RhYmlsaXR5IHN0YWJsZVxuICAgKi9cbiAgcmVhZG9ubHkgYnVpbGRPcHRpb25zPzogQnVpbGRPcHRpb25zO1xuXG4gIC8qKlxuICAgKiBUaGUgZXNidWlsZCBCdWlsZCBBUEkgaW1wbGVtZW50YXRpb24gdG8gYmUgdXNlZC5cbiAgICpcbiAgICogQ29uZmlndXJlIHRoZSBkZWZhdWx0IGBFc2J1aWxkUHJvdmlkZXJgIGZvciBtb3JlIG9wdGlvbnMgb3JcbiAgICogcHJvdmlkZSBhIGN1c3RvbSBgSUJ1aWxkUHJvdmlkZXJgIGFzIGFuIGVzY2FwZSBoYXRjaC5cbiAgICpcbiAgICogQHN0YWJpbGl0eSBzdGFibGVcbiAgICpcbiAgICogQGRlZmF1bHQgbmV3IEVzYnVpbGRQcm92aWRlcigpXG4gICAqL1xuICByZWFkb25seSBidWlsZFByb3ZpZGVyPzogSUJ1aWxkUHJvdmlkZXI7XG5cbiAgLyoqXG4gICAqIENvcHkgYWRkaXRpb25hbCBmaWxlcyB0byB0aGUgY29kZSBbYXNzZXQgc3RhZ2luZyBkaXJlY3RvcnldKGh0dHBzOi8vZG9jcy5hd3MuYW1hem9uLmNvbS9jZGsvYXBpL3YyL2RvY3MvYXdzLWNkay1saWIuQXNzZXRTdGFnaW5nLmh0bWwjYWJzb2x1dGVzdGFnZWRwYXRoKSwgYmVmb3JlIHRoZSBidWlsZCBydW5zLlxuICAgKiBGaWxlcyBjb3BpZWQgbGlrZSB0aGlzIHdpbGwgYmUgb3ZlcndyaXR0ZW4gYnkgZXNidWlsZCBpZiB0aGV5IHNoYXJlIHRoZSBzYW1lIG5hbWUgYXMgYW55IG9mIHRoZSBvdXRwdXRzLlxuICAgKlxuICAgKiAqIFdoZW4gcHJvdmlkZWQgd2l0aCBhIGBzdHJpbmdgIG9yIGBhcnJheWAsIGFsbCBmaWxlcyBhcmUgY29waWVkIHRvIHRoZSByb290IG9mIGFzc2V0IHN0YWdpbmcgZGlyZWN0b3J5LlxuICAgKiAqIFdoZW4gZ2l2ZW4gYSBgbWFwYCwgdGhlIGtleSBpbmRpY2F0ZXMgdGhlIGRlc3RpbmF0aW9uIHJlbGF0aXZlIHRvIHRoZSBhc3NldCBzdGFnaW5nIGRpcmVjdG9yeSBhbmQgdGhlIHZhbHVlIGlzIGEgbGlzdCBvZiBhbGwgc291cmNlcyB0byBiZSBjb3BpZWQuXG4gICAqXG4gICAqIFRoZXJlZm9yZSB0aGUgZm9sbG93aW5nIHZhbHVlcyBmb3IgYGNvcHlEaXJgIGFyZSBhbGwgZXF1aXZhbGVudDpcbiAgICogYGBgXG4gICAqIHsgY29weURpcjogXCJwYXRoL3RvL3NvdXJjZVwiIH1cbiAgICogeyBjb3B5RGlyOiBbXCJwYXRoL3RvL3NvdXJjZVwiXSB9XG4gICAqIHsgY29weURpcjogeyBcIi5cIjogXCJwYXRoL3RvL3NvdXJjZVwiIH0gfVxuICAgKiB7IGNvcHlEaXI6IHsgXCIuXCI6IFtcInBhdGgvdG8vc291cmNlXCJdIH0gfVxuICAgKiBgYGBcbiAgICogVGhlIGRlc3RpbmF0aW9uIGNhbm5vdCBiZSBvdXRzaWRlIG9mIHRoZSBhc3NldCBzdGFnaW5nIGRpcmVjdG9yeS5cbiAgICogSWYgeW91IGFyZSByZWNlaXZpbmcgdGhlIGVycm9yIFwiQ2Fubm90IGNvcHkgZmlsZXMgdG8gb3V0c2lkZSBvZiB0aGUgYXNzZXQgc3RhZ2luZyBkaXJlY3RvcnkuXCJcbiAgICogeW91IGFyZSBsaWtlbHkgdXNpbmcgYC4uYCBvciBhbiBhYnNvbHV0ZSBwYXRoIGFzIGtleSBvbiB0aGUgYGNvcHlEaXJgIG1hcC5cbiAgICogSW5zdGVhZCB1c2Ugb25seSByZWxhdGl2ZSBwYXRocyBhbmQgYXZvaWQgYC4uYC5cbiAgICpcbiAgICogQHN0YWJpbGl0eSBzdGFibGVcbiAgICovXG4gIHJlYWRvbmx5IGNvcHlEaXI/OiBzdHJpbmcgfCBzdHJpbmdbXSB8IFJlY29yZDxzdHJpbmcsIHN0cmluZyB8IHN0cmluZ1tdPjtcbn1cblxuLyoqXG4gKiBMb3ctbGV2ZWwgY29uc3RydWN0IHRoYXQgY2FuIGJlIHVzZWQgd2hlcmUgYEJ1bmRsaW5nT3B0aW9uc2AgYXJlIHJlcXVpcmVkLlxuICogVGhpcyBjbGFzcyBkaXJlY3RseSBpbnRlcmZhY2VzIHdpdGggZXNidWlsZCBhbmQgcHJvdmlkZXMgYWxtb3N0IG5vIGNvbmZpZ3VyYXRpb24gc2FmZWd1YXJkcy5cbiAqXG4gKiBAc3RhYmlsaXR5IGV4cGVyaW1lbnRhbFxuICovXG5leHBvcnQgY2xhc3MgRXNidWlsZEJ1bmRsZXIge1xuICAvKipcbiAgICogSW1wbGVtZW50YXRpb24gb2YgYElMb2NhbEJ1bmRsaW5nYCBpbnRlcmZhY2UsIHJlc3BvbnNpYmxlIGZvciBjYWxsaW5nIGVzYnVpbGQgZnVuY3Rpb25zLlxuICAgKlxuICAgKiBAc3RhYmlsaXR5IGV4cGVyaW1lbnRhbFxuICAgKi9cbiAgcHVibGljIHJlYWRvbmx5IGxvY2FsOiBJTG9jYWxCdW5kbGluZztcblxuICAvKipcbiAgICogQGRlcHJlY2F0ZWQgVGhpcyB2YWx1ZSBpcyBpZ25vcmVkIHNpbmNlIHRoZSBidW5kbGVyIGlzIGFsd2F5cyB1c2luZyBhIGxvY2FsbHkgaW5zdGFsbGVkIHZlcnNpb24gb2YgZXNidWlsZC4gSG93ZXZlciB0aGUgcHJvcGVydHkgaXMgcmVxdWlyZWQgdG8gY29tcGx5IHdpdGggdGhlIGBCdW5kbGluZ09wdGlvbnNgIGludGVyZmFjZS5cbiAgICpcbiAgICogQHN0YWJpbGl0eSBkZXByZWNhdGVkXG4gICAqL1xuICBwdWJsaWMgcmVhZG9ubHkgaW1hZ2UgPSBEb2NrZXJJbWFnZS5mcm9tUmVnaXN0cnkoJ3NjcmF0Y2gnKTtcblxuICAvKipcbiAgICogQHN0YWJpbGl0eSBleHBlcmltZW50YWxcbiAgICovXG4gIHB1YmxpYyBjb25zdHJ1Y3RvcihcbiAgICAvKipcbiAgICAgKiBBIHBhdGggb3IgbGlzdCBvciBtYXAgb2YgcGF0aHMgdG8gdGhlIGVudHJ5IHBvaW50cyBvZiB5b3VyIGNvZGUuXG4gICAgICpcbiAgICAgKiBSZWxhdGl2ZSBwYXRocyBhcmUgYnkgZGVmYXVsdCByZXNvbHZlZCBmcm9tIHRoZSBjdXJyZW50IHdvcmtpbmcgZGlyZWN0b3J5LlxuICAgICAqIFRvIGNoYW5nZSB0aGUgd29ya2luZyBkaXJlY3RvcnksIHNlZSBgYnVpbGRPcHRpb25zLmFic1dvcmtpbmdEaXJgLlxuICAgICAqXG4gICAgICogQWJzb2x1dGUgcGF0aHMgY2FuIGJlIHVzZWQgaWYgZmlsZXMgYXJlIHBhcnQgb2YgdGhlIHdvcmtpbmcgZGlyZWN0b3J5LlxuICAgICAqXG4gICAgICogRXhhbXBsZXM6XG4gICAgICogIC0gYCdzcmMvaW5kZXgudHMnYFxuICAgICAqICAtIGByZXF1aXJlLnJlc29sdmUoJy4vbGFtYmRhJylgXG4gICAgICogIC0gYFsnc3JjL2luZGV4LnRzJywgJ3NyYy91dGlsLnRzJ11gXG4gICAgICogIC0gYHtvbmU6ICdzcmMvdHdvLnRzJywgdHdvOiAnc3JjL29uZS50cyd9YFxuICAgICAqXG4gICAgICogQHN0YWJpbGl0eSBleHBlcmltZW50YWxcbiAgICAgKi9cbiAgICBwdWJsaWMgcmVhZG9ubHkgZW50cnlQb2ludHM6IEVudHJ5UG9pbnRzLFxuXG4gICAgLyoqXG4gICAgICogUHJvcHMgdG8gY2hhbmdlIHRoZSBiZWhhdmlvciBvZiB0aGUgYnVuZGxlci5cbiAgICAgKlxuICAgICAqIEBzdGFiaWxpdHkgZXhwZXJpbWVudGFsXG4gICAgICovXG4gICAgcHVibGljIHJlYWRvbmx5IHByb3BzOiBCdW5kbGVyUHJvcHMsXG4gICkge1xuICAgIGlmIChwcm9wcz8uYnVpbGRPcHRpb25zPy5vdXRmaWxlICYmIHByb3BzPy5idWlsZE9wdGlvbnM/Lm91dGRpcikge1xuICAgICAgdGhyb3cgbmV3IEVycm9yKCdDYW5ub3QgdXNlIGJvdGggXCJvdXRmaWxlXCIgYW5kIFwib3V0ZGlyXCInKTtcbiAgICB9XG4gICAgdGhpcy5sb2NhbCA9IHtcbiAgICAgIHRyeUJ1bmRsZTogKG91dHB1dERpcjogc3RyaW5nLCBfb3B0aW9uczogQnVuZGxpbmdPcHRpb25zKTogYm9vbGVhbiA9PiB7XG5cbiAgICAgICAgaWYgKHRoaXMucHJvcHMuY29weURpcikge1xuICAgICAgICAgIGNvbnN0IGNvcHlEaXIgPSB0aGlzLmdldENvcHlEaXJMaXN0KHRoaXMucHJvcHMuY29weURpcik7XG5cbiAgICAgICAgICBjb3B5RGlyLmZvckVhY2goKFtkZXN0LCBzcmNdKSA9PiB7XG4gICAgICAgICAgICBjb25zdCBzcmNEaXIgPSByZXNvbHZlKFxuICAgICAgICAgICAgICB0aGlzLnByb3BzPy5idWlsZE9wdGlvbnM/LmFic1dvcmtpbmdEaXIgPz8gcHJvY2Vzcy5jd2QoKSxcbiAgICAgICAgICAgICAgc3JjLFxuICAgICAgICAgICAgKTtcbiAgICAgICAgICAgIGNvbnN0IGRlc3REaXIgPSByZXNvbHZlKG91dHB1dERpciwgZGVzdCk7XG5cbiAgICAgICAgICAgIGNvbnN0IGRlc3RUb091dHB1dCA9IHJlbGF0aXZlKG91dHB1dERpciwgZGVzdERpcik7XG4gICAgICAgICAgICBpZiAoZGVzdFRvT3V0cHV0LnN0YXJ0c1dpdGgoJy4uJykgfHwgaXNBYnNvbHV0ZShkZXN0VG9PdXRwdXQpKSB7XG4gICAgICAgICAgICAgIHRocm93IG5ldyBFcnJvcignQ2Fubm90IGNvcHkgZmlsZXMgdG8gb3V0c2lkZSBvZiB0aGUgYXNzZXQgc3RhZ2luZyBkaXJlY3RvcnkuIFNlZSBkb2NzIGZvciBkZXRhaWxzLicpO1xuICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICBpZiAoZXhpc3RzU3luYyhkZXN0RGlyKSkge1xuICAgICAgICAgICAgICBybVN5bmMoZGVzdERpciwgeyByZWN1cnNpdmU6IHRydWUsIGZvcmNlOiB0cnVlIH0pO1xuICAgICAgICAgICAgfVxuICAgICAgICAgICAgbWtkaXJTeW5jKGRlc3REaXIsIHsgcmVjdXJzaXZlOiB0cnVlIH0pO1xuICAgICAgICAgICAgRmlsZVN5c3RlbS5jb3B5RGlyZWN0b3J5KHNyY0RpciwgZGVzdERpcik7XG4gICAgICAgICAgfSk7XG4gICAgICAgIH1cblxuICAgICAgICB0cnkge1xuICAgICAgICAgIGNvbnN0IHByb3ZpZGVyID0gcHJvcHMuYnVpbGRQcm92aWRlciA/PyBFc2J1aWxkUHJvdmlkZXIuZGVmYXVsdEJ1aWxkUHJvdmlkZXIoKTtcblxuICAgICAgICAgIHByb3ZpZGVyLmJ1aWxkU3luYyh7XG4gICAgICAgICAgICBlbnRyeVBvaW50czogdHlwZW9mIGVudHJ5UG9pbnRzID09PSAnc3RyaW5nJyA/IFtlbnRyeVBvaW50c10gOiBlbnRyeVBvaW50cyxcbiAgICAgICAgICAgIGNvbG9yOiBwcm9jZXNzLmVudi5OT19DT0xPUiA/IEJvb2xlYW4ocHJvY2Vzcy5lbnYuTk9fQ09MT1IpIDogdW5kZWZpbmVkLFxuICAgICAgICAgICAgLi4uKHRoaXMucHJvcHM/LmJ1aWxkT3B0aW9ucyB8fCB7fSksXG4gICAgICAgICAgICAuLi50aGlzLmdldE91dHB1dE9wdGlvbnMob3V0cHV0RGlyLCB7IG5vcm1hbGl6ZSwgam9pbiB9KSxcbiAgICAgICAgICB9KTtcbiAgICAgICAgfSBjYXRjaCAoZXJyb3IpIHtcbiAgICAgICAgICBpZiAoaXNFc2J1aWxkRXJyb3IoZXJyb3IpKSB7XG4gICAgICAgICAgICB0aHJvdyBuZXcgRXJyb3IoYEVzYnVpbGQgZmFpbGVkIHRvIGJ1bmRsZSAke2VudHJ5UG9pbnRzfWApO1xuICAgICAgICAgIH1cbiAgICAgICAgICB0aHJvdyBlcnJvcjtcbiAgICAgICAgfVxuXG4gICAgICAgIHJldHVybiB0cnVlO1xuICAgICAgfSxcbiAgICB9O1xuICB9XG5cbiAgcHJpdmF0ZSBnZXRDb3B5RGlyTGlzdChjb3B5RGlyOiBCdW5kbGVyUHJvcHNbJ2NvcHlEaXInXSk6IEFycmF5PFtzdHJpbmcsIHN0cmluZ10+IHtcbiAgICAvLyBOb3RoaW5nIHRvIGNvcHlcbiAgICBpZiAoIWNvcHlEaXIpIHtcbiAgICAgIHJldHVybiBbXTtcbiAgICB9XG5cbiAgICAvLyBMaXN0IG9mIHN0cmluZ3NcbiAgICBpZiAoQXJyYXkuaXNBcnJheShjb3B5RGlyKSkge1xuICAgICAgcmV0dXJuIGNvcHlEaXIubWFwKChzcmM6IHN0cmluZykgPT4gWycuJywgc3JjXSk7XG4gICAgfVxuXG4gICAgLy8gQSBtYXBcbiAgICBpZiAoXG4gICAgICB0eXBlb2YgY29weURpciA9PT0gJ29iamVjdCcgJiZcbiAgICAgICFBcnJheS5pc0FycmF5KGNvcHlEaXIpICYmXG4gICAgICBjb3B5RGlyICE9PSBudWxsXG4gICAgKSB7XG4gICAgICByZXR1cm4gT2JqZWN0XG4gICAgICAgIC5lbnRyaWVzKGNvcHlEaXIpXG4gICAgICAgIC5mbGF0TWFwKChbZGVzdCwgc291cmNlc10pID0+IHtcbiAgICAgICAgICBpZiAoQXJyYXkuaXNBcnJheShzb3VyY2VzKSkge1xuICAgICAgICAgICAgcmV0dXJuIHNvdXJjZXMubWFwKChzcmMpID0+IFtkZXN0LCBzcmNdKSBhcyBBcnJheTxbc3RyaW5nLCBzdHJpbmddPjtcbiAgICAgICAgICB9XG5cbiAgICAgICAgICByZXR1cm4gW1tkZXN0LCBzb3VyY2VzXV07XG4gICAgICAgIH0pO1xuICAgIH1cblxuICAgIC8vIEEgc2luZ2xlIHN0cmluZ1xuICAgIHJldHVybiBbWycuJywgY29weURpciBhcyBzdHJpbmddXTtcbiAgfVxuXG4gIHByaXZhdGUgZ2V0T3V0cHV0T3B0aW9ucyhcbiAgICBjZGtPdXRwdXREaXI6IHN0cmluZyxcbiAgICBwYXRoOiBQaWNrPHR5cGVvZiBwb3NpeCwgJ25vcm1hbGl6ZScgfCAnam9pbic+ID0gcG9zaXgsXG4gICk6IEJ1aWxkT3B0aW9ucyB7XG4gICAgaWYgKHRoaXMucHJvcHM/LmJ1aWxkT3B0aW9ucz8ub3V0ZmlsZSkge1xuICAgICAgcmV0dXJuIHtcbiAgICAgICAgb3V0ZGlyOiB1bmRlZmluZWQsXG4gICAgICAgIG91dGZpbGU6IHBhdGgubm9ybWFsaXplKFxuICAgICAgICAgIHBhdGguam9pbihcbiAgICAgICAgICAgIC4uLihbY2RrT3V0cHV0RGlyLCB0aGlzLnByb3BzPy5idWlsZE9wdGlvbnM/Lm91dGZpbGVdLmZpbHRlcihcbiAgICAgICAgICAgICAgQm9vbGVhbixcbiAgICAgICAgICAgICkgYXMgc3RyaW5nW10pLFxuICAgICAgICAgICksXG4gICAgICAgICksXG4gICAgICB9O1xuICAgIH1cblxuICAgIHJldHVybiB7XG4gICAgICBvdXRkaXI6IHBhdGgubm9ybWFsaXplKFxuICAgICAgICBwYXRoLmpvaW4oXG4gICAgICAgICAgLi4uKFtjZGtPdXRwdXREaXIsIHRoaXMucHJvcHM/LmJ1aWxkT3B0aW9ucz8ub3V0ZGlyXS5maWx0ZXIoXG4gICAgICAgICAgICBCb29sZWFuLFxuICAgICAgICAgICkgYXMgc3RyaW5nW10pLFxuICAgICAgICApLFxuICAgICAgKSxcbiAgICAgIG91dGZpbGU6IHVuZGVmaW5lZCxcbiAgICB9O1xuICB9XG59XG4iXX0=
```

##### package/lib/code.js

###### js-beautify {}

```diff
@@ -98,15 +98,15 @@
         this.asset.addResourceMetadata(resource, resourceProperty);
     }
 }
 exports.EsbuildCode = EsbuildCode;
 _a = JSII_RTTI_SYMBOL_1;
 EsbuildCode[_a] = {
     fqn: "@mrgrain/cdk-esbuild.EsbuildCode",
-    version: "4.2.0"
+    version: "4.2.1"
 };
 /**
  * Represents the deployed JavaScript Code.
  *
  * @stability stable
  */
 class JavaScriptCode extends EsbuildCode {
@@ -145,15 +145,15 @@
         return new asset_1.JavaScriptAsset(scope, this.constructor.name, this.props);
     }
 }
 exports.JavaScriptCode = JavaScriptCode;
 _b = JSII_RTTI_SYMBOL_1;
 JavaScriptCode[_b] = {
     fqn: "@mrgrain/cdk-esbuild.JavaScriptCode",
-    version: "4.2.0"
+    version: "4.2.1"
 };
 /**
  * Represents the deployed TypeScript Code.
  *
  * @stability stable
  */
 class TypeScriptCode extends EsbuildCode {
@@ -192,10 +192,10 @@
         return new asset_1.TypeScriptAsset(scope, this.constructor.name, this.props);
     }
 }
 exports.TypeScriptCode = TypeScriptCode;
 _c = JSII_RTTI_SYMBOL_1;
 TypeScriptCode[_c] = {
     fqn: "@mrgrain/cdk-esbuild.TypeScriptCode",
-    version: "4.2.0"
+    version: "4.2.1"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiY29kZS5qcyIsInNvdXJjZVJvb3QiOiIiLCJzb3VyY2VzIjpbIi4uL3NyYy9jb2RlLnRzIl0sIm5hbWVzIjpbXSwibWFwcGluZ3MiOiI7Ozs7O0FBQUEsNkNBQWlEO0FBQ2pELHVEQUErRTtBQUUvRSxtQ0FNaUI7QUFHakIsMkNBQXVEO0FBR08sQ0FBQztBQUNELENBQUM7QUFFL0Q7Ozs7OztHQU1HO0FBQ0gsTUFBYSxXQUVYLFNBQVEsaUJBQUk7SUFvQlo7SUFDRTs7Ozs7Ozs7Ozs7Ozs7O09BZUc7SUFDTSxXQUF3QjtJQUVqQzs7Ozs7Ozs7O09BU0c7SUFDSCxLQUFZO1FBRVosS0FBSyxFQUFFLENBQUM7UUFkQyxnQkFBVyxHQUFYLFdBQVcsQ0FBYTtRQXhCbkM7Ozs7V0FJRztRQUNJLGFBQVEsR0FBWSxLQUFLLENBQUM7UUFtQy9CLE1BQU0sY0FBYyxHQUEwQiw0QkFBb0IsQ0FBQyxLQUFLLENBQUMsWUFBWSxDQUFDLENBQUM7UUFFdkYsSUFBSSxDQUFDLEtBQUssR0FBRztZQUNYLEdBQUcsS0FBSztZQUNSLFdBQVc7WUFDWCxZQUFZLEVBQUU7Z0JBQ1osR0FBRyxjQUFjO2dCQUNqQixHQUFHLEtBQUssQ0FBQyxZQUFZO2FBQ3RCO1NBQ0YsQ0FBQztJQUNKLENBQUM7SUE5RFMsUUFBUSxDQUFDLEtBQWdCO1FBQ2pDLE9BQU8sSUFBSSxvQkFBWSxDQUNyQixLQUFLLEVBQ0wsSUFBSSxDQUFDLFdBQVcsQ0FBQyxJQUFJLEVBQ3JCLElBQUksQ0FBQyxLQUFLLENBQ1gsQ0FBQztJQUNKLENBQUM7SUEwREQsSUFBSSxDQUFDLEtBQWdCO1FBQ25CLHFGQUFxRjtRQUNyRixJQUFJLENBQUMsSUFBSSxDQUFDLEtBQUssRUFBRTtZQUNmLElBQUksQ0FBQyxLQUFLLEdBQUcsSUFBSSxDQUFDLFFBQVEsQ0FBQyxLQUFLLENBQUMsQ0FBQztTQUNuQzthQUFNLElBQUksbUJBQUssQ0FBQyxFQUFFLENBQUMsSUFBSSxDQUFDLEtBQUssQ0FBQyxLQUFLLG1CQUFLLENBQUMsRUFBRSxDQUFDLEtBQUssQ0FBQyxFQUFFO1lBQ25ELE1BQU0sSUFBSSxLQUFLLENBQ2IsbURBQ0UsbUJBQUssQ0FBQyxFQUFFLENBQUMsSUFBSSxDQUFDLEtBQUssQ0FBQyxDQUFDLFNBQ3ZCLEtBQUssR0FBRyw4Q0FBOEMsQ0FDdkQsQ0FBQztTQUNIO1FBRUQsT0FBTztZQUNMLFVBQVUsRUFBRTtnQkFDVixVQUFVLEVBQUUsSUFBSSxDQUFDLEtBQUssQ0FBQyxZQUFZO2dCQUNuQyxTQUFTLEVBQUUsSUFBSSxDQUFDLEtBQUssQ0FBQyxXQUFXO2FBQ2xDO1NBQ0YsQ0FBQztJQUNKLENBQUM7SUFFRDs7Ozs7OztPQU9HO0lBQ0gsY0FBYyxDQUFDLFFBQXFCLEVBQUUsT0FBNkI7UUFDakUsSUFBSSxDQUFDLElBQUksQ0FBQyxLQUFLLEVBQUU7WUFDZixNQUFNLElBQUksS0FBSyxDQUFDLDhDQUE4QyxDQUFDLENBQUM7U0FDakU7UUFDRCxNQUFNLGdCQUFnQixHQUFHLE9BQU8sRUFBRSxnQkFBZ0IsSUFBSSxJQUFJLENBQUMsV0FBVyxDQUFDLElBQUksQ0FBQztRQUM1RSw2Q0FBNkM7UUFDN0MsSUFBSSxDQUFDLEtBQUssQ0FBQyxtQkFBbUIsQ0FBQyxRQUFRLEVBQUUsZ0JBQWdCLENBQUMsQ0FBQztJQUM3RCxDQUFDOztBQXRHSCxrQ0F1R0M7OztBQUVEOzs7O0dBSUc7QUFDSCxNQUFhLGNBQWUsU0FBUSxXQUFnQztJQVNsRTtJQUNFOzs7Ozs7Ozs7Ozs7Ozs7T0FlRztJQUNILFdBQXdCO0lBRXhCOzs7Ozs7Ozs7T0FTRztJQUNILFFBQTZCLEVBQUU7UUFFL0IsS0FBSyxDQUFDLFdBQVcsRUFBRSxLQUFLLENBQUMsQ0FBQztJQUM1QixDQUFDO0lBeENTLFFBQVEsQ0FBQyxLQUFnQjtRQUNqQyxPQUFPLElBQUksdUJBQU8sQ0FDaEIsS0FBSyxFQUNMLElBQUksQ0FBQyxXQUFXLENBQUMsSUFBSSxFQUNyQixJQUFJLENBQUMsS0FBSyxDQUNYLENBQUM7SUFDSixDQUFDOztBQVBILHdDQTBDQzs7O0FBRUQ7Ozs7R0FJRztBQUNILE1BQWEsY0FBZSxTQUFRLFdBQWdDO0lBU2xFO0lBQ0U7Ozs7Ozs7Ozs7Ozs7OztPQWVHO0lBQ0gsV0FBd0I7SUFFeEI7Ozs7Ozs7OztPQVNHO0lBQ0gsUUFBNkIsRUFBRTtRQUUvQixLQUFLLENBQUMsV0FBVyxFQUFFLEtBQUssQ0FBQyxDQUFDO0lBQzVCLENBQUM7SUF4Q1MsUUFBUSxDQUFDLEtBQWdCO1FBQ2pDLE9BQU8sSUFBSSx1QkFBTyxDQUNoQixLQUFLLEVBQ0wsSUFBSSxDQUFDLFdBQVcsQ0FBQyxJQUFJLEVBQ3JCLElBQUksQ0FBQyxLQUFLLENBQ1gsQ0FBQztJQUNKLENBQUM7O0FBUEgsd0NBMENDIiwic291cmNlc0NvbnRlbnQiOlsiaW1wb3J0IHsgQ2ZuUmVzb3VyY2UsIFN0YWNrIH0gZnJvbSAnYXdzLWNkay1saWInO1xuaW1wb3J0IHsgUmVzb3VyY2VCaW5kT3B0aW9ucywgQ29kZSwgQ29kZUNvbmZpZyB9IGZyb20gJ2F3cy1jZGstbGliL2F3cy1sYW1iZGEnO1xuaW1wb3J0IHsgQ29uc3RydWN0IH0gZnJvbSAnY29uc3RydWN0cyc7XG5pbXBvcnQge1xuICBFc2J1aWxkQXNzZXQsXG4gIEFzc2V0QmFzZVByb3BzLFxuICBBc3NldFByb3BzLFxuICBKYXZhU2NyaXB0QXNzZXQgYXMgSlNBc3NldCxcbiAgVHlwZVNjcmlwdEFzc2V0IGFzIFRTQXNzZXQsXG59IGZyb20gJy4vYXNzZXQnO1xuaW1wb3J0IHsgRW50cnlQb2ludHMgfSBmcm9tICcuL2J1bmRsZXInO1xuaW1wb3J0IHsgQnVpbGRPcHRpb25zIH0gZnJvbSAnLi9lc2J1aWxkLXR5cGVzJztcbmltcG9ydCB7IGRlZmF1bHRQbGF0Zm9ybVByb3BzIH0gZnJvbSAnLi9wcml2YXRlL3V0aWxzJztcblxuZXhwb3J0IHsgQ29kZUNvbmZpZyB9IGZyb20gJ2F3cy1jZGstbGliL2F3cy1sYW1iZGEnO1xuZXhwb3J0IGludGVyZmFjZSBKYXZhU2NyaXB0Q29kZVByb3BzIGV4dGVuZHMgQXNzZXRCYXNlUHJvcHMge307XG5leHBvcnQgaW50ZXJmYWNlIFR5cGVTY3JpcHRDb2RlUHJvcHMgZXh0ZW5kcyBBc3NldEJhc2VQcm9wcyB7fTtcblxuLyoqXG4gKiBSZXByZXNlbnRzIGEgZ2VuZXJpYyBlc2J1aWxkIGNvZGUgYnVuZGxlLlxuICpcbiAqIFlvdSBzaG91bGQgYWx3YXlzIHVzZSBgVHlwZVNjcmlwdENvZGVgIG9yIGBKYXZhU2NyaXB0Q29kZWAuXG4gKlxuICogQHN0YWJpbGl0eSBleHBlcmltZW50YWxcbiAqL1xuZXhwb3J0IGNsYXNzIEVzYnVpbGRDb2RlPFxuICBQcm9wcyBleHRlbmRzIEphdmFTY3JpcHRDb2RlUHJvcHMgfCBUeXBlU2NyaXB0Q29kZVByb3BzLFxuPiBleHRlbmRzIENvZGUge1xuICBwcm90ZWN0ZWQgZ2V0QXNzZXQoc2NvcGU6IENvbnN0cnVjdCk6IEVzYnVpbGRBc3NldDxBc3NldFByb3BzPiB7XG4gICAgcmV0dXJuIG5ldyBFc2J1aWxkQXNzZXQoXG4gICAgICBzY29wZSxcbiAgICAgIHRoaXMuY29uc3RydWN0b3IubmFtZSxcbiAgICAgIHRoaXMucHJvcHMsXG4gICAgKTtcbiAgfVxuXG4gIHByb3RlY3RlZCBwcm9wczogQXNzZXRQcm9wcztcblxuICBwcm90ZWN0ZWQgYXNzZXQhOiBFc2J1aWxkQXNzZXQ8QXNzZXRQcm9wcz47XG5cbiAgLyoqXG4gICAqIERldGVybWluZXMgd2hldGhlciB0aGlzIENvZGUgaXMgaW5saW5lIGNvZGUgb3Igbm90LlxuICAgKlxuICAgKiBAZGVwcmVjYXRlZCB0aGlzIHZhbHVlIGlzIGlnbm9yZWQgc2luY2UgaW5saW5lIGlzIG5vdyBkZXRlcm1pbmVkIGJhc2VkIG9uIHRoZSB0aGUgaW5saW5lQ29kZSBmaWVsZCBvZiBDb2RlQ29uZmlnIHJldHVybmVkIGZyb20gYmluZCgpLlxuICAgKi9cbiAgcHVibGljIGlzSW5saW5lOiBib29sZWFuID0gZmFsc2U7XG5cbiAgY29uc3RydWN0b3IoXG4gICAgLyoqXG4gICAgICogQSBwYXRoIG9yIGxpc3Qgb3IgbWFwIG9mIHBhdGhzIHRvIHRoZSBlbnRyeSBwb2ludHMgb2YgeW91ciBjb2RlLlxuICAgICAqXG4gICAgICogUmVsYXRpdmUgcGF0aHMgYXJlIGJ5IGRlZmF1bHQgcmVzb2x2ZWQgZnJvbSB0aGUgY3VycmVudCB3b3JraW5nIGRpcmVjdG9yeS5cbiAgICAgKiBUbyBjaGFuZ2UgdGhlIHdvcmtpbmcgZGlyZWN0b3J5LCBzZWUgYGJ1aWxkT3B0aW9ucy5hYnNXb3JraW5nRGlyYC5cbiAgICAgKlxuICAgICAqIEFic29sdXRlIHBhdGhzIGNhbiBiZSB1c2VkIGlmIGZpbGVzIGFyZSBwYXJ0IG9mIHRoZSB3b3JraW5nIGRpcmVjdG9yeS5cbiAgICAgKlxuICAgICAqIEV4YW1wbGVzOlxuICAgICAqICAtIGAnc3JjL2luZGV4LnRzJ2BcbiAgICAgKiAgLSBgcmVxdWlyZS5yZXNvbHZlKCcuL2xhbWJkYScpYFxuICAgICAqICAtIGBbJ3NyYy9pbmRleC50cycsICdzcmMvdXRpbC50cyddYFxuICAgICAqICAtIGB7b25lOiAnc3JjL3R3by50cycsIHR3bzogJ3NyYy9vbmUudHMnfWBcbiAgICAgKlxuICAgICAqIEBzdGFiaWxpdHkgc3RhYmxlXG4gICAgICovXG4gICAgcmVhZG9ubHkgZW50cnlQb2ludHM6IEVudHJ5UG9pbnRzLFxuXG4gICAgLyoqXG4gICAgICogUHJvcHMgdG8gY2hhbmdlIHRoZSBiZWhhdmlvciBvZiB0aGUgYnVuZGxlci5cbiAgICAgKlxuICAgICAqIERlZmF1bHQgdmFsdWVzIGZvciBgcHJvcHMuYnVpbGRPcHRpb25zYDpcbiAgICAgKiAtIGBidW5kbGU9dHJ1ZWBcbiAgICAgKiAtIGBwbGF0Zm9ybT1ub2RlYFxuICAgICAqIC0gYHRhcmdldD1ub2RlWGAgd2l0aCBYIGJlaW5nIHRoZSBtYWpvciBub2RlIHZlcnNpb24gcnVubmluZyBsb2NhbGx5XG4gICAgICpcbiAgICAgKiBAc3RhYmlsaXR5IHN0YWJsZVxuICAgICAqL1xuICAgIHByb3BzOiBQcm9wcyxcbiAgKSB7XG4gICAgc3VwZXIoKTtcblxuICAgIGNvbnN0IGRlZmF1bHRPcHRpb25zOiBQYXJ0aWFsPEJ1aWxkT3B0aW9ucz4gPSBkZWZhdWx0UGxhdGZvcm1Qcm9wcyhwcm9wcy5idWlsZE9wdGlvbnMpO1xuXG4gICAgdGhpcy5wcm9wcyA9IHtcbiAgICAgIC4uLnByb3BzLFxuICAgICAgZW50cnlQb2ludHMsXG4gICAgICBidWlsZE9wdGlvbnM6IHtcbiAgICAgICAgLi4uZGVmYXVsdE9wdGlvbnMsXG4gICAgICAgIC4uLnByb3BzLmJ1aWxkT3B0aW9ucyxcbiAgICAgIH0sXG4gICAgfTtcbiAgfVxuXG4gIGJpbmQoc2NvcGU6IENvbnN0cnVjdCk6IENvZGVDb25maWcge1xuICAgIC8vIElmIHRoZSBzYW1lIEFzc2V0Q29kZSBpcyB1c2VkIG11bHRpcGxlIHRpbWVzLCByZXRhaW4gb25seSB0aGUgZmlyc3QgaW5zdGFudGlhdGlvbi5cbiAgICBpZiAoIXRoaXMuYXNzZXQpIHtcbiAgICAgIHRoaXMuYXNzZXQgPSB0aGlzLmdldEFzc2V0KHNjb3BlKTtcbiAgICB9IGVsc2UgaWYgKFN0YWNrLm9mKHRoaXMuYXNzZXQpICE9PSBTdGFjay5vZihzY29wZSkpIHtcbiAgICAgIHRocm93IG5ldyBFcnJvcihcbiAgICAgICAgYEFzc2V0IGlzIGFscmVhZHkgYXNzb2NpYXRlZCB3aXRoIGFub3RoZXIgc3RhY2sgJyR7XG4gICAgICAgICAgU3RhY2sub2YodGhpcy5hc3NldCkuc3RhY2tOYW1lXG4gICAgICAgIH0nLiBgICsgJ0NyZWF0ZSBhIG5ldyBBc3NldCBpbnN0YW5jZSBmb3IgZXZlcnkgc3RhY2suJyxcbiAgICAgICk7XG4gICAgfVxuXG4gICAgcmV0dXJuIHtcbiAgICAgIHMzTG9jYXRpb246IHtcbiAgICAgICAgYnVja2V0TmFtZTogdGhpcy5hc3NldC5zM0J1Y2tldE5hbWUsXG4gICAgICAgIG9iamVjdEtleTogdGhpcy5hc3NldC5zM09iamVjdEtleSxcbiAgICAgIH0sXG4gICAgfTtcbiAgfVxuXG4gIC8qKlxuICAgKiBDYWxsZWQgYWZ0ZXIgdGhlIENGTiBmdW5jdGlvbiByZXNvdXJjZSBoYXMgYmVlbiBjcmVhdGVkIHRvIGFsbG93IHRoZSBjb2RlIGNsYXNzIHRvIGJpbmQgdG8gaXQuXG4gICAqXG4gICAqIFNwZWNpZmljYWxseSBpdCdzIHJlcXVpcmVkIHRvIGFsbG93IGFzc2V0cyB0byBhZGRcbiAgICogbWV0YWRhdGEgZm9yIHRvb2xpbmcgbGlrZSBTQU0gQ0xJIHRvIGJlIGFibGUgdG8gZmluZCB0aGVpciBvcmlnaW5zLlxuICAgKlxuICAgKiBAc3RhYmlsaXR5IHN0YWJsZVxuICAgKi9cbiAgYmluZFRvUmVzb3VyY2UocmVzb3VyY2U6IENmblJlc291cmNlLCBvcHRpb25zPzogUmVzb3VyY2VCaW5kT3B0aW9ucykge1xuICAgIGlmICghdGhpcy5hc3NldCkge1xuICAgICAgdGhyb3cgbmV3IEVycm9yKCdiaW5kVG9SZXNvdXJjZSgpIG11c3QgYmUgY2FsbGVkIGFmdGVyIGJpbmQoKScpO1xuICAgIH1cbiAgICBjb25zdCByZXNvdXJjZVByb3BlcnR5ID0gb3B0aW9ucz8ucmVzb3VyY2VQcm9wZXJ0eSB8fCB0aGlzLmNvbnN0cnVjdG9yLm5hbWU7XG4gICAgLy8gaHR0cHM6Ly9naXRodWIuY29tL2F3cy9hd3MtY2RrL2lzc3Vlcy8xNDMyXG4gICAgdGhpcy5hc3NldC5hZGRSZXNvdXJjZU1ldGFkYXRhKHJlc291cmNlLCByZXNvdXJjZVByb3BlcnR5KTtcbiAgfVxufVxuXG4vKipcbiAqIFJlcHJlc2VudHMgdGhlIGRlcGxveWVkIEphdmFTY3JpcHQgQ29kZS5cbiAqXG4gKiBAc3RhYmlsaXR5IHN0YWJsZVxuICovXG5leHBvcnQgY2xhc3MgSmF2YVNjcmlwdENvZGUgZXh0ZW5kcyBFc2J1aWxkQ29kZTxKYXZhU2NyaXB0Q29kZVByb3BzPiB7XG4gIHByb3RlY3RlZCBnZXRBc3NldChzY29wZTogQ29uc3RydWN0KTogRXNidWlsZEFzc2V0PEFzc2V0UHJvcHM+IHtcbiAgICByZXR1cm4gbmV3IEpTQXNzZXQoXG4gICAgICBzY29wZSxcbiAgICAgIHRoaXMuY29uc3RydWN0b3IubmFtZSxcbiAgICAgIHRoaXMucHJvcHMsXG4gICAgKTtcbiAgfVxuXG4gIGNvbnN0cnVjdG9yKFxuICAgIC8qKlxuICAgICAqIEEgcGF0aCBvciBsaXN0IG9yIG1hcCBvZiBwYXRocyB0byB0aGUgZW50cnkgcG9pbnRzIG9mIHlvdXIgY29kZS5cbiAgICAgKlxuICAgICAqIFJlbGF0aXZlIHBhdGhzIGFyZSBieSBkZWZhdWx0IHJlc29sdmVkIGZyb20gdGhlIGN1cnJlbnQgd29ya2luZyBkaXJlY3RvcnkuXG4gICAgICogVG8gY2hhbmdlIHRoZSB3b3JraW5nIGRpcmVjdG9yeSwgc2VlIGBidWlsZE9wdGlvbnMuYWJzV29ya2luZ0RpcmAuXG4gICAgICpcbiAgICAgKiBBYnNvbHV0ZSBwYXRocyBjYW4gYmUgdXNlZCBpZiBmaWxlcyBhcmUgcGFydCBvZiB0aGUgd29ya2luZyBkaXJlY3RvcnkuXG4gICAgICpcbiAgICAgKiBFeGFtcGxlczpcbiAgICAgKiAgLSBgJ3NyYy9pbmRleC50cydgXG4gICAgICogIC0gYHJlcXVpcmUucmVzb2x2ZSgnLi9sYW1iZGEnKWBcbiAgICAgKiAgLSBgWydzcmMvaW5kZXgudHMnLCAnc3JjL3V0aWwudHMnXWBcbiAgICAgKiAgLSBge29uZTogJ3NyYy90d28udHMnLCB0d286ICdzcmMvb25lLnRzJ31gXG4gICAgICpcbiAgICAgKiBAc3RhYmlsaXR5IHN0YWJsZVxuICAgICAqL1xuICAgIGVudHJ5UG9pbnRzOiBFbnRyeVBvaW50cyxcblxuICAgIC8qKlxuICAgICAqIFByb3BzIHRvIGNoYW5nZSB0aGUgYmVoYXZpb3Igb2YgdGhlIGJ1bmRsZXIuXG4gICAgICpcbiAgICAgKiBEZWZhdWx0IHZhbHVlcyBmb3IgYHByb3BzLmJ1aWxkT3B0aW9uc2A6XG4gICAgICogLSBgYnVuZGxlPXRydWVgXG4gICAgICogLSBgcGxhdGZvcm09bm9kZWBcbiAgICAgKiAtIGB0YXJnZXQ9bm9kZVhgIHdpdGggWCBiZWluZyB0aGUgbWFqb3Igbm9kZSB2ZXJzaW9uIHJ1bm5pbmcgbG9jYWxseVxuICAgICAqXG4gICAgICogQHN0YWJpbGl0eSBzdGFibGVcbiAgICAgKi9cbiAgICBwcm9wczogSmF2YVNjcmlwdENvZGVQcm9wcyA9IHt9LFxuICApIHtcbiAgICBzdXBlcihlbnRyeVBvaW50cywgcHJvcHMpO1xuICB9XG59XG5cbi8qKlxuICogUmVwcmVzZW50cyB0aGUgZGVwbG95ZWQgVHlwZVNjcmlwdCBDb2RlLlxuICpcbiAqIEBzdGFiaWxpdHkgc3RhYmxlXG4gKi9cbmV4cG9ydCBjbGFzcyBUeXBlU2NyaXB0Q29kZSBleHRlbmRzIEVzYnVpbGRDb2RlPFR5cGVTY3JpcHRDb2RlUHJvcHM+IHtcbiAgcHJvdGVjdGVkIGdldEFzc2V0KHNjb3BlOiBDb25zdHJ1Y3QpOiBFc2J1aWxkQXNzZXQ8QXNzZXRQcm9wcz4ge1xuICAgIHJldHVybiBuZXcgVFNBc3NldChcbiAgICAgIHNjb3BlLFxuICAgICAgdGhpcy5jb25zdHJ1Y3Rvci5uYW1lLFxuICAgICAgdGhpcy5wcm9wcyxcbiAgICApO1xuICB9XG5cbiAgY29uc3RydWN0b3IoXG4gICAgLyoqXG4gICAgICogQSBwYXRoIG9yIGxpc3Qgb3IgbWFwIG9mIHBhdGhzIHRvIHRoZSBlbnRyeSBwb2ludHMgb2YgeW91ciBjb2RlLlxuICAgICAqXG4gICAgICogUmVsYXRpdmUgcGF0aHMgYXJlIGJ5IGRlZmF1bHQgcmVzb2x2ZWQgZnJvbSB0aGUgY3VycmVudCB3b3JraW5nIGRpcmVjdG9yeS5cbiAgICAgKiBUbyBjaGFuZ2UgdGhlIHdvcmtpbmcgZGlyZWN0b3J5LCBzZWUgYGJ1aWxkT3B0aW9ucy5hYnNXb3JraW5nRGlyYC5cbiAgICAgKlxuICAgICAqIEFic29sdXRlIHBhdGhzIGNhbiBiZSB1c2VkIGlmIGZpbGVzIGFyZSBwYXJ0IG9mIHRoZSB3b3JraW5nIGRpcmVjdG9yeS5cbiAgICAgKlxuICAgICAqIEV4YW1wbGVzOlxuICAgICAqICAtIGAnc3JjL2luZGV4LnRzJ2BcbiAgICAgKiAgLSBgcmVxdWlyZS5yZXNvbHZlKCcuL2xhbWJkYScpYFxuICAgICAqICAtIGBbJ3NyYy9pbmRleC50cycsICdzcmMvdXRpbC50cyddYFxuICAgICAqICAtIGB7b25lOiAnc3JjL3R3by50cycsIHR3bzogJ3NyYy9vbmUudHMnfWBcbiAgICAgKlxuICAgICAqIEBzdGFiaWxpdHkgc3RhYmxlXG4gICAgICovXG4gICAgZW50cnlQb2ludHM6IEVudHJ5UG9pbnRzLFxuXG4gICAgLyoqXG4gICAgICogUHJvcHMgdG8gY2hhbmdlIHRoZSBiZWhhdmlvciBvZiB0aGUgYnVuZGxlci5cbiAgICAgKlxuICAgICAqIERlZmF1bHQgdmFsdWVzIGZvciBgcHJvcHMuYnVpbGRPcHRpb25zYDpcbiAgICAgKiAtIGBidW5kbGU9dHJ1ZWBcbiAgICAgKiAtIGBwbGF0Zm9ybT1ub2RlYFxuICAgICAqIC0gYHRhcmdldD1ub2RlWGAgd2l0aCBYIGJlaW5nIHRoZSBtYWpvciBub2RlIHZlcnNpb24gcnVubmluZyBsb2NhbGx5XG4gICAgICpcbiAgICAgKiBAc3RhYmlsaXR5IHN0YWJsZVxuICAgICAqL1xuICAgIHByb3BzOiBUeXBlU2NyaXB0Q29kZVByb3BzID0ge30sXG4gICkge1xuICAgIHN1cGVyKGVudHJ5UG9pbnRzLCBwcm9wcyk7XG4gIH1cbn1cbiJdfQ==
```

##### package/lib/private/esbuild-source.js

###### js-beautify {}

```diff
@@ -54,11 +54,11 @@
         return this.dynamicPackage.auto();
     }
 }
 exports.EsbuildSource = EsbuildSource;
 _a = JSII_RTTI_SYMBOL_1;
 EsbuildSource[_a] = {
     fqn: "@mrgrain/cdk-esbuild.EsbuildSource",
-    version: "4.2.0"
+    version: "4.2.1"
 };
 EsbuildSource.dynamicPackage = dynamicEsbuild;
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiZXNidWlsZC1zb3VyY2UuanMiLCJzb3VyY2VSb290IjoiIiwic291cmNlcyI6WyIuLi8uLi9zcmMvcHJpdmF0ZS9lc2J1aWxkLXNvdXJjZS50cyJdLCJuYW1lcyI6W10sIm1hcHBpbmdzIjoiOzs7OztBQUFBLHVEQUFtRDtBQUVuRCxNQUFNLGNBQWMsR0FBRyxJQUFJLGdDQUFjLENBQUMsaUJBQWlCLENBQUMsQ0FBQztBQUVoRCxRQUFBLE9BQU8sR0FBRztJQUNyQixJQUFJLEVBQUUsY0FBYyxDQUFDLElBQUk7SUFDekIsT0FBTyxFQUFFLGNBQWMsQ0FBQyxPQUFPO0lBQy9CLElBQUksRUFBRSxjQUFjLENBQUMsSUFBSTtDQUMxQixDQUFDO0FBRUYsTUFBYSxhQUFhO0lBR3hCLGdCQUF1QixDQUFDO0lBRXhCOztPQUVHO0lBQ0ksTUFBTSxDQUFDLGVBQWU7UUFDM0IsSUFBSSxPQUFPLENBQUMsT0FBTyxDQUFDLEdBQUcsQ0FBQyxVQUFVLENBQUMsRUFBRTtZQUNuQyxPQUFPLElBQUksQ0FBQyxJQUFJLEVBQUUsQ0FBQztTQUNwQjtRQUVELE9BQU8sSUFBSSxDQUFDLE1BQU0sRUFBRSxDQUFDO0lBQ3ZCLENBQUM7SUFFRDs7T0FFRztJQUNJLE1BQU0sQ0FBQyxRQUFRO1FBQ3BCLE9BQU8sSUFBSSxDQUFDLGNBQWMsQ0FBQyxXQUFXLEVBQUUsQ0FBQztJQUMzQyxDQUFDO0lBRUQ7O09BRUc7SUFDSSxNQUFNLENBQUMsV0FBVztRQUN2QixPQUFPLElBQUksQ0FBQyxjQUFjLENBQUMsaUJBQWlCLEVBQUUsQ0FBQztJQUNqRCxDQUFDO0lBRUQ7O09BRUc7SUFDSSxNQUFNLENBQUMsTUFBTTtRQUNsQixPQUFPLElBQUksQ0FBQyxjQUFjLENBQUMsTUFBTSxFQUFFLENBQUM7SUFDdEMsQ0FBQztJQUVEOztPQUVHO0lBQ0ksTUFBTSxDQUFDLE9BQU87UUFDbkIsT0FBTyxJQUFJLENBQUMsY0FBYyxDQUFDLE9BQU8sRUFBRSxDQUFDO0lBQ3ZDLENBQUM7SUFFRDs7T0FFRztJQUNJLE1BQU0sQ0FBQyxJQUFJO1FBQ2hCLE9BQU8sSUFBSSxDQUFDLGNBQWMsQ0FBQyxJQUFJLEVBQUUsQ0FBQztJQUNwQyxDQUFDOztBQWpESCxzQ0FrREM7OztBQWpEZ0IsNEJBQWMsR0FBRyxjQUFjLENBQUMiLCJzb3VyY2VzQ29udGVudCI6WyJpbXBvcnQgeyBEeW5hbWljUGFja2FnZSB9IGZyb20gJy4vZHluYW1pYy1wYWNrYWdlJztcblxuY29uc3QgZHluYW1pY0VzYnVpbGQgPSBuZXcgRHluYW1pY1BhY2thZ2UoJ2VzYnVpbGRAXjAuMTguMCcpO1xuXG5leHBvcnQgY29uc3QgRXNidWlsZCA9IHtcbiAgbmFtZTogZHluYW1pY0VzYnVpbGQubmFtZSxcbiAgdmVyc2lvbjogZHluYW1pY0VzYnVpbGQudmVyc2lvbixcbiAgc3BlYzogZHluYW1pY0VzYnVpbGQuc3BlYyxcbn07XG5cbmV4cG9ydCBjbGFzcyBFc2J1aWxkU291cmNlIHtcbiAgcHJpdmF0ZSBzdGF0aWMgZHluYW1pY1BhY2thZ2UgPSBkeW5hbWljRXNidWlsZDtcblxuICBwcml2YXRlIGNvbnN0cnVjdG9yKCkge31cblxuICAvKipcbiAgICogYEVzYnVpbGRTb3VyY2Uubm9kZUpzKClgIGZvciBOb2RlSnMsIGBFc2J1aWxkU291cmNlLmF1dG8oKWAgZm9yIGFsbCBvdGhlciBsYW5ndWFnZXNcbiAgICovXG4gIHB1YmxpYyBzdGF0aWMgcGxhdGZvcm1EZWZhdWx0KCkge1xuICAgIGlmIChCb29sZWFuKHByb2Nlc3MuZW52LkpTSUlfQUdFTlQpKSB7XG4gICAgICByZXR1cm4gdGhpcy5hdXRvKCk7XG4gICAgfVxuXG4gICAgcmV0dXJuIHRoaXMubm9kZUpzKCk7XG4gIH1cblxuICAvKipcbiAgICogVHJ5IHRvIGZpbmQgdGhlIG1vZHVsZSBpbiBtb3N0IGNvbW1vbiBwYXRocy5cbiAgICovXG4gIHB1YmxpYyBzdGF0aWMgYW55d2hlcmUoKSB7XG4gICAgcmV0dXJuIHRoaXMuZHluYW1pY1BhY2thZ2UuZmluZEluUGF0aHMoKTtcbiAgfVxuXG4gIC8qKlxuICAgKiBUcnkgdG8gZmluZCB0aGUgbW9kdWxlIGluIGNvbW1vbiBnbG9iYWwgaW5zdGFsbGF0aW9uIHBhdGhzLlxuICAgKi9cbiAgcHVibGljIHN0YXRpYyBnbG9iYWxQYXRocygpIHtcbiAgICByZXR1cm4gdGhpcy5keW5hbWljUGFja2FnZS5maW5kSW5HbG9iYWxQYXRocygpO1xuICB9XG5cbiAgLyoqXG4gICAqIFJlcXVpcmUgbW9kdWxlIGJ5IG5hbWUsIGRvIG5vdCBhdHRlbXB0IHRvIGZpbmQgaXQgYW55d2hlcmUgZWxzZS5cbiAgICovXG4gIHB1YmxpYyBzdGF0aWMgbm9kZUpzKCkge1xuICAgIHJldHVybiB0aGlzLmR5bmFtaWNQYWNrYWdlLm5vZGVKcygpO1xuICB9XG5cbiAgLyoqXG4gICAqIEluc3RhbGwgdGhlIG1vZHVsZSB0byBhIHRlbXBvcmFyeSBsb2NhdGlvbi5cbiAgICovXG4gIHB1YmxpYyBzdGF0aWMgaW5zdGFsbCgpIHtcbiAgICByZXR1cm4gdGhpcy5keW5hbWljUGFja2FnZS5pbnN0YWxsKCk7XG4gIH1cblxuICAvKipcbiAgICogRmlyc3QgdHJ5IHRvIGZpbmQgdG8gbW9kdWxlLCB0aGVuIGluc3RhbGwgaXQgdG8gYSB0ZW1wb3JhcnkgbG9jYXRpb24uXG4gICAqL1xuICBwdWJsaWMgc3RhdGljIGF1dG8oKSB7XG4gICAgcmV0dXJuIHRoaXMuZHluYW1pY1BhY2thZ2UuYXV0bygpO1xuICB9XG59XG4iXX0=
```

##### package/lib/inline-code.js

###### js-beautify {}

```diff
@@ -81,15 +81,15 @@
         super(code, transformerProps('js', props));
     }
 }
 exports.InlineJavaScriptCode = InlineJavaScriptCode;
 _a = JSII_RTTI_SYMBOL_1;
 InlineJavaScriptCode[_a] = {
     fqn: "@mrgrain/cdk-esbuild.InlineJavaScriptCode",
-    version: "4.2.0"
+    version: "4.2.1"
 };
 /**
  * An implementation of `lambda.InlineCode` using the esbuild Transform API. Inline function code is limited to 4 KiB after transformation.
  *
  * @stability stable
  */
 class InlineTypeScriptCode extends BaseInlineCode {
@@ -115,10 +115,10 @@
         super(code, transformerProps('ts', props));
     }
 }
 exports.InlineTypeScriptCode = InlineTypeScriptCode;
 _b = JSII_RTTI_SYMBOL_1;
 InlineTypeScriptCode[_b] = {
     fqn: "@mrgrain/cdk-esbuild.InlineTypeScriptCode",
-    version: "4.2.0"
+    version: "4.2.1"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiaW5saW5lLWNvZGUuanMiLCJzb3VyY2VSb290IjoiIiwic291cmNlcyI6WyIuLi9zcmMvaW5saW5lLWNvZGUudHMiXSwibmFtZXMiOltdLCJtYXBwaW5ncyI6Ijs7Ozs7QUFBQSw2Q0FBMEM7QUFDMUMsdURBQWdFO0FBQ2hFLDJDQUE2QztBQUU3QywyQ0FBdUU7QUFDdkUseUNBQWlFO0FBMkJqRSxNQUFlLGNBQWUsU0FBUSx1QkFBVTtJQUk5QyxZQUNFLElBQVksRUFDWixLQUF1QjtRQUV2QixLQUFLLENBQUMsSUFBSSxDQUFDLENBQUM7UUFQRSxhQUFRLEdBQUcsSUFBSSxDQUFDO1FBUzlCLElBQUksQ0FBQyxVQUFVLEdBQUcsa0JBQUksQ0FBQyxNQUFNLENBQUM7WUFDNUIsT0FBTyxFQUFFLEdBQUcsRUFBRTtnQkFDWixJQUFJO29CQUNGLE1BQU0sUUFBUSxHQUFHLEtBQUssQ0FBQyxpQkFBaUIsSUFBSSwwQkFBZSxDQUFDLDZCQUE2QixFQUFFLENBQUM7b0JBRTVGLE1BQU0sZUFBZSxHQUFHLFFBQVEsQ0FBQyxhQUFhLENBQUMsSUFBSSxFQUFFO3dCQUNuRCxLQUFLLEVBQUUsT0FBTyxDQUFDLEdBQUcsQ0FBQyxRQUFRLENBQUMsQ0FBQyxDQUFDLE9BQU8sQ0FBQyxPQUFPLENBQUMsR0FBRyxDQUFDLFFBQVEsQ0FBQyxDQUFDLENBQUMsQ0FBQyxTQUFTO3dCQUN2RSxRQUFRLEVBQUUsU0FBUzt3QkFDbkIsR0FBRyxDQUFDLEtBQUssQ0FBQyxnQkFBZ0IsSUFBSSxFQUFFLENBQUM7cUJBQ2xDLENBQUMsQ0FBQztvQkFFSCxPQUFPLGVBQWUsQ0FBQztpQkFDeEI7Z0JBQUMsT0FBTyxLQUFLLEVBQUU7b0JBQ2QsSUFBSSxzQkFBYyxDQUFDLEtBQUssQ0FBQyxFQUFFO3dCQUN6QixNQUFNLElBQUksS0FBSyxDQUFDLCtCQUErQixJQUFJLENBQUMsV0FBVyxDQUFDLElBQUksRUFBRSxDQUFDLENBQUM7cUJBQ3pFO29CQUNELE1BQU0sS0FBSyxDQUFDO2lCQUNiO1lBQ0gsQ0FBQztTQUNGLENBQUMsQ0FBQztJQUNMLENBQUM7SUFFTSxJQUFJLENBQUMsS0FBZ0I7UUFDMUIsTUFBTSxJQUFJLEdBQUcsS0FBSyxDQUFDLElBQUksQ0FBQyxJQUFJLEdBQUcsaUJBQUksQ0FBQyxRQUFRLEdBQUcsSUFBSSxDQUFDLFdBQVcsQ0FBQyxJQUFJLENBQUM7UUFDckUsT0FBTyxDQUFDLE1BQU0sQ0FBQyxLQUFLLENBQUMsNEJBQTRCLElBQUksT0FBTyxDQUFDLENBQUM7UUFFOUQsT0FBTztZQUNMLFVBQVUsRUFBRSxtQkFBSyxDQUFDLEVBQUUsQ0FBQyxLQUFLLENBQUMsQ0FBQyxPQUFPLENBQUMsSUFBSSxDQUFDLFVBQVUsQ0FBQztTQUNyRCxDQUFDO0lBQ0osQ0FBQztDQUNGO0FBRUQsU0FBUyxnQkFBZ0IsQ0FBQyxNQUFjLEVBQUUsUUFBMEIsRUFBRTtJQUNwRSxPQUFPO1FBQ0wsR0FBRyxLQUFLO1FBQ1IsZ0JBQWdCLEVBQUU7WUFDaEIsTUFBTTtZQUNOLE1BQU0sRUFBRSxLQUFLO1lBQ2IsR0FBRyw0QkFBb0IsQ0FBQyxLQUFLLENBQUMsZ0JBQWdCLENBQUM7WUFDL0MsR0FBRyxLQUFLLENBQUMsZ0JBQWdCO1NBQzFCO0tBQ0YsQ0FBQztBQUNKLENBQUM7QUFFRDs7OztHQUlHO0FBQ0gsTUFBYSxvQkFBcUIsU0FBUSxjQUFjO0lBQ3REO0lBQ0U7Ozs7T0FJRztJQUNILElBQVk7SUFDWjs7Ozs7Ozs7OztPQVVHO0lBQ0gsS0FBd0I7UUFFeEIsS0FBSyxDQUFDLElBQUksRUFBRSxnQkFBZ0IsQ0FBQyxJQUFJLEVBQUUsS0FBSyxDQUFDLENBQUMsQ0FBQztJQUM3QyxDQUFDOztBQXRCSCxvREF1QkM7OztBQUdEOzs7O0dBSUc7QUFDSCxNQUFhLG9CQUFxQixTQUFRLGNBQWM7SUFDdEQ7SUFDRTs7OztPQUlHO0lBQ0gsSUFBWTtJQUNaOzs7Ozs7Ozs7O09BVUc7SUFDSCxLQUF3QjtRQUV4QixLQUFLLENBQUMsSUFBSSxFQUFFLGdCQUFnQixDQUFDLElBQUksRUFBRSxLQUFLLENBQUMsQ0FBQyxDQUFDO0lBQzdDLENBQUM7O0FBdEJILG9EQXVCQyIsInNvdXJjZXNDb250ZW50IjpbImltcG9ydCB7IExhenksIFN0YWNrIH0gZnJvbSAnYXdzLWNkay1saWInO1xuaW1wb3J0IHsgQ29kZUNvbmZpZywgSW5saW5lQ29kZSB9IGZyb20gJ2F3cy1jZGstbGliL2F3cy1sYW1iZGEnO1xuaW1wb3J0IHsgQ29uc3RydWN0LCBOb2RlIH0gZnJvbSAnY29uc3RydWN0cyc7XG5pbXBvcnQgeyBUcmFuc2Zvcm1PcHRpb25zLCBMb2FkZXIgfSBmcm9tICcuL2VzYnVpbGQtdHlwZXMnO1xuaW1wb3J0IHsgZGVmYXVsdFBsYXRmb3JtUHJvcHMsIGlzRXNidWlsZEVycm9yIH0gZnJvbSAnLi9wcml2YXRlL3V0aWxzJztcbmltcG9ydCB7IEVzYnVpbGRQcm92aWRlciwgSVRyYW5zZm9ybVByb3ZpZGVyIH0gZnJvbSAnLi9wcm92aWRlcic7XG5cbi8qKlxuICogQHN0YWJpbGl0eSBzdGFibGVcbiAqL1xuZXhwb3J0IGludGVyZmFjZSBUcmFuc2Zvcm1lclByb3BzIHtcbiAgLyoqXG4gICAqIFRyYW5zZm9ybSBvcHRpb25zIHBhc3NlZCBvbiB0byBlc2J1aWxkLiBQbGVhc2UgcmVmZXIgdG8gdGhlIGVzYnVpbGQgVHJhbnNmb3JtIEFQSSBkb2NzIGZvciBkZXRhaWxzLlxuICAgKlxuICAgKiBAc2VlIGh0dHBzOi8vZXNidWlsZC5naXRodWIuaW8vYXBpLyN0cmFuc2Zvcm0tYXBpXG4gICAqIEBzdGFiaWxpdHkgc3RhYmxlXG4gICAqL1xuICByZWFkb25seSB0cmFuc2Zvcm1PcHRpb25zPzogVHJhbnNmb3JtT3B0aW9ucztcblxuICAvKipcbiAgICogVGhlIGVzYnVpbGQgVHJhbnNmb3JtIEFQSSBpbXBsZW1lbnRhdGlvbiB0byBiZSB1c2VkLlxuICAgKlxuICAgKiBDb25maWd1cmUgdGhlIGRlZmF1bHQgYEVzYnVpbGRQcm92aWRlcmAgZm9yIG1vcmUgb3B0aW9ucyBvclxuICAgKiBwcm92aWRlIGEgY3VzdG9tIGBJVHJhbnNmb3JtUHJvdmlkZXJgIGFzIGFuIGVzY2FwZSBoYXRjaC5cbiAgICpcbiAgICogQHN0YWJpbGl0eSBzdGFibGVcbiAgICpcbiAgICogQGRlZmF1bHQgbmV3IERlZmF1bHRFc2J1aWxkUHJvdmlkZXIoKVxuICAgKi9cbiAgcmVhZG9ubHkgdHJhbnNmb3JtUHJvdmlkZXI/OiBJVHJhbnNmb3JtUHJvdmlkZXI7XG59XG5cbmFic3RyYWN0IGNsYXNzIEJhc2VJbmxpbmVDb2RlIGV4dGVuZHMgSW5saW5lQ29kZSB7XG4gIHB1YmxpYyByZWFkb25seSBpc0lubGluZSA9IHRydWU7XG4gIHByaXZhdGUgcmVhZG9ubHkgaW5saW5lQ29kZTogc3RyaW5nO1xuXG4gIHB1YmxpYyBjb25zdHJ1Y3RvcihcbiAgICBjb2RlOiBzdHJpbmcsXG4gICAgcHJvcHM6IFRyYW5zZm9ybWVyUHJvcHMsXG4gICkge1xuICAgIHN1cGVyKGNvZGUpO1xuXG4gICAgdGhpcy5pbmxpbmVDb2RlID0gTGF6eS5zdHJpbmcoe1xuICAgICAgcHJvZHVjZTogKCkgPT4ge1xuICAgICAgICB0cnkge1xuICAgICAgICAgIGNvbnN0IHByb3ZpZGVyID0gcHJvcHMudHJhbnNmb3JtUHJvdmlkZXIgPz8gRXNidWlsZFByb3ZpZGVyLmRlZmF1bHRUcmFuc2Zvcm1hdGlvblByb3ZpZGVyKCk7XG5cbiAgICAgICAgICBjb25zdCB0cmFuc2Zvcm1lZENvZGUgPSBwcm92aWRlci50cmFuc2Zvcm1TeW5jKGNvZGUsIHtcbiAgICAgICAgICAgIGNvbG9yOiBwcm9jZXNzLmVudi5OT19DT0xPUiA/IEJvb2xlYW4ocHJvY2Vzcy5lbnYuTk9fQ09MT1IpIDogdW5kZWZpbmVkLFxuICAgICAgICAgICAgbG9nTGV2ZWw6ICd3YXJuaW5nJyxcbiAgICAgICAgICAgIC4uLihwcm9wcy50cmFuc2Zvcm1PcHRpb25zIHx8IHt9KSxcbiAgICAgICAgICB9KTtcblxuICAgICAgICAgIHJldHVybiB0cmFuc2Zvcm1lZENvZGU7XG4gICAgICAgIH0gY2F0Y2ggKGVycm9yKSB7XG4gICAgICAgICAgaWYgKGlzRXNidWlsZEVycm9yKGVycm9yKSkge1xuICAgICAgICAgICAgdGhyb3cgbmV3IEVycm9yKGBFc2J1aWxkIGZhaWxlZCB0byB0cmFuc2Zvcm0gJHt0aGlzLmNvbnN0cnVjdG9yLm5hbWV9YCk7XG4gICAgICAgICAgfVxuICAgICAgICAgIHRocm93IGVycm9yO1xuICAgICAgICB9XG4gICAgICB9LFxuICAgIH0pO1xuICB9XG5cbiAgcHVibGljIGJpbmQoc2NvcGU6IENvbnN0cnVjdCk6IENvZGVDb25maWcge1xuICAgIGNvbnN0IG5hbWUgPSBzY29wZS5ub2RlLnBhdGggKyBOb2RlLlBBVEhfU0VQICsgdGhpcy5jb25zdHJ1Y3Rvci5uYW1lO1xuICAgIHByb2Nlc3Muc3RkZXJyLndyaXRlKGBUcmFuc2Zvcm1pbmcgaW5saW5lIGNvZGUgJHtuYW1lfS4uLlxcbmApO1xuXG4gICAgcmV0dXJuIHtcbiAgICAgIGlubGluZUNvZGU6IFN0YWNrLm9mKHNjb3BlKS5yZXNvbHZlKHRoaXMuaW5saW5lQ29kZSksXG4gICAgfTtcbiAgfVxufVxuXG5mdW5jdGlvbiB0cmFuc2Zvcm1lclByb3BzKGxvYWRlcjogTG9hZGVyLCBwcm9wczogVHJhbnNmb3JtZXJQcm9wcyA9IHt9KTogVHJhbnNmb3JtZXJQcm9wcyB7XG4gIHJldHVybiB7XG4gICAgLi4ucHJvcHMsXG4gICAgdHJhbnNmb3JtT3B0aW9uczoge1xuICAgICAgbG9hZGVyLFxuICAgICAgZm9ybWF0OiAnY2pzJyxcbiAgICAgIC4uLmRlZmF1bHRQbGF0Zm9ybVByb3BzKHByb3BzLnRyYW5zZm9ybU9wdGlvbnMpLFxuICAgICAgLi4ucHJvcHMudHJhbnNmb3JtT3B0aW9ucyxcbiAgICB9LFxuICB9O1xufVxuXG4vKipcbiAqIEFuIGltcGxlbWVudGF0aW9uIG9mIGBsYW1iZGEuSW5saW5lQ29kZWAgdXNpbmcgdGhlIGVzYnVpbGQgVHJhbnNmb3JtIEFQSS4gSW5saW5lIGZ1bmN0aW9uIGNvZGUgaXMgbGltaXRlZCB0byA0IEtpQiBhZnRlciB0cmFuc2Zvcm1hdGlvbi5cbiAqXG4gKiBAc3RhYmlsaXR5IHN0YWJsZVxuICovXG5leHBvcnQgY2xhc3MgSW5saW5lSmF2YVNjcmlwdENvZGUgZXh0ZW5kcyBCYXNlSW5saW5lQ29kZSB7XG4gIHB1YmxpYyBjb25zdHJ1Y3RvcihcbiAgICAvKipcbiAgICAgKiBUaGUgaW5saW5lIGNvZGUgdG8gYmUgdHJhbnNmb3JtZWQuXG4gICAgICpcbiAgICAgKiBAc3RhYmlsaXR5IHN0YWJsZVxuICAgICAqL1xuICAgIGNvZGU6IHN0cmluZyxcbiAgICAvKipcbiAgICAgKiBQcm9wcyB0byBjaGFuZ2UgdGhlIGJlaGF2aW9yIG9mIHRoZSB0cmFuc2Zvcm1lci5cbiAgICAgKlxuICAgICAqIERlZmF1bHQgdmFsdWVzIGZvciBgcHJvcHMudHJhbnNmb3JtT3B0aW9uc2A6XG4gICAgICogLSBgbG9hZGVyPSdqcydgXG4gICAgICogLSBgcGxhdGZvcm09bm9kZWBcbiAgICAgKiAtIGB0YXJnZXQ9bm9kZVhgIHdpdGggWCBiZWluZyB0aGUgbWFqb3Igbm9kZSB2ZXJzaW9uIHJ1bm5pbmcgbG9jYWxseVxuICAgICAqXG4gICAgICogQHNlZSBodHRwczovL2VzYnVpbGQuZ2l0aHViLmlvL2FwaS8jdHJhbnNmb3JtLWFwaVxuICAgICAqIEBzdGFiaWxpdHkgc3RhYmxlXG4gICAgICovXG4gICAgcHJvcHM/OiBUcmFuc2Zvcm1lclByb3BzLFxuICApIHtcbiAgICBzdXBlcihjb2RlLCB0cmFuc2Zvcm1lclByb3BzKCdqcycsIHByb3BzKSk7XG4gIH1cbn1cblxuXG4vKipcbiAqIEFuIGltcGxlbWVudGF0aW9uIG9mIGBsYW1iZGEuSW5saW5lQ29kZWAgdXNpbmcgdGhlIGVzYnVpbGQgVHJhbnNmb3JtIEFQSS4gSW5saW5lIGZ1bmN0aW9uIGNvZGUgaXMgbGltaXRlZCB0byA0IEtpQiBhZnRlciB0cmFuc2Zvcm1hdGlvbi5cbiAqXG4gKiBAc3RhYmlsaXR5IHN0YWJsZVxuICovXG5leHBvcnQgY2xhc3MgSW5saW5lVHlwZVNjcmlwdENvZGUgZXh0ZW5kcyBCYXNlSW5saW5lQ29kZSB7XG4gIHB1YmxpYyBjb25zdHJ1Y3RvcihcbiAgICAvKipcbiAgICAgKiBUaGUgaW5saW5lIGNvZGUgdG8gYmUgdHJhbnNmb3JtZWQuXG4gICAgICpcbiAgICAgKiBAc3RhYmlsaXR5IHN0YWJsZVxuICAgICAqL1xuICAgIGNvZGU6IHN0cmluZyxcbiAgICAvKipcbiAgICAgKiBQcm9wcyB0byBjaGFuZ2UgdGhlIGJlaGF2aW9yIG9mIHRoZSB0cmFuc2Zvcm1lci5cbiAgICAgKlxuICAgICAqIERlZmF1bHQgdmFsdWVzIGZvciBgdHJhbnNmb3JtT3B0aW9uc2A6XG4gICAgICogLSBgbG9hZGVyPSd0cydgXG4gICAgICogLSBgcGxhdGZvcm09bm9kZWBcbiAgICAgKiAtIGB0YXJnZXQ9bm9kZVhgIHdpdGggWCBiZWluZyB0aGUgbWFqb3Igbm9kZSB2ZXJzaW9uIHJ1bm5pbmcgbG9jYWxseVxuICAgICAqXG4gICAgICogQHNlZSBodHRwczovL2VzYnVpbGQuZ2l0aHViLmlvL2FwaS8jdHJhbnNmb3JtLWFwaVxuICAgICAqIEBzdGFiaWxpdHkgc3RhYmxlXG4gICAgICovXG4gICAgcHJvcHM/OiBUcmFuc2Zvcm1lclByb3BzLFxuICApIHtcbiAgICBzdXBlcihjb2RlLCB0cmFuc2Zvcm1lclByb3BzKCd0cycsIHByb3BzKSk7XG4gIH1cbn1cbiJdfQ==
```

##### package/lib/provider.js

###### js-beautify {}

```diff
@@ -115,11 +115,11 @@
         });
     }
 }
 exports.EsbuildProvider = EsbuildProvider;
 _a = JSII_RTTI_SYMBOL_1;
 EsbuildProvider[_a] = {
     fqn: "@mrgrain/cdk-esbuild.EsbuildProvider",
-    version: "4.2.0"
+    version: "4.2.1"
 };
 EsbuildProvider._fallbackProvider = new EsbuildProvider();
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoicHJvdmlkZXIuanMiLCJzb3VyY2VSb290IjoiIiwic291cmNlcyI6WyIuLi9zcmMvcHJvdmlkZXIudHMiXSwibmFtZXMiOltdLCJtYXBwaW5ncyI6Ijs7Ozs7QUFBQSw2Q0FBc0Y7QUFDdEYsMkNBQXVDO0FBRXZDLDZEQUFrRTtBQUVsRSwyREFBeUQ7QUFBaEQsK0dBQUEsYUFBYSxPQUFBO0FBc0Z0Qjs7R0FFRztBQUNILE1BQWEsZUFBZTtJQTRDMUIsWUFBbUIsUUFBOEIsRUFBRTtRQUNqRCxJQUFJLENBQUMsaUJBQWlCLEdBQUcsS0FBSyxDQUFDLGlCQUFpQixDQUFDO1FBQ2pELElBQUksQ0FBQyxpQkFBaUIsR0FBRyxLQUFLLENBQUMsaUJBQWlCLENBQUM7SUFDbkQsQ0FBQztJQTFDRDs7T0FFRztJQUNJLE1BQU0sQ0FBQyx1QkFBdUIsQ0FBQyxRQUEwQjtRQUM5RCxJQUFJLENBQUMsNEJBQTRCLENBQUMsUUFBUSxDQUFDLENBQUM7UUFDNUMsSUFBSSxDQUFDLHFDQUFxQyxDQUFDLFFBQVEsQ0FBQyxDQUFDO0lBQ3ZELENBQUM7SUFFRDs7T0FFRztJQUNJLE1BQU0sQ0FBQyw0QkFBNEIsQ0FBQyxRQUF3QjtRQUNqRSxJQUFJLENBQUMsY0FBYyxHQUFHLFFBQVEsQ0FBQztJQUNqQyxDQUFDO0lBRUQ7O09BRUc7SUFDSSxNQUFNLENBQUMsb0JBQW9CO1FBQ2hDLE9BQU8sSUFBSSxDQUFDLGNBQWMsSUFBSSxJQUFJLENBQUMsaUJBQWlCLENBQUM7SUFDdkQsQ0FBQztJQUVEOztPQUVHO0lBQ0ksTUFBTSxDQUFDLHFDQUFxQyxDQUFDLFFBQTRCO1FBQzlFLElBQUksQ0FBQyx1QkFBdUIsR0FBRyxRQUFRLENBQUM7SUFDMUMsQ0FBQztJQUVEOztPQUVHO0lBQ0ksTUFBTSxDQUFDLDZCQUE2QjtRQUN6QyxPQUFPLElBQUksQ0FBQyx1QkFBdUIsSUFBSSxJQUFJLENBQUMsaUJBQWlCLENBQUM7SUFDaEUsQ0FBQztJQVVNLFNBQVMsQ0FBQyxPQUE2QjtRQUM1QyxNQUFNLE9BQU8sR0FBRyxJQUFJLENBQUMsT0FBTyxDQUFDLElBQUksQ0FBQyxpQkFBaUIsQ0FBQyxDQUFDO1FBQ3JELE1BQU0sT0FBTyxHQUFHLElBQUksQ0FBQyxxQkFBcUIsQ0FBQyxPQUFPLENBQUMsU0FBUyxFQUFFLElBQUksQ0FBQyxpQkFBaUIsQ0FBQyxDQUFDO1FBRXRGLE9BQU8sQ0FBQyxPQUFPLENBQUMsQ0FBQztJQUNuQixDQUFDO0lBRU0sYUFBYSxDQUFDLEtBQWEsRUFBRSxPQUFrQztRQUNwRSxNQUFNLE9BQU8sR0FBRyxJQUFJLENBQUMsT0FBTyxDQUFDLElBQUksQ0FBQyxpQkFBaUIsQ0FBQyxDQUFDO1FBQ3JELE1BQU0sV0FBVyxHQUFHLElBQUksQ0FBQyxxQkFBcUIsQ0FBQyxPQUFPLENBQUMsYUFBYSxFQUFFLElBQUksQ0FBQyxpQkFBaUIsQ0FBQyxDQUFDO1FBRTlGLE9BQU8sV0FBVyxDQUFDLEtBQUssRUFBRSxPQUFPLENBQUMsQ0FBQyxJQUFJLENBQUM7SUFDMUMsQ0FBQztJQUVEOzs7T0FHRztJQUNLLHFCQUFxQixDQUE2QixFQUFLLEVBQUUsaUJBQTBCO1FBQ3pGLElBQUksQ0FBQyxpQkFBaUIsRUFBRTtZQUN0QixPQUFPLEVBQUUsQ0FBQztTQUNYO1FBRUQsT0FBTyxDQUFDLEdBQUcsSUFBZSxFQUFFLEVBQUU7WUFDNUIsTUFBTSx5QkFBeUIsR0FBRyxPQUFPLENBQUMsR0FBRyxDQUFDLG1CQUFtQixDQUFDO1lBQ2xFLElBQUksaUJBQWlCLEVBQUU7Z0JBQ3JCLE9BQU8sQ0FBQyxHQUFHLENBQUMsbUJBQW1CLEdBQUcsaUJBQWlCLENBQUM7YUFDckQ7WUFFRCxNQUFNLE1BQU0sR0FBRyxFQUFFLENBQUMsR0FBRyxJQUFJLENBQUMsQ0FBQztZQUUzQjs7O2VBR0c7WUFDSCxJQUFJLGlCQUFpQixFQUFFO2dCQUNyQixPQUFPLENBQUMsR0FBRyxDQUFDLG1CQUFtQixHQUFHLHlCQUF5QixDQUFDO2FBQzdEO1lBRUQsT0FBTyxNQUFNLENBQUM7UUFDaEIsQ0FBQyxDQUFDO0lBQ0osQ0FBQztJQUVEOztPQUVHO0lBQ0ssT0FBTyxDQUFDLElBQWE7UUFDM0IsTUFBTSxNQUFNLEdBQUcsSUFBSSxJQUFJLE9BQU8sQ0FBQyxHQUFHLENBQUMsdUJBQXVCLElBQUksOEJBQWEsQ0FBQyxlQUFlLEVBQUUsSUFBSSx3QkFBTyxDQUFDLElBQUksQ0FBQztRQUU5RyxPQUFPLElBQUksQ0FBQyxRQUFRLENBQUMsSUFBSSxDQUFDLE9BQU8sQ0FBQyxNQUFNLENBQUMsQ0FBQyxDQUFDO0lBQzdDLENBQUM7SUFFRDs7T0FFRztJQUNLLFFBQVEsQ0FBQyxJQUFZO1FBQzNCLGlFQUFpRTtRQUNqRSxPQUFPLE9BQU8sQ0FBQyxJQUFJLENBQUMsQ0FBQztJQUN2QixDQUFDO0lBRUQ7O09BRUc7SUFDSyxPQUFPLENBQUMsS0FBYTtRQUMzQixJQUFJLENBQUMsbUJBQUssQ0FBQyxZQUFZLENBQUMsS0FBSyxDQUFDLEVBQUU7WUFDOUIsT0FBTyxLQUFLLENBQUM7U0FDZDtRQUVELE9BQU8sMEJBQVksQ0FBQyxPQUFPLENBQUMsS0FBSyxFQUFFO1lBQ2pDLEtBQUssRUFBRSxJQUFJLHNCQUFTLENBQUMsU0FBZ0IsRUFBRSxFQUFFLENBQUM7WUFDMUMsUUFBUSxFQUFFLElBQUksa0NBQW9CLENBQUMsSUFBSSwwQkFBWSxFQUFFLENBQUM7U0FDdkQsQ0FBQyxDQUFDO0lBQ0wsQ0FBQzs7QUF6SEgsMENBMEhDOzs7QUF6SGdCLGlDQUFpQixHQUFHLElBQUksZUFBZSxFQUFFLENBQUMiLCJzb3VyY2VzQ29udGVudCI6WyJpbXBvcnQgeyBEZWZhdWx0VG9rZW5SZXNvbHZlciwgU3RyaW5nQ29uY2F0LCBUb2tlbiwgVG9rZW5pemF0aW9uIH0gZnJvbSAnYXdzLWNkay1saWInO1xuaW1wb3J0IHsgQ29uc3RydWN0IH0gZnJvbSAnY29uc3RydWN0cyc7XG5pbXBvcnQgeyBCdWlsZE9wdGlvbnMsIFRyYW5zZm9ybU9wdGlvbnMgfSBmcm9tICcuL2VzYnVpbGQtdHlwZXMnO1xuaW1wb3J0IHsgRXNidWlsZCwgRXNidWlsZFNvdXJjZSB9IGZyb20gJy4vcHJpdmF0ZS9lc2J1aWxkLXNvdXJjZSc7XG5cbmV4cG9ydCB7IEVzYnVpbGRTb3VyY2UgfSBmcm9tICcuL3ByaXZhdGUvZXNidWlsZC1zb3VyY2UnO1xuXG5cbmV4cG9ydCBpbnRlcmZhY2UgUHJvdmlkZXJCdWlsZE9wdGlvbnMgZXh0ZW5kcyBCdWlsZE9wdGlvbnMge1xuICAvKiogRG9jdW1lbnRhdGlvbjogaHR0cHM6Ly9lc2J1aWxkLmdpdGh1Yi5pby9hcGkvI2VudHJ5LXBvaW50cyAqL1xuICByZWFkb25seSBlbnRyeVBvaW50cz86IHN0cmluZ1tdIHwgUmVjb3JkPHN0cmluZywgc3RyaW5nPjtcbn1cblxuZXhwb3J0IGludGVyZmFjZSBQcm92aWRlclRyYW5zZm9ybU9wdGlvbnMgZXh0ZW5kcyBUcmFuc2Zvcm1PcHRpb25zIHt9XG5cblxuLyoqXG4gKiBQcm92aWRlcyBhbiBpbXBsZW1lbnRhdGlvbiBvZiB0aGUgZXNidWlsZCBCdWlsZCBBUElcbiAqL1xuZXhwb3J0IGludGVyZmFjZSBJQnVpbGRQcm92aWRlciB7XG4gIC8qKlxuICAgKiBBIG1ldGhvZCBpbXBsZW1lbnRpbmcgdGhlIGNvZGUgYnVpbGQuXG4gICAqXG4gICAqIER1cmluZyBzeW50aCB0aW1lLCB0aGUgbWV0aG9kIHdpbGwgcmVjZWl2ZSBhbGwgY29tcHV0ZWQgYEJ1aWxkT3B0aW9uc2AgZnJvbSB0aGUgYnVuZGxlci5cbiAgICpcbiAgICogSXQgTVVTVCBpbXBsZW1lbnQgYW55IG91dHB1dCBvcHRpb25zIHRvIGludGVncmF0ZSBjb3JyZWN0bHkgYW5kIE1BWSB1c2UgYW55IG90aGVyIG9wdGlvbnMuXG4gICAqIE9uIGZhaWx1cmUsIGl0IFNIT1VMRCBwcmludCBhbnkgd2FybmluZ3MgJiBlcnJvcnMgdG8gc3RkZXJyIGFuZCB0aHJvdyBhIGBCdWlsZEZhaWx1cmVgIHRvIGluZm9ybSB0aGUgYnVuZGxlci5cbiAgICpcbiAgICogQHRocm93cyBgZXNidWlsZC5CdWlsZEZhaWx1cmVgXG4gICAqL1xuICBidWlsZFN5bmMob3B0aW9uczogUHJvdmlkZXJCdWlsZE9wdGlvbnMpOiB2b2lkO1xufVxuXG4vKipcbiAqIFByb3ZpZGVzIGFuIGltcGxlbWVudGF0aW9uIG9mIHRoZSBlc2J1aWxkIFRyYW5zZm9ybSBBUElcbiAqL1xuZXhwb3J0IGludGVyZmFjZSBJVHJhbnNmb3JtUHJvdmlkZXIge1xuICAvKipcbiAgICogQSBtZXRob2QgaW1wbGVtZW50aW5nIHRoZSBpbmxpbmUgY29kZSB0cmFuc2Zvcm1hdGlvbi5cbiAgICpcbiAgICogRHVyaW5nIHN5bnRoIHRpbWUsIHRoZSBtZXRob2Qgd2lsbCByZWNlaXZlIHRoZSBpbmxpbmUgY29kZSBhbmQgYWxsIGNvbXB1dGVkIGBUcmFuc2Zvcm1PcHRpb25zYCBmcm9tIHRoZSBidW5kbGVyLlxuICAgKlxuICAgKiBNVVNUIHJldHVybiB0aGUgdHJhbnNmb3JtZWQgY29kZSBhcyBhIHN0cmluZyB0byBpbnRlZ3JhdGUgY29ycmVjdGx5LlxuICAgKiBJdCBNQVkgdXNlIHRoZXNlIG9wdGlvbnMgdG8gZG8gc28uXG4gICAqIE9uIGZhaWx1cmUsIGl0IFNIT1VMRCBwcmludCBhbnkgd2FybmluZ3MgJiBlcnJvcnMgdG8gc3RkZXJyIGFuZCB0aHJvdyBhIGBUcmFuc2Zvcm1GYWlsdXJlYCB0byBpbmZvcm0gdGhlIGJ1bmRsZXIuXG4gICAqXG4gICAqIEB0aHJvd3MgYGVzYnVpbGQuVHJhbnNmb3JtRmFpbHVyZWBcbiAgICovXG4gIHRyYW5zZm9ybVN5bmMoaW5wdXQ6IHN0cmluZywgb3B0aW9ucz86IFByb3ZpZGVyVHJhbnNmb3JtT3B0aW9ucyk6IHN0cmluZztcbn1cblxuLyoqXG4gKiBQcm92aWRlcyBhbiBpbXBsZW1lbnRhdGlvbiBvZiB0aGUgZXNidWlsZCBCdWlsZCAmIFRyYW5zZm9ybSBBUElcbiAqL1xuZXhwb3J0IGludGVyZmFjZSBJRXNidWlsZFByb3ZpZGVyIGV4dGVuZHMgSUJ1aWxkUHJvdmlkZXIsIElUcmFuc2Zvcm1Qcm92aWRlciB7fVxuXG4vKipcbiAqIENvbmZpZ3VyZSB0aGUgZGVmYXVsdCBFc2J1aWxkUHJvdmlkZXJcbiAqL1xuZXhwb3J0IGludGVyZmFjZSBFc2J1aWxkUHJvdmlkZXJQcm9wcyB7XG4gIC8qKlxuICAgKiBQYXRoIHRvIHRoZSBiaW5hcnkgdXNlZCBieSBlc2J1aWxkLlxuICAgKlxuICAgKiBUaGlzIGlzIHRoZSBzYW1lIGFzIHNldHRpbmcgdGhlIEVTQlVJTERfQklOQVJZX1BBVEggZW52aXJvbm1lbnQgdmFyaWFibGUuXG4gICAqXG4gICAqIEBzdGFiaWxpdHkgc3RhYmxlXG4gICAqL1xuICByZWFkb25seSBlc2J1aWxkQmluYXJ5UGF0aD86IHN0cmluZztcblxuICAvKipcbiAgICogQWJzb2x1dGUgcGF0aCB0byB0aGUgZXNidWlsZCBtb2R1bGUgSlMgZmlsZS5cbiAgICpcbiAgICogRS5nLiBcIi9ob21lL3VzZXIvLm5wbS9ub2RlX21vZHVsZXMvZXNidWlsZC9saWIvbWFpbi5qc1wiXG4gICAqXG4gICAqIElmIG5vdCBzZXQsIHRoZSBtb2R1bGUgcGF0aCB3aWxsIGJlIGRldGVybWluZWQgaW4gdGhlIGZvbGxvd2luZyBvcmRlcjpcbiAgICpcbiAgICogLSBVc2UgYSBwYXRoIGZyb20gdGhlIGBDREtfRVNCVUlMRF9NT0RVTEVfUEFUSGAgZW52aXJvbm1lbnQgdmFyaWFibGVcbiAgICogLSBJbiBUeXBlU2NyaXB0LCBmYWxsYmFjayB0byB0aGUgZGVmYXVsdCBOb2RlLmpzIHBhY2thZ2UgcmVzb2x1dGlvbiBtZWNoYW5pc21cbiAgICogLSBBbGwgb3RoZXIgbGFuZ3VhZ2VzIChQeXRob24sIEdvLCAuTkVULCBKYXZhKSB1c2UgYW4gYXV0b21hdGljIFwiYmVzdCBlZmZvcnRcIiByZXNvbHV0aW9uIG1lY2hhbmlzbS4gXFxcbiAgICogICBUaGUgZXhhY3QgYWxnb3JpdGhtIG9mIHRoaXMgbWVjaGFuaXNtIGlzIGNvbnNpZGVyZWQgYW4gaW1wbGVtZW50YXRpb24gZGV0YWlsIGFuZCBzaG91bGQgbm90IGJlIHJlbGllZCBvbi5cbiAgICogICBJZiBgZXNidWlsZGAgY2Fubm90IGJlIGZvdW5kLCBpdCBtaWdodCBiZSBpbnN0YWxsZWQgZHluYW1pY2FsbHkgdG8gYSB0ZW1wb3JhcnkgbG9jYXRpb24uXG4gICAqICAgVG8gb3B0LW91dCBvZiB0aGlzIGJlaGF2aW9yLCBzZXQgZWl0aGVyIGBlc2J1aWxkTW9kdWxlUGF0aGAgb3IgYENES19FU0JVSUxEX01PRFVMRV9QQVRIYCBlbnYgdmFyaWFibGUuXG4gICAqXG4gICAqIFVzZSB0aGUgc3RhdGljIG1ldGhvZHMgb24gYEVzYnVpbGRTb3VyY2VgIHRvIGN1c3RvbWl6ZSB0aGUgZGVmYXVsdCBiZWhhdmlvci5cbiAgICpcbiAgICogQHN0YWJpbGl0eSBzdGFibGVcbiAgICogQGRlZmF1bHQgLSBgQ0RLX0VTQlVJTERfTU9EVUxFX1BBVEhgIG9yIHBhY2thZ2UgcmVzb2x1dGlvbiAoc2VlIGRlc2NyaXB0aW9uKVxuICAgKi9cbiAgcmVhZG9ubHkgZXNidWlsZE1vZHVsZVBhdGg/OiBzdHJpbmc7XG59XG5cbi8qKlxuICogRGVmYXVsdCBlc2J1aWxkIGltcGxlbWVudGF0aW9uIGNhbGxpbmcgZXNidWlsZCdzIEphdmFTY3JpcHQgQVBJLlxuICovXG5leHBvcnQgY2xhc3MgRXNidWlsZFByb3ZpZGVyIGltcGxlbWVudHMgSUJ1aWxkUHJvdmlkZXIsIElUcmFuc2Zvcm1Qcm92aWRlciB7XG4gIHByaXZhdGUgc3RhdGljIF9mYWxsYmFja1Byb3ZpZGVyID0gbmV3IEVzYnVpbGRQcm92aWRlcigpO1xuICBwcml2YXRlIHN0YXRpYyBfYnVpbGRQcm92aWRlcjogSUJ1aWxkUHJvdmlkZXI7XG4gIHByaXZhdGUgc3RhdGljIF90cmFuc2Zvcm1hdGlvblByb3ZpZGVyOiBJVHJhbnNmb3JtUHJvdmlkZXI7XG5cbiAgLyoqXG4gICAqIFNldCB0aGUgZGVmYXVsdCBpbXBsZW1lbnRhdGlvbiBmb3IgYm90aCBCdWlsZCBhbmQgVHJhbnNmb3JtYXRpb24gQVBJXG4gICAqL1xuICBwdWJsaWMgc3RhdGljIG92ZXJyaWRlRGVmYXVsdFByb3ZpZGVyKHByb3ZpZGVyOiBJRXNidWlsZFByb3ZpZGVyKSB7XG4gICAgdGhpcy5vdmVycmlkZURlZmF1bHRCdWlsZFByb3ZpZGVyKHByb3ZpZGVyKTtcbiAgICB0aGlzLm92ZXJyaWRlRGVmYXVsdFRyYW5zZm9ybWF0aW9uUHJvdmlkZXIocHJvdmlkZXIpO1xuICB9XG5cbiAgLyoqXG4gICAqIFNldCB0aGUgZGVmYXVsdCBpbXBsZW1lbnRhdGlvbiBmb3IgdGhlIEJ1aWxkIEFQSVxuICAgKi9cbiAgcHVibGljIHN0YXRpYyBvdmVycmlkZURlZmF1bHRCdWlsZFByb3ZpZGVyKHByb3ZpZGVyOiBJQnVpbGRQcm92aWRlcikge1xuICAgIHRoaXMuX2J1aWxkUHJvdmlkZXIgPSBwcm92aWRlcjtcbiAgfVxuXG4gIC8qKlxuICAgKiBHZXQgdGhlIGRlZmF1bHQgaW1wbGVtZW50YXRpb24gZm9yIHRoZSBCdWlsZCBBUElcbiAgICovXG4gIHB1YmxpYyBzdGF0aWMgZGVmYXVsdEJ1aWxkUHJvdmlkZXIoKTogSUJ1aWxkUHJvdmlkZXIge1xuICAgIHJldHVybiB0aGlzLl9idWlsZFByb3ZpZGVyID8/IHRoaXMuX2ZhbGxiYWNrUHJvdmlkZXI7XG4gIH1cblxuICAvKipcbiAgICogU2V0IHRoZSBkZWZhdWx0IGltcGxlbWVudGF0aW9uIGZvciB0aGUgVHJhbnNmb3JtYXRpb24gQVBJXG4gICAqL1xuICBwdWJsaWMgc3RhdGljIG92ZXJyaWRlRGVmYXVsdFRyYW5zZm9ybWF0aW9uUHJvdmlkZXIocHJvdmlkZXI6IElUcmFuc2Zvcm1Qcm92aWRlcikge1xuICAgIHRoaXMuX3RyYW5zZm9ybWF0aW9uUHJvdmlkZXIgPSBwcm92aWRlcjtcbiAgfVxuXG4gIC8qKlxuICAgKiBHZXQgdGhlIGRlZmF1bHQgaW1wbGVtZW50YXRpb24gZm9yIHRoZSBUcmFuc2Zvcm1hdGlvbiBBUElcbiAgICovXG4gIHB1YmxpYyBzdGF0aWMgZGVmYXVsdFRyYW5zZm9ybWF0aW9uUHJvdmlkZXIoKTogSVRyYW5zZm9ybVByb3ZpZGVyIHtcbiAgICByZXR1cm4gdGhpcy5fdHJhbnNmb3JtYXRpb25Qcm92aWRlciA/PyB0aGlzLl9mYWxsYmFja1Byb3ZpZGVyO1xuICB9XG5cbiAgcHJpdmF0ZSByZWFkb25seSBlc2J1aWxkQmluYXJ5UGF0aD86IHN0cmluZztcbiAgcHJpdmF0ZSByZWFkb25seSBlc2J1aWxkTW9kdWxlUGF0aD86IHN0cmluZztcblxuICBwdWJsaWMgY29uc3RydWN0b3IocHJvcHM6IEVzYnVpbGRQcm92aWRlclByb3BzID0ge30pIHtcbiAgICB0aGlzLmVzYnVpbGRCaW5hcnlQYXRoID0gcHJvcHMuZXNidWlsZEJpbmFyeVBhdGg7XG4gICAgdGhpcy5lc2J1aWxkTW9kdWxlUGF0aCA9IHByb3BzLmVzYnVpbGRNb2R1bGVQYXRoO1xuICB9XG5cbiAgcHVibGljIGJ1aWxkU3luYyhvcHRpb25zOiBQcm92aWRlckJ1aWxkT3B0aW9ucyk6IHZvaWQge1xuICAgIGNvbnN0IGVzYnVpbGQgPSB0aGlzLnJlcXVpcmUodGhpcy5lc2J1aWxkTW9kdWxlUGF0aCk7XG4gICAgY29uc3QgYnVpbGRGbiA9IHRoaXMud2l0aEVzYnVpbGRCaW5hcnlQYXRoKGVzYnVpbGQuYnVpbGRTeW5jLCB0aGlzLmVzYnVpbGRCaW5hcnlQYXRoKTtcblxuICAgIGJ1aWxkRm4ob3B0aW9ucyk7XG4gIH1cblxuICBwdWJsaWMgdHJhbnNmb3JtU3luYyhpbnB1dDogc3RyaW5nLCBvcHRpb25zPzogUHJvdmlkZXJUcmFuc2Zvcm1PcHRpb25zKTogc3RyaW5nIHtcbiAgICBjb25zdCBlc2J1aWxkID0gdGhpcy5yZXF1aXJlKHRoaXMuZXNidWlsZE1vZHVsZVBhdGgpO1xuICAgIGNvbnN0IHRyYW5zZm9ybUZuID0gdGhpcy53aXRoRXNidWlsZEJpbmFyeVBhdGgoZXNidWlsZC50cmFuc2Zvcm1TeW5jLCB0aGlzLmVzYnVpbGRCaW5hcnlQYXRoKTtcblxuICAgIHJldHVybiB0cmFuc2Zvcm1GbihpbnB1dCwgb3B0aW9ucykuY29kZTtcbiAgfVxuXG4gIC8qKlxuICAgKiBJbnZva2UgYSBmdW5jdGlvbiB3aXRoIGEgc3BlY2lmaWMgYHByb2Nlc3MuZW52LkVTQlVJTERfQklOQVJZX1BBVEhgXG4gICAqIGFuZCByZXN0b3JlIHRoZSBlbnYgdmFyIGFmdGVyd2FyZHMuXG4gICAqL1xuICBwcml2YXRlIHdpdGhFc2J1aWxkQmluYXJ5UGF0aDxUIGV4dGVuZHMgQ2FsbGFibGVGdW5jdGlvbj4oZm46IFQsIGVzYnVpbGRCaW5hcnlQYXRoPzogc3RyaW5nKSB7XG4gICAgaWYgKCFlc2J1aWxkQmluYXJ5UGF0aCkge1xuICAgICAgcmV0dXJuIGZuO1xuICAgIH1cblxuICAgIHJldHVybiAoLi4uYXJnczogdW5rbm93bltdKSA9PiB7XG4gICAgICBjb25zdCBvcmlnaW5hbEVzYnVpbGRCaW5hcnlQYXRoID0gcHJvY2Vzcy5lbnYuRVNCVUlMRF9CSU5BUllfUEFUSDtcbiAgICAgIGlmIChlc2J1aWxkQmluYXJ5UGF0aCkge1xuICAgICAgICBwcm9jZXNzLmVudi5FU0JVSUxEX0JJTkFSWV9QQVRIID0gZXNidWlsZEJpbmFyeVBhdGg7XG4gICAgICB9XG5cbiAgICAgIGNvbnN0IHJlc3VsdCA9IGZuKC4uLmFyZ3MpO1xuXG4gICAgICAvKipcbiAgICAgICAqIG9ubHkgcmVzZXQgYEVTQlVJTERfQklOQVJZX1BBVEhgIGlmIGl0IHdhcyBleHBsaWNpdGx5IHNldCB2aWEgdGhlIGNvbnN0cnVjdCBwcm9wc1xuICAgICAgICogc2luY2UgYGVzYnVpbGRgIGl0c2VsZiBzb21ldGltZXMgc2V0cyBpdCAoZWcuIHdoZW4gcnVubmluZyBpbiB5YXJuIDIgcGx1ZyZwbGF5KVxuICAgICAgICovXG4gICAgICBpZiAoZXNidWlsZEJpbmFyeVBhdGgpIHtcbiAgICAgICAgcHJvY2Vzcy5lbnYuRVNCVUlMRF9CSU5BUllfUEFUSCA9IG9yaWdpbmFsRXNidWlsZEJpbmFyeVBhdGg7XG4gICAgICB9XG5cbiAgICAgIHJldHVybiByZXN1bHQ7XG4gICAgfTtcbiAgfVxuXG4gIC8qKlxuICAgKiBMb2FkIHRoZSBlc2J1aWxkIG1vZHVsZSBhY2NvcmRpbmcgdG8gZGVmaW5lZCBydWxlcy5cbiAgICovXG4gIHByaXZhdGUgcmVxdWlyZShwYXRoPzogc3RyaW5nKTogSUJ1aWxkUHJvdmlkZXIgJiBJVHJhbnNmb3JtUHJvdmlkZXIge1xuICAgIGNvbnN0IG1vZHVsZSA9IHBhdGggfHwgcHJvY2Vzcy5lbnYuQ0RLX0VTQlVJTERfTU9EVUxFX1BBVEggfHwgRXNidWlsZFNvdXJjZS5wbGF0Zm9ybURlZmF1bHQoKSB8fCBFc2J1aWxkLm5hbWU7XG5cbiAgICByZXR1cm4gdGhpcy5fcmVxdWlyZSh0aGlzLnJlc29sdmUobW9kdWxlKSk7XG4gIH1cblxuICAvKipcbiAgICogV3JhcHBlciBmb3IgcmVxdWlyZVxuICAgKi9cbiAgcHJpdmF0ZSBfcmVxdWlyZShwYXRoOiBzdHJpbmcpOiBJQnVpbGRQcm92aWRlciAmIElUcmFuc2Zvcm1Qcm92aWRlciB7XG4gICAgLy8gZXNsaW50LWRpc2FibGUtbmV4dC1saW5lIEB0eXBlc2NyaXB0LWVzbGludC9uby1yZXF1aXJlLWltcG9ydHNcbiAgICByZXR1cm4gcmVxdWlyZShwYXRoKTtcbiAgfVxuXG4gIC8qKlxuICAgKiBSZXNvbHZlIGEgdG9rZW4gd2l0aG91dCBjb250ZXh0XG4gICAqL1xuICBwcml2YXRlIHJlc29sdmUodG9rZW46IHN0cmluZyk6IHN0cmluZyB7XG4gICAgaWYgKCFUb2tlbi5pc1VucmVzb2x2ZWQodG9rZW4pKSB7XG4gICAgICByZXR1cm4gdG9rZW47XG4gICAgfVxuXG4gICAgcmV0dXJuIFRva2VuaXphdGlvbi5yZXNvbHZlKHRva2VuLCB7XG4gICAgICBzY29wZTogbmV3IENvbnN0cnVjdCh1bmRlZmluZWQgYXMgYW55LCAnJyksXG4gICAgICByZXNvbHZlcjogbmV3IERlZmF1bHRUb2tlblJlc29sdmVyKG5ldyBTdHJpbmdDb25jYXQoKSksXG4gICAgfSk7XG4gIH1cbn1cbiJdfQ==
```

##### package/lib/source.js

###### js-beautify {}

```diff
@@ -101,15 +101,15 @@
         this.assetClass = asset_1.JavaScriptAsset;
     }
 }
 exports.JavaScriptSource = JavaScriptSource;
 _a = JSII_RTTI_SYMBOL_1;
 JavaScriptSource[_a] = {
     fqn: "@mrgrain/cdk-esbuild.JavaScriptSource",
-    version: "4.2.0"
+    version: "4.2.1"
 };
 class TypeScriptSource extends Source {
     constructor(
         /**
          * A path or list or map of paths to the entry points of your code.
          *
          * Relative paths are by default resolved from the current working directory.
@@ -140,10 +140,10 @@
         this.assetClass = asset_1.TypeScriptAsset;
     }
 }
 exports.TypeScriptSource = TypeScriptSource;
 _b = JSII_RTTI_SYMBOL_1;
 TypeScriptSource[_b] = {
     fqn: "@mrgrain/cdk-esbuild.TypeScriptSource",
-    version: "4.2.0"
+    version: "4.2.1"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoic291cmNlLmpzIiwic291cmNlUm9vdCI6IiIsInNvdXJjZXMiOlsiLi4vc3JjL3NvdXJjZS50cyJdLCJuYW1lcyI6W10sIm1hcHBpbmdzIjoiOzs7OztBQUFBLDZDQUFvQztBQU9wQyxtQ0FBdUY7QUFJeEIsQ0FBQztBQUNELENBQUM7QUFFaEUsTUFBZSxNQUFNO0lBY25CO0lBQ0U7Ozs7Ozs7Ozs7Ozs7OztPQWVHO0lBQ0gsV0FBd0I7SUFFeEI7Ozs7Ozs7O09BUUc7SUFDSCxLQUFZO1FBRVosTUFBTSxjQUFjLEdBQTBCO1lBQzVDLFFBQVEsRUFBRSxTQUFTO1NBQ3BCLENBQUM7UUFFRixJQUFJLENBQUMsS0FBSyxHQUFHO1lBQ1gsV0FBVztZQUNYLEdBQUcsS0FBSztZQUNSLFlBQVksRUFBRTtnQkFDWixHQUFHLGNBQWM7Z0JBQ2pCLEdBQUcsS0FBSyxDQUFDLFlBQVk7YUFDdEI7U0FDRixDQUFDO0lBQ0osQ0FBQztJQUVELElBQUksQ0FBQyxLQUFnQixFQUFFLE9BQWlDO1FBQ3RELHFGQUFxRjtRQUNyRixJQUFJLENBQUMsSUFBSSxDQUFDLEtBQUssRUFBRTtZQUNmLElBQUksQ0FBQyxLQUFLLEdBQUcsSUFBSSxJQUFJLENBQUMsVUFBVSxDQUM5QixLQUFLLEVBQ0wsSUFBSSxDQUFDLFdBQVcsQ0FBQyxJQUFJLEVBQ3JCLElBQUksQ0FBQyxLQUFLLENBQ1gsQ0FBQztTQUNIO2FBQU0sSUFBSSxtQkFBSyxDQUFDLEVBQUUsQ0FBQyxJQUFJLENBQUMsS0FBSyxDQUFDLEtBQUssbUJBQUssQ0FBQyxFQUFFLENBQUMsS0FBSyxDQUFDLEVBQUU7WUFDbkQsTUFBTSxJQUFJLEtBQUssQ0FDYixtREFDRSxtQkFBSyxDQUFDLEVBQUUsQ0FBQyxJQUFJLENBQUMsS0FBSyxDQUFDLENBQUMsU0FDdkIsS0FBSyxHQUFHLDhDQUE4QyxDQUN2RCxDQUFDO1NBQ0g7UUFFRCxJQUFJLENBQUMsT0FBTyxFQUFFO1lBQ1osTUFBTSxJQUFJLEtBQUssQ0FDYixZQUFZLElBQUksQ0FBQyxXQUFXLENBQUMsSUFBSSw0QkFBNEIsQ0FDOUQsQ0FBQztTQUNIO1FBRUQsd0VBQXdFO1FBQ3hFLHNFQUFzRTtRQUN0RSw2REFBNkQ7UUFDN0QsSUFBSSxDQUFDLEtBQUssQ0FBQyxNQUFNLENBQUMsU0FBUyxDQUFDLE9BQU8sQ0FBQyxXQUFXLENBQUMsQ0FBQztRQUVqRCxPQUFPO1lBQ0wsTUFBTSxFQUFFLElBQUksQ0FBQyxLQUFLLENBQUMsTUFBTTtZQUN6QixZQUFZLEVBQUUsSUFBSSxDQUFDLEtBQUssQ0FBQyxXQUFXO1NBQ3JDLENBQUM7SUFDSixDQUFDO0NBQ0Y7QUFFRCxNQUFhLGdCQUFpQixTQUFRLE1BR3JDO0lBR0M7SUFFRTs7Ozs7Ozs7Ozs7Ozs7O09BZUc7SUFDSCxXQUF3QjtJQUV4Qjs7Ozs7Ozs7UUFRSTtJQUNKLFFBQStCLEVBQUU7UUFFakMsS0FBSyxDQUFDLFdBQVcsRUFBRSxLQUFLLENBQUMsQ0FBQztRQWpDNUIsZUFBVSxHQUFHLHVCQUFlLENBQUM7SUFrQzdCLENBQUM7O0FBdENILDRDQXVDQzs7O0FBRUQsTUFBYSxnQkFBaUIsU0FBUSxNQUdyQztJQUdDO0lBQ0U7Ozs7Ozs7Ozs7Ozs7OztPQWVHO0lBQ0gsV0FBd0I7SUFFeEI7Ozs7Ozs7O09BUUc7SUFDSCxRQUErQixFQUFFO1FBRWpDLEtBQUssQ0FBQyxXQUFXLEVBQUUsS0FBSyxDQUFDLENBQUM7UUFoQzVCLGVBQVUsR0FBRyx1QkFBZSxDQUFDO0lBaUM3QixDQUFDOztBQXJDSCw0Q0FzQ0MiLCJzb3VyY2VzQ29udGVudCI6WyJpbXBvcnQgeyBTdGFjayB9IGZyb20gJ2F3cy1jZGstbGliJztcbmltcG9ydCB7XG4gIERlcGxveW1lbnRTb3VyY2VDb250ZXh0LFxuICBJU291cmNlLFxuICBTb3VyY2VDb25maWcsXG59IGZyb20gJ2F3cy1jZGstbGliL2F3cy1zMy1kZXBsb3ltZW50JztcbmltcG9ydCB7IENvbnN0cnVjdCB9IGZyb20gJ2NvbnN0cnVjdHMnO1xuaW1wb3J0IHsgQXNzZXRCYXNlUHJvcHMsIEFzc2V0UHJvcHMsIEphdmFTY3JpcHRBc3NldCwgVHlwZVNjcmlwdEFzc2V0IH0gZnJvbSAnLi9hc3NldCc7XG5pbXBvcnQgeyBFbnRyeVBvaW50cyB9IGZyb20gJy4vYnVuZGxlcic7XG5pbXBvcnQgeyBCdWlsZE9wdGlvbnMgfSBmcm9tICcuL2VzYnVpbGQtdHlwZXMnO1xuXG5leHBvcnQgaW50ZXJmYWNlIEphdmFTY3JpcHRTb3VyY2VQcm9wcyBleHRlbmRzIEFzc2V0QmFzZVByb3Bze307XG5leHBvcnQgaW50ZXJmYWNlIFR5cGVTY3JpcHRTb3VyY2VQcm9wcyBleHRlbmRzIEFzc2V0QmFzZVByb3Bze307XG5cbmFic3RyYWN0IGNsYXNzIFNvdXJjZTxcbiAgUHJvcHMgZXh0ZW5kcyBKYXZhU2NyaXB0U291cmNlUHJvcHMgfCBUeXBlU2NyaXB0U291cmNlUHJvcHMsXG4gIEFzc2V0IGV4dGVuZHMgSmF2YVNjcmlwdEFzc2V0IHwgVHlwZVNjcmlwdEFzc2V0LFxuPiBpbXBsZW1lbnRzIElTb3VyY2Uge1xuICBwcm90ZWN0ZWQgcmVhZG9ubHkgYWJzdHJhY3QgYXNzZXRDbGFzczogbmV3IChcbiAgICBzY29wZTogQ29uc3RydWN0LFxuICAgIGlkOiBzdHJpbmcsXG4gICAgcHJvcHM6IEFzc2V0UHJvcHMsXG4gICkgPT4gQXNzZXQ7XG5cbiAgcHJvdGVjdGVkIHByb3BzOiBBc3NldFByb3BzO1xuXG4gIHByb3RlY3RlZCBhc3NldCE6IEFzc2V0O1xuXG4gIGNvbnN0cnVjdG9yKFxuICAgIC8qKlxuICAgICAqIEEgcGF0aCBvciBsaXN0IG9yIG1hcCBvZiBwYXRocyB0byB0aGUgZW50cnkgcG9pbnRzIG9mIHlvdXIgY29kZS5cbiAgICAgKlxuICAgICAqIFJlbGF0aXZlIHBhdGhzIGFyZSBieSBkZWZhdWx0IHJlc29sdmVkIGZyb20gdGhlIGN1cnJlbnQgd29ya2luZyBkaXJlY3RvcnkuXG4gICAgICogVG8gY2hhbmdlIHRoZSB3b3JraW5nIGRpcmVjdG9yeSwgc2VlIGBidWlsZE9wdGlvbnMuYWJzV29ya2luZ0RpcmAuXG4gICAgICpcbiAgICAgKiBBYnNvbHV0ZSBwYXRocyBjYW4gYmUgdXNlZCBpZiBmaWxlcyBhcmUgcGFydCBvZiB0aGUgd29ya2luZyBkaXJlY3RvcnkuXG4gICAgICpcbiAgICAgKiBFeGFtcGxlczpcbiAgICAgKiAgLSBgJ3NyYy9pbmRleC50cydgXG4gICAgICogIC0gYHJlcXVpcmUucmVzb2x2ZSgnLi9sYW1iZGEnKWBcbiAgICAgKiAgLSBgWydzcmMvaW5kZXgudHMnLCAnc3JjL3V0aWwudHMnXWBcbiAgICAgKiAgLSBge29uZTogJ3NyYy90d28udHMnLCB0d286ICdzcmMvb25lLnRzJ31gXG4gICAgICpcbiAgICAgKiBAc3RhYmlsaXR5IHN0YWJsZVxuICAgICAqL1xuICAgIGVudHJ5UG9pbnRzOiBFbnRyeVBvaW50cyxcblxuICAgIC8qKlxuICAgICAqIFByb3BzIHRvIGNoYW5nZSB0aGUgYmVoYXZpb3Igb2YgdGhlIGJ1bmRsZXIuXG4gICAgICpcbiAgICAgKiBEZWZhdWx0IHZhbHVlcyBmb3IgYHByb3BzLmJ1aWxkT3B0aW9uc2A6XG4gICAgICogLSBgYnVuZGxlPXRydWVgXG4gICAgICogLSBgcGxhdGZvcm09YnJvd3NlcmBcbiAgICAgKlxuICAgICAqIEBzdGFiaWxpdHkgc3RhYmxlXG4gICAgICovXG4gICAgcHJvcHM6IFByb3BzLFxuICApIHtcbiAgICBjb25zdCBkZWZhdWx0T3B0aW9uczogUGFydGlhbDxCdWlsZE9wdGlvbnM+ID0ge1xuICAgICAgcGxhdGZvcm06ICdicm93c2VyJyxcbiAgICB9O1xuXG4gICAgdGhpcy5wcm9wcyA9IHtcbiAgICAgIGVudHJ5UG9pbnRzLFxuICAgICAgLi4ucHJvcHMsXG4gICAgICBidWlsZE9wdGlvbnM6IHtcbiAgICAgICAgLi4uZGVmYXVsdE9wdGlvbnMsXG4gICAgICAgIC4uLnByb3BzLmJ1aWxkT3B0aW9ucyxcbiAgICAgIH0sXG4gICAgfTtcbiAgfVxuXG4gIGJpbmQoc2NvcGU6IENvbnN0cnVjdCwgY29udGV4dD86IERlcGxveW1lbnRTb3VyY2VDb250ZXh0KTogU291cmNlQ29uZmlnIHtcbiAgICAvLyBJZiB0aGUgc2FtZSBBc3NldENvZGUgaXMgdXNlZCBtdWx0aXBsZSB0aW1lcywgcmV0YWluIG9ubHkgdGhlIGZpcnN0IGluc3RhbnRpYXRpb24uXG4gICAgaWYgKCF0aGlzLmFzc2V0KSB7XG4gICAgICB0aGlzLmFzc2V0ID0gbmV3IHRoaXMuYXNzZXRDbGFzcyhcbiAgICAgICAgc2NvcGUsXG4gICAgICAgIHRoaXMuY29uc3RydWN0b3IubmFtZSxcbiAgICAgICAgdGhpcy5wcm9wcyxcbiAgICAgICk7XG4gICAgfSBlbHNlIGlmIChTdGFjay5vZih0aGlzLmFzc2V0KSAhPT0gU3RhY2sub2Yoc2NvcGUpKSB7XG4gICAgICB0aHJvdyBuZXcgRXJyb3IoXG4gICAgICAgIGBBc3NldCBpcyBhbHJlYWR5IGFzc29jaWF0ZWQgd2l0aCBhbm90aGVyIHN0YWNrICcke1xuICAgICAgICAgIFN0YWNrLm9mKHRoaXMuYXNzZXQpLnN0YWNrTmFtZVxuICAgICAgICB9Jy4gYCArICdDcmVhdGUgYSBuZXcgQXNzZXQgaW5zdGFuY2UgZm9yIGV2ZXJ5IHN0YWNrLicsXG4gICAgICApO1xuICAgIH1cblxuICAgIGlmICghY29udGV4dCkge1xuICAgICAgdGhyb3cgbmV3IEVycm9yKFxuICAgICAgICBgVG8gdXNlIGEgJHt0aGlzLmNvbnN0cnVjdG9yLm5hbWV9LCBjb250ZXh0IG11c3QgYmUgcHJvdmlkZWRgLFxuICAgICAgKTtcbiAgICB9XG5cbiAgICAvLyB3ZSBnaXZlIHBlcm1pc3Npb25zIG9uIGFsbCBmaWxlcyBpbiB0aGUgYnVja2V0IHNpbmNlIHdlIGRvbid0IHdhbnQgdG9cbiAgICAvLyBhY2NpZGVudGFsbHkgcmV2b2tlIHBlcm1pc3Npb24gb24gb2xkIHZlcnNpb25zIHdoZW4gZGVwbG95aW5nIGEgbmV3XG4gICAgLy8gdmVyc2lvbiAoZm9yIGV4YW1wbGUsIHdoZW4gdXNpbmcgTGFtYmRhIHRyYWZmaWMgc2hpZnRpbmcpLlxuICAgIHRoaXMuYXNzZXQuYnVja2V0LmdyYW50UmVhZChjb250ZXh0LmhhbmRsZXJSb2xlKTtcblxuICAgIHJldHVybiB7XG4gICAgICBidWNrZXQ6IHRoaXMuYXNzZXQuYnVja2V0LFxuICAgICAgemlwT2JqZWN0S2V5OiB0aGlzLmFzc2V0LnMzT2JqZWN0S2V5LFxuICAgIH07XG4gIH1cbn1cblxuZXhwb3J0IGNsYXNzIEphdmFTY3JpcHRTb3VyY2UgZXh0ZW5kcyBTb3VyY2U8XG5KYXZhU2NyaXB0U291cmNlUHJvcHMsXG5KYXZhU2NyaXB0QXNzZXRcbj4ge1xuICBhc3NldENsYXNzID0gSmF2YVNjcmlwdEFzc2V0O1xuXG4gIGNvbnN0cnVjdG9yKFxuXG4gICAgLyoqXG4gICAgICogQSBwYXRoIG9yIGxpc3Qgb3IgbWFwIG9mIHBhdGhzIHRvIHRoZSBlbnRyeSBwb2ludHMgb2YgeW91ciBjb2RlLlxuICAgICAqXG4gICAgICogUmVsYXRpdmUgcGF0aHMgYXJlIGJ5IGRlZmF1bHQgcmVzb2x2ZWQgZnJvbSB0aGUgY3VycmVudCB3b3JraW5nIGRpcmVjdG9yeS5cbiAgICAgKiBUbyBjaGFuZ2UgdGhlIHdvcmtpbmcgZGlyZWN0b3J5LCBzZWUgYGJ1aWxkT3B0aW9ucy5hYnNXb3JraW5nRGlyYC5cbiAgICAgKlxuICAgICAqIEFic29sdXRlIHBhdGhzIGNhbiBiZSB1c2VkIGlmIGZpbGVzIGFyZSBwYXJ0IG9mIHRoZSB3b3JraW5nIGRpcmVjdG9yeS5cbiAgICAgKlxuICAgICAqIEV4YW1wbGVzOlxuICAgICAqICAtIGAnc3JjL2luZGV4LnRzJ2BcbiAgICAgKiAgLSBgcmVxdWlyZS5yZXNvbHZlKCcuL2xhbWJkYScpYFxuICAgICAqICAtIGBbJ3NyYy9pbmRleC50cycsICdzcmMvdXRpbC50cyddYFxuICAgICAqICAtIGB7b25lOiAnc3JjL3R3by50cycsIHR3bzogJ3NyYy9vbmUudHMnfWBcbiAgICAgKlxuICAgICAqIEBzdGFiaWxpdHkgc3RhYmxlXG4gICAgICovXG4gICAgZW50cnlQb2ludHM6IEVudHJ5UG9pbnRzLFxuXG4gICAgLyoqXG4gICAgICAqIFByb3BzIHRvIGNoYW5nZSB0aGUgYmVoYXZpb3Igb2YgdGhlIGJ1bmRsZXIuXG4gICAgICAqXG4gICAgICAqIERlZmF1bHQgdmFsdWVzIGZvciBgcHJvcHMuYnVpbGRPcHRpb25zYDpcbiAgICAgICogLSBgYnVuZGxlPXRydWVgXG4gICAgICAqIC0gYHBsYXRmb3JtPWJyb3dzZXJgXG4gICAgICAqXG4gICAgICAqIEBzdGFiaWxpdHkgc3RhYmxlXG4gICAgICAqL1xuICAgIHByb3BzOiBKYXZhU2NyaXB0U291cmNlUHJvcHMgPSB7fSxcbiAgKSB7XG4gICAgc3VwZXIoZW50cnlQb2ludHMsIHByb3BzKTtcbiAgfVxufVxuXG5leHBvcnQgY2xhc3MgVHlwZVNjcmlwdFNvdXJjZSBleHRlbmRzIFNvdXJjZTxcblR5cGVTY3JpcHRTb3VyY2VQcm9wcyxcblR5cGVTY3JpcHRBc3NldFxuPiB7XG4gIGFzc2V0Q2xhc3MgPSBUeXBlU2NyaXB0QXNzZXQ7XG5cbiAgY29uc3RydWN0b3IoXG4gICAgLyoqXG4gICAgICogQSBwYXRoIG9yIGxpc3Qgb3IgbWFwIG9mIHBhdGhzIHRvIHRoZSBlbnRyeSBwb2ludHMgb2YgeW91ciBjb2RlLlxuICAgICAqXG4gICAgICogUmVsYXRpdmUgcGF0aHMgYXJlIGJ5IGRlZmF1bHQgcmVzb2x2ZWQgZnJvbSB0aGUgY3VycmVudCB3b3JraW5nIGRpcmVjdG9yeS5cbiAgICAgKiBUbyBjaGFuZ2UgdGhlIHdvcmtpbmcgZGlyZWN0b3J5LCBzZWUgYGJ1aWxkT3B0aW9ucy5hYnNXb3JraW5nRGlyYC5cbiAgICAgKlxuICAgICAqIEFic29sdXRlIHBhdGhzIGNhbiBiZSB1c2VkIGlmIGZpbGVzIGFyZSBwYXJ0IG9mIHRoZSB3b3JraW5nIGRpcmVjdG9yeS5cbiAgICAgKlxuICAgICAqIEV4YW1wbGVzOlxuICAgICAqICAtIGAnc3JjL2luZGV4LnRzJ2BcbiAgICAgKiAgLSBgcmVxdWlyZS5yZXNvbHZlKCcuL2xhbWJkYScpYFxuICAgICAqICAtIGBbJ3NyYy9pbmRleC50cycsICdzcmMvdXRpbC50cyddYFxuICAgICAqICAtIGB7b25lOiAnc3JjL3R3by50cycsIHR3bzogJ3NyYy9vbmUudHMnfWBcbiAgICAgKlxuICAgICAqIEBzdGFiaWxpdHkgc3RhYmxlXG4gICAgICovXG4gICAgZW50cnlQb2ludHM6IEVudHJ5UG9pbnRzLFxuXG4gICAgLyoqXG4gICAgICogUHJvcHMgdG8gY2hhbmdlIHRoZSBiZWhhdmlvciBvZiB0aGUgYnVuZGxlci5cbiAgICAgKlxuICAgICAqIERlZmF1bHQgdmFsdWVzIGZvciBgcHJvcHMuYnVpbGRPcHRpb25zYDpcbiAgICAgKiAtIGBidW5kbGU9dHJ1ZWBcbiAgICAgKiAtIGBwbGF0Zm9ybT1icm93c2VyYFxuICAgICAqXG4gICAgICogQHN0YWJpbGl0eSBzdGFibGVcbiAgICAgKi9cbiAgICBwcm9wczogVHlwZVNjcmlwdFNvdXJjZVByb3BzID0ge30sXG4gICkge1xuICAgIHN1cGVyKGVudHJ5UG9pbnRzLCBwcm9wcyk7XG4gIH1cbn1cbiJdfQ==
```

##### package/package.json

###### Pretty-printed

 * *Similarity: 0.9753694581280788%*

 * *Differences: {"'devDependencies'": "{'eslint-plugin-import': '^2.28.0', 'projen': '^0.71.158'}",*

 * * "'version'": "'4.2.1'"}*

```diff
@@ -20,25 +20,25 @@
         "@typescript-eslint/parser": "^5",
         "aws-cdk-lib": "2.12.0",
         "constructs": "10.0.5",
         "esbuild": "^0.18.0",
         "eslint": "^8",
         "eslint-import-resolver-node": "^0.3.7",
         "eslint-import-resolver-typescript": "^2.7.1",
-        "eslint-plugin-import": "^2.27.5",
+        "eslint-plugin-import": "^2.28.0",
         "jest": "^27",
         "jest-junit": "^15",
         "jest-mock": "^27.5.1",
         "jsii": "1.x",
         "jsii-diff": "^1.85.0",
         "jsii-docgen": "^3.8.31",
         "jsii-pacmak": "^1.85.0",
         "jsii-rosetta": "1.x",
         "npm-check-updates": "^16",
-        "projen": "^0.71.150",
+        "projen": "^0.71.158",
         "standard-version": "^9",
         "ts-jest": "^27",
         "ts-morph": "^17.0.1",
         "ts-node": "^10",
         "typescript": "^4.9.5"
     },
     "homepage": "https://github.com/mrgrain/cdk-esbuild",
@@ -170,9 +170,9 @@
         "test:watch": "npx projen test:watch",
         "unbump": "npx projen unbump",
         "upgrade": "npx projen upgrade",
         "watch": "npx projen watch"
     },
     "stability": "stable",
     "types": "lib/index.d.ts",
-    "version": "4.2.0"
+    "version": "4.2.1"
 }
```

### Comparing `mrgrain.cdk-esbuild-4.2.0/src/mrgrain.cdk_esbuild.egg-info/PKG-INFO` & `mrgrain.cdk-esbuild-4.2.1/src/mrgrain.cdk_esbuild.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrgrain.cdk-esbuild
-Version: 4.2.0
+Version: 4.2.1
 Summary: CDK constructs for esbuild, an extremely fast JavaScript bundler
 Home-page: https://github.com/mrgrain/cdk-esbuild
 Author: Moritz Kornher<mail@moritzkornher.de>
 License: MIT
 Project-URL: Source, https://github.com/mrgrain/cdk-esbuild
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

