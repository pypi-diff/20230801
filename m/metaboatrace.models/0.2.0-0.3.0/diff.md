# Comparing `tmp/metaboatrace_models-0.2.0.tar.gz` & `tmp/metaboatrace_models-0.3.0.tar.gz`

## Comparing `metaboatrace_models-0.2.0.tar` & `metaboatrace_models-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/requirements-dev.lock
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/requirements.lock
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/metaboatrace/models/__init__.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/metaboatrace/models/boat.py
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/metaboatrace/models/race.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/metaboatrace/models/racer.py
--rw-r--r--   0        0        0     5755 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/metaboatrace/models/region.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/metaboatrace/models/stadium.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/tests/metaboatrace/models/test_boat.py
--rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/tests/metaboatrace/models/test_racer.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/tests/metaboatrace/models/test_region.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/tests/metaboatrace/models/test_stadium.py
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/tests/metaboatrace/models/race/test_bettings.py
--rw-r--r--   0        0        0     6508 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/tests/metaboatrace/models/race/test_race_entries.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/tests/metaboatrace/models/race/test_races.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/README.md
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 metaboatrace_models-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 metaboatrace_models-0.3.0/requirements-dev.lock
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 metaboatrace_models-0.3.0/requirements.lock
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 metaboatrace_models-0.3.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 metaboatrace_models-0.3.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 metaboatrace_models-0.3.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 metaboatrace_models-0.3.0/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metaboatrace_models-0.3.0/metaboatrace/models/__init__.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 metaboatrace_models-0.3.0/metaboatrace/models/boat.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 metaboatrace_models-0.3.0/metaboatrace/models/race.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 metaboatrace_models-0.3.0/metaboatrace/models/racer.py
+-rw-r--r--   0        0        0     5755 2020-02-02 00:00:00.000000 metaboatrace_models-0.3.0/metaboatrace/models/region.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 metaboatrace_models-0.3.0/metaboatrace/models/stadium.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 metaboatrace_models-0.3.0/tests/metaboatrace/models/test_boat.py
+-rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 metaboatrace_models-0.3.0/tests/metaboatrace/models/test_racer.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 metaboatrace_models-0.3.0/tests/metaboatrace/models/test_region.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 metaboatrace_models-0.3.0/tests/metaboatrace/models/test_stadium.py
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 metaboatrace_models-0.3.0/tests/metaboatrace/models/race/test_bettings.py
+-rw-r--r--   0        0        0     6508 2020-02-02 00:00:00.000000 metaboatrace_models-0.3.0/tests/metaboatrace/models/race/test_race_entries.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 metaboatrace_models-0.3.0/tests/metaboatrace/models/race/test_races.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 metaboatrace_models-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 metaboatrace_models-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 metaboatrace_models-0.3.0/README.md
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 metaboatrace_models-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 metaboatrace_models-0.3.0/PKG-INFO
```

### Comparing `metaboatrace_models-0.2.0/.github/workflows/lint.yml` & `metaboatrace_models-0.3.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.2.0/.github/workflows/publish.yml` & `metaboatrace_models-0.3.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.2.0/.github/workflows/tests.yml` & `metaboatrace_models-0.3.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.2.0/metaboatrace/models/boat.py` & `metaboatrace_models-0.3.0/metaboatrace/models/boat.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.2.0/metaboatrace/models/race.py` & `metaboatrace_models-0.3.0/metaboatrace/models/race.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             if betting_number < 1 or betting_number > 6:
                 raise ValueError("Each betting number must be between 1 and 6")
         return betting_numbers
 
 
 class RaceInformation(_RaceIdentifier):
     title: str
-    race_lap: Literal[2, 3]
+    number_of_laps: Literal[2, 3]
     deadline_at: datetime
     is_course_fixed: bool
     use_stabilizer: bool
 
 
 class RaceEntry(_RaceEntryIdentifier):
     racer_registration_number: StrictInt
```

### Comparing `metaboatrace_models-0.2.0/metaboatrace/models/racer.py` & `metaboatrace_models-0.3.0/metaboatrace/models/racer.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.2.0/metaboatrace/models/region.py` & `metaboatrace_models-0.3.0/metaboatrace/models/region.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.2.0/metaboatrace/models/stadium.py` & `metaboatrace_models-0.3.0/metaboatrace/models/stadium.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.2.0/tests/metaboatrace/models/test_boat.py` & `metaboatrace_models-0.3.0/tests/metaboatrace/models/test_boat.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.2.0/tests/metaboatrace/models/test_racer.py` & `metaboatrace_models-0.3.0/tests/metaboatrace/models/test_racer.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.2.0/tests/metaboatrace/models/test_region.py` & `metaboatrace_models-0.3.0/tests/metaboatrace/models/test_region.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.2.0/tests/metaboatrace/models/test_stadium.py` & `metaboatrace_models-0.3.0/tests/metaboatrace/models/test_stadium.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.2.0/tests/metaboatrace/models/race/test_bettings.py` & `metaboatrace_models-0.3.0/tests/metaboatrace/models/race/test_bettings.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.2.0/tests/metaboatrace/models/race/test_race_entries.py` & `metaboatrace_models-0.3.0/tests/metaboatrace/models/race/test_race_entries.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.2.0/tests/metaboatrace/models/race/test_races.py` & `metaboatrace_models-0.3.0/tests/metaboatrace/models/race/test_races.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,59 +4,59 @@
 from pydantic import ValidationError
 
 from metaboatrace.models.race import RaceInformation
 from metaboatrace.models.stadium import StadiumTelCode
 
 
 @pytest.mark.parametrize(
-    "race_holding_date,stadium_tel_code,race_number,title,race_lap,deadline_at,is_course_fixed,use_stabilizer,expected",
+    "race_holding_date,stadium_tel_code,race_number,title,number_of_laps,deadline_at,is_course_fixed,use_stabilizer,expected",
     [
         # valid case
         (date.today(), StadiumTelCode.HEIWAJIMA, 1, "Race 1", 3, datetime.now(), True, False, True),
         # invalid cases
         (
             date.today(),
             StadiumTelCode.HEIWAJIMA,
             1,
             "Race 1",
             4,
             datetime.now(),
             True,
             False,
             False,
-        ),  # invalid race_lap
+        ),  # invalid number_of_laps
     ],
 )
 def test_race_information(  # type: ignore
     race_holding_date,
     stadium_tel_code,
     race_number,
     title,
-    race_lap,
+    number_of_laps,
     deadline_at,
     is_course_fixed,
     use_stabilizer,
     expected,
 ):
     data = {
         "race_holding_date": race_holding_date,
         "stadium_tel_code": stadium_tel_code,
         "race_number": race_number,
         "title": title,
-        "race_lap": race_lap,
+        "number_of_laps": number_of_laps,
         "deadline_at": deadline_at,
         "is_course_fixed": is_course_fixed,
         "use_stabilizer": use_stabilizer,
     }
     if expected:
         race_information = RaceInformation(**data)
         assert race_information.race_holding_date == data["race_holding_date"]
         assert race_information.stadium_tel_code == data["stadium_tel_code"]
         assert race_information.race_number == data["race_number"]
         assert race_information.title == data["title"]
-        assert race_information.race_lap == data["race_lap"]
+        assert race_information.number_of_laps == data["number_of_laps"]
         assert race_information.deadline_at == data["deadline_at"]
         assert race_information.is_course_fixed == data["is_course_fixed"]
         assert race_information.use_stabilizer == data["use_stabilizer"]
     else:
         with pytest.raises(ValidationError):
             race_information = RaceInformation(**data)
```

### Comparing `metaboatrace_models-0.2.0/.gitignore` & `metaboatrace_models-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.2.0/LICENSE.txt` & `metaboatrace_models-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.2.0/pyproject.toml` & `metaboatrace_models-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "metaboatrace.models"
-version = "0.2.0"
+version = "0.3.0"
 description = "Models of Japanese boatrace"
 authors = [
     { name = "k0kishima", email = "okishimaxyz@gmail.com" }
 ]
 dependencies = [
     "pydantic>=2.0.3",
 ]
```

