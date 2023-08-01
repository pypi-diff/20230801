# Comparing `tmp/pz-sniper-0.1.0.tar.gz` & `tmp/pz-sniper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-sniper-0.1.0.tar", last modified: Sun Jul 30 17:49:03 2023, max compression
+gzip compressed data, was "pz-sniper-0.1.1.tar", last modified: Tue Aug  1 01:49:27 2023, max compression
```

## Comparing `pz-sniper-0.1.0.tar` & `pz-sniper-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,22 @@
-drwxrwxr-x   0 seanmacdonald  (1000) seanmacdonald  (1000)        0 2023-07-30 17:49:03.463858 pz-sniper-0.1.0/
--rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)     1066 2023-07-28 20:51:41.000000 pz-sniper-0.1.0/LICENSE
--rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)      315 2023-07-30 17:49:03.464858 pz-sniper-0.1.0/PKG-INFO
--rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)      239 2023-07-29 20:56:09.000000 pz-sniper-0.1.0/README.md
--rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)       80 2023-07-30 16:56:19.000000 pz-sniper-0.1.0/pyproject.toml
-drwxrwxr-x   0 seanmacdonald  (1000) seanmacdonald  (1000)        0 2023-07-30 17:49:03.461858 pz-sniper-0.1.0/pz_sniper.egg-info/
--rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)      315 2023-07-30 17:49:03.000000 pz-sniper-0.1.0/pz_sniper.egg-info/PKG-INFO
--rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)      436 2023-07-30 17:49:03.000000 pz-sniper-0.1.0/pz_sniper.egg-info/SOURCES.txt
--rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)        1 2023-07-30 17:49:03.000000 pz-sniper-0.1.0/pz_sniper.egg-info/dependency_links.txt
--rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)       43 2023-07-30 17:49:03.000000 pz-sniper-0.1.0/pz_sniper.egg-info/entry_points.txt
--rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)       24 2023-07-30 17:49:03.000000 pz-sniper-0.1.0/pz_sniper.egg-info/requires.txt
--rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)        7 2023-07-30 17:49:03.000000 pz-sniper-0.1.0/pz_sniper.egg-info/top_level.txt
--rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)      526 2023-07-30 17:49:03.464858 pz-sniper-0.1.0/setup.cfg
-drwxrwxr-x   0 seanmacdonald  (1000) seanmacdonald  (1000)        0 2023-07-30 17:49:03.463858 pz-sniper-0.1.0/sniper/
--rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)        0 2023-07-28 18:31:00.000000 pz-sniper-0.1.0/sniper/__init__.py
--rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)      934 2023-07-29 19:35:59.000000 pz-sniper-0.1.0/sniper/ami.py
--rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)      176 2023-07-30 14:20:35.000000 pz-sniper-0.1.0/sniper/aws.py
--rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)      655 2023-07-29 20:17:21.000000 pz-sniper-0.1.0/sniper/cli.py
--rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)     1265 2023-07-30 14:19:25.000000 pz-sniper-0.1.0/sniper/engine.py
--rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)      364 2023-07-28 20:51:03.000000 pz-sniper-0.1.0/sniper/instances.py
--rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)      287 2023-07-28 20:11:07.000000 pz-sniper-0.1.0/sniper/list_buckets.py
--rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)      249 2023-07-28 20:11:13.000000 pz-sniper-0.1.0/sniper/rows.py
--rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)      963 2023-07-29 20:44:30.000000 pz-sniper-0.1.0/sniper/snapshot.py
--rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)      600 2023-07-30 14:25:10.000000 pz-sniper-0.1.0/sniper/sniper.py
--rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)      343 2023-07-30 14:24:21.000000 pz-sniper-0.1.0/sniper/spreadsheet.py
+drwxrwxr-x   0 seanmacdonald  (1000) seanmacdonald  (1000)        0 2023-08-01 01:49:27.516486 pz-sniper-0.1.1/
+-rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)     1066 2023-07-28 20:51:41.000000 pz-sniper-0.1.1/LICENSE
+-rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)      311 2023-08-01 01:49:27.516486 pz-sniper-0.1.1/PKG-INFO
+-rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)     2178 2023-08-01 01:49:11.000000 pz-sniper-0.1.1/README.md
+-rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)       81 2023-08-01 01:46:46.000000 pz-sniper-0.1.1/pyproject.toml
+drwxrwxr-x   0 seanmacdonald  (1000) seanmacdonald  (1000)        0 2023-08-01 01:49:27.514486 pz-sniper-0.1.1/pz_sniper.egg-info/
+-rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)      311 2023-08-01 01:49:27.000000 pz-sniper-0.1.1/pz_sniper.egg-info/PKG-INFO
+-rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)      378 2023-08-01 01:49:27.000000 pz-sniper-0.1.1/pz_sniper.egg-info/SOURCES.txt
+-rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)        1 2023-08-01 01:49:27.000000 pz-sniper-0.1.1/pz_sniper.egg-info/dependency_links.txt
+-rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)       43 2023-08-01 01:49:27.000000 pz-sniper-0.1.1/pz_sniper.egg-info/entry_points.txt
+-rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)       24 2023-08-01 01:49:27.000000 pz-sniper-0.1.1/pz_sniper.egg-info/requires.txt
+-rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)        7 2023-08-01 01:49:27.000000 pz-sniper-0.1.1/pz_sniper.egg-info/top_level.txt
+-rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)      522 2023-08-01 01:49:27.517486 pz-sniper-0.1.1/setup.cfg
+drwxrwxr-x   0 seanmacdonald  (1000) seanmacdonald  (1000)        0 2023-08-01 01:49:27.516486 pz-sniper-0.1.1/sniper/
+-rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)        0 2023-07-28 18:31:00.000000 pz-sniper-0.1.1/sniper/__init__.py
+-rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)      947 2023-08-01 01:44:53.000000 pz-sniper-0.1.1/sniper/ami.py
+-rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)      151 2023-08-01 01:41:20.000000 pz-sniper-0.1.1/sniper/aws.py
+-rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)      655 2023-07-29 20:17:21.000000 pz-sniper-0.1.1/sniper/cli.py
+-rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)     1265 2023-07-30 14:19:25.000000 pz-sniper-0.1.1/sniper/engine.py
+-rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)      439 2023-08-01 01:40:54.000000 pz-sniper-0.1.1/sniper/region.py
+-rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)      963 2023-07-29 20:44:30.000000 pz-sniper-0.1.1/sniper/snapshot.py
+-rw-rw-r--   0 seanmacdonald  (1000) seanmacdonald  (1000)      343 2023-07-30 14:24:21.000000 pz-sniper-0.1.1/sniper/spreadsheet.py
```

### Comparing `pz-sniper-0.1.0/LICENSE` & `pz-sniper-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-sniper-0.1.0/setup.cfg` & `pz-sniper-0.1.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = pz-sniper
-version = 0.1.0
-description = "kill resources across all regions in AWS in a targetted fashion"
-long_description = "This tool iterates over fields in a CSV representing resouces you want to delete. It then makes sure that resource is tagged with deleteme=yes. Then, it deletes."
+version = 0.1.1
+description = kill resources across all regions in AWS in a targetted fashion
+long_description = This tool iterates over fields in a CSV representing resouces you want to delete. It then makes sure that resource is tagged with deleteme=yes. Then, it deletes.
 
 [options]
 packages = find:
 install_requires = 
 	boto3
 	botocore
 	argparse
```

### Comparing `pz-sniper-0.1.0/sniper/ami.py` & `pz-sniper-0.1.1/sniper/ami.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,16 @@
                 has_tag = True
     return has_tag
 
 def deregister(id, dryrun, region):
     try:
         conn = boto3.client(service_name="ec2", region_name=region)
         conn.deregister_image(
-            ImageId=id,DryRun=dryrun
+            ImageId=id,
+            DryRun=dryrun
         )
     except ClientError as ce:
         print(ce.response['Error']['Message'])
         pass
     except Exception as e:
         print(e)
         raise
```

### Comparing `pz-sniper-0.1.0/sniper/cli.py` & `pz-sniper-0.1.1/sniper/cli.py`

 * *Files identical despite different names*

### Comparing `pz-sniper-0.1.0/sniper/engine.py` & `pz-sniper-0.1.1/sniper/engine.py`

 * *Files identical despite different names*

### Comparing `pz-sniper-0.1.0/sniper/snapshot.py` & `pz-sniper-0.1.1/sniper/snapshot.py`

 * *Files identical despite different names*

