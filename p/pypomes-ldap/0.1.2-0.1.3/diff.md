# Comparing `tmp/pypomes_ldap-0.1.2.tar.gz` & `tmp/pypomes_ldap-0.1.3.tar.gz`

## Comparing `pypomes_ldap-0.1.2.tar` & `pypomes_ldap-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.2/src/pypomes_ldap/__init__.py
--rw-r--r--   0        0        0    14106 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.2/src/pypomes_ldap/ldap_pomes.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.2/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.2/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.2/README.md
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0  1418839 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.3/python_ldap-3.4.0-cp310-cp310-win_amd64.whl
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.3/src/pypomes_ldap/__init__.py
+-rw-r--r--   0        0        0    18287 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.3/src/pypomes_ldap/ldap_pomes.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.3/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.3/README.md
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.3/PKG-INFO
```

### Comparing `pypomes_ldap-0.1.2/src/pypomes_ldap/__init__.py` & `pypomes_ldap-0.1.3/src/pypomes_ldap/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,9 +11,9 @@
     LDAP_BASE_DN, LDAP_BIND_DN, LDAP_BIND_PWD,
     LDAP_SERVER_URI, LDAP_TIMEOUT, LDAP_TRACE_FILE, LDAP_TRACE_LEVEL,
     ldap_init, ldap_bind, ldap_unbind, ldap_add_entry, ldap_search, ldap_delete_entry,
     ldap_add_value, ldap_set_value, ldap_get_value, ldap_get_value_list, ldap_get_values,
     ldap_get_values_lists, ldap_change_pwd, ldap_modify_user, ldap_modify_entry,
 ]
 
-__version__ = "0.1.2"
-__version_info__ = (0, 1, 2)
+__version__ = "0.1.3"
+__version_info__ = (0, 1, 3)
```

### Comparing `pypomes_ldap-0.1.2/LICENSE` & `pypomes_ldap-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_ldap-0.1.2/pyproject.toml` & `pypomes_ldap-0.1.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_ldap"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (LDAP module)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "pip>=23.1.2",
-    "pypomes_core>=0.1.2",
+    "pypomes_core>=0.2.1",
     "python-ldap>=3.4.0",
     "setuptools>=68.0.0",
-    "wheel>=0.40.0"
+    "wheel>=0.41.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-LDAP"
 "Bug Tracker" = "https://github.com/TheWiseCoder/PyPomes-LDAP/issues"
```

### Comparing `pypomes_ldap-0.1.2/PKG-INFO` & `pypomes_ldap-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pypomes_ldap
-Version: 0.1.2
+Version: 0.1.3
 Summary: A collection of Python pomes, pennyeach (LDAP module)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-LDAP
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-LDAP/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: pip>=23.1.2
-Requires-Dist: pypomes-core>=0.1.2
+Requires-Dist: pypomes-core>=0.2.1
 Requires-Dist: python-ldap>=3.4.0
 Requires-Dist: setuptools>=68.0.0
-Requires-Dist: wheel>=0.40.0
+Requires-Dist: wheel>=0.41.0
```

