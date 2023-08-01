# Comparing `tmp/visionai-data-format-1.0.7.tar.gz` & `tmp/visionai-data-format-1.0.7a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visionai-data-format-1.0.7.tar", last modified: Tue Aug  1 09:15:03 2023, max compression
+gzip compressed data, was "visionai-data-format-1.0.7a0.tar", last modified: Tue Jul 25 08:54:29 2023, max compression
```

## Comparing `visionai-data-format-1.0.7.tar` & `visionai-data-format-1.0.7a0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-08-01 09:15:03.766998 visionai-data-format-1.0.7/
--rw-r--r--   0 christian   (501) staff       (20)    17296 2023-08-01 09:15:03.766676 visionai-data-format-1.0.7/PKG-INFO
--rw-r--r--   0 christian   (501) staff       (20)    17066 2023-08-01 09:13:32.000000 visionai-data-format-1.0.7/README.md
--rw-r--r--   0 christian   (501) staff       (20)       38 2023-08-01 09:15:03.767058 visionai-data-format-1.0.7/setup.cfg
--rw-r--r--   0 christian   (501) staff       (20)      753 2023-08-01 09:13:32.000000 visionai-data-format-1.0.7/setup.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-08-01 09:15:03.759473 visionai-data-format-1.0.7/tests/
--rw-r--r--   0 christian   (501) staff       (20)     2176 2023-07-31 09:22:29.000000 visionai-data-format-1.0.7/tests/test_schemas.py
--rw-r--r--   0 christian   (501) staff       (20)     4790 2023-08-01 09:13:32.000000 visionai-data-format-1.0.7/tests/test_validators.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-08-01 09:15:03.761259 visionai-data-format-1.0.7/visionai_data_format/
--rw-r--r--   0 christian   (501) staff       (20)        0 2023-07-31 09:22:29.000000 visionai-data-format-1.0.7/visionai_data_format/__init__.py
--rw-r--r--   0 christian   (501) staff       (20)     3180 2023-08-01 09:13:32.000000 visionai-data-format-1.0.7/visionai_data_format/bdd_to_vai.py
--rw-r--r--   0 christian   (501) staff       (20)     7775 2023-07-31 09:22:29.000000 visionai-data-format-1.0.7/visionai_data_format/coco_to_vai.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-08-01 09:15:03.764126 visionai-data-format-1.0.7/visionai_data_format/schemas/
--rw-r--r--   0 christian   (501) staff       (20)        0 2023-07-31 09:22:29.000000 visionai-data-format-1.0.7/visionai_data_format/schemas/__init__.py
--rw-r--r--   0 christian   (501) staff       (20)     2581 2023-08-01 09:13:32.000000 visionai-data-format-1.0.7/visionai_data_format/schemas/bdd_schema.py
--rw-r--r--   0 christian   (501) staff       (20)      679 2023-07-31 09:22:29.000000 visionai-data-format-1.0.7/visionai_data_format/schemas/coco_schema.py
--rw-r--r--   0 christian   (501) staff       (20)     1657 2023-07-31 09:22:29.000000 visionai-data-format-1.0.7/visionai_data_format/schemas/common.py
--rw-r--r--   0 christian   (501) staff       (20)      994 2023-07-31 09:22:29.000000 visionai-data-format-1.0.7/visionai_data_format/schemas/ontology.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-08-01 09:15:03.764446 visionai-data-format-1.0.7/visionai_data_format/schemas/utils/
--rw-r--r--   0 christian   (501) staff       (20)        0 2023-07-31 09:22:29.000000 visionai-data-format-1.0.7/visionai_data_format/schemas/utils/__init__.py
--rw-r--r--   0 christian   (501) staff       (20)    41624 2023-08-01 09:13:32.000000 visionai-data-format-1.0.7/visionai_data_format/schemas/utils/validators.py
--rw-r--r--   0 christian   (501) staff       (20)    28134 2023-08-01 09:13:32.000000 visionai-data-format-1.0.7/visionai_data_format/schemas/visionai_schema.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-08-01 09:15:03.766400 visionai-data-format-1.0.7/visionai_data_format/utils/
--rw-r--r--   0 christian   (501) staff       (20)        0 2023-07-31 09:22:29.000000 visionai-data-format-1.0.7/visionai_data_format/utils/__init__.py
--rw-r--r--   0 christian   (501) staff       (20)      494 2023-07-31 09:22:29.000000 visionai-data-format-1.0.7/visionai_data_format/utils/calculation.py
--rw-r--r--   0 christian   (501) staff       (20)    10506 2023-07-31 09:22:29.000000 visionai-data-format-1.0.7/visionai_data_format/utils/checker.py
--rw-r--r--   0 christian   (501) staff       (20)      761 2023-07-31 09:22:29.000000 visionai-data-format-1.0.7/visionai_data_format/utils/classes.py
--rw-r--r--   0 christian   (501) staff       (20)      335 2023-07-31 09:22:29.000000 visionai-data-format-1.0.7/visionai_data_format/utils/common.py
--rw-r--r--   0 christian   (501) staff       (20)    14161 2023-08-01 09:13:32.000000 visionai-data-format-1.0.7/visionai_data_format/utils/converter.py
--rw-r--r--   0 christian   (501) staff       (20)     4059 2023-07-31 09:22:29.000000 visionai-data-format-1.0.7/visionai_data_format/utils/resize.py
--rw-r--r--   0 christian   (501) staff       (20)     1991 2023-07-31 09:22:29.000000 visionai-data-format-1.0.7/visionai_data_format/utils/validator.py
--rw-r--r--   0 christian   (501) staff       (20)     2308 2023-08-01 09:13:32.000000 visionai-data-format-1.0.7/visionai_data_format/vai_to_bdd.py
--rw-r--r--   0 christian   (501) staff       (20)     6237 2023-07-31 09:22:29.000000 visionai-data-format-1.0.7/visionai_data_format/vai_to_coco.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-08-01 09:15:03.762735 visionai-data-format-1.0.7/visionai_data_format.egg-info/
--rw-r--r--   0 christian   (501) staff       (20)    17296 2023-08-01 09:15:03.000000 visionai-data-format-1.0.7/visionai_data_format.egg-info/PKG-INFO
--rw-r--r--   0 christian   (501) staff       (20)     1122 2023-08-01 09:15:03.000000 visionai-data-format-1.0.7/visionai_data_format.egg-info/SOURCES.txt
--rw-r--r--   0 christian   (501) staff       (20)        1 2023-08-01 09:15:03.000000 visionai-data-format-1.0.7/visionai_data_format.egg-info/dependency_links.txt
--rw-r--r--   0 christian   (501) staff       (20)       45 2023-08-01 09:15:03.000000 visionai-data-format-1.0.7/visionai_data_format.egg-info/requires.txt
--rw-r--r--   0 christian   (501) staff       (20)       21 2023-08-01 09:15:03.000000 visionai-data-format-1.0.7/visionai_data_format.egg-info/top_level.txt
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-25 08:54:29.329596 visionai-data-format-1.0.7a0/
+-rw-r--r--   0 christian   (501) staff       (20)    17298 2023-07-25 08:54:29.327293 visionai-data-format-1.0.7a0/PKG-INFO
+-rw-r--r--   0 christian   (501) staff       (20)    17066 2023-07-25 08:38:17.000000 visionai-data-format-1.0.7a0/README.md
+-rw-r--r--   0 christian   (501) staff       (20)       38 2023-07-25 08:54:29.329716 visionai-data-format-1.0.7a0/setup.cfg
+-rw-r--r--   0 christian   (501) staff       (20)      755 2023-07-25 08:54:14.000000 visionai-data-format-1.0.7a0/setup.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-25 08:54:29.321173 visionai-data-format-1.0.7a0/tests/
+-rw-r--r--   0 christian   (501) staff       (20)     2176 2023-07-17 04:56:18.000000 visionai-data-format-1.0.7a0/tests/test_schemas.py
+-rw-r--r--   0 christian   (501) staff       (20)     4731 2023-07-17 04:56:18.000000 visionai-data-format-1.0.7a0/tests/test_validators.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-25 08:54:29.322414 visionai-data-format-1.0.7a0/visionai_data_format/
+-rw-r--r--   0 christian   (501) staff       (20)        0 2023-07-17 04:56:18.000000 visionai-data-format-1.0.7a0/visionai_data_format/__init__.py
+-rw-r--r--   0 christian   (501) staff       (20)     3180 2023-07-25 08:38:17.000000 visionai-data-format-1.0.7a0/visionai_data_format/bdd_to_vai.py
+-rw-r--r--   0 christian   (501) staff       (20)     7775 2023-07-17 04:56:18.000000 visionai-data-format-1.0.7a0/visionai_data_format/coco_to_vai.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-25 08:54:29.324452 visionai-data-format-1.0.7a0/visionai_data_format/schemas/
+-rw-r--r--   0 christian   (501) staff       (20)        0 2023-07-17 04:56:18.000000 visionai-data-format-1.0.7a0/visionai_data_format/schemas/__init__.py
+-rw-r--r--   0 christian   (501) staff       (20)     2581 2023-07-25 08:38:17.000000 visionai-data-format-1.0.7a0/visionai_data_format/schemas/bdd_schema.py
+-rw-r--r--   0 christian   (501) staff       (20)      679 2023-07-17 04:56:18.000000 visionai-data-format-1.0.7a0/visionai_data_format/schemas/coco_schema.py
+-rw-r--r--   0 christian   (501) staff       (20)     1657 2023-07-17 04:56:18.000000 visionai-data-format-1.0.7a0/visionai_data_format/schemas/common.py
+-rw-r--r--   0 christian   (501) staff       (20)      994 2023-07-17 04:56:18.000000 visionai-data-format-1.0.7a0/visionai_data_format/schemas/ontology.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-25 08:54:29.324913 visionai-data-format-1.0.7a0/visionai_data_format/schemas/utils/
+-rw-r--r--   0 christian   (501) staff       (20)        0 2023-07-17 04:56:18.000000 visionai-data-format-1.0.7a0/visionai_data_format/schemas/utils/__init__.py
+-rw-r--r--   0 christian   (501) staff       (20)    40508 2023-07-25 08:39:08.000000 visionai-data-format-1.0.7a0/visionai_data_format/schemas/utils/validators.py
+-rw-r--r--   0 christian   (501) staff       (20)    27992 2023-07-17 04:56:18.000000 visionai-data-format-1.0.7a0/visionai_data_format/schemas/visionai_schema.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-25 08:54:29.327018 visionai-data-format-1.0.7a0/visionai_data_format/utils/
+-rw-r--r--   0 christian   (501) staff       (20)        0 2023-07-17 04:56:18.000000 visionai-data-format-1.0.7a0/visionai_data_format/utils/__init__.py
+-rw-r--r--   0 christian   (501) staff       (20)      494 2023-07-17 04:56:18.000000 visionai-data-format-1.0.7a0/visionai_data_format/utils/calculation.py
+-rw-r--r--   0 christian   (501) staff       (20)    10506 2023-07-17 04:56:18.000000 visionai-data-format-1.0.7a0/visionai_data_format/utils/checker.py
+-rw-r--r--   0 christian   (501) staff       (20)      761 2023-07-17 04:56:18.000000 visionai-data-format-1.0.7a0/visionai_data_format/utils/classes.py
+-rw-r--r--   0 christian   (501) staff       (20)      335 2023-07-17 04:56:18.000000 visionai-data-format-1.0.7a0/visionai_data_format/utils/common.py
+-rw-r--r--   0 christian   (501) staff       (20)    14161 2023-07-25 08:38:17.000000 visionai-data-format-1.0.7a0/visionai_data_format/utils/converter.py
+-rw-r--r--   0 christian   (501) staff       (20)     4059 2023-07-17 04:56:18.000000 visionai-data-format-1.0.7a0/visionai_data_format/utils/resize.py
+-rw-r--r--   0 christian   (501) staff       (20)     1991 2023-07-17 04:56:18.000000 visionai-data-format-1.0.7a0/visionai_data_format/utils/validator.py
+-rw-r--r--   0 christian   (501) staff       (20)     2308 2023-07-17 04:56:18.000000 visionai-data-format-1.0.7a0/visionai_data_format/vai_to_bdd.py
+-rw-r--r--   0 christian   (501) staff       (20)     6237 2023-07-17 04:56:18.000000 visionai-data-format-1.0.7a0/visionai_data_format/vai_to_coco.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-25 08:54:29.323302 visionai-data-format-1.0.7a0/visionai_data_format.egg-info/
+-rw-r--r--   0 christian   (501) staff       (20)    17298 2023-07-25 08:54:29.000000 visionai-data-format-1.0.7a0/visionai_data_format.egg-info/PKG-INFO
+-rw-r--r--   0 christian   (501) staff       (20)     1122 2023-07-25 08:54:29.000000 visionai-data-format-1.0.7a0/visionai_data_format.egg-info/SOURCES.txt
+-rw-r--r--   0 christian   (501) staff       (20)        1 2023-07-25 08:54:29.000000 visionai-data-format-1.0.7a0/visionai_data_format.egg-info/dependency_links.txt
+-rw-r--r--   0 christian   (501) staff       (20)       45 2023-07-25 08:54:29.000000 visionai-data-format-1.0.7a0/visionai_data_format.egg-info/requires.txt
+-rw-r--r--   0 christian   (501) staff       (20)       21 2023-07-25 08:54:29.000000 visionai-data-format-1.0.7a0/visionai_data_format.egg-info/top_level.txt
```

### Comparing `visionai-data-format-1.0.7/PKG-INFO` & `visionai-data-format-1.0.7a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visionai-data-format
-Version: 1.0.7
+Version: 1.0.7a0
 Summary: converter tool for visionai format
 Home-page: 
 Author: LinkerVision
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `visionai-data-format-1.0.7/README.md` & `visionai-data-format-1.0.7a0/README.md`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.7/setup.py` & `visionai-data-format-1.0.7a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 AUTHOR = "LinkerVision"
 PACKAGE_NAME = "visionai-data-format"
-PACKAGE_VERSION = "1.0.7"
+PACKAGE_VERSION = "1.0.7a0"
 DESC = "converter tool for visionai format"
 REQUIRED = ["pydantic==1.*"]
 REQUIRES_PYTHON = ">=3.7, <4"
 EXTRAS = {
     "test": [
         "pytest",
         "mock",
```

### Comparing `visionai-data-format-1.0.7/tests/test_schemas.py` & `visionai-data-format-1.0.7a0/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.7/tests/test_validators.py` & `visionai-data-format-1.0.7a0/tests/test_validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,18 +115,17 @@
     errors = VisionAIModel(
         **fake_objects_data_single_lidar_wrong_visionai_frame_intervals
     ).validate_with_ontology(
         ontology=ontology,
     )
 
     assert errors == [
-        "Extra frames from `frame_intervals` : {1, 2}\n",
         "validate objects error: objects UUID 893ac389-7782-4bc3-8f61-09a8e48c819f with data pointer"
         + " bbox_shape frame interval(s) error, current data pointer interval (0, 2) "
-        + "doesn't match with objects interval [(0, 0)]",
+        + "doesn't match with objects interval [(0, 0)]"
     ]
 
 
 def test_validate_wrong_object_frame_intervals(
     fake_visionai_ontology,
     fake_objects_data_single_lidar_wrong_objects_frame_intervals,
 ):
```

### Comparing `visionai-data-format-1.0.7/visionai_data_format/bdd_to_vai.py` & `visionai-data-format-1.0.7a0/visionai_data_format/bdd_to_vai.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.7/visionai_data_format/coco_to_vai.py` & `visionai-data-format-1.0.7a0/visionai_data_format/coco_to_vai.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.7/visionai_data_format/schemas/bdd_schema.py` & `visionai-data-format-1.0.7a0/visionai_data_format/schemas/bdd_schema.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.7/visionai_data_format/schemas/coco_schema.py` & `visionai-data-format-1.0.7a0/visionai_data_format/schemas/coco_schema.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.7/visionai_data_format/schemas/common.py` & `visionai-data-format-1.0.7a0/visionai_data_format/schemas/common.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.7/visionai_data_format/schemas/ontology.py` & `visionai-data-format-1.0.7a0/visionai_data_format/schemas/ontology.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.7/visionai_data_format/schemas/utils/validators.py` & `visionai-data-format-1.0.7a0/visionai_data_format/schemas/utils/validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,49 +62,14 @@
         classes_attributes_map[obj_class].update(
             mapping_attributes_type_value(data.get(data_key, None))
         )
 
     return classes_attributes_map
 
 
-def validate_visionai_intervals(visionai: Dict) -> Optional[str]:
-    """Validate frame intervals under visionai with its frames
-
-    Parameters
-    ----------
-    visionai : Dict
-        visionai data in dictionary
-
-    Returns
-    -------
-    Optional[str]
-        error message
-    """
-    msg: Optional[str] = None
-
-    visionai_frame_interval_set = {
-        frame_num
-        for frame_interval in visionai["frame_intervals"]
-        for frame_num in range(
-            frame_interval["frame_start"], frame_interval["frame_end"] + 1
-        )
-    }
-    frame_num_set = {int(frame_num) for frame_num in visionai["frames"].keys()}
-
-    if visionai_frame_interval_set ^ frame_num_set:
-        extra_frames = frame_num_set - visionai_frame_interval_set
-        missing_frames = visionai_frame_interval_set - frame_num_set
-        msg = ""
-        if extra_frames:
-            msg += f"Extra frames from `frame_intervals` : {extra_frames}\n"
-        if missing_frames:
-            msg += f"Missing frames from `frame_intervals` : {missing_frames}\n"
-    return msg
-
-
 def validate_classes(
     visionai: Dict,
     root_key: str,
     sub_root_key: str,
     ontology_classes: Set[str],
 ) -> Tuple[Set[str], Dict[str, Dict[str, Set]]]:
     if not visionai:
@@ -525,15 +490,15 @@
 
 
 def validate_vai_data_frame_intervals(
     root_key: str,
     data_obj_under_vai_intervals: Dict[str, List],
     visionai_frame_intervals: List[Tuple[int, int]],
 ) -> Tuple[bool, str]:
-    """validate frame intervals of object/context under visionai
+    """_summary_
 
     Parameters
     ----------
     root_key : str
         visionai object key, such as `contexts` or `objects`
     data_obj_under_vai_intervals : Dict[str, list]
         a dictionary of object uuid with the list of interval tuple
```

### Comparing `visionai-data-format-1.0.7/visionai_data_format/schemas/visionai_schema.py` & `visionai-data-format-1.0.7a0/visionai_data_format/schemas/visionai_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from visionai_data_format.schemas.common import ExcludedNoneBaseModel
 from visionai_data_format.schemas.ontology import Ontology
 from visionai_data_format.schemas.utils.validators import (
     build_ontology_attributes_map,
     validate_contexts,
     validate_objects,
     validate_streams,
-    validate_visionai_intervals,
 )
 
 
 class SchemaVersion(str, Enum):
     FIELD_1_0_0 = "1.0.0"
 
 
@@ -850,18 +849,14 @@
 
         errors: List[str] = []
 
         tags = ontology.get("tags", {})
 
         visionai = self.visionai.dict(exclude_unset=True, exclude_none=True)
 
-        err = validate_visionai_intervals(visionai=visionai)
-        if err:
-            errors.append(err)
-
         streams_data = ontology["streams"]
 
         sensor_info: Dict[str, str] = {
             sensor_name: sensor_obj["type"]
             for sensor_name, sensor_obj in streams_data.items()
         }
```

### Comparing `visionai-data-format-1.0.7/visionai_data_format/utils/checker.py` & `visionai-data-format-1.0.7a0/visionai_data_format/utils/checker.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.7/visionai_data_format/utils/classes.py` & `visionai-data-format-1.0.7a0/visionai_data_format/utils/classes.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.7/visionai_data_format/utils/converter.py` & `visionai-data-format-1.0.7a0/visionai_data_format/utils/converter.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.7/visionai_data_format/utils/resize.py` & `visionai-data-format-1.0.7a0/visionai_data_format/utils/resize.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.7/visionai_data_format/utils/validator.py` & `visionai-data-format-1.0.7a0/visionai_data_format/utils/validator.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.7/visionai_data_format/vai_to_bdd.py` & `visionai-data-format-1.0.7a0/visionai_data_format/vai_to_bdd.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.7/visionai_data_format/vai_to_coco.py` & `visionai-data-format-1.0.7a0/visionai_data_format/vai_to_coco.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.7/visionai_data_format.egg-info/PKG-INFO` & `visionai-data-format-1.0.7a0/visionai_data_format.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visionai-data-format
-Version: 1.0.7
+Version: 1.0.7a0
 Summary: converter tool for visionai format
 Home-page: 
 Author: LinkerVision
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `visionai-data-format-1.0.7/visionai_data_format.egg-info/SOURCES.txt` & `visionai-data-format-1.0.7a0/visionai_data_format.egg-info/SOURCES.txt`

 * *Files identical despite different names*

