# Comparing `tmp/terragrunt-generator-0.6.4.tar.gz` & `tmp/terragrunt-generator-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terragrunt-generator-0.6.4.tar", last modified: Tue Aug  1 20:11:26 2023, max compression
+gzip compressed data, was "terragrunt-generator-0.6.5.tar", last modified: Tue Aug  1 20:25:50 2023, max compression
```

## Comparing `terragrunt-generator-0.6.4.tar` & `terragrunt-generator-0.6.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:11:26.887263 terragrunt-generator-0.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-01 20:11:06.000000 terragrunt-generator-0.6.4/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)    21166 2023-08-01 20:11:26.887263 terragrunt-generator-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-08-01 20:11:06.000000 terragrunt-generator-0.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:11:26.887263 terragrunt-generator-0.6.4/generator/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-01 20:11:16.000000 terragrunt-generator-0.6.4/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-01 20:11:06.000000 terragrunt-generator-0.6.4/generator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-08-01 20:11:06.000000 terragrunt-generator-0.6.4/generator/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-01 20:11:06.000000 terragrunt-generator-0.6.4/generator/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-01 20:11:06.000000 terragrunt-generator-0.6.4/generator/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-01 20:11:06.000000 terragrunt-generator-0.6.4/generator/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-01 20:11:06.000000 terragrunt-generator-0.6.4/generator/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-01 20:11:16.000000 terragrunt-generator-0.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 20:11:26.887263 terragrunt-generator-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-01 20:11:06.000000 terragrunt-generator-0.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:11:26.887263 terragrunt-generator-0.6.4/terragrunt_generator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21166 2023-08-01 20:11:26.000000 terragrunt-generator-0.6.4/terragrunt_generator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-08-01 20:11:26.000000 terragrunt-generator-0.6.4/terragrunt_generator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:11:26.000000 terragrunt-generator-0.6.4/terragrunt_generator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 20:11:26.000000 terragrunt-generator-0.6.4/terragrunt_generator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-01 20:11:26.000000 terragrunt-generator-0.6.4/terragrunt_generator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 20:11:26.000000 terragrunt-generator-0.6.4/terragrunt_generator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:11:26.887263 terragrunt-generator-0.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:11:06.000000 terragrunt-generator-0.6.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-08-01 20:11:06.000000 terragrunt-generator-0.6.4/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-01 20:11:06.000000 terragrunt-generator-0.6.4/tests/test_git.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-08-01 20:11:06.000000 terragrunt-generator-0.6.4/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-01 20:11:06.000000 terragrunt-generator-0.6.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:25:50.156776 terragrunt-generator-0.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-01 20:25:27.000000 terragrunt-generator-0.6.5/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)    21326 2023-08-01 20:25:50.156776 terragrunt-generator-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21075 2023-08-01 20:25:27.000000 terragrunt-generator-0.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:25:50.156776 terragrunt-generator-0.6.5/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-01 20:25:38.000000 terragrunt-generator-0.6.5/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-01 20:25:27.000000 terragrunt-generator-0.6.5/generator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-08-01 20:25:27.000000 terragrunt-generator-0.6.5/generator/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-01 20:25:27.000000 terragrunt-generator-0.6.5/generator/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-01 20:25:27.000000 terragrunt-generator-0.6.5/generator/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-01 20:25:27.000000 terragrunt-generator-0.6.5/generator/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-01 20:25:27.000000 terragrunt-generator-0.6.5/generator/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-01 20:25:38.000000 terragrunt-generator-0.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 20:25:50.156776 terragrunt-generator-0.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-01 20:25:27.000000 terragrunt-generator-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:25:50.156776 terragrunt-generator-0.6.5/terragrunt_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21326 2023-08-01 20:25:50.000000 terragrunt-generator-0.6.5/terragrunt_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-08-01 20:25:50.000000 terragrunt-generator-0.6.5/terragrunt_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:25:50.000000 terragrunt-generator-0.6.5/terragrunt_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 20:25:50.000000 terragrunt-generator-0.6.5/terragrunt_generator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-01 20:25:50.000000 terragrunt-generator-0.6.5/terragrunt_generator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 20:25:50.000000 terragrunt-generator-0.6.5/terragrunt_generator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:25:50.156776 terragrunt-generator-0.6.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:25:27.000000 terragrunt-generator-0.6.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-08-01 20:25:27.000000 terragrunt-generator-0.6.5/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-01 20:25:27.000000 terragrunt-generator-0.6.5/tests/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-08-01 20:25:27.000000 terragrunt-generator-0.6.5/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-01 20:25:27.000000 terragrunt-generator-0.6.5/tests/test_utils.py
```

### Comparing `terragrunt-generator-0.6.4/COPYING` & `terragrunt-generator-0.6.5/COPYING`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.6.4/PKG-INFO` & `terragrunt-generator-0.6.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terragrunt-generator
-Version: 0.6.4
+Version: 0.6.5
 Summary: generate terragrunt manifest from terraform module.
 Author: Chris
 Author-email: goabonga@pm.me
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: COPYING
 
@@ -290,25 +290,25 @@
     usage_bucket_prefix = lookup(local.all.project, "usage_bucket_prefix", "")
     # vpc_service_control_attach_enabled - Whether the project will be attached to a VPC Service Control Perimeter
     vpc_service_control_attach_enabled = lookup(local.all.project, "vpc_service_control_attach_enabled", false)
     # vpc_service_control_sleep_duration - The duration to sleep in seconds before adding the project to a shared VPC after the project is added to the VPC Service Control Perimeter. VPC-SC is eventually consistent.
     vpc_service_control_sleep_duration = lookup(local.all.project, "vpc_service_control_sleep_duration", "5s")
 },
   # budget_alert_pubsub_topic - The name of the Cloud Pub/Sub topic where budget related messages will be published, in the form of `projects/{project_id}/topics/{topic_id}`
-  (lookup(project, "budget_alert_pubsub_topic", null) == null ? {} : { budget_alert_pubsub_topic =  lookup(project, "budget_alert_pubsub_topic") }),
+  (lookup(local.all.project, "budget_alert_pubsub_topic", null) == null ? {} : { budget_alert_pubsub_topic =  lookup(local.all.project, "budget_alert_pubsub_topic") }),
   # budget_amount - The amount to use for a budget alert
-  (lookup(project, "budget_amount", null) == null ? {} : { budget_amount =  lookup(project, "budget_amount") }),
+  (lookup(local.all.project, "budget_amount", null) == null ? {} : { budget_amount =  lookup(local.all.project, "budget_amount") }),
   # budget_calendar_period - Specifies the calendar period for the budget. Possible values are MONTH, QUARTER, YEAR, CALENDAR_PERIOD_UNSPECIFIED, CUSTOM. custom_period_start_date and custom_period_end_date must be set if CUSTOM
-  (lookup(project, "budget_calendar_period", null) == null ? {} : { budget_calendar_period =  lookup(project, "budget_calendar_period") }),
+  (lookup(local.all.project, "budget_calendar_period", null) == null ? {} : { budget_calendar_period =  lookup(local.all.project, "budget_calendar_period") }),
   # budget_custom_period_end_date - Specifies the end date (DD-MM-YYYY) for the calendar_period CUSTOM
-  (lookup(project, "budget_custom_period_end_date", null) == null ? {} : { budget_custom_period_end_date =  lookup(project, "budget_custom_period_end_date") }),
+  (lookup(local.all.project, "budget_custom_period_end_date", null) == null ? {} : { budget_custom_period_end_date =  lookup(local.all.project, "budget_custom_period_end_date") }),
   # budget_custom_period_start_date - Specifies the start date (DD-MM-YYYY) for the calendar_period CUSTOM
-  (lookup(project, "budget_custom_period_start_date", null) == null ? {} : { budget_custom_period_start_date =  lookup(project, "budget_custom_period_start_date") }),
+  (lookup(local.all.project, "budget_custom_period_start_date", null) == null ? {} : { budget_custom_period_start_date =  lookup(local.all.project, "budget_custom_period_start_date") }),
   # budget_display_name - The display name of the budget. If not set defaults to `Budget For <projects[0]|All Projects>`
-  (lookup(project, "budget_display_name", null) == null ? {} : { budget_display_name =  lookup(project, "budget_display_name") }),
+  (lookup(local.all.project, "budget_display_name", null) == null ? {} : { budget_display_name =  lookup(local.all.project, "budget_display_name") }),
   # random_project_id_length - Sets the length of `random_project_id` to the provided length, and uses a `random_string` for a larger collusion domain.  Recommended for use with CI.
-  (lookup(project, "random_project_id_length", null) == null ? {} : { random_project_id_length =  lookup(project, "random_project_id_length") }),
+  (lookup(local.all.project, "random_project_id_length", null) == null ? {} : { random_project_id_length =  lookup(local.all.project, "random_project_id_length") }),
   # vpc_service_control_perimeter_name - The name of a VPC Service Control Perimeter to add the created project to
-  (lookup(project, "vpc_service_control_perimeter_name", null) == null ? {} : { vpc_service_control_perimeter_name =  lookup(project, "vpc_service_control_perimeter_name") })
+  (lookup(local.all.project, "vpc_service_control_perimeter_name", null) == null ? {} : { vpc_service_control_perimeter_name =  lookup(local.all.project, "vpc_service_control_perimeter_name") })
 )
 
 ```
```

### Comparing `terragrunt-generator-0.6.4/README.md` & `terragrunt-generator-0.6.5/terragrunt_generator.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: terragrunt-generator
+Version: 0.6.5
+Summary: generate terragrunt manifest from terraform module.
+Author: Chris
+Author-email: goabonga@pm.me
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: COPYING
+
 # terragrunt-generator
 
 **terragrunt-generator** provide a way to generate a ```terragrunt.hcl``` file with documented inputs who's coming from variables exposed by terraform module.
 
 The result is easily configurable with a **yaml** file.
 ## Requirements
 
@@ -280,25 +290,25 @@
     usage_bucket_prefix = lookup(local.all.project, "usage_bucket_prefix", "")
     # vpc_service_control_attach_enabled - Whether the project will be attached to a VPC Service Control Perimeter
     vpc_service_control_attach_enabled = lookup(local.all.project, "vpc_service_control_attach_enabled", false)
     # vpc_service_control_sleep_duration - The duration to sleep in seconds before adding the project to a shared VPC after the project is added to the VPC Service Control Perimeter. VPC-SC is eventually consistent.
     vpc_service_control_sleep_duration = lookup(local.all.project, "vpc_service_control_sleep_duration", "5s")
 },
   # budget_alert_pubsub_topic - The name of the Cloud Pub/Sub topic where budget related messages will be published, in the form of `projects/{project_id}/topics/{topic_id}`
-  (lookup(project, "budget_alert_pubsub_topic", null) == null ? {} : { budget_alert_pubsub_topic =  lookup(project, "budget_alert_pubsub_topic") }),
+  (lookup(local.all.project, "budget_alert_pubsub_topic", null) == null ? {} : { budget_alert_pubsub_topic =  lookup(local.all.project, "budget_alert_pubsub_topic") }),
   # budget_amount - The amount to use for a budget alert
-  (lookup(project, "budget_amount", null) == null ? {} : { budget_amount =  lookup(project, "budget_amount") }),
+  (lookup(local.all.project, "budget_amount", null) == null ? {} : { budget_amount =  lookup(local.all.project, "budget_amount") }),
   # budget_calendar_period - Specifies the calendar period for the budget. Possible values are MONTH, QUARTER, YEAR, CALENDAR_PERIOD_UNSPECIFIED, CUSTOM. custom_period_start_date and custom_period_end_date must be set if CUSTOM
-  (lookup(project, "budget_calendar_period", null) == null ? {} : { budget_calendar_period =  lookup(project, "budget_calendar_period") }),
+  (lookup(local.all.project, "budget_calendar_period", null) == null ? {} : { budget_calendar_period =  lookup(local.all.project, "budget_calendar_period") }),
   # budget_custom_period_end_date - Specifies the end date (DD-MM-YYYY) for the calendar_period CUSTOM
-  (lookup(project, "budget_custom_period_end_date", null) == null ? {} : { budget_custom_period_end_date =  lookup(project, "budget_custom_period_end_date") }),
+  (lookup(local.all.project, "budget_custom_period_end_date", null) == null ? {} : { budget_custom_period_end_date =  lookup(local.all.project, "budget_custom_period_end_date") }),
   # budget_custom_period_start_date - Specifies the start date (DD-MM-YYYY) for the calendar_period CUSTOM
-  (lookup(project, "budget_custom_period_start_date", null) == null ? {} : { budget_custom_period_start_date =  lookup(project, "budget_custom_period_start_date") }),
+  (lookup(local.all.project, "budget_custom_period_start_date", null) == null ? {} : { budget_custom_period_start_date =  lookup(local.all.project, "budget_custom_period_start_date") }),
   # budget_display_name - The display name of the budget. If not set defaults to `Budget For <projects[0]|All Projects>`
-  (lookup(project, "budget_display_name", null) == null ? {} : { budget_display_name =  lookup(project, "budget_display_name") }),
+  (lookup(local.all.project, "budget_display_name", null) == null ? {} : { budget_display_name =  lookup(local.all.project, "budget_display_name") }),
   # random_project_id_length - Sets the length of `random_project_id` to the provided length, and uses a `random_string` for a larger collusion domain.  Recommended for use with CI.
-  (lookup(project, "random_project_id_length", null) == null ? {} : { random_project_id_length =  lookup(project, "random_project_id_length") }),
+  (lookup(local.all.project, "random_project_id_length", null) == null ? {} : { random_project_id_length =  lookup(local.all.project, "random_project_id_length") }),
   # vpc_service_control_perimeter_name - The name of a VPC Service Control Perimeter to add the created project to
-  (lookup(project, "vpc_service_control_perimeter_name", null) == null ? {} : { vpc_service_control_perimeter_name =  lookup(project, "vpc_service_control_perimeter_name") })
+  (lookup(local.all.project, "vpc_service_control_perimeter_name", null) == null ? {} : { vpc_service_control_perimeter_name =  lookup(local.all.project, "vpc_service_control_perimeter_name") })
 )
 
 ```
```

### Comparing `terragrunt-generator-0.6.4/generator/generate.py` & `terragrunt-generator-0.6.5/generator/generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,17 +128,17 @@
             if variable.get('mandatory', False) is True:
                 content_fisrt += _content
             else:
                 content_next += _content
         else:
             name = variable.get('name')
             content_nullable += f'\n  # {name} - {description}'
-            content_nullable += f'\n  (lookup({lookup}, "{name}", null)'
+            content_nullable += f'\n  (lookup(local.all.{lookup}, "{name}", null)'
             content_nullable += ' == null ? {} : '
-            content_nullable += f'{{ {name} =  lookup({lookup}, "{name}") }}'
+            content_nullable += f'{{ {name} =  lookup(local.all.{lookup}, "{name}") }}'
             content_nullable += '),'
 
     if content_nullable != '':
         return f"""
 inputs = merge({{
 {content_fisrt}{content_next.rstrip(content_next[-1])}
 }},{content_nullable.rstrip(content_nullable[-1])}
```

### Comparing `terragrunt-generator-0.6.4/generator/main.py` & `terragrunt-generator-0.6.5/generator/main.py`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.6.4/pyproject.toml` & `terragrunt-generator-0.6.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,13 +19,13 @@
   | build
   | dist
 )/
 '''
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.6.4"
+version = "0.6.5"
 tag_format = "$major.$minor.$patch$prerelease"
 version_files = [
     "pyproject.toml:version",
     "generator/__init__.py",
 ]
```

### Comparing `terragrunt-generator-0.6.4/setup.py` & `terragrunt-generator-0.6.5/setup.py`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.6.4/terragrunt_generator.egg-info/PKG-INFO` & `terragrunt-generator-0.6.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: terragrunt-generator
-Version: 0.6.4
-Summary: generate terragrunt manifest from terraform module.
-Author: Chris
-Author-email: goabonga@pm.me
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: COPYING
-
 # terragrunt-generator
 
 **terragrunt-generator** provide a way to generate a ```terragrunt.hcl``` file with documented inputs who's coming from variables exposed by terraform module.
 
 The result is easily configurable with a **yaml** file.
 ## Requirements
 
@@ -290,25 +280,25 @@
     usage_bucket_prefix = lookup(local.all.project, "usage_bucket_prefix", "")
     # vpc_service_control_attach_enabled - Whether the project will be attached to a VPC Service Control Perimeter
     vpc_service_control_attach_enabled = lookup(local.all.project, "vpc_service_control_attach_enabled", false)
     # vpc_service_control_sleep_duration - The duration to sleep in seconds before adding the project to a shared VPC after the project is added to the VPC Service Control Perimeter. VPC-SC is eventually consistent.
     vpc_service_control_sleep_duration = lookup(local.all.project, "vpc_service_control_sleep_duration", "5s")
 },
   # budget_alert_pubsub_topic - The name of the Cloud Pub/Sub topic where budget related messages will be published, in the form of `projects/{project_id}/topics/{topic_id}`
-  (lookup(project, "budget_alert_pubsub_topic", null) == null ? {} : { budget_alert_pubsub_topic =  lookup(project, "budget_alert_pubsub_topic") }),
+  (lookup(local.all.project, "budget_alert_pubsub_topic", null) == null ? {} : { budget_alert_pubsub_topic =  lookup(local.all.project, "budget_alert_pubsub_topic") }),
   # budget_amount - The amount to use for a budget alert
-  (lookup(project, "budget_amount", null) == null ? {} : { budget_amount =  lookup(project, "budget_amount") }),
+  (lookup(local.all.project, "budget_amount", null) == null ? {} : { budget_amount =  lookup(local.all.project, "budget_amount") }),
   # budget_calendar_period - Specifies the calendar period for the budget. Possible values are MONTH, QUARTER, YEAR, CALENDAR_PERIOD_UNSPECIFIED, CUSTOM. custom_period_start_date and custom_period_end_date must be set if CUSTOM
-  (lookup(project, "budget_calendar_period", null) == null ? {} : { budget_calendar_period =  lookup(project, "budget_calendar_period") }),
+  (lookup(local.all.project, "budget_calendar_period", null) == null ? {} : { budget_calendar_period =  lookup(local.all.project, "budget_calendar_period") }),
   # budget_custom_period_end_date - Specifies the end date (DD-MM-YYYY) for the calendar_period CUSTOM
-  (lookup(project, "budget_custom_period_end_date", null) == null ? {} : { budget_custom_period_end_date =  lookup(project, "budget_custom_period_end_date") }),
+  (lookup(local.all.project, "budget_custom_period_end_date", null) == null ? {} : { budget_custom_period_end_date =  lookup(local.all.project, "budget_custom_period_end_date") }),
   # budget_custom_period_start_date - Specifies the start date (DD-MM-YYYY) for the calendar_period CUSTOM
-  (lookup(project, "budget_custom_period_start_date", null) == null ? {} : { budget_custom_period_start_date =  lookup(project, "budget_custom_period_start_date") }),
+  (lookup(local.all.project, "budget_custom_period_start_date", null) == null ? {} : { budget_custom_period_start_date =  lookup(local.all.project, "budget_custom_period_start_date") }),
   # budget_display_name - The display name of the budget. If not set defaults to `Budget For <projects[0]|All Projects>`
-  (lookup(project, "budget_display_name", null) == null ? {} : { budget_display_name =  lookup(project, "budget_display_name") }),
+  (lookup(local.all.project, "budget_display_name", null) == null ? {} : { budget_display_name =  lookup(local.all.project, "budget_display_name") }),
   # random_project_id_length - Sets the length of `random_project_id` to the provided length, and uses a `random_string` for a larger collusion domain.  Recommended for use with CI.
-  (lookup(project, "random_project_id_length", null) == null ? {} : { random_project_id_length =  lookup(project, "random_project_id_length") }),
+  (lookup(local.all.project, "random_project_id_length", null) == null ? {} : { random_project_id_length =  lookup(local.all.project, "random_project_id_length") }),
   # vpc_service_control_perimeter_name - The name of a VPC Service Control Perimeter to add the created project to
-  (lookup(project, "vpc_service_control_perimeter_name", null) == null ? {} : { vpc_service_control_perimeter_name =  lookup(project, "vpc_service_control_perimeter_name") })
+  (lookup(local.all.project, "vpc_service_control_perimeter_name", null) == null ? {} : { vpc_service_control_perimeter_name =  lookup(local.all.project, "vpc_service_control_perimeter_name") })
 )
 
 ```
```

### Comparing `terragrunt-generator-0.6.4/terragrunt_generator.egg-info/SOURCES.txt` & `terragrunt-generator-0.6.5/terragrunt_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.6.4/tests/test_generate.py` & `terragrunt-generator-0.6.5/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.6.4/tests/test_reader.py` & `terragrunt-generator-0.6.5/tests/test_reader.py`

 * *Files identical despite different names*

