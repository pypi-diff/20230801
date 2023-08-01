# Comparing `tmp/pysep-adjtomo-0.4.0.tar.gz` & `tmp/pysep-adjtomo-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysep-adjtomo-0.4.0.tar", last modified: Wed Jul 19 20:49:32 2023, max compression
+gzip compressed data, was "pysep-adjtomo-0.4.1.tar", last modified: Tue Aug  1 19:25:47 2023, max compression
```

## Comparing `pysep-adjtomo-0.4.0.tar` & `pysep-adjtomo-0.4.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 bchow     (1000) bchow     (1000)        0 2023-07-19 20:49:32.418764 pysep-adjtomo-0.4.0/
--rw-r--r--   0 bchow     (1000) bchow     (1000)     1082 2022-08-30 23:24:45.000000 pysep-adjtomo-0.4.0/LICENSE.txt
--rw-r--r--   0 bchow     (1000) bchow     (1000)       76 2023-03-02 17:58:11.000000 pysep-adjtomo-0.4.0/MANIFEST.in
--rw-r--r--   0 bchow     (1000) bchow     (1000)     2921 2023-07-19 20:49:32.418764 pysep-adjtomo-0.4.0/PKG-INFO
--rw-r--r--   0 bchow     (1000) bchow     (1000)     1217 2023-07-19 20:20:46.000000 pysep-adjtomo-0.4.0/README.md
--rw-r--r--   0 bchow     (1000) bchow     (1000)      729 2023-07-19 20:45:37.000000 pysep-adjtomo-0.4.0/pyproject.toml
-drwxr-xr-x   0 bchow     (1000) bchow     (1000)        0 2023-07-19 20:49:32.415764 pysep-adjtomo-0.4.0/pysep/
--rw-r--r--   0 bchow     (1000) bchow     (1000)      528 2023-07-19 20:20:46.000000 pysep-adjtomo-0.4.0/pysep/__init__.py
-drwxr-xr-x   0 bchow     (1000) bchow     (1000)        0 2023-07-19 20:49:32.414764 pysep-adjtomo-0.4.0/pysep/configs/
-drwxr-xr-x   0 bchow     (1000) bchow     (1000)        0 2023-07-19 20:49:32.415764 pysep-adjtomo-0.4.0/pysep/configs/alvizuri_tape_2018/
--rw-r--r--   0 bchow     (1000) bchow     (1000)      945 2023-07-19 20:20:46.000000 pysep-adjtomo-0.4.0/pysep/configs/alvizuri_tape_2018/2006-10-09T013528_NORTH_KOREA.yaml
--rw-r--r--   0 bchow     (1000) bchow     (1000)      576 2022-08-30 23:24:45.000000 pysep-adjtomo-0.4.0/pysep/configs/alvizuri_tape_2018/event_list_alvizuri_tape_2018.txt
-drwxr-xr-x   0 bchow     (1000) bchow     (1000)        0 2023-07-19 20:49:32.416764 pysep-adjtomo-0.4.0/pysep/configs/denali_nodal/
--rw-r--r--   0 bchow     (1000) bchow     (1000)      988 2023-07-19 20:20:46.000000 pysep-adjtomo-0.4.0/pysep/configs/denali_nodal/2019-02-25T182230_CANTWELL_NODAL.yaml
--rw-r--r--   0 bchow     (1000) bchow     (1000)     1021 2023-07-19 20:20:46.000000 pysep-adjtomo-0.4.0/pysep/configs/denali_nodal/2019-02-25T182230_CANTWELL_NONNODAL.yaml
-drwxr-xr-x   0 bchow     (1000) bchow     (1000)        0 2023-07-19 20:49:32.416764 pysep-adjtomo-0.4.0/pysep/configs/misc_events/
--rw-r--r--   0 bchow     (1000) bchow     (1000)     1017 2023-07-19 20:20:46.000000 pysep-adjtomo-0.4.0/pysep/configs/misc_events/1988-02-15T181000_KERNVILLE_EXPLOSION.yaml
--rw-r--r--   0 bchow     (1000) bchow     (1000)      980 2023-07-19 20:20:46.000000 pysep-adjtomo-0.4.0/pysep/configs/misc_events/2015-10-18T051831_TAAN_FJORD_LANDSLIDE.yaml
--rw-r--r--   0 bchow     (1000) bchow     (1000)      979 2023-07-19 20:20:46.000000 pysep-adjtomo-0.4.0/pysep/configs/misc_events/2016-01-24T103037_INISKIN.yaml
-drwxr-xr-x   0 bchow     (1000) bchow     (1000)        0 2023-07-19 20:49:32.416764 pysep-adjtomo-0.4.0/pysep/configs/mtuq_workshop_2022/
--rw-r--r--   0 bchow     (1000) bchow     (1000)     1003 2023-07-19 20:20:46.000000 pysep-adjtomo-0.4.0/pysep/configs/mtuq_workshop_2022/2009-04-07T201255_ANCHORAGE.yaml
--rw-r--r--   0 bchow     (1000) bchow     (1000)     1022 2023-07-19 20:20:46.000000 pysep-adjtomo-0.4.0/pysep/configs/mtuq_workshop_2022/2014-08-25T161903_ICELAND.yaml
--rw-r--r--   0 bchow     (1000) bchow     (1000)     1016 2023-07-19 20:20:46.000000 pysep-adjtomo-0.4.0/pysep/configs/mtuq_workshop_2022/2017-09-03T033001_NORTH_KOREA.yaml
--rw-r--r--   0 bchow     (1000) bchow     (1000)     1085 2023-07-19 20:20:46.000000 pysep-adjtomo-0.4.0/pysep/configs/mtuq_workshop_2022/2020-04-04T015318_SOUTHERN_CALIFORNIA.yaml
-drwxr-xr-x   0 bchow     (1000) bchow     (1000)        0 2023-07-19 20:49:32.416764 pysep-adjtomo-0.4.0/pysep/configs/scec/
--rw-r--r--   0 bchow     (1000) bchow     (1000)      981 2023-07-19 20:20:46.000000 pysep-adjtomo-0.4.0/pysep/configs/scec/2002-03-16T213324_SOUTHERN_CALIFORNIA.yaml
--rw-r--r--   0 bchow     (1000) bchow     (1000)      792 2022-08-30 23:24:45.000000 pysep-adjtomo-0.4.0/pysep/configs/scec/event_list_scec_simulations.txt
-drwxr-xr-x   0 bchow     (1000) bchow     (1000)        0 2023-07-19 20:49:32.416764 pysep-adjtomo-0.4.0/pysep/configs/tape_etal_2018/
--rw-r--r--   0 bchow     (1000) bchow     (1000)      957 2023-07-19 20:20:46.000000 pysep-adjtomo-0.4.0/pysep/configs/tape_etal_2018/2012-04-11T092157_TAPE_2018.yaml
--rw-r--r--   0 bchow     (1000) bchow     (1000)      311 2022-08-30 23:24:45.000000 pysep-adjtomo-0.4.0/pysep/configs/tape_etal_2018/event_list_tape_etal_2018.txt
-drwxr-xr-x   0 bchow     (1000) bchow     (1000)        0 2023-07-19 20:49:32.417764 pysep-adjtomo-0.4.0/pysep/configs/test/
--rw-r--r--   0 bchow     (1000) bchow     (1000)      934 2023-07-19 20:20:46.000000 pysep-adjtomo-0.4.0/pysep/configs/test/check_rotate_12Z.yaml
--rw-r--r--   0 bchow     (1000) bchow     (1000)      948 2023-07-19 20:20:46.000000 pysep-adjtomo-0.4.0/pysep/configs/test/test_config_rotate_bug.yaml
--rw-r--r--   0 bchow     (1000) bchow     (1000)     1008 2023-07-19 20:20:46.000000 pysep-adjtomo-0.4.0/pysep/configs/test/test_mass_download.yaml
--rw-r--r--   0 bchow     (1000) bchow     (1000)      992 2023-07-19 20:20:46.000000 pysep-adjtomo-0.4.0/pysep/configs/test/test_remove_data_gaps.yaml
--rw-r--r--   0 bchow     (1000) bchow     (1000)     1003 2023-07-19 20:20:46.000000 pysep-adjtomo-0.4.0/pysep/configs/test/test_station_ids.yaml
--rw-r--r--   0 bchow     (1000) bchow     (1000)    46932 2023-03-02 17:58:11.000000 pysep-adjtomo-0.4.0/pysep/declust.py
--rw-r--r--   0 bchow     (1000) bchow     (1000)    98585 2023-07-19 20:20:46.000000 pysep-adjtomo-0.4.0/pysep/pysep.py
--rwxr-xr-x   0 bchow     (1000) bchow     (1000)   108776 2023-07-19 20:20:46.000000 pysep-adjtomo-0.4.0/pysep/recsec.py
-drwxr-xr-x   0 bchow     (1000) bchow     (1000)        0 2023-07-19 20:49:32.417764 pysep-adjtomo-0.4.0/pysep/tests/
--rw-r--r--   0 bchow     (1000) bchow     (1000)     3548 2023-03-02 17:58:11.000000 pysep-adjtomo-0.4.0/pysep/tests/test_declust.py
--rw-r--r--   0 bchow     (1000) bchow     (1000)     8441 2023-07-19 20:20:46.000000 pysep-adjtomo-0.4.0/pysep/tests/test_process.py
--rw-r--r--   0 bchow     (1000) bchow     (1000)     1857 2023-03-10 02:48:07.000000 pysep-adjtomo-0.4.0/pysep/tests/test_pysep.py
--rw-r--r--   0 bchow     (1000) bchow     (1000)     4601 2022-12-02 21:57:51.000000 pysep-adjtomo-0.4.0/pysep/tests/test_recsec.py
--rw-r--r--   0 bchow     (1000) bchow     (1000)     8298 2023-07-19 20:20:46.000000 pysep-adjtomo-0.4.0/pysep/tests/test_utils.py
-drwxr-xr-x   0 bchow     (1000) bchow     (1000)        0 2023-07-19 20:49:32.418764 pysep-adjtomo-0.4.0/pysep/utils/
--rw-r--r--   0 bchow     (1000) bchow     (1000)        0 2022-08-30 23:24:45.000000 pysep-adjtomo-0.4.0/pysep/utils/__init__.py
--rw-r--r--   0 bchow     (1000) bchow     (1000)    14648 2023-07-19 20:20:46.000000 pysep-adjtomo-0.4.0/pysep/utils/cap_sac.py
--rw-r--r--   0 bchow     (1000) bchow     (1000)    12778 2023-07-19 20:20:46.000000 pysep-adjtomo-0.4.0/pysep/utils/curtail.py
--rw-r--r--   0 bchow     (1000) bchow     (1000)     7426 2023-07-19 20:20:46.000000 pysep-adjtomo-0.4.0/pysep/utils/fetch.py
--rw-r--r--   0 bchow     (1000) bchow     (1000)     6522 2023-03-02 17:58:11.000000 pysep-adjtomo-0.4.0/pysep/utils/fmt.py
--rw-r--r--   0 bchow     (1000) bchow     (1000)    26544 2023-07-19 20:20:46.000000 pysep-adjtomo-0.4.0/pysep/utils/io.py
--rw-r--r--   0 bchow     (1000) bchow     (1000)     4447 2022-08-30 23:24:45.000000 pysep-adjtomo-0.4.0/pysep/utils/llnl.py
--rw-r--r--   0 bchow     (1000) bchow     (1000)    21867 2023-03-02 17:58:11.000000 pysep-adjtomo-0.4.0/pysep/utils/mt.py
--rw-r--r--   0 bchow     (1000) bchow     (1000)    16417 2023-07-19 20:20:46.000000 pysep-adjtomo-0.4.0/pysep/utils/plot.py
--rw-r--r--   0 bchow     (1000) bchow     (1000)    19844 2023-07-19 20:20:46.000000 pysep-adjtomo-0.4.0/pysep/utils/process.py
-drwxr-xr-x   0 bchow     (1000) bchow     (1000)        0 2023-07-19 20:49:32.418764 pysep-adjtomo-0.4.0/pysep_adjtomo.egg-info/
--rw-r--r--   0 bchow     (1000) bchow     (1000)     2921 2023-07-19 20:49:32.000000 pysep-adjtomo-0.4.0/pysep_adjtomo.egg-info/PKG-INFO
--rw-r--r--   0 bchow     (1000) bchow     (1000)     1881 2023-07-19 20:49:32.000000 pysep-adjtomo-0.4.0/pysep_adjtomo.egg-info/SOURCES.txt
--rw-r--r--   0 bchow     (1000) bchow     (1000)        1 2023-07-19 20:49:32.000000 pysep-adjtomo-0.4.0/pysep_adjtomo.egg-info/dependency_links.txt
--rw-r--r--   0 bchow     (1000) bchow     (1000)       70 2023-07-19 20:49:32.000000 pysep-adjtomo-0.4.0/pysep_adjtomo.egg-info/entry_points.txt
--rw-r--r--   0 bchow     (1000) bchow     (1000)       48 2023-07-19 20:49:32.000000 pysep-adjtomo-0.4.0/pysep_adjtomo.egg-info/requires.txt
--rw-r--r--   0 bchow     (1000) bchow     (1000)        6 2023-07-19 20:49:32.000000 pysep-adjtomo-0.4.0/pysep_adjtomo.egg-info/top_level.txt
--rw-r--r--   0 bchow     (1000) bchow     (1000)       38 2023-07-19 20:49:32.418764 pysep-adjtomo-0.4.0/setup.cfg
--rw-r--r--   0 bchow     (1000) bchow     (1000)       38 2023-03-02 17:58:11.000000 pysep-adjtomo-0.4.0/setup.py
+drwxr-xr-x   0 bchow    (13129) users      (100)        0 2023-08-01 19:25:47.215438 pysep-adjtomo-0.4.1/
+-rw-r--r--   0 bchow    (13129) users      (100)     1082 2022-06-28 19:02:51.000000 pysep-adjtomo-0.4.1/LICENSE.txt
+-rw-r--r--   0 bchow    (13129) users      (100)       76 2023-02-23 23:07:03.000000 pysep-adjtomo-0.4.1/MANIFEST.in
+-rw-r--r--   0 bchow    (13129) users      (100)     2919 2023-08-01 19:25:47.207438 pysep-adjtomo-0.4.1/PKG-INFO
+-rw-r--r--   0 bchow    (13129) users      (100)     1217 2023-07-25 22:33:44.000000 pysep-adjtomo-0.4.1/README.md
+-rw-r--r--   0 bchow    (13129) users      (100)      727 2023-08-01 19:21:31.000000 pysep-adjtomo-0.4.1/pyproject.toml
+drwxr-xr-x   0 bchow    (13129) users      (100)        0 2023-08-01 19:25:46.920434 pysep-adjtomo-0.4.1/pysep/
+-rw-r--r--   0 bchow    (13129) users      (100)      528 2023-08-01 19:21:31.000000 pysep-adjtomo-0.4.1/pysep/__init__.py
+drwxr-xr-x   0 bchow    (13129) users      (100)        0 2023-08-01 19:25:46.889433 pysep-adjtomo-0.4.1/pysep/configs/
+drwxr-xr-x   0 bchow    (13129) users      (100)        0 2023-08-01 19:25:46.927434 pysep-adjtomo-0.4.1/pysep/configs/alvizuri_tape_2018/
+-rw-r--r--   0 bchow    (13129) users      (100)      945 2023-07-25 22:33:44.000000 pysep-adjtomo-0.4.1/pysep/configs/alvizuri_tape_2018/2006-10-09T013528_NORTH_KOREA.yaml
+-rw-r--r--   0 bchow    (13129) users      (100)      576 2022-06-28 19:02:52.000000 pysep-adjtomo-0.4.1/pysep/configs/alvizuri_tape_2018/event_list_alvizuri_tape_2018.txt
+drwxr-xr-x   0 bchow    (13129) users      (100)        0 2023-08-01 19:25:46.932434 pysep-adjtomo-0.4.1/pysep/configs/denali_nodal/
+-rw-r--r--   0 bchow    (13129) users      (100)      988 2023-07-25 22:33:44.000000 pysep-adjtomo-0.4.1/pysep/configs/denali_nodal/2019-02-25T182230_CANTWELL_NODAL.yaml
+-rw-r--r--   0 bchow    (13129) users      (100)     1021 2023-07-25 22:33:44.000000 pysep-adjtomo-0.4.1/pysep/configs/denali_nodal/2019-02-25T182230_CANTWELL_NONNODAL.yaml
+drwxr-xr-x   0 bchow    (13129) users      (100)        0 2023-08-01 19:25:46.938434 pysep-adjtomo-0.4.1/pysep/configs/misc_events/
+-rw-r--r--   0 bchow    (13129) users      (100)     1017 2023-07-25 22:33:44.000000 pysep-adjtomo-0.4.1/pysep/configs/misc_events/1988-02-15T181000_KERNVILLE_EXPLOSION.yaml
+-rw-r--r--   0 bchow    (13129) users      (100)      980 2023-07-25 22:33:44.000000 pysep-adjtomo-0.4.1/pysep/configs/misc_events/2015-10-18T051831_TAAN_FJORD_LANDSLIDE.yaml
+-rw-r--r--   0 bchow    (13129) users      (100)      979 2023-07-25 22:33:44.000000 pysep-adjtomo-0.4.1/pysep/configs/misc_events/2016-01-24T103037_INISKIN.yaml
+drwxr-xr-x   0 bchow    (13129) users      (100)        0 2023-08-01 19:25:46.995435 pysep-adjtomo-0.4.1/pysep/configs/mtuq_workshop_2022/
+-rw-r--r--   0 bchow    (13129) users      (100)     1003 2023-07-25 22:33:44.000000 pysep-adjtomo-0.4.1/pysep/configs/mtuq_workshop_2022/2009-04-07T201255_ANCHORAGE.yaml
+-rw-r--r--   0 bchow    (13129) users      (100)     1022 2023-07-25 22:33:44.000000 pysep-adjtomo-0.4.1/pysep/configs/mtuq_workshop_2022/2014-08-25T161903_ICELAND.yaml
+-rw-r--r--   0 bchow    (13129) users      (100)     1016 2023-07-25 22:33:44.000000 pysep-adjtomo-0.4.1/pysep/configs/mtuq_workshop_2022/2017-09-03T033001_NORTH_KOREA.yaml
+-rw-r--r--   0 bchow    (13129) users      (100)     1085 2023-07-25 22:33:44.000000 pysep-adjtomo-0.4.1/pysep/configs/mtuq_workshop_2022/2020-04-04T015318_SOUTHERN_CALIFORNIA.yaml
+drwxr-xr-x   0 bchow    (13129) users      (100)        0 2023-08-01 19:25:47.002435 pysep-adjtomo-0.4.1/pysep/configs/scec/
+-rw-r--r--   0 bchow    (13129) users      (100)      981 2023-07-25 22:33:44.000000 pysep-adjtomo-0.4.1/pysep/configs/scec/2002-03-16T213324_SOUTHERN_CALIFORNIA.yaml
+-rw-r--r--   0 bchow    (13129) users      (100)      792 2022-06-28 19:02:52.000000 pysep-adjtomo-0.4.1/pysep/configs/scec/event_list_scec_simulations.txt
+drwxr-xr-x   0 bchow    (13129) users      (100)        0 2023-08-01 19:25:47.044436 pysep-adjtomo-0.4.1/pysep/configs/tape_etal_2018/
+-rw-r--r--   0 bchow    (13129) users      (100)      957 2023-07-25 22:33:44.000000 pysep-adjtomo-0.4.1/pysep/configs/tape_etal_2018/2012-04-11T092157_TAPE_2018.yaml
+-rw-r--r--   0 bchow    (13129) users      (100)      311 2022-06-28 19:02:52.000000 pysep-adjtomo-0.4.1/pysep/configs/tape_etal_2018/event_list_tape_etal_2018.txt
+drwxr-xr-x   0 bchow    (13129) users      (100)        0 2023-08-01 19:25:47.112437 pysep-adjtomo-0.4.1/pysep/configs/test/
+-rw-r--r--   0 bchow    (13129) users      (100)      934 2023-07-25 22:33:44.000000 pysep-adjtomo-0.4.1/pysep/configs/test/check_rotate_12Z.yaml
+-rw-r--r--   0 bchow    (13129) users      (100)      948 2023-07-25 22:33:44.000000 pysep-adjtomo-0.4.1/pysep/configs/test/test_config_rotate_bug.yaml
+-rw-r--r--   0 bchow    (13129) users      (100)     1008 2023-07-25 22:33:44.000000 pysep-adjtomo-0.4.1/pysep/configs/test/test_mass_download.yaml
+-rw-r--r--   0 bchow    (13129) users      (100)      992 2023-07-25 22:33:44.000000 pysep-adjtomo-0.4.1/pysep/configs/test/test_remove_data_gaps.yaml
+-rw-r--r--   0 bchow    (13129) users      (100)     1003 2023-07-25 22:33:44.000000 pysep-adjtomo-0.4.1/pysep/configs/test/test_station_ids.yaml
+-rw-r--r--   0 bchow    (13129) users      (100)    46932 2023-04-11 06:33:07.000000 pysep-adjtomo-0.4.1/pysep/declust.py
+-rw-r--r--   0 bchow    (13129) users      (100)    98585 2023-07-25 22:33:44.000000 pysep-adjtomo-0.4.1/pysep/pysep.py
+-rwxr-xr-x   0 bchow    (13129) users      (100)   108776 2023-07-25 22:33:44.000000 pysep-adjtomo-0.4.1/pysep/recsec.py
+drwxr-xr-x   0 bchow    (13129) users      (100)        0 2023-08-01 19:25:47.125437 pysep-adjtomo-0.4.1/pysep/tests/
+-rw-r--r--   0 bchow    (13129) users      (100)     3548 2023-02-18 00:52:54.000000 pysep-adjtomo-0.4.1/pysep/tests/test_declust.py
+-rw-r--r--   0 bchow    (13129) users      (100)     8441 2023-07-25 22:33:44.000000 pysep-adjtomo-0.4.1/pysep/tests/test_process.py
+-rw-r--r--   0 bchow    (13129) users      (100)     1857 2022-09-09 17:43:50.000000 pysep-adjtomo-0.4.1/pysep/tests/test_pysep.py
+-rw-r--r--   0 bchow    (13129) users      (100)     4601 2023-04-12 04:47:13.000000 pysep-adjtomo-0.4.1/pysep/tests/test_recsec.py
+-rw-r--r--   0 bchow    (13129) users      (100)     8298 2023-07-25 22:33:45.000000 pysep-adjtomo-0.4.1/pysep/tests/test_utils.py
+drwxr-xr-x   0 bchow    (13129) users      (100)        0 2023-08-01 19:25:47.169438 pysep-adjtomo-0.4.1/pysep/utils/
+-rw-r--r--   0 bchow    (13129) users      (100)        0 2022-06-28 19:02:52.000000 pysep-adjtomo-0.4.1/pysep/utils/__init__.py
+-rw-r--r--   0 bchow    (13129) users      (100)    14648 2023-07-25 22:33:45.000000 pysep-adjtomo-0.4.1/pysep/utils/cap_sac.py
+-rw-r--r--   0 bchow    (13129) users      (100)    12778 2023-07-25 22:33:45.000000 pysep-adjtomo-0.4.1/pysep/utils/curtail.py
+-rw-r--r--   0 bchow    (13129) users      (100)     7426 2023-07-25 22:33:45.000000 pysep-adjtomo-0.4.1/pysep/utils/fetch.py
+-rw-r--r--   0 bchow    (13129) users      (100)     6522 2023-02-18 00:52:54.000000 pysep-adjtomo-0.4.1/pysep/utils/fmt.py
+-rw-r--r--   0 bchow    (13129) users      (100)    26544 2023-07-25 22:33:45.000000 pysep-adjtomo-0.4.1/pysep/utils/io.py
+-rw-r--r--   0 bchow    (13129) users      (100)     4447 2022-06-28 19:02:53.000000 pysep-adjtomo-0.4.1/pysep/utils/llnl.py
+-rw-r--r--   0 bchow    (13129) users      (100)    21867 2023-02-18 00:52:54.000000 pysep-adjtomo-0.4.1/pysep/utils/mt.py
+-rw-r--r--   0 bchow    (13129) users      (100)    16417 2023-07-25 22:33:45.000000 pysep-adjtomo-0.4.1/pysep/utils/plot.py
+-rw-r--r--   0 bchow    (13129) users      (100)    19844 2023-07-25 22:33:45.000000 pysep-adjtomo-0.4.1/pysep/utils/process.py
+drwxr-xr-x   0 bchow    (13129) users      (100)        0 2023-08-01 19:25:47.193438 pysep-adjtomo-0.4.1/pysep_adjtomo.egg-info/
+-rw-r--r--   0 bchow    (13129) users      (100)     2919 2023-08-01 19:25:46.000000 pysep-adjtomo-0.4.1/pysep_adjtomo.egg-info/PKG-INFO
+-rw-r--r--   0 bchow    (13129) users      (100)     1881 2023-08-01 19:25:46.000000 pysep-adjtomo-0.4.1/pysep_adjtomo.egg-info/SOURCES.txt
+-rw-r--r--   0 bchow    (13129) users      (100)        1 2023-08-01 19:25:46.000000 pysep-adjtomo-0.4.1/pysep_adjtomo.egg-info/dependency_links.txt
+-rw-r--r--   0 bchow    (13129) users      (100)       70 2023-08-01 19:25:46.000000 pysep-adjtomo-0.4.1/pysep_adjtomo.egg-info/entry_points.txt
+-rw-r--r--   0 bchow    (13129) users      (100)       48 2023-08-01 19:25:46.000000 pysep-adjtomo-0.4.1/pysep_adjtomo.egg-info/requires.txt
+-rw-r--r--   0 bchow    (13129) users      (100)        6 2023-08-01 19:25:46.000000 pysep-adjtomo-0.4.1/pysep_adjtomo.egg-info/top_level.txt
+-rw-r--r--   0 bchow    (13129) users      (100)       38 2023-08-01 19:25:47.219438 pysep-adjtomo-0.4.1/setup.cfg
+-rw-r--r--   0 bchow    (13129) users      (100)       38 2023-02-18 00:52:54.000000 pysep-adjtomo-0.4.1/setup.py
```

### Comparing `pysep-adjtomo-0.4.0/LICENSE.txt` & `pysep-adjtomo-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/PKG-INFO` & `pysep-adjtomo-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysep-adjtomo
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python Seismogram Extraction and Processing
 Author: adjTomo Dev Team
 Author-email: adjtomo@gmail.com
 License: MIT License
         
         Copyright (c) University of Alaska Fairbanks
         
@@ -22,16 +22,16 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: homepage, https://github.com/adjtomo/
-Project-URL: documentation, https://pysep.readthedocs.io/
+Project-URL: homepage, https://github.com/adjtomo
+Project-URL: documentation, https://pysep.readthedocs.io
 Project-URL: repository, https://github.com/adjtomo/pysep
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 Python Seismogram Extraction and Processing
```

### Comparing `pysep-adjtomo-0.4.0/README.md` & `pysep-adjtomo-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pyproject.toml` & `pysep-adjtomo-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysep-adjtomo"
-version = "0.4.0"
+version = "0.4.1"
 description = "Python Seismogram Extraction and Processing"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 authors = [
     {name = "adjTomo Dev Team"},
     {email = "adjtomo@gmail.com"}
@@ -19,14 +19,14 @@
     "pyyaml",
 ]
 
 [project.optional-dependencies]
 dev = ["pytest", "ipython", "ipdb"]
 
 [project.urls]
-homepage = "https://github.com/adjtomo/"
-documentation = "https://pysep.readthedocs.io/"
+homepage = "https://github.com/adjtomo"
+documentation = "https://pysep.readthedocs.io"
 repository = "https://github.com/adjtomo/pysep"
 
 [project.scripts]
 pysep = "pysep.pysep:main"
 recsec = "pysep.recsec:main"
```

### Comparing `pysep-adjtomo-0.4.0/pysep/__init__.py` & `pysep-adjtomo-0.4.1/pysep/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 
 logger = logging.getLogger("pysep")
 logger.setLevel("INFO")
 logger.propagate = 0
 ch = logging.StreamHandler()
 FORMAT = "[%(asctime)s] - %(name)s - %(levelname)s: %(message)s"
 formatter = logging.Formatter(FORMAT, datefmt="%Y-%m-%d %H:%M:%S")
```

### Comparing `pysep-adjtomo-0.4.0/pysep/configs/alvizuri_tape_2018/2006-10-09T013528_NORTH_KOREA.yaml` & `pysep-adjtomo-0.4.1/pysep/configs/alvizuri_tape_2018/2006-10-09T013528_NORTH_KOREA.yaml`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep/configs/alvizuri_tape_2018/event_list_alvizuri_tape_2018.txt` & `pysep-adjtomo-0.4.1/pysep/configs/alvizuri_tape_2018/event_list_alvizuri_tape_2018.txt`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep/configs/denali_nodal/2019-02-25T182230_CANTWELL_NODAL.yaml` & `pysep-adjtomo-0.4.1/pysep/configs/denali_nodal/2019-02-25T182230_CANTWELL_NODAL.yaml`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep/configs/denali_nodal/2019-02-25T182230_CANTWELL_NONNODAL.yaml` & `pysep-adjtomo-0.4.1/pysep/configs/denali_nodal/2019-02-25T182230_CANTWELL_NONNODAL.yaml`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep/configs/misc_events/1988-02-15T181000_KERNVILLE_EXPLOSION.yaml` & `pysep-adjtomo-0.4.1/pysep/configs/misc_events/1988-02-15T181000_KERNVILLE_EXPLOSION.yaml`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep/configs/misc_events/2015-10-18T051831_TAAN_FJORD_LANDSLIDE.yaml` & `pysep-adjtomo-0.4.1/pysep/configs/misc_events/2015-10-18T051831_TAAN_FJORD_LANDSLIDE.yaml`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep/configs/misc_events/2016-01-24T103037_INISKIN.yaml` & `pysep-adjtomo-0.4.1/pysep/configs/misc_events/2016-01-24T103037_INISKIN.yaml`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep/configs/mtuq_workshop_2022/2009-04-07T201255_ANCHORAGE.yaml` & `pysep-adjtomo-0.4.1/pysep/configs/mtuq_workshop_2022/2009-04-07T201255_ANCHORAGE.yaml`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep/configs/mtuq_workshop_2022/2014-08-25T161903_ICELAND.yaml` & `pysep-adjtomo-0.4.1/pysep/configs/mtuq_workshop_2022/2014-08-25T161903_ICELAND.yaml`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep/configs/mtuq_workshop_2022/2017-09-03T033001_NORTH_KOREA.yaml` & `pysep-adjtomo-0.4.1/pysep/configs/mtuq_workshop_2022/2017-09-03T033001_NORTH_KOREA.yaml`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep/configs/mtuq_workshop_2022/2020-04-04T015318_SOUTHERN_CALIFORNIA.yaml` & `pysep-adjtomo-0.4.1/pysep/configs/mtuq_workshop_2022/2020-04-04T015318_SOUTHERN_CALIFORNIA.yaml`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep/configs/scec/2002-03-16T213324_SOUTHERN_CALIFORNIA.yaml` & `pysep-adjtomo-0.4.1/pysep/configs/scec/2002-03-16T213324_SOUTHERN_CALIFORNIA.yaml`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep/configs/scec/event_list_scec_simulations.txt` & `pysep-adjtomo-0.4.1/pysep/configs/scec/event_list_scec_simulations.txt`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep/configs/tape_etal_2018/2012-04-11T092157_TAPE_2018.yaml` & `pysep-adjtomo-0.4.1/pysep/configs/tape_etal_2018/2012-04-11T092157_TAPE_2018.yaml`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep/configs/test/check_rotate_12Z.yaml` & `pysep-adjtomo-0.4.1/pysep/configs/test/check_rotate_12Z.yaml`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep/configs/test/test_config_rotate_bug.yaml` & `pysep-adjtomo-0.4.1/pysep/configs/test/test_config_rotate_bug.yaml`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep/configs/test/test_mass_download.yaml` & `pysep-adjtomo-0.4.1/pysep/configs/test/test_mass_download.yaml`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep/configs/test/test_remove_data_gaps.yaml` & `pysep-adjtomo-0.4.1/pysep/configs/test/test_remove_data_gaps.yaml`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep/configs/test/test_station_ids.yaml` & `pysep-adjtomo-0.4.1/pysep/configs/test/test_station_ids.yaml`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep/declust.py` & `pysep-adjtomo-0.4.1/pysep/declust.py`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep/pysep.py` & `pysep-adjtomo-0.4.1/pysep/pysep.py`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep/recsec.py` & `pysep-adjtomo-0.4.1/pysep/recsec.py`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep/tests/test_declust.py` & `pysep-adjtomo-0.4.1/pysep/tests/test_declust.py`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep/tests/test_process.py` & `pysep-adjtomo-0.4.1/pysep/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep/tests/test_pysep.py` & `pysep-adjtomo-0.4.1/pysep/tests/test_pysep.py`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep/tests/test_recsec.py` & `pysep-adjtomo-0.4.1/pysep/tests/test_recsec.py`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep/tests/test_utils.py` & `pysep-adjtomo-0.4.1/pysep/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep/utils/cap_sac.py` & `pysep-adjtomo-0.4.1/pysep/utils/cap_sac.py`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep/utils/curtail.py` & `pysep-adjtomo-0.4.1/pysep/utils/curtail.py`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep/utils/fetch.py` & `pysep-adjtomo-0.4.1/pysep/utils/fetch.py`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep/utils/fmt.py` & `pysep-adjtomo-0.4.1/pysep/utils/fmt.py`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep/utils/io.py` & `pysep-adjtomo-0.4.1/pysep/utils/io.py`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep/utils/llnl.py` & `pysep-adjtomo-0.4.1/pysep/utils/llnl.py`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep/utils/mt.py` & `pysep-adjtomo-0.4.1/pysep/utils/mt.py`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep/utils/plot.py` & `pysep-adjtomo-0.4.1/pysep/utils/plot.py`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep/utils/process.py` & `pysep-adjtomo-0.4.1/pysep/utils/process.py`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.4.0/pysep_adjtomo.egg-info/PKG-INFO` & `pysep-adjtomo-0.4.1/pysep_adjtomo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysep-adjtomo
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python Seismogram Extraction and Processing
 Author: adjTomo Dev Team
 Author-email: adjtomo@gmail.com
 License: MIT License
         
         Copyright (c) University of Alaska Fairbanks
         
@@ -22,16 +22,16 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: homepage, https://github.com/adjtomo/
-Project-URL: documentation, https://pysep.readthedocs.io/
+Project-URL: homepage, https://github.com/adjtomo
+Project-URL: documentation, https://pysep.readthedocs.io
 Project-URL: repository, https://github.com/adjtomo/pysep
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 Python Seismogram Extraction and Processing
```

### Comparing `pysep-adjtomo-0.4.0/pysep_adjtomo.egg-info/SOURCES.txt` & `pysep-adjtomo-0.4.1/pysep_adjtomo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

