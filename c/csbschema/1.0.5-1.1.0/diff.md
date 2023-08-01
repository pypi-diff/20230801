# Comparing `tmp/csbschema-1.0.5.tar.gz` & `tmp/csbschema-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csbschema-1.0.5.tar", last modified: Tue Jul 18 19:28:30 2023, max compression
+gzip compressed data, was "csbschema-1.1.0.tar", last modified: Tue Aug  1 19:37:24 2023, max compression
```

## Comparing `csbschema-1.0.5.tar` & `csbschema-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxr-xr-x   0 miles      (505) staff       (20)        0 2023-07-18 19:28:30.276269 csbschema-1.0.5/
--rw-r--r--   0 miles      (505) staff       (20)     1143 2023-01-23 01:58:17.000000 csbschema-1.0.5/LICENSE.txt
--rw-r--r--   0 miles      (505) staff       (20)      213 2023-04-10 14:31:46.000000 csbschema-1.0.5/MANIFEST.in
--rw-r--r--   0 miles      (505) staff       (20)     4268 2023-07-18 19:28:30.276134 csbschema-1.0.5/PKG-INFO
--rw-r--r--   0 miles      (505) staff       (20)     3659 2023-07-18 19:26:57.000000 csbschema-1.0.5/README.md
-drwxr-xr-x   0 miles      (505) staff       (20)        0 2023-07-18 19:28:30.272978 csbschema-1.0.5/csbschema/
--rw-r--r--   0 miles      (505) staff       (20)     1418 2023-07-18 19:26:57.000000 csbschema-1.0.5/csbschema/__init__.py
-drwxr-xr-x   0 miles      (505) staff       (20)        0 2023-07-18 19:28:30.274724 csbschema-1.0.5/csbschema/cmd/
--rw-r--r--   0 miles      (505) staff       (20)      285 2023-01-23 01:58:17.000000 csbschema-1.0.5/csbschema/cmd/__init__.py
--rw-r--r--   0 miles      (505) staff       (20)     1360 2023-01-23 01:58:17.000000 csbschema-1.0.5/csbschema/cmd/__main__.py
--rw-r--r--   0 miles      (505) staff       (20)     1230 2023-02-15 18:16:21.000000 csbschema-1.0.5/csbschema/cmd/validate.py
-drwxr-xr-x   0 miles      (505) staff       (20)        0 2023-07-18 19:28:30.275973 csbschema-1.0.5/csbschema/data/
--rw-r--r--   0 miles      (505) staff       (20)    22704 2023-04-10 14:31:46.000000 csbschema-1.0.5/csbschema/data/CSB-schema-3_0_0-2023-03.json
--rw-r--r--   0 miles      (505) staff       (20)    20601 2023-04-10 14:31:46.000000 csbschema-1.0.5/csbschema/data/CSB-schema-3_1_0-2023-03.json
--rw-r--r--   0 miles      (505) staff       (20)    20519 2023-04-10 14:31:46.000000 csbschema-1.0.5/csbschema/data/CSB-schema-3_2_0-BETA.json
--rw-r--r--   0 miles      (505) staff       (20)    20280 2023-04-10 14:31:46.000000 csbschema-1.0.5/csbschema/data/XYZ-CSB-schema-3_0_0-2023-03.json
--rw-r--r--   0 miles      (505) staff       (20)        0 2023-03-08 19:42:06.000000 csbschema-1.0.5/csbschema/data/__init__.py
--rw-r--r--   0 miles      (505) staff       (20)    20170 2023-07-18 19:26:57.000000 csbschema-1.0.5/csbschema/validators.py
-drwxr-xr-x   0 miles      (505) staff       (20)        0 2023-07-18 19:28:30.273917 csbschema-1.0.5/csbschema.egg-info/
--rw-r--r--   0 miles      (505) staff       (20)     4268 2023-07-18 19:28:30.000000 csbschema-1.0.5/csbschema.egg-info/PKG-INFO
--rw-r--r--   0 miles      (505) staff       (20)      580 2023-07-18 19:28:30.000000 csbschema-1.0.5/csbschema.egg-info/SOURCES.txt
--rw-r--r--   0 miles      (505) staff       (20)        1 2023-07-18 19:28:30.000000 csbschema-1.0.5/csbschema.egg-info/dependency_links.txt
--rw-r--r--   0 miles      (505) staff       (20)       58 2023-07-18 19:28:30.000000 csbschema-1.0.5/csbschema.egg-info/entry_points.txt
--rw-r--r--   0 miles      (505) staff       (20)      135 2023-07-18 19:28:30.000000 csbschema-1.0.5/csbschema.egg-info/requires.txt
--rw-r--r--   0 miles      (505) staff       (20)       10 2023-07-18 19:28:30.000000 csbschema-1.0.5/csbschema.egg-info/top_level.txt
--rw-r--r--   0 miles      (505) staff       (20)     1055 2023-04-10 14:51:54.000000 csbschema-1.0.5/pyproject.toml
--rw-r--r--   0 miles      (505) staff       (20)       38 2023-07-18 19:28:30.276308 csbschema-1.0.5/setup.cfg
+drwxr-xr-x   0 miles      (505) staff       (20)        0 2023-08-01 19:37:24.978525 csbschema-1.1.0/
+-rw-r--r--   0 miles      (505) staff       (20)     1143 2023-01-23 01:58:17.000000 csbschema-1.1.0/LICENSE.txt
+-rw-r--r--   0 miles      (505) staff       (20)      376 2023-08-01 19:35:57.000000 csbschema-1.1.0/MANIFEST.in
+-rw-r--r--   0 miles      (505) staff       (20)     4268 2023-08-01 19:37:24.978412 csbschema-1.1.0/PKG-INFO
+-rw-r--r--   0 miles      (505) staff       (20)     3659 2023-07-18 19:26:57.000000 csbschema-1.1.0/README.md
+drwxr-xr-x   0 miles      (505) staff       (20)        0 2023-08-01 19:37:24.975237 csbschema-1.1.0/csbschema/
+-rw-r--r--   0 miles      (505) staff       (20)     1911 2023-08-01 19:35:57.000000 csbschema-1.1.0/csbschema/__init__.py
+drwxr-xr-x   0 miles      (505) staff       (20)        0 2023-08-01 19:37:24.976660 csbschema-1.1.0/csbschema/command/
+-rw-r--r--   0 miles      (505) staff       (20)      285 2023-08-01 19:35:57.000000 csbschema-1.1.0/csbschema/command/__init__.py
+-rw-r--r--   0 miles      (505) staff       (20)     1368 2023-08-01 19:35:57.000000 csbschema-1.1.0/csbschema/command/__main__.py
+-rw-r--r--   0 miles      (505) staff       (20)     1234 2023-08-01 19:35:57.000000 csbschema-1.1.0/csbschema/command/validate.py
+drwxr-xr-x   0 miles      (505) staff       (20)        0 2023-08-01 19:37:24.978284 csbschema-1.1.0/csbschema/data/
+-rw-r--r--   0 miles      (505) staff       (20)    22704 2023-04-10 14:31:46.000000 csbschema-1.1.0/csbschema/data/CSB-schema-3_0_0-2023-03.json
+-rw-r--r--   0 miles      (505) staff       (20)    27028 2023-08-01 19:35:57.000000 csbschema-1.1.0/csbschema/data/CSB-schema-3_0_0-2023-08.json
+-rw-r--r--   0 miles      (505) staff       (20)    20601 2023-04-10 14:31:46.000000 csbschema-1.1.0/csbschema/data/CSB-schema-3_1_0-2023-03.json
+-rw-r--r--   0 miles      (505) staff       (20)    24735 2023-08-01 19:35:57.000000 csbschema-1.1.0/csbschema/data/CSB-schema-3_1_0-2023-08.json
+-rw-r--r--   0 miles      (505) staff       (20)    24283 2023-08-01 19:35:57.000000 csbschema-1.1.0/csbschema/data/CSB-schema-3_2_0-BETA.json
+-rw-r--r--   0 miles      (505) staff       (20)    20280 2023-04-10 14:31:46.000000 csbschema-1.1.0/csbschema/data/XYZ-CSB-schema-3_0_0-2023-03.json
+-rw-r--r--   0 miles      (505) staff       (20)    24608 2023-08-01 19:35:57.000000 csbschema-1.1.0/csbschema/data/XYZ-CSB-schema-3_0_0-2023-08.json
+-rw-r--r--   0 miles      (505) staff       (20)        0 2023-03-08 19:42:06.000000 csbschema-1.1.0/csbschema/data/__init__.py
+-rw-r--r--   0 miles      (505) staff       (20)    29329 2023-08-01 19:35:57.000000 csbschema-1.1.0/csbschema/validators.py
+drwxr-xr-x   0 miles      (505) staff       (20)        0 2023-08-01 19:37:24.976241 csbschema-1.1.0/csbschema.egg-info/
+-rw-r--r--   0 miles      (505) staff       (20)     4268 2023-08-01 19:37:24.000000 csbschema-1.1.0/csbschema.egg-info/PKG-INFO
+-rw-r--r--   0 miles      (505) staff       (20)      731 2023-08-01 19:37:24.000000 csbschema-1.1.0/csbschema.egg-info/SOURCES.txt
+-rw-r--r--   0 miles      (505) staff       (20)        1 2023-08-01 19:37:24.000000 csbschema-1.1.0/csbschema.egg-info/dependency_links.txt
+-rw-r--r--   0 miles      (505) staff       (20)       62 2023-08-01 19:37:24.000000 csbschema-1.1.0/csbschema.egg-info/entry_points.txt
+-rw-r--r--   0 miles      (505) staff       (20)      135 2023-08-01 19:37:24.000000 csbschema-1.1.0/csbschema.egg-info/requires.txt
+-rw-r--r--   0 miles      (505) staff       (20)       10 2023-08-01 19:37:24.000000 csbschema-1.1.0/csbschema.egg-info/top_level.txt
+-rw-r--r--   0 miles      (505) staff       (20)     1059 2023-08-01 19:35:57.000000 csbschema-1.1.0/pyproject.toml
+-rw-r--r--   0 miles      (505) staff       (20)       38 2023-08-01 19:37:24.978554 csbschema-1.1.0/setup.cfg
```

### Comparing `csbschema-1.0.5/LICENSE.txt` & `csbschema-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `csbschema-1.0.5/PKG-INFO` & `csbschema-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csbschema
-Version: 1.0.5
+Version: 1.1.0
 Summary: JSON Schema and validator for IHO B-12 Crowdsourced Bathymetry metadata and data
 Author-email: Brian Miles <bmiles@ccom.unh.edu>, Brian Calder <brc@ccom.unh.edu>
 Project-URL: Homepage, https://github.com/CCOMJHC/csbschema
 Project-URL: Bug Tracker, https://github.com/CCOMJHC/csbschema/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `csbschema-1.0.5/README.md` & `csbschema-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `csbschema-1.0.5/csbschema/cmd/__main__.py` & `csbschema-1.1.0/csbschema/command/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import argparse
 from typing import Union
 
 from csbschema import __version__ as version
-from csbschema.cmd import EXIT_USAGE
-from csbschema.cmd.validate import validate
+from csbschema.command import EXIT_USAGE
+from csbschema.command.validate import validate
 
 
 class CSBSchema:
     def __init__(self):
         parser = argparse.ArgumentParser(
             description='CSB schema tools',
             usage='''csbschema <command> [<arguments>]
```

### Comparing `csbschema-1.0.5/csbschema/cmd/validate.py` & `csbschema-1.1.0/csbschema/command/validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 from typing import Union
 import argparse
 import logging
 
-from csbschema.cmd import EXIT_DATAERR, EXIT_OK
+from csbschema.command import EXIT_DATAERR, EXIT_OK
 from csbschema import DEFAULT_VALIDATOR_VERSION, VALIDATORS, validate_data
 
 logger = logging.getLogger(__name__)
 
 
 def validate() -> Union[int, str]:
     parser = argparse.ArgumentParser(
```

### Comparing `csbschema-1.0.5/csbschema/data/CSB-schema-3_0_0-2023-03.json` & `csbschema-1.1.0/csbschema/data/CSB-schema-3_0_0-2023-03.json`

 * *Files identical despite different names*

### Comparing `csbschema-1.0.5/csbschema/data/CSB-schema-3_1_0-2023-03.json` & `csbschema-1.1.0/csbschema/data/CSB-schema-3_1_0-2023-03.json`

 * *Files identical despite different names*

### Comparing `csbschema-1.0.5/csbschema/data/CSB-schema-3_2_0-BETA.json` & `csbschema-1.1.0/csbschema/data/XYZ-CSB-schema-3_0_0-2023-03.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6893271302299855%*

 * *Differences: {"'$id'": "'https://raw.githubusercontent.com/CCOMJHC/csbschema/main/csbschema/data/XYZ-CSB-schema-3_0_0-2023-03.json'",*

 * * "'definitions'": "{'RFC3339_time': {'description': 'RFC3339 UTC time stamp (note: version 3.0.0 "*

 * *                  "allows timezone naive timestamps).', 'pattern': "*

 * *                  "'^([0-9]+)-(0[1-9]|1[012])-(0[1-9]|[12][0-9]|3[01])[Tt]([01][0-9]|2[0-3]):([0-5][0-9]):([0-5][0-9]|60)([.][0-9]+)?[Zz]?$'}, "*

 * *                  "'IDNumber_MMSI': {'type': 'integer', 'minimum': 100000000,  […]*

```diff
@@ -1,173 +1,121 @@
 {
-    "$id": "https://raw.githubusercontent.com/CCOMJHC/csbschema/main/csbschema/data/CSB-schema-3_2_0-BETA.json",
+    "$id": "https://raw.githubusercontent.com/CCOMJHC/csbschema/main/csbschema/data/XYZ-CSB-schema-3_0_0-2023-03.json",
     "$schema": "https://json-schema.org/draft/2020-12/schema",
     "definitions": {
-        "B12_Metadata": {
-            "properties": {
-                "observationCollection": {
-                    "$ref": "#/definitions/ObservationCollection"
-                },
-                "trustedNode": {
-                    "$ref": "#/definitions/TrustedNodePlatform"
-                }
-            },
-            "required": [
-                "trustedNodePlatform"
-            ],
-            "type": "object"
-        },
-        "CRS": {
-            "properties": {
-                "properties": {
-                    "properties": {
-                        "name": {
-                            "$ref": "#/definitions/CRS_Name"
-                        }
-                    },
-                    "required": [
-                        "name"
-                    ],
-                    "type": "object"
-                }
+        "Algorithms": {
+            "description": "Array of algorithms applied to the data.",
+            "items": {
+                "required": [
+                    "name",
+                    "params"
+                ],
+                "type": "object"
             },
-            "required": [
-                "properties"
-            ],
-            "type": "object"
+            "minItems": 1,
+            "type": "array"
         },
         "CRS_Name": {
             "description": "CRS name as an EPSG string.",
             "pattern": "^EPSG:(3276[0-7]$|327[0-5]\\d$|32[0-6]\\d\\d$|3[0-1]\\d\\d\\d$|[1-2][0-9]{4}$|102[4-9]|10[3-9][0-9]$|1[1-9][0-9][0-9]$|[2-9][0-9][0-9][0-9]$)",
             "type": "string"
         },
-        "CSBDatum": {
-            "properties": {
-                "depth": {
-                    "description": "The distance from the vertical reference point to the seafloor. Should be collected as a positive value, in metres, with decimetre precision.",
-                    "type": "number"
-                },
-                "time": {
-                    "$ref": "#/definitions/RFC3339_time",
-                    "description": "The date and UTC time stamp for the depth measurement as well as can be determined, ideally to millisecond precision in RFC3339 format."
-                }
-            },
-            "required": [
-                "depth",
-                "time"
+        "Convention": {
+            "description": "This field describes the format and version for the data and metadata, such as GeoJSON, CSV, or XYZT. Reference the version of the CSB data convention (e.g., CSB 2.0, CSB 3.0) where possible.",
+            "enum": [
+                "XYZ CSB 3.0"
             ],
-            "type": "object"
+            "type": "string"
         },
-        "GeoJSONFeature": {
+        "Correctors": {
             "properties": {
-                "geometry": {
-                    "oneOf": [
-                        {
-                            "type": "null"
-                        },
-                        {
-                            "properties": {
-                                "bbox": {
-                                    "items": {
-                                        "type": "number"
-                                    },
-                                    "minItems": 4,
-                                    "type": "array"
-                                },
-                                "coordinates": {
-                                    "items": {
-                                        "type": "number"
-                                    },
-                                    "minItems": 2,
-                                    "type": "array"
-                                },
-                                "type": {
-                                    "enum": [
-                                        "Point"
-                                    ],
-                                    "type": "string"
-                                }
-                            },
-                            "required": [
-                                "type",
-                                "coordinates"
-                            ],
-                            "title": "GeoJSON Point",
-                            "type": "object"
-                        }
-                    ]
+                "dataProcessed": {
+                    "description": "Raw data, without tidal corrections or additional processing, are preferable as a contribution to the IHO DCDB. This field allows the data contributor to state whether the data has been processed or corrected (\u2018True\u2019) or not (\u2018False\u2019). If \u2018True\u2019, it is strongly recommended that detailed information be captured in optional metadata fields as outlined in section 3.3.4. If \u2018False\u2019, information in section 3.3.4 is not needed.",
+                    "type": "boolean"
                 },
-                "id": {
-                    "oneOf": [
-                        {
-                            "type": "number"
-                        },
-                        {
-                            "type": "string"
-                        }
-                    ]
+                "draftApplied": {
+                    "description": "Describes whether vessel draft has been corrected for.",
+                    "type": "boolean"
                 },
-                "properties": {
-                    "$ref": "#/definitions/CSBDatum"
+                "motionOffsetsApplied": {
+                    "description": "Describes whether vessel motion has been corrected for.",
+                    "type": "boolean"
                 },
-                "type": {
+                "positionOffsetsDocumented": {
+                    "description": "Describes whether the final vessel position (longitude and latitude) has been corrected for the lateral and longitudinal offsets between the GNSS receiver and the transducer (\u201cTrue\u201d), or if they were not (\u201cFalse\u201d). If \u201cTrue\u201d, the position element of the sensor description field in Table 3 should be populated.",
+                    "type": "boolean"
+                },
+                "positionReferencePoint": {
                     "enum": [
-                        "Feature"
+                        "GNSS"
                     ],
                     "type": "string"
+                },
+                "soundSpeedDocumented": {
+                    "description": "Some systems may have the ability to provide sound speed data and correct the sounding. If details regarding such corrections are known (\u201cTrue\u201d), it is strongly recommended that the \u2018Sound Speed Correction\u2019 field in Table 4 be populated. If \u201cFalse\u201d, no information about how sound speed was applied has been recorded.",
+                    "type": "boolean"
                 }
             },
             "required": [
-                "type",
-                "properties",
-                "geometry"
+                "positionReferencePoint"
             ],
-            "title": "GeoJSON Feature",
             "type": "object"
         },
-        "IDNumber_IMO": {
-            "pattern": "^IMO\\d{7}$",
+        "DataLicense": {
+            "description": "The license under which the Trusted Node is\n providing CSB data to the IHO DCDB.\n",
             "type": "string"
         },
+        "EPSG_Number": {
+            "maximum": 32767,
+            "minimum": 1024,
+            "type": "integer"
+        },
+        "IDNumber_IMO": {
+            "maximum": 9999999,
+            "minimum": 1000000,
+            "type": "integer"
+        },
         "IDNumber_MMSI": {
-            "pattern": "^\\d{9}$",
-            "type": "string"
+            "maximum": 999999999,
+            "minimum": 100000000,
+            "type": "integer"
         },
-        "ObservationCollection": {
+        "Platform": {
             "properties": {
-                "platform": {
-                    "$ref": "#/definitions/ObservationCollectionPlatform"
-                },
-                "processing": {
-                    "$ref": "#/definitions/ObservationCollectionProcessing"
+                "IDNumber": {
+                    "description": "The value for the ID Type. MMSI numbers are often nine digits, while IMO numbers are the letters \u201cIMO,\u201d followed by a seven-digit number.",
+                    "oneOf": [
+                        {
+                            "$ref": "#/definitions/IDNumber_MMSI"
+                        },
+                        {
+                            "$ref": "#/definitions/IDNumber_IMO"
+                        }
+                    ],
+                    "type": "integer"
                 },
-                "trustedNode": {
-                    "$ref": "#/definitions/ObservationCollectionTrustedNode"
-                }
-            },
-            "type": "object"
-        },
-        "ObservationCollectionPlatform": {
-            "properties": {
-                "contributorComments": {
-                    "description": "If the contributor believes there were any problems or events that may have degraded the quality of the position or depth measurements, they can enter that information in this free-text field.",
+                "IDType": {
+                    "description": "ID numbers used to uniquely identify vessels. Currently, only two types are available: Maritime Mobile Service Identity (MMSI) or International Maritime Organization (IMO) number. The MMSI number is used to uniquely identify a vessel through services such as AIS. The IMO number is linked to a vessel for its lifetime, regardless of change in flag or ownership. Contributors may select only one ID Type.",
+                    "enum": [
+                        "MMSI",
+                        "IMO"
+                    ],
                     "type": "string"
                 },
-                "dataProcessed": {
-                    "description": "Raw data, without tidal corrections or additional processing, are preferable as a contribution to the IHO DCDB. This field allows the data contributor to state whether the data has been processed or corrected (\u2018True\u2019) or not (\u2018False\u2019). If \u2018True\u2019, it is strongly recommended that detailed information be captured in optional metadata fields as outlined in section 3.3.4. If \u2018False\u2019, information in section 3.3.4 is not needed.",
-                    "type": "boolean"
+                "correctors": {
+                    "$ref": "#/definitions/Correctors"
                 },
                 "length": {
                     "description": "The length overall (LOA) of the vessel, expressed as a positive value, in metres, to the nearest metre.",
                     "minimum": 1,
                     "type": "integer"
                 },
-                "positionOffsetsDocumented": {
-                    "description": "Describes whether the final vessel position (longitude and latitude) has been corrected for the lateral and longitudinal offsets between the GNSS receiver and the transducer (\u201cTrue\u201d), or if they were not (\u201cFalse\u201d). If \u201cTrue\u201d, the position element of the sensor description field in Table 3 should be populated.",
-                    "type": "boolean"
+                "name": {
+                    "description": "The name of the vessel, in open string format.",
+                    "type": "string"
                 },
                 "sensors": {
                     "description": "Composite element containing all information about a given sensor in use on the collection platform. Minimum specification of fields as shown; some sensors may have additional fields (e.g., frequency for an echo sounder). Position is given from the PRP (Position Reference Point) in metres. The offsets are positive NED (North (Bow), East (Starboard), Down)",
                     "items": {
                         "oneOf": [
                             {
                                 "$ref": "#/definitions/SensorDescriptionSounder"
@@ -179,30 +127,40 @@
                                 "$ref": "#/definitions/SensorDescriptionGNSS"
                             }
                         ]
                     },
                     "minItems": 1,
                     "type": "array"
                 },
-                "soundSpeedDocumented": {
-                    "description": "Some systems may have the ability to provide sound speed data and correct the sounding. If details regarding such corrections are known (\u201cTrue\u201d), it is strongly recommended that the \u2018Sound Speed Correction\u2019 field in Table 4 be populated. If \u201cFalse\u201d, no information about how sound speed was applied has been recorded.",
-                    "type": "boolean"
+                "type": {
+                    "description": "The type of vessel collecting the data, such as a cargo ship, fishing vessel, private vessel,\nresearch vessel, etc.",
+                    "type": "string"
+                },
+                "uniqueID": {
+                    "$ref": "#/definitions/UniqueVesselID"
                 }
             },
+            "required": [
+                "uniqueID",
+                "correctors"
+            ],
             "type": "object"
         },
-        "ObservationCollectionProcessing": {
+        "Processing": {
             "description": "List of processing steps recorded for the data",
             "items": {
                 "oneOf": [
                     {
                         "$ref": "#/definitions/ProcessingTimeStampInterpolation"
                     },
                     {
-                        "$ref": "#/definitions/ProcessingCoordinateReferenceChange"
+                        "$ref": "#/definitions/ProcessingCRSTransformation"
+                    },
+                    {
+                        "$ref": "#/definitions/ProcessingCRS"
                     },
                     {
                         "$ref": "#/definitions/ProcessingVerticalReduction"
                     },
                     {
                         "$ref": "#/definitions/ProcessingGNSS"
                     },
@@ -213,286 +171,352 @@
                         "$ref": "#/definitions/ProcessingAlgorithm"
                     }
                 ]
             },
             "minItems": 1,
             "type": "array"
         },
-        "ObservationCollectionTrustedNode": {
+        "ProcessingAlgorithm": {
+            "description": "General algorithm used to triage data",
             "properties": {
-                "convention": {
-                    "description": "This field describes the format and version for the data and metadata, such as GeoJSON, CSV, or XYZT. Reference the version of the CSB data convention (e.g., CSB 2.0, CSB 3.0) where possible.",
-                    "enum": [
-                        "GeoJSON CSB 3.2"
+                "detail": {
+                    "properties": {
+                        "comment": {
+                            "description": "Explanatory text related to algorithm or its outputs.",
+                            "type": "string"
+                        },
+                        "name": {
+                            "description": "Examples: deduplicate, uncertainty estimation, manual editing.",
+                            "type": "string"
+                        },
+                        "parameters": {
+                            "description": "Parameters used in data processing.",
+                            "type": "string"
+                        }
+                    },
+                    "required": [
+                        "name",
+                        "parameters",
+                        "comment"
                     ],
-                    "type": "string"
-                },
-                "dataLicense": {
-                    "description": "The Creative Commons public domain\n dedication under which the Trusted Node is\n providing CSB data to the IHO DCDB.\n ",
-                    "type": "string"
-                },
-                "navigationCRS": {
-                    "$ref": "#/definitions/CRS_Name",
-                    "description": "The EPSG code referring to the Coordinate Reference System (CRS) of the navigation data"
-                },
-                "providerLogger": {
-                    "description": "The software program or hardware logger used to log the data.",
-                    "type": "string"
-                },
-                "providerLoggerVersion": {
-                    "description": "The software or hardware logger version.",
-                    "type": "string"
+                    "type": "object"
                 },
-                "verticalReferenceOfDepth": {
-                    "description": "The vertical reference of the depth. The vertical reference will most likely be the transducer (ex: NMEA DBT string) or the waterline (ex: NMEA DPT string).",
-                    "enum": [
-                        "Transducer",
-                        "Unknown"
-                    ],
-                    "type": "string"
+                "timestamp": {
+                    "$ref": "#/definitions/RFC3339_time"
                 },
-                "vesselPositionReferencePoint": {
-                    "description": "Position Reference Point (PRP) is the reference point where the navigation data is output. Most likely the reference point will be the location of the GNSS antenna.",
+                "type": {
                     "enum": [
-                        "GNSS",
-                        "Transducer",
-                        "ReferencePlace"
+                        "algorithm"
                     ],
                     "type": "string"
                 }
             },
+            "required": [
+                "type",
+                "timestamp",
+                "detail"
+            ],
             "type": "object"
         },
-        "ProcessingAlgorithm": {
-            "description": "General algorithm used to triage data",
+        "ProcessingCRS": {
+            "description": "Processing that transformed the reference system of the data. Must include the original and destination coordinate reference system, and the method used to change.",
             "properties": {
-                "comment": {
-                    "description": "Explanatory text related to algorithm or its outputs",
-                    "type": "string"
-                },
-                "name": {
-                    "description": "Examples: deduplicate, uncertainty estimation, manual editing",
-                    "type": "string"
-                },
-                "parameters": {
-                    "description": "Parameters used in data processing.",
-                    "type": [
-                        "null",
-                        "object"
-                    ]
-                },
-                "source": {
-                    "description": "Source (e.g., project, library) of the algorithm applied",
-                    "type": "string"
+                "detail": {
+                    "properties": {
+                        "comment": {
+                            "description": "Comments regarding method used to change coordinates (e.g., GeoTrans).",
+                            "type": "string"
+                        },
+                        "type": {
+                            "enum": [
+                                "EPSG"
+                            ],
+                            "type": "string"
+                        },
+                        "value": {
+                            "$ref": "#/definitions/EPSG_Number"
+                        }
+                    },
+                    "required": [
+                        "type",
+                        "value",
+                        "comment"
+                    ],
+                    "type": "object"
                 },
                 "timestamp": {
                     "$ref": "#/definitions/RFC3339_time"
                 },
                 "type": {
                     "enum": [
-                        "Algorithm"
+                        "CRS"
                     ],
                     "type": "string"
-                },
-                "version": {
-                    "description": "Version of algorithm used to triage data.",
-                    "type": "string"
                 }
             },
             "required": [
                 "type",
                 "timestamp",
-                "name"
+                "detail"
             ],
             "type": "object"
         },
-        "ProcessingCoordinateReferenceChange": {
-            "description": "Processing that changed the reference system of the data. Must include the original and destination coordinate reference system, and the method used to change.",
+        "ProcessingCRSTransformation": {
+            "description": "Processing that transformed the reference system of the data. Must include the original and destination coordinate reference system, and the method used to change.",
             "properties": {
-                "destination": {
-                    "description": "Coordinate reference system to which data were transformed (e.g., EPSG:8252).",
-                    "type": "string"
-                },
-                "method": {
-                    "description": "Method used to change coordinates (e.g., GeoTrans).",
-                    "type": "string"
-                },
-                "original": {
-                    "description": "Original coordinate reference system of the data (e.g., EPSG:4326).",
-                    "type": "string"
+                "detail": {
+                    "properties": {
+                        "destination": {
+                            "$ref": "#/definitions/CRS_Name"
+                        },
+                        "method": {
+                            "description": "Method used to change coordinates (e.g., GeoTrans).",
+                            "type": "string"
+                        },
+                        "origin": {
+                            "$ref": "#/definitions/CRS_Name"
+                        }
+                    },
+                    "required": [
+                        "origin",
+                        "destination",
+                        "method"
+                    ],
+                    "type": "object"
                 },
                 "timestamp": {
                     "$ref": "#/definitions/RFC3339_time"
                 },
                 "type": {
                     "enum": [
-                        "CRSChange"
+                        "CRSTransformation"
                     ],
                     "type": "string"
                 }
             },
             "required": [
                 "type",
                 "timestamp",
-                "original",
-                "destination"
+                "detail"
             ],
             "type": "object"
         },
         "ProcessingGNSS": {
             "description": "Steps taken to post-process or improve horizontal and vertical positioning.",
             "properties": {
-                "algorithm": {
-                    "description": "Algorithm used for GNSS post-processing",
-                    "enum": [
-                        "RTKLib",
-                        "CSRS-PPP"
+                "detail": {
+                    "properties": {
+                        "algorithm": {
+                            "description": "Algorithm used for GNSS post-processing, e.g., RTKLib | CSRS-PPP | ...",
+                            "type": "string"
+                        },
+                        "comment": {
+                            "description": "Comments regarding the algorithm used for GNSS processing.",
+                            "type": "string"
+                        },
+                        "version": {
+                            "description": "Version of GNSS post-processing algorithm method used.",
+                            "type": "string"
+                        }
+                    },
+                    "required": [
+                        "algorithm",
+                        "version",
+                        "comment"
                     ],
-                    "type": "string"
+                    "type": "object"
                 },
                 "timestamp": {
                     "$ref": "#/definitions/RFC3339_time"
                 },
                 "type": {
                     "enum": [
-                        "GNSS"
+                        "GNSSProcessing"
                     ],
                     "type": "string"
-                },
-                "version": {
-                    "description": "Version of GNSS post-processing algoritm method used.",
-                    "type": "string"
                 }
             },
             "required": [
                 "type",
                 "timestamp",
-                "algorithm"
+                "detail"
             ],
             "type": "object"
         },
         "ProcessingSoundSpeedCorrection": {
             "description": "Correction to soundings for sound speed in the water.",
             "properties": {
-                "method": {
-                    "description": "Method of sounding correction.",
-                    "type": "string"
-                },
-                "source": {
-                    "description": "Source of correction to soundings.",
-                    "type": "string"
+                "detail": {
+                    "properties": {
+                        "algorithm": {
+                            "description": "Algorithm for sound speed correction, e.g., CIDCO-Ocean | Raytraced | ...",
+                            "type": "string"
+                        },
+                        "comment": {
+                            "description": "Comments regarding the algorithm used for sound speed correction.",
+                            "type": "string"
+                        },
+                        "source": {
+                            "description": "Source of correction to soundings, e.g., Model | Profile | GeometricMean | Fixed | CarterTable | MatthewTable | WOA13 |...",
+                            "type": "string"
+                        },
+                        "version": {
+                            "description": "Version of sound speed algorithm method used.",
+                            "type": "string"
+                        }
+                    },
+                    "required": [
+                        "source",
+                        "algorithm",
+                        "version",
+                        "comment"
+                    ],
+                    "type": "object"
                 },
                 "timestamp": {
                     "$ref": "#/definitions/RFC3339_time"
                 },
                 "type": {
                     "enum": [
-                        "SoundSpeed"
+                        "SoundSpeedCorrection"
                     ],
                     "type": "string"
-                },
-                "version": {
-                    "description": "Version of sounding correction method used.",
-                    "type": "string"
                 }
             },
             "required": [
                 "type",
                 "timestamp",
-                "source",
-                "method"
+                "detail"
             ],
             "type": "object"
         },
         "ProcessingTimeStampInterpolation": {
             "description": "Method by which times are assigned to data being recorded.",
             "properties": {
-                "algorithm": {
-                    "description": "Algorithm used to interpolate timestamps.",
-                    "type": "string"
-                },
-                "method": {
-                    "description": "Name of timestamp interpolation method.",
-                    "type": "string"
+                "detail": {
+                    "properties": {
+                        "comment": {
+                            "description": "Comments regarding the source and method of time interpolation.",
+                            "type": "string"
+                        },
+                        "method": {
+                            "description": "The method of time interpolation, e.g., Midway | ElapsedTime | DataSource | NTP | PTP | ...",
+                            "type": "string"
+                        },
+                        "source": {
+                            "description": "The source of the time interpolation, e.g., SystemTime | ZDA | RMC | ...",
+                            "type": "string"
+                        }
+                    },
+                    "required": [
+                        "source",
+                        "method",
+                        "comment"
+                    ],
+                    "type": "object"
                 },
                 "timestamp": {
                     "$ref": "#/definitions/RFC3339_time"
                 },
                 "type": {
                     "enum": [
-                        "soundSpeed"
+                        "TimeInterpolation"
                     ],
                     "type": "string"
-                },
-                "version": {
-                    "description": "Version of timestamp interpolation method used.",
-                    "type": "string"
                 }
             },
             "required": [
                 "type",
                 "timestamp",
-                "method"
+                "detail"
             ],
             "type": "object"
         },
         "ProcessingVerticalReduction": {
             "description": "Steps taken to reduce raw data to a vertical reference system (Chart Datum, MSL, ellipsoid, water level, etc.). Must include the vertical reference system, and method used.",
             "properties": {
-                "datum": {
-                    "description": "Datum of vertical reference system.",
-                    "type": "string"
-                },
-                "method": {
-                    "description": "Method used to reduce raw data to vertical reference system.",
-                    "enum": [
-                        "EllipsoidReduction",
-                        "Observed Waterlevel",
-                        "Predicted Waterlevel"
+                "detail": {
+                    "properties": {
+                        "comment": {
+                            "description": "Comments regarding the vertical reduction.",
+                            "type": "string"
+                        },
+                        "method": {
+                            "description": "Method used to reduce raw data to vertical reference system, e.g., ObservedWL | PredictedWL | ModelledWL | EllipsoidReduction | ...",
+                            "type": "string"
+                        },
+                        "model": {
+                            "description": "Model used for reduction of raw data to vertical reference system, e.g., CANNORTH2016v1HyVSEP_NAD83v6_CD | StationReference | VDatum | VORF | ...",
+                            "type": "string"
+                        },
+                        "reference": {
+                            "description": "Vertical reference system, e.g., Chart Datum, MSL, ellipsoid, water level, etc.",
+                            "type": "string"
+                        }
+                    },
+                    "required": [
+                        "reference",
+                        "method",
+                        "model",
+                        "comment"
                     ],
-                    "type": "string"
-                },
-                "model": {
-                    "description": "Model used for reduction of raw data to vertical reference system",
-                    "type": "string"
-                },
-                "reference": {
-                    "description": "Vertical reference system (e.g., Chart Datum, MSL, ellipsoid, water level, etc.)",
-                    "type": "string"
+                    "type": "object"
                 },
                 "timestamp": {
                     "$ref": "#/definitions/RFC3339_time"
                 },
                 "type": {
                     "enum": [
                         "VerticalReduction"
                     ],
                     "type": "string"
                 }
             },
             "required": [
                 "type",
                 "timestamp",
-                "reference",
-                "datum",
-                "method"
+                "detail"
+            ],
+            "type": "object"
+        },
+        "ProviderContactPoint": {
+            "properties": {
+                "email": {
+                    "description": "A free-text field for the Trusted Node\u2019s email address, so that data users can contact the Trusted Node with questions about the data.",
+                    "pattern": "^[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\\.[A-Za-z]{2,6}$",
+                    "type": "string"
+                },
+                "logger": {
+                    "description": "The software program or hardware logger used to log the data.",
+                    "type": "string"
+                },
+                "loggerVersion": {
+                    "description": "The software or hardware logger version.",
+                    "type": "string"
+                },
+                "orgName": {
+                    "description": "The Trusted Node\u2019s name, in free-text format.",
+                    "type": "string"
+                }
+            },
+            "required": [
+                "orgName",
+                "email",
+                "logger",
+                "loggerVersion"
             ],
             "type": "object"
         },
         "RFC3339_time": {
-            "description": "RFC3339 UTC time stamp",
-            "pattern": "^([0-9]+)-(0[1-9]|1[012])-(0[1-9]|[12][0-9]|3[01])[Tt]([01][0-9]|2[0-3]):([0-5][0-9]):([0-5][0-9]|60)([.][0-9]+)?[Zz]$",
+            "description": "RFC3339 UTC time stamp (note: version 3.0.0 allows timezone naive timestamps).",
+            "pattern": "^([0-9]+)-(0[1-9]|1[012])-(0[1-9]|[12][0-9]|3[01])[Tt]([01][0-9]|2[0-3]):([0-5][0-9]):([0-5][0-9]|60)([.][0-9]+)?[Zz]?$",
             "type": "string"
         },
         "SensorDescriptionGNSS": {
             "properties": {
-                "antennaModel": {
-                    "description": "Model of GNSS antenna",
-                    "type": "string"
-                },
                 "make": {
                     "$ref": "#/definitions/SensorMake"
                 },
                 "model": {
                     "$ref": "#/definitions/SensorModel"
                 },
                 "position": {
@@ -521,15 +545,15 @@
                     "$ref": "#/definitions/SensorModel"
                 },
                 "position": {
                     "$ref": "#/definitions/SensorPosition"
                 },
                 "type": {
                     "enum": [
-                        "IMU"
+                        "MotionSensor"
                     ],
                     "type": "string"
                 }
             },
             "required": [
                 "type",
                 "make",
@@ -540,34 +564,30 @@
         },
         "SensorDescriptionSounder": {
             "properties": {
                 "draft": {
                     "description": "Draft of vessel",
                     "type": "number"
                 },
-                "draftUncert": {
-                    "description": "Uncertainty in vessel draft",
-                    "type": "number"
-                },
                 "frequency": {
                     "description": "Frequency of echo sounder",
                     "type": "number"
                 },
                 "make": {
                     "$ref": "#/definitions/SensorMake"
                 },
                 "model": {
                     "$ref": "#/definitions/SensorModel"
                 },
                 "position": {
                     "$ref": "#/definitions/SensorPosition"
                 },
-                "pulseLength": {
-                    "description": "Pulse length of echo sounder",
-                    "type": "number"
+                "transducer": {
+                    "description": "Transducer used with echo sounder",
+                    "type": "string"
                 },
                 "type": {
                     "enum": [
                         "Sounder"
                     ],
                     "type": "string"
                 }
@@ -593,89 +613,82 @@
             "items": {
                 "type": "number"
             },
             "maxItems": 3,
             "minItems": 3,
             "type": "array"
         },
-        "TrustedNodePlatform": {
+        "UniqueVesselID": {
+            "description": "Generated by the Trusted Node, this number identifies the Trusted Node and uniquely identifies the contributing vessel. The characters preceding the hyphen (-) identify the Trusted Node, followed by a hyphen (-), and then the vessel\u2019s unique identifier. The UUID assigned by the Trusted Node is consistent for each contributing vessel, throughout the life of service of the vessel. However, if the vessel chooses to remain anonymous to data users, the Trusted Node does not need to publish the vessel name in association with the UUID.",
+            "pattern": "^([0-9a-zA-Z]{2,}(-[0-9a-zA-Z]{2,})+)$",
+            "type": "string"
+        }
+    },
+    "properties": {
+        "algorithms": {
+            "$ref": "#/definitions/Algorithms"
+        },
+        "convention": {
+            "$ref": "#/definitions/Convention"
+        },
+        "crs": {
             "properties": {
-                "IDNumber": {
-                    "description": "The value for the ID Type. MMSI numbers are often nine digits, while IMO numbers are the letters \u201cIMO,\u201d followed by a seven-digit number.",
-                    "oneOf": [
-                        {
-                            "$ref": "#/definitions/IDNumber_MMSI"
+                "horizontal": {
+                    "properties": {
+                        "type": {
+                            "enum": [
+                                "EPSG"
+                            ],
+                            "type": "string"
                         },
-                        {
-                            "$ref": "#/definitions/IDNumber_IMO"
+                        "value": {
+                            "$ref": "#/definitions/EPSG_Number"
                         }
+                    },
+                    "required": [
+                        "type",
+                        "value"
                     ],
-                    "type": "string"
+                    "type": "object"
                 },
-                "IDType": {
-                    "description": "ID numbers used to uniquely identify vessels. Currently, only two types are available: Maritime Mobile Service Identity (MMSI) or International Maritime Organization (IMO) number. The MMSI number is used to uniquely identify a vessel through services such as AIS. The IMO number is linked to a vessel for its lifetime, regardless of change in flag or ownership. Contributors may select only one ID Type.",
+                "vertical": {
                     "enum": [
-                        "MMSI",
-                        "IMO"
+                        "Transducer"
                     ],
                     "type": "string"
-                },
-                "name": {
-                    "description": "The name of the vessel, in open string format.",
-                    "type": "string"
-                },
-                "providerEmail": {
-                    "description": "A free-text field for the Trusted Node\u2019s email address, so that data users can contact the Trusted Node with questions about the data.",
-                    "pattern": "^[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\\.[A-Za-z]{2,6}$",
-                    "type": "string"
-                },
-                "providerOrganizationName": {
-                    "description": "The Trusted Node\u2019s name, in free-text format.",
-                    "type": "string"
-                },
-                "type": {
-                    "description": "The type of vessel collecting the data, such as a cargo ship, fishing vessel, private vessel,\nresearch vessel, etc.",
-                    "type": "string"
-                },
-                "uniqueVesselID": {
-                    "description": "Generated by the Trusted Node, this number identifies the Trusted Node and uniquely identifies the contributing vessel. The characters preceding the hyphen (-) identify the Trusted Node, followed by a hyphen (-), and then the vessel\u2019s unique identifier. The UUID assigned by the Trusted Node is consistent for each contributing vessel, throughout the life of service of the vessel. However, if the vessel chooses to remain anonymous to data users, the Trusted Node does not need to publish the vessel name in association with the UUID.",
-                    "pattern": "^[a-zA-Z][a-zA-Z0-9]*-[0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{12}$",
-                    "type": "string"
                 }
             },
             "required": [
-                "providerOrganizationName",
-                "providerEmail",
-                "uniqueVesselID"
+                "horizontal",
+                "vertical"
             ],
             "type": "object"
-        }
-    },
-    "properties": {
-        "crs": {
-            "$ref": "#/definitions/CRS"
         },
-        "features": {
-            "items": {
-                "$ref": "#/definitions/GeoJSONFeature"
-            },
-            "type": "array"
+        "dataLicense": {
+            "$ref": "#/definitions/DataLicense"
+        },
+        "lineage": {
+            "$ref": "#/definitions/Processing"
+        },
+        "platform": {
+            "$ref": "#/definitions/Platform"
         },
-        "properties": {
-            "$ref": "#/definitions/B12_Metadata"
+        "providerContactPoint": {
+            "$ref": "#/definitions/ProviderContactPoint"
         },
         "type": {
             "enum": [
                 "FeatureCollection"
             ],
             "type": "string"
         }
     },
     "required": [
-        "type",
         "crs",
-        "properties",
-        "features"
+        "providerContactPoint",
+        "convention",
+        "dataLicense",
+        "platform"
     ],
-    "title": "Schema for Crowdsourced Bathymetry data and metadata, version 3.2.0-BETA",
+    "title": "Schema for Crowdsourced Bathymetry metadata (to accompany separate XYZ data), version 3.0.0",
     "type": "object"
 }
```

### Comparing `csbschema-1.0.5/csbschema/data/XYZ-CSB-schema-3_0_0-2023-03.json` & `csbschema-1.1.0/csbschema/data/CSB-schema-3_1_0-2023-08.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6948546691776633%*

 * *Differences: {"'$id'": "'https://raw.githubusercontent.com/CCOMJHC/csbschema/main/csbschema/data/CSB-schema-3_1_0-2023-08.json'",*

 * * "'definitions'": "{'RFC3339_time': {'description': 'RFC3339 UTC time stamp', 'pattern': "*

 * *                  "'^([0-9]+)-(0[1-9]|1[012])-(0[1-9]|[12][0-9]|3[01])[Tt]([01][0-9]|2[0-3]):([0-5][0-9]):([0-5][0-9]|60)([.][0-9]+)?[Zz]$'}, "*

 * *                  "'UniqueVesselID': {'pattern': "*

 * *                  "'^[a-zA-Z][a-zA-Z0-9]*-[0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-f […]*

```diff
@@ -1,122 +1,196 @@
 {
-    "$id": "https://raw.githubusercontent.com/CCOMJHC/csbschema/main/csbschema/data/XYZ-CSB-schema-3_0_0-2023-03.json",
+    "$id": "https://raw.githubusercontent.com/CCOMJHC/csbschema/main/csbschema/data/CSB-schema-3_1_0-2023-08.json",
     "$schema": "https://json-schema.org/draft/2020-12/schema",
     "definitions": {
-        "Algorithms": {
-            "description": "Array of algorithms applied to the data.",
-            "items": {
-                "required": [
-                    "name",
-                    "params"
-                ],
-                "type": "object"
+        "B12_Metadata": {
+            "properties": {
+                "platform": {
+                    "$ref": "#/definitions/Platform"
+                },
+                "processing": {
+                    "$ref": "#/definitions/Processing"
+                },
+                "trustedNode": {
+                    "$ref": "#/definitions/TrustedNode"
+                }
             },
-            "minItems": 1,
-            "type": "array"
+            "required": [
+                "trustedNode"
+            ],
+            "type": "object"
+        },
+        "CRS": {
+            "properties": {
+                "properties": {
+                    "properties": {
+                        "name": {
+                            "$ref": "#/definitions/CRS_Name"
+                        }
+                    },
+                    "required": [
+                        "name"
+                    ],
+                    "type": "object"
+                }
+            },
+            "required": [
+                "properties"
+            ],
+            "type": "object"
         },
         "CRS_Name": {
             "description": "CRS name as an EPSG string.",
             "pattern": "^EPSG:(3276[0-7]$|327[0-5]\\d$|32[0-6]\\d\\d$|3[0-1]\\d\\d\\d$|[1-2][0-9]{4}$|102[4-9]|10[3-9][0-9]$|1[1-9][0-9][0-9]$|[2-9][0-9][0-9][0-9]$)",
             "type": "string"
         },
-        "Convention": {
-            "description": "This field describes the format and version for the data and metadata, such as GeoJSON, CSV, or XYZT. Reference the version of the CSB data convention (e.g., CSB 2.0, CSB 3.0) where possible.",
-            "enum": [
-                "XYZ CSB 3.0"
+        "CSBDatum": {
+            "properties": {
+                "depth": {
+                    "description": "The distance from the vertical reference point to the seafloor. Should be collected as a positive value, in metres, with decimetre precision.",
+                    "type": "number"
+                },
+                "time": {
+                    "$ref": "#/definitions/RFC3339_time",
+                    "description": "The date and UTC time stamp for the depth measurement as well as can be determined, ideally to millisecond precision in RFC3339 format."
+                },
+                "uncertainty": {
+                    "description": "3-tuple composed of: horizontal X (i.e. east-to-west) uncertainty, horizontal Y (i.e. north-to-south) uncertainty, and vertical Z uncertainty (i.e. depth uncertainty)",
+                    "items": {
+                        "type": "number"
+                    },
+                    "maxItems": 3,
+                    "minItems": 3,
+                    "type": "array"
+                }
+            },
+            "required": [
+                "depth",
+                "time"
             ],
-            "type": "string"
+            "type": "object"
         },
-        "Correctors": {
+        "GeoJSONFeature": {
             "properties": {
-                "dataProcessed": {
-                    "description": "Raw data, without tidal corrections or additional processing, are preferable as a contribution to the IHO DCDB. This field allows the data contributor to state whether the data has been processed or corrected (\u2018True\u2019) or not (\u2018False\u2019). If \u2018True\u2019, it is strongly recommended that detailed information be captured in optional metadata fields as outlined in section 3.3.4. If \u2018False\u2019, information in section 3.3.4 is not needed.",
-                    "type": "boolean"
-                },
-                "draftApplied": {
-                    "description": "Describes whether vessel draft has been corrected for.",
-                    "type": "boolean"
+                "geometry": {
+                    "oneOf": [
+                        {
+                            "type": "null"
+                        },
+                        {
+                            "properties": {
+                                "bbox": {
+                                    "items": {
+                                        "type": "number"
+                                    },
+                                    "minItems": 4,
+                                    "type": "array"
+                                },
+                                "coordinates": {
+                                    "items": {
+                                        "type": "number"
+                                    },
+                                    "minItems": 2,
+                                    "type": "array"
+                                },
+                                "type": {
+                                    "enum": [
+                                        "Point"
+                                    ],
+                                    "type": "string"
+                                }
+                            },
+                            "required": [
+                                "type",
+                                "coordinates"
+                            ],
+                            "title": "GeoJSON Point",
+                            "type": "object"
+                        }
+                    ]
                 },
-                "motionOffsetsApplied": {
-                    "description": "Describes whether vessel motion has been corrected for.",
-                    "type": "boolean"
+                "id": {
+                    "oneOf": [
+                        {
+                            "type": "number"
+                        },
+                        {
+                            "type": "string"
+                        }
+                    ]
                 },
-                "positionOffsetsDocumented": {
-                    "description": "Describes whether the final vessel position (longitude and latitude) has been corrected for the lateral and longitudinal offsets between the GNSS receiver and the transducer (\u201cTrue\u201d), or if they were not (\u201cFalse\u201d). If \u201cTrue\u201d, the position element of the sensor description field in Table 3 should be populated.",
-                    "type": "boolean"
+                "properties": {
+                    "$ref": "#/definitions/CSBDatum"
                 },
-                "positionReferencePoint": {
+                "type": {
                     "enum": [
-                        "GNSS"
+                        "Feature"
                     ],
                     "type": "string"
-                },
-                "soundSpeedDocumented": {
-                    "description": "Some systems may have the ability to provide sound speed data and correct the sounding. If details regarding such corrections are known (\u201cTrue\u201d), it is strongly recommended that the \u2018Sound Speed Correction\u2019 field in Table 4 be populated. If \u201cFalse\u201d, no information about how sound speed was applied has been recorded.",
-                    "type": "boolean"
                 }
             },
             "required": [
-                "positionReferencePoint"
+                "type",
+                "properties",
+                "geometry"
             ],
+            "title": "GeoJSON Feature",
             "type": "object"
         },
-        "DataLicense": {
-            "description": "The license under which the Trusted Node is\n providing CSB data to the IHO DCDB.\n",
-            "type": "string"
-        },
-        "EPSG_Number": {
-            "maximum": 32767,
-            "minimum": 1024,
-            "type": "integer"
-        },
         "IDNumber_IMO": {
-            "maximum": 9999999,
-            "minimum": 1000000,
-            "type": "integer"
+            "pattern": "^IMO\\d{7}$",
+            "type": "string"
         },
         "IDNumber_MMSI": {
-            "maximum": 999999999,
-            "minimum": 100000000,
-            "type": "integer"
+            "pattern": "^\\d{9}$",
+            "type": "string"
         },
         "Platform": {
             "properties": {
                 "IDNumber": {
                     "description": "The value for the ID Type. MMSI numbers are often nine digits, while IMO numbers are the letters \u201cIMO,\u201d followed by a seven-digit number.",
                     "oneOf": [
                         {
                             "$ref": "#/definitions/IDNumber_MMSI"
                         },
                         {
                             "$ref": "#/definitions/IDNumber_IMO"
                         }
                     ],
-                    "type": "integer"
+                    "type": "string"
                 },
                 "IDType": {
                     "description": "ID numbers used to uniquely identify vessels. Currently, only two types are available: Maritime Mobile Service Identity (MMSI) or International Maritime Organization (IMO) number. The MMSI number is used to uniquely identify a vessel through services such as AIS. The IMO number is linked to a vessel for its lifetime, regardless of change in flag or ownership. Contributors may select only one ID Type.",
                     "enum": [
                         "MMSI",
                         "IMO"
                     ],
                     "type": "string"
                 },
-                "correctors": {
-                    "$ref": "#/definitions/Correctors"
+                "contributorComments": {
+                    "description": "If the contributor believes there were any problems or events that may have degraded the quality of the position or depth measurements, they can enter that information in this free-text field.",
+                    "type": "string"
+                },
+                "dataProcessed": {
+                    "description": "Raw data, without tidal corrections or additional processing, are preferable as a contribution to the IHO DCDB. This field allows the data contributor to state whether the data has been processed or corrected (\u2018True\u2019) or not (\u2018False\u2019). If \u2018True\u2019, it is strongly recommended that detailed information be captured in optional metadata fields as outlined in section 3.3.4. If \u2018False\u2019, information in section 3.3.4 is not needed.",
+                    "type": "boolean"
                 },
                 "length": {
                     "description": "The length overall (LOA) of the vessel, expressed as a positive value, in metres, to the nearest metre.",
                     "minimum": 1,
                     "type": "integer"
                 },
                 "name": {
                     "description": "The name of the vessel, in open string format.",
                     "type": "string"
                 },
+                "positionOffsetsDocumented": {
+                    "description": "Describes whether the final vessel position (longitude and latitude) has been corrected for the lateral and longitudinal offsets between the GNSS receiver and the transducer (\u201cTrue\u201d), or if they were not (\u201cFalse\u201d). If \u201cTrue\u201d, the position element of the sensor description field in Table 3 should be populated.",
+                    "type": "boolean"
+                },
                 "sensors": {
                     "description": "Composite element containing all information about a given sensor in use on the collection platform. Minimum specification of fields as shown; some sensors may have additional fields (e.g., frequency for an echo sounder). Position is given from the PRP (Position Reference Point) in metres. The offsets are positive NED (North (Bow), East (Starboard), Down)",
                     "items": {
                         "oneOf": [
                             {
                                 "$ref": "#/definitions/SensorDescriptionSounder"
                             },
@@ -127,396 +201,394 @@
                                 "$ref": "#/definitions/SensorDescriptionGNSS"
                             }
                         ]
                     },
                     "minItems": 1,
                     "type": "array"
                 },
+                "soundSpeedDocumented": {
+                    "description": "Some systems may have the ability to provide sound speed data and correct the sounding. If details regarding such corrections are known (\u201cTrue\u201d), it is strongly recommended that the \u2018Sound Speed Correction\u2019 field in Table 4 be populated. If \u201cFalse\u201d, no information about how sound speed was applied has been recorded.",
+                    "type": "boolean"
+                },
                 "type": {
                     "description": "The type of vessel collecting the data, such as a cargo ship, fishing vessel, private vessel,\nresearch vessel, etc.",
                     "type": "string"
                 },
                 "uniqueID": {
                     "$ref": "#/definitions/UniqueVesselID"
                 }
             },
             "required": [
-                "uniqueID",
-                "correctors"
+                "type",
+                "name",
+                "length",
+                "IDType",
+                "IDNumber",
+                "soundSpeedDocumented",
+                "positionOffsetsDocumented",
+                "dataProcessed"
             ],
             "type": "object"
         },
         "Processing": {
             "description": "List of processing steps recorded for the data",
             "items": {
                 "oneOf": [
                     {
                         "$ref": "#/definitions/ProcessingTimeStampInterpolation"
                     },
                     {
-                        "$ref": "#/definitions/ProcessingCRSTransformation"
-                    },
-                    {
-                        "$ref": "#/definitions/ProcessingCRS"
+                        "$ref": "#/definitions/ProcessingCoordinateReferenceChange"
                     },
                     {
                         "$ref": "#/definitions/ProcessingVerticalReduction"
                     },
                     {
                         "$ref": "#/definitions/ProcessingGNSS"
                     },
                     {
                         "$ref": "#/definitions/ProcessingSoundSpeedCorrection"
                     },
                     {
+                        "$ref": "#/definitions/ProcessingUncertainty"
+                    },
+                    {
+                        "$ref": "#/definitions/ProcessingVerticalOffsetAnalysis"
+                    },
+                    {
                         "$ref": "#/definitions/ProcessingAlgorithm"
                     }
                 ]
             },
             "minItems": 1,
             "type": "array"
         },
         "ProcessingAlgorithm": {
             "description": "General algorithm used to triage data",
             "properties": {
-                "detail": {
-                    "properties": {
-                        "comment": {
-                            "description": "Explanatory text related to algorithm or its outputs.",
-                            "type": "string"
-                        },
-                        "name": {
-                            "description": "Examples: deduplicate, uncertainty estimation, manual editing.",
-                            "type": "string"
-                        },
-                        "parameters": {
-                            "description": "Parameters used in data processing.",
-                            "type": "string"
-                        }
-                    },
-                    "required": [
-                        "name",
-                        "parameters",
-                        "comment"
-                    ],
-                    "type": "object"
+                "comment": {
+                    "description": "Explanatory text related to algorithm or its outputs",
+                    "type": "string"
+                },
+                "name": {
+                    "description": "Examples: deduplicate, uncertainty estimation, manual editing",
+                    "type": "string"
+                },
+                "parameters": {
+                    "description": "Parameters used in data processing.",
+                    "type": [
+                        "null",
+                        "object"
+                    ]
+                },
+                "source": {
+                    "description": "Source (e.g., project, library) of the algorithm applied",
+                    "type": "string"
                 },
                 "timestamp": {
                     "$ref": "#/definitions/RFC3339_time"
                 },
                 "type": {
                     "enum": [
-                        "algorithm"
+                        "Algorithm"
                     ],
                     "type": "string"
+                },
+                "version": {
+                    "description": "Version of algorithm used to triage data.",
+                    "type": "string"
                 }
             },
             "required": [
                 "type",
                 "timestamp",
-                "detail"
+                "name"
             ],
             "type": "object"
         },
-        "ProcessingCRS": {
-            "description": "Processing that transformed the reference system of the data. Must include the original and destination coordinate reference system, and the method used to change.",
+        "ProcessingCoordinateReferenceChange": {
+            "description": "Processing that changed the reference system of the data. Must include the original and destination coordinate reference system, and the method used to change.",
             "properties": {
-                "detail": {
-                    "properties": {
-                        "comment": {
-                            "description": "Comments regarding method used to change coordinates (e.g., GeoTrans).",
-                            "type": "string"
-                        },
-                        "type": {
-                            "enum": [
-                                "EPSG"
-                            ],
-                            "type": "string"
-                        },
-                        "value": {
-                            "$ref": "#/definitions/EPSG_Number"
-                        }
-                    },
-                    "required": [
-                        "type",
-                        "value",
-                        "comment"
-                    ],
-                    "type": "object"
+                "destination": {
+                    "description": "Coordinate reference system to which data were transformed (e.g., EPSG:8252).",
+                    "type": "string"
+                },
+                "method": {
+                    "description": "Method used to change coordinates (e.g., GeoTrans).",
+                    "type": "string"
+                },
+                "original": {
+                    "description": "Original coordinate reference system of the data (e.g., EPSG:4326).",
+                    "type": "string"
                 },
                 "timestamp": {
                     "$ref": "#/definitions/RFC3339_time"
                 },
                 "type": {
                     "enum": [
-                        "CRS"
+                        "CRSChange"
                     ],
                     "type": "string"
                 }
             },
             "required": [
                 "type",
                 "timestamp",
-                "detail"
+                "original",
+                "destination"
             ],
             "type": "object"
         },
-        "ProcessingCRSTransformation": {
-            "description": "Processing that transformed the reference system of the data. Must include the original and destination coordinate reference system, and the method used to change.",
+        "ProcessingGNSS": {
+            "description": "Steps taken to post-process or improve horizontal and vertical positioning.",
             "properties": {
-                "detail": {
-                    "properties": {
-                        "destination": {
-                            "$ref": "#/definitions/CRS_Name"
-                        },
-                        "method": {
-                            "description": "Method used to change coordinates (e.g., GeoTrans).",
-                            "type": "string"
-                        },
-                        "origin": {
-                            "$ref": "#/definitions/CRS_Name"
-                        }
-                    },
-                    "required": [
-                        "origin",
-                        "destination",
-                        "method"
+                "algorithm": {
+                    "description": "Algorithm used for GNSS post-processing",
+                    "enum": [
+                        "RTKLib",
+                        "CSRS-PPP"
                     ],
-                    "type": "object"
+                    "type": "string"
                 },
                 "timestamp": {
                     "$ref": "#/definitions/RFC3339_time"
                 },
                 "type": {
                     "enum": [
-                        "CRSTransformation"
+                        "GNSS"
                     ],
                     "type": "string"
+                },
+                "version": {
+                    "description": "Version of GNSS post-processing algoritm method used.",
+                    "type": "string"
                 }
             },
             "required": [
                 "type",
                 "timestamp",
-                "detail"
+                "algorithm"
             ],
             "type": "object"
         },
-        "ProcessingGNSS": {
-            "description": "Steps taken to post-process or improve horizontal and vertical positioning.",
+        "ProcessingSoundSpeedCorrection": {
+            "description": "Correction to soundings for sound speed in the water.",
             "properties": {
-                "detail": {
-                    "properties": {
-                        "algorithm": {
-                            "description": "Algorithm used for GNSS post-processing, e.g., RTKLib | CSRS-PPP | ...",
-                            "type": "string"
-                        },
-                        "comment": {
-                            "description": "Comments regarding the algorithm used for GNSS processing.",
-                            "type": "string"
-                        },
-                        "version": {
-                            "description": "Version of GNSS post-processing algorithm method used.",
-                            "type": "string"
-                        }
-                    },
-                    "required": [
-                        "algorithm",
-                        "version",
-                        "comment"
-                    ],
-                    "type": "object"
+                "method": {
+                    "description": "Method of sounding correction.",
+                    "type": "string"
+                },
+                "source": {
+                    "description": "Source of correction to soundings.",
+                    "type": "string"
                 },
                 "timestamp": {
                     "$ref": "#/definitions/RFC3339_time"
                 },
                 "type": {
                     "enum": [
-                        "GNSSProcessing"
+                        "SoundSpeed"
                     ],
                     "type": "string"
+                },
+                "version": {
+                    "description": "Version of sounding correction method used.",
+                    "type": "string"
                 }
             },
             "required": [
                 "type",
                 "timestamp",
-                "detail"
+                "source",
+                "method"
             ],
             "type": "object"
         },
-        "ProcessingSoundSpeedCorrection": {
-            "description": "Correction to soundings for sound speed in the water.",
+        "ProcessingTimeStampInterpolation": {
+            "description": "Method by which times are assigned to data being recorded.",
             "properties": {
-                "detail": {
-                    "properties": {
-                        "algorithm": {
-                            "description": "Algorithm for sound speed correction, e.g., CIDCO-Ocean | Raytraced | ...",
-                            "type": "string"
-                        },
-                        "comment": {
-                            "description": "Comments regarding the algorithm used for sound speed correction.",
-                            "type": "string"
-                        },
-                        "source": {
-                            "description": "Source of correction to soundings, e.g., Model | Profile | GeometricMean | Fixed | CarterTable | MatthewTable | WOA13 |...",
-                            "type": "string"
-                        },
-                        "version": {
-                            "description": "Version of sound speed algorithm method used.",
-                            "type": "string"
-                        }
-                    },
-                    "required": [
-                        "source",
-                        "algorithm",
-                        "version",
-                        "comment"
-                    ],
-                    "type": "object"
+                "algorithm": {
+                    "description": "Algorithm used to interpolate timestamps.",
+                    "type": "string"
+                },
+                "method": {
+                    "description": "Name of timestamp interpolation method.",
+                    "type": "string"
                 },
                 "timestamp": {
                     "$ref": "#/definitions/RFC3339_time"
                 },
                 "type": {
                     "enum": [
-                        "SoundSpeedCorrection"
+                        "soundSpeed"
                     ],
                     "type": "string"
+                },
+                "version": {
+                    "description": "Version of timestamp interpolation method used.",
+                    "type": "string"
                 }
             },
             "required": [
                 "type",
                 "timestamp",
-                "detail"
+                "method"
             ],
             "type": "object"
         },
-        "ProcessingTimeStampInterpolation": {
-            "description": "Method by which times are assigned to data being recorded.",
+        "ProcessingUncertainty": {
+            "description": "Algorithm for estimating horizontal and vertical uncertainty of soundings.",
             "properties": {
-                "detail": {
-                    "properties": {
-                        "comment": {
-                            "description": "Comments regarding the source and method of time interpolation.",
-                            "type": "string"
-                        },
-                        "method": {
-                            "description": "The method of time interpolation, e.g., Midway | ElapsedTime | DataSource | NTP | PTP | ...",
-                            "type": "string"
-                        },
-                        "source": {
-                            "description": "The source of the time interpolation, e.g., SystemTime | ZDA | RMC | ...",
-                            "type": "string"
-                        }
-                    },
-                    "required": [
-                        "source",
-                        "method",
-                        "comment"
-                    ],
+                "comment": {
+                    "description": "Explanatory text related to uncertainty estimation algorithm or its inputs/outputs",
+                    "type": "string"
+                },
+                "name": {
+                    "description": "Name of uncertainty estimation algorithm",
+                    "type": "string"
+                },
+                "parameters": {
+                    "description": "Parameters used in application of uncertainty estimation algorithm.",
                     "type": "object"
                 },
+                "reference": {
+                    "description": "Source (e.g., paper, project, library) of the algorithm applied. Formats can be: DOI, URL or other.",
+                    "type": "string"
+                },
                 "timestamp": {
                     "$ref": "#/definitions/RFC3339_time"
                 },
                 "type": {
                     "enum": [
-                        "TimeInterpolation"
+                        "Uncertainty"
                     ],
                     "type": "string"
+                },
+                "version": {
+                    "description": "Version of uncertainty estimation algorithm used.",
+                    "type": "string"
                 }
             },
             "required": [
                 "type",
                 "timestamp",
-                "detail"
+                "name",
+                "parameters",
+                "version",
+                "comment",
+                "reference"
             ],
             "type": "object"
         },
-        "ProcessingVerticalReduction": {
-            "description": "Steps taken to reduce raw data to a vertical reference system (Chart Datum, MSL, ellipsoid, water level, etc.). Must include the vertical reference system, and method used.",
+        "ProcessingVerticalOffsetAnalysis": {
+            "description": "Analysis of vertical offsets of soundings recorded by intersecting track lines.",
             "properties": {
-                "detail": {
-                    "properties": {
-                        "comment": {
-                            "description": "Comments regarding the vertical reduction.",
-                            "type": "string"
-                        },
-                        "method": {
-                            "description": "Method used to reduce raw data to vertical reference system, e.g., ObservedWL | PredictedWL | ModelledWL | EllipsoidReduction | ...",
-                            "type": "string"
-                        },
-                        "model": {
-                            "description": "Model used for reduction of raw data to vertical reference system, e.g., CANNORTH2016v1HyVSEP_NAD83v6_CD | StationReference | VDatum | VORF | ...",
-                            "type": "string"
-                        },
-                        "reference": {
-                            "description": "Vertical reference system, e.g., Chart Datum, MSL, ellipsoid, water level, etc.",
-                            "type": "string"
-                        }
+                "analysis": {
+                    "items": {
+                        "$ref": "#/definitions/VerticalOffsetAnalysisAnalysisMeta"
                     },
-                    "required": [
-                        "reference",
-                        "method",
-                        "model",
-                        "comment"
-                    ],
-                    "type": "object"
+                    "minItems": 1,
+                    "type": "array"
+                },
+                "comment": {
+                    "description": "Explanatory text related to vertical offset analysis algorithm or its inputs/outputs",
+                    "type": "string"
+                },
+                "name": {
+                    "description": "Name of vertical offset analysis algorithm.",
+                    "type": "string"
+                },
+                "offsets": {
+                    "items": {
+                        "$ref": "#/definitions/VerticalOffsetAnalysisOffset"
+                    },
+                    "minItems": 1,
+                    "type": "array"
+                },
+                "reference": {
+                    "description": "Source (e.g., paper, project, library) of the algorithm applied. Formats can be: DOI, URL or other.",
+                    "type": "string"
                 },
                 "timestamp": {
                     "$ref": "#/definitions/RFC3339_time"
                 },
                 "type": {
                     "enum": [
-                        "VerticalReduction"
+                        "VerticalOffsetAnalysis"
                     ],
                     "type": "string"
+                },
+                "version": {
+                    "description": "Version of vertical offset analysis algorithm used.",
+                    "type": "string"
                 }
             },
             "required": [
                 "type",
                 "timestamp",
-                "detail"
+                "name",
+                "version",
+                "offsets"
             ],
             "type": "object"
         },
-        "ProviderContactPoint": {
+        "ProcessingVerticalReduction": {
+            "description": "Steps taken to reduce raw data to a vertical reference system (Chart Datum, MSL, ellipsoid, water level, etc.). Must include the vertical reference system, and method used.",
             "properties": {
-                "email": {
-                    "description": "A free-text field for the Trusted Node\u2019s email address, so that data users can contact the Trusted Node with questions about the data.",
-                    "pattern": "^[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\\.[A-Za-z]{2,6}$",
+                "datum": {
+                    "description": "Datum of vertical reference system.",
                     "type": "string"
                 },
-                "logger": {
-                    "description": "The software program or hardware logger used to log the data.",
+                "method": {
+                    "description": "Method used to reduce raw data to vertical reference system.",
+                    "enum": [
+                        "EllipsoidReduction",
+                        "Observed Waterlevel",
+                        "Predicted Waterlevel"
+                    ],
                     "type": "string"
                 },
-                "loggerVersion": {
-                    "description": "The software or hardware logger version.",
+                "model": {
+                    "description": "Model used for reduction of raw data to vertical reference system",
                     "type": "string"
                 },
-                "orgName": {
-                    "description": "The Trusted Node\u2019s name, in free-text format.",
+                "reference": {
+                    "description": "Vertical reference system (e.g., Chart Datum, MSL, ellipsoid, water level, etc.)",
+                    "type": "string"
+                },
+                "timestamp": {
+                    "$ref": "#/definitions/RFC3339_time"
+                },
+                "type": {
+                    "enum": [
+                        "VerticalReduction"
+                    ],
                     "type": "string"
                 }
             },
             "required": [
-                "orgName",
-                "email",
-                "logger",
-                "loggerVersion"
+                "type",
+                "timestamp",
+                "reference",
+                "datum",
+                "method"
             ],
             "type": "object"
         },
         "RFC3339_time": {
-            "description": "RFC3339 UTC time stamp (note: version 3.0.0 allows timezone naive timestamps).",
-            "pattern": "^([0-9]+)-(0[1-9]|1[012])-(0[1-9]|[12][0-9]|3[01])[Tt]([01][0-9]|2[0-3]):([0-5][0-9]):([0-5][0-9]|60)([.][0-9]+)?[Zz]?$",
+            "description": "RFC3339 UTC time stamp",
+            "pattern": "^([0-9]+)-(0[1-9]|1[012])-(0[1-9]|[12][0-9]|3[01])[Tt]([01][0-9]|2[0-3]):([0-5][0-9]):([0-5][0-9]|60)([.][0-9]+)?[Zz]$",
             "type": "string"
         },
         "SensorDescriptionGNSS": {
             "properties": {
+                "antennaModel": {
+                    "description": "Model of GNSS antenna",
+                    "type": "string"
+                },
                 "make": {
                     "$ref": "#/definitions/SensorMake"
                 },
                 "model": {
                     "$ref": "#/definitions/SensorModel"
                 },
                 "position": {
@@ -545,15 +617,15 @@
                     "$ref": "#/definitions/SensorModel"
                 },
                 "position": {
                     "$ref": "#/definitions/SensorPosition"
                 },
                 "type": {
                     "enum": [
-                        "MotionSensor"
+                        "IMU"
                     ],
                     "type": "string"
                 }
             },
             "required": [
                 "type",
                 "make",
@@ -564,30 +636,34 @@
         },
         "SensorDescriptionSounder": {
             "properties": {
                 "draft": {
                     "description": "Draft of vessel",
                     "type": "number"
                 },
+                "draftUncert": {
+                    "description": "Uncertainty in vessel draft",
+                    "type": "number"
+                },
                 "frequency": {
                     "description": "Frequency of echo sounder",
                     "type": "number"
                 },
                 "make": {
                     "$ref": "#/definitions/SensorMake"
                 },
                 "model": {
                     "$ref": "#/definitions/SensorModel"
                 },
                 "position": {
                     "$ref": "#/definitions/SensorPosition"
                 },
-                "transducer": {
-                    "description": "Transducer used with echo sounder",
-                    "type": "string"
+                "pulseLength": {
+                    "description": "Pulse length of echo sounder",
+                    "type": "number"
                 },
                 "type": {
                     "enum": [
                         "Sounder"
                     ],
                     "type": "string"
                 }
@@ -613,82 +689,161 @@
             "items": {
                 "type": "number"
             },
             "maxItems": 3,
             "minItems": 3,
             "type": "array"
         },
+        "TrustedNode": {
+            "properties": {
+                "convention": {
+                    "description": "This field describes the format and version for the data and metadata, such as GeoJSON, CSV, or XYZT. Reference the version of the CSB data convention (e.g., CSB 2.0, CSB 3.0) where possible.",
+                    "enum": [
+                        "GeoJSON CSB 3.1"
+                    ],
+                    "type": "string"
+                },
+                "dataLicense": {
+                    "description": "The Creative Commons public domain\n dedication under which the Trusted Node is\n providing CSB data to the IHO DCDB.\n ",
+                    "type": "string"
+                },
+                "navigationCRS": {
+                    "$ref": "#/definitions/CRS_Name",
+                    "description": "The EPSG code referring to the Coordinate Reference System (CRS) of the navigation data"
+                },
+                "providerEmail": {
+                    "description": "A free-text field for the Trusted Node\u2019s email address, so that data users can contact the Trusted Node with questions about the data.",
+                    "pattern": "^[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\\.[A-Za-z]{2,6}$",
+                    "type": "string"
+                },
+                "providerLogger": {
+                    "description": "The software program or hardware logger used to log the data.",
+                    "type": "string"
+                },
+                "providerLoggerVersion": {
+                    "description": "The software or hardware logger version.",
+                    "type": "string"
+                },
+                "providerOrganizationName": {
+                    "description": "The Trusted Node\u2019s name, in free-text format.",
+                    "type": "string"
+                },
+                "uniqueVesselID": {
+                    "$ref": "#/definitions/UniqueVesselID"
+                },
+                "verticalReferenceOfDepth": {
+                    "description": "The vertical reference of the depth. The vertical reference will most likely be the transducer (ex: NMEA DBT string) or the waterline (ex: NMEA DPT string).",
+                    "enum": [
+                        "Transducer",
+                        "Waterline",
+                        "Unknown"
+                    ],
+                    "type": "string"
+                },
+                "vesselPositionReferencePoint": {
+                    "description": "Position Reference Point (PRP) is the reference point where the navigation data is output. Most likely the reference point will be the location of the GNSS antenna.",
+                    "enum": [
+                        "GNSS",
+                        "Transducer",
+                        "ReferencePlace"
+                    ],
+                    "type": "string"
+                }
+            },
+            "required": [
+                "providerOrganizationName",
+                "providerEmail",
+                "uniqueVesselID",
+                "convention",
+                "dataLicense",
+                "providerLogger",
+                "providerLoggerVersion",
+                "navigationCRS",
+                "verticalReferenceOfDepth",
+                "vesselPositionReferencePoint"
+            ],
+            "type": "object"
+        },
         "UniqueVesselID": {
             "description": "Generated by the Trusted Node, this number identifies the Trusted Node and uniquely identifies the contributing vessel. The characters preceding the hyphen (-) identify the Trusted Node, followed by a hyphen (-), and then the vessel\u2019s unique identifier. The UUID assigned by the Trusted Node is consistent for each contributing vessel, throughout the life of service of the vessel. However, if the vessel chooses to remain anonymous to data users, the Trusted Node does not need to publish the vessel name in association with the UUID.",
-            "pattern": "^([0-9a-zA-Z]{2,}(-[0-9a-zA-Z]{2,})+)$",
+            "pattern": "^[a-zA-Z][a-zA-Z0-9]*-[0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{12}$",
             "type": "string"
-        }
-    },
-    "properties": {
-        "algorithms": {
-            "$ref": "#/definitions/Algorithms"
         },
-        "convention": {
-            "$ref": "#/definitions/Convention"
-        },
-        "crs": {
+        "VerticalOffsetAnalysisAnalysisMeta": {
             "properties": {
-                "horizontal": {
-                    "properties": {
-                        "type": {
-                            "enum": [
-                                "EPSG"
-                            ],
-                            "type": "string"
-                        },
-                        "value": {
-                            "$ref": "#/definitions/EPSG_Number"
-                        }
-                    },
-                    "required": [
-                        "type",
-                        "value"
-                    ],
+                "comment": {
+                    "description": "Explanatory text related to analysis or its inputs/outputs",
+                    "type": "string"
+                },
+                "name": {
+                    "type": "string"
+                },
+                "parameters": {
                     "type": "object"
                 },
-                "vertical": {
-                    "enum": [
-                        "Transducer"
-                    ],
+                "pass": {
+                    "type": "boolean"
+                },
+                "reference": {
+                    "description": "Source (e.g., paper, project, library) of the algorithm applied. Formats can be: DOI, URL or other.",
                     "type": "string"
                 }
             },
             "required": [
-                "horizontal",
-                "vertical"
+                "name",
+                "pass",
+                "parameters"
             ],
             "type": "object"
         },
-        "dataLicense": {
-            "$ref": "#/definitions/DataLicense"
-        },
-        "lineage": {
-            "$ref": "#/definitions/Processing"
+        "VerticalOffsetAnalysisOffset": {
+            "properties": {
+                "delta": {
+                    "type": "number"
+                },
+                "x": {
+                    "type": "number"
+                },
+                "y": {
+                    "type": "number"
+                },
+                "z": {
+                    "type": "number"
+                }
+            },
+            "required": [
+                "x",
+                "y",
+                "delta"
+            ],
+            "type": "object"
+        }
+    },
+    "properties": {
+        "crs": {
+            "$ref": "#/definitions/CRS"
         },
-        "platform": {
-            "$ref": "#/definitions/Platform"
+        "features": {
+            "items": {
+                "$ref": "#/definitions/GeoJSONFeature"
+            },
+            "type": "array"
         },
-        "providerContactPoint": {
-            "$ref": "#/definitions/ProviderContactPoint"
+        "properties": {
+            "$ref": "#/definitions/B12_Metadata"
         },
         "type": {
             "enum": [
                 "FeatureCollection"
             ],
             "type": "string"
         }
     },
     "required": [
+        "type",
         "crs",
-        "providerContactPoint",
-        "convention",
-        "dataLicense",
-        "platform"
+        "properties",
+        "features"
     ],
-    "title": "Schema for Crowdsourced Bathymetry metadata (to accompany separate XYZ data), version 3.0.0",
+    "title": "Schema for Crowdsourced Bathymetry data and metadata, version 3.1.0",
     "type": "object"
 }
```

### Comparing `csbschema-1.0.5/csbschema/validators.py` & `csbschema-1.1.0/csbschema/validators.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+from __future__ import annotations
+
 import sys
 import mmap
 import json
 from pathlib import Path
-from typing import Tuple, Union, List
+from typing import Tuple, Union, List, Optional
+from collections.abc import Callable
 import re
 from importlib import resources
 
 import jsonschema
 from jsonschema import Draft202012Validator
 
 ID_NUMBER_MMSI_RE = re.compile(r"^\d{9}$")
@@ -49,34 +52,164 @@
 
 def _open_document(document_path: Union[Path, str]) -> Union[dict, list]:
     with open(document_path, 'rb') as f:
         with mmap.mmap(f.fileno(), length=0, access=mmap.ACCESS_READ) as mm:
             return json.load(mm)
 
 
-def validate_b12_3_0_0_2023_03(document_path: Union[Path, str]) -> Tuple[bool, dict]:
+def _get_properties(document: dict, errors: List, *,
+                    not_found_mesg: Optional[str] = None) -> Optional[dict]:
+    if 'properties' not in document:
+        mesg = not_found_mesg
+        if mesg is None:
+            mesg = "'properties' property is needed for semantic validation, but was not found."
+        errors.append(_error_factory('/',
+                                     mesg))
+        return None
+    return document['properties']
+
+
+def _get_properties_processing(properties: dict, errors: List, *,
+                               not_found_mesg: Optional[str] = None,
+                               context_path: str = '/properties') -> Optional[dict]:
+    if 'processing' not in properties:
+        mesg = not_found_mesg
+        if mesg is None:
+            mesg = "'processing' property is needed for semantic validation, but was not found."
+        errors.append(_error_factory(context_path,
+                                     mesg))
+        return None
+    return properties['processing']
+
+
+def _get_properties_obs_coll_processing(properties: dict, errors: List, *,
+                                        not_found_mesg: Optional[str] = None) -> Optional[dict]:
+    if 'observationCollection' not in properties:
+        mesg = not_found_mesg
+        if mesg is None:
+            mesg = "'observationCollection' property is needed for semantic validation, but was not found."
+        errors.append(_error_factory('/properties',
+                                     mesg))
+        return None
+
+    observationCollection = properties['observationCollection']
+
+    return _get_properties_processing(properties['observationCollection'], errors,
+                                      context_path='/properties/observationCollection')
+
+
+def _get_lineage(document: dict, errors: List, *,
+                 not_found_mesg: Optional[str] = None) -> Optional[dict]:
+    if 'lineage' not in document:
+        mesg = not_found_mesg
+        if mesg is None:
+            mesg = "'lineage' property is needed for semantic validation, but was not found."
+        errors.append(_error_factory('/',
+                                     mesg))
+        return None
+    return document['lineage']
+
+
+def _get_features(document: dict, errors: List, *,
+                  not_found_mesg: Optional[str] = None) -> Optional[dict]:
+    if 'features' not in document:
+        mesg = not_found_mesg
+        if mesg is None:
+            mesg = "'features' property is needed for semantic validation, but was not found."
+        errors.append(_error_factory('/',
+                                     mesg))
+        return None
+    return document['features']
+
+
+def validate_b12_3_0_0_properties(document: dict, errors: List) -> None:
     """
-    Validate B12 version 3.0.0 CSB data and metadata against 2023-03 JSON schema
-    :param document_path: The document to validate
-    :return: Tuple[bool, dict]. If bool is True (which signals that validation succeeded), then dict will contain
-        a single key 'document' whose value is a dict representing the document that was validated. If bool is False
-        (which signals that validation failed), then dict will contain two keys: (1) 'document' whose value
-        is a dict representing the document that failed validation; and (2) 'errors' whose value is a list
-        of dicts mapping JSON path elements to errors encountered at that element.
+    Do custom semantic validation on metadata properties
     """
-    return validate_b12_3_0_0('CSB-schema-3_0_0-2023-03.json', document_path)
+    properties: dict = _get_properties(document, errors)
+    if properties is None:
+        return None
+
+    if 'platform' not in properties:
+        return None
+
+    # There is 'platform' metadata, in which case we'll want to do some custom validation
+    platform = properties['platform']
+    # Custom validation for Platform.IDNumber, which depends on Platform.IDType
+    id_type_present = False
+    id_num_present = False
+    if 'IDType' in platform:
+        id_type_present = True
+    if 'IDNumber' in platform:
+        id_num_present = True
+
+    if id_type_present and not id_num_present:
+        errors.append(_error_factory('/properties/platform',
+                                     "'IDNumber' attribute not present, but 'IDType' was specified."))
+    elif id_num_present and not id_type_present:
+        errors.append(_error_factory('/properties/platform',
+                                     "'IDType' attribute not present, but 'IDNumber' was specified."))
+    if id_type_present and id_num_present:
+        id_type = platform['IDType']
+        id_number = str(platform['IDNumber'])
+        if id_type == 'IMO':
+            # Use the same
+            id_number = f"IMO{id_number}"
+        try:
+            if not ID_NUMBER_RE[id_type].match(id_number):
+                errors.append(_error_factory('/properties/platform/IDNumber',
+                                             f"IDNumber {platform['IDNumber']} is not valid for IDType {id_type}."))
+        except KeyError:
+            errors.append(_error_factory('/properties/platform/IDType',
+                                         f"Unknown IDType {id_type}."))
+
+
+def validate_b12_3_0_0_features(document: dict, errors: List) -> None:
+    """
+
+    """
+    features = _get_features(document, errors)
+    if features is None:
+        return
+
+    # Look for presence of uncertainty in any datum, if present, make sure Uncertainty processing metadata
+    # element is also present
+    uncert_present = False
+    first_feature_with_uncert = 0
+    for f in features:
+        if 'uncertainty' in f['properties']:
+            uncert_present = True
+            break
+        first_feature_with_uncert += 1
+    if uncert_present:
+        properties: dict = _get_properties(document, errors)
+        if properties is None:
+            return
+
+        error_mesg: str = 'Observation uncertainty found, but Uncertainty metadata was not found.'
+        uncert_meta_present = False
+        lineage: dict = _get_lineage(document, errors)
+        if lineage is not None:
+            for l in lineage:
+                if l['type'] == 'Uncertainty':
+                    uncert_meta_present = True
+                    break
+        if not uncert_meta_present:
+            errors.append(_error_factory(f"/features/{first_feature_with_uncert}/properties",
+                                         error_mesg))
 
 
 def validate_b12_3_0_0(schema_rsrc_name: str,
-                       document_path: Union[Path, str]) -> Tuple[bool, dict]:
+                       document_path: Union[Path, str], *,
+                       validate_uncertainty: bool = True) -> Tuple[bool, dict]:
     """
     Validate B12 version 3.0.0 CSB data and metadata against JSON schema
     :param schema_rsrc_name: Internal resource name of schema document to use for validation
     :param document_path: The document to validate
-    :param validator:
+    :param validate_uncertainty: Boolean flag controlling whether uncertainty metadata should be validated.
     :return: Tuple[bool, dict]. If bool is True (which signals that validation succeeded), then dict will contain
         a single key 'document' whose value is a dict representing the document that was validated. If bool is False
         (which signals that validation failed), then dict will contain two keys: (1) 'document' whose value
         is a dict representing the document that failed validation; and (2) 'errors' whose value is a list
         of dicts mapping JSON path elements to errors encountered at that element.
     """
     validator = _get_validator(schema_rsrc_name)
@@ -84,68 +217,47 @@
 
     errors = []
     for e in validator.iter_errors(document):
         # Basic validation against schema failed, note the failures, but allow validation to continue
         errors.append(_error_factory('/' + '/'.join([str(elem) for elem in e.absolute_path]),
                                      e.message))
 
-    if 'properties' not in document:
-        errors.append(_error_factory('/',
-                                     "'properties' is a required property."))
-        return _validate_return(document, errors)
+    # Do custom "semantic" validation that is difficult/not possible to express in JSON schema
+    validate_b12_3_0_0_properties(document, errors)
+    if validate_uncertainty:
+        validate_b12_3_0_0_features(document, errors)
 
-    properties = document['properties']
+    return _validate_return(document, errors)
 
-    # See if there is 'platform' metadata, in which case we'll want to do some custom validation
-    if 'platform' in properties:
-        platform = properties['platform']
-        # Custom validation for Platform.IDNumber, which depends on Platform.IDType
-        id_type_present = False
-        id_num_present = False
-        if 'IDType' in platform:
-            id_type_present = True
-        if 'IDNumber' in platform:
-            id_num_present = True
-
-        if id_type_present and not id_num_present:
-            errors.append(_error_factory('/properties/platform',
-                                         "'IDNumber' attribute not present, but 'IDType' was specified."))
-        elif id_num_present and not id_type_present:
-            errors.append(_error_factory('/properties/platform',
-                                         "'IDType' attribute not present, but 'IDNumber' was specified."))
-        if id_type_present and id_num_present:
-            id_type = platform['IDType']
-            id_number = str(platform['IDNumber'])
-            if id_type == 'IMO':
-                # Use the same
-                id_number = f"IMO{id_number}"
-            try:
-                if not ID_NUMBER_RE[id_type].match(id_number):
-                    errors.append(_error_factory('/properties/platform/IDNumber',
-                                                 f"IDNumber {platform['IDNumber']} is not valid for IDType {id_type}."))
-            except KeyError:
-                errors.append(_error_factory('/properties/platform/IDType',
-                              f"Unknown IDType {id_type}."))
 
-    return _validate_return(document, errors)
+def validate_b12_3_0_0_2023_03(document_path: Union[Path, str]) -> Tuple[bool, dict]:
+    """
+    Validate B12 version 3.0.0 CSB data and metadata against 2023-03 JSON schema
+    :param document_path: The document to validate
+    :return: Tuple[bool, dict]. If bool is True (which signals that validation succeeded), then dict will contain
+        a single key 'document' whose value is a dict representing the document that was validated. If bool is False
+        (which signals that validation failed), then dict will contain two keys: (1) 'document' whose value
+        is a dict representing the document that failed validation; and (2) 'errors' whose value is a list
+        of dicts mapping JSON path elements to errors encountered at that element.
+    """
+    return validate_b12_3_0_0('CSB-schema-3_0_0-2023-03.json', document_path,
+                              validate_uncertainty=False)
 
 
-def validate_b12_xyz_3_0_0_2023_03(document_path: Union[Path, str]) -> Tuple[bool, dict]:
+def validate_b12_3_0_0_2023_08(document_path: Union[Path, str]) -> Tuple[bool, dict]:
     """
-    Validate B12 version 3.0.0 CSB XYZ metadata against 2023-03 JSON schema. Note: this validates
-    metadata only, and is intended for use with metadata JSON files that are separate from CSB
-    data provided in CSV or other file types.
+    Validate B12 version 3.0.0 CSB data and metadata against 2023-08 JSON schema
     :param document_path: The document to validate
     :return: Tuple[bool, dict]. If bool is True (which signals that validation succeeded), then dict will contain
         a single key 'document' whose value is a dict representing the document that was validated. If bool is False
         (which signals that validation failed), then dict will contain two keys: (1) 'document' whose value
         is a dict representing the document that failed validation; and (2) 'errors' whose value is a list
         of dicts mapping JSON path elements to errors encountered at that element.
     """
-    return validate_b12_xyz_3_0_0('XYZ-CSB-schema-3_0_0-2023-03.json', document_path)
+    return validate_b12_3_0_0('CSB-schema-3_0_0-2023-08.json', document_path)
 
 
 def validate_b12_xyz_3_0_0(schema_rsrc_name: str,
                            document_path: Union[Path, str]) -> Tuple[bool, dict]:
     """
     Validate B12 version 3.0.0 CSB XYZ metadata against JSON schema
     :param schema_rsrc_name: Internal resource name of schema document to use for validation
@@ -199,145 +311,196 @@
         except KeyError:
             errors.append(_error_factory('/platform/IDType',
                           f"Unknown IDType {id_type}."))
 
     return _validate_return(document, errors)
 
 
-def validate_b12_3_1_0_2023_03(document_path: Union[Path, str]) -> Tuple[bool, dict]:
+def validate_b12_xyz_3_0_0_2023_03(document_path: Union[Path, str]) -> Tuple[bool, dict]:
     """
-    Validate B12 version 3.1.0 CSB data and metadata against 2023-03 JSON schema
+    Validate B12 version 3.0.0 CSB XYZ metadata against 2023-03 JSON schema. Note: this validates
+    metadata only, and is intended for use with metadata JSON files that are separate from CSB
+    data provided in CSV or other file types.
+    :param document_path: The document to validate
+    :return: Tuple[bool, dict]. If bool is True (which signals that validation succeeded), then dict will contain
+        a single key 'document' whose value is a dict representing the document that was validated. If bool is False
+        (which signals that validation failed), then dict will contain two keys: (1) 'document' whose value
+        is a dict representing the document that failed validation; and (2) 'errors' whose value is a list
+        of dicts mapping JSON path elements to errors encountered at that element.
+    """
+    return validate_b12_xyz_3_0_0('XYZ-CSB-schema-3_0_0-2023-03.json', document_path)
+
+
+def validate_b12_xyz_3_0_0_2023_08(document_path: Union[Path, str]) -> Tuple[bool, dict]:
+    """
+    Validate B12 version 3.0.0 CSB XYZ metadata against 2023-03 JSON schema. Note: this validates
+    metadata only, and is intended for use with metadata JSON files that are separate from CSB
+    data provided in CSV or other file types.
     :param document_path: The document to validate
     :return: Tuple[bool, dict]. If bool is True (which signals that validation succeeded), then dict will contain
         a single key 'document' whose value is a dict representing the document that was validated. If bool is False
         (which signals that validation failed), then dict will contain two keys: (1) 'document' whose value
         is a dict representing the document that failed validation; and (2) 'errors' whose value is a list
         of dicts mapping JSON path elements to errors encountered at that element.
     """
-    return validate_b12_3_1_0('CSB-schema-3_1_0-2023-03.json', document_path)
+    return validate_b12_xyz_3_0_0('XYZ-CSB-schema-3_0_0-2023-08.json', document_path)
+
+
+def validate_b12_3_1_0_properties(document: dict, errors: List) -> None:
+    """
+    Do custom semantic validation on metadata properties
+    """
+    properties: dict = _get_properties(document, errors)
+    if properties is None:
+        return
+
+    if 'platform' not in properties:
+        return
+
+    # There is 'platform' metadata, in which case we'll want to do some custom validation
+    platform = properties['platform']
+    # Custom validator for Platform.IDNumber, which depends on Platform.IDType
+    if 'IDType' not in platform:
+        errors.append(_error_factory('/properties/platform',
+                                     "'IDType' attribute not present, but must be."))
+    id_type = platform['IDType']
+    if 'IDNumber' not in platform:
+        errors.append(_error_factory('/properties/platform',
+                                     "'IDNumber' attribute not present, but must be."))
+    id_number = platform['IDNumber']
+    try:
+        if not ID_NUMBER_RE[id_type].match(id_number):
+            errors.append(_error_factory('/properties/platform/IDNumber',
+                                         f"IDNumber {id_number} is not valid for IDType {id_type}."))
+    except KeyError:
+        errors.append(_error_factory('/properties/platform/IDType',
+                                     f"Unknown IDType {id_type}."))
+
+    # Add custom validator for Platform.dataProcessed, which if False, Processing entries should not be present.
+    data_processed = platform.get('dataProcessed', False)
+    if data_processed:
+        # dataProcessed is True, so "processing" entry ought to be present
+        if 'processing' not in properties:
+            errors.append(_error_factory('/properties/platform/dataProcessed',
+                                         f"dataProcessed flag is 'true', but 'processing' properties were not found."))
+    else:
+        # dataProcessed is False, so "processing" entry should not be present
+        if 'processing' in properties:
+            errors.append(_error_factory('/properties/platform/dataProcessed',
+                                         f"dataProcessed flag is 'false', but 'processing' properties were found."))
+    if 'uniqueID' in platform:
+        # 'uniqueID' can be present in platform as a duplicate of the required element 'uniqueVesselID` in
+        # trustedNode. This is necessary to provide backward compatibility with DCDB ingest processing.
+        if platform['uniqueID'] != properties['trustedNode']['uniqueVesselID']:
+            errors.append(_error_factory('/properties/platform/uniqueID',
+                                         f"uniqueID: {platform['uniqueID']} "
+                                         'does not match /properties/trustedNode/uniqueVesselID: '
+                                         f"{properties['trustedNode']['uniqueVesselID']}"))
+
+
+def validate_b12_3_1_0_plus_features(document: dict, errors: List,
+                                     get_processing_meta: Callable[[dict, list], Optional[dict]] = \
+                                             _get_properties_processing) -> None:
+    """
+    Do custom semantic validation on features for B12 v. 3.1.0, 3.2.0-BETA, and later
+    """
+
+    features = _get_features(document, errors)
+    if features is None:
+        return
+
+    # Look for presence of uncertainty in any datum, if present, make sure Uncertainty processing metadata
+    # element is also present
+    uncert_present = False
+    first_feature_with_uncert = 0
+    for f in features:
+        if 'uncertainty' in f['properties']:
+            uncert_present = True
+            break
+        first_feature_with_uncert += 1
+    if uncert_present:
+        properties: dict = _get_properties(document, errors)
+        if properties is None:
+            return
+
+        error_mesg: str = 'Observation uncertainty found, but Uncertainty metadata was not found.'
+        uncert_meta_present = False
+        processing: dict = get_processing_meta(properties, errors)
+        if processing is not None:
+            for p in processing:
+                if p['type'] == 'Uncertainty':
+                    uncert_meta_present = True
+                    break
+        if not uncert_meta_present:
+            errors.append(_error_factory(f"/features/{first_feature_with_uncert}/properties",
+                                         error_mesg))
 
 
 def validate_b12_3_1_0(schema_rsrc_name: str,
-                       document_path: Union[Path, str]) -> Tuple[bool, dict]:
+                       document_path: Union[Path, str], *,
+                       validate_uncertainty: bool = True) -> Tuple[bool, dict]:
     """
     Validate B12 version 3.1.0 CSB data and metadata against JSON schema
     :param schema_rsrc_name: Internal resource name of schema document to use for validation
     :param document_path: The document to validate
-    :param validator:
+    :param validate_uncertainty: Boolean flag controlling whether uncertainty metadata should be validated.
     :return: Tuple[bool, dict]. If bool is True (which signals that validation succeeded), then dict will contain
         a single key 'document' whose value is a dict representing the document that was validated. If bool is False
         (which signals that validation failed), then dict will contain two keys: (1) 'document' whose value
         is a dict representing the document that failed validation; and (2) 'errors' whose value is a list
         of dicts mapping JSON path elements to errors encountered at that element.
     """
     validator = _get_validator(schema_rsrc_name)
     document = _open_document(document_path)
 
+    # Do "structural" validation using jsonschema and capture all errors encountered
     errors = []
     for e in validator.iter_errors(document):
         # Basic validation against schema failed, note the failures, but allow validation to continue
         errors.append(_error_factory('/' + '/'.join([str(elem) for elem in e.absolute_path]),
                                      e.message))
 
-    if 'properties' not in document:
-        errors.append(_error_factory('/',
-                                     "'properties' is a required property."))
-        return _validate_return(document, errors)
-
-    properties = document['properties']
-
-    # See if there is 'platform' metadata, in which case we'll want to do some custom validation
-    if 'platform' in properties:
-        platform = properties['platform']
-        # Custom validator for Platform.IDNumber, which depends on Platform.IDType
-        if 'IDType' not in platform:
-            errors.append(_error_factory('/properties/platform',
-                                         "'IDType' attribute not present, but must be."))
-        id_type = platform['IDType']
-        if 'IDNumber' not in platform:
-            errors.append(_error_factory('/properties/platform',
-                                         "'IDNumber' attribute not present, but must be."))
-        id_number = platform['IDNumber']
-        try:
-            if not ID_NUMBER_RE[id_type].match(id_number):
-                errors.append(_error_factory('/properties/platform/IDNumber',
-                                             f"IDNumber {id_number} is not valid for IDType {id_type}."))
-        except KeyError:
-            errors.append(_error_factory('/properties/platform/IDType',
-                          f"Unknown IDType {id_type}."))
-
-        # Add custom validator for Platform.dataProcessed, which if False, Processing entries should not be present.
-        data_processed = platform.get('dataProcessed', False)
-        if data_processed:
-            # dataProcessed is True, so "processing" entry ought to be present
-            if 'processing' not in properties:
-                errors.append(_error_factory('/properties/platform/dataProcessed',
-                                             f"dataProcessed flag is 'true', but 'processing' properties were not found."))
-        else:
-            # dataProcessed is False, so "processing" entry should not be present
-            if 'processing' in properties:
-                errors.append(_error_factory('/properties/platform/dataProcessed',
-                                             f"dataProcessed flag is 'false', but 'processing' properties were found."))
-        if 'uniqueID' in platform:
-            # 'uniqueID' can be present in platform as a duplicate of the required element 'uniqueVesselID` in
-            # trustedNode. This is necessary to provide backward compatibility with DCDB ingest processing.
-            if platform['uniqueID'] != properties['trustedNode']['uniqueVesselID']:
-                errors.append(_error_factory('/properties/platform/uniqueID',
-                                             f"uniqueID: {platform['uniqueID']} "
-                                             'does not match /properties/trustedNode/uniqueVesselID: '
-                                             f"{properties['trustedNode']['uniqueVesselID']}"))
+    # Do custom "semantic" validation that is difficult/not possible to express in JSON schema
+    validate_b12_3_1_0_properties(document, errors)
+    if validate_uncertainty:
+        validate_b12_3_1_0_plus_features(document, errors)
 
     return _validate_return(document, errors)
 
 
-def validate_b12_3_2_0_BETA(document_path: Union[Path, str]) -> Tuple[bool, dict]:
+def validate_b12_3_1_0_2023_03(document_path: Union[Path, str]) -> Tuple[bool, dict]:
     """
-    Validate B12 version 3.2.0-BETA CSB data and metadata against BETA JSON schema
+    Validate B12 version 3.1.0 CSB data and metadata against 2023-03 JSON schema
     :param document_path: The document to validate
-    :return: If bool is True (which signals that validation succeeded), then dict will contain
+    :return: Tuple[bool, dict]. If bool is True (which signals that validation succeeded), then dict will contain
         a single key 'document' whose value is a dict representing the document that was validated. If bool is False
         (which signals that validation failed), then dict will contain two keys: (1) 'document' whose value
         is a dict representing the document that failed validation; and (2) 'errors' whose value is a list
         of dicts mapping JSON path elements to errors encountered at that element.
     """
-    return validate_b12_3_2_0('CSB-schema-3_2_0-BETA.json', document_path)
+    return validate_b12_3_1_0('CSB-schema-3_1_0-2023-03.json', document_path, validate_uncertainty=False)
 
 
-def validate_b12_3_2_0(schema_rsrc_name: str,
-                       document_path: Union[Path, str]) -> Tuple[bool, dict]:
+def validate_b12_3_1_0_2023_08(document_path: Union[Path, str]) -> Tuple[bool, dict]:
     """
-    Validate B12 version 3.2.0 CSB data and metadata against JSON schema
-    :param schema_rsrc_name: Internal resource name of schema document to use for validation
+    Validate B12 version 3.1.0 CSB data and metadata against 2023-08 JSON schema
     :param document_path: The document to validate
-    :param validator:
     :return: Tuple[bool, dict]. If bool is True (which signals that validation succeeded), then dict will contain
         a single key 'document' whose value is a dict representing the document that was validated. If bool is False
         (which signals that validation failed), then dict will contain two keys: (1) 'document' whose value
         is a dict representing the document that failed validation; and (2) 'errors' whose value is a list
         of dicts mapping JSON path elements to errors encountered at that element.
     """
-    validator = _get_validator(schema_rsrc_name)
-    document = _open_document(document_path)
+    return validate_b12_3_1_0('CSB-schema-3_1_0-2023-08.json', document_path)
 
-    valid = True
-    result = {'document': document}
 
-    errors = []
-    result['errors'] = errors
-    for e in validator.iter_errors(document):
-        # Basic validation against schema failed, note the failures, but allow validation to continue
-        errors.append(_error_factory('/' + '/'.join([str(elem) for elem in e.absolute_path]),
-                                     e.message))
-
-    if 'properties' not in document:
-        errors.append(_error_factory('/',
-                                     "'properties' is a required property."))
-        return _validate_return(document, errors)
-
-    properties = document['properties']
+def validate_b12_3_2_0_properties(document: dict, errors: List) -> None:
+    properties: dict = _get_properties(document, errors)
+    if properties is None:
+        return None
 
     # See if there is 'trustedNodePlatform' metadata, in which case we'll want to do some custom validation
     if 'trustedNodePlatform' in properties:
         tnp = properties['trustedNodePlatform']
         # Custom validator for trustedNodePlatform/IDNumber, which depends on trustedNodePlatform/IDType
         if 'IDType' not in tnp:
             errors.append(_error_factory('/properties/trustedNodePlatform',
@@ -349,15 +512,15 @@
         id_number = tnp['IDNumber']
         try:
             if not ID_NUMBER_RE[id_type].match(id_number):
                 errors.append(_error_factory('/properties/trustedNodePlatform/IDNumber',
                                              f"IDNumber {id_number} is not valid for IDType {id_type}."))
         except KeyError:
             errors.append(_error_factory('/properties/trustedNodePlatform/IDType',
-                          f"Unknown IDType {id_type}."))
+                                         f"Unknown IDType {id_type}."))
 
     if 'observationCollection' in properties:
         obs_coll = properties['observationCollection']
         if 'platform' in obs_coll:
             platform = obs_coll['platform']
             # Add custom validator for Platform.dataProcessed, which if False, Processing entries should not be present.
             data_processed = platform.get('dataProcessed', False)
@@ -374,8 +537,53 @@
                 if 'processing' in obs_coll:
                     errors.append(_error_factory('/properties/observationCollection/platform',
                                                  ("dataProcessed flag is 'false', but "
                                                   "'/properties/observationCollection/processing' "
                                                   "properties were found."))
                                   )
 
+
+def validate_b12_3_2_0(schema_rsrc_name: str,
+                       document_path: Union[Path, str]) -> Tuple[bool, dict]:
+    """
+    Validate B12 version 3.2.0 CSB data and metadata against JSON schema
+    :param schema_rsrc_name: Internal resource name of schema document to use for validation
+    :param document_path: The document to validate
+    :param validator:
+    :return: Tuple[bool, dict]. If bool is True (which signals that validation succeeded), then dict will contain
+        a single key 'document' whose value is a dict representing the document that was validated. If bool is False
+        (which signals that validation failed), then dict will contain two keys: (1) 'document' whose value
+        is a dict representing the document that failed validation; and (2) 'errors' whose value is a list
+        of dicts mapping JSON path elements to errors encountered at that element.
+    """
+    validator = _get_validator(schema_rsrc_name)
+    document = _open_document(document_path)
+
+    valid = True
+    result = {'document': document}
+
+    errors = []
+    result['errors'] = errors
+    for e in validator.iter_errors(document):
+        # Basic validation against schema failed, note the failures, but allow validation to continue
+        errors.append(_error_factory('/' + '/'.join([str(elem) for elem in e.absolute_path]),
+                                     e.message))
+
+    # Do custom "semantic" validation that is difficult/not possible to express in JSON schema
+    validate_b12_3_2_0_properties(document, errors)
+    validate_b12_3_1_0_plus_features(document, errors,
+                                     get_processing_meta=_get_properties_obs_coll_processing)
+
     return _validate_return(document, errors)
+
+
+def validate_b12_3_2_0_BETA(document_path: Union[Path, str]) -> Tuple[bool, dict]:
+    """
+    Validate B12 version 3.2.0-BETA CSB data and metadata against BETA JSON schema
+    :param document_path: The document to validate
+    :return: If bool is True (which signals that validation succeeded), then dict will contain
+        a single key 'document' whose value is a dict representing the document that was validated. If bool is False
+        (which signals that validation failed), then dict will contain two keys: (1) 'document' whose value
+        is a dict representing the document that failed validation; and (2) 'errors' whose value is a list
+        of dicts mapping JSON path elements to errors encountered at that element.
+    """
+    return validate_b12_3_2_0('CSB-schema-3_2_0-BETA.json', document_path)
```

### Comparing `csbschema-1.0.5/csbschema.egg-info/PKG-INFO` & `csbschema-1.1.0/csbschema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csbschema
-Version: 1.0.5
+Version: 1.1.0
 Summary: JSON Schema and validator for IHO B-12 Crowdsourced Bathymetry metadata and data
 Author-email: Brian Miles <bmiles@ccom.unh.edu>, Brian Calder <brc@ccom.unh.edu>
 Project-URL: Homepage, https://github.com/CCOMJHC/csbschema
 Project-URL: Bug Tracker, https://github.com/CCOMJHC/csbschema/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `csbschema-1.0.5/csbschema.egg-info/SOURCES.txt` & `csbschema-1.1.0/csbschema.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 csbschema/validators.py
 csbschema.egg-info/PKG-INFO
 csbschema.egg-info/SOURCES.txt
 csbschema.egg-info/dependency_links.txt
 csbschema.egg-info/entry_points.txt
 csbschema.egg-info/requires.txt
 csbschema.egg-info/top_level.txt
-csbschema/cmd/__init__.py
-csbschema/cmd/__main__.py
-csbschema/cmd/validate.py
+csbschema/command/__init__.py
+csbschema/command/__main__.py
+csbschema/command/validate.py
 csbschema/data/CSB-schema-3_0_0-2023-03.json
+csbschema/data/CSB-schema-3_0_0-2023-08.json
 csbschema/data/CSB-schema-3_1_0-2023-03.json
+csbschema/data/CSB-schema-3_1_0-2023-08.json
 csbschema/data/CSB-schema-3_2_0-BETA.json
 csbschema/data/XYZ-CSB-schema-3_0_0-2023-03.json
+csbschema/data/XYZ-CSB-schema-3_0_0-2023-08.json
 csbschema/data/__init__.py
```

### Comparing `csbschema-1.0.5/pyproject.toml` & `csbschema-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -32,11 +32,11 @@
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/CCOMJHC/csbschema"
 "Bug Tracker" = "https://github.com/CCOMJHC/csbschema/issues"
 
 [project.scripts]
-csbschema = "csbschema.cmd.__main__:main"
+csbschema = "csbschema.command.__main__:main"
 
 [tool.setuptools.dynamic]
 version = {attr = "csbschema.__version__"}
```

