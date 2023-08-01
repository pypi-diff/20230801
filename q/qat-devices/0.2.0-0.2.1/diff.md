# Comparing `tmp/qat_devices-0.2.0-cp39-cp39-win_amd64.whl.zip` & `tmp/qat_devices-0.2.1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 513473 bytes, number of entries: 15
--rw-r--r--  2.0 unx        0 b- defN 22-Nov-04 21:27 qat/__init__.py
--rwxr-xr-x  2.0 unx   121577 b- defN 22-Nov-04 21:27 qat/devices/__init__.pyd
--rwxr-xr-x  2.0 unx   151962 b- defN 22-Nov-04 21:27 qat/devices/cas.pyd
--rwxr-xr-x  2.0 unx   236032 b- defN 22-Nov-04 21:27 qat/devices/common.pyd
--rwxr-xr-x  2.0 unx   164399 b- defN 22-Nov-04 21:27 qat/devices/google.pyd
--rwxr-xr-x  2.0 unx   292106 b- defN 22-Nov-04 21:27 qat/devices/ibm.pyd
--rwxr-xr-x  2.0 unx   159774 b- defN 22-Nov-04 21:27 qat/devices/rigetti.pyd
--rwxr-xr-x  2.0 unx   179436 b- defN 22-Nov-04 21:27 qat/devices/rydberg.pyd
--rwxr-xr-x  2.0 unx   142596 b- defN 22-Nov-04 21:27 qat/devices/util.pyd
--rwxr-xr-x  2.0 unx   109642 b- defN 22-Nov-04 21:27 qat/devices/version.pyd
--rw-r--r--  2.0 unx     4752 b- defN 22-Nov-04 21:27 qat_devices-0.2.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     1648 b- defN 22-Nov-04 21:27 qat_devices-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 22-Nov-04 21:27 qat_devices-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 22-Nov-04 21:27 qat_devices-0.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1204 b- defN 22-Nov-04 21:27 qat_devices-0.2.0.dist-info/RECORD
-15 files, 1565231 bytes uncompressed, 511525 bytes compressed:  67.3%
+Zip file size: 400529 bytes, number of entries: 15
+-rw-r--r--  2.0 unx       75 b- defN 23-Jul-31 22:42 qat/__init__.py
+-rwxr-xr-x  2.0 unx    85080 b- defN 23-Jul-31 22:42 qat/devices/__init__.pyd
+-rwxr-xr-x  2.0 unx   114930 b- defN 23-Jul-31 22:42 qat/devices/cas.pyd
+-rwxr-xr-x  2.0 unx   201415 b- defN 23-Jul-31 22:42 qat/devices/common.pyd
+-rwxr-xr-x  2.0 unx   126855 b- defN 23-Jul-31 22:42 qat/devices/google.pyd
+-rwxr-xr-x  2.0 unx   268896 b- defN 23-Jul-31 22:42 qat/devices/ibm.pyd
+-rwxr-xr-x  2.0 unx   126324 b- defN 23-Jul-31 22:42 qat/devices/rigetti.pyd
+-rwxr-xr-x  2.0 unx   145256 b- defN 23-Jul-31 22:42 qat/devices/rydberg.pyd
+-rwxr-xr-x  2.0 unx   106368 b- defN 23-Jul-31 22:42 qat/devices/util.pyd
+-rwxr-xr-x  2.0 unx    73122 b- defN 23-Jul-31 22:42 qat/devices/version.pyd
+-rw-r--r--  2.0 unx     4752 b- defN 23-Jul-31 22:42 qat_devices-0.2.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     1646 b- defN 23-Jul-31 22:42 qat_devices-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jul-31 22:42 qat_devices-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-Jul-31 22:42 qat_devices-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1203 b- defN 23-Jul-31 22:42 qat_devices-0.2.1.dist-info/RECORD
+15 files, 1256025 bytes uncompressed, 398581 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: qat/devices/util.pyd
 Comment: 
 
 Filename: qat/devices/version.pyd
 Comment: 
 
-Filename: qat_devices-0.2.0.dist-info/LICENSE.txt
+Filename: qat_devices-0.2.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: qat_devices-0.2.0.dist-info/METADATA
+Filename: qat_devices-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: qat_devices-0.2.0.dist-info/WHEEL
+Filename: qat_devices-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: qat_devices-0.2.0.dist-info/top_level.txt
+Filename: qat_devices-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: qat_devices-0.2.0.dist-info/RECORD
+Filename: qat_devices-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qat/__init__.py

```diff
@@ -0,0 +1,5 @@
+00000000: 6672 6f6d 2070 6b67 7574 696c 2069 6d70  from pkgutil imp
+00000010: 6f72 7420 6578 7465 6e64 5f70 6174 680a  ort extend_path.
+00000020: 5f5f 7061 7468 5f5f 203d 2065 7874 656e  __path__ = exten
+00000030: 645f 7061 7468 285f 5f70 6174 685f 5f2c  d_path(__path__,
+00000040: 205f 5f6e 616d 655f 5f29 0a               __name__).
```

## Comparing `qat_devices-0.2.0.dist-info/LICENSE.txt` & `qat_devices-0.2.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `qat_devices-0.2.0.dist-info/METADATA` & `qat_devices-0.2.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: qat-devices
-Version: 0.2.0
-Summary: Module qat-devices [0594fd5] - Compiled by Atos
+Version: 0.2.1
+Summary: Module qat-devices [0e91055] - Compiled by Atos
 Home-page: https://atos.net/en/lp/myqlm
 Author: Atos Quantum Lab
 Author-email: myqlm@atos.net
 License: Atos myQLM EULA
 Project-URL: Documentation, https://myqlm.github.io
 Project-URL: Bug Tracker, https://github.com/myQLM/myqlm-issues/issues
 Project-URL: Community, https://myqlmworkspace.slack.com
@@ -39,9 +39,7 @@
 
 ```
 pip install myqlm
 ```
 
 ## License
 [Atos myQLM EULA](https://myqlm.github.io/myqlm_specific/license.html#proprietary-part)
-
-
```

## Comparing `qat_devices-0.2.0.dist-info/RECORD` & `qat_devices-0.2.1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-qat/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-qat/devices/__init__.pyd,sha256=cjWPBgONA1GxR-m4uvcUzSMqyLajZlCONWPWRawSCEU,121577
-qat/devices/cas.pyd,sha256=4OK12FkB0J5vCVdQgc_2UovsL-qsgcTytj5ER_md40s,151962
-qat/devices/common.pyd,sha256=58faa_tg_Hv_M0UVRflxb8guOXY-g6c9gb-sBzNOnjA,236032
-qat/devices/google.pyd,sha256=HyFpfsgCJ_aTvu7ifUizWol-11rEZdEIyw3XTwAJcxM,164399
-qat/devices/ibm.pyd,sha256=f5s-BWgyvA60j7dGXTI4fRTdIpU8IKh2wJG_RaB9Qms,292106
-qat/devices/rigetti.pyd,sha256=onw5HLxLnfGflueeQ8qW6JlbELabU3RJtttlX8t6cJ8,159774
-qat/devices/rydberg.pyd,sha256=BZnvaAn8dNlON5_6e3uXv1UwIoDPSq_DnOpW2bFi5xM,179436
-qat/devices/util.pyd,sha256=n9xsEW4CNQDAu9SXS7NjYtb-fTPdsF2olfzD5gPQlQs,142596
-qat/devices/version.pyd,sha256=ypy7tzCpb5cyJ00kmon3L0-7z47d3XWNHbKzhaDHViM,109642
-qat_devices-0.2.0.dist-info/LICENSE.txt,sha256=Vl03FJBySK7FEYdw_Y0dV66UAVedEyIuqJTJxREyRgs,4752
-qat_devices-0.2.0.dist-info/METADATA,sha256=UfKXtddUngXrxtDMLzbNx-N3m0qpxerp_FFk3iTViio,1648
-qat_devices-0.2.0.dist-info/WHEEL,sha256=tt4lsxJnjXk2H9eLhI8bjAPrV2EafbzBfQ9L1C8sG4k,99
-qat_devices-0.2.0.dist-info/top_level.txt,sha256=EtiE-lzXpV6tDPK3leIRADd9p6cOal7g6fxvqQ-u_yc,4
-qat_devices-0.2.0.dist-info/RECORD,,
+qat/__init__.py,sha256=QDJyS5jtJnGFsSuOx43ZvLBCOrHImm8NrZk5f9URWdk,75
+qat/devices/__init__.pyd,sha256=P0QPHQo1q312wwJHvqJ4YzERUsEZarzbq3AG3T8zA94,85080
+qat/devices/cas.pyd,sha256=LPwPrqAhX3wo68o5NyXvsc-FE2lk6Pt-TqIyf4FEpqg,114930
+qat/devices/common.pyd,sha256=w0Z8ydsEJmeJeGYL8wnk_C4zSFDGwqkuxsU-EtEadxs,201415
+qat/devices/google.pyd,sha256=NT5YZB6bBmBrM7XJyO4Gbz-9lDV5NaqlQQD5VyGtMWU,126855
+qat/devices/ibm.pyd,sha256=-wumNQ391W0AEJQoAHwnwldNQ7q43BvAFz0_tR8JbRU,268896
+qat/devices/rigetti.pyd,sha256=OqAMot7CAAhUHrkDwTQwSF8VUURpv7NEvq5aRoa1bcE,126324
+qat/devices/rydberg.pyd,sha256=1WGg2Fgcce827ZBbwF9klCx9TMnyVRWmJKLbyRvICNA,145256
+qat/devices/util.pyd,sha256=bUqxI7GKrFOl1vxsSh1Ahp2yt3482p6XNkDorkQNDac,106368
+qat/devices/version.pyd,sha256=k0E561Bu1mB_7G40FoLRKWXqR9Tvx32yu7CEhnDuy7M,73122
+qat_devices-0.2.1.dist-info/LICENSE.txt,sha256=Vl03FJBySK7FEYdw_Y0dV66UAVedEyIuqJTJxREyRgs,4752
+qat_devices-0.2.1.dist-info/METADATA,sha256=UNWg7VVdwog5aTm3HFtBtxdNov-JEALQx_6iMx2P7eU,1646
+qat_devices-0.2.1.dist-info/WHEEL,sha256=afrrEnV2j93N2XVAju0ZvLCr9SJdI5iiSHnWAgTXSfQ,99
+qat_devices-0.2.1.dist-info/top_level.txt,sha256=EtiE-lzXpV6tDPK3leIRADd9p6cOal7g6fxvqQ-u_yc,4
+qat_devices-0.2.1.dist-info/RECORD,,
```

