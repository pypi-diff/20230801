# Comparing `tmp/eyeball_pp-0.0.5.tar.gz` & `tmp/eyeball_pp-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eyeball_pp-0.0.5.tar", last modified: Fri Jul 28 06:34:15 2023, max compression
+gzip compressed data, was "eyeball_pp-0.0.6.tar", last modified: Tue Aug  1 20:05:20 2023, max compression
```

## Comparing `eyeball_pp-0.0.5.tar` & `eyeball_pp-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-07-28 06:34:15.066982 eyeball_pp-0.0.5/
--rw-r--r--   0 revant     (501) staff       (20)    11357 2023-06-21 17:31:20.000000 eyeball_pp-0.0.5/LICENSE
--rw-r--r--   0 revant     (501) staff       (20)     8903 2023-07-28 06:34:15.067147 eyeball_pp-0.0.5/PKG-INFO
--rw-r--r--   0 revant     (501) staff       (20)     8520 2023-07-12 19:49:37.000000 eyeball_pp-0.0.5/README.md
-drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-07-28 06:34:15.065050 eyeball_pp-0.0.5/eyeball_pp/
--rw-r--r--   0 revant     (501) staff       (20)      757 2023-06-27 22:22:21.000000 eyeball_pp-0.0.5/eyeball_pp/__init__.py
--rw-r--r--   0 revant     (501) staff       (20)     2307 2023-07-13 18:39:56.000000 eyeball_pp-0.0.5/eyeball_pp/classes.py
--rw-r--r--   0 revant     (501) staff       (20)     2137 2023-07-12 21:50:50.000000 eyeball_pp-0.0.5/eyeball_pp/comparators.py
--rw-r--r--   0 revant     (501) staff       (20)      201 2023-06-27 19:58:23.000000 eyeball_pp-0.0.5/eyeball_pp/compare_checkpoints.py
--rw-r--r--   0 revant     (501) staff       (20)    40130 2023-07-28 06:25:03.000000 eyeball_pp-0.0.5/eyeball_pp/eval.py
--rw-r--r--   0 revant     (501) staff       (20)    36960 2023-07-28 05:50:48.000000 eyeball_pp-0.0.5/eyeball_pp/recorders.py
--rw-r--r--   0 revant     (501) staff       (20)      728 2023-07-26 18:52:02.000000 eyeball_pp-0.0.5/eyeball_pp/utils.py
-drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-07-28 06:34:15.066717 eyeball_pp-0.0.5/eyeball_pp.egg-info/
--rw-r--r--   0 revant     (501) staff       (20)     8903 2023-07-28 06:34:15.000000 eyeball_pp-0.0.5/eyeball_pp.egg-info/PKG-INFO
--rw-r--r--   0 revant     (501) staff       (20)      340 2023-07-28 06:34:15.000000 eyeball_pp-0.0.5/eyeball_pp.egg-info/SOURCES.txt
--rw-r--r--   0 revant     (501) staff       (20)        1 2023-07-28 06:34:15.000000 eyeball_pp-0.0.5/eyeball_pp.egg-info/dependency_links.txt
--rw-r--r--   0 revant     (501) staff       (20)       11 2023-07-28 06:34:15.000000 eyeball_pp-0.0.5/eyeball_pp.egg-info/top_level.txt
--rw-r--r--   0 revant     (501) staff       (20)      527 2023-07-28 06:34:15.067987 eyeball_pp-0.0.5/setup.cfg
--rw-r--r--   0 revant     (501) staff       (20)       38 2023-06-23 17:41:10.000000 eyeball_pp-0.0.5/setup.py
+drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-08-01 20:05:20.752260 eyeball_pp-0.0.6/
+-rw-r--r--   0 revant     (501) staff       (20)    11357 2023-06-21 17:31:20.000000 eyeball_pp-0.0.6/LICENSE
+-rw-r--r--   0 revant     (501) staff       (20)     8982 2023-08-01 20:05:20.752408 eyeball_pp-0.0.6/PKG-INFO
+-rw-r--r--   0 revant     (501) staff       (20)     8599 2023-07-31 17:27:10.000000 eyeball_pp-0.0.6/README.md
+drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-08-01 20:05:20.742570 eyeball_pp-0.0.6/eyeball_pp/
+-rw-r--r--   0 revant     (501) staff       (20)      757 2023-06-27 22:22:21.000000 eyeball_pp-0.0.6/eyeball_pp/__init__.py
+-rw-r--r--   0 revant     (501) staff       (20)     2307 2023-07-13 18:39:56.000000 eyeball_pp-0.0.6/eyeball_pp/classes.py
+-rw-r--r--   0 revant     (501) staff       (20)     2137 2023-07-12 21:50:50.000000 eyeball_pp-0.0.6/eyeball_pp/comparators.py
+-rw-r--r--   0 revant     (501) staff       (20)      201 2023-06-27 19:58:23.000000 eyeball_pp-0.0.6/eyeball_pp/compare_checkpoints.py
+-rw-r--r--   0 revant     (501) staff       (20)    40161 2023-08-01 20:04:24.000000 eyeball_pp-0.0.6/eyeball_pp/eval.py
+-rw-r--r--   0 revant     (501) staff       (20)    36960 2023-07-28 05:50:48.000000 eyeball_pp-0.0.6/eyeball_pp/recorders.py
+-rw-r--r--   0 revant     (501) staff       (20)      728 2023-07-26 18:52:02.000000 eyeball_pp-0.0.6/eyeball_pp/utils.py
+drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-08-01 20:05:20.751952 eyeball_pp-0.0.6/eyeball_pp.egg-info/
+-rw-r--r--   0 revant     (501) staff       (20)     8982 2023-08-01 20:05:20.000000 eyeball_pp-0.0.6/eyeball_pp.egg-info/PKG-INFO
+-rw-r--r--   0 revant     (501) staff       (20)      340 2023-08-01 20:05:20.000000 eyeball_pp-0.0.6/eyeball_pp.egg-info/SOURCES.txt
+-rw-r--r--   0 revant     (501) staff       (20)        1 2023-08-01 20:05:20.000000 eyeball_pp-0.0.6/eyeball_pp.egg-info/dependency_links.txt
+-rw-r--r--   0 revant     (501) staff       (20)       11 2023-08-01 20:05:20.000000 eyeball_pp-0.0.6/eyeball_pp.egg-info/top_level.txt
+-rw-r--r--   0 revant     (501) staff       (20)      527 2023-08-01 20:05:20.753051 eyeball_pp-0.0.6/setup.cfg
+-rw-r--r--   0 revant     (501) staff       (20)       38 2023-06-23 17:41:10.000000 eyeball_pp-0.0.6/setup.py
```

### Comparing `eyeball_pp-0.0.5/LICENSE` & `eyeball_pp-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `eyeball_pp-0.0.5/PKG-INFO` & `eyeball_pp-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyeball_pp
-Version: 0.0.5
+Version: 0.0.6
 Summary: A python package for evaluating tasks which use llms
 Home-page: https://github.com/revantk/eyeball-plus-plus
 Author: Revant
 Author-email: revant.kapoor@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -22,16 +22,19 @@
 If you've been eyeballing how well your changes are working, this framework should fit right in and help you evaluate your task in a more methodical manner.
 
 # Installation
 eyeball_pp is a python library which can be installed via pip 
 
 `pip install eyeball_pp`
 
+# Example 
+To see an example see this [notebook](examples/qa_task_notebook.ipynb) or checkout more examples in the [examples](examples/) folder. 
+
 # Concepts 
-eyeball_pp has 3 simple concepts -- record, rerun and compare. To see a detailed example check out the examples/ folder in the repo
+eyeball_pp has 3 simple concepts -- record, rerun and compare. 
 
 ## Record
 eyeball_pp consists of a recorder which records the inputs and outputs of your task runs as you are running it and saves them as checkpoints. You can record this locally while developing or from a production system. You can optionally record human feedback for the task output too.
 
 You can record your task using the `record_task` decorator. This will record every run of this function call as a `Checkpoint` for future comparison. The args_to_record specify which inputs to record and the function return value is saved as the output.
 ```python
 import eyeball_pp
```

### Comparing `eyeball_pp-0.0.5/README.md` & `eyeball_pp-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,19 @@
 If you've been eyeballing how well your changes are working, this framework should fit right in and help you evaluate your task in a more methodical manner.
 
 # Installation
 eyeball_pp is a python library which can be installed via pip 
 
 `pip install eyeball_pp`
 
+# Example 
+To see an example see this [notebook](examples/qa_task_notebook.ipynb) or checkout more examples in the [examples](examples/) folder. 
+
 # Concepts 
-eyeball_pp has 3 simple concepts -- record, rerun and compare. To see a detailed example check out the examples/ folder in the repo
+eyeball_pp has 3 simple concepts -- record, rerun and compare. 
 
 ## Record
 eyeball_pp consists of a recorder which records the inputs and outputs of your task runs as you are running it and saves them as checkpoints. You can record this locally while developing or from a production system. You can optionally record human feedback for the task output too.
 
 You can record your task using the `record_task` decorator. This will record every run of this function call as a `Checkpoint` for future comparison. The args_to_record specify which inputs to record and the function return value is saved as the output.
 ```python
 import eyeball_pp
```

### Comparing `eyeball_pp-0.0.5/eyeball_pp/__init__.py` & `eyeball_pp-0.0.6/eyeball_pp/__init__.py`

 * *Files identical despite different names*

### Comparing `eyeball_pp-0.0.5/eyeball_pp/classes.py` & `eyeball_pp-0.0.6/eyeball_pp/classes.py`

 * *Files identical despite different names*

### Comparing `eyeball_pp-0.0.5/eyeball_pp/comparators.py` & `eyeball_pp-0.0.6/eyeball_pp/comparators.py`

 * *Files identical despite different names*

### Comparing `eyeball_pp-0.0.5/eyeball_pp/eval.py` & `eyeball_pp-0.0.6/eyeball_pp/eval.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     def set_config(self, **config_kwargs) -> None:
         self.config = EvaluatorConfig._merge(self.config, **config_kwargs)
         self.data_dir = os.path.join(self.config.dir_path, "eyeball_data")
         if self.config.api_key is not None:
             self.recorder: EvalRecorder = ApiClientRecorder(
                 api_key=self.config.api_key, api_url=self.config.api_url
             )
-        elif self.running_in_notebook:
+        elif self.running_in_notebook or not self.config.sample_rate:
             self.recorder = MemoryRecorder()
         else:
             self.recorder = FileRecorder(self.data_dir)
 
     @contextmanager
     def start_recording_session(
         self,
```

### Comparing `eyeball_pp-0.0.5/eyeball_pp/recorders.py` & `eyeball_pp-0.0.6/eyeball_pp/recorders.py`

 * *Files identical despite different names*

### Comparing `eyeball_pp-0.0.5/eyeball_pp/utils.py` & `eyeball_pp-0.0.6/eyeball_pp/utils.py`

 * *Files identical despite different names*

### Comparing `eyeball_pp-0.0.5/eyeball_pp.egg-info/PKG-INFO` & `eyeball_pp-0.0.6/eyeball_pp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyeball-pp
-Version: 0.0.5
+Version: 0.0.6
 Summary: A python package for evaluating tasks which use llms
 Home-page: https://github.com/revantk/eyeball-plus-plus
 Author: Revant
 Author-email: revant.kapoor@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -22,16 +22,19 @@
 If you've been eyeballing how well your changes are working, this framework should fit right in and help you evaluate your task in a more methodical manner.
 
 # Installation
 eyeball_pp is a python library which can be installed via pip 
 
 `pip install eyeball_pp`
 
+# Example 
+To see an example see this [notebook](examples/qa_task_notebook.ipynb) or checkout more examples in the [examples](examples/) folder. 
+
 # Concepts 
-eyeball_pp has 3 simple concepts -- record, rerun and compare. To see a detailed example check out the examples/ folder in the repo
+eyeball_pp has 3 simple concepts -- record, rerun and compare. 
 
 ## Record
 eyeball_pp consists of a recorder which records the inputs and outputs of your task runs as you are running it and saves them as checkpoints. You can record this locally while developing or from a production system. You can optionally record human feedback for the task output too.
 
 You can record your task using the `record_task` decorator. This will record every run of this function call as a `Checkpoint` for future comparison. The args_to_record specify which inputs to record and the function return value is saved as the output.
 ```python
 import eyeball_pp
```

### Comparing `eyeball_pp-0.0.5/setup.cfg` & `eyeball_pp-0.0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eyeball_pp
-version = 0.0.5
+version = 0.0.6
 description = A python package for evaluating tasks which use llms
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Revant
 author_email = revant.kapoor@gmail.com
 url = https://github.com/revantk/eyeball-plus-plus
 license_files = LICENSE
```

