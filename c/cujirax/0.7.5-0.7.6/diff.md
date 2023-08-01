# Comparing `tmp/cujirax-0.7.5.tar.gz` & `tmp/cujirax-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cujirax-0.7.5.tar", last modified: Fri Jul 14 14:54:11 2023, max compression
+gzip compressed data, was "cujirax-0.7.6.tar", last modified: Tue Aug  1 16:37:52 2023, max compression
```

## Comparing `cujirax-0.7.5.tar` & `cujirax-0.7.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1836 2023-03-28 01:53:23.346105 cujirax-0.7.5/.gitignore
--rw-r--r--   0        0        0     1064 2023-03-08 08:56:39.228892 cujirax-0.7.5/LICENSE
--rw-r--r--   0        0        0      519 2023-03-11 13:29:07.840641 cujirax-0.7.5/README.md
--rw-r--r--   0        0        0    10592 2023-07-14 14:53:19.473427 cujirax-0.7.5/cujirax/__init__.py
--rw-r--r--   0        0        0     2120 2023-06-22 16:26:46.910876 cujirax-0.7.5/cujirax/cucumber.py
--rw-r--r--   0        0        0     4230 2023-04-13 07:40:02.924013 cujirax-0.7.5/cujirax/jira.py
--rw-r--r--   0        0        0     2735 2023-04-24 16:49:30.639020 cujirax-0.7.5/cujirax/xray/__init__.py
--rw-r--r--   0        0        0      961 2023-04-24 16:50:20.686692 cujirax-0.7.5/cujirax/xray/graphql.py
--rw-r--r--   0        0        0     1605 2023-03-30 07:41:41.303508 cujirax-0.7.5/cujirax/xray/import_results.py
--rw-r--r--   0        0        0     2079 2023-03-30 13:06:45.294265 cujirax-0.7.5/cujirax/xray/import_tests.py
--rw-r--r--   0        0        0      483 2023-07-14 14:52:14.617711 cujirax-0.7.5/pyproject.toml
--rw-r--r--   0        0        0      932 1970-01-01 00:00:00.000000 cujirax-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0     1836 2023-03-28 01:53:23.346105 cujirax-0.7.6/.gitignore
+-rw-r--r--   0        0        0     1064 2023-03-08 08:56:39.228892 cujirax-0.7.6/LICENSE
+-rw-r--r--   0        0        0      519 2023-03-11 13:29:07.840641 cujirax-0.7.6/README.md
+-rw-r--r--   0        0        0    10879 2023-08-01 16:36:46.872051 cujirax-0.7.6/cujirax/__init__.py
+-rw-r--r--   0        0        0     2120 2023-06-22 16:26:46.910876 cujirax-0.7.6/cujirax/cucumber.py
+-rw-r--r--   0        0        0     4230 2023-04-13 07:40:02.924013 cujirax-0.7.6/cujirax/jira.py
+-rw-r--r--   0        0        0     2735 2023-04-24 16:49:30.639020 cujirax-0.7.6/cujirax/xray/__init__.py
+-rw-r--r--   0        0        0      961 2023-04-24 16:50:20.686692 cujirax-0.7.6/cujirax/xray/graphql.py
+-rw-r--r--   0        0        0     1605 2023-03-30 07:41:41.303508 cujirax-0.7.6/cujirax/xray/import_results.py
+-rw-r--r--   0        0        0     2079 2023-03-30 13:06:45.294265 cujirax-0.7.6/cujirax/xray/import_tests.py
+-rw-r--r--   0        0        0      483 2023-07-14 14:52:14.617711 cujirax-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0      932 1970-01-01 00:00:00.000000 cujirax-0.7.6/PKG-INFO
```

### Comparing `cujirax-0.7.5/.gitignore` & `cujirax-0.7.6/.gitignore`

 * *Files identical despite different names*

### Comparing `cujirax-0.7.5/LICENSE` & `cujirax-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cujirax-0.7.5/README.md` & `cujirax-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `cujirax-0.7.5/cujirax/__init__.py` & `cujirax-0.7.6/cujirax/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Cucumber result to Jira Xray Test repository
 
 """
-__version__ = "0.7.5"
+__version__ = "0.7.6"
 
 
 import datetime
 
 import cujirax.cucumber as cucumber
 import cujirax.xray.import_results as result
 import cujirax.xray.import_tests as test
@@ -163,59 +163,64 @@
         assert testplan_name, "Test plan name cannot be None"
         return self.jira.create_testplan(summary=testplan_name, description=testplan_desc)
 
     @classmethod
     def _get_results(cls, elements: Element, j: JiraX, ignore_duplicate):
         test_request_obj = []
         results = []
-        for el in elements:
-            test_name = cls.scenarioid_to_tescasename(el.id, el.keyword)
-            tests = j.get_tests(test_name)
-            if not tests:
-                raise ValueError("Test not created: {}".format(test_name))
-            
-            test_key = tests[0]
-            if not ignore_duplicate:
-                if len(tests) > 1:
-                    logger.error(test_name)
-                    logger.error(["{}".format(t) for t in tests])
-                    raise ValueError("More than 1 test key detected: ", tests, test_name)
-                    
-            statuses = [step.result.status.value for step in el.steps]
-            agg_result = "passed" if all(s == 'passed' for s in statuses) else "failed"
-            test_request_obj.append(result.Test(testKey=str(test_key), status=agg_result))
-            results.append(agg_result)
-        grand_result = "passed" if all(s == 'passed' for s in results) else "failed"
+        logger.info(elements)
+        if elements:
+            for el in elements:
+                test_name = cls.scenarioid_to_tescasename(el.id, el.keyword)
+                tests = j.get_tests(test_name)
+                if not tests:
+                    raise ValueError("Test not created: {}".format(test_name))
+                
+                test_key = tests[0]
+                if not ignore_duplicate:
+                    if len(tests) > 1:
+                        logger.error(test_name)
+                        logger.error(["{}".format(t) for t in tests])
+                        raise ValueError("More than 1 test key detected: ", tests, test_name)
+                        
+                statuses = [step.result.status.value for step in el.steps]
+                agg_result = "passed" if all(s == 'passed' for s in statuses) else "failed"
+                test_request_obj.append(result.Test(testKey=str(test_key), status=agg_result))
+                results.append(agg_result)
+            grand_result = "passed" if all(s == 'passed' for s in results) else "failed"
+        else:
+            grand_result = "failed"
         return test_request_obj, grand_result
 
     @classmethod
     def _split_elements_to_exist_and_new(cls, elements: Element, j: JiraX, ignore_duplicate):
         found= []
         not_found = []
-        
-        for el in elements:
-            test_name = cls.scenarioid_to_tescasename(el.id, el.keyword)
-            logger.info("searching_test_name: " + test_name)
-
-            tests = j.get_tests(test_name)
-
-            if tests and not ignore_duplicate:
-                if len(tests) > 1:
-                    logger.error(test_name)
-                    logger.error(["{}".format(t) for t in tests])
-                    raise ValueError("More than 1 test key detected: ", tests, test_name)
-            logger.info("found_in_jira: " + str(tests))
-            found.append(el) if j.get_tests(test_name) else not_found.append(el)
-        
-        # check duplicate for new test
-        if not ignore_duplicate:
-            new_testnames = [cls.scenarioid_to_tescasename(el.id, el.keyword) for el in not_found]
-            duplicates = [item for item, count in Counter(new_testnames).items() if count > 1]
-            if duplicates:
-                raise ValueError("More than 1 same test detected: ", duplicates)
+        logger.info(elements)
+        if elements:
+            for el in elements:
+                test_name = cls.scenarioid_to_tescasename(el.id, el.keyword)
+                logger.info("searching_test_name: " + test_name)
+
+                tests = j.get_tests(test_name)
+
+                if tests and not ignore_duplicate:
+                    if len(tests) > 1:
+                        logger.error(test_name)
+                        logger.error(["{}".format(t) for t in tests])
+                        raise ValueError("More than 1 test key detected: ", tests, test_name)
+                logger.info("found_in_jira: " + str(tests))
+                found.append(el) if j.get_tests(test_name) else not_found.append(el)
+            
+            # check duplicate for new test
+            if not ignore_duplicate:
+                new_testnames = [cls.scenarioid_to_tescasename(el.id, el.keyword) for el in not_found]
+                duplicates = [item for item, count in Counter(new_testnames).items() if count > 1]
+                if duplicates:
+                    raise ValueError("More than 1 same test detected: ", duplicates)
 
         return found, not_found
     
     @classmethod
     def _new_testcase(
         cls, 
         element: Element,
```

### Comparing `cujirax-0.7.5/cujirax/cucumber.py` & `cujirax-0.7.6/cujirax/cucumber.py`

 * *Files identical despite different names*

### Comparing `cujirax-0.7.5/cujirax/jira.py` & `cujirax-0.7.6/cujirax/jira.py`

 * *Files identical despite different names*

### Comparing `cujirax-0.7.5/cujirax/xray/__init__.py` & `cujirax-0.7.6/cujirax/xray/__init__.py`

 * *Files identical despite different names*

### Comparing `cujirax-0.7.5/cujirax/xray/graphql.py` & `cujirax-0.7.6/cujirax/xray/graphql.py`

 * *Files identical despite different names*

### Comparing `cujirax-0.7.5/cujirax/xray/import_results.py` & `cujirax-0.7.6/cujirax/xray/import_results.py`

 * *Files identical despite different names*

### Comparing `cujirax-0.7.5/cujirax/xray/import_tests.py` & `cujirax-0.7.6/cujirax/xray/import_tests.py`

 * *Files identical despite different names*

### Comparing `cujirax-0.7.5/PKG-INFO` & `cujirax-0.7.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cujirax
-Version: 0.7.5
+Version: 0.7.6
 Summary: Cucumber result to Jira Xray Test repository
 Author-email: Max Leow <maxengiu@outlook.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: pydantic==1.10.10
 Requires-Dist: atlassian-python-api
 Requires-Dist: requests
```

