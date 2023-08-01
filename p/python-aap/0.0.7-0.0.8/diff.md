# Comparing `tmp/python-aap-0.0.7.tar.gz` & `tmp/python-aap-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-aap-0.0.7.tar", last modified: Mon Jul 31 09:27:57 2023, max compression
+gzip compressed data, was "python-aap-0.0.8.tar", last modified: Tue Aug  1 11:38:26 2023, max compression
```

## Comparing `python-aap-0.0.7.tar` & `python-aap-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 gitlab-runner   (988) gitlab-runner   (982)        0 2023-07-31 09:27:57.246124 python-aap-0.0.7/
--rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)     2735 2023-07-28 10:54:04.000000 python-aap-0.0.7/.gitignore
--rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)     1963 2023-07-28 12:41:45.000000 python-aap-0.0.7/.gitlab-ci.yml
--rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)    18020 2023-07-26 20:23:00.000000 python-aap-0.0.7/LICENSE
--rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)     5310 2023-07-31 09:27:57.245124 python-aap-0.0.7/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)     4717 2023-07-31 09:27:45.000000 python-aap-0.0.7/README.md
--rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)      817 2023-07-31 09:27:45.000000 python-aap-0.0.7/pyproject.toml
--rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)       17 2023-07-28 10:54:04.000000 python-aap-0.0.7/requirements.txt
--rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)       38 2023-07-31 09:27:57.246124 python-aap-0.0.7/setup.cfg
-drwxrwxr-x   0 gitlab-runner   (988) gitlab-runner   (982)        0 2023-07-31 09:27:57.239123 python-aap-0.0.7/src/
-drwxrwxr-x   0 gitlab-runner   (988) gitlab-runner   (982)        0 2023-07-31 09:27:57.244124 python-aap-0.0.7/src/aap/
--rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)      265 2023-07-28 12:41:45.000000 python-aap-0.0.7/src/aap/__init__.py
--rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)     4037 2023-07-31 09:26:15.000000 python-aap-0.0.7/src/aap/__main__.py
--rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)     5364 2023-07-28 12:41:45.000000 python-aap-0.0.7/src/aap/base.py
--rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)     3090 2023-07-28 12:41:45.000000 python-aap-0.0.7/src/aap/endpoints.py
--rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)     1901 2023-07-28 12:41:45.000000 python-aap-0.0.7/src/aap/mixins.py
-drwxrwxr-x   0 gitlab-runner   (988) gitlab-runner   (982)        0 2023-07-31 09:27:57.245124 python-aap-0.0.7/src/python_aap.egg-info/
--rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)     5310 2023-07-31 09:27:57.000000 python-aap-0.0.7/src/python_aap.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)      400 2023-07-31 09:27:57.000000 python-aap-0.0.7/src/python_aap.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)        1 2023-07-31 09:27:57.000000 python-aap-0.0.7/src/python_aap.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)       40 2023-07-31 09:27:57.000000 python-aap-0.0.7/src/python_aap.egg-info/entry_points.txt
--rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)       18 2023-07-31 09:27:57.000000 python-aap-0.0.7/src/python_aap.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)        4 2023-07-31 09:27:57.000000 python-aap-0.0.7/src/python_aap.egg-info/top_level.txt
+drwxrwxr-x   0 gitlab-runner   (991) gitlab-runner   (985)        0 2023-08-01 11:38:26.047817 python-aap-0.0.8/
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)     2735 2023-07-28 10:53:51.000000 python-aap-0.0.8/.gitignore
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)     1963 2023-07-28 12:41:45.000000 python-aap-0.0.8/.gitlab-ci.yml
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)    18020 2023-07-25 17:28:11.000000 python-aap-0.0.8/LICENSE
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)     5374 2023-08-01 11:38:26.046817 python-aap-0.0.8/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)     4781 2023-08-01 11:37:59.000000 python-aap-0.0.8/README.md
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)      817 2023-08-01 11:37:59.000000 python-aap-0.0.8/pyproject.toml
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)       17 2023-07-28 10:53:51.000000 python-aap-0.0.8/requirements.txt
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)       38 2023-08-01 11:38:26.047817 python-aap-0.0.8/setup.cfg
+drwxrwxr-x   0 gitlab-runner   (991) gitlab-runner   (985)        0 2023-08-01 11:38:26.040817 python-aap-0.0.8/src/
+drwxrwxr-x   0 gitlab-runner   (991) gitlab-runner   (985)        0 2023-08-01 11:38:26.045817 python-aap-0.0.8/src/aap/
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)      265 2023-07-28 10:53:51.000000 python-aap-0.0.8/src/aap/__init__.py
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)     4037 2023-08-01 11:37:59.000000 python-aap-0.0.8/src/aap/__main__.py
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)     5364 2023-07-28 12:08:32.000000 python-aap-0.0.8/src/aap/base.py
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)     3090 2023-07-28 12:08:32.000000 python-aap-0.0.8/src/aap/endpoints.py
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)     1901 2023-07-28 12:08:32.000000 python-aap-0.0.8/src/aap/mixins.py
+drwxrwxr-x   0 gitlab-runner   (991) gitlab-runner   (985)        0 2023-08-01 11:38:26.046817 python-aap-0.0.8/src/python_aap.egg-info/
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)     5374 2023-08-01 11:38:26.000000 python-aap-0.0.8/src/python_aap.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)      400 2023-08-01 11:38:26.000000 python-aap-0.0.8/src/python_aap.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)        1 2023-08-01 11:38:26.000000 python-aap-0.0.8/src/python_aap.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)       40 2023-08-01 11:38:26.000000 python-aap-0.0.8/src/python_aap.egg-info/entry_points.txt
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)       18 2023-08-01 11:38:26.000000 python-aap-0.0.8/src/python_aap.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)        4 2023-08-01 11:38:26.000000 python-aap-0.0.8/src/python_aap.egg-info/top_level.txt
```

### Comparing `python-aap-0.0.7/.gitignore` & `python-aap-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `python-aap-0.0.7/.gitlab-ci.yml` & `python-aap-0.0.8/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `python-aap-0.0.7/LICENSE` & `python-aap-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `python-aap-0.0.7/PKG-INFO` & `python-aap-0.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,12 @@
-Metadata-Version: 2.1
-Name: python-aap
-Version: 0.0.7
-Summary: Unofficial python wrapper over Ansible Automation Platform REST API
-Author-email: Ivan Mitruk <imitruk@redhat.com>
-Project-URL: Homepage, https://gitlab.corp.redhat.com/network/python-aap/
-Project-URL: Bug Tracker, https://gitlab.corp.redhat.com/network/python-aap/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Ansible Automation Platform Python Module
 
 This is unofficial wrapper for Ansible Automation Platform (AAP) API.
 
-To see an example how this module can be used please view [__main__.py](./src/aap/__main__.py)
+To see an example how this module can be used please view [\_\_main\_\_.py](https://gitlab.corp.redhat.com/network/python-aap/-/blob/main/src/aap/__main__.py)
 
 ## Executing jobs from CLI
 
 Python module can be invoked directly to execute job in aap and report status to terminal. AAP Credentials need to be specified either via CLI arguments or env variables
```

### Comparing `python-aap-0.0.7/README.md` & `python-aap-0.0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,26 @@
+Metadata-Version: 2.1
+Name: python-aap
+Version: 0.0.8
+Summary: Unofficial python wrapper over Ansible Automation Platform REST API
+Author-email: Ivan Mitruk <imitruk@redhat.com>
+Project-URL: Homepage, https://gitlab.corp.redhat.com/network/python-aap/
+Project-URL: Bug Tracker, https://gitlab.corp.redhat.com/network/python-aap/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Ansible Automation Platform Python Module
 
 This is unofficial wrapper for Ansible Automation Platform (AAP) API.
 
-To see an example how this module can be used please view [__main__.py](./src/aap/__main__.py)
+To see an example how this module can be used please view [\_\_main\_\_.py](https://gitlab.corp.redhat.com/network/python-aap/-/blob/main/src/aap/__main__.py)
 
 ## Executing jobs from CLI
 
 Python module can be invoked directly to execute job in aap and report status to terminal. AAP Credentials need to be specified either via CLI arguments or env variables
```

### Comparing `python-aap-0.0.7/pyproject.toml` & `python-aap-0.0.8/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "python-aap"
-version = "0.0.7"
+version = "0.0.8"
 dependencies = [
   'requests',
   'datetime'
 ]
 authors = [
   { name="Ivan Mitruk", email="imitruk@redhat.com" },
 ]
```

### Comparing `python-aap-0.0.7/src/aap/__main__.py` & `python-aap-0.0.8/src/aap/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     parser.add_argument('-l', '--limit', dest="limit", action="store",
                         default=[], help="Limit as comma separated list")
     parser.add_argument('-e', '--extra-vars', dest="extra", action="store",
                         default={}, help="json formatted extra variables")
     parser.add_argument('-r', '--retries', dest="retries", action="store",
                         type=int, default=3, help="Number of retries on API error")
     parser.add_argument('-t', '--poll-timeout', dest="timeout", action="store",
-                        type=int, default=1, help="Number of seconds between 2 polling requests to aap")
+                        type=int, default=5, help="Number of seconds between 2 polling requests to aap")
     parser.add_argument('--ignore-fail', dest="ingore_fail", action="store_true",
                         default=False, help="Program will return successfull even if job fails")
 
     args = parser.parse_args()
 
     if not args.username or not args.password or not args.url:
         print("Please provide AAP URL and credentials,"
```

### Comparing `python-aap-0.0.7/src/aap/base.py` & `python-aap-0.0.8/src/aap/base.py`

 * *Files identical despite different names*

### Comparing `python-aap-0.0.7/src/aap/endpoints.py` & `python-aap-0.0.8/src/aap/endpoints.py`

 * *Files identical despite different names*

### Comparing `python-aap-0.0.7/src/aap/mixins.py` & `python-aap-0.0.8/src/aap/mixins.py`

 * *Files identical despite different names*

### Comparing `python-aap-0.0.7/src/python_aap.egg-info/PKG-INFO` & `python-aap-0.0.8/src/python_aap.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-aap
-Version: 0.0.7
+Version: 0.0.8
 Summary: Unofficial python wrapper over Ansible Automation Platform REST API
 Author-email: Ivan Mitruk <imitruk@redhat.com>
 Project-URL: Homepage, https://gitlab.corp.redhat.com/network/python-aap/
 Project-URL: Bug Tracker, https://gitlab.corp.redhat.com/network/python-aap/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Ansible Automation Platform Python Module
 
 This is unofficial wrapper for Ansible Automation Platform (AAP) API.
 
-To see an example how this module can be used please view [__main__.py](./src/aap/__main__.py)
+To see an example how this module can be used please view [\_\_main\_\_.py](https://gitlab.corp.redhat.com/network/python-aap/-/blob/main/src/aap/__main__.py)
 
 ## Executing jobs from CLI
 
 Python module can be invoked directly to execute job in aap and report status to terminal. AAP Credentials need to be specified either via CLI arguments or env variables
```

