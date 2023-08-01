# Comparing `tmp/siriuspy-2.79.0.tar.gz` & `tmp/siriuspy-2.79.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siriuspy-2.79.0.tar", last modified: Sun Jul 30 14:45:12 2023, max compression
+gzip compressed data, was "siriuspy-2.79.1.tar", last modified: Tue Aug  1 18:59:56 2023, max compression
```

## Comparing `siriuspy-2.79.0.tar` & `siriuspy-2.79.1.tar`

### file list

```diff
@@ -1,399 +1,399 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.893647 siriuspy-2.79.0/
--rw-r--r--   0 runner    (1001) docker     (122)    34494 2023-07-30 14:45:00.000000 siriuspy-2.79.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-07-30 14:45:00.000000 siriuspy-2.79.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-07-30 14:45:12.893647 siriuspy-2.79.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      954 2023-07-30 14:45:00.000000 siriuspy-2.79.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-07-30 14:45:00.000000 siriuspy-2.79.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-30 14:45:12.893647 siriuspy-2.79.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     1243 2023-07-30 14:45:00.000000 siriuspy-2.79.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.853647 siriuspy-2.79.0/siriuspy/
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)      515 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.857647 siriuspy-2.79.0/siriuspy/bsmp/
--rw-r--r--   0 runner    (1001) docker     (122)      422 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/bsmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15885 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/bsmp/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)     1904 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/bsmp/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    11790 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/bsmp/entities.py
--rw-r--r--   0 runner    (1001) docker     (122)      610 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/bsmp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     8110 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/bsmp/serial.py
--rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/bsmp/types.py
--rw-r--r--   0 runner    (1001) docker     (122)     2992 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.857647 siriuspy-2.79.0/siriuspy/clientarch/
--rw-r--r--   0 runner    (1001) docker     (122)      306 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientarch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientarch/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     6392 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientarch/devices.py
--rw-r--r--   0 runner    (1001) docker     (122)      643 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientarch/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    20400 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientarch/pvarch.py
--rw-r--r--   0 runner    (1001) docker     (122)     5003 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientarch/time.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.857647 siriuspy-2.79.0/siriuspy/clientconfigdb/
--rw-r--r--   0 runner    (1001) docker     (122)      227 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3345 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/_templates.py
--rw-r--r--   0 runner    (1001) docker     (122)     9599 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/configdb_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     5448 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/configdb_document.py
--rw-r--r--   0 runner    (1001) docker     (122)     4785 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/pvsconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.865647 siriuspy-2.79.0/siriuspy/clientconfigdb/types/
--rw-r--r--   0 runner    (1001) docker     (122)      286 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13746 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/as_corrloop_params.py
--rw-r--r--   0 runner    (1001) docker     (122)    49080 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/as_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (122)     6681 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/as_pwrstate.py
--rw-r--r--   0 runner    (1001) docker     (122)    34247 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/as_rf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/bo_chromcorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     3984 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/bo_normalized.py
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      700 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/bo_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     3042 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/bo_ramp.py
--rw-r--r--   0 runner    (1001) docker     (122)      975 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/bo_tunecorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)   124502 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/global_config.py
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_bbadata.py
--rw-r--r--   0 runner    (1001) docker     (122)    18619 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_bbbproc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_chromcorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)     4741 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_fofb.py
--rw-r--r--   0 runner    (1001) docker     (122)      957 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_id.py
--rw-r--r--   0 runner    (1001) docker     (122)     3181 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_idff.py
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      701 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_tunecorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     1738 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/tb_normalized.py
--rw-r--r--   0 runner    (1001) docker     (122)      969 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      693 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/tb_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/tb_posang_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      969 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      693 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/ts_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1721 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientconfigdb/types/ts_posang_respm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.865647 siriuspy-2.79.0/siriuspy/clientweb/
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientweb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5896 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/clientweb/implementation.py
--rw-r--r--   0 runner    (1001) docker     (122)     2236 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.865647 siriuspy-2.79.0/siriuspy/currinfo/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/currinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9620 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/currinfo/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.865647 siriuspy-2.79.0/siriuspy/currinfo/lifetime/
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/currinfo/lifetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12607 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/currinfo/lifetime/main.py
--rw-r--r--   0 runner    (1001) docker     (122)    23275 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/currinfo/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.865647 siriuspy-2.79.0/siriuspy/cycle/
--rw-r--r--   0 runner    (1001) docker     (122)      514 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/cycle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   104994 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/cycle/bo_cycle_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    31135 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/cycle/conn.py
--rw-r--r--   0 runner    (1001) docker     (122)     9781 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/cycle/fc_cycle_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     3286 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/cycle/li_cycle_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    38408 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/cycle/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     3574 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/cycle/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.869647 siriuspy-2.79.0/siriuspy/devices/
--rw-r--r--   0 runner    (1001) docker     (122)     1969 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4172 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/afc_acq_core.py
--rw-r--r--   0 runner    (1001) docker     (122)    48546 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/bbb.py
--rw-r--r--   0 runner    (1001) docker     (122)     2786 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/blctrl.py
--rw-r--r--   0 runner    (1001) docker     (122)    40718 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/bpm.py
--rw-r--r--   0 runner    (1001) docker     (122)     7380 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/currinfo.py
--rw-r--r--   0 runner    (1001) docker     (122)     2402 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/dcct.py
--rw-r--r--   0 runner    (1001) docker     (122)    13949 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (122)    19400 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/dvf.py
--rw-r--r--   0 runner    (1001) docker     (122)    30814 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/egun.py
--rw-r--r--   0 runner    (1001) docker     (122)     1743 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/energy.py
--rw-r--r--   0 runner    (1001) docker     (122)    51455 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/fofb.py
--rw-r--r--   0 runner    (1001) docker     (122)    46088 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/fofb_acq.py
--rw-r--r--   0 runner    (1001) docker     (122)     2121 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/ict.py
--rw-r--r--   0 runner    (1001) docker     (122)    10051 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/idff.py
--rw-r--r--   0 runner    (1001) docker     (122)    21328 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/ids.py
--rw-r--r--   0 runner    (1001) docker     (122)    20759 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/injctrl.py
--rw-r--r--   0 runner    (1001) docker     (122)    38127 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/injsys.py
--rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/lienergy.py
--rw-r--r--   0 runner    (1001) docker     (122)     6948 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/lillrf.py
--rw-r--r--   0 runner    (1001) docker     (122)      964 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/machshift.py
--rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/modltr.py
--rw-r--r--   0 runner    (1001) docker     (122)    36084 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/orbit_interlock.py
--rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/posang.py
--rw-r--r--   0 runner    (1001) docker     (122)    10195 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/psconv.py
--rw-r--r--   0 runner    (1001) docker     (122)    12184 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/pssofb.py
--rw-r--r--   0 runner    (1001) docker     (122)    20070 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/pstesters.py
--rw-r--r--   0 runner    (1001) docker     (122)    30064 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/pwrsupply.py
--rw-r--r--   0 runner    (1001) docker     (122)    35448 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/rf.py
--rw-r--r--   0 runner    (1001) docker     (122)     8522 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/scraper.py
--rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/screen.py
--rw-r--r--   0 runner    (1001) docker     (122)    25271 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/sofb.py
--rw-r--r--   0 runner    (1001) docker     (122)     2652 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/syncd.py
--rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/timing.py
--rw-r--r--   0 runner    (1001) docker     (122)     5055 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/devices/tune.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.869647 siriuspy-2.79.0/siriuspy/diagbeam/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagbeam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.869647 siriuspy-2.79.0/siriuspy/diagbeam/bpm/
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagbeam/bpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    24054 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagbeam/bpm/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.869647 siriuspy-2.79.0/siriuspy/diagbeam/dcct/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagbeam/dcct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8215 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagbeam/dcct/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.869647 siriuspy-2.79.0/siriuspy/diagbeam/ict/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagbeam/ict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4878 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagbeam/ict/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.869647 siriuspy-2.79.0/siriuspy/diagbeam/screen/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagbeam/screen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12756 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagbeam/screen/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.869647 siriuspy-2.79.0/siriuspy/diagbeam/slit/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagbeam/slit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6750 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagbeam/slit/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.869647 siriuspy-2.79.0/siriuspy/diagsys/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1484 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.869647 siriuspy-2.79.0/siriuspy/diagsys/lidiag/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/lidiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5193 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/lidiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     8168 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/lidiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     8774 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/lidiag/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.873647 siriuspy-2.79.0/siriuspy/diagsys/psdiag/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/psdiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2699 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/psdiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     4582 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/psdiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     7692 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/psdiag/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.873647 siriuspy-2.79.0/siriuspy/diagsys/pudiag/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/pudiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1418 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/pudiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     2871 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/pudiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     4099 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/pudiag/pvs.py
--rw-r--r--   0 runner    (1001) docker     (122)     6792 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.873647 siriuspy-2.79.0/siriuspy/diagsys/rfdiag/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/rfdiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2409 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/rfdiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     3783 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/rfdiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     4891 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/diagsys/rfdiag/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.873647 siriuspy-2.79.0/siriuspy/dvfimgproc/
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/dvfimgproc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7692 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/dvfimgproc/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    15295 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/dvfimgproc/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     7082 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/dvfimgproc/meas.py
--rw-r--r--   0 runner    (1001) docker     (122)     2135 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/envars.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.873647 siriuspy-2.79.0/siriuspy/epics/
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/epics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      624 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/epics/multiproc.py
--rw-r--r--   0 runner    (1001) docker     (122)     9097 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/epics/properties.py
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/epics/pv.py
--rw-r--r--   0 runner    (1001) docker     (122)    29251 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/epics/pv_fake.py
--rw-r--r--   0 runner    (1001) docker     (122)     9170 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/epics/pv_time_serie.py
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/epics/threading.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.873647 siriuspy-2.79.0/siriuspy/fofb/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/fofb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19263 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/fofb/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    77425 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/fofb/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.873647 siriuspy-2.79.0/siriuspy/idff/
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/idff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7315 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/idff/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     3408 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/idff/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    14175 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/idff/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.873647 siriuspy-2.79.0/siriuspy/injctrl/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/injctrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15253 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/injctrl/bias_feedback.py
--rw-r--r--   0 runner    (1001) docker     (122)    24732 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/injctrl/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    70114 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/injctrl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.877647 siriuspy-2.79.0/siriuspy/machshift/
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/machshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1297 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/machshift/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     6903 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/machshift/gensumm_macreport.py
--rw-r--r--   0 runner    (1001) docker     (122)    78928 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/machshift/macreport.py
--rw-r--r--   0 runner    (1001) docker     (122)     9197 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/machshift/macschedule.py
--rw-r--r--   0 runner    (1001) docker     (122)     2237 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/machshift/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     2539 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/machshift/savedata_macreport.py
--rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/machshift/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.877647 siriuspy-2.79.0/siriuspy/magnet/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/magnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/magnet/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     8736 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/magnet/excdata.py
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/magnet/factory.py
--rw-r--r--   0 runner    (1001) docker     (122)    15453 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/magnet/normalizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     7185 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/magnet/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.877647 siriuspy-2.79.0/siriuspy/meas/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/meas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11826 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/meas/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.877647 siriuspy-2.79.0/siriuspy/meas/liemit/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/meas/liemit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/meas/liemit/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    13017 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/meas/liemit/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.877647 siriuspy-2.79.0/siriuspy/meas/lienergy/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/meas/lienergy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/meas/lienergy/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     8714 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/meas/lienergy/main.py
--rw-r--r--   0 runner    (1001) docker     (122)    25137 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/meas/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.877647 siriuspy-2.79.0/siriuspy/namesys/
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/namesys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/namesys/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.877647 siriuspy-2.79.0/siriuspy/optics/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/optics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      363 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/optics/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     8749 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/optics/lattice_survey.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.877647 siriuspy-2.79.0/siriuspy/opticscorr/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/opticscorr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    34878 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/opticscorr/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    16096 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/opticscorr/chrom.py
--rw-r--r--   0 runner    (1001) docker     (122)    13454 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/opticscorr/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    18765 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/opticscorr/opticscorr.py
--rw-r--r--   0 runner    (1001) docker     (122)     8006 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/opticscorr/tune.py
--rw-r--r--   0 runner    (1001) docker     (122)     1846 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/opticscorr/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.877647 siriuspy-2.79.0/siriuspy/oscilloscope/
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/oscilloscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7003 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/oscilloscope/keysight.py
--rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/oscilloscope/scopes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.877647 siriuspy-2.79.0/siriuspy/posang/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/posang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/posang/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    19747 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/posang/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/posang/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.881647 siriuspy-2.79.0/siriuspy/pwrsupply/
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8950 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/beaglebone.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.881647 siriuspy-2.79.0/siriuspy/pwrsupply/bsmp/
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/bsmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    25156 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/bsmp/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)    19464 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/bsmp/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    53763 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/bsmp/entities.py
--rw-r--r--   0 runner    (1001) docker     (122)      850 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/bsmp/factory.py
--rw-r--r--   0 runner    (1001) docker     (122)   150566 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     3624 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/data.py
--rw-r--r--   0 runner    (1001) docker     (122)    10629 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.881647 siriuspy-2.79.0/siriuspy/pwrsupply/pructrl/
--rw-r--r--   0 runner    (1001) docker     (122)      841 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/pructrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3393 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/pructrl/pru.py
--rw-r--r--   0 runner    (1001) docker     (122)    25723 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/pructrl/prucontroller.py
--rw-r--r--   0 runner    (1001) docker     (122)     6133 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/pructrl/prucparms.py
--rw-r--r--   0 runner    (1001) docker     (122)    10280 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/pructrl/psdevstate.py
--rw-r--r--   0 runner    (1001) docker     (122)     7712 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/pructrl/udc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.881647 siriuspy-2.79.0/siriuspy/pwrsupply/psctrl/
--rw-r--r--   0 runner    (1001) docker     (122)      866 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/psctrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7884 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/psctrl/pscontroller.py
--rw-r--r--   0 runner    (1001) docker     (122)     6262 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/psctrl/pscreaders.py
--rw-r--r--   0 runner    (1001) docker     (122)     5502 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/psctrl/pscstatus.py
--rw-r--r--   0 runner    (1001) docker     (122)    17064 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/psctrl/pscwriters.py
--rw-r--r--   0 runner    (1001) docker     (122)    42124 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/psctrl/psmodel.py
--rw-r--r--   0 runner    (1001) docker     (122)    34142 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/pssofb.py
--rw-r--r--   0 runner    (1001) docker     (122)    12500 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/pwrsupply/siggen.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.881647 siriuspy-2.79.0/siriuspy/ramp/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/ramp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    28999 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/ramp/conn.py
--rw-r--r--   0 runner    (1001) docker     (122)      346 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/ramp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3969 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/ramp/magnet.py
--rw-r--r--   0 runner    (1001) docker     (122)    45093 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/ramp/ramp.py
--rw-r--r--   0 runner    (1001) docker     (122)    29333 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/ramp/reconst_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6985 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/ramp/test_reconst_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4158 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/ramp/testwfm.py
--rw-r--r--   0 runner    (1001) docker     (122)     5584 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/ramp/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    30145 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/ramp/waveform.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.885647 siriuspy-2.79.0/siriuspy/search/
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3537 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/search/bpms_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     6903 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/search/hl_time_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     5566 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/search/id_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     4152 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/search/ioc_search.py
--rw-r--r--   0 runner    (1001) docker     (122)    17480 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/search/ll_time_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     7219 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/search/ma_search.py
--rw-r--r--   0 runner    (1001) docker     (122)    23882 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/search/ps_search.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.885647 siriuspy-2.79.0/siriuspy/simul/
--rw-r--r--   0 runner    (1001) docker     (122)      311 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/simul/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/simul/simfactory.py
--rw-r--r--   0 runner    (1001) docker     (122)     6298 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/simul/simps.py
--rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/simul/simpv.py
--rw-r--r--   0 runner    (1001) docker     (122)     7391 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/simul/simulation.py
--rw-r--r--   0 runner    (1001) docker     (122)     4266 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/simul/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.889647 siriuspy-2.79.0/siriuspy/sofb/
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/sofb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4869 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/sofb/base_class.py
--rw-r--r--   0 runner    (1001) docker     (122)    28072 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/sofb/bpms.py
--rw-r--r--   0 runner    (1001) docker     (122)    32010 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/sofb/correctors.py
--rw-r--r--   0 runner    (1001) docker     (122)    47062 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/sofb/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    46398 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/sofb/main.py
--rw-r--r--   0 runner    (1001) docker     (122)    11841 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/sofb/matrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    36357 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/sofb/orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/sofb/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.889647 siriuspy-2.79.0/siriuspy/stabinfo/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/stabinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3558 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/stabinfo/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     7708 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/stabinfo/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     8598 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/thread.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.889647 siriuspy-2.79.0/siriuspy/timesys/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/timesys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20485 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/timesys/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    12705 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/timesys/hl_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)    33336 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/timesys/ll_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     6015 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/timesys/plot_network.py
--rw-r--r--   0 runner    (1001) docker     (122)     5957 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/timesys/static_table.py
--rw-r--r--   0 runner    (1001) docker     (122)     8732 2023-07-30 14:45:00.000000 siriuspy-2.79.0/siriuspy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.857647 siriuspy-2.79.0/siriuspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-07-30 14:45:12.000000 siriuspy-2.79.0/siriuspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10223 2023-07-30 14:45:12.000000 siriuspy-2.79.0/siriuspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-30 14:45:12.000000 siriuspy-2.79.0/siriuspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-30 14:45:12.000000 siriuspy-2.79.0/siriuspy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-07-30 14:45:12.000000 siriuspy-2.79.0/siriuspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-30 14:45:12.000000 siriuspy-2.79.0/siriuspy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.889647 siriuspy-2.79.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      441 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.889647 siriuspy-2.79.0/tests/bsmp/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/bsmp/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5698 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/bsmp/test_bsmp.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    14788 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/bsmp/test_commands.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    13382 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/bsmp/test_entities.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7719 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/bsmp/test_serial.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1837 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/bsmp/test_types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.889647 siriuspy-2.79.0/tests/clientconfigdb/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/clientconfigdb/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2843 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/clientconfigdb/test_configdb_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.889647 siriuspy-2.79.0/tests/clientweb/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/clientweb/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    11633 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/clientweb/test_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.889647 siriuspy-2.79.0/tests/currinfo/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/currinfo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.889647 siriuspy-2.79.0/tests/currinfo/lifetime/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/currinfo/lifetime/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1908 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/currinfo/lifetime/test_main.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6495 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/currinfo/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2653 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/currinfo/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.889647 siriuspy-2.79.0/tests/magnet/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/magnet/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2275 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/magnet/test_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2687 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/magnet/tests_normalizer.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3618 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/mock_servweb.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.889647 siriuspy-2.79.0/tests/namesys/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/namesys/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4896 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/namesys/test_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.893647 siriuspy-2.79.0/tests/opticscorr/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/opticscorr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5490 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/opticscorr/test_chrom.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4609 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/opticscorr/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    23381 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/opticscorr/test_opticscorr.py
--rw-r--r--   0 runner    (1001) docker     (122)     5692 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/opticscorr/test_tune.py
--rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/opticscorr/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.893647 siriuspy-2.79.0/tests/posang/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/posang/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2872 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/posang/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3164 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/posang/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.893647 siriuspy-2.79.0/tests/pwrsupply/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/pwrsupply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18979 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/pwrsupply/db.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.893647 siriuspy-2.79.0/tests/pwrsupply/pructrl/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/pwrsupply/pructrl/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2257 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/pwrsupply/pructrl/test_pru.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.893647 siriuspy-2.79.0/tests/pwrsupply/psctrl/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/pwrsupply/psctrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4853 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/pwrsupply/psctrl/test_pscwriters.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      166 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/pwrsupply/test_beaglebone.py
--rwxr-xr-x   0 runner    (1001) docker     (122)       89 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/pwrsupply/test_bsmp.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6439 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/pwrsupply/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7331 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/pwrsupply/test_data.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2323 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/pwrsupply/test_siggen.py
--rw-r--r--   0 runner    (1001) docker     (122)     3146 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/pwrsupply/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.893647 siriuspy-2.79.0/tests/ramp/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/ramp/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5699 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/ramp/test_magnet.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7235 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/ramp/test_waveform.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.893647 siriuspy-2.79.0/tests/search/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2433 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/search/test_hl_time_search.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      559 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/search/test_init.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3886 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/search/test_ll_time_search.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6120 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/search/test_ma_search.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    13502 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/search/test_ps_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/test_callbacks.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1009 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1605 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/test_envars.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    11533 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:12.893647 siriuspy-2.79.0/tests/timesys/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/timesys/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5018 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/timesys/test_csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)      978 2023-07-30 14:45:00.000000 siriuspy-2.79.0/tests/timesys/test_plot_network.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.740632 siriuspy-2.79.1/
+-rw-r--r--   0 runner    (1001) docker     (122)    34494 2023-08-01 18:59:48.000000 siriuspy-2.79.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-08-01 18:59:48.000000 siriuspy-2.79.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-08-01 18:59:56.740632 siriuspy-2.79.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      954 2023-08-01 18:59:48.000000 siriuspy-2.79.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-08-01 18:59:48.000000 siriuspy-2.79.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-01 18:59:56.740632 siriuspy-2.79.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1243 2023-08-01 18:59:48.000000 siriuspy-2.79.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.708632 siriuspy-2.79.1/siriuspy/
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.708632 siriuspy-2.79.1/siriuspy/bsmp/
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/bsmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15885 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/bsmp/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1904 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/bsmp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11790 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/bsmp/entities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/bsmp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8110 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/bsmp/serial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/bsmp/types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2992 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.708632 siriuspy-2.79.1/siriuspy/clientarch/
+-rw-r--r--   0 runner    (1001) docker     (122)      306 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientarch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientarch/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6392 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientarch/devices.py
+-rw-r--r--   0 runner    (1001) docker     (122)      643 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientarch/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20400 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientarch/pvarch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5003 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientarch/time.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.708632 siriuspy-2.79.1/siriuspy/clientconfigdb/
+-rw-r--r--   0 runner    (1001) docker     (122)      227 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3345 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/_templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9599 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/configdb_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5448 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/configdb_document.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4785 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/pvsconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.712632 siriuspy-2.79.1/siriuspy/clientconfigdb/types/
+-rw-r--r--   0 runner    (1001) docker     (122)      286 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13746 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/as_corrloop_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)    49080 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/as_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6681 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/as_pwrstate.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34247 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/as_rf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/bo_chromcorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3984 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/bo_normalized.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      700 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/bo_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3042 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/bo_ramp.py
+-rw-r--r--   0 runner    (1001) docker     (122)      975 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/bo_tunecorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)   124502 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/global_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_bbadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18619 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_bbbproc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_chromcorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4741 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_fofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)      957 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3181 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_idff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      701 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_tunecorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1738 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/tb_normalized.py
+-rw-r--r--   0 runner    (1001) docker     (122)      969 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/tb_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/tb_posang_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      969 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/ts_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1721 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientconfigdb/types/ts_posang_respm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.712632 siriuspy-2.79.1/siriuspy/clientweb/
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientweb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5896 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/clientweb/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2236 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.712632 siriuspy-2.79.1/siriuspy/currinfo/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/currinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9620 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/currinfo/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.712632 siriuspy-2.79.1/siriuspy/currinfo/lifetime/
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/currinfo/lifetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12607 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/currinfo/lifetime/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23275 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/currinfo/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.712632 siriuspy-2.79.1/siriuspy/cycle/
+-rw-r--r--   0 runner    (1001) docker     (122)      514 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/cycle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   104994 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/cycle/bo_cycle_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31135 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/cycle/conn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9781 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/cycle/fc_cycle_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3286 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/cycle/li_cycle_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38408 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/cycle/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3574 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/cycle/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.716632 siriuspy-2.79.1/siriuspy/devices/
+-rw-r--r--   0 runner    (1001) docker     (122)     1969 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4172 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/afc_acq_core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    48546 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/bbb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2786 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/blctrl.py
+-rw-r--r--   0 runner    (1001) docker     (122)    40718 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/bpm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7380 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/currinfo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2402 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/dcct.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13949 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19400 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/dvf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30814 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/egun.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1743 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/energy.py
+-rw-r--r--   0 runner    (1001) docker     (122)    51455 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/fofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)    46088 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/fofb_acq.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2121 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/ict.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10051 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/idff.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21328 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/ids.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20759 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/injctrl.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38127 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/injsys.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/lienergy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6948 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/lillrf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      964 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/machshift.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/modltr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36084 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/orbit_interlock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/posang.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10195 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/psconv.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12184 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/pssofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20070 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/pstesters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30064 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/pwrsupply.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35448 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/rf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8522 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/scraper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/screen.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25271 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/sofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2652 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/syncd.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/timing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5055 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/devices/tune.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.720632 siriuspy-2.79.1/siriuspy/diagbeam/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagbeam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.720632 siriuspy-2.79.1/siriuspy/diagbeam/bpm/
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagbeam/bpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24054 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagbeam/bpm/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.720632 siriuspy-2.79.1/siriuspy/diagbeam/dcct/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagbeam/dcct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8215 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagbeam/dcct/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.720632 siriuspy-2.79.1/siriuspy/diagbeam/ict/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagbeam/ict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4878 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagbeam/ict/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.720632 siriuspy-2.79.1/siriuspy/diagbeam/screen/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagbeam/screen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12756 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagbeam/screen/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.720632 siriuspy-2.79.1/siriuspy/diagbeam/slit/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagbeam/slit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6750 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagbeam/slit/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.720632 siriuspy-2.79.1/siriuspy/diagsys/
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1484 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.720632 siriuspy-2.79.1/siriuspy/diagsys/lidiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/lidiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5193 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/lidiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8168 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/lidiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8774 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/lidiag/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.720632 siriuspy-2.79.1/siriuspy/diagsys/psdiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/psdiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2699 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/psdiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4582 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/psdiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7692 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/psdiag/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.720632 siriuspy-2.79.1/siriuspy/diagsys/pudiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/pudiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1418 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/pudiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2871 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/pudiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4099 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/pudiag/pvs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6792 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.720632 siriuspy-2.79.1/siriuspy/diagsys/rfdiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/rfdiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2409 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/rfdiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3783 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/rfdiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4891 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/diagsys/rfdiag/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.720632 siriuspy-2.79.1/siriuspy/dvfimgproc/
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/dvfimgproc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7692 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/dvfimgproc/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15295 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/dvfimgproc/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7082 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/dvfimgproc/meas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2135 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/envars.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.724632 siriuspy-2.79.1/siriuspy/epics/
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/epics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      624 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/epics/multiproc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9097 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/epics/properties.py
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/epics/pv.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29251 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/epics/pv_fake.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9170 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/epics/pv_time_serie.py
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/epics/threading.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.724632 siriuspy-2.79.1/siriuspy/fofb/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/fofb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19263 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/fofb/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    77425 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/fofb/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.724632 siriuspy-2.79.1/siriuspy/idff/
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/idff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7315 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/idff/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3408 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/idff/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14175 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/idff/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.724632 siriuspy-2.79.1/siriuspy/injctrl/
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/injctrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15253 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/injctrl/bias_feedback.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24724 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/injctrl/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    70231 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/injctrl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.724632 siriuspy-2.79.1/siriuspy/machshift/
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/machshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1297 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/machshift/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6903 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/machshift/gensumm_macreport.py
+-rw-r--r--   0 runner    (1001) docker     (122)    78928 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/machshift/macreport.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9197 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/machshift/macschedule.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2237 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/machshift/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2539 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/machshift/savedata_macreport.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/machshift/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.724632 siriuspy-2.79.1/siriuspy/magnet/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/magnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/magnet/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8736 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/magnet/excdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/magnet/factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15453 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/magnet/normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7185 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/magnet/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.724632 siriuspy-2.79.1/siriuspy/meas/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/meas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11826 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/meas/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.724632 siriuspy-2.79.1/siriuspy/meas/liemit/
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/meas/liemit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/meas/liemit/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13017 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/meas/liemit/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.724632 siriuspy-2.79.1/siriuspy/meas/lienergy/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/meas/lienergy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/meas/lienergy/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8714 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/meas/lienergy/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25137 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/meas/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.728632 siriuspy-2.79.1/siriuspy/namesys/
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/namesys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/namesys/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.728632 siriuspy-2.79.1/siriuspy/optics/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/optics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      363 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/optics/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8749 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/optics/lattice_survey.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.728632 siriuspy-2.79.1/siriuspy/opticscorr/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/opticscorr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34878 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/opticscorr/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16096 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/opticscorr/chrom.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13454 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/opticscorr/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18765 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/opticscorr/opticscorr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8006 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/opticscorr/tune.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1846 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/opticscorr/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.728632 siriuspy-2.79.1/siriuspy/oscilloscope/
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/oscilloscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7003 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/oscilloscope/keysight.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/oscilloscope/scopes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.728632 siriuspy-2.79.1/siriuspy/posang/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/posang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/posang/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19747 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/posang/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/posang/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.728632 siriuspy-2.79.1/siriuspy/pwrsupply/
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8950 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/beaglebone.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.728632 siriuspy-2.79.1/siriuspy/pwrsupply/bsmp/
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/bsmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25156 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/bsmp/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19464 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/bsmp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    53763 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/bsmp/entities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      850 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/bsmp/factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)   150566 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3624 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10629 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.732632 siriuspy-2.79.1/siriuspy/pwrsupply/pructrl/
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/pructrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3393 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/pructrl/pru.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25723 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/pructrl/prucontroller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6133 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/pructrl/prucparms.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10280 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/pructrl/psdevstate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7712 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/pructrl/udc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.732632 siriuspy-2.79.1/siriuspy/pwrsupply/psctrl/
+-rw-r--r--   0 runner    (1001) docker     (122)      866 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/psctrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7884 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/psctrl/pscontroller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6262 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/psctrl/pscreaders.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5502 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/psctrl/pscstatus.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17064 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/psctrl/pscwriters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42124 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/psctrl/psmodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34142 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/pssofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12500 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/pwrsupply/siggen.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.732632 siriuspy-2.79.1/siriuspy/ramp/
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/ramp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28999 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/ramp/conn.py
+-rw-r--r--   0 runner    (1001) docker     (122)      346 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/ramp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3969 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/ramp/magnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45093 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/ramp/ramp.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29333 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/ramp/reconst_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6985 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/ramp/test_reconst_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4158 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/ramp/testwfm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5584 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/ramp/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30145 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/ramp/waveform.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.732632 siriuspy-2.79.1/siriuspy/search/
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3537 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/search/bpms_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6903 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/search/hl_time_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5566 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/search/id_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4152 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/search/ioc_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17480 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/search/ll_time_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7219 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/search/ma_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23882 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/search/ps_search.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.732632 siriuspy-2.79.1/siriuspy/simul/
+-rw-r--r--   0 runner    (1001) docker     (122)      311 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/simul/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/simul/simfactory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6298 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/simul/simps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/simul/simpv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7391 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/simul/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4266 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/simul/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.736632 siriuspy-2.79.1/siriuspy/sofb/
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/sofb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4869 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/sofb/base_class.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28072 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/sofb/bpms.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32010 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/sofb/correctors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    47062 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/sofb/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    46398 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/sofb/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11841 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/sofb/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36357 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/sofb/orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/sofb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.736632 siriuspy-2.79.1/siriuspy/stabinfo/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/stabinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3558 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/stabinfo/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7708 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/stabinfo/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8598 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/thread.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.736632 siriuspy-2.79.1/siriuspy/timesys/
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/timesys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20485 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/timesys/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12705 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/timesys/hl_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33336 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/timesys/ll_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6015 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/timesys/plot_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5957 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/timesys/static_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8732 2023-08-01 18:59:48.000000 siriuspy-2.79.1/siriuspy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.708632 siriuspy-2.79.1/siriuspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-08-01 18:59:56.000000 siriuspy-2.79.1/siriuspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    10223 2023-08-01 18:59:56.000000 siriuspy-2.79.1/siriuspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-01 18:59:56.000000 siriuspy-2.79.1/siriuspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-01 18:59:56.000000 siriuspy-2.79.1/siriuspy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-08-01 18:59:56.000000 siriuspy-2.79.1/siriuspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-08-01 18:59:56.000000 siriuspy-2.79.1/siriuspy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.736632 siriuspy-2.79.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      441 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.736632 siriuspy-2.79.1/tests/bsmp/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/bsmp/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5698 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/bsmp/test_bsmp.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    14788 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/bsmp/test_commands.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    13382 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/bsmp/test_entities.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7719 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/bsmp/test_serial.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1837 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/bsmp/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.736632 siriuspy-2.79.1/tests/clientconfigdb/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/clientconfigdb/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2843 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/clientconfigdb/test_configdb_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.736632 siriuspy-2.79.1/tests/clientweb/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/clientweb/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    11633 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/clientweb/test_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.736632 siriuspy-2.79.1/tests/currinfo/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/currinfo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.736632 siriuspy-2.79.1/tests/currinfo/lifetime/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/currinfo/lifetime/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1908 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/currinfo/lifetime/test_main.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6495 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/currinfo/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2653 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/currinfo/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.736632 siriuspy-2.79.1/tests/magnet/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/magnet/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2275 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/magnet/test_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2687 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/magnet/tests_normalizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3618 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/mock_servweb.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.736632 siriuspy-2.79.1/tests/namesys/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/namesys/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4896 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/namesys/test_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.740632 siriuspy-2.79.1/tests/opticscorr/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/opticscorr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5490 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/opticscorr/test_chrom.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4609 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/opticscorr/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    23381 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/opticscorr/test_opticscorr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5692 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/opticscorr/test_tune.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/opticscorr/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.740632 siriuspy-2.79.1/tests/posang/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/posang/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2872 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/posang/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3164 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/posang/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.740632 siriuspy-2.79.1/tests/pwrsupply/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/pwrsupply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18979 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/pwrsupply/db.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.740632 siriuspy-2.79.1/tests/pwrsupply/pructrl/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/pwrsupply/pructrl/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2257 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/pwrsupply/pructrl/test_pru.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.740632 siriuspy-2.79.1/tests/pwrsupply/psctrl/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/pwrsupply/psctrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4853 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/pwrsupply/psctrl/test_pscwriters.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      166 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/pwrsupply/test_beaglebone.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)       89 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/pwrsupply/test_bsmp.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6439 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/pwrsupply/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7331 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/pwrsupply/test_data.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2323 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/pwrsupply/test_siggen.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3146 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/pwrsupply/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.740632 siriuspy-2.79.1/tests/ramp/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/ramp/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5699 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/ramp/test_magnet.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7235 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/ramp/test_waveform.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.740632 siriuspy-2.79.1/tests/search/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2433 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/search/test_hl_time_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      559 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/search/test_init.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3886 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/search/test_ll_time_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6120 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/search/test_ma_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    13502 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/search/test_ps_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/test_callbacks.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1009 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1605 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/test_envars.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    11533 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:56.740632 siriuspy-2.79.1/tests/timesys/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/timesys/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5018 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/timesys/test_csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)      978 2023-08-01 18:59:48.000000 siriuspy-2.79.1/tests/timesys/test_plot_network.py
```

### Comparing `siriuspy-2.79.0/LICENSE` & `siriuspy-2.79.1/LICENSE`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/PKG-INFO` & `siriuspy-2.79.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siriuspy
-Version: 2.79.0
+Version: 2.79.1
 Summary: Development packages for Sirius
 Home-page: https://github.com/lnls-sirius/dev-packages
 Download-URL: https://github.com/lnls-sirius/dev-packages
 Author: lnls-sirius
 License: GNU GPLv3
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `siriuspy-2.79.0/README.md` & `siriuspy-2.79.1/README.md`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/setup.py` & `siriuspy-2.79.1/setup.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/__init__.py` & `siriuspy-2.79.1/siriuspy/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/bsmp/commands.py` & `siriuspy-2.79.1/siriuspy/bsmp/commands.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/bsmp/constants.py` & `siriuspy-2.79.1/siriuspy/bsmp/constants.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/bsmp/entities.py` & `siriuspy-2.79.1/siriuspy/bsmp/entities.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/bsmp/exceptions.py` & `siriuspy-2.79.1/siriuspy/bsmp/exceptions.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/bsmp/serial.py` & `siriuspy-2.79.1/siriuspy/bsmp/serial.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/bsmp/types.py` & `siriuspy-2.79.1/siriuspy/bsmp/types.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/callbacks.py` & `siriuspy-2.79.1/siriuspy/callbacks.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientarch/client.py` & `siriuspy-2.79.1/siriuspy/clientarch/client.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientarch/devices.py` & `siriuspy-2.79.1/siriuspy/clientarch/devices.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientarch/exceptions.py` & `siriuspy-2.79.1/siriuspy/clientarch/exceptions.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientarch/pvarch.py` & `siriuspy-2.79.1/siriuspy/clientarch/pvarch.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientarch/time.py` & `siriuspy-2.79.1/siriuspy/clientarch/time.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientconfigdb/_templates.py` & `siriuspy-2.79.1/siriuspy/clientconfigdb/_templates.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientconfigdb/configdb_client.py` & `siriuspy-2.79.1/siriuspy/clientconfigdb/configdb_client.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientconfigdb/configdb_document.py` & `siriuspy-2.79.1/siriuspy/clientconfigdb/configdb_document.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientconfigdb/pvsconfig.py` & `siriuspy-2.79.1/siriuspy/clientconfigdb/pvsconfig.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientconfigdb/types/as_corrloop_params.py` & `siriuspy-2.79.1/siriuspy/clientconfigdb/types/as_corrloop_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientconfigdb/types/as_diagnostics.py` & `siriuspy-2.79.1/siriuspy/clientconfigdb/types/as_diagnostics.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientconfigdb/types/as_pwrstate.py` & `siriuspy-2.79.1/siriuspy/clientconfigdb/types/as_pwrstate.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientconfigdb/types/as_rf.py` & `siriuspy-2.79.1/siriuspy/clientconfigdb/types/as_rf.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientconfigdb/types/bo_chromcorr_params.py` & `siriuspy-2.79.1/siriuspy/clientconfigdb/types/bo_chromcorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientconfigdb/types/bo_normalized.py` & `siriuspy-2.79.1/siriuspy/clientconfigdb/types/bo_normalized.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py` & `siriuspy-2.79.1/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientconfigdb/types/bo_orbit.py` & `siriuspy-2.79.1/siriuspy/clientconfigdb/types/bo_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientconfigdb/types/bo_ramp.py` & `siriuspy-2.79.1/siriuspy/clientconfigdb/types/bo_ramp.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientconfigdb/types/bo_tunecorr_params.py` & `siriuspy-2.79.1/siriuspy/clientconfigdb/types/bo_tunecorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientconfigdb/types/global_config.py` & `siriuspy-2.79.1/siriuspy/clientconfigdb/types/global_config.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_bbadata.py` & `siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_bbadata.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_bbbproc.py` & `siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_bbbproc.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_chromcorr_params.py` & `siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_chromcorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py` & `siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_fofb.py` & `siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_fofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_id.py` & `siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_id.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_idff.py` & `siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_idff.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_orbcorr_respm.py` & `siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_orbit.py` & `siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientconfigdb/types/si_tunecorr_params.py` & `siriuspy-2.79.1/siriuspy/clientconfigdb/types/si_tunecorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientconfigdb/types/tb_normalized.py` & `siriuspy-2.79.1/siriuspy/clientconfigdb/types/tb_normalized.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py` & `siriuspy-2.79.1/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientconfigdb/types/tb_orbit.py` & `siriuspy-2.79.1/siriuspy/clientconfigdb/types/tb_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientconfigdb/types/tb_posang_respm.py` & `siriuspy-2.79.1/siriuspy/clientconfigdb/types/tb_posang_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py` & `siriuspy-2.79.1/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientconfigdb/types/ts_orbit.py` & `siriuspy-2.79.1/siriuspy/clientconfigdb/types/ts_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientconfigdb/types/ts_posang_respm.py` & `siriuspy-2.79.1/siriuspy/clientconfigdb/types/ts_posang_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/clientweb/implementation.py` & `siriuspy-2.79.1/siriuspy/clientweb/implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/csdev.py` & `siriuspy-2.79.1/siriuspy/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/currinfo/csdev.py` & `siriuspy-2.79.1/siriuspy/currinfo/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/currinfo/lifetime/main.py` & `siriuspy-2.79.1/siriuspy/currinfo/lifetime/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/currinfo/main.py` & `siriuspy-2.79.1/siriuspy/currinfo/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/cycle/__init__.py` & `siriuspy-2.79.1/siriuspy/cycle/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/cycle/bo_cycle_data.py` & `siriuspy-2.79.1/siriuspy/cycle/bo_cycle_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/cycle/conn.py` & `siriuspy-2.79.1/siriuspy/cycle/conn.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/cycle/fc_cycle_data.py` & `siriuspy-2.79.1/siriuspy/cycle/fc_cycle_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/cycle/li_cycle_data.py` & `siriuspy-2.79.1/siriuspy/cycle/li_cycle_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/cycle/main.py` & `siriuspy-2.79.1/siriuspy/cycle/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/cycle/util.py` & `siriuspy-2.79.1/siriuspy/cycle/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/devices/__init__.py` & `siriuspy-2.79.1/siriuspy/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/devices/afc_acq_core.py` & `siriuspy-2.79.1/siriuspy/devices/afc_acq_core.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/devices/bbb.py` & `siriuspy-2.79.1/siriuspy/devices/bbb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/devices/blctrl.py` & `siriuspy-2.79.1/siriuspy/devices/blctrl.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/devices/bpm.py` & `siriuspy-2.79.1/siriuspy/devices/bpm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/devices/currinfo.py` & `siriuspy-2.79.1/siriuspy/devices/currinfo.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/devices/dcct.py` & `siriuspy-2.79.1/siriuspy/devices/dcct.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/devices/device.py` & `siriuspy-2.79.1/siriuspy/devices/device.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/devices/dvf.py` & `siriuspy-2.79.1/siriuspy/devices/dvf.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/devices/egun.py` & `siriuspy-2.79.1/siriuspy/devices/egun.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/devices/energy.py` & `siriuspy-2.79.1/siriuspy/devices/energy.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/devices/fofb.py` & `siriuspy-2.79.1/siriuspy/devices/fofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/devices/fofb_acq.py` & `siriuspy-2.79.1/siriuspy/devices/fofb_acq.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/devices/ict.py` & `siriuspy-2.79.1/siriuspy/devices/ict.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/devices/idff.py` & `siriuspy-2.79.1/siriuspy/devices/idff.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/devices/ids.py` & `siriuspy-2.79.1/siriuspy/devices/ids.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/devices/injctrl.py` & `siriuspy-2.79.1/siriuspy/devices/injctrl.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/devices/injsys.py` & `siriuspy-2.79.1/siriuspy/devices/injsys.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/devices/lienergy.py` & `siriuspy-2.79.1/siriuspy/devices/lienergy.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/devices/lillrf.py` & `siriuspy-2.79.1/siriuspy/devices/lillrf.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/devices/machshift.py` & `siriuspy-2.79.1/siriuspy/devices/machshift.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/devices/modltr.py` & `siriuspy-2.79.1/siriuspy/devices/modltr.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/devices/orbit_interlock.py` & `siriuspy-2.79.1/siriuspy/devices/orbit_interlock.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/devices/posang.py` & `siriuspy-2.79.1/siriuspy/devices/posang.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/devices/psconv.py` & `siriuspy-2.79.1/siriuspy/devices/psconv.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/devices/pssofb.py` & `siriuspy-2.79.1/siriuspy/devices/pssofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/devices/pstesters.py` & `siriuspy-2.79.1/siriuspy/devices/pstesters.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/devices/pwrsupply.py` & `siriuspy-2.79.1/siriuspy/devices/pwrsupply.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/devices/rf.py` & `siriuspy-2.79.1/siriuspy/devices/rf.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/devices/scraper.py` & `siriuspy-2.79.1/siriuspy/devices/scraper.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/devices/screen.py` & `siriuspy-2.79.1/siriuspy/devices/screen.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/devices/sofb.py` & `siriuspy-2.79.1/siriuspy/devices/sofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/devices/syncd.py` & `siriuspy-2.79.1/siriuspy/devices/syncd.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/devices/timing.py` & `siriuspy-2.79.1/siriuspy/devices/timing.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/devices/tune.py` & `siriuspy-2.79.1/siriuspy/devices/tune.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/diagbeam/bpm/csdev.py` & `siriuspy-2.79.1/siriuspy/diagbeam/bpm/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/diagbeam/dcct/csdev.py` & `siriuspy-2.79.1/siriuspy/diagbeam/dcct/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/diagbeam/ict/csdev.py` & `siriuspy-2.79.1/siriuspy/diagbeam/ict/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/diagbeam/screen/csdev.py` & `siriuspy-2.79.1/siriuspy/diagbeam/screen/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/diagbeam/slit/csdev.py` & `siriuspy-2.79.1/siriuspy/diagbeam/slit/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/diagsys/app.py` & `siriuspy-2.79.1/siriuspy/diagsys/app.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/diagsys/lidiag/csdev.py` & `siriuspy-2.79.1/siriuspy/diagsys/lidiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/diagsys/lidiag/main.py` & `siriuspy-2.79.1/siriuspy/diagsys/lidiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/diagsys/lidiag/pvs.py` & `siriuspy-2.79.1/siriuspy/diagsys/lidiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/diagsys/psdiag/csdev.py` & `siriuspy-2.79.1/siriuspy/diagsys/psdiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/diagsys/psdiag/main.py` & `siriuspy-2.79.1/siriuspy/diagsys/psdiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/diagsys/psdiag/pvs.py` & `siriuspy-2.79.1/siriuspy/diagsys/psdiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/diagsys/pudiag/csdev.py` & `siriuspy-2.79.1/siriuspy/diagsys/pudiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/diagsys/pudiag/main.py` & `siriuspy-2.79.1/siriuspy/diagsys/pudiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/diagsys/pudiag/pvs.py` & `siriuspy-2.79.1/siriuspy/diagsys/pudiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/diagsys/pvs.py` & `siriuspy-2.79.1/siriuspy/diagsys/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/diagsys/rfdiag/csdev.py` & `siriuspy-2.79.1/siriuspy/diagsys/rfdiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/diagsys/rfdiag/main.py` & `siriuspy-2.79.1/siriuspy/diagsys/rfdiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/diagsys/rfdiag/pvs.py` & `siriuspy-2.79.1/siriuspy/diagsys/rfdiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/dvfimgproc/csdev.py` & `siriuspy-2.79.1/siriuspy/dvfimgproc/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/dvfimgproc/main.py` & `siriuspy-2.79.1/siriuspy/dvfimgproc/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/dvfimgproc/meas.py` & `siriuspy-2.79.1/siriuspy/dvfimgproc/meas.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/envars.py` & `siriuspy-2.79.1/siriuspy/envars.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/epics/multiproc.py` & `siriuspy-2.79.1/siriuspy/epics/multiproc.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/epics/properties.py` & `siriuspy-2.79.1/siriuspy/epics/properties.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/epics/pv_fake.py` & `siriuspy-2.79.1/siriuspy/epics/pv_fake.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/epics/pv_time_serie.py` & `siriuspy-2.79.1/siriuspy/epics/pv_time_serie.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/fofb/csdev.py` & `siriuspy-2.79.1/siriuspy/fofb/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/fofb/main.py` & `siriuspy-2.79.1/siriuspy/fofb/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/idff/config.py` & `siriuspy-2.79.1/siriuspy/idff/config.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/idff/csdev.py` & `siriuspy-2.79.1/siriuspy/idff/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/idff/main.py` & `siriuspy-2.79.1/siriuspy/idff/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/injctrl/bias_feedback.py` & `siriuspy-2.79.1/siriuspy/injctrl/bias_feedback.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/injctrl/csdev.py` & `siriuspy-2.79.1/siriuspy/injctrl/csdev.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,19 +224,19 @@
         'BucketListStop-SP': {
             'type': 'int', 'value': 864, 'unit': 'bucket index',
             'lolim': _ct.MIN_BKT, 'hilim': _ct.MAX_BKT, },
         'BucketListStop-RB': {
             'type': 'int', 'value': 864, 'unit': 'bucket index',
             'lolim': _ct.MIN_BKT, 'hilim': _ct.MAX_BKT},
         'BucketListStep-SP': {
-            'type': 'int', 'value': 15, 'unit': 'buckets',
-            'lolim': -_ct.MAX_BKT+1, 'hilim': _ct.MAX_BKT-1},
+            'type': 'int', 'value': 29, 'unit': 'buckets',
+            'lolim': -_ct.MAX_BKT, 'hilim': _ct.MAX_BKT},
         'BucketListStep-RB': {
-            'type': 'int', 'value': 15, 'unit': 'buckets',
-            'lolim': -_ct.MAX_BKT+1, 'hilim': _ct.MAX_BKT-1},
+            'type': 'int', 'value': 29, 'unit': 'buckets',
+            'lolim': -_ct.MAX_BKT, 'hilim': _ct.MAX_BKT},
         'IsInjecting-Mon': {
             'type': 'enum', 'value': _ct.IdleInjecting.Idle,
             'enums': _et.IDLEINJECTING, 'unit': 'Idle_Inj'},
         'IsInjDelay-SP': {
             'type': 'int', 'value': 0, 'unit': 'ms',
             'lolim': 0, 'hilim': 1000},
         'IsInjDelay-RB': {
```

### Comparing `siriuspy-2.79.0/siriuspy/injctrl/main.py` & `siriuspy-2.79.1/siriuspy/injctrl/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -442,15 +442,15 @@
             self._setting_mode = False
 
         if value != _Const.InjMode.Decay:
             stg = 'top-up' if value == _Const.InjMode.TopUp else 'accumulation'
 
             if self._pumode != _Const.PUMode.Accumulation:
                 self._update_log('ERR:Set PUMode to Accumulation before')
-                self._update_log('ERR:changing mode to {stg}')
+                self._update_log(f'ERR:changing mode to {stg:s}')
                 return False
 
             self._update_log('Configuring EVG RepeatBucketList...')
             self._evg_dev['RepeatBucketList-SP'] = 1
             self._update_log(f'...done. Ready to start {stg:s}.')
 
         self._mode = value
@@ -646,15 +646,18 @@
                 return False
         self._bucketlist_stop = stop
         self.run_callbacks('BucketListStop-RB', stop)
         return True
 
     def set_bucketlist_step(self, step):
         """Set bucketlist_step."""
-        if not -_Const.MAX_BKT+1 <= step <= _Const.MAX_BKT-1:
+        if not -_Const.MAX_BKT <= step <= _Const.MAX_BKT:
+            return False
+        if step == 0:
+            self._update_log('ERR:Bucket list step must not be zero.')
             return False
         if self._mode != _Const.InjMode.Decay:
             if not self._update_bucket_list(step=step):
                 return False
         else:
             start = self._bucketlist_start
             stop = self._bucketlist_stop
```

### Comparing `siriuspy-2.79.0/siriuspy/machshift/csdev.py` & `siriuspy-2.79.1/siriuspy/machshift/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/machshift/gensumm_macreport.py` & `siriuspy-2.79.1/siriuspy/machshift/gensumm_macreport.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/machshift/macreport.py` & `siriuspy-2.79.1/siriuspy/machshift/macreport.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/machshift/macschedule.py` & `siriuspy-2.79.1/siriuspy/machshift/macschedule.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/machshift/main.py` & `siriuspy-2.79.1/siriuspy/machshift/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/machshift/savedata_macreport.py` & `siriuspy-2.79.1/siriuspy/machshift/savedata_macreport.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/machshift/utils.py` & `siriuspy-2.79.1/siriuspy/machshift/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/magnet/data.py` & `siriuspy-2.79.1/siriuspy/magnet/data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/magnet/excdata.py` & `siriuspy-2.79.1/siriuspy/magnet/excdata.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/magnet/factory.py` & `siriuspy-2.79.1/siriuspy/magnet/factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/magnet/normalizer.py` & `siriuspy-2.79.1/siriuspy/magnet/normalizer.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/magnet/util.py` & `siriuspy-2.79.1/siriuspy/magnet/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/meas/csdev.py` & `siriuspy-2.79.1/siriuspy/meas/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/meas/liemit/csdev.py` & `siriuspy-2.79.1/siriuspy/meas/liemit/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/meas/liemit/main.py` & `siriuspy-2.79.1/siriuspy/meas/liemit/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/meas/lienergy/csdev.py` & `siriuspy-2.79.1/siriuspy/meas/lienergy/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/meas/lienergy/main.py` & `siriuspy-2.79.1/siriuspy/meas/lienergy/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/meas/util.py` & `siriuspy-2.79.1/siriuspy/meas/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/namesys/implementation.py` & `siriuspy-2.79.1/siriuspy/namesys/implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/optics/lattice_survey.py` & `siriuspy-2.79.1/siriuspy/optics/lattice_survey.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/opticscorr/base.py` & `siriuspy-2.79.1/siriuspy/opticscorr/base.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/opticscorr/chrom.py` & `siriuspy-2.79.1/siriuspy/opticscorr/chrom.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/opticscorr/csdev.py` & `siriuspy-2.79.1/siriuspy/opticscorr/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/opticscorr/opticscorr.py` & `siriuspy-2.79.1/siriuspy/opticscorr/opticscorr.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/opticscorr/tune.py` & `siriuspy-2.79.1/siriuspy/opticscorr/tune.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/opticscorr/utils.py` & `siriuspy-2.79.1/siriuspy/opticscorr/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/oscilloscope/keysight.py` & `siriuspy-2.79.1/siriuspy/oscilloscope/keysight.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/oscilloscope/scopes.py` & `siriuspy-2.79.1/siriuspy/oscilloscope/scopes.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/posang/csdev.py` & `siriuspy-2.79.1/siriuspy/posang/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/posang/main.py` & `siriuspy-2.79.1/siriuspy/posang/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/posang/utils.py` & `siriuspy-2.79.1/siriuspy/posang/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/pwrsupply/beaglebone.py` & `siriuspy-2.79.1/siriuspy/pwrsupply/beaglebone.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/pwrsupply/bsmp/commands.py` & `siriuspy-2.79.1/siriuspy/pwrsupply/bsmp/commands.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/pwrsupply/bsmp/constants.py` & `siriuspy-2.79.1/siriuspy/pwrsupply/bsmp/constants.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/pwrsupply/bsmp/entities.py` & `siriuspy-2.79.1/siriuspy/pwrsupply/bsmp/entities.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/pwrsupply/bsmp/factory.py` & `siriuspy-2.79.1/siriuspy/pwrsupply/bsmp/factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/pwrsupply/csdev.py` & `siriuspy-2.79.1/siriuspy/pwrsupply/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/pwrsupply/data.py` & `siriuspy-2.79.1/siriuspy/pwrsupply/data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/pwrsupply/factory.py` & `siriuspy-2.79.1/siriuspy/pwrsupply/factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/pwrsupply/pructrl/__init__.py` & `siriuspy-2.79.1/siriuspy/pwrsupply/pructrl/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/pwrsupply/pructrl/pru.py` & `siriuspy-2.79.1/siriuspy/pwrsupply/pructrl/pru.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/pwrsupply/pructrl/prucontroller.py` & `siriuspy-2.79.1/siriuspy/pwrsupply/pructrl/prucontroller.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/pwrsupply/pructrl/prucparms.py` & `siriuspy-2.79.1/siriuspy/pwrsupply/pructrl/prucparms.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/pwrsupply/pructrl/psdevstate.py` & `siriuspy-2.79.1/siriuspy/pwrsupply/pructrl/psdevstate.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/pwrsupply/pructrl/udc.py` & `siriuspy-2.79.1/siriuspy/pwrsupply/pructrl/udc.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/pwrsupply/psctrl/__init__.py` & `siriuspy-2.79.1/siriuspy/pwrsupply/psctrl/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/pwrsupply/psctrl/pscontroller.py` & `siriuspy-2.79.1/siriuspy/pwrsupply/psctrl/pscontroller.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/pwrsupply/psctrl/pscreaders.py` & `siriuspy-2.79.1/siriuspy/pwrsupply/psctrl/pscreaders.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/pwrsupply/psctrl/pscstatus.py` & `siriuspy-2.79.1/siriuspy/pwrsupply/psctrl/pscstatus.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/pwrsupply/psctrl/pscwriters.py` & `siriuspy-2.79.1/siriuspy/pwrsupply/psctrl/pscwriters.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/pwrsupply/psctrl/psmodel.py` & `siriuspy-2.79.1/siriuspy/pwrsupply/psctrl/psmodel.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/pwrsupply/pssofb.py` & `siriuspy-2.79.1/siriuspy/pwrsupply/pssofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/pwrsupply/siggen.py` & `siriuspy-2.79.1/siriuspy/pwrsupply/siggen.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/ramp/conn.py` & `siriuspy-2.79.1/siriuspy/ramp/conn.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/ramp/magnet.py` & `siriuspy-2.79.1/siriuspy/ramp/magnet.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/ramp/ramp.py` & `siriuspy-2.79.1/siriuspy/ramp/ramp.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/ramp/reconst_factory.py` & `siriuspy-2.79.1/siriuspy/ramp/reconst_factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/ramp/test_reconst_factory.py` & `siriuspy-2.79.1/siriuspy/ramp/test_reconst_factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/ramp/testwfm.py` & `siriuspy-2.79.1/siriuspy/ramp/testwfm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/ramp/util.py` & `siriuspy-2.79.1/siriuspy/ramp/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/ramp/waveform.py` & `siriuspy-2.79.1/siriuspy/ramp/waveform.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/search/bpms_search.py` & `siriuspy-2.79.1/siriuspy/search/bpms_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/search/hl_time_search.py` & `siriuspy-2.79.1/siriuspy/search/hl_time_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/search/id_search.py` & `siriuspy-2.79.1/siriuspy/search/id_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/search/ioc_search.py` & `siriuspy-2.79.1/siriuspy/search/ioc_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/search/ll_time_search.py` & `siriuspy-2.79.1/siriuspy/search/ll_time_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/search/ma_search.py` & `siriuspy-2.79.1/siriuspy/search/ma_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/search/ps_search.py` & `siriuspy-2.79.1/siriuspy/search/ps_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/simul/simfactory.py` & `siriuspy-2.79.1/siriuspy/simul/simfactory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/simul/simps.py` & `siriuspy-2.79.1/siriuspy/simul/simps.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/simul/simpv.py` & `siriuspy-2.79.1/siriuspy/simul/simpv.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/simul/simulation.py` & `siriuspy-2.79.1/siriuspy/simul/simulation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/simul/simulator.py` & `siriuspy-2.79.1/siriuspy/simul/simulator.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/sofb/base_class.py` & `siriuspy-2.79.1/siriuspy/sofb/base_class.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/sofb/bpms.py` & `siriuspy-2.79.1/siriuspy/sofb/bpms.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/sofb/correctors.py` & `siriuspy-2.79.1/siriuspy/sofb/correctors.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/sofb/csdev.py` & `siriuspy-2.79.1/siriuspy/sofb/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/sofb/main.py` & `siriuspy-2.79.1/siriuspy/sofb/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/sofb/matrix.py` & `siriuspy-2.79.1/siriuspy/sofb/matrix.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/sofb/orbit.py` & `siriuspy-2.79.1/siriuspy/sofb/orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/sofb/utils.py` & `siriuspy-2.79.1/siriuspy/sofb/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/stabinfo/csdev.py` & `siriuspy-2.79.1/siriuspy/stabinfo/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/stabinfo/main.py` & `siriuspy-2.79.1/siriuspy/stabinfo/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/thread.py` & `siriuspy-2.79.1/siriuspy/thread.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/timesys/csdev.py` & `siriuspy-2.79.1/siriuspy/timesys/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/timesys/hl_classes.py` & `siriuspy-2.79.1/siriuspy/timesys/hl_classes.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/timesys/ll_classes.py` & `siriuspy-2.79.1/siriuspy/timesys/ll_classes.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/timesys/plot_network.py` & `siriuspy-2.79.1/siriuspy/timesys/plot_network.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/timesys/static_table.py` & `siriuspy-2.79.1/siriuspy/timesys/static_table.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy/util.py` & `siriuspy-2.79.1/siriuspy/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/siriuspy.egg-info/PKG-INFO` & `siriuspy-2.79.1/siriuspy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siriuspy
-Version: 2.79.0
+Version: 2.79.1
 Summary: Development packages for Sirius
 Home-page: https://github.com/lnls-sirius/dev-packages
 Download-URL: https://github.com/lnls-sirius/dev-packages
 Author: lnls-sirius
 License: GNU GPLv3
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `siriuspy-2.79.0/siriuspy.egg-info/SOURCES.txt` & `siriuspy-2.79.1/siriuspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/bsmp/test_bsmp.py` & `siriuspy-2.79.1/tests/bsmp/test_bsmp.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/bsmp/test_commands.py` & `siriuspy-2.79.1/tests/bsmp/test_commands.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/bsmp/test_entities.py` & `siriuspy-2.79.1/tests/bsmp/test_entities.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/bsmp/test_serial.py` & `siriuspy-2.79.1/tests/bsmp/test_serial.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/bsmp/test_types.py` & `siriuspy-2.79.1/tests/bsmp/test_types.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/clientconfigdb/test_configdb_client.py` & `siriuspy-2.79.1/tests/clientconfigdb/test_configdb_client.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/clientweb/test_implementation.py` & `siriuspy-2.79.1/tests/clientweb/test_implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/currinfo/lifetime/test_main.py` & `siriuspy-2.79.1/tests/currinfo/lifetime/test_main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/currinfo/test_csdev.py` & `siriuspy-2.79.1/tests/currinfo/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/currinfo/test_main.py` & `siriuspy-2.79.1/tests/currinfo/test_main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/magnet/test_factory.py` & `siriuspy-2.79.1/tests/magnet/test_factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/magnet/tests_normalizer.py` & `siriuspy-2.79.1/tests/magnet/tests_normalizer.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/mock_servweb.py` & `siriuspy-2.79.1/tests/mock_servweb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/namesys/test_implementation.py` & `siriuspy-2.79.1/tests/namesys/test_implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/opticscorr/test_chrom.py` & `siriuspy-2.79.1/tests/opticscorr/test_chrom.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/opticscorr/test_csdev.py` & `siriuspy-2.79.1/tests/opticscorr/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/opticscorr/test_opticscorr.py` & `siriuspy-2.79.1/tests/opticscorr/test_opticscorr.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/opticscorr/test_tune.py` & `siriuspy-2.79.1/tests/opticscorr/test_tune.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/opticscorr/test_utils.py` & `siriuspy-2.79.1/tests/opticscorr/test_utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/posang/test_csdev.py` & `siriuspy-2.79.1/tests/posang/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/posang/test_main.py` & `siriuspy-2.79.1/tests/posang/test_main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/pwrsupply/db.py` & `siriuspy-2.79.1/tests/pwrsupply/db.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/pwrsupply/pructrl/test_pru.py` & `siriuspy-2.79.1/tests/pwrsupply/pructrl/test_pru.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/pwrsupply/psctrl/test_pscwriters.py` & `siriuspy-2.79.1/tests/pwrsupply/psctrl/test_pscwriters.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/pwrsupply/test_csdev.py` & `siriuspy-2.79.1/tests/pwrsupply/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/pwrsupply/test_data.py` & `siriuspy-2.79.1/tests/pwrsupply/test_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/pwrsupply/test_siggen.py` & `siriuspy-2.79.1/tests/pwrsupply/test_siggen.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/pwrsupply/variables.py` & `siriuspy-2.79.1/tests/pwrsupply/variables.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/ramp/test_magnet.py` & `siriuspy-2.79.1/tests/ramp/test_magnet.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/ramp/test_waveform.py` & `siriuspy-2.79.1/tests/ramp/test_waveform.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/search/test_hl_time_search.py` & `siriuspy-2.79.1/tests/search/test_hl_time_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/search/test_init.py` & `siriuspy-2.79.1/tests/search/test_init.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/search/test_ll_time_search.py` & `siriuspy-2.79.1/tests/search/test_ll_time_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/search/test_ma_search.py` & `siriuspy-2.79.1/tests/search/test_ma_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/search/test_ps_search.py` & `siriuspy-2.79.1/tests/search/test_ps_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/test_callbacks.py` & `siriuspy-2.79.1/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/test_csdev.py` & `siriuspy-2.79.1/tests/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/test_envars.py` & `siriuspy-2.79.1/tests/test_envars.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/test_util.py` & `siriuspy-2.79.1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/timesys/test_csdev.py` & `siriuspy-2.79.1/tests/timesys/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.79.0/tests/timesys/test_plot_network.py` & `siriuspy-2.79.1/tests/timesys/test_plot_network.py`

 * *Files identical despite different names*

