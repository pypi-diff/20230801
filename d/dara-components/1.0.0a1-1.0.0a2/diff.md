# Comparing `tmp/dara_components-1.0.0a1-py3-none-any.whl.zip` & `tmp/dara_components-1.0.0a2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2976094 bytes, number of entries: 81
+Zip file size: 2976095 bytes, number of entries: 81
 -rw-r--r--  2.0 unx      808 b- defN 80-Jan-01 00:00 dara/components/__init__.py
 -rw-r--r--  2.0 unx     3866 b- defN 80-Jan-01 00:00 dara/components/common/__init__.py
 -rw-r--r--  2.0 unx     9446 b- defN 80-Jan-01 00:00 dara/components/common/accordion.py
 -rw-r--r--  2.0 unx     2869 b- defN 80-Jan-01 00:00 dara/components/common/anchor.py
 -rw-r--r--  2.0 unx     3827 b- defN 80-Jan-01 00:00 dara/components/common/base_component.py
 -rw-r--r--  2.0 unx     1433 b- defN 80-Jan-01 00:00 dara/components/common/bullet_list.py
 -rw-r--r--  2.0 unx     4684 b- defN 80-Jan-01 00:00 dara/components/common/button.py
@@ -72,12 +72,12 @@
 -rw-r--r--  2.0 unx     1315 b- defN 80-Jan-01 00:00 dara/components/smart/data_slicer/extension/filter_status_button.py
 -rw-r--r--  2.0 unx     8627 b- defN 80-Jan-01 00:00 dara/components/smart/data_slicer/utils/core.py
 -rw-r--r--  2.0 unx     1722 b- defN 80-Jan-01 00:00 dara/components/smart/data_slicer/utils/data_preview.py
 -rw-r--r--  2.0 unx     3313 b- defN 80-Jan-01 00:00 dara/components/smart/data_slicer/utils/plotting.py
 -rw-r--r--  2.0 unx     2877 b- defN 80-Jan-01 00:00 dara/components/smart/hierarchy.py
 -rw-r--r--  2.0 unx 16583252 b- defN 80-Jan-01 00:00 dara/components/umd/dara.components.umd.js
 -rw-r--r--  2.0 unx    23576 b- defN 80-Jan-01 00:00 dara/components/umd/style.css
--rw-r--r--  2.0 unx    10944 b- defN 80-Jan-01 00:00 dara_components-1.0.0a1.dist-info/LICENSE
--rw-r--r--  2.0 unx      955 b- defN 80-Jan-01 00:00 dara_components-1.0.0a1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 dara_components-1.0.0a1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     7691 b- defN 16-Jan-01 00:00 dara_components-1.0.0a1.dist-info/RECORD
-81 files, 16879859 bytes uncompressed, 2963648 bytes compressed:  82.4%
+-rw-r--r--  2.0 unx    10944 b- defN 80-Jan-01 00:00 dara_components-1.0.0a2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      955 b- defN 80-Jan-01 00:00 dara_components-1.0.0a2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 dara_components-1.0.0a2.dist-info/WHEEL
+?rw-r--r--  2.0 unx     7691 b- defN 16-Jan-01 00:00 dara_components-1.0.0a2.dist-info/RECORD
+81 files, 16879859 bytes uncompressed, 2963649 bytes compressed:  82.4%
```

## zipnote {}

```diff
@@ -225,20 +225,20 @@
 
 Filename: dara/components/umd/dara.components.umd.js
 Comment: 
 
 Filename: dara/components/umd/style.css
 Comment: 
 
-Filename: dara_components-1.0.0a1.dist-info/LICENSE
+Filename: dara_components-1.0.0a2.dist-info/LICENSE
 Comment: 
 
-Filename: dara_components-1.0.0a1.dist-info/METADATA
+Filename: dara_components-1.0.0a2.dist-info/METADATA
 Comment: 
 
-Filename: dara_components-1.0.0a1.dist-info/WHEEL
+Filename: dara_components-1.0.0a2.dist-info/WHEEL
 Comment: 
 
-Filename: dara_components-1.0.0a1.dist-info/RECORD
+Filename: dara_components-1.0.0a2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `dara_components-1.0.0a1.dist-info/LICENSE` & `dara_components-1.0.0a2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dara_components-1.0.0a1.dist-info/METADATA` & `dara_components-1.0.0a2.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: dara-components
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Components for the Dara Framework
 Home-page: https://dara.causalens.com/
 License: Apache-2.0
 Author: Patricia Jacob
 Author-email: patricia@causalens.com
 Requires-Python: >=3.8.0,<3.12.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bokeh (>=3.1.0,<3.2.0)
 Requires-Dist: cai-causal-graph (>=0.0.1)
-Requires-Dist: dara-core (==1.0.0-a.1)
+Requires-Dist: dara-core (==1.0.0-a.2)
 Requires-Dist: dill (>=0.3.0,<0.4.0)
 Requires-Dist: matplotlib (>=2.0.0)
 Requires-Dist: pandas (>=1.1.0,<3.0.0)
 Requires-Dist: plotly (>=5.14.0,<5.15.0)
 Requires-Dist: scipy
 Requires-Dist: seaborn (>=0.11.0)
 Project-URL: Repository, https://github.com/causalens/dara
```

## Comparing `dara_components-1.0.0a1.dist-info/RECORD` & `dara_components-1.0.0a2.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -71,11 +71,11 @@
 dara/components/smart/data_slicer/extension/filter_status_button.py,sha256=_IuwYk2oA6SSO_pZSarfgjNHV3a0aJekXU50r8B2ZwE,1315
 dara/components/smart/data_slicer/utils/core.py,sha256=ofoBkLSdcw3Rs_IX_hqI5OCtnsfKynOQpkRGtIWuujU,8627
 dara/components/smart/data_slicer/utils/data_preview.py,sha256=OAphjMrm3F76XmJ09X7sZSeOeKqGJFwN5ooo3qcyrG4,1722
 dara/components/smart/data_slicer/utils/plotting.py,sha256=JYzdQLXdAD0A8k2W-764xUr7zN0Ri5nf3OQ2Nb_iuiY,3313
 dara/components/smart/hierarchy.py,sha256=STkgyZiVB1c6KJtcKnn1r8lnjZAIrWkTCpZ_WCyCI1c,2877
 dara/components/umd/dara.components.umd.js,sha256=wN4NcwNyWTuGCSIdG7LbZ0Lo1mAqv5itByOd_C-f0lo,16583252
 dara/components/umd/style.css,sha256=cvNU48TRRp73QxBrE9awB-zm3YURFnFlASafeLTNa_U,23576
-dara_components-1.0.0a1.dist-info/LICENSE,sha256=r9u1w2RvpLMV6YjuXHIKXRBKzia3fx_roPwboGcLqCc,10944
-dara_components-1.0.0a1.dist-info/METADATA,sha256=hO5nCEYwerc13slYGw64cdXiWDfhDQ1MFPZAO-TnGZ8,955
-dara_components-1.0.0a1.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-dara_components-1.0.0a1.dist-info/RECORD,,
+dara_components-1.0.0a2.dist-info/LICENSE,sha256=r9u1w2RvpLMV6YjuXHIKXRBKzia3fx_roPwboGcLqCc,10944
+dara_components-1.0.0a2.dist-info/METADATA,sha256=R3qydt3vdzlN6xzJgsGqIOLBjZtQsxBzrEzbbHWljCU,955
+dara_components-1.0.0a2.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+dara_components-1.0.0a2.dist-info/RECORD,,
```

