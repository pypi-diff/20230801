# Comparing `tmp/metaboatrace_models-0.1.0.tar.gz` & `tmp/metaboatrace_models-0.2.0.tar.gz`

## Comparing `metaboatrace_models-0.1.0.tar` & `metaboatrace_models-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/requirements-dev.lock
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/requirements.lock
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/metaboatrace/models/__init__.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/metaboatrace/models/boat.py
--rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/metaboatrace/models/race.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/metaboatrace/models/racer.py
--rw-r--r--   0        0        0     5755 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/metaboatrace/models/region.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/metaboatrace/models/stadium.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/tests/metaboatrace/models/test_boat.py
--rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/tests/metaboatrace/models/test_racer.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/tests/metaboatrace/models/test_region.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/tests/metaboatrace/models/test_stadium.py
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/tests/metaboatrace/models/race/test_bettings.py
--rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/tests/metaboatrace/models/race/test_race_entries.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/tests/metaboatrace/models/race/test_races.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/README.md
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/requirements-dev.lock
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/requirements.lock
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/metaboatrace/models/__init__.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/metaboatrace/models/boat.py
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/metaboatrace/models/race.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/metaboatrace/models/racer.py
+-rw-r--r--   0        0        0     5755 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/metaboatrace/models/region.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/metaboatrace/models/stadium.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/tests/metaboatrace/models/test_boat.py
+-rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/tests/metaboatrace/models/test_racer.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/tests/metaboatrace/models/test_region.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/tests/metaboatrace/models/test_stadium.py
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/tests/metaboatrace/models/race/test_bettings.py
+-rw-r--r--   0        0        0     6508 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/tests/metaboatrace/models/race/test_race_entries.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/tests/metaboatrace/models/race/test_races.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/README.md
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/PKG-INFO
```

### Comparing `metaboatrace_models-0.1.0/.github/workflows/lint.yml` & `metaboatrace_models-0.2.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.1.0/.github/workflows/publish.yml` & `metaboatrace_models-0.2.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.1.0/.github/workflows/tests.yml` & `metaboatrace_models-0.2.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.1.0/metaboatrace/models/boat.py` & `metaboatrace_models-0.2.0/metaboatrace/models/boat.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.1.0/metaboatrace/models/race.py` & `metaboatrace_models-0.2.0/metaboatrace/models/race.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 class _RaceIdentifier(BaseModel):
     race_holding_date: date
     stadium_tel_code: StadiumTelCode
     race_number: StrictInt = Field(..., ge=1, le=12)
 
 
-class _RaceEntryIdentifier(BaseModel):
+class _RaceEntryIdentifier(_RaceIdentifier):
     pit_number: StrictInt = Field(..., ge=1, le=6)
 
 
 class _BettingMixin(BaseModel):
     betting_method: BettingMethod = BettingMethod.TRIFECTA
     betting_numbers: List[int]
 
@@ -73,14 +73,15 @@
     race_lap: Literal[2, 3]
     deadline_at: datetime
     is_course_fixed: bool
     use_stabilizer: bool
 
 
 class RaceEntry(_RaceEntryIdentifier):
+    racer_registration_number: StrictInt
     is_absent: bool
     motor_number: StrictInt = Field(..., ge=1, le=99)
     boat_number: StrictInt = Field(..., ge=1, le=999)
 
 
 class StartExhibitionRecord(_RaceEntryIdentifier):
     start_course: StrictInt = Field(..., ge=1, le=6)
```

### Comparing `metaboatrace_models-0.1.0/metaboatrace/models/racer.py` & `metaboatrace_models-0.2.0/metaboatrace/models/racer.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.1.0/metaboatrace/models/region.py` & `metaboatrace_models-0.2.0/metaboatrace/models/region.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.1.0/metaboatrace/models/stadium.py` & `metaboatrace_models-0.2.0/metaboatrace/models/stadium.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.1.0/tests/metaboatrace/models/test_boat.py` & `metaboatrace_models-0.2.0/tests/metaboatrace/models/test_boat.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.1.0/tests/metaboatrace/models/test_racer.py` & `metaboatrace_models-0.2.0/tests/metaboatrace/models/test_racer.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.1.0/tests/metaboatrace/models/test_region.py` & `metaboatrace_models-0.2.0/tests/metaboatrace/models/test_region.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.1.0/tests/metaboatrace/models/test_stadium.py` & `metaboatrace_models-0.2.0/tests/metaboatrace/models/test_stadium.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.1.0/tests/metaboatrace/models/race/test_bettings.py` & `metaboatrace_models-0.2.0/tests/metaboatrace/models/race/test_bettings.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.1.0/tests/metaboatrace/models/race/test_race_entries.py` & `metaboatrace_models-0.2.0/tests/metaboatrace/models/race/test_race_entries.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,38 @@
+from datetime import date
+
 import pytest
 from pydantic import ValidationError
 
 from metaboatrace.models.race import (
     BoatSetting,
     CircumferenceExhibitionRecord,
     RaceEntry,
     RaceRecord,
     StartExhibitionRecord,
     WinningTrick,
 )
+from metaboatrace.models.stadium import StadiumTelCode
+
+base_data = {
+    "race_holding_date": date.today(),
+    "stadium_tel_code": StadiumTelCode.HEIWAJIMA,
+    "race_number": 1,
+}
 
 
 def test_race_entry_valid():  # type: ignore
-    valid_data = {"pit_number": 3, "is_absent": False, "motor_number": 10, "boat_number": 123}
+    valid_data = {
+        **base_data,
+        "pit_number": 3,
+        "racer_registration_number": 1234,
+        "is_absent": False,
+        "motor_number": 10,
+        "boat_number": 123,
+    }
     entry = RaceEntry(**valid_data)  # type: ignore
     assert entry.pit_number == valid_data["pit_number"]
     assert entry.is_absent == valid_data["is_absent"]
     assert entry.motor_number == valid_data["motor_number"]
     assert entry.boat_number == valid_data["boat_number"]
 
 
@@ -26,28 +42,30 @@
         (7, False, 10, 123, False),  # invalid pit_number
         (3, False, 0, 123, False),  # invalid motor_number
         (3, False, 10, 1000, False),  # invalid boat_number
     ],
 )
 def test_race_entry_invalid(pit_number, is_absent, motor_number, boat_number, expected):  # type: ignore
     data = {
+        **base_data,
         "pit_number": pit_number,
         "is_absent": is_absent,
         "motor_number": motor_number,
         "boat_number": boat_number,
     }
     if expected:
         RaceEntry(**data)
     else:
         with pytest.raises(ValidationError):
             RaceEntry(**data)
 
 
 def test_boat_setting_valid():  # type: ignore
     valid_data = {
+        **base_data,
         "pit_number": 3,
         "tilt": 2.5,
         "is_new_propeller": True,
         "motor_parts_exchanges": [],
     }
     setting = BoatSetting(**valid_data)  # type: ignore
     assert setting.pit_number == valid_data["pit_number"]
@@ -62,14 +80,15 @@
         (7, 2.5, True, [], False),  # invalid pit_number
         (3, 0.4, True, [], False),  # invalid tilt (below lower limit)
         (3, 3.1, True, [], False),  # invalid tilt (above upper limit)
     ],
 )
 def test_boat_setting_invalid(pit_number, tilt, is_new_propeller, motor_parts_exchanges, expected):  # type: ignore
     data = {
+        **base_data,
         "pit_number": pit_number,
         "tilt": tilt,
         "is_new_propeller": is_new_propeller,
         "motor_parts_exchanges": motor_parts_exchanges,
     }
     if expected:
         BoatSetting(**data)
@@ -89,14 +108,15 @@
         (1, 0, 1.23, False),  # invalid start_course
         (1, 7, 1.23, False),  # invalid start_course
         (1, 1, None, False),  # missing start_time
     ],
 )
 def test_start_exhibition_record(pit_number, start_course, start_time, expected):  # type: ignore
     data = {
+        **base_data,
         "pit_number": pit_number,
         "start_course": start_course,
         "start_time": start_time,
     }
     if expected:
         record = StartExhibitionRecord(**data)
         assert record.pit_number == data["pit_number"]
@@ -115,14 +135,15 @@
         (1, 1.23, True),
         # invalid cases
         (1, None, False),  # missing exhibition_time
     ],
 )
 def test_circumference_exhibition_record(pit_number, exhibition_time, expected):  # type: ignore
     data = {
+        **base_data,
         "pit_number": pit_number,
         "exhibition_time": exhibition_time,
     }
     if expected:
         record = CircumferenceExhibitionRecord(**data)
         assert record.pit_number == data["pit_number"]
         assert record.exhibition_time == data["exhibition_time"]
@@ -153,14 +174,15 @@
     total_time,
     start_time,
     winning_trick,
     disqualification,
     expected,
 ):
     data = {
+        **base_data,
         "pit_number": pit_number,
         "start_course": start_course,
         "arrival": arrival,
         "total_time": total_time,
         "start_time": start_time,
         "winning_trick": winning_trick,
         "disqualification": disqualification,
```

### Comparing `metaboatrace_models-0.1.0/tests/metaboatrace/models/race/test_races.py` & `metaboatrace_models-0.2.0/tests/metaboatrace/models/race/test_races.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.1.0/.gitignore` & `metaboatrace_models-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.1.0/LICENSE.txt` & `metaboatrace_models-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.1.0/pyproject.toml` & `metaboatrace_models-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "metaboatrace.models"
-version = "0.1.0"
+version = "0.2.0"
 description = "Models of Japanese boatrace"
 authors = [
     { name = "k0kishima", email = "okishimaxyz@gmail.com" }
 ]
 dependencies = [
     "pydantic>=2.0.3",
 ]
```

