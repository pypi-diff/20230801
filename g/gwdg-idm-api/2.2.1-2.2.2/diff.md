# Comparing `tmp/gwdg_idm_api-2.2.1.tar.gz` & `tmp/gwdg_idm_api-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwdg_idm_api-2.2.1.tar", last modified: Thu Jul 20 16:45:03 2023, max compression
+gzip compressed data, was "gwdg_idm_api-2.2.2.tar", last modified: Tue Aug  1 09:45:45 2023, max compression
```

## Comparing `gwdg_idm_api-2.2.1.tar` & `gwdg_idm_api-2.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:45:03.391746 gwdg_idm_api-2.2.1/
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      279 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1120 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1085 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      685 2023-07-20 16:45:03.391746 gwdg_idm_api-2.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      196 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      915 2023-07-20 16:45:03.391746 gwdg_idm_api-2.2.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:45:03.387746 gwdg_idm_api-2.2.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:45:03.391746 gwdg_idm_api-2.2.1/src/gwdg_idm_api/
--rw-rw-rw-   0 root         (0) root         (0)      132 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.1/src/gwdg_idm_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-07-20 16:45:03.000000 gwdg_idm_api-2.2.1/src/gwdg_idm_api/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     5096 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.1/src/gwdg_idm_api/benutzerverwaltung.py
--rw-rw-rw-   0 root         (0) root         (0)     6803 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.1/src/gwdg_idm_api/models.py
--rw-rw-rw-   0 root         (0) root         (0)     6878 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.1/src/gwdg_idm_api/string_cleaner.py
--rw-rw-rw-   0 root         (0) root         (0)     1399 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.1/src/gwdg_idm_api/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:45:03.391746 gwdg_idm_api-2.2.1/src/gwdg_idm_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)      685 2023-07-20 16:45:03.000000 gwdg_idm_api-2.2.1/src/gwdg_idm_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      566 2023-07-20 16:45:03.000000 gwdg_idm_api-2.2.1/src/gwdg_idm_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 16:45:03.000000 gwdg_idm_api-2.2.1/src/gwdg_idm_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 16:45:03.000000 gwdg_idm_api-2.2.1/src/gwdg_idm_api.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       50 2023-07-20 16:45:03.000000 gwdg_idm_api-2.2.1/src/gwdg_idm_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-20 16:45:03.000000 gwdg_idm_api-2.2.1/src/gwdg_idm_api.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:45:03.391746 gwdg_idm_api-2.2.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3302 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.1/tests/examples.py
--rw-rw-rw-   0 root         (0) root         (0)      891 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.1/tests/predict_username.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.1/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:45:45.565526 gwdg_idm_api-2.2.2/
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-08-01 09:45:28.000000 gwdg_idm_api-2.2.2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      279 2023-08-01 09:45:28.000000 gwdg_idm_api-2.2.2/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1120 2023-08-01 09:45:28.000000 gwdg_idm_api-2.2.2/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-08-01 09:45:28.000000 gwdg_idm_api-2.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      685 2023-08-01 09:45:45.565526 gwdg_idm_api-2.2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-08-01 09:45:28.000000 gwdg_idm_api-2.2.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      196 2023-08-01 09:45:28.000000 gwdg_idm_api-2.2.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      915 2023-08-01 09:45:45.569526 gwdg_idm_api-2.2.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:45:45.561526 gwdg_idm_api-2.2.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:45:45.565526 gwdg_idm_api-2.2.2/src/gwdg_idm_api/
+-rw-rw-rw-   0 root         (0) root         (0)      132 2023-08-01 09:45:28.000000 gwdg_idm_api-2.2.2/src/gwdg_idm_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-08-01 09:45:45.000000 gwdg_idm_api-2.2.2/src/gwdg_idm_api/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     5096 2023-08-01 09:45:28.000000 gwdg_idm_api-2.2.2/src/gwdg_idm_api/benutzerverwaltung.py
+-rw-rw-rw-   0 root         (0) root         (0)     6930 2023-08-01 09:45:28.000000 gwdg_idm_api-2.2.2/src/gwdg_idm_api/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     6878 2023-08-01 09:45:28.000000 gwdg_idm_api-2.2.2/src/gwdg_idm_api/string_cleaner.py
+-rw-rw-rw-   0 root         (0) root         (0)     1399 2023-08-01 09:45:28.000000 gwdg_idm_api-2.2.2/src/gwdg_idm_api/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:45:45.565526 gwdg_idm_api-2.2.2/src/gwdg_idm_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      685 2023-08-01 09:45:45.000000 gwdg_idm_api-2.2.2/src/gwdg_idm_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      566 2023-08-01 09:45:45.000000 gwdg_idm_api-2.2.2/src/gwdg_idm_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 09:45:45.000000 gwdg_idm_api-2.2.2/src/gwdg_idm_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 09:45:45.000000 gwdg_idm_api-2.2.2/src/gwdg_idm_api.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       50 2023-08-01 09:45:45.000000 gwdg_idm_api-2.2.2/src/gwdg_idm_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 09:45:45.000000 gwdg_idm_api-2.2.2/src/gwdg_idm_api.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:45:45.565526 gwdg_idm_api-2.2.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3617 2023-08-01 09:45:28.000000 gwdg_idm_api-2.2.2/tests/examples.py
+-rw-rw-rw-   0 root         (0) root         (0)      891 2023-08-01 09:45:28.000000 gwdg_idm_api-2.2.2/tests/predict_username.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-08-01 09:45:28.000000 gwdg_idm_api-2.2.2/tox.ini
```

### Comparing `gwdg_idm_api-2.2.1/.pre-commit-config.yaml` & `gwdg_idm_api-2.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.2.1/LICENSE` & `gwdg_idm_api-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.2.1/PKG-INFO` & `gwdg_idm_api-2.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdg_idm_api
-Version: 2.2.1
+Version: 2.2.2
 Summary: Interface to the GWDG IDM api
 Home-page: https://gitlab.gwdg.de/mpi-dortmund/ze-edv-public/gwdg_idm_api
 Author: Markus Stabrin
 Author-email: markus.stabrin@mpi-dortmund.mpg.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gwdg_idm_api-2.2.1/setup.cfg` & `gwdg_idm_api-2.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.2.1/src/gwdg_idm_api/benutzerverwaltung.py` & `gwdg_idm_api-2.2.2/src/gwdg_idm_api/benutzerverwaltung.py`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.2.1/src/gwdg_idm_api/models.py` & `gwdg_idm_api-2.2.2/src/gwdg_idm_api/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,14 +55,19 @@
 
 class ChangeTemplate(pydantic.BaseModel):
     id: str
     goesternExpirationDate: str = None
     isScheduledForDeletion: str = None
     goesternUserStatus: str = None
 
+    @pydantic.validator("isScheduledForDeletion")
+    @classmethod
+    def to_upper(cls, value):
+        return value.upper()
+
     @staticmethod
     def update_json(name: str, value: str | list[str] | None) -> str:
         if value is not None:
             value = [value] if not isinstance(value, list) else value
         else:
             value = []
         data = {
```

### Comparing `gwdg_idm_api-2.2.1/src/gwdg_idm_api/string_cleaner.py` & `gwdg_idm_api-2.2.2/src/gwdg_idm_api/string_cleaner.py`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.2.1/src/gwdg_idm_api/util.py` & `gwdg_idm_api-2.2.2/src/gwdg_idm_api/util.py`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.2.1/src/gwdg_idm_api.egg-info/PKG-INFO` & `gwdg_idm_api-2.2.2/src/gwdg_idm_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdg-idm-api
-Version: 2.2.1
+Version: 2.2.2
 Summary: Interface to the GWDG IDM api
 Home-page: https://gitlab.gwdg.de/mpi-dortmund/ze-edv-public/gwdg_idm_api
 Author: Markus Stabrin
 Author-email: markus.stabrin@mpi-dortmund.mpg.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gwdg_idm_api-2.2.1/src/gwdg_idm_api.egg-info/SOURCES.txt` & `gwdg_idm_api-2.2.2/src/gwdg_idm_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.2.1/tests/examples.py` & `gwdg_idm_api-2.2.2/tests/examples.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import datetime
 import os
+import uuid
 
 from gwdg_idm_api.benutzerverwaltung import Benutzerverwaltung
 from gwdg_idm_api.models import BaseGWDGUser, CreateTemplate
 from gwdg_idm_api.util import AlreadyDeletedError, pretty_print
 
 
 # This are the values for our CreateTemplate for a new IDM user
@@ -20,17 +21,17 @@
     externalTaskCommand: str = "CreateMailbox"
 
 
 # This are the values for our MPIDoUser, we have some additional fields
 # for workGroup, dn, and externalTaskCommand
 # Adjust the fields to your template.
 class MPIDoUser(BaseGWDGUser):
-    workGroup: str
-    dn: str
-    externalTaskCommand: str
+    workGroup: str = None
+    dn: str = None
+    externalTaskCommand: str = None
 
 
 # Load idm credentials
 # Do not upload credentials in any way to github/gitlab etc.
 idm_username = os.environ["IDM_USERNAME"]
 idm_password = os.environ["IDM_PASSWORD"]
 
@@ -53,14 +54,24 @@
 print(pretty_print(sn_a_users[:2]))
 
 # Take the first user and print a more detailed view
 print("# Get detailed information")
 single_user = benutzerverwaltung.get_single_user(sn_a_users[0].id)
 print(pretty_print(single_user))
 
+single_user = benutzerverwaltung.create_user(
+    NewGWDGUser(
+        givenName=str(uuid.uuid4())[:8],
+        sn=str(uuid.uuid4())[:8],
+        workGroup="best_group",
+        departmentNumber="best_department",
+    )
+)
+print("# Create new user")
+print(pretty_print(single_user))
 
 # Change the lastname of the user to 'Upps bad lastnäme' and workGroup to '-'
 # and check if the update happened
 print("# Update user")
 updated_user = benutzerverwaltung.update_user(
     single_user, {"workGroup": "-", "sn": "Upps bad lastnäme"}
 )
```

### Comparing `gwdg_idm_api-2.2.1/tests/predict_username.py` & `gwdg_idm_api-2.2.2/tests/predict_username.py`

 * *Files identical despite different names*

