# Comparing `tmp/omni_infer_api-0.0.1-py3-none-any.whl.zip` & `tmp/omni_infer_api-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 9362 bytes, number of entries: 20
--rw-rw-rw-  2.0 fat       81 b- defN 23-Jul-31 02:53 omniifer_api/__init__.py
+Zip file size: 9390 bytes, number of entries: 20
+-rw-rw-rw-  2.0 fat      122 b- defN 23-Aug-01 08:12 omniifer_api/__init__.py
 -rw-rw-rw-  2.0 fat       64 b- defN 23-Jul-30 01:10 omniifer_api/config.py
 -rw-rw-rw-  2.0 fat      181 b- defN 23-Jul-30 01:30 omniifer_api/error.py
 -rw-rw-rw-  2.0 fat       94 b- defN 23-Jul-31 07:03 omniifer_api/image_generate/__init__.py
 -rw-rw-rw-  2.0 fat     2717 b- defN 23-Jul-31 07:37 omniifer_api/image_generate/img2img.py
 -rw-rw-rw-  2.0 fat      720 b- defN 23-Jul-31 07:30 omniifer_api/image_generate/progress.py
--rw-rw-rw-  2.0 fat     3790 b- defN 23-Jul-31 05:57 omniifer_api/image_generate/txt2img.py
+-rw-rw-rw-  2.0 fat     3790 b- defN 23-Aug-01 08:12 omniifer_api/image_generate/txt2img.py
 -rw-rw-rw-  2.0 fat      176 b- defN 23-Jul-31 07:03 omniifer_api/model_list/__init__.py
 -rw-rw-rw-  2.0 fat      830 b- defN 23-Jul-31 07:37 omniifer_api/model_list/get_model.py
 -rw-rw-rw-  2.0 fat      438 b- defN 23-Jul-31 07:37 omniifer_api/model_list/get_models.py
 -rw-rw-rw-  2.0 fat      237 b- defN 23-Jul-31 07:35 omniifer_api/model_list/model_available.py
 -rw-rw-rw-  2.0 fat      716 b- defN 23-Jul-30 14:23 omniifer_api/model_list/put_model.py
 -rw-rw-rw-  2.0 fat     1250 b- defN 23-Jul-30 14:08 omniifer_api/model_list/search_models.py
 -rw-rw-rw-  2.0 fat      564 b- defN 23-Jul-30 14:23 omniifer_api/model_list/update.py
 -rw-rw-rw-  2.0 fat       33 b- defN 23-Jul-31 07:37 omniifer_api/tools/__init__.py
 -rw-rw-rw-  2.0 fat      307 b- defN 23-Jul-30 02:18 omniifer_api/tools/response_check.py
--rw-rw-rw-  2.0 fat      199 b- defN 23-Jul-31 08:37 omni_infer_api-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-31 08:37 omni_infer_api-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 23-Jul-31 08:37 omni_infer_api-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1766 b- defN 23-Jul-31 08:37 omni_infer_api-0.0.1.dist-info/RECORD
-20 files, 14268 bytes uncompressed, 6416 bytes compressed:  55.0%
+-rw-rw-rw-  2.0 fat      199 b- defN 23-Aug-01 08:14 omni_infer_api-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-01 08:14 omni_infer_api-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Aug-01 08:14 omni_infer_api-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1767 b- defN 23-Aug-01 08:14 omni_infer_api-0.0.2.dist-info/RECORD
+20 files, 14310 bytes uncompressed, 6444 bytes compressed:  55.0%
```

## zipnote {}

```diff
@@ -42,20 +42,20 @@
 
 Filename: omniifer_api/tools/__init__.py
 Comment: 
 
 Filename: omniifer_api/tools/response_check.py
 Comment: 
 
-Filename: omni_infer_api-0.0.1.dist-info/METADATA
+Filename: omni_infer_api-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: omni_infer_api-0.0.1.dist-info/WHEEL
+Filename: omni_infer_api-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: omni_infer_api-0.0.1.dist-info/top_level.txt
+Filename: omni_infer_api-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: omni_infer_api-0.0.1.dist-info/RECORD
+Filename: omni_infer_api-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## omniifer_api/__init__.py

```diff
@@ -1,3 +1,4 @@
 from .model_list import *
 from .config import *
 from .image_generate import *
+from .error import OMNI_INFER_API_ERROR
```

## omniifer_api/image_generate/txt2img.py

```diff
@@ -5,18 +5,18 @@
 from . import progress
 
 
 # controlnet_mask=-1 = don't use controlnet_mask
 # 返回task_id
 def txt2img(prompt: str, model_name: str, negative_prompt="", sampler_name="Euler a", batch_size=1, n_iter=1, steps=20
             , cfg_scale=7, seed=-1, height=512, width=512, restore_faces=False, clip_skip=2, using_controlnet=False
-            , controlnet_model="", controlnet_module="none", controlnet_weight=1.0, controlnet_input_image="base64", control_mode=0
-            , controlnet_mask=-1, controlnet_resize_mode=0, controlnet_lowvram=False, controlnet_processor_res=64
-            , controlnet_threshold_a=64, controlnet_threshold_b=64, controlnet_guidance_start=0.0
-            , controlnet_guidance_end=1.0, controlnet_pixel_perfect=False):
+            , controlnet_model="", controlnet_module="none", controlnet_weight=1.0, controlnet_input_image="base64"
+            , control_mode=0, controlnet_mask=-1, controlnet_resize_mode=0, controlnet_lowvram=False
+            , controlnet_processor_res=64, controlnet_threshold_a=64, controlnet_threshold_b=64
+            , controlnet_guidance_start=0.0, controlnet_guidance_end=1.0, controlnet_pixel_perfect=False):
     if not 1 <= batch_size <= 8:
         raise error.OMNI_INFER_API_ERROR("Error batch size: " + str(batch_size))
     if not 1 <= n_iter <= 8:
         raise error.OMNI_INFER_API_ERROR("Error n iter: " + str(n_iter))
     if not 1 <= steps <= 50:
         raise error.OMNI_INFER_API_ERROR("Error steps: " + str(steps))
     if not 1 <= cfg_scale <= 30:
```

## Comparing `omni_infer_api-0.0.1.dist-info/RECORD` & `omni_infer_api-0.0.2.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-omniifer_api/__init__.py,sha256=hrR8hFRlaIUWdylJlbqmsnSOjooM6ZNfAYlALBkFWkw,81
+omniifer_api/__init__.py,sha256=u0VFTki9sLh0vIMB7nFn2nL86ZNYFVJ72p2PkNccNjs,122
 omniifer_api/config.py,sha256=XQOwj3lkD7rK9NAhYqkuEmCiZ7TJOJUgIb-JiSrB7Ns,64
 omniifer_api/error.py,sha256=0vXK1xTR3KjXsYCcw9W3G4Wz9q5QEcsCRR1hfKA2gZk,181
 omniifer_api/image_generate/__init__.py,sha256=NBmouScnfMygwpFo0xX5Ezm4h0FZLKvQqEdnt1HvS_4,94
 omniifer_api/image_generate/img2img.py,sha256=cu8ZoVTc_8Xk2rVqBrrcKtedexGH5u-7BQb9L3bMACA,2717
 omniifer_api/image_generate/progress.py,sha256=sE3H1baRhisBMOFXTshwJV8smXUEAhF8v1qK2an-Kvo,720
-omniifer_api/image_generate/txt2img.py,sha256=wyjE4InF8E2FHg7T2FI1bQDM8D4uIa7asUxc1dwH4d8,3790
+omniifer_api/image_generate/txt2img.py,sha256=jr9x1hATq4L0Wv3f6n0IZJD51kxNAWd-L4mIgiQQI9k,3790
 omniifer_api/model_list/__init__.py,sha256=QH1XUsdx0lPb5meXsgAtaSoEID76eptJuzfRkv524I8,176
 omniifer_api/model_list/get_model.py,sha256=qY_kRyRaeNN2iig9eniFgPLBGYEY6fvhUhuT-jDJu64,830
 omniifer_api/model_list/get_models.py,sha256=2jHaTTS_7pPxCpAkB2NS-40BCYL8A_qxo667ViPxKdw,438
 omniifer_api/model_list/model_available.py,sha256=ldlVh9n5rakrhR9clAiuy-7NqoWikOcyTT5QvhoRfpU,237
 omniifer_api/model_list/put_model.py,sha256=gNeg3QTRG02qkZfT9QftWzljQnJwLgJerDxTksNAxsQ,716
 omniifer_api/model_list/search_models.py,sha256=fwQ-XdhK_jrIP0cJ_t_oOLyMrnPXh62CZAA6P0p7ST0,1250
 omniifer_api/model_list/update.py,sha256=h7gt3Vfwp4UScrGRSh4iGQCTB_wlfvR-YKpBMNpSx1o,564
 omniifer_api/tools/__init__.py,sha256=PbUs8cnYO79sGl1Y6zsKhOiZHHExEidiyrntyJ-aTDg,33
 omniifer_api/tools/response_check.py,sha256=PJbyxy5CXICZnRenoS1Qxyvp3vYzSOCAQSbUGqdTzJc,307
-omni_infer_api-0.0.1.dist-info/METADATA,sha256=i7cbz-vmrUm1yehABJOJQ4DFtNJBGW_c0u30T2WGHlo,199
-omni_infer_api-0.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-omni_infer_api-0.0.1.dist-info/top_level.txt,sha256=-5RhHKNFz5hCy5blJH5c-osZ5xLeU7Vk5unquKrtgIM,13
-omni_infer_api-0.0.1.dist-info/RECORD,,
+omni_infer_api-0.0.2.dist-info/METADATA,sha256=dqgSOSdcMY7AU00P83oRMvzWuwCpAsXjlSheXYohauk,199
+omni_infer_api-0.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+omni_infer_api-0.0.2.dist-info/top_level.txt,sha256=-5RhHKNFz5hCy5blJH5c-osZ5xLeU7Vk5unquKrtgIM,13
+omni_infer_api-0.0.2.dist-info/RECORD,,
```

