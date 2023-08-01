# Comparing `tmp/mtgpu-0.7.202305021336-py3-none-any.whl.zip` & `tmp/mtgpu-0.7.202308011011-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 8298 bytes, number of entries: 14
--rw-rw-r--  2.0 unx     2510 b- defN 23-May-02 10:17 mt/gpu/__init__.py
+Zip file size: 8299 bytes, number of entries: 14
+-rw-rw-r--  2.0 unx     2515 b- defN 23-Aug-01 10:11 mt/gpu/__init__.py
 -rw-rw-r--  2.0 unx     3093 b- defN 23-May-02 10:39 mt/gpu/arch.py
 -rw-rw-r--  2.0 unx     1879 b- defN 22-Oct-04 12:51 mt/gpu/arch_amd64_amd.py
 -rw-rw-r--  2.0 unx      245 b- defN 22-Oct-04 12:51 mt/gpu/arch_amd64_cpu.py
 -rw-rw-r--  2.0 unx     1682 b- defN 22-Oct-04 12:51 mt/gpu/arch_amd64_nvidia.py
 -rw-rw-r--  2.0 unx      462 b- defN 22-Oct-04 12:51 mt/gpu/arch_rpi.py
 -rw-rw-r--  2.0 unx     2425 b- defN 23-May-02 13:36 mt/gpu/arch_tegra.py
--rw-rw-r--  2.0 unx      396 b- defN 23-May-02 13:36 mt/gpu/version.py
--rwxrwxr-x  2.0 unx       87 b- defN 23-May-02 13:36 mtgpu-0.7.202305021336.data/scripts/detect_machine
--rw-rw-r--  2.0 unx     1070 b- defN 23-May-02 13:36 mtgpu-0.7.202305021336.dist-info/LICENSE
--rw-rw-r--  2.0 unx      399 b- defN 23-May-02 13:36 mtgpu-0.7.202305021336.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-02 13:36 mtgpu-0.7.202305021336.dist-info/WHEEL
--rw-rw-r--  2.0 unx        3 b- defN 23-May-02 13:36 mtgpu-0.7.202305021336.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1149 b- defN 23-May-02 13:36 mtgpu-0.7.202305021336.dist-info/RECORD
-14 files, 15492 bytes uncompressed, 6380 bytes compressed:  58.8%
+-rw-rw-r--  2.0 unx      396 b- defN 23-Aug-01 10:11 mt/gpu/version.py
+-rwxrwxr-x  2.0 unx       87 b- defN 23-Aug-01 10:11 mtgpu-0.7.202308011011.data/scripts/detect_machine
+-rw-rw-r--  2.0 unx     1070 b- defN 23-Aug-01 10:11 mtgpu-0.7.202308011011.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      399 b- defN 23-Aug-01 10:11 mtgpu-0.7.202308011011.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Aug-01 10:11 mtgpu-0.7.202308011011.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        3 b- defN 23-Aug-01 10:11 mtgpu-0.7.202308011011.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1149 b- defN 23-Aug-01 10:11 mtgpu-0.7.202308011011.dist-info/RECORD
+14 files, 15497 bytes uncompressed, 6381 bytes compressed:  58.8%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: mt/gpu/arch_tegra.py
 Comment: 
 
 Filename: mt/gpu/version.py
 Comment: 
 
-Filename: mtgpu-0.7.202305021336.data/scripts/detect_machine
+Filename: mtgpu-0.7.202308011011.data/scripts/detect_machine
 Comment: 
 
-Filename: mtgpu-0.7.202305021336.dist-info/LICENSE
+Filename: mtgpu-0.7.202308011011.dist-info/LICENSE
 Comment: 
 
-Filename: mtgpu-0.7.202305021336.dist-info/METADATA
+Filename: mtgpu-0.7.202308011011.dist-info/METADATA
 Comment: 
 
-Filename: mtgpu-0.7.202305021336.dist-info/WHEEL
+Filename: mtgpu-0.7.202308011011.dist-info/WHEEL
 Comment: 
 
-Filename: mtgpu-0.7.202305021336.dist-info/top_level.txt
+Filename: mtgpu-0.7.202308011011.dist-info/top_level.txt
 Comment: 
 
-Filename: mtgpu-0.7.202305021336.dist-info/RECORD
+Filename: mtgpu-0.7.202308011011.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mt/gpu/__init__.py

```diff
@@ -37,15 +37,15 @@
         from .arch_tegra import get_mem_info_impl
 
         res = get_mem_info_impl(arch)
     elif arch == "unknown":
         res = None
 
     if print_bars and res:
-        from tqdm import tqdm
+        from tqdm.auto import tqdm
 
         MB = 1024 * 1024
 
         is_cgpu = res.get("cpu_mem_shared_with_gpu", False)
 
         cpu_desc = "cpu_gpu" if is_cgpu else "cpu"
         cpu_bar = tqdm(
```

## mt/gpu/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
-VERSION_MONTH = int('05')
-VERSION_DAY = int('02')
-VERSION_HOUR = int('13')
-VERSION_MINUTE = int('36')
+VERSION_MONTH = int('08')
+VERSION_DAY = int('01')
+VERSION_HOUR = int('10')
+VERSION_MINUTE = int('11')
 MAJOR_VERSION = 0
 MINOR_VERSION = 7
-PATCH_VERSION = 202305021336
-version_date = '2023/05/02 13:36'
+PATCH_VERSION = 202308011011
+version_date = '2023/08/01 10:11'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `mtgpu-0.7.202305021336.dist-info/LICENSE` & `mtgpu-0.7.202308011011.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mtgpu-0.7.202305021336.dist-info/RECORD` & `mtgpu-0.7.202308011011.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-mt/gpu/__init__.py,sha256=v5_zfaqe2WN2TNXqNieWg2UjcjVJ-b0uEt2l2XGm0Ek,2510
+mt/gpu/__init__.py,sha256=QdcjEy4QIluibfTnI9p8dAmlAcv_I4bf-y-T_QLesDA,2515
 mt/gpu/arch.py,sha256=dfbm41vRf4zX7HLZD3S_QvZtqT50HBe5wBkHG6gxdeQ,3093
 mt/gpu/arch_amd64_amd.py,sha256=tp7rkq9mtXK3_5u2Y93VCtHWnVtbv3uB9q0MIPrpXdg,1879
 mt/gpu/arch_amd64_cpu.py,sha256=wdavcOtmwgj0i6yWcdX1A3hzpwjOUJ1_9Yg3HcPJq6M,245
 mt/gpu/arch_amd64_nvidia.py,sha256=l5bZas2wik1FYFzK3GOyAPPZQ4Jwb9cY0dg4cliTZcQ,1682
 mt/gpu/arch_rpi.py,sha256=FHzifWhV1YijXMSN4PglMKuLD2bcnFOHVSYmWxZDg2g,462
 mt/gpu/arch_tegra.py,sha256=blQVFk7g5VcqzNNR0MqaIxzNzoJrLnyd0Twjw92RiCs,2425
-mt/gpu/version.py,sha256=i8kLhmp_Y2xtOmM_auOldZWWLOr134qsobwyA9BSdQk,396
-mtgpu-0.7.202305021336.data/scripts/detect_machine,sha256=7lX1WIVJNSZqsGpnHwJIp6C2EFWl_Ow74cBNc9uZQ0w,87
-mtgpu-0.7.202305021336.dist-info/LICENSE,sha256=PojkRlQzTT5Eg6Nj03XoIVEefN3u8iiIFf1p4rqe_t4,1070
-mtgpu-0.7.202305021336.dist-info/METADATA,sha256=O7n0RQ_AUDxfaIBV5q6JSyKvZ3gsUObpXXMMteMit5s,399
-mtgpu-0.7.202305021336.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-mtgpu-0.7.202305021336.dist-info/top_level.txt,sha256=WcqGFu9cV7iMZg09iam8eNxUvGpLSKKF2Iubf6SJVOo,3
-mtgpu-0.7.202305021336.dist-info/RECORD,,
+mt/gpu/version.py,sha256=BGHvQDOM1ZTL9a2Pd8oAKnH5YdwcrdFxBZ9EPYwS_-A,396
+mtgpu-0.7.202308011011.data/scripts/detect_machine,sha256=7lX1WIVJNSZqsGpnHwJIp6C2EFWl_Ow74cBNc9uZQ0w,87
+mtgpu-0.7.202308011011.dist-info/LICENSE,sha256=PojkRlQzTT5Eg6Nj03XoIVEefN3u8iiIFf1p4rqe_t4,1070
+mtgpu-0.7.202308011011.dist-info/METADATA,sha256=GmbN8hWKwiZ9k_buY-W93pcqDFHLAVxVHGTLyIrfhqM,399
+mtgpu-0.7.202308011011.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+mtgpu-0.7.202308011011.dist-info/top_level.txt,sha256=WcqGFu9cV7iMZg09iam8eNxUvGpLSKKF2Iubf6SJVOo,3
+mtgpu-0.7.202308011011.dist-info/RECORD,,
```

