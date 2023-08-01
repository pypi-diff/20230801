# Comparing `tmp/cwtune-0.1.11.tar.gz` & `tmp/cwtune-0.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cwtune-0.1.11.tar", last modified: Tue Aug  1 11:34:18 2023, max compression
+gzip compressed data, was "cwtune-0.1.12.tar", last modified: Tue Aug  1 11:38:29 2023, max compression
```

## Comparing `cwtune-0.1.11.tar` & `cwtune-0.1.12.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-01 11:34:18.178901 cwtune-0.1.11/
--rw-r--r--   0 arran      (501) staff       (20)     1204 2023-07-25 11:17:40.000000 cwtune-0.1.11/.gitignore
--rw-r--r--   0 arran      (501) staff       (20)     1070 2023-07-25 11:24:31.000000 cwtune-0.1.11/LICENSE
--rw-r--r--   0 arran      (501) staff       (20)     1532 2023-08-01 11:34:18.179196 cwtune-0.1.11/PKG-INFO
--rw-r--r--   0 arran      (501) staff       (20)      860 2023-07-11 11:02:07.000000 cwtune-0.1.11/README.rst
-drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-01 11:34:18.153554 cwtune-0.1.11/cwtune/
--rw-r--r--   0 arran      (501) staff       (20)      123 2023-07-11 11:02:07.000000 cwtune-0.1.11/cwtune/__init__.py
--rw-r--r--   0 arran      (501) staff       (20)     5599 2023-07-25 10:25:39.000000 cwtune-0.1.11/cwtune/aws.py
--rw-r--r--   0 arran      (501) staff       (20)     1060 2023-07-25 15:12:24.000000 cwtune-0.1.11/cwtune/cli.py
--rw-r--r--   0 arran      (501) staff       (20)     9126 2023-07-25 15:12:09.000000 cwtune-0.1.11/cwtune/main.py
--rw-r--r--   0 arran      (501) staff       (20)     2400 2023-07-24 12:37:41.000000 cwtune-0.1.11/cwtune/timeseries.py
--rw-r--r--   0 arran      (501) staff       (20)     2760 2023-07-25 12:45:29.000000 cwtune-0.1.11/cwtune/utils.py
-drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-01 11:34:18.161755 cwtune-0.1.11/cwtune.egg-info/
--rw-r--r--   0 arran      (501) staff       (20)     1532 2023-08-01 11:34:17.000000 cwtune-0.1.11/cwtune.egg-info/PKG-INFO
--rw-r--r--   0 arran      (501) staff       (20)      562 2023-08-01 11:34:18.000000 cwtune-0.1.11/cwtune.egg-info/SOURCES.txt
--rw-r--r--   0 arran      (501) staff       (20)        1 2023-08-01 11:34:17.000000 cwtune-0.1.11/cwtune.egg-info/dependency_links.txt
--rw-r--r--   0 arran      (501) staff       (20)       43 2023-08-01 11:34:17.000000 cwtune-0.1.11/cwtune.egg-info/entry_points.txt
--rw-r--r--   0 arran      (501) staff       (20)        1 2023-08-01 11:29:13.000000 cwtune-0.1.11/cwtune.egg-info/not-zip-safe
--rw-r--r--   0 arran      (501) staff       (20)       65 2023-08-01 11:34:17.000000 cwtune-0.1.11/cwtune.egg-info/requires.txt
--rw-r--r--   0 arran      (501) staff       (20)        7 2023-08-01 11:34:17.000000 cwtune-0.1.11/cwtune.egg-info/top_level.txt
--rw-r--r--   0 arran      (501) staff       (20)       66 2023-07-25 12:31:11.000000 cwtune-0.1.11/requirements.txt
--rw-r--r--   0 arran      (501) staff       (20)      424 2023-08-01 11:34:18.183290 cwtune-0.1.11/setup.cfg
--rw-r--r--   0 arran      (501) staff       (20)     1338 2023-08-01 11:34:00.000000 cwtune-0.1.11/setup.py
-drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-01 11:34:18.164379 cwtune-0.1.11/tests/
--rw-r--r--   0 arran      (501) staff       (20)       36 2023-07-11 11:02:07.000000 cwtune-0.1.11/tests/__init__.py
-drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-01 11:34:18.174403 cwtune-0.1.11/tests/__pycache__/
--rw-r--r--   0 arran      (501) staff       (20)      208 2023-07-11 11:10:33.000000 cwtune-0.1.11/tests/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 arran      (501) staff       (20)     4029 2023-07-11 11:10:33.000000 cwtune-0.1.11/tests/__pycache__/test_cwtune.cpython-311-pytest-6.2.4.pyc
--rw-r--r--   0 arran      (501) staff       (20)     7071 2023-07-17 14:03:14.000000 cwtune-0.1.11/tests/__pycache__/test_cwtune.cpython-311.pyc
--rw-r--r--   0 arran      (501) staff       (20)     3754 2023-07-17 14:03:13.000000 cwtune-0.1.11/tests/test_cwtune.py
+drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-01 11:38:29.302383 cwtune-0.1.12/
+-rw-r--r--   0 arran      (501) staff       (20)     1204 2023-07-25 11:17:40.000000 cwtune-0.1.12/.gitignore
+-rw-r--r--   0 arran      (501) staff       (20)     1070 2023-07-25 11:24:31.000000 cwtune-0.1.12/LICENSE
+-rw-r--r--   0 arran      (501) staff       (20)     1532 2023-08-01 11:38:29.302726 cwtune-0.1.12/PKG-INFO
+-rw-r--r--   0 arran      (501) staff       (20)      860 2023-07-11 11:02:07.000000 cwtune-0.1.12/README.rst
+drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-01 11:38:29.278648 cwtune-0.1.12/cwtune/
+-rw-r--r--   0 arran      (501) staff       (20)      123 2023-07-11 11:02:07.000000 cwtune-0.1.12/cwtune/__init__.py
+-rw-r--r--   0 arran      (501) staff       (20)     9126 2023-07-25 15:12:09.000000 cwtune-0.1.12/cwtune/analyze.py
+-rw-r--r--   0 arran      (501) staff       (20)     5599 2023-07-25 10:25:39.000000 cwtune-0.1.12/cwtune/aws.py
+-rw-r--r--   0 arran      (501) staff       (20)     1065 2023-08-01 11:37:11.000000 cwtune-0.1.12/cwtune/cli.py
+-rw-r--r--   0 arran      (501) staff       (20)     2400 2023-07-24 12:37:41.000000 cwtune-0.1.12/cwtune/timeseries.py
+-rw-r--r--   0 arran      (501) staff       (20)     2760 2023-07-25 12:45:29.000000 cwtune-0.1.12/cwtune/utils.py
+drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-01 11:38:29.285986 cwtune-0.1.12/cwtune.egg-info/
+-rw-r--r--   0 arran      (501) staff       (20)     1532 2023-08-01 11:38:28.000000 cwtune-0.1.12/cwtune.egg-info/PKG-INFO
+-rw-r--r--   0 arran      (501) staff       (20)      565 2023-08-01 11:38:29.000000 cwtune-0.1.12/cwtune.egg-info/SOURCES.txt
+-rw-r--r--   0 arran      (501) staff       (20)        1 2023-08-01 11:38:28.000000 cwtune-0.1.12/cwtune.egg-info/dependency_links.txt
+-rw-r--r--   0 arran      (501) staff       (20)       43 2023-08-01 11:38:28.000000 cwtune-0.1.12/cwtune.egg-info/entry_points.txt
+-rw-r--r--   0 arran      (501) staff       (20)        1 2023-08-01 11:38:28.000000 cwtune-0.1.12/cwtune.egg-info/not-zip-safe
+-rw-r--r--   0 arran      (501) staff       (20)       65 2023-08-01 11:38:28.000000 cwtune-0.1.12/cwtune.egg-info/requires.txt
+-rw-r--r--   0 arran      (501) staff       (20)        7 2023-08-01 11:38:28.000000 cwtune-0.1.12/cwtune.egg-info/top_level.txt
+-rw-r--r--   0 arran      (501) staff       (20)       66 2023-07-25 12:31:11.000000 cwtune-0.1.12/requirements.txt
+-rw-r--r--   0 arran      (501) staff       (20)      424 2023-08-01 11:38:29.305114 cwtune-0.1.12/setup.cfg
+-rw-r--r--   0 arran      (501) staff       (20)     1338 2023-08-01 11:37:22.000000 cwtune-0.1.12/setup.py
+drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-01 11:38:29.292542 cwtune-0.1.12/tests/
+-rw-r--r--   0 arran      (501) staff       (20)       36 2023-07-11 11:02:07.000000 cwtune-0.1.12/tests/__init__.py
+drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-01 11:38:29.300148 cwtune-0.1.12/tests/__pycache__/
+-rw-r--r--   0 arran      (501) staff       (20)      208 2023-07-11 11:10:33.000000 cwtune-0.1.12/tests/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 arran      (501) staff       (20)     4029 2023-07-11 11:10:33.000000 cwtune-0.1.12/tests/__pycache__/test_cwtune.cpython-311-pytest-6.2.4.pyc
+-rw-r--r--   0 arran      (501) staff       (20)     7071 2023-07-17 14:03:14.000000 cwtune-0.1.12/tests/__pycache__/test_cwtune.cpython-311.pyc
+-rw-r--r--   0 arran      (501) staff       (20)     3754 2023-07-17 14:03:13.000000 cwtune-0.1.12/tests/test_cwtune.py
```

### Comparing `cwtune-0.1.11/.gitignore` & `cwtune-0.1.12/.gitignore`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.11/LICENSE` & `cwtune-0.1.12/LICENSE`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.11/PKG-INFO` & `cwtune-0.1.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwtune
-Version: 0.1.11
+Version: 0.1.12
 Summary: CLI for AWS CLoudWatch Alarm Tuning/Creation
 Home-page: https://github.com/availabl-co/cwtune
 Author: Arran McCabe
 Author-email: arran@availabl.ai
 License: MIT license
 Keywords: cwtune
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `cwtune-0.1.11/README.rst` & `cwtune-0.1.12/README.rst`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.11/cwtune/aws.py` & `cwtune-0.1.12/cwtune/aws.py`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.11/cwtune/cli.py` & `cwtune-0.1.12/cwtune/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """Console script for CloudTune."""
 import sys
 import click
-import main
+import analyze
 
 @click.command()
 @click.option('--alarm-type', prompt='Alarm Type', type=click.Choice(['gt', 'lt']), help='The type of alarm, greater than (gt) or less than (lt).')
 @click.option('--period', prompt='Period (Mins)', default="5", type=click.Choice(["1", "5", "60"]), help='The period of the CloudWatch metric in minutes.')
 @click.option('--statistic', prompt='Statistic', default='Sum', type=click.Choice(['Sum', 'Average', 'Min', 'Max']), help='The statistic of the CloudWatch metric.')
 @click.option('--region', prompt='Region', help='The region of the CloudWatch metric.')
 @click.option('--aws-profile', prompt='AWS CLI Profile', required=False, help='(Optional) The profile configured in AWS CLI to use for making API calls.')
 def main(alarm_type, aws_profile=None, period=5, statistic='Sum', region='us-east-1'):
-    main.run(alarm_type, aws_profile, int(period), statistic=statistic, region=region)
-
+    analyze.run(alarm_type, aws_profile, int(period), statistic=statistic, region=region)
     return 0
 
 
 if __name__ == "__main__":
     sys.exit(main())  # pragma: no cover
```

### Comparing `cwtune-0.1.11/cwtune/main.py` & `cwtune-0.1.12/cwtune/analyze.py`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.11/cwtune/timeseries.py` & `cwtune-0.1.12/cwtune/timeseries.py`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.11/cwtune/utils.py` & `cwtune-0.1.12/cwtune/utils.py`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.11/cwtune.egg-info/PKG-INFO` & `cwtune-0.1.12/cwtune.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwtune
-Version: 0.1.11
+Version: 0.1.12
 Summary: CLI for AWS CLoudWatch Alarm Tuning/Creation
 Home-page: https://github.com/availabl-co/cwtune
 Author: Arran McCabe
 Author-email: arran@availabl.ai
 License: MIT license
 Keywords: cwtune
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `cwtune-0.1.11/cwtune.egg-info/SOURCES.txt` & `cwtune-0.1.12/cwtune.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 .gitignore
 LICENSE
 README.rst
 requirements.txt
 setup.cfg
 setup.py
 cwtune/__init__.py
+cwtune/analyze.py
 cwtune/aws.py
 cwtune/cli.py
-cwtune/main.py
 cwtune/timeseries.py
 cwtune/utils.py
 cwtune.egg-info/PKG-INFO
 cwtune.egg-info/SOURCES.txt
 cwtune.egg-info/dependency_links.txt
 cwtune.egg-info/entry_points.txt
 cwtune.egg-info/not-zip-safe
```

### Comparing `cwtune-0.1.11/setup.py` & `cwtune-0.1.12/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     include_package_data=True,
     keywords='cwtune',
     name='cwtune',
     packages=find_packages(include=['cwtune', 'cwtune.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/availabl-co/cwtune',
-    version='0.1.11',
+    version='0.1.12',
     zip_safe=False,
 )
```

### Comparing `cwtune-0.1.11/tests/__pycache__/test_cwtune.cpython-311-pytest-6.2.4.pyc` & `cwtune-0.1.12/tests/__pycache__/test_cwtune.cpython-311-pytest-6.2.4.pyc`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.11/tests/__pycache__/test_cwtune.cpython-311.pyc` & `cwtune-0.1.12/tests/__pycache__/test_cwtune.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.11/tests/test_cwtune.py` & `cwtune-0.1.12/tests/test_cwtune.py`

 * *Files identical despite different names*

