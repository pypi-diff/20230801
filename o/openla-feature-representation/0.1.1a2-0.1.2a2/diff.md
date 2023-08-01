# Comparing `tmp/openla_feature_representation-0.1.1a2.tar.gz` & `tmp/openla_feature_representation-0.1.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openla_feature_representation-0.1.1a2.tar", max compression
+gzip compressed data, was "openla_feature_representation-0.1.2a2.tar", max compression
```

## Comparing `openla_feature_representation-0.1.1a2.tar` & `openla_feature_representation-0.1.2a2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1061 2023-06-12 07:23:54.810526 openla_feature_representation-0.1.1a2/LICENSE
--rw-r--r--   0        0        0     5867 2023-07-11 07:33:03.678501 openla_feature_representation-0.1.1a2/README.md
--rw-r--r--   0        0        0      119 2023-07-03 04:59:58.021381 openla_feature_representation-0.1.1a2/openla_feature_representation/__init__.py
--rw-r--r--   0        0        0       77 2023-07-03 04:59:58.021619 openla_feature_representation-0.1.1a2/openla_feature_representation/alp/__init__.py
--rw-r--r--   0        0        0    17877 2023-07-03 04:59:58.021933 openla_feature_representation-0.1.1a2/openla_feature_representation/alp/extract_feature_alp.py
--rw-r--r--   0        0        0     4140 2023-07-03 04:59:58.022118 openla_feature_representation-0.1.1a2/openla_feature_representation/alp/features_extracted_function.py
--rw-r--r--   0        0        0    12068 2023-07-03 04:59:58.022306 openla_feature_representation-0.1.1a2/openla_feature_representation/alp/load_dataset.py
--rw-r--r--   0        0        0     5761 2023-07-03 04:59:58.022503 openla_feature_representation-0.1.1a2/openla_feature_representation/alp/utils.py
--rw-r--r--   0        0        0    15978 2023-07-03 04:59:58.022609 openla_feature_representation-0.1.1a2/openla_feature_representation/e2vec/openla_e2vec.py
--rw-r--r--   0        0        0      478 2023-07-19 00:51:00.610428 openla_feature_representation-0.1.1a2/pyproject.toml
--rw-r--r--   0        0        0     6502 1970-01-01 00:00:00.000000 openla_feature_representation-0.1.1a2/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-12 07:23:54.810526 openla_feature_representation-0.1.2a2/LICENSE
+-rw-r--r--   0        0        0     6637 2023-08-01 02:58:55.090720 openla_feature_representation-0.1.2a2/README.md
+-rw-r--r--   0        0        0      144 2023-08-01 02:58:55.091262 openla_feature_representation-0.1.2a2/openla_feature_representation/__init__.py
+-rw-r--r--   0        0        0       98 2023-08-01 02:58:55.091502 openla_feature_representation-0.1.2a2/openla_feature_representation/alp/__init__.py
+-rw-r--r--   0        0        0     4229 2023-08-01 02:58:55.091724 openla_feature_representation-0.1.2a2/openla_feature_representation/alp/alp.py
+-rw-r--r--   0        0        0    17877 2023-07-24 07:25:27.952909 openla_feature_representation-0.1.2a2/openla_feature_representation/alp/extract_feature_alp.py
+-rw-r--r--   0        0        0     4140 2023-07-19 01:21:26.861240 openla_feature_representation-0.1.2a2/openla_feature_representation/alp/features_extracted_function.py
+-rw-r--r--   0        0        0    12068 2023-07-19 01:21:26.861594 openla_feature_representation-0.1.2a2/openla_feature_representation/alp/load_dataset.py
+-rw-r--r--   0        0        0     5761 2023-07-19 01:21:26.861915 openla_feature_representation-0.1.2a2/openla_feature_representation/alp/utils.py
+-rw-r--r--   0        0        0    23073 2023-08-01 02:58:55.092209 openla_feature_representation-0.1.2a2/openla_feature_representation/e2vec/openla_e2vec.py
+-rw-r--r--   0        0        0      480 2023-08-01 04:17:54.117181 openla_feature_representation-0.1.2a2/pyproject.toml
+-rw-r--r--   0        0        0     7272 1970-01-01 00:00:00.000000 openla_feature_representation-0.1.2a2/PKG-INFO
```

### Comparing `openla_feature_representation-0.1.1a2/LICENSE` & `openla_feature_representation-0.1.2a2/LICENSE`

 * *Files identical despite different names*

### Comparing `openla_feature_representation-0.1.1a2/README.md` & `openla_feature_representation-0.1.2a2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -26,138 +26,149 @@
 ```
 
 ### Initializing the class
 
 This is the constructor:
 
 ```py
-e2Vec = lafr.E2Vec(fT_model_path, info_dir, course_id)
+e2Vec = lafr.E2Vec(ftmodel_path, input_csv_dir_path, course_id)
 ```
 
-- `fT_model_path` is the path to a fastText language model trained for this task
-- `info_dir` is the path to a directory with the dataset (see below)
+- `ftmodel_path` is the path to a fastText language model trained for this task
+- `input_csv_dir_path` is the path to a directory with the dataset (see below)
 - `course_id` is a string to identify files for the course to analyze within the `info_dir` directory (e.g. `'A-2023'`)
 
 After getting your own `e2Vec` object, all methods the class provides can be used on it.
 
 ### Generate sentences for the event log
 
 The fastText model uses an artificial language to express event log entries as sentences. This is how you can generate them:
 
 ```py
-sentences = e2Vec.get_Sentences(
-    sentences_path=sentence_path,
-    eventstream_path=eventstream_path,
-    info_dir=info_dir,
+sentences = e2Vec.generate_sentences(
+    sentences_dir_path=sentences_dir_path,
+    eventstream_file_path=eventstream_file_path,
+    input_csv_dir_path=input_csv_dir_path,
     course_id=course_id,
 )
 ```
 
 If you need to select or filter a time span:
 
 ```py
-sentences = e2Vec.get_Sentences(
-    sentences_path=sentence_path,
-    mode="select",
-    start=0,
-    period=90,
-    eventstream_path=eventstream_path,
-    info_dir=info_dir,
+sentences = e2Vec.generate_sentences(
+    sentences_dir_path=sentence_path,
+    use_timespan=True,
+    start_minute=0,
+    total_minutes=90,
+    eventstream_file_path=eventstream_file_path,
+    input_csv_dir_path=input_csv_dir_path,
     course_id=course_id,
 )
 ```
 
-- `sentence_path` is the path to the directory where you want the sentence files to be written
-- `eventstream_path` is the path to the event stream csv file
-- `info_dir` is the path to a directory with the dataset (see below)
+- `sentences_dir_path` is the path to the directory where you want the sentence files to be written
+- `eventstream_file_path` is the path to the event stream csv file
+- `input_csv_dir_path` is the path to a directory with the dataset (see below)
 - `course_id` is a string to identify files for the course to analyze within the `info_dir` directory
-- `mode` can be either `"all"` or `"select"` (optional)
-- `start` is the minute in the data the sentence generation should start (optional)
-- `period` is the number of minutes worth of sentences that should be generated (optional)
+- `use_timespan` if `True`, the args below will be used to extract a timespan from the data (optional)
+- `start_minute` is the minute in the data the sentence generation should start (optional)
+- `total_minutes` is the number of minutes worth of sentences that should be generated (optional)
 
 This function saves the sentences to a text file and returns a path to it.
 
 ### Vectorize the sentences
 
 This function returns a pandas DataFrame with the vectors generated from the sentences.
 
 ```py
-user_vectors = e2Vec.sentences_to_vector(sentences_path, save_path)
+user_vectors = e2Vec.vectorize_sentences(sentences_file_path)
 ```
 
-- `sentences_path` is the path to the sentence files generated in the previous step
-- `save_path` needs a string, but it is currently unused (to be removed)
+- `sentences_file_path` is the path to the sentence files generated in the previous step
 
 ### Concatenation
 
 The class has a function to concatenate vectors by time (minutes) or weeks.
 
 This will concatenate the vectors in 10-minute spans.
 
 ```py
-user_vec_C = e2Vec.get_concat_vectors(
-    sentences_path=sentence_path,
-    eventstream_path=eventstream_path,
-    vector_path="",
-    info_dir=eduData,
+vectors = e2Vec.concatenate_vectors(
+    sentences_dir_path=sentences_dir_path,
+    eventstream_file_path=eventstream_file_path,
+    input_csv_dir_path=eduData,
     course_id=course_id,
-    concat_mode="time",
-    start=0,
-    period=10,
+    start_minute=0,
+    total_minutes=10,
 )
 ```
 
 This will concatenate the vectors by the week or lesson.
 
 ```py
-user_vec_C = e2Vec.get_concat_vectors(
-    sentences_path=sentence_path,
-    eventstream_path=eventstream_path,
-    vector_path="",
-    info_dir=eduData,
+vectors = e2Vec.concatenate_vectors(
+    sentences_dir_path=sentences_dir_path,
+    eventstream_file_path=eventstream_file_path,
+    input_csv_dir_path=eduData,
     course_id=course_id,
-    concat_mode="week",
-    start=0,
+    by_weeks=True,
+    start_minute=0,
 )
 ```
 
-- `sentences_path` is the path to the sentence files generated in the previous step
-- `eventstream_path` is the path to the event stream csv file
-- `vector_path` needs a string, but it is currently unused (to be removed)
-- `info_dir` is the path to a directory with the dataset (see below)
+- `sentences_dir_path` is the path to the sentence files generated in the previous step
+- `eventstream_file_path` is the path to the event stream csv file
+- `input_csv_dir_path` is the path to a directory with the dataset (see below)
 - `course_id` is a string to identify files for the course to analyze within the `info_dir` directory
-- `concat_mode` needs to be "time" or "week"
-- `start` is the minute in the data the sentence generation should start (optional)
-- `period` is the number of minutes worth of sentences that should be generated each time (optional)
+- `by_weeks` concatenates vectors by week if `True` (by time by default)
+- `start_minute` is the minute in the data the sentence generation should start (optional)
+- `total_minutes` is the number of minutes worth of sentences that should be generated each time (optional)
 
-## Usage of the ALP (Active Learner Point) functions
+## Usage of the ALP class
 
-ALP is a set of metrics that take BookRoll (ebook) and Moodle activity per lecture into account: attendance, report submissions, course views, slide views, adding markers or memos, and other actions.
-
-First, the `aggregate_feature` function aggregates the number of times each user took any of the actions above for each lecture, resulting on a DataFrame that we will call `features_df` on this example. These are the features ALP will work with.
+ALP (Active Learner Point) is a set of metrics that take BookRoll (ebook) and Moodle activity per lecture into account: attendance, report submissions, course views, slide views, adding markers or memos, and other actions.
 
 ```py
-from openla_feature_representation import aggregate_feature
-features_df = aggregate_feature(course_id=course_id)
+from openla_feature_representation import Alp
+alp = Alp(course_id="114")
 ```
 
-- `course_id` is an `int` to identify files for the course to analyze within the `Dataset` directory
+- `course_id` is a string to identify files for the course to analyze within the `Dataset` directory
+
+The `Alp` class constructor above makes three DataFrames available as properties of the returned `Alp` object:
+
+- `features_df`: aggregated totals of how many times each user took any of the relevant actions for each lecture
+- `alp_df`: the features above replaced by a number from 0 to 5 following the criteria below
+- `alp_df_normalized`: same as above, only the 0 to 5 numbers are normalized between 0 and 1
 
-To further ready the data for ML and other analysis, the `feature2ALP` function returns a DataFrame that we will call `alp_df`, in which the feature is replaced by a number from 0 to 5 with the following meaning:
+### Criteria for the ALP 0-to-5 scale
 
-- `5`: Top 10%, or attending the lecture, or submitting a report
-- `4`: Top 20%
-- `3`: Top 30%, or being late to the lecture, or submitting late
-- `2`: Top 40%
-- `1`: Top 50%
-- `0`: Bottom 50%, or not attending, or not submitting
+| value | description                                               |
+| ----- | --------------------------------------------------------- |
+| `5`:  | Top 10%, or attending the lecture, or submitting a report |
+| `4`:  | Top 20%                                                   |
+| `3`:  | Top 30%, or being late to the lecture, or submitting late |
+| `2`:  | Top 40%                                                   |
+| `1`:  | Top 50%                                                   |
+| `0`:  | Bottom 50%, or not attending, or not submitting           |
 
-The additional `alp_df_normalized` DataFrame returned by the function is the same data as `alp_df`, only normalized to `1`.
+### Examples for the class's methods and instance variables
 
 ```py
-from openla_feature_representation import feature2ALP
-alp_df, alp_df_normalized = feature2ALP(features_df=features_df)
+alp.features_df       # These are the aggregated features
+alp.alp_df            # These are the ALP 0-to-5 values
+alp.alp_df_normalized # These are the normalized values
+
+# The following will write CSV files for the relevant DataFrame
+# Paths and filenames can be specified, but there are default
+# filenames and the paths default to the present directory
+alp.write_features_csv()
+alp.write_alp_csv()
+alp.write_alp_normalized_csv()
 ```
 
 ## Datasets for OpenLA
 
 This module uses data in the same or a similar format as OpenLA. Please refer to the [OpenLA documentation](https://limu.ait.kyushu-u.ac.jp/~openLA/) for further information.
+
+Datasets for the `Alp` class must be placed in the `"Dataset/"` directory relative to the Python script they are called from.
```

### Comparing `openla_feature_representation-0.1.1a2/openla_feature_representation/alp/extract_feature_alp.py` & `openla_feature_representation-0.1.2a2/openla_feature_representation/alp/extract_feature_alp.py`

 * *Files identical despite different names*

### Comparing `openla_feature_representation-0.1.1a2/openla_feature_representation/alp/features_extracted_function.py` & `openla_feature_representation-0.1.2a2/openla_feature_representation/alp/features_extracted_function.py`

 * *Files identical despite different names*

### Comparing `openla_feature_representation-0.1.1a2/openla_feature_representation/alp/load_dataset.py` & `openla_feature_representation-0.1.2a2/openla_feature_representation/alp/load_dataset.py`

 * *Files identical despite different names*

### Comparing `openla_feature_representation-0.1.1a2/openla_feature_representation/alp/utils.py` & `openla_feature_representation-0.1.2a2/openla_feature_representation/alp/utils.py`

 * *Files identical despite different names*

### Comparing `openla_feature_representation-0.1.1a2/PKG-INFO` & `openla_feature_representation-0.1.2a2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openla-feature-representation
-Version: 0.1.1a2
+Version: 0.1.2a2
 Summary: A Python module that adds features to OpenLA data to make it easier to use for ML
 Author: LIMU
 Author-email: repository@limu.ait.kyushu-u.ac.jp
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -42,139 +42,150 @@
 ```
 
 ### Initializing the class
 
 This is the constructor:
 
 ```py
-e2Vec = lafr.E2Vec(fT_model_path, info_dir, course_id)
+e2Vec = lafr.E2Vec(ftmodel_path, input_csv_dir_path, course_id)
 ```
 
-- `fT_model_path` is the path to a fastText language model trained for this task
-- `info_dir` is the path to a directory with the dataset (see below)
+- `ftmodel_path` is the path to a fastText language model trained for this task
+- `input_csv_dir_path` is the path to a directory with the dataset (see below)
 - `course_id` is a string to identify files for the course to analyze within the `info_dir` directory (e.g. `'A-2023'`)
 
 After getting your own `e2Vec` object, all methods the class provides can be used on it.
 
 ### Generate sentences for the event log
 
 The fastText model uses an artificial language to express event log entries as sentences. This is how you can generate them:
 
 ```py
-sentences = e2Vec.get_Sentences(
-    sentences_path=sentence_path,
-    eventstream_path=eventstream_path,
-    info_dir=info_dir,
+sentences = e2Vec.generate_sentences(
+    sentences_dir_path=sentences_dir_path,
+    eventstream_file_path=eventstream_file_path,
+    input_csv_dir_path=input_csv_dir_path,
     course_id=course_id,
 )
 ```
 
 If you need to select or filter a time span:
 
 ```py
-sentences = e2Vec.get_Sentences(
-    sentences_path=sentence_path,
-    mode="select",
-    start=0,
-    period=90,
-    eventstream_path=eventstream_path,
-    info_dir=info_dir,
+sentences = e2Vec.generate_sentences(
+    sentences_dir_path=sentence_path,
+    use_timespan=True,
+    start_minute=0,
+    total_minutes=90,
+    eventstream_file_path=eventstream_file_path,
+    input_csv_dir_path=input_csv_dir_path,
     course_id=course_id,
 )
 ```
 
-- `sentence_path` is the path to the directory where you want the sentence files to be written
-- `eventstream_path` is the path to the event stream csv file
-- `info_dir` is the path to a directory with the dataset (see below)
+- `sentences_dir_path` is the path to the directory where you want the sentence files to be written
+- `eventstream_file_path` is the path to the event stream csv file
+- `input_csv_dir_path` is the path to a directory with the dataset (see below)
 - `course_id` is a string to identify files for the course to analyze within the `info_dir` directory
-- `mode` can be either `"all"` or `"select"` (optional)
-- `start` is the minute in the data the sentence generation should start (optional)
-- `period` is the number of minutes worth of sentences that should be generated (optional)
+- `use_timespan` if `True`, the args below will be used to extract a timespan from the data (optional)
+- `start_minute` is the minute in the data the sentence generation should start (optional)
+- `total_minutes` is the number of minutes worth of sentences that should be generated (optional)
 
 This function saves the sentences to a text file and returns a path to it.
 
 ### Vectorize the sentences
 
 This function returns a pandas DataFrame with the vectors generated from the sentences.
 
 ```py
-user_vectors = e2Vec.sentences_to_vector(sentences_path, save_path)
+user_vectors = e2Vec.vectorize_sentences(sentences_file_path)
 ```
 
-- `sentences_path` is the path to the sentence files generated in the previous step
-- `save_path` needs a string, but it is currently unused (to be removed)
+- `sentences_file_path` is the path to the sentence files generated in the previous step
 
 ### Concatenation
 
 The class has a function to concatenate vectors by time (minutes) or weeks.
 
 This will concatenate the vectors in 10-minute spans.
 
 ```py
-user_vec_C = e2Vec.get_concat_vectors(
-    sentences_path=sentence_path,
-    eventstream_path=eventstream_path,
-    vector_path="",
-    info_dir=eduData,
+vectors = e2Vec.concatenate_vectors(
+    sentences_dir_path=sentences_dir_path,
+    eventstream_file_path=eventstream_file_path,
+    input_csv_dir_path=eduData,
     course_id=course_id,
-    concat_mode="time",
-    start=0,
-    period=10,
+    start_minute=0,
+    total_minutes=10,
 )
 ```
 
 This will concatenate the vectors by the week or lesson.
 
 ```py
-user_vec_C = e2Vec.get_concat_vectors(
-    sentences_path=sentence_path,
-    eventstream_path=eventstream_path,
-    vector_path="",
-    info_dir=eduData,
+vectors = e2Vec.concatenate_vectors(
+    sentences_dir_path=sentences_dir_path,
+    eventstream_file_path=eventstream_file_path,
+    input_csv_dir_path=eduData,
     course_id=course_id,
-    concat_mode="week",
-    start=0,
+    by_weeks=True,
+    start_minute=0,
 )
 ```
 
-- `sentences_path` is the path to the sentence files generated in the previous step
-- `eventstream_path` is the path to the event stream csv file
-- `vector_path` needs a string, but it is currently unused (to be removed)
-- `info_dir` is the path to a directory with the dataset (see below)
+- `sentences_dir_path` is the path to the sentence files generated in the previous step
+- `eventstream_file_path` is the path to the event stream csv file
+- `input_csv_dir_path` is the path to a directory with the dataset (see below)
 - `course_id` is a string to identify files for the course to analyze within the `info_dir` directory
-- `concat_mode` needs to be "time" or "week"
-- `start` is the minute in the data the sentence generation should start (optional)
-- `period` is the number of minutes worth of sentences that should be generated each time (optional)
+- `by_weeks` concatenates vectors by week if `True` (by time by default)
+- `start_minute` is the minute in the data the sentence generation should start (optional)
+- `total_minutes` is the number of minutes worth of sentences that should be generated each time (optional)
 
-## Usage of the ALP (Active Learner Point) functions
+## Usage of the ALP class
 
-ALP is a set of metrics that take BookRoll (ebook) and Moodle activity per lecture into account: attendance, report submissions, course views, slide views, adding markers or memos, and other actions.
-
-First, the `aggregate_feature` function aggregates the number of times each user took any of the actions above for each lecture, resulting on a DataFrame that we will call `features_df` on this example. These are the features ALP will work with.
+ALP (Active Learner Point) is a set of metrics that take BookRoll (ebook) and Moodle activity per lecture into account: attendance, report submissions, course views, slide views, adding markers or memos, and other actions.
 
 ```py
-from openla_feature_representation import aggregate_feature
-features_df = aggregate_feature(course_id=course_id)
+from openla_feature_representation import Alp
+alp = Alp(course_id="114")
 ```
 
-- `course_id` is an `int` to identify files for the course to analyze within the `Dataset` directory
+- `course_id` is a string to identify files for the course to analyze within the `Dataset` directory
+
+The `Alp` class constructor above makes three DataFrames available as properties of the returned `Alp` object:
+
+- `features_df`: aggregated totals of how many times each user took any of the relevant actions for each lecture
+- `alp_df`: the features above replaced by a number from 0 to 5 following the criteria below
+- `alp_df_normalized`: same as above, only the 0 to 5 numbers are normalized between 0 and 1
 
-To further ready the data for ML and other analysis, the `feature2ALP` function returns a DataFrame that we will call `alp_df`, in which the feature is replaced by a number from 0 to 5 with the following meaning:
+### Criteria for the ALP 0-to-5 scale
 
-- `5`: Top 10%, or attending the lecture, or submitting a report
-- `4`: Top 20%
-- `3`: Top 30%, or being late to the lecture, or submitting late
-- `2`: Top 40%
-- `1`: Top 50%
-- `0`: Bottom 50%, or not attending, or not submitting
+| value | description                                               |
+| ----- | --------------------------------------------------------- |
+| `5`:  | Top 10%, or attending the lecture, or submitting a report |
+| `4`:  | Top 20%                                                   |
+| `3`:  | Top 30%, or being late to the lecture, or submitting late |
+| `2`:  | Top 40%                                                   |
+| `1`:  | Top 50%                                                   |
+| `0`:  | Bottom 50%, or not attending, or not submitting           |
 
-The additional `alp_df_normalized` DataFrame returned by the function is the same data as `alp_df`, only normalized to `1`.
+### Examples for the class's methods and instance variables
 
 ```py
-from openla_feature_representation import feature2ALP
-alp_df, alp_df_normalized = feature2ALP(features_df=features_df)
+alp.features_df       # These are the aggregated features
+alp.alp_df            # These are the ALP 0-to-5 values
+alp.alp_df_normalized # These are the normalized values
+
+# The following will write CSV files for the relevant DataFrame
+# Paths and filenames can be specified, but there are default
+# filenames and the paths default to the present directory
+alp.write_features_csv()
+alp.write_alp_csv()
+alp.write_alp_normalized_csv()
 ```
 
 ## Datasets for OpenLA
 
 This module uses data in the same or a similar format as OpenLA. Please refer to the [OpenLA documentation](https://limu.ait.kyushu-u.ac.jp/~openLA/) for further information.
 
+Datasets for the `Alp` class must be placed in the `"Dataset/"` directory relative to the Python script they are called from.
+
```

