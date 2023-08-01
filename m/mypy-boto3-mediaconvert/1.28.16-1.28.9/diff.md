# Comparing `tmp/mypy-boto3-mediaconvert-1.28.16.tar.gz` & `tmp/mypy-boto3-mediaconvert-1.28.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediaconvert-1.28.16.tar", last modified: Tue Aug  1 11:37:18 2023, max compression
+gzip compressed data, was "mypy-boto3-mediaconvert-1.28.9.tar", last modified: Fri Jul 21 20:32:58 2023, max compression
```

## Comparing `mypy-boto3-mediaconvert-1.28.16.tar` & `mypy-boto3-mediaconvert-1.28.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:18.468826 mypy-boto3-mediaconvert-1.28.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:23:44.000000 mypy-boto3-mediaconvert-1.28.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    34780 2023-08-01 11:37:18.456826 mypy-boto3-mediaconvert-1.28.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    33276 2023-08-01 11:23:44.000000 mypy-boto3-mediaconvert-1.28.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:18.452826 mypy-boto3-mediaconvert-1.28.16/mypy_boto3_mediaconvert/
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-08-01 11:23:44.000000 mypy-boto3-mediaconvert-1.28.16/mypy_boto3_mediaconvert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-01 11:23:44.000000 mypy-boto3-mediaconvert-1.28.16/mypy_boto3_mediaconvert/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-01 11:23:44.000000 mypy-boto3-mediaconvert-1.28.16/mypy_boto3_mediaconvert/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22553 2023-08-01 11:23:45.000000 mypy-boto3-mediaconvert-1.28.16/mypy_boto3_mediaconvert/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22513 2023-08-01 11:23:44.000000 mypy-boto3-mediaconvert-1.28.16/mypy_boto3_mediaconvert/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    55606 2023-08-01 11:23:46.000000 mypy-boto3-mediaconvert-1.28.16/mypy_boto3_mediaconvert/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    55604 2023-08-01 11:23:45.000000 mypy-boto3-mediaconvert-1.28.16/mypy_boto3_mediaconvert/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-08-01 11:23:45.000000 mypy-boto3-mediaconvert-1.28.16/mypy_boto3_mediaconvert/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-08-01 11:23:45.000000 mypy-boto3-mediaconvert-1.28.16/mypy_boto3_mediaconvert/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:23:44.000000 mypy-boto3-mediaconvert-1.28.16/mypy_boto3_mediaconvert/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   127144 2023-08-01 11:23:52.000000 mypy-boto3-mediaconvert-1.28.16/mypy_boto3_mediaconvert/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   127119 2023-08-01 11:23:50.000000 mypy-boto3-mediaconvert-1.28.16/mypy_boto3_mediaconvert/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:23:44.000000 mypy-boto3-mediaconvert-1.28.16/mypy_boto3_mediaconvert/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:18.456826 mypy-boto3-mediaconvert-1.28.16/mypy_boto3_mediaconvert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    34780 2023-08-01 11:37:18.000000 mypy-boto3-mediaconvert-1.28.16/mypy_boto3_mediaconvert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-01 11:37:18.000000 mypy-boto3-mediaconvert-1.28.16/mypy_boto3_mediaconvert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:18.000000 mypy-boto3-mediaconvert-1.28.16/mypy_boto3_mediaconvert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:18.000000 mypy-boto3-mediaconvert-1.28.16/mypy_boto3_mediaconvert.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:18.000000 mypy-boto3-mediaconvert-1.28.16/mypy_boto3_mediaconvert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 11:37:18.000000 mypy-boto3-mediaconvert-1.28.16/mypy_boto3_mediaconvert.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:18.468826 mypy-boto3-mediaconvert-1.28.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-01 11:23:44.000000 mypy-boto3-mediaconvert-1.28.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:58.227903 mypy-boto3-mediaconvert-1.28.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    39103 2023-07-21 20:32:58.223902 mypy-boto3-mediaconvert-1.28.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    37598 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:58.223902 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22513 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22473 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    55551 2023-07-21 20:32:30.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55549 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   171396 2023-07-21 20:32:34.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   171379 2023-07-21 20:32:31.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:58.223902 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    39103 2023-07-21 20:32:58.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-21 20:32:58.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:32:58.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:32:58.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-21 20:32:58.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-21 20:32:58.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 20:32:58.227903 mypy-boto3-mediaconvert-1.28.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-21 20:32:27.000000 mypy-boto3-mediaconvert-1.28.9/setup.py
```

### Comparing `mypy-boto3-mediaconvert-1.28.16/LICENSE` & `mypy-boto3-mediaconvert-1.28.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.28.16/PKG-INFO` & `mypy-boto3-mediaconvert-1.28.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-mediaconvert
-Version: 1.28.16
-Summary: Type annotations for boto3.MediaConvert 1.28.16 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 mediaconvert type-annotations botocore mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-mediaconvert"></a>
 
 # mypy-boto3-mediaconvert
 
 [![PyPI - mypy-boto3-mediaconvert](https://img.shields.io/pypi/v/mypy-boto3-mediaconvert.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconvert)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediaconvert.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconvert)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediaconvert)](https://pepy.tech/project/mypy-boto3-mediaconvert)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediaconvert?color=blue)](https://pypistats.org/packages/mypy-boto3-mediaconvert)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaConvert 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
+[boto3.MediaConvert 1.28.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-mediaconvert docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +42,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
-    - [Type definitions](#type-definitions)
+    - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -734,180 +702,281 @@
 )
 
 
 def check_value(value: AacAudioDescriptionBroadcasterMixType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_mediaconvert.type_defs` module contains structures and shapes
-assembled to typed dictionaries and unions for additional type checking.
+assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediaconvert.type_defs import (
+    AacSettingsOutputTypeDef,
     AacSettingsTypeDef,
+    Ac3SettingsOutputTypeDef,
     Ac3SettingsTypeDef,
+    AccelerationSettingsOutputTypeDef,
     AccelerationSettingsTypeDef,
+    AdvancedInputFilterSettingsOutputTypeDef,
     AdvancedInputFilterSettingsTypeDef,
+    AiffSettingsOutputTypeDef,
     AiffSettingsTypeDef,
+    AllowedRenditionSizeOutputTypeDef,
     AllowedRenditionSizeTypeDef,
+    AncillarySourceSettingsOutputTypeDef,
     AncillarySourceSettingsTypeDef,
     AssociateCertificateRequestRequestTypeDef,
+    AudioChannelTaggingSettingsOutputTypeDef,
     AudioChannelTaggingSettingsTypeDef,
+    Eac3AtmosSettingsOutputTypeDef,
+    Eac3SettingsOutputTypeDef,
+    Mp2SettingsOutputTypeDef,
+    Mp3SettingsOutputTypeDef,
+    OpusSettingsOutputTypeDef,
+    VorbisSettingsOutputTypeDef,
+    WavSettingsOutputTypeDef,
     Eac3AtmosSettingsTypeDef,
     Eac3SettingsTypeDef,
     Mp2SettingsTypeDef,
     Mp3SettingsTypeDef,
     OpusSettingsTypeDef,
     VorbisSettingsTypeDef,
     WavSettingsTypeDef,
+    AudioNormalizationSettingsOutputTypeDef,
     AudioNormalizationSettingsTypeDef,
     AudioSelectorGroupOutputTypeDef,
     AudioSelectorGroupTypeDef,
+    HlsRenditionGroupSettingsOutputTypeDef,
     HlsRenditionGroupSettingsTypeDef,
+    ForceIncludeRenditionSizeOutputTypeDef,
+    MinBottomRenditionSizeOutputTypeDef,
+    MinTopRenditionSizeOutputTypeDef,
     ForceIncludeRenditionSizeTypeDef,
     MinBottomRenditionSizeTypeDef,
     MinTopRenditionSizeTypeDef,
+    Av1QvbrSettingsOutputTypeDef,
     Av1QvbrSettingsTypeDef,
+    AvailBlankingOutputTypeDef,
     AvailBlankingTypeDef,
+    AvcIntraUhdSettingsOutputTypeDef,
     AvcIntraUhdSettingsTypeDef,
+    BandwidthReductionFilterOutputTypeDef,
     BandwidthReductionFilterTypeDef,
+    BurninDestinationSettingsOutputTypeDef,
     BurninDestinationSettingsTypeDef,
     CancelJobRequestRequestTypeDef,
+    DvbSubDestinationSettingsOutputTypeDef,
+    EmbeddedDestinationSettingsOutputTypeDef,
+    ImscDestinationSettingsOutputTypeDef,
+    SccDestinationSettingsOutputTypeDef,
+    SrtDestinationSettingsOutputTypeDef,
+    TeletextDestinationSettingsOutputTypeDef,
+    TtmlDestinationSettingsOutputTypeDef,
+    WebvttDestinationSettingsOutputTypeDef,
     DvbSubDestinationSettingsTypeDef,
     EmbeddedDestinationSettingsTypeDef,
     ImscDestinationSettingsTypeDef,
     SccDestinationSettingsTypeDef,
     SrtDestinationSettingsTypeDef,
-    TeletextDestinationSettingsOutputTypeDef,
+    TeletextDestinationSettingsTypeDef,
     TtmlDestinationSettingsTypeDef,
     WebvttDestinationSettingsTypeDef,
-    TeletextDestinationSettingsTypeDef,
+    CaptionSourceFramerateOutputTypeDef,
     CaptionSourceFramerateTypeDef,
+    DvbSubSourceSettingsOutputTypeDef,
+    EmbeddedSourceSettingsOutputTypeDef,
+    TeletextSourceSettingsOutputTypeDef,
+    TrackSourceSettingsOutputTypeDef,
+    WebvttHlsSourceSettingsOutputTypeDef,
     DvbSubSourceSettingsTypeDef,
     EmbeddedSourceSettingsTypeDef,
     TeletextSourceSettingsTypeDef,
     TrackSourceSettingsTypeDef,
     WebvttHlsSourceSettingsTypeDef,
     OutputChannelMappingOutputTypeDef,
     OutputChannelMappingTypeDef,
+    ClipLimitsOutputTypeDef,
     ClipLimitsTypeDef,
     CmafAdditionalManifestOutputTypeDef,
     CmafAdditionalManifestTypeDef,
     SpekeKeyProviderCmafOutputTypeDef,
-    StaticKeyProviderTypeDef,
+    StaticKeyProviderOutputTypeDef,
     SpekeKeyProviderCmafTypeDef,
+    StaticKeyProviderTypeDef,
+    CmafImageBasedTrickPlaySettingsOutputTypeDef,
     CmafImageBasedTrickPlaySettingsTypeDef,
+    CmfcSettingsOutputTypeDef,
     CmfcSettingsTypeDef,
+    Hdr10MetadataOutputTypeDef,
     Hdr10MetadataTypeDef,
-    F4vSettingsTypeDef,
+    F4vSettingsOutputTypeDef,
     M3u8SettingsOutputTypeDef,
+    MovSettingsOutputTypeDef,
+    Mp4SettingsOutputTypeDef,
+    MpdSettingsOutputTypeDef,
+    F4vSettingsTypeDef,
+    M3u8SettingsTypeDef,
     MovSettingsTypeDef,
     Mp4SettingsTypeDef,
     MpdSettingsTypeDef,
-    M3u8SettingsTypeDef,
     HopDestinationTypeDef,
     ResponseMetadataTypeDef,
     ReservationPlanSettingsTypeDef,
     DashAdditionalManifestOutputTypeDef,
     DashAdditionalManifestTypeDef,
     SpekeKeyProviderOutputTypeDef,
     SpekeKeyProviderTypeDef,
+    DashIsoImageBasedTrickPlaySettingsOutputTypeDef,
     DashIsoImageBasedTrickPlaySettingsTypeDef,
+    DeinterlacerOutputTypeDef,
     DeinterlacerTypeDef,
     DeleteJobTemplateRequestRequestTypeDef,
     DeletePresetRequestRequestTypeDef,
     DeleteQueueRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeEndpointsRequestRequestTypeDef,
     EndpointTypeDef,
     DisassociateCertificateRequestRequestTypeDef,
+    DolbyVisionLevel6MetadataOutputTypeDef,
     DolbyVisionLevel6MetadataTypeDef,
+    DvbNitSettingsOutputTypeDef,
     DvbNitSettingsTypeDef,
+    DvbSdtSettingsOutputTypeDef,
     DvbSdtSettingsTypeDef,
+    DvbTdtSettingsOutputTypeDef,
     DvbTdtSettingsTypeDef,
+    EsamManifestConfirmConditionNotificationOutputTypeDef,
     EsamManifestConfirmConditionNotificationTypeDef,
+    EsamSignalProcessingNotificationOutputTypeDef,
     EsamSignalProcessingNotificationTypeDef,
+    ExtendedDataServicesOutputTypeDef,
     ExtendedDataServicesTypeDef,
+    FrameCaptureSettingsOutputTypeDef,
     FrameCaptureSettingsTypeDef,
     GetJobRequestRequestTypeDef,
     GetJobTemplateRequestRequestTypeDef,
-    PolicyTypeDef,
+    PolicyOutputTypeDef,
     GetPresetRequestRequestTypeDef,
     GetQueueRequestRequestTypeDef,
+    H264QvbrSettingsOutputTypeDef,
     H264QvbrSettingsTypeDef,
+    H265QvbrSettingsOutputTypeDef,
     H265QvbrSettingsTypeDef,
+    Hdr10PlusOutputTypeDef,
     Hdr10PlusTypeDef,
     HlsAdditionalManifestOutputTypeDef,
     HlsAdditionalManifestTypeDef,
+    HlsCaptionLanguageMappingOutputTypeDef,
     HlsCaptionLanguageMappingTypeDef,
+    HlsImageBasedTrickPlaySettingsOutputTypeDef,
     HlsImageBasedTrickPlaySettingsTypeDef,
-    HlsSettingsTypeDef,
+    HlsSettingsOutputTypeDef,
+    HopDestinationOutputTypeDef,
+    Id3InsertionOutputTypeDef,
     Id3InsertionTypeDef,
+    InsertableImageOutputTypeDef,
     InsertableImageTypeDef,
+    InputClippingOutputTypeDef,
     InputClippingTypeDef,
+    InputDecryptionSettingsOutputTypeDef,
     InputDecryptionSettingsTypeDef,
-    InputVideoGeneratorTypeDef,
+    InputVideoGeneratorOutputTypeDef,
+    RectangleOutputTypeDef,
     RectangleTypeDef,
+    InputVideoGeneratorTypeDef,
     JobMessagesTypeDef,
+    KantarWatermarkSettingsOutputTypeDef,
+    NielsenConfigurationOutputTypeDef,
+    NielsenNonLinearWatermarkSettingsOutputTypeDef,
+    TimecodeConfigOutputTypeDef,
     KantarWatermarkSettingsTypeDef,
     NielsenConfigurationTypeDef,
     NielsenNonLinearWatermarkSettingsTypeDef,
     TimecodeConfigTypeDef,
     QueueTransitionTypeDef,
     TimingTypeDef,
     WarningGroupTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListPresetsRequestRequestTypeDef,
     ListQueuesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ResourceTagsTypeDef,
+    M2tsScte35EsamOutputTypeDef,
     M2tsScte35EsamTypeDef,
+    MotionImageInsertionFramerateOutputTypeDef,
+    MotionImageInsertionOffsetOutputTypeDef,
     MotionImageInsertionFramerateTypeDef,
     MotionImageInsertionOffsetTypeDef,
+    Mpeg2SettingsOutputTypeDef,
     Mpeg2SettingsTypeDef,
     MsSmoothAdditionalManifestOutputTypeDef,
     MsSmoothAdditionalManifestTypeDef,
+    MxfXavcProfileSettingsOutputTypeDef,
     MxfXavcProfileSettingsTypeDef,
+    NexGuardFileMarkerSettingsOutputTypeDef,
     NexGuardFileMarkerSettingsTypeDef,
+    NoiseReducerFilterSettingsOutputTypeDef,
     NoiseReducerFilterSettingsTypeDef,
+    NoiseReducerSpatialFilterSettingsOutputTypeDef,
+    NoiseReducerTemporalFilterSettingsOutputTypeDef,
     NoiseReducerSpatialFilterSettingsTypeDef,
     NoiseReducerTemporalFilterSettingsTypeDef,
     VideoDetailTypeDef,
+    PolicyTypeDef,
+    ProresSettingsOutputTypeDef,
     ProresSettingsTypeDef,
     ReservationPlanTypeDef,
+    S3DestinationAccessControlOutputTypeDef,
     S3DestinationAccessControlTypeDef,
+    S3EncryptionSettingsOutputTypeDef,
     S3EncryptionSettingsTypeDef,
     TagResourceRequestRequestTypeDef,
+    TimecodeBurninOutputTypeDef,
     TimecodeBurninTypeDef,
     UntagResourceRequestRequestTypeDef,
+    Vc3SettingsOutputTypeDef,
     Vc3SettingsTypeDef,
+    Vp8SettingsOutputTypeDef,
+    Vp9SettingsOutputTypeDef,
     Vp8SettingsTypeDef,
     Vp9SettingsTypeDef,
+    Xavc4kIntraCbgProfileSettingsOutputTypeDef,
     Xavc4kIntraCbgProfileSettingsTypeDef,
+    Xavc4kIntraVbrProfileSettingsOutputTypeDef,
     Xavc4kIntraVbrProfileSettingsTypeDef,
+    Xavc4kProfileSettingsOutputTypeDef,
     Xavc4kProfileSettingsTypeDef,
+    XavcHdIntraCbgProfileSettingsOutputTypeDef,
     XavcHdIntraCbgProfileSettingsTypeDef,
+    XavcHdProfileSettingsOutputTypeDef,
     XavcHdProfileSettingsTypeDef,
+    AudioCodecSettingsOutputTypeDef,
     AudioCodecSettingsTypeDef,
     AutomatedAbrRuleOutputTypeDef,
     AutomatedAbrRuleTypeDef,
+    Av1SettingsOutputTypeDef,
     Av1SettingsTypeDef,
+    AvcIntraSettingsOutputTypeDef,
     AvcIntraSettingsTypeDef,
     CaptionDestinationSettingsOutputTypeDef,
     CaptionDestinationSettingsTypeDef,
+    FileSourceSettingsOutputTypeDef,
     FileSourceSettingsTypeDef,
     ChannelMappingOutputTypeDef,
     ChannelMappingTypeDef,
     CmafEncryptionSettingsOutputTypeDef,
     CmafEncryptionSettingsTypeDef,
+    ColorCorrectorOutputTypeDef,
+    VideoSelectorOutputTypeDef,
     ColorCorrectorTypeDef,
     VideoSelectorTypeDef,
     CreateQueueRequestRequestTypeDef,
     UpdateQueueRequestRequestTypeDef,
     DashIsoEncryptionSettingsOutputTypeDef,
     HlsEncryptionSettingsOutputTypeDef,
     MsSmoothEncryptionSettingsOutputTypeDef,
@@ -916,115 +985,127 @@
     MsSmoothEncryptionSettingsTypeDef,
     DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef,
     ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
     ListPresetsRequestListPresetsPaginateTypeDef,
     ListQueuesRequestListQueuesPaginateTypeDef,
     DescribeEndpointsResponseTypeDef,
+    DolbyVisionOutputTypeDef,
     DolbyVisionTypeDef,
+    EsamSettingsOutputTypeDef,
     EsamSettingsTypeDef,
     GetPolicyResponseTypeDef,
-    PutPolicyRequestRequestTypeDef,
     PutPolicyResponseTypeDef,
+    H264SettingsOutputTypeDef,
     H264SettingsTypeDef,
+    H265SettingsOutputTypeDef,
     H265SettingsTypeDef,
-    OutputSettingsTypeDef,
+    OutputSettingsOutputTypeDef,
     TimedMetadataInsertionOutputTypeDef,
     TimedMetadataInsertionTypeDef,
     ImageInserterOutputTypeDef,
     ImageInserterTypeDef,
     ListTagsForResourceResponseTypeDef,
     M2tsSettingsOutputTypeDef,
     M2tsSettingsTypeDef,
+    MotionImageInserterOutputTypeDef,
     MotionImageInserterTypeDef,
+    MxfSettingsOutputTypeDef,
     MxfSettingsTypeDef,
+    PartnerWatermarkingOutputTypeDef,
     PartnerWatermarkingTypeDef,
+    NoiseReducerOutputTypeDef,
     NoiseReducerTypeDef,
     OutputDetailTypeDef,
+    PutPolicyRequestRequestTypeDef,
     QueueTypeDef,
+    S3DestinationSettingsOutputTypeDef,
     S3DestinationSettingsTypeDef,
+    XavcSettingsOutputTypeDef,
     XavcSettingsTypeDef,
     AutomatedAbrSettingsOutputTypeDef,
     AutomatedAbrSettingsTypeDef,
+    CaptionDescriptionOutputTypeDef,
     CaptionDescriptionPresetOutputTypeDef,
     CaptionDescriptionPresetTypeDef,
-    CaptionDescriptionTypeDef,
+    CaptionSourceSettingsOutputTypeDef,
     CaptionSourceSettingsTypeDef,
     RemixSettingsOutputTypeDef,
     RemixSettingsTypeDef,
     ContainerSettingsOutputTypeDef,
     ContainerSettingsTypeDef,
     VideoPreprocessorOutputTypeDef,
     VideoPreprocessorTypeDef,
     OutputGroupDetailTypeDef,
     CreateQueueResponseTypeDef,
     GetQueueResponseTypeDef,
     ListQueuesResponseTypeDef,
     UpdateQueueResponseTypeDef,
+    DestinationSettingsOutputTypeDef,
     DestinationSettingsTypeDef,
+    VideoCodecSettingsOutputTypeDef,
     VideoCodecSettingsTypeDef,
     AutomatedEncodingSettingsOutputTypeDef,
     AutomatedEncodingSettingsTypeDef,
+    CaptionSelectorOutputTypeDef,
     CaptionSelectorTypeDef,
     AudioDescriptionOutputTypeDef,
     AudioSelectorOutputTypeDef,
     AudioDescriptionTypeDef,
     AudioSelectorTypeDef,
     CmafGroupSettingsOutputTypeDef,
-    CmafGroupSettingsTypeDef,
     DashIsoGroupSettingsOutputTypeDef,
+    FileGroupSettingsOutputTypeDef,
+    HlsGroupSettingsOutputTypeDef,
+    MsSmoothGroupSettingsOutputTypeDef,
+    CmafGroupSettingsTypeDef,
     DashIsoGroupSettingsTypeDef,
     FileGroupSettingsTypeDef,
-    HlsGroupSettingsOutputTypeDef,
     HlsGroupSettingsTypeDef,
-    MsSmoothGroupSettingsOutputTypeDef,
     MsSmoothGroupSettingsTypeDef,
     VideoDescriptionOutputTypeDef,
     VideoDescriptionTypeDef,
     InputOutputTypeDef,
     InputTemplateOutputTypeDef,
     InputTemplateTypeDef,
     InputTypeDef,
     OutputGroupSettingsOutputTypeDef,
     OutputGroupSettingsTypeDef,
-    PresetSettingsOutputTypeDef,
     OutputTypeDef,
+    PresetSettingsOutputTypeDef,
     PresetSettingsTypeDef,
-    PresetTypeDef,
     OutputGroupOutputTypeDef,
     OutputGroupTypeDef,
+    PresetTypeDef,
     CreatePresetRequestRequestTypeDef,
-    PresetSettingsUnionTypeDef,
     UpdatePresetRequestRequestTypeDef,
-    CreatePresetResponseTypeDef,
-    GetPresetResponseTypeDef,
-    ListPresetsResponseTypeDef,
-    UpdatePresetResponseTypeDef,
     JobSettingsOutputTypeDef,
     JobTemplateSettingsOutputTypeDef,
     JobSettingsTypeDef,
     JobTemplateSettingsTypeDef,
+    CreatePresetResponseTypeDef,
+    GetPresetResponseTypeDef,
+    ListPresetsResponseTypeDef,
+    UpdatePresetResponseTypeDef,
     JobTypeDef,
     JobTemplateTypeDef,
     CreateJobRequestRequestTypeDef,
-    JobSettingsUnionTypeDef,
     CreateJobTemplateRequestRequestTypeDef,
-    JobTemplateSettingsUnionTypeDef,
     UpdateJobTemplateRequestRequestTypeDef,
     CreateJobResponseTypeDef,
     GetJobResponseTypeDef,
     ListJobsResponseTypeDef,
     CreateJobTemplateResponseTypeDef,
     GetJobTemplateResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
     UpdateJobTemplateResponseTypeDef,
 )
 
 
-def get_value() -> AacSettingsTypeDef:
+def get_structure() -> AacSettingsOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mediaconvert-1.28.16/README.md` & `mypy-boto3-mediaconvert-1.28.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-mediaconvert
+Version: 1.28.9
+Summary: Type annotations for boto3.MediaConvert 1.28.9 service generated with mypy-boto3-builder 7.15.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 mediaconvert type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-mediaconvert"></a>
 
 # mypy-boto3-mediaconvert
 
 [![PyPI - mypy-boto3-mediaconvert](https://img.shields.io/pypi/v/mypy-boto3-mediaconvert.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconvert)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediaconvert.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconvert)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediaconvert)](https://pepy.tech/project/mypy-boto3-mediaconvert)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediaconvert?color=blue)](https://pypistats.org/packages/mypy-boto3-mediaconvert)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaConvert 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
+[boto3.MediaConvert 1.28.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-mediaconvert docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/).
 
 See how it helps to find and fix potential bugs:
 
@@ -42,15 +74,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
-    - [Type definitions](#type-definitions)
+    - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -702,180 +734,281 @@
 )
 
 
 def check_value(value: AacAudioDescriptionBroadcasterMixType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_mediaconvert.type_defs` module contains structures and shapes
-assembled to typed dictionaries and unions for additional type checking.
+assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediaconvert.type_defs import (
+    AacSettingsOutputTypeDef,
     AacSettingsTypeDef,
+    Ac3SettingsOutputTypeDef,
     Ac3SettingsTypeDef,
+    AccelerationSettingsOutputTypeDef,
     AccelerationSettingsTypeDef,
+    AdvancedInputFilterSettingsOutputTypeDef,
     AdvancedInputFilterSettingsTypeDef,
+    AiffSettingsOutputTypeDef,
     AiffSettingsTypeDef,
+    AllowedRenditionSizeOutputTypeDef,
     AllowedRenditionSizeTypeDef,
+    AncillarySourceSettingsOutputTypeDef,
     AncillarySourceSettingsTypeDef,
     AssociateCertificateRequestRequestTypeDef,
+    AudioChannelTaggingSettingsOutputTypeDef,
     AudioChannelTaggingSettingsTypeDef,
+    Eac3AtmosSettingsOutputTypeDef,
+    Eac3SettingsOutputTypeDef,
+    Mp2SettingsOutputTypeDef,
+    Mp3SettingsOutputTypeDef,
+    OpusSettingsOutputTypeDef,
+    VorbisSettingsOutputTypeDef,
+    WavSettingsOutputTypeDef,
     Eac3AtmosSettingsTypeDef,
     Eac3SettingsTypeDef,
     Mp2SettingsTypeDef,
     Mp3SettingsTypeDef,
     OpusSettingsTypeDef,
     VorbisSettingsTypeDef,
     WavSettingsTypeDef,
+    AudioNormalizationSettingsOutputTypeDef,
     AudioNormalizationSettingsTypeDef,
     AudioSelectorGroupOutputTypeDef,
     AudioSelectorGroupTypeDef,
+    HlsRenditionGroupSettingsOutputTypeDef,
     HlsRenditionGroupSettingsTypeDef,
+    ForceIncludeRenditionSizeOutputTypeDef,
+    MinBottomRenditionSizeOutputTypeDef,
+    MinTopRenditionSizeOutputTypeDef,
     ForceIncludeRenditionSizeTypeDef,
     MinBottomRenditionSizeTypeDef,
     MinTopRenditionSizeTypeDef,
+    Av1QvbrSettingsOutputTypeDef,
     Av1QvbrSettingsTypeDef,
+    AvailBlankingOutputTypeDef,
     AvailBlankingTypeDef,
+    AvcIntraUhdSettingsOutputTypeDef,
     AvcIntraUhdSettingsTypeDef,
+    BandwidthReductionFilterOutputTypeDef,
     BandwidthReductionFilterTypeDef,
+    BurninDestinationSettingsOutputTypeDef,
     BurninDestinationSettingsTypeDef,
     CancelJobRequestRequestTypeDef,
+    DvbSubDestinationSettingsOutputTypeDef,
+    EmbeddedDestinationSettingsOutputTypeDef,
+    ImscDestinationSettingsOutputTypeDef,
+    SccDestinationSettingsOutputTypeDef,
+    SrtDestinationSettingsOutputTypeDef,
+    TeletextDestinationSettingsOutputTypeDef,
+    TtmlDestinationSettingsOutputTypeDef,
+    WebvttDestinationSettingsOutputTypeDef,
     DvbSubDestinationSettingsTypeDef,
     EmbeddedDestinationSettingsTypeDef,
     ImscDestinationSettingsTypeDef,
     SccDestinationSettingsTypeDef,
     SrtDestinationSettingsTypeDef,
-    TeletextDestinationSettingsOutputTypeDef,
+    TeletextDestinationSettingsTypeDef,
     TtmlDestinationSettingsTypeDef,
     WebvttDestinationSettingsTypeDef,
-    TeletextDestinationSettingsTypeDef,
+    CaptionSourceFramerateOutputTypeDef,
     CaptionSourceFramerateTypeDef,
+    DvbSubSourceSettingsOutputTypeDef,
+    EmbeddedSourceSettingsOutputTypeDef,
+    TeletextSourceSettingsOutputTypeDef,
+    TrackSourceSettingsOutputTypeDef,
+    WebvttHlsSourceSettingsOutputTypeDef,
     DvbSubSourceSettingsTypeDef,
     EmbeddedSourceSettingsTypeDef,
     TeletextSourceSettingsTypeDef,
     TrackSourceSettingsTypeDef,
     WebvttHlsSourceSettingsTypeDef,
     OutputChannelMappingOutputTypeDef,
     OutputChannelMappingTypeDef,
+    ClipLimitsOutputTypeDef,
     ClipLimitsTypeDef,
     CmafAdditionalManifestOutputTypeDef,
     CmafAdditionalManifestTypeDef,
     SpekeKeyProviderCmafOutputTypeDef,
-    StaticKeyProviderTypeDef,
+    StaticKeyProviderOutputTypeDef,
     SpekeKeyProviderCmafTypeDef,
+    StaticKeyProviderTypeDef,
+    CmafImageBasedTrickPlaySettingsOutputTypeDef,
     CmafImageBasedTrickPlaySettingsTypeDef,
+    CmfcSettingsOutputTypeDef,
     CmfcSettingsTypeDef,
+    Hdr10MetadataOutputTypeDef,
     Hdr10MetadataTypeDef,
-    F4vSettingsTypeDef,
+    F4vSettingsOutputTypeDef,
     M3u8SettingsOutputTypeDef,
+    MovSettingsOutputTypeDef,
+    Mp4SettingsOutputTypeDef,
+    MpdSettingsOutputTypeDef,
+    F4vSettingsTypeDef,
+    M3u8SettingsTypeDef,
     MovSettingsTypeDef,
     Mp4SettingsTypeDef,
     MpdSettingsTypeDef,
-    M3u8SettingsTypeDef,
     HopDestinationTypeDef,
     ResponseMetadataTypeDef,
     ReservationPlanSettingsTypeDef,
     DashAdditionalManifestOutputTypeDef,
     DashAdditionalManifestTypeDef,
     SpekeKeyProviderOutputTypeDef,
     SpekeKeyProviderTypeDef,
+    DashIsoImageBasedTrickPlaySettingsOutputTypeDef,
     DashIsoImageBasedTrickPlaySettingsTypeDef,
+    DeinterlacerOutputTypeDef,
     DeinterlacerTypeDef,
     DeleteJobTemplateRequestRequestTypeDef,
     DeletePresetRequestRequestTypeDef,
     DeleteQueueRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeEndpointsRequestRequestTypeDef,
     EndpointTypeDef,
     DisassociateCertificateRequestRequestTypeDef,
+    DolbyVisionLevel6MetadataOutputTypeDef,
     DolbyVisionLevel6MetadataTypeDef,
+    DvbNitSettingsOutputTypeDef,
     DvbNitSettingsTypeDef,
+    DvbSdtSettingsOutputTypeDef,
     DvbSdtSettingsTypeDef,
+    DvbTdtSettingsOutputTypeDef,
     DvbTdtSettingsTypeDef,
+    EsamManifestConfirmConditionNotificationOutputTypeDef,
     EsamManifestConfirmConditionNotificationTypeDef,
+    EsamSignalProcessingNotificationOutputTypeDef,
     EsamSignalProcessingNotificationTypeDef,
+    ExtendedDataServicesOutputTypeDef,
     ExtendedDataServicesTypeDef,
+    FrameCaptureSettingsOutputTypeDef,
     FrameCaptureSettingsTypeDef,
     GetJobRequestRequestTypeDef,
     GetJobTemplateRequestRequestTypeDef,
-    PolicyTypeDef,
+    PolicyOutputTypeDef,
     GetPresetRequestRequestTypeDef,
     GetQueueRequestRequestTypeDef,
+    H264QvbrSettingsOutputTypeDef,
     H264QvbrSettingsTypeDef,
+    H265QvbrSettingsOutputTypeDef,
     H265QvbrSettingsTypeDef,
+    Hdr10PlusOutputTypeDef,
     Hdr10PlusTypeDef,
     HlsAdditionalManifestOutputTypeDef,
     HlsAdditionalManifestTypeDef,
+    HlsCaptionLanguageMappingOutputTypeDef,
     HlsCaptionLanguageMappingTypeDef,
+    HlsImageBasedTrickPlaySettingsOutputTypeDef,
     HlsImageBasedTrickPlaySettingsTypeDef,
-    HlsSettingsTypeDef,
+    HlsSettingsOutputTypeDef,
+    HopDestinationOutputTypeDef,
+    Id3InsertionOutputTypeDef,
     Id3InsertionTypeDef,
+    InsertableImageOutputTypeDef,
     InsertableImageTypeDef,
+    InputClippingOutputTypeDef,
     InputClippingTypeDef,
+    InputDecryptionSettingsOutputTypeDef,
     InputDecryptionSettingsTypeDef,
-    InputVideoGeneratorTypeDef,
+    InputVideoGeneratorOutputTypeDef,
+    RectangleOutputTypeDef,
     RectangleTypeDef,
+    InputVideoGeneratorTypeDef,
     JobMessagesTypeDef,
+    KantarWatermarkSettingsOutputTypeDef,
+    NielsenConfigurationOutputTypeDef,
+    NielsenNonLinearWatermarkSettingsOutputTypeDef,
+    TimecodeConfigOutputTypeDef,
     KantarWatermarkSettingsTypeDef,
     NielsenConfigurationTypeDef,
     NielsenNonLinearWatermarkSettingsTypeDef,
     TimecodeConfigTypeDef,
     QueueTransitionTypeDef,
     TimingTypeDef,
     WarningGroupTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListPresetsRequestRequestTypeDef,
     ListQueuesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ResourceTagsTypeDef,
+    M2tsScte35EsamOutputTypeDef,
     M2tsScte35EsamTypeDef,
+    MotionImageInsertionFramerateOutputTypeDef,
+    MotionImageInsertionOffsetOutputTypeDef,
     MotionImageInsertionFramerateTypeDef,
     MotionImageInsertionOffsetTypeDef,
+    Mpeg2SettingsOutputTypeDef,
     Mpeg2SettingsTypeDef,
     MsSmoothAdditionalManifestOutputTypeDef,
     MsSmoothAdditionalManifestTypeDef,
+    MxfXavcProfileSettingsOutputTypeDef,
     MxfXavcProfileSettingsTypeDef,
+    NexGuardFileMarkerSettingsOutputTypeDef,
     NexGuardFileMarkerSettingsTypeDef,
+    NoiseReducerFilterSettingsOutputTypeDef,
     NoiseReducerFilterSettingsTypeDef,
+    NoiseReducerSpatialFilterSettingsOutputTypeDef,
+    NoiseReducerTemporalFilterSettingsOutputTypeDef,
     NoiseReducerSpatialFilterSettingsTypeDef,
     NoiseReducerTemporalFilterSettingsTypeDef,
     VideoDetailTypeDef,
+    PolicyTypeDef,
+    ProresSettingsOutputTypeDef,
     ProresSettingsTypeDef,
     ReservationPlanTypeDef,
+    S3DestinationAccessControlOutputTypeDef,
     S3DestinationAccessControlTypeDef,
+    S3EncryptionSettingsOutputTypeDef,
     S3EncryptionSettingsTypeDef,
     TagResourceRequestRequestTypeDef,
+    TimecodeBurninOutputTypeDef,
     TimecodeBurninTypeDef,
     UntagResourceRequestRequestTypeDef,
+    Vc3SettingsOutputTypeDef,
     Vc3SettingsTypeDef,
+    Vp8SettingsOutputTypeDef,
+    Vp9SettingsOutputTypeDef,
     Vp8SettingsTypeDef,
     Vp9SettingsTypeDef,
+    Xavc4kIntraCbgProfileSettingsOutputTypeDef,
     Xavc4kIntraCbgProfileSettingsTypeDef,
+    Xavc4kIntraVbrProfileSettingsOutputTypeDef,
     Xavc4kIntraVbrProfileSettingsTypeDef,
+    Xavc4kProfileSettingsOutputTypeDef,
     Xavc4kProfileSettingsTypeDef,
+    XavcHdIntraCbgProfileSettingsOutputTypeDef,
     XavcHdIntraCbgProfileSettingsTypeDef,
+    XavcHdProfileSettingsOutputTypeDef,
     XavcHdProfileSettingsTypeDef,
+    AudioCodecSettingsOutputTypeDef,
     AudioCodecSettingsTypeDef,
     AutomatedAbrRuleOutputTypeDef,
     AutomatedAbrRuleTypeDef,
+    Av1SettingsOutputTypeDef,
     Av1SettingsTypeDef,
+    AvcIntraSettingsOutputTypeDef,
     AvcIntraSettingsTypeDef,
     CaptionDestinationSettingsOutputTypeDef,
     CaptionDestinationSettingsTypeDef,
+    FileSourceSettingsOutputTypeDef,
     FileSourceSettingsTypeDef,
     ChannelMappingOutputTypeDef,
     ChannelMappingTypeDef,
     CmafEncryptionSettingsOutputTypeDef,
     CmafEncryptionSettingsTypeDef,
+    ColorCorrectorOutputTypeDef,
+    VideoSelectorOutputTypeDef,
     ColorCorrectorTypeDef,
     VideoSelectorTypeDef,
     CreateQueueRequestRequestTypeDef,
     UpdateQueueRequestRequestTypeDef,
     DashIsoEncryptionSettingsOutputTypeDef,
     HlsEncryptionSettingsOutputTypeDef,
     MsSmoothEncryptionSettingsOutputTypeDef,
@@ -884,115 +1017,127 @@
     MsSmoothEncryptionSettingsTypeDef,
     DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef,
     ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
     ListPresetsRequestListPresetsPaginateTypeDef,
     ListQueuesRequestListQueuesPaginateTypeDef,
     DescribeEndpointsResponseTypeDef,
+    DolbyVisionOutputTypeDef,
     DolbyVisionTypeDef,
+    EsamSettingsOutputTypeDef,
     EsamSettingsTypeDef,
     GetPolicyResponseTypeDef,
-    PutPolicyRequestRequestTypeDef,
     PutPolicyResponseTypeDef,
+    H264SettingsOutputTypeDef,
     H264SettingsTypeDef,
+    H265SettingsOutputTypeDef,
     H265SettingsTypeDef,
-    OutputSettingsTypeDef,
+    OutputSettingsOutputTypeDef,
     TimedMetadataInsertionOutputTypeDef,
     TimedMetadataInsertionTypeDef,
     ImageInserterOutputTypeDef,
     ImageInserterTypeDef,
     ListTagsForResourceResponseTypeDef,
     M2tsSettingsOutputTypeDef,
     M2tsSettingsTypeDef,
+    MotionImageInserterOutputTypeDef,
     MotionImageInserterTypeDef,
+    MxfSettingsOutputTypeDef,
     MxfSettingsTypeDef,
+    PartnerWatermarkingOutputTypeDef,
     PartnerWatermarkingTypeDef,
+    NoiseReducerOutputTypeDef,
     NoiseReducerTypeDef,
     OutputDetailTypeDef,
+    PutPolicyRequestRequestTypeDef,
     QueueTypeDef,
+    S3DestinationSettingsOutputTypeDef,
     S3DestinationSettingsTypeDef,
+    XavcSettingsOutputTypeDef,
     XavcSettingsTypeDef,
     AutomatedAbrSettingsOutputTypeDef,
     AutomatedAbrSettingsTypeDef,
+    CaptionDescriptionOutputTypeDef,
     CaptionDescriptionPresetOutputTypeDef,
     CaptionDescriptionPresetTypeDef,
-    CaptionDescriptionTypeDef,
+    CaptionSourceSettingsOutputTypeDef,
     CaptionSourceSettingsTypeDef,
     RemixSettingsOutputTypeDef,
     RemixSettingsTypeDef,
     ContainerSettingsOutputTypeDef,
     ContainerSettingsTypeDef,
     VideoPreprocessorOutputTypeDef,
     VideoPreprocessorTypeDef,
     OutputGroupDetailTypeDef,
     CreateQueueResponseTypeDef,
     GetQueueResponseTypeDef,
     ListQueuesResponseTypeDef,
     UpdateQueueResponseTypeDef,
+    DestinationSettingsOutputTypeDef,
     DestinationSettingsTypeDef,
+    VideoCodecSettingsOutputTypeDef,
     VideoCodecSettingsTypeDef,
     AutomatedEncodingSettingsOutputTypeDef,
     AutomatedEncodingSettingsTypeDef,
+    CaptionSelectorOutputTypeDef,
     CaptionSelectorTypeDef,
     AudioDescriptionOutputTypeDef,
     AudioSelectorOutputTypeDef,
     AudioDescriptionTypeDef,
     AudioSelectorTypeDef,
     CmafGroupSettingsOutputTypeDef,
-    CmafGroupSettingsTypeDef,
     DashIsoGroupSettingsOutputTypeDef,
+    FileGroupSettingsOutputTypeDef,
+    HlsGroupSettingsOutputTypeDef,
+    MsSmoothGroupSettingsOutputTypeDef,
+    CmafGroupSettingsTypeDef,
     DashIsoGroupSettingsTypeDef,
     FileGroupSettingsTypeDef,
-    HlsGroupSettingsOutputTypeDef,
     HlsGroupSettingsTypeDef,
-    MsSmoothGroupSettingsOutputTypeDef,
     MsSmoothGroupSettingsTypeDef,
     VideoDescriptionOutputTypeDef,
     VideoDescriptionTypeDef,
     InputOutputTypeDef,
     InputTemplateOutputTypeDef,
     InputTemplateTypeDef,
     InputTypeDef,
     OutputGroupSettingsOutputTypeDef,
     OutputGroupSettingsTypeDef,
-    PresetSettingsOutputTypeDef,
     OutputTypeDef,
+    PresetSettingsOutputTypeDef,
     PresetSettingsTypeDef,
-    PresetTypeDef,
     OutputGroupOutputTypeDef,
     OutputGroupTypeDef,
+    PresetTypeDef,
     CreatePresetRequestRequestTypeDef,
-    PresetSettingsUnionTypeDef,
     UpdatePresetRequestRequestTypeDef,
-    CreatePresetResponseTypeDef,
-    GetPresetResponseTypeDef,
-    ListPresetsResponseTypeDef,
-    UpdatePresetResponseTypeDef,
     JobSettingsOutputTypeDef,
     JobTemplateSettingsOutputTypeDef,
     JobSettingsTypeDef,
     JobTemplateSettingsTypeDef,
+    CreatePresetResponseTypeDef,
+    GetPresetResponseTypeDef,
+    ListPresetsResponseTypeDef,
+    UpdatePresetResponseTypeDef,
     JobTypeDef,
     JobTemplateTypeDef,
     CreateJobRequestRequestTypeDef,
-    JobSettingsUnionTypeDef,
     CreateJobTemplateRequestRequestTypeDef,
-    JobTemplateSettingsUnionTypeDef,
     UpdateJobTemplateRequestRequestTypeDef,
     CreateJobResponseTypeDef,
     GetJobResponseTypeDef,
     ListJobsResponseTypeDef,
     CreateJobTemplateResponseTypeDef,
     GetJobTemplateResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
     UpdateJobTemplateResponseTypeDef,
 )
 
 
-def get_value() -> AacSettingsTypeDef:
+def get_structure() -> AacSettingsOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mediaconvert-1.28.16/mypy_boto3_mediaconvert/__init__.py` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.28.16/mypy_boto3_mediaconvert/__init__.pyi` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.28.16/mypy_boto3_mediaconvert/__main__.py` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaConvert 1.28.16\nVersion:         1.28.16\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for boto3.MediaConvert 1.28.9\nVersion:         1.28.9\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.16")
+    print("1.28.9")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-mediaconvert-1.28.16/mypy_boto3_mediaconvert/client.py` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,23 +47,23 @@
     DescribeEndpointsResponseTypeDef,
     GetJobResponseTypeDef,
     GetJobTemplateResponseTypeDef,
     GetPolicyResponseTypeDef,
     GetPresetResponseTypeDef,
     GetQueueResponseTypeDef,
     HopDestinationTypeDef,
-    JobSettingsUnionTypeDef,
-    JobTemplateSettingsUnionTypeDef,
+    JobSettingsTypeDef,
+    JobTemplateSettingsTypeDef,
     ListJobsResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
     ListPresetsResponseTypeDef,
     ListQueuesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PolicyTypeDef,
-    PresetSettingsUnionTypeDef,
+    PresetSettingsTypeDef,
     PutPolicyResponseTypeDef,
     ReservationPlanSettingsTypeDef,
     UpdateJobTemplateResponseTypeDef,
     UpdatePresetResponseTypeDef,
     UpdateQueueResponseTypeDef,
 )
 
@@ -144,15 +144,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/client/#close)
         """
 
     def create_job(
         self,
         *,
         Role: str,
-        Settings: JobSettingsUnionTypeDef,
+        Settings: JobSettingsTypeDef,
         AccelerationSettings: AccelerationSettingsTypeDef = ...,
         BillingTagsSource: BillingTagsSourceType = ...,
         ClientRequestToken: str = ...,
         HopDestinations: Sequence[HopDestinationTypeDef] = ...,
         JobTemplate: str = ...,
         Priority: int = ...,
         Queue: str = ...,
@@ -168,15 +168,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/client/#create_job)
         """
 
     def create_job_template(
         self,
         *,
         Name: str,
-        Settings: JobTemplateSettingsUnionTypeDef,
+        Settings: JobTemplateSettingsTypeDef,
         AccelerationSettings: AccelerationSettingsTypeDef = ...,
         Category: str = ...,
         Description: str = ...,
         HopDestinations: Sequence[HopDestinationTypeDef] = ...,
         Priority: int = ...,
         Queue: str = ...,
         StatusUpdateInterval: StatusUpdateIntervalType = ...,
@@ -189,15 +189,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/client/#create_job_template)
         """
 
     def create_preset(
         self,
         *,
         Name: str,
-        Settings: PresetSettingsUnionTypeDef,
+        Settings: PresetSettingsTypeDef,
         Category: str = ...,
         Description: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreatePresetResponseTypeDef:
         """
         Create a new preset.
 
@@ -430,15 +430,15 @@
         Name: str,
         AccelerationSettings: AccelerationSettingsTypeDef = ...,
         Category: str = ...,
         Description: str = ...,
         HopDestinations: Sequence[HopDestinationTypeDef] = ...,
         Priority: int = ...,
         Queue: str = ...,
-        Settings: JobTemplateSettingsUnionTypeDef = ...,
+        Settings: JobTemplateSettingsTypeDef = ...,
         StatusUpdateInterval: StatusUpdateIntervalType = ...
     ) -> UpdateJobTemplateResponseTypeDef:
         """
         Modify one of your existing job templates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.update_job_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/client/#update_job_template)
@@ -446,15 +446,15 @@
 
     def update_preset(
         self,
         *,
         Name: str,
         Category: str = ...,
         Description: str = ...,
-        Settings: PresetSettingsUnionTypeDef = ...
+        Settings: PresetSettingsTypeDef = ...
     ) -> UpdatePresetResponseTypeDef:
         """
         Modify one of your existing presets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.update_preset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/client/#update_preset)
         """
```

### Comparing `mypy-boto3-mediaconvert-1.28.16/mypy_boto3_mediaconvert/client.pyi` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -47,23 +47,23 @@
     DescribeEndpointsResponseTypeDef,
     GetJobResponseTypeDef,
     GetJobTemplateResponseTypeDef,
     GetPolicyResponseTypeDef,
     GetPresetResponseTypeDef,
     GetQueueResponseTypeDef,
     HopDestinationTypeDef,
-    JobSettingsUnionTypeDef,
-    JobTemplateSettingsUnionTypeDef,
+    JobSettingsTypeDef,
+    JobTemplateSettingsTypeDef,
     ListJobsResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
     ListPresetsResponseTypeDef,
     ListQueuesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PolicyTypeDef,
-    PresetSettingsUnionTypeDef,
+    PresetSettingsTypeDef,
     PutPolicyResponseTypeDef,
     ReservationPlanSettingsTypeDef,
     UpdateJobTemplateResponseTypeDef,
     UpdatePresetResponseTypeDef,
     UpdateQueueResponseTypeDef,
 )
 
@@ -135,15 +135,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/client/#close)
         """
     def create_job(
         self,
         *,
         Role: str,
-        Settings: JobSettingsUnionTypeDef,
+        Settings: JobSettingsTypeDef,
         AccelerationSettings: AccelerationSettingsTypeDef = ...,
         BillingTagsSource: BillingTagsSourceType = ...,
         ClientRequestToken: str = ...,
         HopDestinations: Sequence[HopDestinationTypeDef] = ...,
         JobTemplate: str = ...,
         Priority: int = ...,
         Queue: str = ...,
@@ -158,15 +158,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.create_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/client/#create_job)
         """
     def create_job_template(
         self,
         *,
         Name: str,
-        Settings: JobTemplateSettingsUnionTypeDef,
+        Settings: JobTemplateSettingsTypeDef,
         AccelerationSettings: AccelerationSettingsTypeDef = ...,
         Category: str = ...,
         Description: str = ...,
         HopDestinations: Sequence[HopDestinationTypeDef] = ...,
         Priority: int = ...,
         Queue: str = ...,
         StatusUpdateInterval: StatusUpdateIntervalType = ...,
@@ -178,15 +178,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.create_job_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/client/#create_job_template)
         """
     def create_preset(
         self,
         *,
         Name: str,
-        Settings: PresetSettingsUnionTypeDef,
+        Settings: PresetSettingsTypeDef,
         Category: str = ...,
         Description: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreatePresetResponseTypeDef:
         """
         Create a new preset.
 
@@ -397,30 +397,30 @@
         Name: str,
         AccelerationSettings: AccelerationSettingsTypeDef = ...,
         Category: str = ...,
         Description: str = ...,
         HopDestinations: Sequence[HopDestinationTypeDef] = ...,
         Priority: int = ...,
         Queue: str = ...,
-        Settings: JobTemplateSettingsUnionTypeDef = ...,
+        Settings: JobTemplateSettingsTypeDef = ...,
         StatusUpdateInterval: StatusUpdateIntervalType = ...
     ) -> UpdateJobTemplateResponseTypeDef:
         """
         Modify one of your existing job templates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.update_job_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/client/#update_job_template)
         """
     def update_preset(
         self,
         *,
         Name: str,
         Category: str = ...,
         Description: str = ...,
-        Settings: PresetSettingsUnionTypeDef = ...
+        Settings: PresetSettingsTypeDef = ...
     ) -> UpdatePresetResponseTypeDef:
         """
         Modify one of your existing presets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.update_preset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/client/#update_preset)
         """
```

### Comparing `mypy-boto3-mediaconvert-1.28.16/mypy_boto3_mediaconvert/literals.py` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1413,15 +1413,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -1500,15 +1499,14 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
```

### Comparing `mypy-boto3-mediaconvert-1.28.16/mypy_boto3_mediaconvert/literals.pyi` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1411,15 +1411,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -1498,15 +1497,14 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
```

### Comparing `mypy-boto3-mediaconvert-1.28.16/mypy_boto3_mediaconvert/paginator.py` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.28.16/mypy_boto3_mediaconvert/paginator.pyi` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.28.16/mypy_boto3_mediaconvert/type_defs.py` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/type_defs.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for mediaconvert service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_mediaconvert.type_defs import AacSettingsTypeDef
+    from mypy_boto3_mediaconvert.type_defs import AacSettingsOutputTypeDef
 
-    data: AacSettingsTypeDef = ...
+    data: AacSettingsOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AacAudioDescriptionBroadcasterMixType,
     AacCodecProfileType,
     AacCodingModeType,
     AacRateControlModeType,
     AacRawFormatType,
@@ -428,171 +428,272 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AacSettingsOutputTypeDef",
     "AacSettingsTypeDef",
+    "Ac3SettingsOutputTypeDef",
     "Ac3SettingsTypeDef",
+    "AccelerationSettingsOutputTypeDef",
     "AccelerationSettingsTypeDef",
+    "AdvancedInputFilterSettingsOutputTypeDef",
     "AdvancedInputFilterSettingsTypeDef",
+    "AiffSettingsOutputTypeDef",
     "AiffSettingsTypeDef",
+    "AllowedRenditionSizeOutputTypeDef",
     "AllowedRenditionSizeTypeDef",
+    "AncillarySourceSettingsOutputTypeDef",
     "AncillarySourceSettingsTypeDef",
     "AssociateCertificateRequestRequestTypeDef",
+    "AudioChannelTaggingSettingsOutputTypeDef",
     "AudioChannelTaggingSettingsTypeDef",
+    "Eac3AtmosSettingsOutputTypeDef",
+    "Eac3SettingsOutputTypeDef",
+    "Mp2SettingsOutputTypeDef",
+    "Mp3SettingsOutputTypeDef",
+    "OpusSettingsOutputTypeDef",
+    "VorbisSettingsOutputTypeDef",
+    "WavSettingsOutputTypeDef",
     "Eac3AtmosSettingsTypeDef",
     "Eac3SettingsTypeDef",
     "Mp2SettingsTypeDef",
     "Mp3SettingsTypeDef",
     "OpusSettingsTypeDef",
     "VorbisSettingsTypeDef",
     "WavSettingsTypeDef",
+    "AudioNormalizationSettingsOutputTypeDef",
     "AudioNormalizationSettingsTypeDef",
     "AudioSelectorGroupOutputTypeDef",
     "AudioSelectorGroupTypeDef",
+    "HlsRenditionGroupSettingsOutputTypeDef",
     "HlsRenditionGroupSettingsTypeDef",
+    "ForceIncludeRenditionSizeOutputTypeDef",
+    "MinBottomRenditionSizeOutputTypeDef",
+    "MinTopRenditionSizeOutputTypeDef",
     "ForceIncludeRenditionSizeTypeDef",
     "MinBottomRenditionSizeTypeDef",
     "MinTopRenditionSizeTypeDef",
+    "Av1QvbrSettingsOutputTypeDef",
     "Av1QvbrSettingsTypeDef",
+    "AvailBlankingOutputTypeDef",
     "AvailBlankingTypeDef",
+    "AvcIntraUhdSettingsOutputTypeDef",
     "AvcIntraUhdSettingsTypeDef",
+    "BandwidthReductionFilterOutputTypeDef",
     "BandwidthReductionFilterTypeDef",
+    "BurninDestinationSettingsOutputTypeDef",
     "BurninDestinationSettingsTypeDef",
     "CancelJobRequestRequestTypeDef",
+    "DvbSubDestinationSettingsOutputTypeDef",
+    "EmbeddedDestinationSettingsOutputTypeDef",
+    "ImscDestinationSettingsOutputTypeDef",
+    "SccDestinationSettingsOutputTypeDef",
+    "SrtDestinationSettingsOutputTypeDef",
+    "TeletextDestinationSettingsOutputTypeDef",
+    "TtmlDestinationSettingsOutputTypeDef",
+    "WebvttDestinationSettingsOutputTypeDef",
     "DvbSubDestinationSettingsTypeDef",
     "EmbeddedDestinationSettingsTypeDef",
     "ImscDestinationSettingsTypeDef",
     "SccDestinationSettingsTypeDef",
     "SrtDestinationSettingsTypeDef",
-    "TeletextDestinationSettingsOutputTypeDef",
+    "TeletextDestinationSettingsTypeDef",
     "TtmlDestinationSettingsTypeDef",
     "WebvttDestinationSettingsTypeDef",
-    "TeletextDestinationSettingsTypeDef",
+    "CaptionSourceFramerateOutputTypeDef",
     "CaptionSourceFramerateTypeDef",
+    "DvbSubSourceSettingsOutputTypeDef",
+    "EmbeddedSourceSettingsOutputTypeDef",
+    "TeletextSourceSettingsOutputTypeDef",
+    "TrackSourceSettingsOutputTypeDef",
+    "WebvttHlsSourceSettingsOutputTypeDef",
     "DvbSubSourceSettingsTypeDef",
     "EmbeddedSourceSettingsTypeDef",
     "TeletextSourceSettingsTypeDef",
     "TrackSourceSettingsTypeDef",
     "WebvttHlsSourceSettingsTypeDef",
     "OutputChannelMappingOutputTypeDef",
     "OutputChannelMappingTypeDef",
+    "ClipLimitsOutputTypeDef",
     "ClipLimitsTypeDef",
     "CmafAdditionalManifestOutputTypeDef",
     "CmafAdditionalManifestTypeDef",
     "SpekeKeyProviderCmafOutputTypeDef",
-    "StaticKeyProviderTypeDef",
+    "StaticKeyProviderOutputTypeDef",
     "SpekeKeyProviderCmafTypeDef",
+    "StaticKeyProviderTypeDef",
+    "CmafImageBasedTrickPlaySettingsOutputTypeDef",
     "CmafImageBasedTrickPlaySettingsTypeDef",
+    "CmfcSettingsOutputTypeDef",
     "CmfcSettingsTypeDef",
+    "Hdr10MetadataOutputTypeDef",
     "Hdr10MetadataTypeDef",
-    "F4vSettingsTypeDef",
+    "F4vSettingsOutputTypeDef",
     "M3u8SettingsOutputTypeDef",
+    "MovSettingsOutputTypeDef",
+    "Mp4SettingsOutputTypeDef",
+    "MpdSettingsOutputTypeDef",
+    "F4vSettingsTypeDef",
+    "M3u8SettingsTypeDef",
     "MovSettingsTypeDef",
     "Mp4SettingsTypeDef",
     "MpdSettingsTypeDef",
-    "M3u8SettingsTypeDef",
     "HopDestinationTypeDef",
     "ResponseMetadataTypeDef",
     "ReservationPlanSettingsTypeDef",
     "DashAdditionalManifestOutputTypeDef",
     "DashAdditionalManifestTypeDef",
     "SpekeKeyProviderOutputTypeDef",
     "SpekeKeyProviderTypeDef",
+    "DashIsoImageBasedTrickPlaySettingsOutputTypeDef",
     "DashIsoImageBasedTrickPlaySettingsTypeDef",
+    "DeinterlacerOutputTypeDef",
     "DeinterlacerTypeDef",
     "DeleteJobTemplateRequestRequestTypeDef",
     "DeletePresetRequestRequestTypeDef",
     "DeleteQueueRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeEndpointsRequestRequestTypeDef",
     "EndpointTypeDef",
     "DisassociateCertificateRequestRequestTypeDef",
+    "DolbyVisionLevel6MetadataOutputTypeDef",
     "DolbyVisionLevel6MetadataTypeDef",
+    "DvbNitSettingsOutputTypeDef",
     "DvbNitSettingsTypeDef",
+    "DvbSdtSettingsOutputTypeDef",
     "DvbSdtSettingsTypeDef",
+    "DvbTdtSettingsOutputTypeDef",
     "DvbTdtSettingsTypeDef",
+    "EsamManifestConfirmConditionNotificationOutputTypeDef",
     "EsamManifestConfirmConditionNotificationTypeDef",
+    "EsamSignalProcessingNotificationOutputTypeDef",
     "EsamSignalProcessingNotificationTypeDef",
+    "ExtendedDataServicesOutputTypeDef",
     "ExtendedDataServicesTypeDef",
+    "FrameCaptureSettingsOutputTypeDef",
     "FrameCaptureSettingsTypeDef",
     "GetJobRequestRequestTypeDef",
     "GetJobTemplateRequestRequestTypeDef",
-    "PolicyTypeDef",
+    "PolicyOutputTypeDef",
     "GetPresetRequestRequestTypeDef",
     "GetQueueRequestRequestTypeDef",
+    "H264QvbrSettingsOutputTypeDef",
     "H264QvbrSettingsTypeDef",
+    "H265QvbrSettingsOutputTypeDef",
     "H265QvbrSettingsTypeDef",
+    "Hdr10PlusOutputTypeDef",
     "Hdr10PlusTypeDef",
     "HlsAdditionalManifestOutputTypeDef",
     "HlsAdditionalManifestTypeDef",
+    "HlsCaptionLanguageMappingOutputTypeDef",
     "HlsCaptionLanguageMappingTypeDef",
+    "HlsImageBasedTrickPlaySettingsOutputTypeDef",
     "HlsImageBasedTrickPlaySettingsTypeDef",
-    "HlsSettingsTypeDef",
+    "HlsSettingsOutputTypeDef",
+    "HopDestinationOutputTypeDef",
+    "Id3InsertionOutputTypeDef",
     "Id3InsertionTypeDef",
+    "InsertableImageOutputTypeDef",
     "InsertableImageTypeDef",
+    "InputClippingOutputTypeDef",
     "InputClippingTypeDef",
+    "InputDecryptionSettingsOutputTypeDef",
     "InputDecryptionSettingsTypeDef",
-    "InputVideoGeneratorTypeDef",
+    "InputVideoGeneratorOutputTypeDef",
+    "RectangleOutputTypeDef",
     "RectangleTypeDef",
+    "InputVideoGeneratorTypeDef",
     "JobMessagesTypeDef",
+    "KantarWatermarkSettingsOutputTypeDef",
+    "NielsenConfigurationOutputTypeDef",
+    "NielsenNonLinearWatermarkSettingsOutputTypeDef",
+    "TimecodeConfigOutputTypeDef",
     "KantarWatermarkSettingsTypeDef",
     "NielsenConfigurationTypeDef",
     "NielsenNonLinearWatermarkSettingsTypeDef",
     "TimecodeConfigTypeDef",
     "QueueTransitionTypeDef",
     "TimingTypeDef",
     "WarningGroupTypeDef",
     "ListJobTemplatesRequestRequestTypeDef",
     "ListJobsRequestRequestTypeDef",
     "ListPresetsRequestRequestTypeDef",
     "ListQueuesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ResourceTagsTypeDef",
+    "M2tsScte35EsamOutputTypeDef",
     "M2tsScte35EsamTypeDef",
+    "MotionImageInsertionFramerateOutputTypeDef",
+    "MotionImageInsertionOffsetOutputTypeDef",
     "MotionImageInsertionFramerateTypeDef",
     "MotionImageInsertionOffsetTypeDef",
+    "Mpeg2SettingsOutputTypeDef",
     "Mpeg2SettingsTypeDef",
     "MsSmoothAdditionalManifestOutputTypeDef",
     "MsSmoothAdditionalManifestTypeDef",
+    "MxfXavcProfileSettingsOutputTypeDef",
     "MxfXavcProfileSettingsTypeDef",
+    "NexGuardFileMarkerSettingsOutputTypeDef",
     "NexGuardFileMarkerSettingsTypeDef",
+    "NoiseReducerFilterSettingsOutputTypeDef",
     "NoiseReducerFilterSettingsTypeDef",
+    "NoiseReducerSpatialFilterSettingsOutputTypeDef",
+    "NoiseReducerTemporalFilterSettingsOutputTypeDef",
     "NoiseReducerSpatialFilterSettingsTypeDef",
     "NoiseReducerTemporalFilterSettingsTypeDef",
     "VideoDetailTypeDef",
+    "PolicyTypeDef",
+    "ProresSettingsOutputTypeDef",
     "ProresSettingsTypeDef",
     "ReservationPlanTypeDef",
+    "S3DestinationAccessControlOutputTypeDef",
     "S3DestinationAccessControlTypeDef",
+    "S3EncryptionSettingsOutputTypeDef",
     "S3EncryptionSettingsTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "TimecodeBurninOutputTypeDef",
     "TimecodeBurninTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "Vc3SettingsOutputTypeDef",
     "Vc3SettingsTypeDef",
+    "Vp8SettingsOutputTypeDef",
+    "Vp9SettingsOutputTypeDef",
     "Vp8SettingsTypeDef",
     "Vp9SettingsTypeDef",
+    "Xavc4kIntraCbgProfileSettingsOutputTypeDef",
     "Xavc4kIntraCbgProfileSettingsTypeDef",
+    "Xavc4kIntraVbrProfileSettingsOutputTypeDef",
     "Xavc4kIntraVbrProfileSettingsTypeDef",
+    "Xavc4kProfileSettingsOutputTypeDef",
     "Xavc4kProfileSettingsTypeDef",
+    "XavcHdIntraCbgProfileSettingsOutputTypeDef",
     "XavcHdIntraCbgProfileSettingsTypeDef",
+    "XavcHdProfileSettingsOutputTypeDef",
     "XavcHdProfileSettingsTypeDef",
+    "AudioCodecSettingsOutputTypeDef",
     "AudioCodecSettingsTypeDef",
     "AutomatedAbrRuleOutputTypeDef",
     "AutomatedAbrRuleTypeDef",
+    "Av1SettingsOutputTypeDef",
     "Av1SettingsTypeDef",
+    "AvcIntraSettingsOutputTypeDef",
     "AvcIntraSettingsTypeDef",
     "CaptionDestinationSettingsOutputTypeDef",
     "CaptionDestinationSettingsTypeDef",
+    "FileSourceSettingsOutputTypeDef",
     "FileSourceSettingsTypeDef",
     "ChannelMappingOutputTypeDef",
     "ChannelMappingTypeDef",
     "CmafEncryptionSettingsOutputTypeDef",
     "CmafEncryptionSettingsTypeDef",
+    "ColorCorrectorOutputTypeDef",
+    "VideoSelectorOutputTypeDef",
     "ColorCorrectorTypeDef",
     "VideoSelectorTypeDef",
     "CreateQueueRequestRequestTypeDef",
     "UpdateQueueRequestRequestTypeDef",
     "DashIsoEncryptionSettingsOutputTypeDef",
     "HlsEncryptionSettingsOutputTypeDef",
     "MsSmoothEncryptionSettingsOutputTypeDef",
@@ -601,113 +702,140 @@
     "MsSmoothEncryptionSettingsTypeDef",
     "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
     "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
     "ListPresetsRequestListPresetsPaginateTypeDef",
     "ListQueuesRequestListQueuesPaginateTypeDef",
     "DescribeEndpointsResponseTypeDef",
+    "DolbyVisionOutputTypeDef",
     "DolbyVisionTypeDef",
+    "EsamSettingsOutputTypeDef",
     "EsamSettingsTypeDef",
     "GetPolicyResponseTypeDef",
-    "PutPolicyRequestRequestTypeDef",
     "PutPolicyResponseTypeDef",
+    "H264SettingsOutputTypeDef",
     "H264SettingsTypeDef",
+    "H265SettingsOutputTypeDef",
     "H265SettingsTypeDef",
-    "OutputSettingsTypeDef",
+    "OutputSettingsOutputTypeDef",
     "TimedMetadataInsertionOutputTypeDef",
     "TimedMetadataInsertionTypeDef",
     "ImageInserterOutputTypeDef",
     "ImageInserterTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "M2tsSettingsOutputTypeDef",
     "M2tsSettingsTypeDef",
+    "MotionImageInserterOutputTypeDef",
     "MotionImageInserterTypeDef",
+    "MxfSettingsOutputTypeDef",
     "MxfSettingsTypeDef",
+    "PartnerWatermarkingOutputTypeDef",
     "PartnerWatermarkingTypeDef",
+    "NoiseReducerOutputTypeDef",
     "NoiseReducerTypeDef",
     "OutputDetailTypeDef",
+    "PutPolicyRequestRequestTypeDef",
     "QueueTypeDef",
+    "S3DestinationSettingsOutputTypeDef",
     "S3DestinationSettingsTypeDef",
+    "XavcSettingsOutputTypeDef",
     "XavcSettingsTypeDef",
     "AutomatedAbrSettingsOutputTypeDef",
     "AutomatedAbrSettingsTypeDef",
+    "CaptionDescriptionOutputTypeDef",
     "CaptionDescriptionPresetOutputTypeDef",
     "CaptionDescriptionPresetTypeDef",
-    "CaptionDescriptionTypeDef",
+    "CaptionSourceSettingsOutputTypeDef",
     "CaptionSourceSettingsTypeDef",
     "RemixSettingsOutputTypeDef",
     "RemixSettingsTypeDef",
     "ContainerSettingsOutputTypeDef",
     "ContainerSettingsTypeDef",
     "VideoPreprocessorOutputTypeDef",
     "VideoPreprocessorTypeDef",
     "OutputGroupDetailTypeDef",
     "CreateQueueResponseTypeDef",
     "GetQueueResponseTypeDef",
     "ListQueuesResponseTypeDef",
     "UpdateQueueResponseTypeDef",
+    "DestinationSettingsOutputTypeDef",
     "DestinationSettingsTypeDef",
+    "VideoCodecSettingsOutputTypeDef",
     "VideoCodecSettingsTypeDef",
     "AutomatedEncodingSettingsOutputTypeDef",
     "AutomatedEncodingSettingsTypeDef",
+    "CaptionSelectorOutputTypeDef",
     "CaptionSelectorTypeDef",
     "AudioDescriptionOutputTypeDef",
     "AudioSelectorOutputTypeDef",
     "AudioDescriptionTypeDef",
     "AudioSelectorTypeDef",
     "CmafGroupSettingsOutputTypeDef",
-    "CmafGroupSettingsTypeDef",
     "DashIsoGroupSettingsOutputTypeDef",
+    "FileGroupSettingsOutputTypeDef",
+    "HlsGroupSettingsOutputTypeDef",
+    "MsSmoothGroupSettingsOutputTypeDef",
+    "CmafGroupSettingsTypeDef",
     "DashIsoGroupSettingsTypeDef",
     "FileGroupSettingsTypeDef",
-    "HlsGroupSettingsOutputTypeDef",
     "HlsGroupSettingsTypeDef",
-    "MsSmoothGroupSettingsOutputTypeDef",
     "MsSmoothGroupSettingsTypeDef",
     "VideoDescriptionOutputTypeDef",
     "VideoDescriptionTypeDef",
     "InputOutputTypeDef",
     "InputTemplateOutputTypeDef",
     "InputTemplateTypeDef",
     "InputTypeDef",
     "OutputGroupSettingsOutputTypeDef",
     "OutputGroupSettingsTypeDef",
-    "PresetSettingsOutputTypeDef",
     "OutputTypeDef",
+    "PresetSettingsOutputTypeDef",
     "PresetSettingsTypeDef",
-    "PresetTypeDef",
     "OutputGroupOutputTypeDef",
     "OutputGroupTypeDef",
+    "PresetTypeDef",
     "CreatePresetRequestRequestTypeDef",
-    "PresetSettingsUnionTypeDef",
     "UpdatePresetRequestRequestTypeDef",
-    "CreatePresetResponseTypeDef",
-    "GetPresetResponseTypeDef",
-    "ListPresetsResponseTypeDef",
-    "UpdatePresetResponseTypeDef",
     "JobSettingsOutputTypeDef",
     "JobTemplateSettingsOutputTypeDef",
     "JobSettingsTypeDef",
     "JobTemplateSettingsTypeDef",
+    "CreatePresetResponseTypeDef",
+    "GetPresetResponseTypeDef",
+    "ListPresetsResponseTypeDef",
+    "UpdatePresetResponseTypeDef",
     "JobTypeDef",
     "JobTemplateTypeDef",
     "CreateJobRequestRequestTypeDef",
-    "JobSettingsUnionTypeDef",
     "CreateJobTemplateRequestRequestTypeDef",
-    "JobTemplateSettingsUnionTypeDef",
     "UpdateJobTemplateRequestRequestTypeDef",
     "CreateJobResponseTypeDef",
     "GetJobResponseTypeDef",
     "ListJobsResponseTypeDef",
     "CreateJobTemplateResponseTypeDef",
     "GetJobTemplateResponseTypeDef",
     "ListJobTemplatesResponseTypeDef",
     "UpdateJobTemplateResponseTypeDef",
 )
 
+AacSettingsOutputTypeDef = TypedDict(
+    "AacSettingsOutputTypeDef",
+    {
+        "AudioDescriptionBroadcasterMix": AacAudioDescriptionBroadcasterMixType,
+        "Bitrate": int,
+        "CodecProfile": AacCodecProfileType,
+        "CodingMode": AacCodingModeType,
+        "RateControlMode": AacRateControlModeType,
+        "RawFormat": AacRawFormatType,
+        "SampleRate": int,
+        "Specification": AacSpecificationType,
+        "VbrQuality": AacVbrQualityType,
+    },
+)
+
 AacSettingsTypeDef = TypedDict(
     "AacSettingsTypeDef",
     {
         "AudioDescriptionBroadcasterMix": AacAudioDescriptionBroadcasterMixType,
         "Bitrate": int,
         "CodecProfile": AacCodecProfileType,
         "CodingMode": AacCodingModeType,
@@ -716,14 +844,30 @@
         "SampleRate": int,
         "Specification": AacSpecificationType,
         "VbrQuality": AacVbrQualityType,
     },
     total=False,
 )
 
+Ac3SettingsOutputTypeDef = TypedDict(
+    "Ac3SettingsOutputTypeDef",
+    {
+        "Bitrate": int,
+        "BitstreamMode": Ac3BitstreamModeType,
+        "CodingMode": Ac3CodingModeType,
+        "Dialnorm": int,
+        "DynamicRangeCompressionLine": Ac3DynamicRangeCompressionLineType,
+        "DynamicRangeCompressionProfile": Ac3DynamicRangeCompressionProfileType,
+        "DynamicRangeCompressionRf": Ac3DynamicRangeCompressionRfType,
+        "LfeFilter": Ac3LfeFilterType,
+        "MetadataControl": Ac3MetadataControlType,
+        "SampleRate": int,
+    },
+)
+
 Ac3SettingsTypeDef = TypedDict(
     "Ac3SettingsTypeDef",
     {
         "Bitrate": int,
         "BitstreamMode": Ac3BitstreamModeType,
         "CodingMode": Ac3CodingModeType,
         "Dialnorm": int,
@@ -733,50 +877,92 @@
         "LfeFilter": Ac3LfeFilterType,
         "MetadataControl": Ac3MetadataControlType,
         "SampleRate": int,
     },
     total=False,
 )
 
+AccelerationSettingsOutputTypeDef = TypedDict(
+    "AccelerationSettingsOutputTypeDef",
+    {
+        "Mode": AccelerationModeType,
+    },
+)
+
 AccelerationSettingsTypeDef = TypedDict(
     "AccelerationSettingsTypeDef",
     {
         "Mode": AccelerationModeType,
     },
 )
 
+AdvancedInputFilterSettingsOutputTypeDef = TypedDict(
+    "AdvancedInputFilterSettingsOutputTypeDef",
+    {
+        "AddTexture": AdvancedInputFilterAddTextureType,
+        "Sharpening": AdvancedInputFilterSharpenType,
+    },
+)
+
 AdvancedInputFilterSettingsTypeDef = TypedDict(
     "AdvancedInputFilterSettingsTypeDef",
     {
         "AddTexture": AdvancedInputFilterAddTextureType,
         "Sharpening": AdvancedInputFilterSharpenType,
     },
     total=False,
 )
 
+AiffSettingsOutputTypeDef = TypedDict(
+    "AiffSettingsOutputTypeDef",
+    {
+        "BitDepth": int,
+        "Channels": int,
+        "SampleRate": int,
+    },
+)
+
 AiffSettingsTypeDef = TypedDict(
     "AiffSettingsTypeDef",
     {
         "BitDepth": int,
         "Channels": int,
         "SampleRate": int,
     },
     total=False,
 )
 
+AllowedRenditionSizeOutputTypeDef = TypedDict(
+    "AllowedRenditionSizeOutputTypeDef",
+    {
+        "Height": int,
+        "Required": RequiredFlagType,
+        "Width": int,
+    },
+)
+
 AllowedRenditionSizeTypeDef = TypedDict(
     "AllowedRenditionSizeTypeDef",
     {
         "Height": int,
         "Required": RequiredFlagType,
         "Width": int,
     },
     total=False,
 )
 
+AncillarySourceSettingsOutputTypeDef = TypedDict(
+    "AncillarySourceSettingsOutputTypeDef",
+    {
+        "Convert608To708": AncillaryConvert608To708Type,
+        "SourceAncillaryChannelNumber": int,
+        "TerminateCaptions": AncillaryTerminateCaptionsType,
+    },
+)
+
 AncillarySourceSettingsTypeDef = TypedDict(
     "AncillarySourceSettingsTypeDef",
     {
         "Convert608To708": AncillaryConvert608To708Type,
         "SourceAncillaryChannelNumber": int,
         "TerminateCaptions": AncillaryTerminateCaptionsType,
     },
@@ -786,22 +972,127 @@
 AssociateCertificateRequestRequestTypeDef = TypedDict(
     "AssociateCertificateRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
+AudioChannelTaggingSettingsOutputTypeDef = TypedDict(
+    "AudioChannelTaggingSettingsOutputTypeDef",
+    {
+        "ChannelTag": AudioChannelTagType,
+    },
+)
+
 AudioChannelTaggingSettingsTypeDef = TypedDict(
     "AudioChannelTaggingSettingsTypeDef",
     {
         "ChannelTag": AudioChannelTagType,
     },
     total=False,
 )
 
+Eac3AtmosSettingsOutputTypeDef = TypedDict(
+    "Eac3AtmosSettingsOutputTypeDef",
+    {
+        "Bitrate": int,
+        "BitstreamMode": Literal["COMPLETE_MAIN"],
+        "CodingMode": Eac3AtmosCodingModeType,
+        "DialogueIntelligence": Eac3AtmosDialogueIntelligenceType,
+        "DownmixControl": Eac3AtmosDownmixControlType,
+        "DynamicRangeCompressionLine": Eac3AtmosDynamicRangeCompressionLineType,
+        "DynamicRangeCompressionRf": Eac3AtmosDynamicRangeCompressionRfType,
+        "DynamicRangeControl": Eac3AtmosDynamicRangeControlType,
+        "LoRoCenterMixLevel": float,
+        "LoRoSurroundMixLevel": float,
+        "LtRtCenterMixLevel": float,
+        "LtRtSurroundMixLevel": float,
+        "MeteringMode": Eac3AtmosMeteringModeType,
+        "SampleRate": int,
+        "SpeechThreshold": int,
+        "StereoDownmix": Eac3AtmosStereoDownmixType,
+        "SurroundExMode": Eac3AtmosSurroundExModeType,
+    },
+)
+
+Eac3SettingsOutputTypeDef = TypedDict(
+    "Eac3SettingsOutputTypeDef",
+    {
+        "AttenuationControl": Eac3AttenuationControlType,
+        "Bitrate": int,
+        "BitstreamMode": Eac3BitstreamModeType,
+        "CodingMode": Eac3CodingModeType,
+        "DcFilter": Eac3DcFilterType,
+        "Dialnorm": int,
+        "DynamicRangeCompressionLine": Eac3DynamicRangeCompressionLineType,
+        "DynamicRangeCompressionRf": Eac3DynamicRangeCompressionRfType,
+        "LfeControl": Eac3LfeControlType,
+        "LfeFilter": Eac3LfeFilterType,
+        "LoRoCenterMixLevel": float,
+        "LoRoSurroundMixLevel": float,
+        "LtRtCenterMixLevel": float,
+        "LtRtSurroundMixLevel": float,
+        "MetadataControl": Eac3MetadataControlType,
+        "PassthroughControl": Eac3PassthroughControlType,
+        "PhaseControl": Eac3PhaseControlType,
+        "SampleRate": int,
+        "StereoDownmix": Eac3StereoDownmixType,
+        "SurroundExMode": Eac3SurroundExModeType,
+        "SurroundMode": Eac3SurroundModeType,
+    },
+)
+
+Mp2SettingsOutputTypeDef = TypedDict(
+    "Mp2SettingsOutputTypeDef",
+    {
+        "Bitrate": int,
+        "Channels": int,
+        "SampleRate": int,
+    },
+)
+
+Mp3SettingsOutputTypeDef = TypedDict(
+    "Mp3SettingsOutputTypeDef",
+    {
+        "Bitrate": int,
+        "Channels": int,
+        "RateControlMode": Mp3RateControlModeType,
+        "SampleRate": int,
+        "VbrQuality": int,
+    },
+)
+
+OpusSettingsOutputTypeDef = TypedDict(
+    "OpusSettingsOutputTypeDef",
+    {
+        "Bitrate": int,
+        "Channels": int,
+        "SampleRate": int,
+    },
+)
+
+VorbisSettingsOutputTypeDef = TypedDict(
+    "VorbisSettingsOutputTypeDef",
+    {
+        "Channels": int,
+        "SampleRate": int,
+        "VbrQuality": int,
+    },
+)
+
+WavSettingsOutputTypeDef = TypedDict(
+    "WavSettingsOutputTypeDef",
+    {
+        "BitDepth": int,
+        "Channels": int,
+        "Format": WavFormatType,
+        "SampleRate": int,
+    },
+)
+
 Eac3AtmosSettingsTypeDef = TypedDict(
     "Eac3AtmosSettingsTypeDef",
     {
         "Bitrate": int,
         "BitstreamMode": Literal["COMPLETE_MAIN"],
         "CodingMode": Eac3AtmosCodingModeType,
         "DialogueIntelligence": Eac3AtmosDialogueIntelligenceType,
@@ -899,14 +1190,27 @@
         "Channels": int,
         "Format": WavFormatType,
         "SampleRate": int,
     },
     total=False,
 )
 
+AudioNormalizationSettingsOutputTypeDef = TypedDict(
+    "AudioNormalizationSettingsOutputTypeDef",
+    {
+        "Algorithm": AudioNormalizationAlgorithmType,
+        "AlgorithmControl": AudioNormalizationAlgorithmControlType,
+        "CorrectionGateLevel": int,
+        "LoudnessLogging": AudioNormalizationLoudnessLoggingType,
+        "PeakCalculation": AudioNormalizationPeakCalculationType,
+        "TargetLkfs": float,
+        "TruePeakLimiterThreshold": float,
+    },
+)
+
 AudioNormalizationSettingsTypeDef = TypedDict(
     "AudioNormalizationSettingsTypeDef",
     {
         "Algorithm": AudioNormalizationAlgorithmType,
         "AlgorithmControl": AudioNormalizationAlgorithmControlType,
         "CorrectionGateLevel": int,
         "LoudnessLogging": AudioNormalizationLoudnessLoggingType,
@@ -918,35 +1222,67 @@
 )
 
 AudioSelectorGroupOutputTypeDef = TypedDict(
     "AudioSelectorGroupOutputTypeDef",
     {
         "AudioSelectorNames": List[str],
     },
-    total=False,
 )
 
 AudioSelectorGroupTypeDef = TypedDict(
     "AudioSelectorGroupTypeDef",
     {
         "AudioSelectorNames": Sequence[str],
     },
     total=False,
 )
 
+HlsRenditionGroupSettingsOutputTypeDef = TypedDict(
+    "HlsRenditionGroupSettingsOutputTypeDef",
+    {
+        "RenditionGroupId": str,
+        "RenditionLanguageCode": LanguageCodeType,
+        "RenditionName": str,
+    },
+)
+
 HlsRenditionGroupSettingsTypeDef = TypedDict(
     "HlsRenditionGroupSettingsTypeDef",
     {
         "RenditionGroupId": str,
         "RenditionLanguageCode": LanguageCodeType,
         "RenditionName": str,
     },
     total=False,
 )
 
+ForceIncludeRenditionSizeOutputTypeDef = TypedDict(
+    "ForceIncludeRenditionSizeOutputTypeDef",
+    {
+        "Height": int,
+        "Width": int,
+    },
+)
+
+MinBottomRenditionSizeOutputTypeDef = TypedDict(
+    "MinBottomRenditionSizeOutputTypeDef",
+    {
+        "Height": int,
+        "Width": int,
+    },
+)
+
+MinTopRenditionSizeOutputTypeDef = TypedDict(
+    "MinTopRenditionSizeOutputTypeDef",
+    {
+        "Height": int,
+        "Width": int,
+    },
+)
+
 ForceIncludeRenditionSizeTypeDef = TypedDict(
     "ForceIncludeRenditionSizeTypeDef",
     {
         "Height": int,
         "Width": int,
     },
     total=False,
@@ -966,48 +1302,105 @@
     {
         "Height": int,
         "Width": int,
     },
     total=False,
 )
 
+Av1QvbrSettingsOutputTypeDef = TypedDict(
+    "Av1QvbrSettingsOutputTypeDef",
+    {
+        "QvbrQualityLevel": int,
+        "QvbrQualityLevelFineTune": float,
+    },
+)
+
 Av1QvbrSettingsTypeDef = TypedDict(
     "Av1QvbrSettingsTypeDef",
     {
         "QvbrQualityLevel": int,
         "QvbrQualityLevelFineTune": float,
     },
     total=False,
 )
 
+AvailBlankingOutputTypeDef = TypedDict(
+    "AvailBlankingOutputTypeDef",
+    {
+        "AvailBlankingImage": str,
+    },
+)
+
 AvailBlankingTypeDef = TypedDict(
     "AvailBlankingTypeDef",
     {
         "AvailBlankingImage": str,
     },
     total=False,
 )
 
+AvcIntraUhdSettingsOutputTypeDef = TypedDict(
+    "AvcIntraUhdSettingsOutputTypeDef",
+    {
+        "QualityTuningLevel": AvcIntraUhdQualityTuningLevelType,
+    },
+)
+
 AvcIntraUhdSettingsTypeDef = TypedDict(
     "AvcIntraUhdSettingsTypeDef",
     {
         "QualityTuningLevel": AvcIntraUhdQualityTuningLevelType,
     },
     total=False,
 )
 
+BandwidthReductionFilterOutputTypeDef = TypedDict(
+    "BandwidthReductionFilterOutputTypeDef",
+    {
+        "Sharpening": BandwidthReductionFilterSharpeningType,
+        "Strength": BandwidthReductionFilterStrengthType,
+    },
+)
+
 BandwidthReductionFilterTypeDef = TypedDict(
     "BandwidthReductionFilterTypeDef",
     {
         "Sharpening": BandwidthReductionFilterSharpeningType,
         "Strength": BandwidthReductionFilterStrengthType,
     },
     total=False,
 )
 
+BurninDestinationSettingsOutputTypeDef = TypedDict(
+    "BurninDestinationSettingsOutputTypeDef",
+    {
+        "Alignment": BurninSubtitleAlignmentType,
+        "ApplyFontColor": BurninSubtitleApplyFontColorType,
+        "BackgroundColor": BurninSubtitleBackgroundColorType,
+        "BackgroundOpacity": int,
+        "FallbackFont": BurninSubtitleFallbackFontType,
+        "FontColor": BurninSubtitleFontColorType,
+        "FontOpacity": int,
+        "FontResolution": int,
+        "FontScript": FontScriptType,
+        "FontSize": int,
+        "HexFontColor": str,
+        "OutlineColor": BurninSubtitleOutlineColorType,
+        "OutlineSize": int,
+        "ShadowColor": BurninSubtitleShadowColorType,
+        "ShadowOpacity": int,
+        "ShadowXOffset": int,
+        "ShadowYOffset": int,
+        "StylePassthrough": BurnInSubtitleStylePassthroughType,
+        "TeletextSpacing": BurninSubtitleTeletextSpacingType,
+        "XPosition": int,
+        "YPosition": int,
+    },
+)
+
 BurninDestinationSettingsTypeDef = TypedDict(
     "BurninDestinationSettingsTypeDef",
     {
         "Alignment": BurninSubtitleAlignmentType,
         "ApplyFontColor": BurninSubtitleApplyFontColorType,
         "BackgroundColor": BurninSubtitleBackgroundColorType,
         "BackgroundOpacity": int,
@@ -1035,14 +1428,100 @@
 CancelJobRequestRequestTypeDef = TypedDict(
     "CancelJobRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+DvbSubDestinationSettingsOutputTypeDef = TypedDict(
+    "DvbSubDestinationSettingsOutputTypeDef",
+    {
+        "Alignment": DvbSubtitleAlignmentType,
+        "ApplyFontColor": DvbSubtitleApplyFontColorType,
+        "BackgroundColor": DvbSubtitleBackgroundColorType,
+        "BackgroundOpacity": int,
+        "DdsHandling": DvbddsHandlingType,
+        "DdsXCoordinate": int,
+        "DdsYCoordinate": int,
+        "FallbackFont": DvbSubSubtitleFallbackFontType,
+        "FontColor": DvbSubtitleFontColorType,
+        "FontOpacity": int,
+        "FontResolution": int,
+        "FontScript": FontScriptType,
+        "FontSize": int,
+        "Height": int,
+        "HexFontColor": str,
+        "OutlineColor": DvbSubtitleOutlineColorType,
+        "OutlineSize": int,
+        "ShadowColor": DvbSubtitleShadowColorType,
+        "ShadowOpacity": int,
+        "ShadowXOffset": int,
+        "ShadowYOffset": int,
+        "StylePassthrough": DvbSubtitleStylePassthroughType,
+        "SubtitlingType": DvbSubtitlingTypeType,
+        "TeletextSpacing": DvbSubtitleTeletextSpacingType,
+        "Width": int,
+        "XPosition": int,
+        "YPosition": int,
+    },
+)
+
+EmbeddedDestinationSettingsOutputTypeDef = TypedDict(
+    "EmbeddedDestinationSettingsOutputTypeDef",
+    {
+        "Destination608ChannelNumber": int,
+        "Destination708ServiceNumber": int,
+    },
+)
+
+ImscDestinationSettingsOutputTypeDef = TypedDict(
+    "ImscDestinationSettingsOutputTypeDef",
+    {
+        "Accessibility": ImscAccessibilitySubsType,
+        "StylePassthrough": ImscStylePassthroughType,
+    },
+)
+
+SccDestinationSettingsOutputTypeDef = TypedDict(
+    "SccDestinationSettingsOutputTypeDef",
+    {
+        "Framerate": SccDestinationFramerateType,
+    },
+)
+
+SrtDestinationSettingsOutputTypeDef = TypedDict(
+    "SrtDestinationSettingsOutputTypeDef",
+    {
+        "StylePassthrough": SrtStylePassthroughType,
+    },
+)
+
+TeletextDestinationSettingsOutputTypeDef = TypedDict(
+    "TeletextDestinationSettingsOutputTypeDef",
+    {
+        "PageNumber": str,
+        "PageTypes": List[TeletextPageTypeType],
+    },
+)
+
+TtmlDestinationSettingsOutputTypeDef = TypedDict(
+    "TtmlDestinationSettingsOutputTypeDef",
+    {
+        "StylePassthrough": TtmlStylePassthroughType,
+    },
+)
+
+WebvttDestinationSettingsOutputTypeDef = TypedDict(
+    "WebvttDestinationSettingsOutputTypeDef",
+    {
+        "Accessibility": WebvttAccessibilitySubsType,
+        "StylePassthrough": WebvttStylePassthroughType,
+    },
+)
+
 DvbSubDestinationSettingsTypeDef = TypedDict(
     "DvbSubDestinationSettingsTypeDef",
     {
         "Alignment": DvbSubtitleAlignmentType,
         "ApplyFontColor": DvbSubtitleApplyFontColorType,
         "BackgroundColor": DvbSubtitleBackgroundColorType,
         "BackgroundOpacity": int,
@@ -1103,19 +1582,19 @@
     "SrtDestinationSettingsTypeDef",
     {
         "StylePassthrough": SrtStylePassthroughType,
     },
     total=False,
 )
 
-TeletextDestinationSettingsOutputTypeDef = TypedDict(
-    "TeletextDestinationSettingsOutputTypeDef",
+TeletextDestinationSettingsTypeDef = TypedDict(
+    "TeletextDestinationSettingsTypeDef",
     {
         "PageNumber": str,
-        "PageTypes": List[TeletextPageTypeType],
+        "PageTypes": Sequence[TeletextPageTypeType],
     },
     total=False,
 )
 
 TtmlDestinationSettingsTypeDef = TypedDict(
     "TtmlDestinationSettingsTypeDef",
     {
@@ -1129,32 +1608,71 @@
     {
         "Accessibility": WebvttAccessibilitySubsType,
         "StylePassthrough": WebvttStylePassthroughType,
     },
     total=False,
 )
 
-TeletextDestinationSettingsTypeDef = TypedDict(
-    "TeletextDestinationSettingsTypeDef",
+CaptionSourceFramerateOutputTypeDef = TypedDict(
+    "CaptionSourceFramerateOutputTypeDef",
     {
-        "PageNumber": str,
-        "PageTypes": Sequence[TeletextPageTypeType],
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
     },
-    total=False,
 )
 
 CaptionSourceFramerateTypeDef = TypedDict(
     "CaptionSourceFramerateTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
     },
     total=False,
 )
 
+DvbSubSourceSettingsOutputTypeDef = TypedDict(
+    "DvbSubSourceSettingsOutputTypeDef",
+    {
+        "Pid": int,
+    },
+)
+
+EmbeddedSourceSettingsOutputTypeDef = TypedDict(
+    "EmbeddedSourceSettingsOutputTypeDef",
+    {
+        "Convert608To708": EmbeddedConvert608To708Type,
+        "Source608ChannelNumber": int,
+        "Source608TrackNumber": int,
+        "TerminateCaptions": EmbeddedTerminateCaptionsType,
+    },
+)
+
+TeletextSourceSettingsOutputTypeDef = TypedDict(
+    "TeletextSourceSettingsOutputTypeDef",
+    {
+        "PageNumber": str,
+    },
+)
+
+TrackSourceSettingsOutputTypeDef = TypedDict(
+    "TrackSourceSettingsOutputTypeDef",
+    {
+        "TrackNumber": int,
+    },
+)
+
+WebvttHlsSourceSettingsOutputTypeDef = TypedDict(
+    "WebvttHlsSourceSettingsOutputTypeDef",
+    {
+        "RenditionGroupId": str,
+        "RenditionLanguageCode": LanguageCodeType,
+        "RenditionName": str,
+    },
+)
+
 DvbSubSourceSettingsTypeDef = TypedDict(
     "DvbSubSourceSettingsTypeDef",
     {
         "Pid": int,
     },
     total=False,
 )
@@ -1198,26 +1716,35 @@
 
 OutputChannelMappingOutputTypeDef = TypedDict(
     "OutputChannelMappingOutputTypeDef",
     {
         "InputChannels": List[int],
         "InputChannelsFineTune": List[float],
     },
-    total=False,
 )
 
 OutputChannelMappingTypeDef = TypedDict(
     "OutputChannelMappingTypeDef",
     {
         "InputChannels": Sequence[int],
         "InputChannelsFineTune": Sequence[float],
     },
     total=False,
 )
 
+ClipLimitsOutputTypeDef = TypedDict(
+    "ClipLimitsOutputTypeDef",
+    {
+        "MaximumRGBTolerance": int,
+        "MaximumYUV": int,
+        "MinimumRGBTolerance": int,
+        "MinimumYUV": int,
+    },
+)
+
 ClipLimitsTypeDef = TypedDict(
     "ClipLimitsTypeDef",
     {
         "MaximumRGBTolerance": int,
         "MaximumYUV": int,
         "MinimumRGBTolerance": int,
         "MinimumYUV": int,
@@ -1227,15 +1754,14 @@
 
 CmafAdditionalManifestOutputTypeDef = TypedDict(
     "CmafAdditionalManifestOutputTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": List[str],
     },
-    total=False,
 )
 
 CmafAdditionalManifestTypeDef = TypedDict(
     "CmafAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
@@ -1248,53 +1774,94 @@
     {
         "CertificateArn": str,
         "DashSignaledSystemIds": List[str],
         "HlsSignaledSystemIds": List[str],
         "ResourceId": str,
         "Url": str,
     },
-    total=False,
 )
 
-StaticKeyProviderTypeDef = TypedDict(
-    "StaticKeyProviderTypeDef",
+StaticKeyProviderOutputTypeDef = TypedDict(
+    "StaticKeyProviderOutputTypeDef",
     {
         "KeyFormat": str,
         "KeyFormatVersions": str,
         "StaticKeyValue": str,
         "Url": str,
     },
-    total=False,
 )
 
 SpekeKeyProviderCmafTypeDef = TypedDict(
     "SpekeKeyProviderCmafTypeDef",
     {
         "CertificateArn": str,
         "DashSignaledSystemIds": Sequence[str],
         "HlsSignaledSystemIds": Sequence[str],
         "ResourceId": str,
         "Url": str,
     },
     total=False,
 )
 
+StaticKeyProviderTypeDef = TypedDict(
+    "StaticKeyProviderTypeDef",
+    {
+        "KeyFormat": str,
+        "KeyFormatVersions": str,
+        "StaticKeyValue": str,
+        "Url": str,
+    },
+    total=False,
+)
+
+CmafImageBasedTrickPlaySettingsOutputTypeDef = TypedDict(
+    "CmafImageBasedTrickPlaySettingsOutputTypeDef",
+    {
+        "IntervalCadence": CmafIntervalCadenceType,
+        "ThumbnailHeight": int,
+        "ThumbnailInterval": float,
+        "ThumbnailWidth": int,
+        "TileHeight": int,
+        "TileWidth": int,
+    },
+)
+
 CmafImageBasedTrickPlaySettingsTypeDef = TypedDict(
     "CmafImageBasedTrickPlaySettingsTypeDef",
     {
         "IntervalCadence": CmafIntervalCadenceType,
         "ThumbnailHeight": int,
         "ThumbnailInterval": float,
         "ThumbnailWidth": int,
         "TileHeight": int,
         "TileWidth": int,
     },
     total=False,
 )
 
+CmfcSettingsOutputTypeDef = TypedDict(
+    "CmfcSettingsOutputTypeDef",
+    {
+        "AudioDuration": CmfcAudioDurationType,
+        "AudioGroupId": str,
+        "AudioRenditionSets": str,
+        "AudioTrackType": CmfcAudioTrackTypeType,
+        "DescriptiveVideoServiceFlag": CmfcDescriptiveVideoServiceFlagType,
+        "IFrameOnlyManifest": CmfcIFrameOnlyManifestType,
+        "KlvMetadata": CmfcKlvMetadataType,
+        "ManifestMetadataSignaling": CmfcManifestMetadataSignalingType,
+        "Scte35Esam": CmfcScte35EsamType,
+        "Scte35Source": CmfcScte35SourceType,
+        "TimedMetadata": CmfcTimedMetadataType,
+        "TimedMetadataBoxVersion": CmfcTimedMetadataBoxVersionType,
+        "TimedMetadataSchemeIdUri": str,
+        "TimedMetadataValue": str,
+    },
+)
+
 CmfcSettingsTypeDef = TypedDict(
     "CmfcSettingsTypeDef",
     {
         "AudioDuration": CmfcAudioDurationType,
         "AudioGroupId": str,
         "AudioRenditionSets": str,
         "AudioTrackType": CmfcAudioTrackTypeType,
@@ -1308,14 +1875,32 @@
         "TimedMetadataBoxVersion": CmfcTimedMetadataBoxVersionType,
         "TimedMetadataSchemeIdUri": str,
         "TimedMetadataValue": str,
     },
     total=False,
 )
 
+Hdr10MetadataOutputTypeDef = TypedDict(
+    "Hdr10MetadataOutputTypeDef",
+    {
+        "BluePrimaryX": int,
+        "BluePrimaryY": int,
+        "GreenPrimaryX": int,
+        "GreenPrimaryY": int,
+        "MaxContentLightLevel": int,
+        "MaxFrameAverageLightLevel": int,
+        "MaxLuminance": int,
+        "MinLuminance": int,
+        "RedPrimaryX": int,
+        "RedPrimaryY": int,
+        "WhitePointX": int,
+        "WhitePointY": int,
+    },
+)
+
 Hdr10MetadataTypeDef = TypedDict(
     "Hdr10MetadataTypeDef",
     {
         "BluePrimaryX": int,
         "BluePrimaryY": int,
         "GreenPrimaryX": int,
         "GreenPrimaryY": int,
@@ -1327,20 +1912,19 @@
         "RedPrimaryY": int,
         "WhitePointX": int,
         "WhitePointY": int,
     },
     total=False,
 )
 
-F4vSettingsTypeDef = TypedDict(
-    "F4vSettingsTypeDef",
+F4vSettingsOutputTypeDef = TypedDict(
+    "F4vSettingsOutputTypeDef",
     {
         "MoovPlacement": F4vMoovPlacementType,
     },
-    total=False,
 )
 
 M3u8SettingsOutputTypeDef = TypedDict(
     "M3u8SettingsOutputTypeDef",
     {
         "AudioDuration": M3u8AudioDurationType,
         "AudioFramesPerPes": int,
@@ -1358,57 +1942,61 @@
         "Scte35Pid": int,
         "Scte35Source": M3u8Scte35SourceType,
         "TimedMetadata": TimedMetadataType,
         "TimedMetadataPid": int,
         "TransportStreamId": int,
         "VideoPid": int,
     },
-    total=False,
 )
 
-MovSettingsTypeDef = TypedDict(
-    "MovSettingsTypeDef",
+MovSettingsOutputTypeDef = TypedDict(
+    "MovSettingsOutputTypeDef",
     {
         "ClapAtom": MovClapAtomType,
         "CslgAtom": MovCslgAtomType,
         "Mpeg2FourCCControl": MovMpeg2FourCCControlType,
         "PaddingControl": MovPaddingControlType,
         "Reference": MovReferenceType,
     },
-    total=False,
 )
 
-Mp4SettingsTypeDef = TypedDict(
-    "Mp4SettingsTypeDef",
+Mp4SettingsOutputTypeDef = TypedDict(
+    "Mp4SettingsOutputTypeDef",
     {
         "AudioDuration": CmfcAudioDurationType,
         "CslgAtom": Mp4CslgAtomType,
         "CttsVersion": int,
         "FreeSpaceBox": Mp4FreeSpaceBoxType,
         "MoovPlacement": Mp4MoovPlacementType,
         "Mp4MajorBrand": str,
     },
-    total=False,
 )
 
-MpdSettingsTypeDef = TypedDict(
-    "MpdSettingsTypeDef",
+MpdSettingsOutputTypeDef = TypedDict(
+    "MpdSettingsOutputTypeDef",
     {
         "AccessibilityCaptionHints": MpdAccessibilityCaptionHintsType,
         "AudioDuration": MpdAudioDurationType,
         "CaptionContainerType": MpdCaptionContainerTypeType,
         "KlvMetadata": MpdKlvMetadataType,
         "ManifestMetadataSignaling": MpdManifestMetadataSignalingType,
         "Scte35Esam": MpdScte35EsamType,
         "Scte35Source": MpdScte35SourceType,
         "TimedMetadata": MpdTimedMetadataType,
         "TimedMetadataBoxVersion": MpdTimedMetadataBoxVersionType,
         "TimedMetadataSchemeIdUri": str,
         "TimedMetadataValue": str,
     },
+)
+
+F4vSettingsTypeDef = TypedDict(
+    "F4vSettingsTypeDef",
+    {
+        "MoovPlacement": F4vMoovPlacementType,
+    },
     total=False,
 )
 
 M3u8SettingsTypeDef = TypedDict(
     "M3u8SettingsTypeDef",
     {
         "AudioDuration": M3u8AudioDurationType,
@@ -1430,14 +2018,57 @@
         "TimedMetadataPid": int,
         "TransportStreamId": int,
         "VideoPid": int,
     },
     total=False,
 )
 
+MovSettingsTypeDef = TypedDict(
+    "MovSettingsTypeDef",
+    {
+        "ClapAtom": MovClapAtomType,
+        "CslgAtom": MovCslgAtomType,
+        "Mpeg2FourCCControl": MovMpeg2FourCCControlType,
+        "PaddingControl": MovPaddingControlType,
+        "Reference": MovReferenceType,
+    },
+    total=False,
+)
+
+Mp4SettingsTypeDef = TypedDict(
+    "Mp4SettingsTypeDef",
+    {
+        "AudioDuration": CmfcAudioDurationType,
+        "CslgAtom": Mp4CslgAtomType,
+        "CttsVersion": int,
+        "FreeSpaceBox": Mp4FreeSpaceBoxType,
+        "MoovPlacement": Mp4MoovPlacementType,
+        "Mp4MajorBrand": str,
+    },
+    total=False,
+)
+
+MpdSettingsTypeDef = TypedDict(
+    "MpdSettingsTypeDef",
+    {
+        "AccessibilityCaptionHints": MpdAccessibilityCaptionHintsType,
+        "AudioDuration": MpdAudioDurationType,
+        "CaptionContainerType": MpdCaptionContainerTypeType,
+        "KlvMetadata": MpdKlvMetadataType,
+        "ManifestMetadataSignaling": MpdManifestMetadataSignalingType,
+        "Scte35Esam": MpdScte35EsamType,
+        "Scte35Source": MpdScte35SourceType,
+        "TimedMetadata": MpdTimedMetadataType,
+        "TimedMetadataBoxVersion": MpdTimedMetadataBoxVersionType,
+        "TimedMetadataSchemeIdUri": str,
+        "TimedMetadataValue": str,
+    },
+    total=False,
+)
+
 HopDestinationTypeDef = TypedDict(
     "HopDestinationTypeDef",
     {
         "Priority": int,
         "Queue": str,
         "WaitMinutes": int,
     },
@@ -1466,15 +2097,14 @@
 
 DashAdditionalManifestOutputTypeDef = TypedDict(
     "DashAdditionalManifestOutputTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": List[str],
     },
-    total=False,
 )
 
 DashAdditionalManifestTypeDef = TypedDict(
     "DashAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
@@ -1486,41 +2116,61 @@
     "SpekeKeyProviderOutputTypeDef",
     {
         "CertificateArn": str,
         "ResourceId": str,
         "SystemIds": List[str],
         "Url": str,
     },
-    total=False,
 )
 
 SpekeKeyProviderTypeDef = TypedDict(
     "SpekeKeyProviderTypeDef",
     {
         "CertificateArn": str,
         "ResourceId": str,
         "SystemIds": Sequence[str],
         "Url": str,
     },
     total=False,
 )
 
+DashIsoImageBasedTrickPlaySettingsOutputTypeDef = TypedDict(
+    "DashIsoImageBasedTrickPlaySettingsOutputTypeDef",
+    {
+        "IntervalCadence": DashIsoIntervalCadenceType,
+        "ThumbnailHeight": int,
+        "ThumbnailInterval": float,
+        "ThumbnailWidth": int,
+        "TileHeight": int,
+        "TileWidth": int,
+    },
+)
+
 DashIsoImageBasedTrickPlaySettingsTypeDef = TypedDict(
     "DashIsoImageBasedTrickPlaySettingsTypeDef",
     {
         "IntervalCadence": DashIsoIntervalCadenceType,
         "ThumbnailHeight": int,
         "ThumbnailInterval": float,
         "ThumbnailWidth": int,
         "TileHeight": int,
         "TileWidth": int,
     },
     total=False,
 )
 
+DeinterlacerOutputTypeDef = TypedDict(
+    "DeinterlacerOutputTypeDef",
+    {
+        "Algorithm": DeinterlaceAlgorithmType,
+        "Control": DeinterlacerControlType,
+        "Mode": DeinterlacerModeType,
+    },
+)
+
 DeinterlacerTypeDef = TypedDict(
     "DeinterlacerTypeDef",
     {
         "Algorithm": DeinterlaceAlgorithmType,
         "Control": DeinterlacerControlType,
         "Mode": DeinterlacerModeType,
     },
@@ -1569,87 +2219,152 @@
 )
 
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "Url": str,
     },
-    total=False,
 )
 
 DisassociateCertificateRequestRequestTypeDef = TypedDict(
     "DisassociateCertificateRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
+DolbyVisionLevel6MetadataOutputTypeDef = TypedDict(
+    "DolbyVisionLevel6MetadataOutputTypeDef",
+    {
+        "MaxCll": int,
+        "MaxFall": int,
+    },
+)
+
 DolbyVisionLevel6MetadataTypeDef = TypedDict(
     "DolbyVisionLevel6MetadataTypeDef",
     {
         "MaxCll": int,
         "MaxFall": int,
     },
     total=False,
 )
 
+DvbNitSettingsOutputTypeDef = TypedDict(
+    "DvbNitSettingsOutputTypeDef",
+    {
+        "NetworkId": int,
+        "NetworkName": str,
+        "NitInterval": int,
+    },
+)
+
 DvbNitSettingsTypeDef = TypedDict(
     "DvbNitSettingsTypeDef",
     {
         "NetworkId": int,
         "NetworkName": str,
         "NitInterval": int,
     },
     total=False,
 )
 
+DvbSdtSettingsOutputTypeDef = TypedDict(
+    "DvbSdtSettingsOutputTypeDef",
+    {
+        "OutputSdt": OutputSdtType,
+        "SdtInterval": int,
+        "ServiceName": str,
+        "ServiceProviderName": str,
+    },
+)
+
 DvbSdtSettingsTypeDef = TypedDict(
     "DvbSdtSettingsTypeDef",
     {
         "OutputSdt": OutputSdtType,
         "SdtInterval": int,
         "ServiceName": str,
         "ServiceProviderName": str,
     },
     total=False,
 )
 
+DvbTdtSettingsOutputTypeDef = TypedDict(
+    "DvbTdtSettingsOutputTypeDef",
+    {
+        "TdtInterval": int,
+    },
+)
+
 DvbTdtSettingsTypeDef = TypedDict(
     "DvbTdtSettingsTypeDef",
     {
         "TdtInterval": int,
     },
     total=False,
 )
 
+EsamManifestConfirmConditionNotificationOutputTypeDef = TypedDict(
+    "EsamManifestConfirmConditionNotificationOutputTypeDef",
+    {
+        "MccXml": str,
+    },
+)
+
 EsamManifestConfirmConditionNotificationTypeDef = TypedDict(
     "EsamManifestConfirmConditionNotificationTypeDef",
     {
         "MccXml": str,
     },
     total=False,
 )
 
+EsamSignalProcessingNotificationOutputTypeDef = TypedDict(
+    "EsamSignalProcessingNotificationOutputTypeDef",
+    {
+        "SccXml": str,
+    },
+)
+
 EsamSignalProcessingNotificationTypeDef = TypedDict(
     "EsamSignalProcessingNotificationTypeDef",
     {
         "SccXml": str,
     },
     total=False,
 )
 
+ExtendedDataServicesOutputTypeDef = TypedDict(
+    "ExtendedDataServicesOutputTypeDef",
+    {
+        "CopyProtectionAction": CopyProtectionActionType,
+        "VchipAction": VchipActionType,
+    },
+)
+
 ExtendedDataServicesTypeDef = TypedDict(
     "ExtendedDataServicesTypeDef",
     {
         "CopyProtectionAction": CopyProtectionActionType,
         "VchipAction": VchipActionType,
     },
     total=False,
 )
 
+FrameCaptureSettingsOutputTypeDef = TypedDict(
+    "FrameCaptureSettingsOutputTypeDef",
+    {
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "MaxCaptures": int,
+        "Quality": int,
+    },
+)
+
 FrameCaptureSettingsTypeDef = TypedDict(
     "FrameCaptureSettingsTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
         "MaxCaptures": int,
         "Quality": int,
@@ -1667,22 +2382,21 @@
 GetJobTemplateRequestRequestTypeDef = TypedDict(
     "GetJobTemplateRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-PolicyTypeDef = TypedDict(
-    "PolicyTypeDef",
+PolicyOutputTypeDef = TypedDict(
+    "PolicyOutputTypeDef",
     {
         "HttpInputs": InputPolicyType,
         "HttpsInputs": InputPolicyType,
         "S3Inputs": InputPolicyType,
     },
-    total=False,
 )
 
 GetPresetRequestRequestTypeDef = TypedDict(
     "GetPresetRequestRequestTypeDef",
     {
         "Name": str,
     },
@@ -1691,34 +2405,60 @@
 GetQueueRequestRequestTypeDef = TypedDict(
     "GetQueueRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+H264QvbrSettingsOutputTypeDef = TypedDict(
+    "H264QvbrSettingsOutputTypeDef",
+    {
+        "MaxAverageBitrate": int,
+        "QvbrQualityLevel": int,
+        "QvbrQualityLevelFineTune": float,
+    },
+)
+
 H264QvbrSettingsTypeDef = TypedDict(
     "H264QvbrSettingsTypeDef",
     {
         "MaxAverageBitrate": int,
         "QvbrQualityLevel": int,
         "QvbrQualityLevelFineTune": float,
     },
     total=False,
 )
 
+H265QvbrSettingsOutputTypeDef = TypedDict(
+    "H265QvbrSettingsOutputTypeDef",
+    {
+        "MaxAverageBitrate": int,
+        "QvbrQualityLevel": int,
+        "QvbrQualityLevelFineTune": float,
+    },
+)
+
 H265QvbrSettingsTypeDef = TypedDict(
     "H265QvbrSettingsTypeDef",
     {
         "MaxAverageBitrate": int,
         "QvbrQualityLevel": int,
         "QvbrQualityLevelFineTune": float,
     },
     total=False,
 )
 
+Hdr10PlusOutputTypeDef = TypedDict(
+    "Hdr10PlusOutputTypeDef",
+    {
+        "MasteringMonitorNits": int,
+        "TargetMonitorNits": int,
+    },
+)
+
 Hdr10PlusTypeDef = TypedDict(
     "Hdr10PlusTypeDef",
     {
         "MasteringMonitorNits": int,
         "TargetMonitorNits": int,
     },
     total=False,
@@ -1726,73 +2466,127 @@
 
 HlsAdditionalManifestOutputTypeDef = TypedDict(
     "HlsAdditionalManifestOutputTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": List[str],
     },
-    total=False,
 )
 
 HlsAdditionalManifestTypeDef = TypedDict(
     "HlsAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
     },
     total=False,
 )
 
+HlsCaptionLanguageMappingOutputTypeDef = TypedDict(
+    "HlsCaptionLanguageMappingOutputTypeDef",
+    {
+        "CaptionChannel": int,
+        "CustomLanguageCode": str,
+        "LanguageCode": LanguageCodeType,
+        "LanguageDescription": str,
+    },
+)
+
 HlsCaptionLanguageMappingTypeDef = TypedDict(
     "HlsCaptionLanguageMappingTypeDef",
     {
         "CaptionChannel": int,
         "CustomLanguageCode": str,
         "LanguageCode": LanguageCodeType,
         "LanguageDescription": str,
     },
     total=False,
 )
 
+HlsImageBasedTrickPlaySettingsOutputTypeDef = TypedDict(
+    "HlsImageBasedTrickPlaySettingsOutputTypeDef",
+    {
+        "IntervalCadence": HlsIntervalCadenceType,
+        "ThumbnailHeight": int,
+        "ThumbnailInterval": float,
+        "ThumbnailWidth": int,
+        "TileHeight": int,
+        "TileWidth": int,
+    },
+)
+
 HlsImageBasedTrickPlaySettingsTypeDef = TypedDict(
     "HlsImageBasedTrickPlaySettingsTypeDef",
     {
         "IntervalCadence": HlsIntervalCadenceType,
         "ThumbnailHeight": int,
         "ThumbnailInterval": float,
         "ThumbnailWidth": int,
         "TileHeight": int,
         "TileWidth": int,
     },
     total=False,
 )
 
-HlsSettingsTypeDef = TypedDict(
-    "HlsSettingsTypeDef",
+HlsSettingsOutputTypeDef = TypedDict(
+    "HlsSettingsOutputTypeDef",
     {
         "AudioGroupId": str,
         "AudioOnlyContainer": HlsAudioOnlyContainerType,
         "AudioRenditionSets": str,
         "AudioTrackType": HlsAudioTrackTypeType,
         "DescriptiveVideoServiceFlag": HlsDescriptiveVideoServiceFlagType,
         "IFrameOnlyManifest": HlsIFrameOnlyManifestType,
         "SegmentModifier": str,
     },
-    total=False,
+)
+
+HopDestinationOutputTypeDef = TypedDict(
+    "HopDestinationOutputTypeDef",
+    {
+        "Priority": int,
+        "Queue": str,
+        "WaitMinutes": int,
+    },
+)
+
+Id3InsertionOutputTypeDef = TypedDict(
+    "Id3InsertionOutputTypeDef",
+    {
+        "Id3": str,
+        "Timecode": str,
+    },
 )
 
 Id3InsertionTypeDef = TypedDict(
     "Id3InsertionTypeDef",
     {
         "Id3": str,
         "Timecode": str,
     },
     total=False,
 )
 
+InsertableImageOutputTypeDef = TypedDict(
+    "InsertableImageOutputTypeDef",
+    {
+        "Duration": int,
+        "FadeIn": int,
+        "FadeOut": int,
+        "Height": int,
+        "ImageInserterInput": str,
+        "ImageX": int,
+        "ImageY": int,
+        "Layer": int,
+        "Opacity": int,
+        "StartTime": str,
+        "Width": int,
+    },
+)
+
 InsertableImageTypeDef = TypedDict(
     "InsertableImageTypeDef",
     {
         "Duration": int,
         "FadeIn": int,
         "FadeOut": int,
         "Height": int,
@@ -1803,60 +2597,148 @@
         "Opacity": int,
         "StartTime": str,
         "Width": int,
     },
     total=False,
 )
 
+InputClippingOutputTypeDef = TypedDict(
+    "InputClippingOutputTypeDef",
+    {
+        "EndTimecode": str,
+        "StartTimecode": str,
+    },
+)
+
 InputClippingTypeDef = TypedDict(
     "InputClippingTypeDef",
     {
         "EndTimecode": str,
         "StartTimecode": str,
     },
     total=False,
 )
 
+InputDecryptionSettingsOutputTypeDef = TypedDict(
+    "InputDecryptionSettingsOutputTypeDef",
+    {
+        "DecryptionMode": DecryptionModeType,
+        "EncryptedDecryptionKey": str,
+        "InitializationVector": str,
+        "KmsKeyRegion": str,
+    },
+)
+
 InputDecryptionSettingsTypeDef = TypedDict(
     "InputDecryptionSettingsTypeDef",
     {
         "DecryptionMode": DecryptionModeType,
         "EncryptedDecryptionKey": str,
         "InitializationVector": str,
         "KmsKeyRegion": str,
     },
     total=False,
 )
 
-InputVideoGeneratorTypeDef = TypedDict(
-    "InputVideoGeneratorTypeDef",
+InputVideoGeneratorOutputTypeDef = TypedDict(
+    "InputVideoGeneratorOutputTypeDef",
     {
         "Duration": int,
     },
-    total=False,
+)
+
+RectangleOutputTypeDef = TypedDict(
+    "RectangleOutputTypeDef",
+    {
+        "Height": int,
+        "Width": int,
+        "X": int,
+        "Y": int,
+    },
 )
 
 RectangleTypeDef = TypedDict(
     "RectangleTypeDef",
     {
         "Height": int,
         "Width": int,
         "X": int,
         "Y": int,
     },
     total=False,
 )
 
+InputVideoGeneratorTypeDef = TypedDict(
+    "InputVideoGeneratorTypeDef",
+    {
+        "Duration": int,
+    },
+    total=False,
+)
+
 JobMessagesTypeDef = TypedDict(
     "JobMessagesTypeDef",
     {
         "Info": List[str],
         "Warning": List[str],
     },
-    total=False,
+)
+
+KantarWatermarkSettingsOutputTypeDef = TypedDict(
+    "KantarWatermarkSettingsOutputTypeDef",
+    {
+        "ChannelName": str,
+        "ContentReference": str,
+        "CredentialsSecretName": str,
+        "FileOffset": float,
+        "KantarLicenseId": int,
+        "KantarServerUrl": str,
+        "LogDestination": str,
+        "Metadata3": str,
+        "Metadata4": str,
+        "Metadata5": str,
+        "Metadata6": str,
+        "Metadata7": str,
+        "Metadata8": str,
+    },
+)
+
+NielsenConfigurationOutputTypeDef = TypedDict(
+    "NielsenConfigurationOutputTypeDef",
+    {
+        "BreakoutCode": int,
+        "DistributorId": str,
+    },
+)
+
+NielsenNonLinearWatermarkSettingsOutputTypeDef = TypedDict(
+    "NielsenNonLinearWatermarkSettingsOutputTypeDef",
+    {
+        "ActiveWatermarkProcess": NielsenActiveWatermarkProcessTypeType,
+        "AdiFilename": str,
+        "AssetId": str,
+        "AssetName": str,
+        "CbetSourceId": str,
+        "EpisodeId": str,
+        "MetadataDestination": str,
+        "SourceId": int,
+        "SourceWatermarkStatus": NielsenSourceWatermarkStatusTypeType,
+        "TicServerUrl": str,
+        "UniqueTicPerAudioTrack": NielsenUniqueTicPerAudioTrackTypeType,
+    },
+)
+
+TimecodeConfigOutputTypeDef = TypedDict(
+    "TimecodeConfigOutputTypeDef",
+    {
+        "Anchor": str,
+        "Source": TimecodeSourceType,
+        "Start": str,
+        "TimestampOffset": str,
+    },
 )
 
 KantarWatermarkSettingsTypeDef = TypedDict(
     "KantarWatermarkSettingsTypeDef",
     {
         "ChannelName": str,
         "ContentReference": str,
@@ -1916,25 +2798,23 @@
 QueueTransitionTypeDef = TypedDict(
     "QueueTransitionTypeDef",
     {
         "DestinationQueue": str,
         "SourceQueue": str,
         "Timestamp": datetime,
     },
-    total=False,
 )
 
 TimingTypeDef = TypedDict(
     "TimingTypeDef",
     {
         "FinishTime": datetime,
         "StartTime": datetime,
         "SubmitTime": datetime,
     },
-    total=False,
 )
 
 WarningGroupTypeDef = TypedDict(
     "WarningGroupTypeDef",
     {
         "Code": int,
         "Count": int,
@@ -1997,25 +2877,47 @@
 
 ResourceTagsTypeDef = TypedDict(
     "ResourceTagsTypeDef",
     {
         "Arn": str,
         "Tags": Dict[str, str],
     },
-    total=False,
+)
+
+M2tsScte35EsamOutputTypeDef = TypedDict(
+    "M2tsScte35EsamOutputTypeDef",
+    {
+        "Scte35EsamPid": int,
+    },
 )
 
 M2tsScte35EsamTypeDef = TypedDict(
     "M2tsScte35EsamTypeDef",
     {
         "Scte35EsamPid": int,
     },
     total=False,
 )
 
+MotionImageInsertionFramerateOutputTypeDef = TypedDict(
+    "MotionImageInsertionFramerateOutputTypeDef",
+    {
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+    },
+)
+
+MotionImageInsertionOffsetOutputTypeDef = TypedDict(
+    "MotionImageInsertionOffsetOutputTypeDef",
+    {
+        "ImageX": int,
+        "ImageY": int,
+    },
+)
+
 MotionImageInsertionFramerateTypeDef = TypedDict(
     "MotionImageInsertionFramerateTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
     },
     total=False,
@@ -2026,14 +2928,53 @@
     {
         "ImageX": int,
         "ImageY": int,
     },
     total=False,
 )
 
+Mpeg2SettingsOutputTypeDef = TypedDict(
+    "Mpeg2SettingsOutputTypeDef",
+    {
+        "AdaptiveQuantization": Mpeg2AdaptiveQuantizationType,
+        "Bitrate": int,
+        "CodecLevel": Mpeg2CodecLevelType,
+        "CodecProfile": Mpeg2CodecProfileType,
+        "DynamicSubGop": Mpeg2DynamicSubGopType,
+        "FramerateControl": Mpeg2FramerateControlType,
+        "FramerateConversionAlgorithm": Mpeg2FramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "GopClosedCadence": int,
+        "GopSize": float,
+        "GopSizeUnits": Mpeg2GopSizeUnitsType,
+        "HrdBufferFinalFillPercentage": int,
+        "HrdBufferInitialFillPercentage": int,
+        "HrdBufferSize": int,
+        "InterlaceMode": Mpeg2InterlaceModeType,
+        "IntraDcPrecision": Mpeg2IntraDcPrecisionType,
+        "MaxBitrate": int,
+        "MinIInterval": int,
+        "NumberBFramesBetweenReferenceFrames": int,
+        "ParControl": Mpeg2ParControlType,
+        "ParDenominator": int,
+        "ParNumerator": int,
+        "QualityTuningLevel": Mpeg2QualityTuningLevelType,
+        "RateControlMode": Mpeg2RateControlModeType,
+        "ScanTypeConversionMode": Mpeg2ScanTypeConversionModeType,
+        "SceneChangeDetect": Mpeg2SceneChangeDetectType,
+        "SlowPal": Mpeg2SlowPalType,
+        "Softness": int,
+        "SpatialAdaptiveQuantization": Mpeg2SpatialAdaptiveQuantizationType,
+        "Syntax": Mpeg2SyntaxType,
+        "Telecine": Mpeg2TelecineType,
+        "TemporalAdaptiveQuantization": Mpeg2TemporalAdaptiveQuantizationType,
+    },
+)
+
 Mpeg2SettingsTypeDef = TypedDict(
     "Mpeg2SettingsTypeDef",
     {
         "AdaptiveQuantization": Mpeg2AdaptiveQuantizationType,
         "Bitrate": int,
         "CodecLevel": Mpeg2CodecLevelType,
         "CodecProfile": Mpeg2CodecProfileType,
@@ -2072,54 +3013,98 @@
 
 MsSmoothAdditionalManifestOutputTypeDef = TypedDict(
     "MsSmoothAdditionalManifestOutputTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": List[str],
     },
-    total=False,
 )
 
 MsSmoothAdditionalManifestTypeDef = TypedDict(
     "MsSmoothAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
     },
     total=False,
 )
 
+MxfXavcProfileSettingsOutputTypeDef = TypedDict(
+    "MxfXavcProfileSettingsOutputTypeDef",
+    {
+        "DurationMode": MxfXavcDurationModeType,
+        "MaxAncDataSize": int,
+    },
+)
+
 MxfXavcProfileSettingsTypeDef = TypedDict(
     "MxfXavcProfileSettingsTypeDef",
     {
         "DurationMode": MxfXavcDurationModeType,
         "MaxAncDataSize": int,
     },
     total=False,
 )
 
+NexGuardFileMarkerSettingsOutputTypeDef = TypedDict(
+    "NexGuardFileMarkerSettingsOutputTypeDef",
+    {
+        "License": str,
+        "Payload": int,
+        "Preset": str,
+        "Strength": WatermarkingStrengthType,
+    },
+)
+
 NexGuardFileMarkerSettingsTypeDef = TypedDict(
     "NexGuardFileMarkerSettingsTypeDef",
     {
         "License": str,
         "Payload": int,
         "Preset": str,
         "Strength": WatermarkingStrengthType,
     },
     total=False,
 )
 
+NoiseReducerFilterSettingsOutputTypeDef = TypedDict(
+    "NoiseReducerFilterSettingsOutputTypeDef",
+    {
+        "Strength": int,
+    },
+)
+
 NoiseReducerFilterSettingsTypeDef = TypedDict(
     "NoiseReducerFilterSettingsTypeDef",
     {
         "Strength": int,
     },
     total=False,
 )
 
+NoiseReducerSpatialFilterSettingsOutputTypeDef = TypedDict(
+    "NoiseReducerSpatialFilterSettingsOutputTypeDef",
+    {
+        "PostFilterSharpenStrength": int,
+        "Speed": int,
+        "Strength": int,
+    },
+)
+
+NoiseReducerTemporalFilterSettingsOutputTypeDef = TypedDict(
+    "NoiseReducerTemporalFilterSettingsOutputTypeDef",
+    {
+        "AggressiveMode": int,
+        "PostTemporalSharpening": NoiseFilterPostTemporalSharpeningType,
+        "PostTemporalSharpeningStrength": NoiseFilterPostTemporalSharpeningStrengthType,
+        "Speed": int,
+        "Strength": int,
+    },
+)
+
 NoiseReducerSpatialFilterSettingsTypeDef = TypedDict(
     "NoiseReducerSpatialFilterSettingsTypeDef",
     {
         "PostFilterSharpenStrength": int,
         "Speed": int,
         "Strength": int,
     },
@@ -2140,17 +3125,45 @@
 
 VideoDetailTypeDef = TypedDict(
     "VideoDetailTypeDef",
     {
         "HeightInPx": int,
         "WidthInPx": int,
     },
+)
+
+PolicyTypeDef = TypedDict(
+    "PolicyTypeDef",
+    {
+        "HttpInputs": InputPolicyType,
+        "HttpsInputs": InputPolicyType,
+        "S3Inputs": InputPolicyType,
+    },
     total=False,
 )
 
+ProresSettingsOutputTypeDef = TypedDict(
+    "ProresSettingsOutputTypeDef",
+    {
+        "ChromaSampling": ProresChromaSamplingType,
+        "CodecProfile": ProresCodecProfileType,
+        "FramerateControl": ProresFramerateControlType,
+        "FramerateConversionAlgorithm": ProresFramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "InterlaceMode": ProresInterlaceModeType,
+        "ParControl": ProresParControlType,
+        "ParDenominator": int,
+        "ParNumerator": int,
+        "ScanTypeConversionMode": ProresScanTypeConversionModeType,
+        "SlowPal": ProresSlowPalType,
+        "Telecine": ProresTelecineType,
+    },
+)
+
 ProresSettingsTypeDef = TypedDict(
     "ProresSettingsTypeDef",
     {
         "ChromaSampling": ProresChromaSamplingType,
         "CodecProfile": ProresCodecProfileType,
         "FramerateControl": ProresFramerateControlType,
         "FramerateConversionAlgorithm": ProresFramerateConversionAlgorithmType,
@@ -2173,25 +3186,40 @@
         "Commitment": Literal["ONE_YEAR"],
         "ExpiresAt": datetime,
         "PurchasedAt": datetime,
         "RenewalType": RenewalTypeType,
         "ReservedSlots": int,
         "Status": ReservationPlanStatusType,
     },
-    total=False,
+)
+
+S3DestinationAccessControlOutputTypeDef = TypedDict(
+    "S3DestinationAccessControlOutputTypeDef",
+    {
+        "CannedAcl": S3ObjectCannedAclType,
+    },
 )
 
 S3DestinationAccessControlTypeDef = TypedDict(
     "S3DestinationAccessControlTypeDef",
     {
         "CannedAcl": S3ObjectCannedAclType,
     },
     total=False,
 )
 
+S3EncryptionSettingsOutputTypeDef = TypedDict(
+    "S3EncryptionSettingsOutputTypeDef",
+    {
+        "EncryptionType": S3ServerSideEncryptionTypeType,
+        "KmsEncryptionContext": str,
+        "KmsKeyArn": str,
+    },
+)
+
 S3EncryptionSettingsTypeDef = TypedDict(
     "S3EncryptionSettingsTypeDef",
     {
         "EncryptionType": S3ServerSideEncryptionTypeType,
         "KmsEncryptionContext": str,
         "KmsKeyArn": str,
     },
@@ -2202,14 +3230,23 @@
     "TagResourceRequestRequestTypeDef",
     {
         "Arn": str,
         "Tags": Mapping[str, str],
     },
 )
 
+TimecodeBurninOutputTypeDef = TypedDict(
+    "TimecodeBurninOutputTypeDef",
+    {
+        "FontSize": int,
+        "Position": TimecodeBurninPositionType,
+        "Prefix": str,
+    },
+)
+
 TimecodeBurninTypeDef = TypedDict(
     "TimecodeBurninTypeDef",
     {
         "FontSize": int,
         "Position": TimecodeBurninPositionType,
         "Prefix": str,
     },
@@ -2233,14 +3270,29 @@
 
 class UntagResourceRequestRequestTypeDef(
     _RequiredUntagResourceRequestRequestTypeDef, _OptionalUntagResourceRequestRequestTypeDef
 ):
     pass
 
 
+Vc3SettingsOutputTypeDef = TypedDict(
+    "Vc3SettingsOutputTypeDef",
+    {
+        "FramerateControl": Vc3FramerateControlType,
+        "FramerateConversionAlgorithm": Vc3FramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "InterlaceMode": Vc3InterlaceModeType,
+        "ScanTypeConversionMode": Vc3ScanTypeConversionModeType,
+        "SlowPal": Vc3SlowPalType,
+        "Telecine": Vc3TelecineType,
+        "Vc3Class": Vc3ClassType,
+    },
+)
+
 Vc3SettingsTypeDef = TypedDict(
     "Vc3SettingsTypeDef",
     {
         "FramerateControl": Vc3FramerateControlType,
         "FramerateConversionAlgorithm": Vc3FramerateConversionAlgorithmType,
         "FramerateDenominator": int,
         "FramerateNumerator": int,
@@ -2249,14 +3301,52 @@
         "SlowPal": Vc3SlowPalType,
         "Telecine": Vc3TelecineType,
         "Vc3Class": Vc3ClassType,
     },
     total=False,
 )
 
+Vp8SettingsOutputTypeDef = TypedDict(
+    "Vp8SettingsOutputTypeDef",
+    {
+        "Bitrate": int,
+        "FramerateControl": Vp8FramerateControlType,
+        "FramerateConversionAlgorithm": Vp8FramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "GopSize": float,
+        "HrdBufferSize": int,
+        "MaxBitrate": int,
+        "ParControl": Vp8ParControlType,
+        "ParDenominator": int,
+        "ParNumerator": int,
+        "QualityTuningLevel": Vp8QualityTuningLevelType,
+        "RateControlMode": Literal["VBR"],
+    },
+)
+
+Vp9SettingsOutputTypeDef = TypedDict(
+    "Vp9SettingsOutputTypeDef",
+    {
+        "Bitrate": int,
+        "FramerateControl": Vp9FramerateControlType,
+        "FramerateConversionAlgorithm": Vp9FramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "GopSize": float,
+        "HrdBufferSize": int,
+        "MaxBitrate": int,
+        "ParControl": Vp9ParControlType,
+        "ParDenominator": int,
+        "ParNumerator": int,
+        "QualityTuningLevel": Vp9QualityTuningLevelType,
+        "RateControlMode": Literal["VBR"],
+    },
+)
+
 Vp8SettingsTypeDef = TypedDict(
     "Vp8SettingsTypeDef",
     {
         "Bitrate": int,
         "FramerateControl": Vp8FramerateControlType,
         "FramerateConversionAlgorithm": Vp8FramerateConversionAlgorithmType,
         "FramerateDenominator": int,
@@ -2289,30 +3379,58 @@
         "ParNumerator": int,
         "QualityTuningLevel": Vp9QualityTuningLevelType,
         "RateControlMode": Literal["VBR"],
     },
     total=False,
 )
 
+Xavc4kIntraCbgProfileSettingsOutputTypeDef = TypedDict(
+    "Xavc4kIntraCbgProfileSettingsOutputTypeDef",
+    {
+        "XavcClass": Xavc4kIntraCbgProfileClassType,
+    },
+)
+
 Xavc4kIntraCbgProfileSettingsTypeDef = TypedDict(
     "Xavc4kIntraCbgProfileSettingsTypeDef",
     {
         "XavcClass": Xavc4kIntraCbgProfileClassType,
     },
     total=False,
 )
 
+Xavc4kIntraVbrProfileSettingsOutputTypeDef = TypedDict(
+    "Xavc4kIntraVbrProfileSettingsOutputTypeDef",
+    {
+        "XavcClass": Xavc4kIntraVbrProfileClassType,
+    },
+)
+
 Xavc4kIntraVbrProfileSettingsTypeDef = TypedDict(
     "Xavc4kIntraVbrProfileSettingsTypeDef",
     {
         "XavcClass": Xavc4kIntraVbrProfileClassType,
     },
     total=False,
 )
 
+Xavc4kProfileSettingsOutputTypeDef = TypedDict(
+    "Xavc4kProfileSettingsOutputTypeDef",
+    {
+        "BitrateClass": Xavc4kProfileBitrateClassType,
+        "CodecProfile": Xavc4kProfileCodecProfileType,
+        "FlickerAdaptiveQuantization": XavcFlickerAdaptiveQuantizationType,
+        "GopBReference": XavcGopBReferenceType,
+        "GopClosedCadence": int,
+        "HrdBufferSize": int,
+        "QualityTuningLevel": Xavc4kProfileQualityTuningLevelType,
+        "Slices": int,
+    },
+)
+
 Xavc4kProfileSettingsTypeDef = TypedDict(
     "Xavc4kProfileSettingsTypeDef",
     {
         "BitrateClass": Xavc4kProfileBitrateClassType,
         "CodecProfile": Xavc4kProfileCodecProfileType,
         "FlickerAdaptiveQuantization": XavcFlickerAdaptiveQuantizationType,
         "GopBReference": XavcGopBReferenceType,
@@ -2320,22 +3438,44 @@
         "HrdBufferSize": int,
         "QualityTuningLevel": Xavc4kProfileQualityTuningLevelType,
         "Slices": int,
     },
     total=False,
 )
 
+XavcHdIntraCbgProfileSettingsOutputTypeDef = TypedDict(
+    "XavcHdIntraCbgProfileSettingsOutputTypeDef",
+    {
+        "XavcClass": XavcHdIntraCbgProfileClassType,
+    },
+)
+
 XavcHdIntraCbgProfileSettingsTypeDef = TypedDict(
     "XavcHdIntraCbgProfileSettingsTypeDef",
     {
         "XavcClass": XavcHdIntraCbgProfileClassType,
     },
     total=False,
 )
 
+XavcHdProfileSettingsOutputTypeDef = TypedDict(
+    "XavcHdProfileSettingsOutputTypeDef",
+    {
+        "BitrateClass": XavcHdProfileBitrateClassType,
+        "FlickerAdaptiveQuantization": XavcFlickerAdaptiveQuantizationType,
+        "GopBReference": XavcGopBReferenceType,
+        "GopClosedCadence": int,
+        "HrdBufferSize": int,
+        "InterlaceMode": XavcInterlaceModeType,
+        "QualityTuningLevel": XavcHdProfileQualityTuningLevelType,
+        "Slices": int,
+        "Telecine": XavcHdProfileTelecineType,
+    },
+)
+
 XavcHdProfileSettingsTypeDef = TypedDict(
     "XavcHdProfileSettingsTypeDef",
     {
         "BitrateClass": XavcHdProfileBitrateClassType,
         "FlickerAdaptiveQuantization": XavcFlickerAdaptiveQuantizationType,
         "GopBReference": XavcGopBReferenceType,
         "GopClosedCadence": int,
@@ -2344,14 +3484,31 @@
         "QualityTuningLevel": XavcHdProfileQualityTuningLevelType,
         "Slices": int,
         "Telecine": XavcHdProfileTelecineType,
     },
     total=False,
 )
 
+AudioCodecSettingsOutputTypeDef = TypedDict(
+    "AudioCodecSettingsOutputTypeDef",
+    {
+        "AacSettings": AacSettingsOutputTypeDef,
+        "Ac3Settings": Ac3SettingsOutputTypeDef,
+        "AiffSettings": AiffSettingsOutputTypeDef,
+        "Codec": AudioCodecType,
+        "Eac3AtmosSettings": Eac3AtmosSettingsOutputTypeDef,
+        "Eac3Settings": Eac3SettingsOutputTypeDef,
+        "Mp2Settings": Mp2SettingsOutputTypeDef,
+        "Mp3Settings": Mp3SettingsOutputTypeDef,
+        "OpusSettings": OpusSettingsOutputTypeDef,
+        "VorbisSettings": VorbisSettingsOutputTypeDef,
+        "WavSettings": WavSettingsOutputTypeDef,
+    },
+)
+
 AudioCodecSettingsTypeDef = TypedDict(
     "AudioCodecSettingsTypeDef",
     {
         "AacSettings": AacSettingsTypeDef,
         "Ac3Settings": Ac3SettingsTypeDef,
         "AiffSettings": AiffSettingsTypeDef,
         "Codec": AudioCodecType,
@@ -2365,35 +3522,53 @@
     },
     total=False,
 )
 
 AutomatedAbrRuleOutputTypeDef = TypedDict(
     "AutomatedAbrRuleOutputTypeDef",
     {
-        "AllowedRenditions": List[AllowedRenditionSizeTypeDef],
-        "ForceIncludeRenditions": List[ForceIncludeRenditionSizeTypeDef],
-        "MinBottomRenditionSize": MinBottomRenditionSizeTypeDef,
-        "MinTopRenditionSize": MinTopRenditionSizeTypeDef,
+        "AllowedRenditions": List[AllowedRenditionSizeOutputTypeDef],
+        "ForceIncludeRenditions": List[ForceIncludeRenditionSizeOutputTypeDef],
+        "MinBottomRenditionSize": MinBottomRenditionSizeOutputTypeDef,
+        "MinTopRenditionSize": MinTopRenditionSizeOutputTypeDef,
         "Type": RuleTypeType,
     },
-    total=False,
 )
 
 AutomatedAbrRuleTypeDef = TypedDict(
     "AutomatedAbrRuleTypeDef",
     {
         "AllowedRenditions": Sequence[AllowedRenditionSizeTypeDef],
         "ForceIncludeRenditions": Sequence[ForceIncludeRenditionSizeTypeDef],
         "MinBottomRenditionSize": MinBottomRenditionSizeTypeDef,
         "MinTopRenditionSize": MinTopRenditionSizeTypeDef,
         "Type": RuleTypeType,
     },
     total=False,
 )
 
+Av1SettingsOutputTypeDef = TypedDict(
+    "Av1SettingsOutputTypeDef",
+    {
+        "AdaptiveQuantization": Av1AdaptiveQuantizationType,
+        "BitDepth": Av1BitDepthType,
+        "FramerateControl": Av1FramerateControlType,
+        "FramerateConversionAlgorithm": Av1FramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "GopSize": float,
+        "MaxBitrate": int,
+        "NumberBFramesBetweenReferenceFrames": int,
+        "QvbrSettings": Av1QvbrSettingsOutputTypeDef,
+        "RateControlMode": Literal["QVBR"],
+        "Slices": int,
+        "SpatialAdaptiveQuantization": Av1SpatialAdaptiveQuantizationType,
+    },
+)
+
 Av1SettingsTypeDef = TypedDict(
     "Av1SettingsTypeDef",
     {
         "AdaptiveQuantization": Av1AdaptiveQuantizationType,
         "BitDepth": Av1BitDepthType,
         "FramerateControl": Av1FramerateControlType,
         "FramerateConversionAlgorithm": Av1FramerateConversionAlgorithmType,
@@ -2406,14 +3581,30 @@
         "RateControlMode": Literal["QVBR"],
         "Slices": int,
         "SpatialAdaptiveQuantization": Av1SpatialAdaptiveQuantizationType,
     },
     total=False,
 )
 
+AvcIntraSettingsOutputTypeDef = TypedDict(
+    "AvcIntraSettingsOutputTypeDef",
+    {
+        "AvcIntraClass": AvcIntraClassType,
+        "AvcIntraUhdSettings": AvcIntraUhdSettingsOutputTypeDef,
+        "FramerateControl": AvcIntraFramerateControlType,
+        "FramerateConversionAlgorithm": AvcIntraFramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "InterlaceMode": AvcIntraInterlaceModeType,
+        "ScanTypeConversionMode": AvcIntraScanTypeConversionModeType,
+        "SlowPal": AvcIntraSlowPalType,
+        "Telecine": AvcIntraTelecineType,
+    },
+)
+
 AvcIntraSettingsTypeDef = TypedDict(
     "AvcIntraSettingsTypeDef",
     {
         "AvcIntraClass": AvcIntraClassType,
         "AvcIntraUhdSettings": AvcIntraUhdSettingsTypeDef,
         "FramerateControl": AvcIntraFramerateControlType,
         "FramerateConversionAlgorithm": AvcIntraFramerateConversionAlgorithmType,
@@ -2426,26 +3617,25 @@
     },
     total=False,
 )
 
 CaptionDestinationSettingsOutputTypeDef = TypedDict(
     "CaptionDestinationSettingsOutputTypeDef",
     {
-        "BurninDestinationSettings": BurninDestinationSettingsTypeDef,
+        "BurninDestinationSettings": BurninDestinationSettingsOutputTypeDef,
         "DestinationType": CaptionDestinationTypeType,
-        "DvbSubDestinationSettings": DvbSubDestinationSettingsTypeDef,
-        "EmbeddedDestinationSettings": EmbeddedDestinationSettingsTypeDef,
-        "ImscDestinationSettings": ImscDestinationSettingsTypeDef,
-        "SccDestinationSettings": SccDestinationSettingsTypeDef,
-        "SrtDestinationSettings": SrtDestinationSettingsTypeDef,
+        "DvbSubDestinationSettings": DvbSubDestinationSettingsOutputTypeDef,
+        "EmbeddedDestinationSettings": EmbeddedDestinationSettingsOutputTypeDef,
+        "ImscDestinationSettings": ImscDestinationSettingsOutputTypeDef,
+        "SccDestinationSettings": SccDestinationSettingsOutputTypeDef,
+        "SrtDestinationSettings": SrtDestinationSettingsOutputTypeDef,
         "TeletextDestinationSettings": TeletextDestinationSettingsOutputTypeDef,
-        "TtmlDestinationSettings": TtmlDestinationSettingsTypeDef,
-        "WebvttDestinationSettings": WebvttDestinationSettingsTypeDef,
+        "TtmlDestinationSettings": TtmlDestinationSettingsOutputTypeDef,
+        "WebvttDestinationSettings": WebvttDestinationSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 CaptionDestinationSettingsTypeDef = TypedDict(
     "CaptionDestinationSettingsTypeDef",
     {
         "BurninDestinationSettings": BurninDestinationSettingsTypeDef,
         "DestinationType": CaptionDestinationTypeType,
@@ -2457,14 +3647,26 @@
         "TeletextDestinationSettings": TeletextDestinationSettingsTypeDef,
         "TtmlDestinationSettings": TtmlDestinationSettingsTypeDef,
         "WebvttDestinationSettings": WebvttDestinationSettingsTypeDef,
     },
     total=False,
 )
 
+FileSourceSettingsOutputTypeDef = TypedDict(
+    "FileSourceSettingsOutputTypeDef",
+    {
+        "Convert608To708": FileSourceConvert608To708Type,
+        "ConvertPaintToPop": CaptionSourceConvertPaintOnToPopOnType,
+        "Framerate": CaptionSourceFramerateOutputTypeDef,
+        "SourceFile": str,
+        "TimeDelta": int,
+        "TimeDeltaUnits": FileSourceTimeDeltaUnitsType,
+    },
+)
+
 FileSourceSettingsTypeDef = TypedDict(
     "FileSourceSettingsTypeDef",
     {
         "Convert608To708": FileSourceConvert608To708Type,
         "ConvertPaintToPop": CaptionSourceConvertPaintOnToPopOnType,
         "Framerate": CaptionSourceFramerateTypeDef,
         "SourceFile": str,
@@ -2475,15 +3677,14 @@
 )
 
 ChannelMappingOutputTypeDef = TypedDict(
     "ChannelMappingOutputTypeDef",
     {
         "OutputChannels": List[OutputChannelMappingOutputTypeDef],
     },
-    total=False,
 )
 
 ChannelMappingTypeDef = TypedDict(
     "ChannelMappingTypeDef",
     {
         "OutputChannels": Sequence[OutputChannelMappingTypeDef],
     },
@@ -2493,18 +3694,17 @@
 CmafEncryptionSettingsOutputTypeDef = TypedDict(
     "CmafEncryptionSettingsOutputTypeDef",
     {
         "ConstantInitializationVector": str,
         "EncryptionMethod": CmafEncryptionTypeType,
         "InitializationVectorInManifest": CmafInitializationVectorInManifestType,
         "SpekeKeyProvider": SpekeKeyProviderCmafOutputTypeDef,
-        "StaticKeyProvider": StaticKeyProviderTypeDef,
+        "StaticKeyProvider": StaticKeyProviderOutputTypeDef,
         "Type": CmafKeyProviderTypeType,
     },
-    total=False,
 )
 
 CmafEncryptionSettingsTypeDef = TypedDict(
     "CmafEncryptionSettingsTypeDef",
     {
         "ConstantInitializationVector": str,
         "EncryptionMethod": CmafEncryptionTypeType,
@@ -2512,14 +3712,46 @@
         "SpekeKeyProvider": SpekeKeyProviderCmafTypeDef,
         "StaticKeyProvider": StaticKeyProviderTypeDef,
         "Type": CmafKeyProviderTypeType,
     },
     total=False,
 )
 
+ColorCorrectorOutputTypeDef = TypedDict(
+    "ColorCorrectorOutputTypeDef",
+    {
+        "Brightness": int,
+        "ClipLimits": ClipLimitsOutputTypeDef,
+        "ColorSpaceConversion": ColorSpaceConversionType,
+        "Contrast": int,
+        "Hdr10Metadata": Hdr10MetadataOutputTypeDef,
+        "HdrToSdrToneMapper": HDRToSDRToneMapperType,
+        "Hue": int,
+        "SampleRangeConversion": SampleRangeConversionType,
+        "Saturation": int,
+        "SdrReferenceWhiteLevel": int,
+    },
+)
+
+VideoSelectorOutputTypeDef = TypedDict(
+    "VideoSelectorOutputTypeDef",
+    {
+        "AlphaBehavior": AlphaBehaviorType,
+        "ColorSpace": ColorSpaceType,
+        "ColorSpaceUsage": ColorSpaceUsageType,
+        "EmbeddedTimecodeOverride": EmbeddedTimecodeOverrideType,
+        "Hdr10Metadata": Hdr10MetadataOutputTypeDef,
+        "PadVideo": PadVideoType,
+        "Pid": int,
+        "ProgramNumber": int,
+        "Rotate": InputRotateType,
+        "SampleRange": InputSampleRangeType,
+    },
+)
+
 ColorCorrectorTypeDef = TypedDict(
     "ColorCorrectorTypeDef",
     {
         "Brightness": int,
         "ClipLimits": ClipLimitsTypeDef,
         "ColorSpaceConversion": ColorSpaceConversionType,
         "Contrast": int,
@@ -2600,37 +3832,34 @@
 
 DashIsoEncryptionSettingsOutputTypeDef = TypedDict(
     "DashIsoEncryptionSettingsOutputTypeDef",
     {
         "PlaybackDeviceCompatibility": DashIsoPlaybackDeviceCompatibilityType,
         "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
     },
-    total=False,
 )
 
 HlsEncryptionSettingsOutputTypeDef = TypedDict(
     "HlsEncryptionSettingsOutputTypeDef",
     {
         "ConstantInitializationVector": str,
         "EncryptionMethod": HlsEncryptionTypeType,
         "InitializationVectorInManifest": HlsInitializationVectorInManifestType,
         "OfflineEncrypted": HlsOfflineEncryptedType,
         "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
-        "StaticKeyProvider": StaticKeyProviderTypeDef,
+        "StaticKeyProvider": StaticKeyProviderOutputTypeDef,
         "Type": HlsKeyProviderTypeType,
     },
-    total=False,
 )
 
 MsSmoothEncryptionSettingsOutputTypeDef = TypedDict(
     "MsSmoothEncryptionSettingsOutputTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
     },
-    total=False,
 )
 
 DashIsoEncryptionSettingsTypeDef = TypedDict(
     "DashIsoEncryptionSettingsTypeDef",
     {
         "PlaybackDeviceCompatibility": DashIsoPlaybackDeviceCompatibilityType,
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
@@ -2717,55 +3946,117 @@
     {
         "Endpoints": List[EndpointTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DolbyVisionOutputTypeDef = TypedDict(
+    "DolbyVisionOutputTypeDef",
+    {
+        "L6Metadata": DolbyVisionLevel6MetadataOutputTypeDef,
+        "L6Mode": DolbyVisionLevel6ModeType,
+        "Mapping": DolbyVisionMappingType,
+        "Profile": DolbyVisionProfileType,
+    },
+)
+
 DolbyVisionTypeDef = TypedDict(
     "DolbyVisionTypeDef",
     {
         "L6Metadata": DolbyVisionLevel6MetadataTypeDef,
         "L6Mode": DolbyVisionLevel6ModeType,
         "Mapping": DolbyVisionMappingType,
         "Profile": DolbyVisionProfileType,
     },
     total=False,
 )
 
+EsamSettingsOutputTypeDef = TypedDict(
+    "EsamSettingsOutputTypeDef",
+    {
+        "ManifestConfirmConditionNotification": (
+            EsamManifestConfirmConditionNotificationOutputTypeDef
+        ),
+        "ResponseSignalPreroll": int,
+        "SignalProcessingNotification": EsamSignalProcessingNotificationOutputTypeDef,
+    },
+)
+
 EsamSettingsTypeDef = TypedDict(
     "EsamSettingsTypeDef",
     {
         "ManifestConfirmConditionNotification": EsamManifestConfirmConditionNotificationTypeDef,
         "ResponseSignalPreroll": int,
         "SignalProcessingNotification": EsamSignalProcessingNotificationTypeDef,
     },
     total=False,
 )
 
 GetPolicyResponseTypeDef = TypedDict(
     "GetPolicyResponseTypeDef",
     {
-        "Policy": PolicyTypeDef,
+        "Policy": PolicyOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutPolicyRequestRequestTypeDef = TypedDict(
-    "PutPolicyRequestRequestTypeDef",
+PutPolicyResponseTypeDef = TypedDict(
+    "PutPolicyResponseTypeDef",
     {
-        "Policy": PolicyTypeDef,
+        "Policy": PolicyOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutPolicyResponseTypeDef = TypedDict(
-    "PutPolicyResponseTypeDef",
+H264SettingsOutputTypeDef = TypedDict(
+    "H264SettingsOutputTypeDef",
     {
-        "Policy": PolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AdaptiveQuantization": H264AdaptiveQuantizationType,
+        "BandwidthReductionFilter": BandwidthReductionFilterOutputTypeDef,
+        "Bitrate": int,
+        "CodecLevel": H264CodecLevelType,
+        "CodecProfile": H264CodecProfileType,
+        "DynamicSubGop": H264DynamicSubGopType,
+        "EntropyEncoding": H264EntropyEncodingType,
+        "FieldEncoding": H264FieldEncodingType,
+        "FlickerAdaptiveQuantization": H264FlickerAdaptiveQuantizationType,
+        "FramerateControl": H264FramerateControlType,
+        "FramerateConversionAlgorithm": H264FramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "GopBReference": H264GopBReferenceType,
+        "GopClosedCadence": int,
+        "GopSize": float,
+        "GopSizeUnits": H264GopSizeUnitsType,
+        "HrdBufferFinalFillPercentage": int,
+        "HrdBufferInitialFillPercentage": int,
+        "HrdBufferSize": int,
+        "InterlaceMode": H264InterlaceModeType,
+        "MaxBitrate": int,
+        "MinIInterval": int,
+        "NumberBFramesBetweenReferenceFrames": int,
+        "NumberReferenceFrames": int,
+        "ParControl": H264ParControlType,
+        "ParDenominator": int,
+        "ParNumerator": int,
+        "QualityTuningLevel": H264QualityTuningLevelType,
+        "QvbrSettings": H264QvbrSettingsOutputTypeDef,
+        "RateControlMode": H264RateControlModeType,
+        "RepeatPps": H264RepeatPpsType,
+        "ScanTypeConversionMode": H264ScanTypeConversionModeType,
+        "SceneChangeDetect": H264SceneChangeDetectType,
+        "Slices": int,
+        "SlowPal": H264SlowPalType,
+        "Softness": int,
+        "SpatialAdaptiveQuantization": H264SpatialAdaptiveQuantizationType,
+        "Syntax": H264SyntaxType,
+        "Telecine": H264TelecineType,
+        "TemporalAdaptiveQuantization": H264TemporalAdaptiveQuantizationType,
+        "UnregisteredSeiTimecode": H264UnregisteredSeiTimecodeType,
     },
 )
 
 H264SettingsTypeDef = TypedDict(
     "H264SettingsTypeDef",
     {
         "AdaptiveQuantization": H264AdaptiveQuantizationType,
@@ -2810,14 +4101,62 @@
         "Telecine": H264TelecineType,
         "TemporalAdaptiveQuantization": H264TemporalAdaptiveQuantizationType,
         "UnregisteredSeiTimecode": H264UnregisteredSeiTimecodeType,
     },
     total=False,
 )
 
+H265SettingsOutputTypeDef = TypedDict(
+    "H265SettingsOutputTypeDef",
+    {
+        "AdaptiveQuantization": H265AdaptiveQuantizationType,
+        "AlternateTransferFunctionSei": H265AlternateTransferFunctionSeiType,
+        "BandwidthReductionFilter": BandwidthReductionFilterOutputTypeDef,
+        "Bitrate": int,
+        "CodecLevel": H265CodecLevelType,
+        "CodecProfile": H265CodecProfileType,
+        "DynamicSubGop": H265DynamicSubGopType,
+        "FlickerAdaptiveQuantization": H265FlickerAdaptiveQuantizationType,
+        "FramerateControl": H265FramerateControlType,
+        "FramerateConversionAlgorithm": H265FramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "GopBReference": H265GopBReferenceType,
+        "GopClosedCadence": int,
+        "GopSize": float,
+        "GopSizeUnits": H265GopSizeUnitsType,
+        "HrdBufferFinalFillPercentage": int,
+        "HrdBufferInitialFillPercentage": int,
+        "HrdBufferSize": int,
+        "InterlaceMode": H265InterlaceModeType,
+        "MaxBitrate": int,
+        "MinIInterval": int,
+        "NumberBFramesBetweenReferenceFrames": int,
+        "NumberReferenceFrames": int,
+        "ParControl": H265ParControlType,
+        "ParDenominator": int,
+        "ParNumerator": int,
+        "QualityTuningLevel": H265QualityTuningLevelType,
+        "QvbrSettings": H265QvbrSettingsOutputTypeDef,
+        "RateControlMode": H265RateControlModeType,
+        "SampleAdaptiveOffsetFilterMode": H265SampleAdaptiveOffsetFilterModeType,
+        "ScanTypeConversionMode": H265ScanTypeConversionModeType,
+        "SceneChangeDetect": H265SceneChangeDetectType,
+        "Slices": int,
+        "SlowPal": H265SlowPalType,
+        "SpatialAdaptiveQuantization": H265SpatialAdaptiveQuantizationType,
+        "Telecine": H265TelecineType,
+        "TemporalAdaptiveQuantization": H265TemporalAdaptiveQuantizationType,
+        "TemporalIds": H265TemporalIdsType,
+        "Tiles": H265TilesType,
+        "UnregisteredSeiTimecode": H265UnregisteredSeiTimecodeType,
+        "WriteMp4PackagingType": H265WriteMp4PackagingTypeType,
+    },
+)
+
 H265SettingsTypeDef = TypedDict(
     "H265SettingsTypeDef",
     {
         "AdaptiveQuantization": H265AdaptiveQuantizationType,
         "AlternateTransferFunctionSei": H265AlternateTransferFunctionSeiType,
         "BandwidthReductionFilter": BandwidthReductionFilterTypeDef,
         "Bitrate": int,
@@ -2859,45 +4198,42 @@
         "Tiles": H265TilesType,
         "UnregisteredSeiTimecode": H265UnregisteredSeiTimecodeType,
         "WriteMp4PackagingType": H265WriteMp4PackagingTypeType,
     },
     total=False,
 )
 
-OutputSettingsTypeDef = TypedDict(
-    "OutputSettingsTypeDef",
+OutputSettingsOutputTypeDef = TypedDict(
+    "OutputSettingsOutputTypeDef",
     {
-        "HlsSettings": HlsSettingsTypeDef,
+        "HlsSettings": HlsSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 TimedMetadataInsertionOutputTypeDef = TypedDict(
     "TimedMetadataInsertionOutputTypeDef",
     {
-        "Id3Insertions": List[Id3InsertionTypeDef],
+        "Id3Insertions": List[Id3InsertionOutputTypeDef],
     },
-    total=False,
 )
 
 TimedMetadataInsertionTypeDef = TypedDict(
     "TimedMetadataInsertionTypeDef",
     {
         "Id3Insertions": Sequence[Id3InsertionTypeDef],
     },
     total=False,
 )
 
 ImageInserterOutputTypeDef = TypedDict(
     "ImageInserterOutputTypeDef",
     {
-        "InsertableImages": List[InsertableImageTypeDef],
+        "InsertableImages": List[InsertableImageOutputTypeDef],
         "SdrReferenceWhiteLevel": int,
     },
-    total=False,
 )
 
 ImageInserterTypeDef = TypedDict(
     "ImageInserterTypeDef",
     {
         "InsertableImages": Sequence[InsertableImageTypeDef],
         "SdrReferenceWhiteLevel": int,
@@ -2919,18 +4255,18 @@
         "AudioBufferModel": M2tsAudioBufferModelType,
         "AudioDuration": M2tsAudioDurationType,
         "AudioFramesPerPes": int,
         "AudioPids": List[int],
         "Bitrate": int,
         "BufferModel": M2tsBufferModelType,
         "DataPTSControl": M2tsDataPtsControlType,
-        "DvbNitSettings": DvbNitSettingsTypeDef,
-        "DvbSdtSettings": DvbSdtSettingsTypeDef,
+        "DvbNitSettings": DvbNitSettingsOutputTypeDef,
+        "DvbSdtSettings": DvbSdtSettingsOutputTypeDef,
         "DvbSubPids": List[int],
-        "DvbTdtSettings": DvbTdtSettingsTypeDef,
+        "DvbTdtSettings": DvbTdtSettingsOutputTypeDef,
         "DvbTeletextPid": int,
         "EbpAudioInterval": M2tsEbpAudioIntervalType,
         "EbpPlacement": M2tsEbpPlacementType,
         "EsRateInPes": M2tsEsRateInPesType,
         "ForceTsVideoEbpOrder": M2tsForceTsVideoEbpOrderType,
         "FragmentTime": float,
         "KlvMetadata": M2tsKlvMetadataType,
@@ -2942,25 +4278,24 @@
         "PcrControl": M2tsPcrControlType,
         "PcrPid": int,
         "PmtInterval": int,
         "PmtPid": int,
         "PrivateMetadataPid": int,
         "ProgramNumber": int,
         "RateMode": M2tsRateModeType,
-        "Scte35Esam": M2tsScte35EsamTypeDef,
+        "Scte35Esam": M2tsScte35EsamOutputTypeDef,
         "Scte35Pid": int,
         "Scte35Source": M2tsScte35SourceType,
         "SegmentationMarkers": M2tsSegmentationMarkersType,
         "SegmentationStyle": M2tsSegmentationStyleType,
         "SegmentationTime": float,
         "TimedMetadataPid": int,
         "TransportStreamId": int,
         "VideoPid": int,
     },
-    total=False,
 )
 
 M2tsSettingsTypeDef = TypedDict(
     "M2tsSettingsTypeDef",
     {
         "AudioBufferModel": M2tsAudioBufferModelType,
         "AudioDuration": M2tsAudioDurationType,
@@ -3001,45 +4336,83 @@
         "TimedMetadataPid": int,
         "TransportStreamId": int,
         "VideoPid": int,
     },
     total=False,
 )
 
+MotionImageInserterOutputTypeDef = TypedDict(
+    "MotionImageInserterOutputTypeDef",
+    {
+        "Framerate": MotionImageInsertionFramerateOutputTypeDef,
+        "Input": str,
+        "InsertionMode": MotionImageInsertionModeType,
+        "Offset": MotionImageInsertionOffsetOutputTypeDef,
+        "Playback": MotionImagePlaybackType,
+        "StartTime": str,
+    },
+)
+
 MotionImageInserterTypeDef = TypedDict(
     "MotionImageInserterTypeDef",
     {
         "Framerate": MotionImageInsertionFramerateTypeDef,
         "Input": str,
         "InsertionMode": MotionImageInsertionModeType,
         "Offset": MotionImageInsertionOffsetTypeDef,
         "Playback": MotionImagePlaybackType,
         "StartTime": str,
     },
     total=False,
 )
 
+MxfSettingsOutputTypeDef = TypedDict(
+    "MxfSettingsOutputTypeDef",
+    {
+        "AfdSignaling": MxfAfdSignalingType,
+        "Profile": MxfProfileType,
+        "XavcProfileSettings": MxfXavcProfileSettingsOutputTypeDef,
+    },
+)
+
 MxfSettingsTypeDef = TypedDict(
     "MxfSettingsTypeDef",
     {
         "AfdSignaling": MxfAfdSignalingType,
         "Profile": MxfProfileType,
         "XavcProfileSettings": MxfXavcProfileSettingsTypeDef,
     },
     total=False,
 )
 
+PartnerWatermarkingOutputTypeDef = TypedDict(
+    "PartnerWatermarkingOutputTypeDef",
+    {
+        "NexguardFileMarkerSettings": NexGuardFileMarkerSettingsOutputTypeDef,
+    },
+)
+
 PartnerWatermarkingTypeDef = TypedDict(
     "PartnerWatermarkingTypeDef",
     {
         "NexguardFileMarkerSettings": NexGuardFileMarkerSettingsTypeDef,
     },
     total=False,
 )
 
+NoiseReducerOutputTypeDef = TypedDict(
+    "NoiseReducerOutputTypeDef",
+    {
+        "Filter": NoiseReducerFilterType,
+        "FilterSettings": NoiseReducerFilterSettingsOutputTypeDef,
+        "SpatialFilterSettings": NoiseReducerSpatialFilterSettingsOutputTypeDef,
+        "TemporalFilterSettings": NoiseReducerTemporalFilterSettingsOutputTypeDef,
+    },
+)
+
 NoiseReducerTypeDef = TypedDict(
     "NoiseReducerTypeDef",
     {
         "Filter": NoiseReducerFilterType,
         "FilterSettings": NoiseReducerFilterSettingsTypeDef,
         "SpatialFilterSettings": NoiseReducerSpatialFilterSettingsTypeDef,
         "TemporalFilterSettings": NoiseReducerTemporalFilterSettingsTypeDef,
@@ -3049,54 +4422,79 @@
 
 OutputDetailTypeDef = TypedDict(
     "OutputDetailTypeDef",
     {
         "DurationInMs": int,
         "VideoDetails": VideoDetailTypeDef,
     },
-    total=False,
 )
 
-_RequiredQueueTypeDef = TypedDict(
-    "_RequiredQueueTypeDef",
+PutPolicyRequestRequestTypeDef = TypedDict(
+    "PutPolicyRequestRequestTypeDef",
     {
-        "Name": str,
+        "Policy": PolicyTypeDef,
     },
 )
-_OptionalQueueTypeDef = TypedDict(
-    "_OptionalQueueTypeDef",
+
+QueueTypeDef = TypedDict(
+    "QueueTypeDef",
     {
         "Arn": str,
         "CreatedAt": datetime,
         "Description": str,
         "LastUpdated": datetime,
+        "Name": str,
         "PricingPlan": PricingPlanType,
         "ProgressingJobsCount": int,
         "ReservationPlan": ReservationPlanTypeDef,
         "Status": QueueStatusType,
         "SubmittedJobsCount": int,
         "Type": TypeType,
     },
-    total=False,
 )
 
-
-class QueueTypeDef(_RequiredQueueTypeDef, _OptionalQueueTypeDef):
-    pass
-
+S3DestinationSettingsOutputTypeDef = TypedDict(
+    "S3DestinationSettingsOutputTypeDef",
+    {
+        "AccessControl": S3DestinationAccessControlOutputTypeDef,
+        "Encryption": S3EncryptionSettingsOutputTypeDef,
+    },
+)
 
 S3DestinationSettingsTypeDef = TypedDict(
     "S3DestinationSettingsTypeDef",
     {
         "AccessControl": S3DestinationAccessControlTypeDef,
         "Encryption": S3EncryptionSettingsTypeDef,
     },
     total=False,
 )
 
+XavcSettingsOutputTypeDef = TypedDict(
+    "XavcSettingsOutputTypeDef",
+    {
+        "AdaptiveQuantization": XavcAdaptiveQuantizationType,
+        "EntropyEncoding": XavcEntropyEncodingType,
+        "FramerateControl": XavcFramerateControlType,
+        "FramerateConversionAlgorithm": XavcFramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "Profile": XavcProfileType,
+        "SlowPal": XavcSlowPalType,
+        "Softness": int,
+        "SpatialAdaptiveQuantization": XavcSpatialAdaptiveQuantizationType,
+        "TemporalAdaptiveQuantization": XavcTemporalAdaptiveQuantizationType,
+        "Xavc4kIntraCbgProfileSettings": Xavc4kIntraCbgProfileSettingsOutputTypeDef,
+        "Xavc4kIntraVbrProfileSettings": Xavc4kIntraVbrProfileSettingsOutputTypeDef,
+        "Xavc4kProfileSettings": Xavc4kProfileSettingsOutputTypeDef,
+        "XavcHdIntraCbgProfileSettings": XavcHdIntraCbgProfileSettingsOutputTypeDef,
+        "XavcHdProfileSettings": XavcHdProfileSettingsOutputTypeDef,
+    },
+)
+
 XavcSettingsTypeDef = TypedDict(
     "XavcSettingsTypeDef",
     {
         "AdaptiveQuantization": XavcAdaptiveQuantizationType,
         "EntropyEncoding": XavcEntropyEncodingType,
         "FramerateControl": XavcFramerateControlType,
         "FramerateConversionAlgorithm": XavcFramerateConversionAlgorithmType,
@@ -3120,60 +4518,71 @@
     "AutomatedAbrSettingsOutputTypeDef",
     {
         "MaxAbrBitrate": int,
         "MaxRenditions": int,
         "MinAbrBitrate": int,
         "Rules": List[AutomatedAbrRuleOutputTypeDef],
     },
-    total=False,
 )
 
 AutomatedAbrSettingsTypeDef = TypedDict(
     "AutomatedAbrSettingsTypeDef",
     {
         "MaxAbrBitrate": int,
         "MaxRenditions": int,
         "MinAbrBitrate": int,
         "Rules": Sequence[AutomatedAbrRuleTypeDef],
     },
     total=False,
 )
 
+CaptionDescriptionOutputTypeDef = TypedDict(
+    "CaptionDescriptionOutputTypeDef",
+    {
+        "CaptionSelectorName": str,
+        "CustomLanguageCode": str,
+        "DestinationSettings": CaptionDestinationSettingsOutputTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "LanguageDescription": str,
+    },
+)
+
 CaptionDescriptionPresetOutputTypeDef = TypedDict(
     "CaptionDescriptionPresetOutputTypeDef",
     {
         "CustomLanguageCode": str,
         "DestinationSettings": CaptionDestinationSettingsOutputTypeDef,
         "LanguageCode": LanguageCodeType,
         "LanguageDescription": str,
     },
-    total=False,
 )
 
 CaptionDescriptionPresetTypeDef = TypedDict(
     "CaptionDescriptionPresetTypeDef",
     {
         "CustomLanguageCode": str,
         "DestinationSettings": CaptionDestinationSettingsTypeDef,
         "LanguageCode": LanguageCodeType,
         "LanguageDescription": str,
     },
     total=False,
 )
 
-CaptionDescriptionTypeDef = TypedDict(
-    "CaptionDescriptionTypeDef",
+CaptionSourceSettingsOutputTypeDef = TypedDict(
+    "CaptionSourceSettingsOutputTypeDef",
     {
-        "CaptionSelectorName": str,
-        "CustomLanguageCode": str,
-        "DestinationSettings": CaptionDestinationSettingsTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "LanguageDescription": str,
+        "AncillarySourceSettings": AncillarySourceSettingsOutputTypeDef,
+        "DvbSubSourceSettings": DvbSubSourceSettingsOutputTypeDef,
+        "EmbeddedSourceSettings": EmbeddedSourceSettingsOutputTypeDef,
+        "FileSourceSettings": FileSourceSettingsOutputTypeDef,
+        "SourceType": CaptionSourceTypeType,
+        "TeletextSourceSettings": TeletextSourceSettingsOutputTypeDef,
+        "TrackSourceSettings": TrackSourceSettingsOutputTypeDef,
+        "WebvttHlsSourceSettings": WebvttHlsSourceSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 CaptionSourceSettingsTypeDef = TypedDict(
     "CaptionSourceSettingsTypeDef",
     {
         "AncillarySourceSettings": AncillarySourceSettingsTypeDef,
         "DvbSubSourceSettings": DvbSubSourceSettingsTypeDef,
@@ -3190,15 +4599,14 @@
 RemixSettingsOutputTypeDef = TypedDict(
     "RemixSettingsOutputTypeDef",
     {
         "ChannelMapping": ChannelMappingOutputTypeDef,
         "ChannelsIn": int,
         "ChannelsOut": int,
     },
-    total=False,
 )
 
 RemixSettingsTypeDef = TypedDict(
     "RemixSettingsTypeDef",
     {
         "ChannelMapping": ChannelMappingTypeDef,
         "ChannelsIn": int,
@@ -3206,25 +4614,24 @@
     },
     total=False,
 )
 
 ContainerSettingsOutputTypeDef = TypedDict(
     "ContainerSettingsOutputTypeDef",
     {
-        "CmfcSettings": CmfcSettingsTypeDef,
+        "CmfcSettings": CmfcSettingsOutputTypeDef,
         "Container": ContainerTypeType,
-        "F4vSettings": F4vSettingsTypeDef,
+        "F4vSettings": F4vSettingsOutputTypeDef,
         "M2tsSettings": M2tsSettingsOutputTypeDef,
         "M3u8Settings": M3u8SettingsOutputTypeDef,
-        "MovSettings": MovSettingsTypeDef,
-        "Mp4Settings": Mp4SettingsTypeDef,
-        "MpdSettings": MpdSettingsTypeDef,
-        "MxfSettings": MxfSettingsTypeDef,
+        "MovSettings": MovSettingsOutputTypeDef,
+        "Mp4Settings": Mp4SettingsOutputTypeDef,
+        "MpdSettings": MpdSettingsOutputTypeDef,
+        "MxfSettings": MxfSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 ContainerSettingsTypeDef = TypedDict(
     "ContainerSettingsTypeDef",
     {
         "CmfcSettings": CmfcSettingsTypeDef,
         "Container": ContainerTypeType,
@@ -3238,24 +4645,23 @@
     },
     total=False,
 )
 
 VideoPreprocessorOutputTypeDef = TypedDict(
     "VideoPreprocessorOutputTypeDef",
     {
-        "ColorCorrector": ColorCorrectorTypeDef,
-        "Deinterlacer": DeinterlacerTypeDef,
-        "DolbyVision": DolbyVisionTypeDef,
-        "Hdr10Plus": Hdr10PlusTypeDef,
+        "ColorCorrector": ColorCorrectorOutputTypeDef,
+        "Deinterlacer": DeinterlacerOutputTypeDef,
+        "DolbyVision": DolbyVisionOutputTypeDef,
+        "Hdr10Plus": Hdr10PlusOutputTypeDef,
         "ImageInserter": ImageInserterOutputTypeDef,
-        "NoiseReducer": NoiseReducerTypeDef,
-        "PartnerWatermarking": PartnerWatermarkingTypeDef,
-        "TimecodeBurnin": TimecodeBurninTypeDef,
+        "NoiseReducer": NoiseReducerOutputTypeDef,
+        "PartnerWatermarking": PartnerWatermarkingOutputTypeDef,
+        "TimecodeBurnin": TimecodeBurninOutputTypeDef,
     },
-    total=False,
 )
 
 VideoPreprocessorTypeDef = TypedDict(
     "VideoPreprocessorTypeDef",
     {
         "ColorCorrector": ColorCorrectorTypeDef,
         "Deinterlacer": DeinterlacerTypeDef,
@@ -3270,15 +4676,14 @@
 )
 
 OutputGroupDetailTypeDef = TypedDict(
     "OutputGroupDetailTypeDef",
     {
         "OutputDetails": List[OutputDetailTypeDef],
     },
-    total=False,
 )
 
 CreateQueueResponseTypeDef = TypedDict(
     "CreateQueueResponseTypeDef",
     {
         "Queue": QueueTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3306,22 +4711,47 @@
     "UpdateQueueResponseTypeDef",
     {
         "Queue": QueueTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DestinationSettingsOutputTypeDef = TypedDict(
+    "DestinationSettingsOutputTypeDef",
+    {
+        "S3Settings": S3DestinationSettingsOutputTypeDef,
+    },
+)
+
 DestinationSettingsTypeDef = TypedDict(
     "DestinationSettingsTypeDef",
     {
         "S3Settings": S3DestinationSettingsTypeDef,
     },
     total=False,
 )
 
+VideoCodecSettingsOutputTypeDef = TypedDict(
+    "VideoCodecSettingsOutputTypeDef",
+    {
+        "Av1Settings": Av1SettingsOutputTypeDef,
+        "AvcIntraSettings": AvcIntraSettingsOutputTypeDef,
+        "Codec": VideoCodecType,
+        "FrameCaptureSettings": FrameCaptureSettingsOutputTypeDef,
+        "H264Settings": H264SettingsOutputTypeDef,
+        "H265Settings": H265SettingsOutputTypeDef,
+        "Mpeg2Settings": Mpeg2SettingsOutputTypeDef,
+        "ProresSettings": ProresSettingsOutputTypeDef,
+        "Vc3Settings": Vc3SettingsOutputTypeDef,
+        "Vp8Settings": Vp8SettingsOutputTypeDef,
+        "Vp9Settings": Vp9SettingsOutputTypeDef,
+        "XavcSettings": XavcSettingsOutputTypeDef,
+    },
+)
+
 VideoCodecSettingsTypeDef = TypedDict(
     "VideoCodecSettingsTypeDef",
     {
         "Av1Settings": Av1SettingsTypeDef,
         "AvcIntraSettings": AvcIntraSettingsTypeDef,
         "Codec": VideoCodecType,
         "FrameCaptureSettings": FrameCaptureSettingsTypeDef,
@@ -3338,70 +4768,76 @@
 )
 
 AutomatedEncodingSettingsOutputTypeDef = TypedDict(
     "AutomatedEncodingSettingsOutputTypeDef",
     {
         "AbrSettings": AutomatedAbrSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 AutomatedEncodingSettingsTypeDef = TypedDict(
     "AutomatedEncodingSettingsTypeDef",
     {
         "AbrSettings": AutomatedAbrSettingsTypeDef,
     },
     total=False,
 )
 
+CaptionSelectorOutputTypeDef = TypedDict(
+    "CaptionSelectorOutputTypeDef",
+    {
+        "CustomLanguageCode": str,
+        "LanguageCode": LanguageCodeType,
+        "SourceSettings": CaptionSourceSettingsOutputTypeDef,
+    },
+)
+
 CaptionSelectorTypeDef = TypedDict(
     "CaptionSelectorTypeDef",
     {
         "CustomLanguageCode": str,
         "LanguageCode": LanguageCodeType,
         "SourceSettings": CaptionSourceSettingsTypeDef,
     },
     total=False,
 )
 
 AudioDescriptionOutputTypeDef = TypedDict(
     "AudioDescriptionOutputTypeDef",
     {
-        "AudioChannelTaggingSettings": AudioChannelTaggingSettingsTypeDef,
-        "AudioNormalizationSettings": AudioNormalizationSettingsTypeDef,
+        "AudioChannelTaggingSettings": AudioChannelTaggingSettingsOutputTypeDef,
+        "AudioNormalizationSettings": AudioNormalizationSettingsOutputTypeDef,
         "AudioSourceName": str,
         "AudioType": int,
         "AudioTypeControl": AudioTypeControlType,
-        "CodecSettings": AudioCodecSettingsTypeDef,
+        "CodecSettings": AudioCodecSettingsOutputTypeDef,
         "CustomLanguageCode": str,
         "LanguageCode": LanguageCodeType,
         "LanguageCodeControl": AudioLanguageCodeControlType,
         "RemixSettings": RemixSettingsOutputTypeDef,
         "StreamName": str,
     },
-    total=False,
 )
 
 AudioSelectorOutputTypeDef = TypedDict(
     "AudioSelectorOutputTypeDef",
     {
         "AudioDurationCorrection": AudioDurationCorrectionType,
         "CustomLanguageCode": str,
         "DefaultSelection": AudioDefaultSelectionType,
         "ExternalAudioFileInput": str,
-        "HlsRenditionGroupSettings": HlsRenditionGroupSettingsTypeDef,
+        "HlsRenditionGroupSettings": HlsRenditionGroupSettingsOutputTypeDef,
         "LanguageCode": LanguageCodeType,
         "Offset": int,
         "Pids": List[int],
         "ProgramSelection": int,
         "RemixSettings": RemixSettingsOutputTypeDef,
         "SelectorType": AudioSelectorTypeType,
         "Tracks": List[int],
     },
-    total=False,
 )
 
 AudioDescriptionTypeDef = TypedDict(
     "AudioDescriptionTypeDef",
     {
         "AudioChannelTaggingSettings": AudioChannelTaggingSettingsTypeDef,
         "AudioNormalizationSettings": AudioNormalizationSettingsTypeDef,
@@ -3442,19 +4878,19 @@
     {
         "AdditionalManifests": List[CmafAdditionalManifestOutputTypeDef],
         "BaseUrl": str,
         "ClientCache": CmafClientCacheType,
         "CodecSpecification": CmafCodecSpecificationType,
         "DashManifestStyle": DashManifestStyleType,
         "Destination": str,
-        "DestinationSettings": DestinationSettingsTypeDef,
+        "DestinationSettings": DestinationSettingsOutputTypeDef,
         "Encryption": CmafEncryptionSettingsOutputTypeDef,
         "FragmentLength": int,
         "ImageBasedTrickPlay": CmafImageBasedTrickPlayType,
-        "ImageBasedTrickPlaySettings": CmafImageBasedTrickPlaySettingsTypeDef,
+        "ImageBasedTrickPlaySettings": CmafImageBasedTrickPlaySettingsOutputTypeDef,
         "ManifestCompression": CmafManifestCompressionType,
         "ManifestDurationFormat": CmafManifestDurationFormatType,
         "MinBufferTime": int,
         "MinFinalSegmentLength": float,
         "MpdManifestBandwidthType": CmafMpdManifestBandwidthTypeType,
         "MpdProfile": CmafMpdProfileType,
         "PtsOffsetHandlingForBFrames": CmafPtsOffsetHandlingForBFramesType,
@@ -3464,15 +4900,101 @@
         "StreamInfResolution": CmafStreamInfResolutionType,
         "TargetDurationCompatibilityMode": CmafTargetDurationCompatibilityModeType,
         "VideoCompositionOffsets": CmafVideoCompositionOffsetsType,
         "WriteDashManifest": CmafWriteDASHManifestType,
         "WriteHlsManifest": CmafWriteHLSManifestType,
         "WriteSegmentTimelineInRepresentation": CmafWriteSegmentTimelineInRepresentationType,
     },
-    total=False,
+)
+
+DashIsoGroupSettingsOutputTypeDef = TypedDict(
+    "DashIsoGroupSettingsOutputTypeDef",
+    {
+        "AdditionalManifests": List[DashAdditionalManifestOutputTypeDef],
+        "AudioChannelConfigSchemeIdUri": DashIsoGroupAudioChannelConfigSchemeIdUriType,
+        "BaseUrl": str,
+        "DashManifestStyle": DashManifestStyleType,
+        "Destination": str,
+        "DestinationSettings": DestinationSettingsOutputTypeDef,
+        "Encryption": DashIsoEncryptionSettingsOutputTypeDef,
+        "FragmentLength": int,
+        "HbbtvCompliance": DashIsoHbbtvComplianceType,
+        "ImageBasedTrickPlay": DashIsoImageBasedTrickPlayType,
+        "ImageBasedTrickPlaySettings": DashIsoImageBasedTrickPlaySettingsOutputTypeDef,
+        "MinBufferTime": int,
+        "MinFinalSegmentLength": float,
+        "MpdManifestBandwidthType": DashIsoMpdManifestBandwidthTypeType,
+        "MpdProfile": DashIsoMpdProfileType,
+        "PtsOffsetHandlingForBFrames": DashIsoPtsOffsetHandlingForBFramesType,
+        "SegmentControl": DashIsoSegmentControlType,
+        "SegmentLength": int,
+        "SegmentLengthControl": DashIsoSegmentLengthControlType,
+        "VideoCompositionOffsets": DashIsoVideoCompositionOffsetsType,
+        "WriteSegmentTimelineInRepresentation": DashIsoWriteSegmentTimelineInRepresentationType,
+    },
+)
+
+FileGroupSettingsOutputTypeDef = TypedDict(
+    "FileGroupSettingsOutputTypeDef",
+    {
+        "Destination": str,
+        "DestinationSettings": DestinationSettingsOutputTypeDef,
+    },
+)
+
+HlsGroupSettingsOutputTypeDef = TypedDict(
+    "HlsGroupSettingsOutputTypeDef",
+    {
+        "AdMarkers": List[HlsAdMarkersType],
+        "AdditionalManifests": List[HlsAdditionalManifestOutputTypeDef],
+        "AudioOnlyHeader": HlsAudioOnlyHeaderType,
+        "BaseUrl": str,
+        "CaptionLanguageMappings": List[HlsCaptionLanguageMappingOutputTypeDef],
+        "CaptionLanguageSetting": HlsCaptionLanguageSettingType,
+        "CaptionSegmentLengthControl": HlsCaptionSegmentLengthControlType,
+        "ClientCache": HlsClientCacheType,
+        "CodecSpecification": HlsCodecSpecificationType,
+        "Destination": str,
+        "DestinationSettings": DestinationSettingsOutputTypeDef,
+        "DirectoryStructure": HlsDirectoryStructureType,
+        "Encryption": HlsEncryptionSettingsOutputTypeDef,
+        "ImageBasedTrickPlay": HlsImageBasedTrickPlayType,
+        "ImageBasedTrickPlaySettings": HlsImageBasedTrickPlaySettingsOutputTypeDef,
+        "ManifestCompression": HlsManifestCompressionType,
+        "ManifestDurationFormat": HlsManifestDurationFormatType,
+        "MinFinalSegmentLength": float,
+        "MinSegmentLength": int,
+        "OutputSelection": HlsOutputSelectionType,
+        "ProgramDateTime": HlsProgramDateTimeType,
+        "ProgramDateTimePeriod": int,
+        "ProgressiveWriteHlsManifest": HlsProgressiveWriteHlsManifestType,
+        "SegmentControl": HlsSegmentControlType,
+        "SegmentLength": int,
+        "SegmentLengthControl": HlsSegmentLengthControlType,
+        "SegmentsPerSubdirectory": int,
+        "StreamInfResolution": HlsStreamInfResolutionType,
+        "TargetDurationCompatibilityMode": HlsTargetDurationCompatibilityModeType,
+        "TimedMetadataId3Frame": HlsTimedMetadataId3FrameType,
+        "TimedMetadataId3Period": int,
+        "TimestampDeltaMilliseconds": int,
+    },
+)
+
+MsSmoothGroupSettingsOutputTypeDef = TypedDict(
+    "MsSmoothGroupSettingsOutputTypeDef",
+    {
+        "AdditionalManifests": List[MsSmoothAdditionalManifestOutputTypeDef],
+        "AudioDeduplication": MsSmoothAudioDeduplicationType,
+        "Destination": str,
+        "DestinationSettings": DestinationSettingsOutputTypeDef,
+        "Encryption": MsSmoothEncryptionSettingsOutputTypeDef,
+        "FragmentLength": int,
+        "FragmentLengthControl": MsSmoothFragmentLengthControlType,
+        "ManifestEncoding": MsSmoothManifestEncodingType,
+    },
 )
 
 CmafGroupSettingsTypeDef = TypedDict(
     "CmafGroupSettingsTypeDef",
     {
         "AdditionalManifests": Sequence[CmafAdditionalManifestTypeDef],
         "BaseUrl": str,
@@ -3501,42 +5023,14 @@
         "WriteDashManifest": CmafWriteDASHManifestType,
         "WriteHlsManifest": CmafWriteHLSManifestType,
         "WriteSegmentTimelineInRepresentation": CmafWriteSegmentTimelineInRepresentationType,
     },
     total=False,
 )
 
-DashIsoGroupSettingsOutputTypeDef = TypedDict(
-    "DashIsoGroupSettingsOutputTypeDef",
-    {
-        "AdditionalManifests": List[DashAdditionalManifestOutputTypeDef],
-        "AudioChannelConfigSchemeIdUri": DashIsoGroupAudioChannelConfigSchemeIdUriType,
-        "BaseUrl": str,
-        "DashManifestStyle": DashManifestStyleType,
-        "Destination": str,
-        "DestinationSettings": DestinationSettingsTypeDef,
-        "Encryption": DashIsoEncryptionSettingsOutputTypeDef,
-        "FragmentLength": int,
-        "HbbtvCompliance": DashIsoHbbtvComplianceType,
-        "ImageBasedTrickPlay": DashIsoImageBasedTrickPlayType,
-        "ImageBasedTrickPlaySettings": DashIsoImageBasedTrickPlaySettingsTypeDef,
-        "MinBufferTime": int,
-        "MinFinalSegmentLength": float,
-        "MpdManifestBandwidthType": DashIsoMpdManifestBandwidthTypeType,
-        "MpdProfile": DashIsoMpdProfileType,
-        "PtsOffsetHandlingForBFrames": DashIsoPtsOffsetHandlingForBFramesType,
-        "SegmentControl": DashIsoSegmentControlType,
-        "SegmentLength": int,
-        "SegmentLengthControl": DashIsoSegmentLengthControlType,
-        "VideoCompositionOffsets": DashIsoVideoCompositionOffsetsType,
-        "WriteSegmentTimelineInRepresentation": DashIsoWriteSegmentTimelineInRepresentationType,
-    },
-    total=False,
-)
-
 DashIsoGroupSettingsTypeDef = TypedDict(
     "DashIsoGroupSettingsTypeDef",
     {
         "AdditionalManifests": Sequence[DashAdditionalManifestTypeDef],
         "AudioChannelConfigSchemeIdUri": DashIsoGroupAudioChannelConfigSchemeIdUriType,
         "BaseUrl": str,
         "DashManifestStyle": DashManifestStyleType,
@@ -3566,53 +5060,14 @@
     {
         "Destination": str,
         "DestinationSettings": DestinationSettingsTypeDef,
     },
     total=False,
 )
 
-HlsGroupSettingsOutputTypeDef = TypedDict(
-    "HlsGroupSettingsOutputTypeDef",
-    {
-        "AdMarkers": List[HlsAdMarkersType],
-        "AdditionalManifests": List[HlsAdditionalManifestOutputTypeDef],
-        "AudioOnlyHeader": HlsAudioOnlyHeaderType,
-        "BaseUrl": str,
-        "CaptionLanguageMappings": List[HlsCaptionLanguageMappingTypeDef],
-        "CaptionLanguageSetting": HlsCaptionLanguageSettingType,
-        "CaptionSegmentLengthControl": HlsCaptionSegmentLengthControlType,
-        "ClientCache": HlsClientCacheType,
-        "CodecSpecification": HlsCodecSpecificationType,
-        "Destination": str,
-        "DestinationSettings": DestinationSettingsTypeDef,
-        "DirectoryStructure": HlsDirectoryStructureType,
-        "Encryption": HlsEncryptionSettingsOutputTypeDef,
-        "ImageBasedTrickPlay": HlsImageBasedTrickPlayType,
-        "ImageBasedTrickPlaySettings": HlsImageBasedTrickPlaySettingsTypeDef,
-        "ManifestCompression": HlsManifestCompressionType,
-        "ManifestDurationFormat": HlsManifestDurationFormatType,
-        "MinFinalSegmentLength": float,
-        "MinSegmentLength": int,
-        "OutputSelection": HlsOutputSelectionType,
-        "ProgramDateTime": HlsProgramDateTimeType,
-        "ProgramDateTimePeriod": int,
-        "ProgressiveWriteHlsManifest": HlsProgressiveWriteHlsManifestType,
-        "SegmentControl": HlsSegmentControlType,
-        "SegmentLength": int,
-        "SegmentLengthControl": HlsSegmentLengthControlType,
-        "SegmentsPerSubdirectory": int,
-        "StreamInfResolution": HlsStreamInfResolutionType,
-        "TargetDurationCompatibilityMode": HlsTargetDurationCompatibilityModeType,
-        "TimedMetadataId3Frame": HlsTimedMetadataId3FrameType,
-        "TimedMetadataId3Period": int,
-        "TimestampDeltaMilliseconds": int,
-    },
-    total=False,
-)
-
 HlsGroupSettingsTypeDef = TypedDict(
     "HlsGroupSettingsTypeDef",
     {
         "AdMarkers": Sequence[HlsAdMarkersType],
         "AdditionalManifests": Sequence[HlsAdditionalManifestTypeDef],
         "AudioOnlyHeader": HlsAudioOnlyHeaderType,
         "BaseUrl": str,
@@ -3644,29 +5099,14 @@
         "TimedMetadataId3Frame": HlsTimedMetadataId3FrameType,
         "TimedMetadataId3Period": int,
         "TimestampDeltaMilliseconds": int,
     },
     total=False,
 )
 
-MsSmoothGroupSettingsOutputTypeDef = TypedDict(
-    "MsSmoothGroupSettingsOutputTypeDef",
-    {
-        "AdditionalManifests": List[MsSmoothAdditionalManifestOutputTypeDef],
-        "AudioDeduplication": MsSmoothAudioDeduplicationType,
-        "Destination": str,
-        "DestinationSettings": DestinationSettingsTypeDef,
-        "Encryption": MsSmoothEncryptionSettingsOutputTypeDef,
-        "FragmentLength": int,
-        "FragmentLengthControl": MsSmoothFragmentLengthControlType,
-        "ManifestEncoding": MsSmoothManifestEncodingType,
-    },
-    total=False,
-)
-
 MsSmoothGroupSettingsTypeDef = TypedDict(
     "MsSmoothGroupSettingsTypeDef",
     {
         "AdditionalManifests": Sequence[MsSmoothAdditionalManifestTypeDef],
         "AudioDeduplication": MsSmoothAudioDeduplicationType,
         "Destination": str,
         "DestinationSettings": DestinationSettingsTypeDef,
@@ -3679,29 +5119,28 @@
 )
 
 VideoDescriptionOutputTypeDef = TypedDict(
     "VideoDescriptionOutputTypeDef",
     {
         "AfdSignaling": AfdSignalingType,
         "AntiAlias": AntiAliasType,
-        "CodecSettings": VideoCodecSettingsTypeDef,
+        "CodecSettings": VideoCodecSettingsOutputTypeDef,
         "ColorMetadata": ColorMetadataType,
-        "Crop": RectangleTypeDef,
+        "Crop": RectangleOutputTypeDef,
         "DropFrameTimecode": DropFrameTimecodeType,
         "FixedAfd": int,
         "Height": int,
-        "Position": RectangleTypeDef,
+        "Position": RectangleOutputTypeDef,
         "RespondToAfd": RespondToAfdType,
         "ScalingBehavior": ScalingBehaviorType,
         "Sharpness": int,
         "TimecodeInsertion": VideoTimecodeInsertionType,
         "VideoPreprocessors": VideoPreprocessorOutputTypeDef,
         "Width": int,
     },
-    total=False,
 )
 
 VideoDescriptionTypeDef = TypedDict(
     "VideoDescriptionTypeDef",
     {
         "AfdSignaling": AfdSignalingType,
         "AntiAlias": AntiAliasType,
@@ -3722,66 +5161,64 @@
     total=False,
 )
 
 InputOutputTypeDef = TypedDict(
     "InputOutputTypeDef",
     {
         "AdvancedInputFilter": AdvancedInputFilterType,
-        "AdvancedInputFilterSettings": AdvancedInputFilterSettingsTypeDef,
+        "AdvancedInputFilterSettings": AdvancedInputFilterSettingsOutputTypeDef,
         "AudioSelectorGroups": Dict[str, AudioSelectorGroupOutputTypeDef],
         "AudioSelectors": Dict[str, AudioSelectorOutputTypeDef],
-        "CaptionSelectors": Dict[str, CaptionSelectorTypeDef],
-        "Crop": RectangleTypeDef,
+        "CaptionSelectors": Dict[str, CaptionSelectorOutputTypeDef],
+        "Crop": RectangleOutputTypeDef,
         "DeblockFilter": InputDeblockFilterType,
-        "DecryptionSettings": InputDecryptionSettingsTypeDef,
+        "DecryptionSettings": InputDecryptionSettingsOutputTypeDef,
         "DenoiseFilter": InputDenoiseFilterType,
         "DolbyVisionMetadataXml": str,
         "FileInput": str,
         "FilterEnable": InputFilterEnableType,
         "FilterStrength": int,
         "ImageInserter": ImageInserterOutputTypeDef,
-        "InputClippings": List[InputClippingTypeDef],
+        "InputClippings": List[InputClippingOutputTypeDef],
         "InputScanType": InputScanTypeType,
-        "Position": RectangleTypeDef,
+        "Position": RectangleOutputTypeDef,
         "ProgramNumber": int,
         "PsiControl": InputPsiControlType,
         "SupplementalImps": List[str],
         "TimecodeSource": InputTimecodeSourceType,
         "TimecodeStart": str,
-        "VideoGenerator": InputVideoGeneratorTypeDef,
-        "VideoSelector": VideoSelectorTypeDef,
+        "VideoGenerator": InputVideoGeneratorOutputTypeDef,
+        "VideoSelector": VideoSelectorOutputTypeDef,
     },
-    total=False,
 )
 
 InputTemplateOutputTypeDef = TypedDict(
     "InputTemplateOutputTypeDef",
     {
         "AdvancedInputFilter": AdvancedInputFilterType,
-        "AdvancedInputFilterSettings": AdvancedInputFilterSettingsTypeDef,
+        "AdvancedInputFilterSettings": AdvancedInputFilterSettingsOutputTypeDef,
         "AudioSelectorGroups": Dict[str, AudioSelectorGroupOutputTypeDef],
         "AudioSelectors": Dict[str, AudioSelectorOutputTypeDef],
-        "CaptionSelectors": Dict[str, CaptionSelectorTypeDef],
-        "Crop": RectangleTypeDef,
+        "CaptionSelectors": Dict[str, CaptionSelectorOutputTypeDef],
+        "Crop": RectangleOutputTypeDef,
         "DeblockFilter": InputDeblockFilterType,
         "DenoiseFilter": InputDenoiseFilterType,
         "DolbyVisionMetadataXml": str,
         "FilterEnable": InputFilterEnableType,
         "FilterStrength": int,
         "ImageInserter": ImageInserterOutputTypeDef,
-        "InputClippings": List[InputClippingTypeDef],
+        "InputClippings": List[InputClippingOutputTypeDef],
         "InputScanType": InputScanTypeType,
-        "Position": RectangleTypeDef,
+        "Position": RectangleOutputTypeDef,
         "ProgramNumber": int,
         "PsiControl": InputPsiControlType,
         "TimecodeSource": InputTimecodeSourceType,
         "TimecodeStart": str,
-        "VideoSelector": VideoSelectorTypeDef,
+        "VideoSelector": VideoSelectorOutputTypeDef,
     },
-    total=False,
 )
 
 InputTemplateTypeDef = TypedDict(
     "InputTemplateTypeDef",
     {
         "AdvancedInputFilter": AdvancedInputFilterType,
         "AdvancedInputFilterSettings": AdvancedInputFilterSettingsTypeDef,
@@ -3839,20 +5276,19 @@
 )
 
 OutputGroupSettingsOutputTypeDef = TypedDict(
     "OutputGroupSettingsOutputTypeDef",
     {
         "CmafGroupSettings": CmafGroupSettingsOutputTypeDef,
         "DashIsoGroupSettings": DashIsoGroupSettingsOutputTypeDef,
-        "FileGroupSettings": FileGroupSettingsTypeDef,
+        "FileGroupSettings": FileGroupSettingsOutputTypeDef,
         "HlsGroupSettings": HlsGroupSettingsOutputTypeDef,
         "MsSmoothGroupSettings": MsSmoothGroupSettingsOutputTypeDef,
         "Type": OutputGroupTypeType,
     },
-    total=False,
 )
 
 OutputGroupSettingsTypeDef = TypedDict(
     "OutputGroupSettingsTypeDef",
     {
         "CmafGroupSettings": CmafGroupSettingsTypeDef,
         "DashIsoGroupSettings": DashIsoGroupSettingsTypeDef,
@@ -3860,100 +5296,86 @@
         "HlsGroupSettings": HlsGroupSettingsTypeDef,
         "MsSmoothGroupSettings": MsSmoothGroupSettingsTypeDef,
         "Type": OutputGroupTypeType,
     },
     total=False,
 )
 
-PresetSettingsOutputTypeDef = TypedDict(
-    "PresetSettingsOutputTypeDef",
+OutputTypeDef = TypedDict(
+    "OutputTypeDef",
     {
         "AudioDescriptions": List[AudioDescriptionOutputTypeDef],
-        "CaptionDescriptions": List[CaptionDescriptionPresetOutputTypeDef],
+        "CaptionDescriptions": List[CaptionDescriptionOutputTypeDef],
         "ContainerSettings": ContainerSettingsOutputTypeDef,
+        "Extension": str,
+        "NameModifier": str,
+        "OutputSettings": OutputSettingsOutputTypeDef,
+        "Preset": str,
         "VideoDescription": VideoDescriptionOutputTypeDef,
     },
-    total=False,
 )
 
-OutputTypeDef = TypedDict(
-    "OutputTypeDef",
+PresetSettingsOutputTypeDef = TypedDict(
+    "PresetSettingsOutputTypeDef",
     {
-        "AudioDescriptions": Sequence[AudioDescriptionTypeDef],
-        "CaptionDescriptions": Sequence[CaptionDescriptionTypeDef],
-        "ContainerSettings": ContainerSettingsTypeDef,
-        "Extension": str,
-        "NameModifier": str,
-        "OutputSettings": OutputSettingsTypeDef,
-        "Preset": str,
-        "VideoDescription": VideoDescriptionTypeDef,
+        "AudioDescriptions": List[AudioDescriptionOutputTypeDef],
+        "CaptionDescriptions": List[CaptionDescriptionPresetOutputTypeDef],
+        "ContainerSettings": ContainerSettingsOutputTypeDef,
+        "VideoDescription": VideoDescriptionOutputTypeDef,
     },
-    total=False,
 )
 
 PresetSettingsTypeDef = TypedDict(
     "PresetSettingsTypeDef",
     {
         "AudioDescriptions": Sequence[AudioDescriptionTypeDef],
         "CaptionDescriptions": Sequence[CaptionDescriptionPresetTypeDef],
         "ContainerSettings": ContainerSettingsTypeDef,
         "VideoDescription": VideoDescriptionTypeDef,
     },
     total=False,
 )
 
-_RequiredPresetTypeDef = TypedDict(
-    "_RequiredPresetTypeDef",
-    {
-        "Name": str,
-        "Settings": PresetSettingsOutputTypeDef,
-    },
-)
-_OptionalPresetTypeDef = TypedDict(
-    "_OptionalPresetTypeDef",
-    {
-        "Arn": str,
-        "Category": str,
-        "CreatedAt": datetime,
-        "Description": str,
-        "LastUpdated": datetime,
-        "Type": TypeType,
-    },
-    total=False,
-)
-
-
-class PresetTypeDef(_RequiredPresetTypeDef, _OptionalPresetTypeDef):
-    pass
-
-
 OutputGroupOutputTypeDef = TypedDict(
     "OutputGroupOutputTypeDef",
     {
         "AutomatedEncodingSettings": AutomatedEncodingSettingsOutputTypeDef,
         "CustomName": str,
         "Name": str,
         "OutputGroupSettings": OutputGroupSettingsOutputTypeDef,
         "Outputs": List[OutputTypeDef],
     },
-    total=False,
 )
 
 OutputGroupTypeDef = TypedDict(
     "OutputGroupTypeDef",
     {
         "AutomatedEncodingSettings": AutomatedEncodingSettingsTypeDef,
         "CustomName": str,
         "Name": str,
         "OutputGroupSettings": OutputGroupSettingsTypeDef,
         "Outputs": Sequence[OutputTypeDef],
     },
     total=False,
 )
 
+PresetTypeDef = TypedDict(
+    "PresetTypeDef",
+    {
+        "Arn": str,
+        "Category": str,
+        "CreatedAt": datetime,
+        "Description": str,
+        "LastUpdated": datetime,
+        "Name": str,
+        "Settings": PresetSettingsOutputTypeDef,
+        "Type": TypeType,
+    },
+)
+
 _RequiredCreatePresetRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePresetRequestRequestTypeDef",
     {
         "Name": str,
         "Settings": PresetSettingsTypeDef,
     },
 )
@@ -3970,15 +5392,14 @@
 
 class CreatePresetRequestRequestTypeDef(
     _RequiredCreatePresetRequestRequestTypeDef, _OptionalCreatePresetRequestRequestTypeDef
 ):
     pass
 
 
-PresetSettingsUnionTypeDef = Union[PresetSettingsTypeDef, PresetSettingsOutputTypeDef]
 _RequiredUpdatePresetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePresetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdatePresetRequestRequestTypeDef = TypedDict(
@@ -3994,83 +5415,48 @@
 
 class UpdatePresetRequestRequestTypeDef(
     _RequiredUpdatePresetRequestRequestTypeDef, _OptionalUpdatePresetRequestRequestTypeDef
 ):
     pass
 
 
-CreatePresetResponseTypeDef = TypedDict(
-    "CreatePresetResponseTypeDef",
-    {
-        "Preset": PresetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPresetResponseTypeDef = TypedDict(
-    "GetPresetResponseTypeDef",
-    {
-        "Preset": PresetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListPresetsResponseTypeDef = TypedDict(
-    "ListPresetsResponseTypeDef",
-    {
-        "NextToken": str,
-        "Presets": List[PresetTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdatePresetResponseTypeDef = TypedDict(
-    "UpdatePresetResponseTypeDef",
-    {
-        "Preset": PresetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 JobSettingsOutputTypeDef = TypedDict(
     "JobSettingsOutputTypeDef",
     {
         "AdAvailOffset": int,
-        "AvailBlanking": AvailBlankingTypeDef,
-        "Esam": EsamSettingsTypeDef,
-        "ExtendedDataServices": ExtendedDataServicesTypeDef,
+        "AvailBlanking": AvailBlankingOutputTypeDef,
+        "Esam": EsamSettingsOutputTypeDef,
+        "ExtendedDataServices": ExtendedDataServicesOutputTypeDef,
         "Inputs": List[InputOutputTypeDef],
-        "KantarWatermark": KantarWatermarkSettingsTypeDef,
-        "MotionImageInserter": MotionImageInserterTypeDef,
-        "NielsenConfiguration": NielsenConfigurationTypeDef,
-        "NielsenNonLinearWatermark": NielsenNonLinearWatermarkSettingsTypeDef,
+        "KantarWatermark": KantarWatermarkSettingsOutputTypeDef,
+        "MotionImageInserter": MotionImageInserterOutputTypeDef,
+        "NielsenConfiguration": NielsenConfigurationOutputTypeDef,
+        "NielsenNonLinearWatermark": NielsenNonLinearWatermarkSettingsOutputTypeDef,
         "OutputGroups": List[OutputGroupOutputTypeDef],
-        "TimecodeConfig": TimecodeConfigTypeDef,
+        "TimecodeConfig": TimecodeConfigOutputTypeDef,
         "TimedMetadataInsertion": TimedMetadataInsertionOutputTypeDef,
     },
-    total=False,
 )
 
 JobTemplateSettingsOutputTypeDef = TypedDict(
     "JobTemplateSettingsOutputTypeDef",
     {
         "AdAvailOffset": int,
-        "AvailBlanking": AvailBlankingTypeDef,
-        "Esam": EsamSettingsTypeDef,
-        "ExtendedDataServices": ExtendedDataServicesTypeDef,
+        "AvailBlanking": AvailBlankingOutputTypeDef,
+        "Esam": EsamSettingsOutputTypeDef,
+        "ExtendedDataServices": ExtendedDataServicesOutputTypeDef,
         "Inputs": List[InputTemplateOutputTypeDef],
-        "KantarWatermark": KantarWatermarkSettingsTypeDef,
-        "MotionImageInserter": MotionImageInserterTypeDef,
-        "NielsenConfiguration": NielsenConfigurationTypeDef,
-        "NielsenNonLinearWatermark": NielsenNonLinearWatermarkSettingsTypeDef,
+        "KantarWatermark": KantarWatermarkSettingsOutputTypeDef,
+        "MotionImageInserter": MotionImageInserterOutputTypeDef,
+        "NielsenConfiguration": NielsenConfigurationOutputTypeDef,
+        "NielsenNonLinearWatermark": NielsenNonLinearWatermarkSettingsOutputTypeDef,
         "OutputGroups": List[OutputGroupOutputTypeDef],
-        "TimecodeConfig": TimecodeConfigTypeDef,
+        "TimecodeConfig": TimecodeConfigOutputTypeDef,
         "TimedMetadataInsertion": TimedMetadataInsertionOutputTypeDef,
     },
-    total=False,
 )
 
 JobSettingsTypeDef = TypedDict(
     "JobSettingsTypeDef",
     {
         "AdAvailOffset": int,
         "AvailBlanking": AvailBlankingTypeDef,
@@ -4103,88 +5489,99 @@
         "OutputGroups": Sequence[OutputGroupTypeDef],
         "TimecodeConfig": TimecodeConfigTypeDef,
         "TimedMetadataInsertion": TimedMetadataInsertionTypeDef,
     },
     total=False,
 )
 
-_RequiredJobTypeDef = TypedDict(
-    "_RequiredJobTypeDef",
+CreatePresetResponseTypeDef = TypedDict(
+    "CreatePresetResponseTypeDef",
     {
-        "Role": str,
-        "Settings": JobSettingsOutputTypeDef,
+        "Preset": PresetTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalJobTypeDef = TypedDict(
-    "_OptionalJobTypeDef",
+
+GetPresetResponseTypeDef = TypedDict(
+    "GetPresetResponseTypeDef",
     {
-        "AccelerationSettings": AccelerationSettingsTypeDef,
+        "Preset": PresetTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPresetsResponseTypeDef = TypedDict(
+    "ListPresetsResponseTypeDef",
+    {
+        "NextToken": str,
+        "Presets": List[PresetTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePresetResponseTypeDef = TypedDict(
+    "UpdatePresetResponseTypeDef",
+    {
+        "Preset": PresetTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+JobTypeDef = TypedDict(
+    "JobTypeDef",
+    {
+        "AccelerationSettings": AccelerationSettingsOutputTypeDef,
         "AccelerationStatus": AccelerationStatusType,
         "Arn": str,
         "BillingTagsSource": BillingTagsSourceType,
         "ClientRequestToken": str,
         "CreatedAt": datetime,
         "CurrentPhase": JobPhaseType,
         "ErrorCode": int,
         "ErrorMessage": str,
-        "HopDestinations": List[HopDestinationTypeDef],
+        "HopDestinations": List[HopDestinationOutputTypeDef],
         "Id": str,
         "JobPercentComplete": int,
         "JobTemplate": str,
         "Messages": JobMessagesTypeDef,
         "OutputGroupDetails": List[OutputGroupDetailTypeDef],
         "Priority": int,
         "Queue": str,
         "QueueTransitions": List[QueueTransitionTypeDef],
         "RetryCount": int,
+        "Role": str,
+        "Settings": JobSettingsOutputTypeDef,
         "SimulateReservedQueue": SimulateReservedQueueType,
         "Status": JobStatusType,
         "StatusUpdateInterval": StatusUpdateIntervalType,
         "Timing": TimingTypeDef,
         "UserMetadata": Dict[str, str],
         "Warnings": List[WarningGroupTypeDef],
     },
-    total=False,
 )
 
-
-class JobTypeDef(_RequiredJobTypeDef, _OptionalJobTypeDef):
-    pass
-
-
-_RequiredJobTemplateTypeDef = TypedDict(
-    "_RequiredJobTemplateTypeDef",
-    {
-        "Name": str,
-        "Settings": JobTemplateSettingsOutputTypeDef,
-    },
-)
-_OptionalJobTemplateTypeDef = TypedDict(
-    "_OptionalJobTemplateTypeDef",
+JobTemplateTypeDef = TypedDict(
+    "JobTemplateTypeDef",
     {
-        "AccelerationSettings": AccelerationSettingsTypeDef,
+        "AccelerationSettings": AccelerationSettingsOutputTypeDef,
         "Arn": str,
         "Category": str,
         "CreatedAt": datetime,
         "Description": str,
-        "HopDestinations": List[HopDestinationTypeDef],
+        "HopDestinations": List[HopDestinationOutputTypeDef],
         "LastUpdated": datetime,
+        "Name": str,
         "Priority": int,
         "Queue": str,
+        "Settings": JobTemplateSettingsOutputTypeDef,
         "StatusUpdateInterval": StatusUpdateIntervalType,
         "Type": TypeType,
     },
-    total=False,
 )
 
-
-class JobTemplateTypeDef(_RequiredJobTemplateTypeDef, _OptionalJobTemplateTypeDef):
-    pass
-
-
 _RequiredCreateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobRequestRequestTypeDef",
     {
         "Role": str,
         "Settings": JobSettingsTypeDef,
     },
 )
@@ -4209,15 +5606,14 @@
 
 class CreateJobRequestRequestTypeDef(
     _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
 ):
     pass
 
 
-JobSettingsUnionTypeDef = Union[JobSettingsTypeDef, JobSettingsOutputTypeDef]
 _RequiredCreateJobTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobTemplateRequestRequestTypeDef",
     {
         "Name": str,
         "Settings": JobTemplateSettingsTypeDef,
     },
 )
@@ -4239,17 +5635,14 @@
 
 class CreateJobTemplateRequestRequestTypeDef(
     _RequiredCreateJobTemplateRequestRequestTypeDef, _OptionalCreateJobTemplateRequestRequestTypeDef
 ):
     pass
 
 
-JobTemplateSettingsUnionTypeDef = Union[
-    JobTemplateSettingsTypeDef, JobTemplateSettingsOutputTypeDef
-]
 _RequiredUpdateJobTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateJobTemplateRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateJobTemplateRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-mediaconvert-1.28.16/mypy_boto3_mediaconvert/type_defs.pyi` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/type_defs.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for mediaconvert service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_mediaconvert.type_defs import AacSettingsTypeDef
+    from mypy_boto3_mediaconvert.type_defs import AacSettingsOutputTypeDef
 
-    data: AacSettingsTypeDef = ...
+    data: AacSettingsOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AacAudioDescriptionBroadcasterMixType,
     AacCodecProfileType,
     AacCodingModeType,
     AacRateControlModeType,
     AacRawFormatType,
@@ -427,171 +427,272 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AacSettingsOutputTypeDef",
     "AacSettingsTypeDef",
+    "Ac3SettingsOutputTypeDef",
     "Ac3SettingsTypeDef",
+    "AccelerationSettingsOutputTypeDef",
     "AccelerationSettingsTypeDef",
+    "AdvancedInputFilterSettingsOutputTypeDef",
     "AdvancedInputFilterSettingsTypeDef",
+    "AiffSettingsOutputTypeDef",
     "AiffSettingsTypeDef",
+    "AllowedRenditionSizeOutputTypeDef",
     "AllowedRenditionSizeTypeDef",
+    "AncillarySourceSettingsOutputTypeDef",
     "AncillarySourceSettingsTypeDef",
     "AssociateCertificateRequestRequestTypeDef",
+    "AudioChannelTaggingSettingsOutputTypeDef",
     "AudioChannelTaggingSettingsTypeDef",
+    "Eac3AtmosSettingsOutputTypeDef",
+    "Eac3SettingsOutputTypeDef",
+    "Mp2SettingsOutputTypeDef",
+    "Mp3SettingsOutputTypeDef",
+    "OpusSettingsOutputTypeDef",
+    "VorbisSettingsOutputTypeDef",
+    "WavSettingsOutputTypeDef",
     "Eac3AtmosSettingsTypeDef",
     "Eac3SettingsTypeDef",
     "Mp2SettingsTypeDef",
     "Mp3SettingsTypeDef",
     "OpusSettingsTypeDef",
     "VorbisSettingsTypeDef",
     "WavSettingsTypeDef",
+    "AudioNormalizationSettingsOutputTypeDef",
     "AudioNormalizationSettingsTypeDef",
     "AudioSelectorGroupOutputTypeDef",
     "AudioSelectorGroupTypeDef",
+    "HlsRenditionGroupSettingsOutputTypeDef",
     "HlsRenditionGroupSettingsTypeDef",
+    "ForceIncludeRenditionSizeOutputTypeDef",
+    "MinBottomRenditionSizeOutputTypeDef",
+    "MinTopRenditionSizeOutputTypeDef",
     "ForceIncludeRenditionSizeTypeDef",
     "MinBottomRenditionSizeTypeDef",
     "MinTopRenditionSizeTypeDef",
+    "Av1QvbrSettingsOutputTypeDef",
     "Av1QvbrSettingsTypeDef",
+    "AvailBlankingOutputTypeDef",
     "AvailBlankingTypeDef",
+    "AvcIntraUhdSettingsOutputTypeDef",
     "AvcIntraUhdSettingsTypeDef",
+    "BandwidthReductionFilterOutputTypeDef",
     "BandwidthReductionFilterTypeDef",
+    "BurninDestinationSettingsOutputTypeDef",
     "BurninDestinationSettingsTypeDef",
     "CancelJobRequestRequestTypeDef",
+    "DvbSubDestinationSettingsOutputTypeDef",
+    "EmbeddedDestinationSettingsOutputTypeDef",
+    "ImscDestinationSettingsOutputTypeDef",
+    "SccDestinationSettingsOutputTypeDef",
+    "SrtDestinationSettingsOutputTypeDef",
+    "TeletextDestinationSettingsOutputTypeDef",
+    "TtmlDestinationSettingsOutputTypeDef",
+    "WebvttDestinationSettingsOutputTypeDef",
     "DvbSubDestinationSettingsTypeDef",
     "EmbeddedDestinationSettingsTypeDef",
     "ImscDestinationSettingsTypeDef",
     "SccDestinationSettingsTypeDef",
     "SrtDestinationSettingsTypeDef",
-    "TeletextDestinationSettingsOutputTypeDef",
+    "TeletextDestinationSettingsTypeDef",
     "TtmlDestinationSettingsTypeDef",
     "WebvttDestinationSettingsTypeDef",
-    "TeletextDestinationSettingsTypeDef",
+    "CaptionSourceFramerateOutputTypeDef",
     "CaptionSourceFramerateTypeDef",
+    "DvbSubSourceSettingsOutputTypeDef",
+    "EmbeddedSourceSettingsOutputTypeDef",
+    "TeletextSourceSettingsOutputTypeDef",
+    "TrackSourceSettingsOutputTypeDef",
+    "WebvttHlsSourceSettingsOutputTypeDef",
     "DvbSubSourceSettingsTypeDef",
     "EmbeddedSourceSettingsTypeDef",
     "TeletextSourceSettingsTypeDef",
     "TrackSourceSettingsTypeDef",
     "WebvttHlsSourceSettingsTypeDef",
     "OutputChannelMappingOutputTypeDef",
     "OutputChannelMappingTypeDef",
+    "ClipLimitsOutputTypeDef",
     "ClipLimitsTypeDef",
     "CmafAdditionalManifestOutputTypeDef",
     "CmafAdditionalManifestTypeDef",
     "SpekeKeyProviderCmafOutputTypeDef",
-    "StaticKeyProviderTypeDef",
+    "StaticKeyProviderOutputTypeDef",
     "SpekeKeyProviderCmafTypeDef",
+    "StaticKeyProviderTypeDef",
+    "CmafImageBasedTrickPlaySettingsOutputTypeDef",
     "CmafImageBasedTrickPlaySettingsTypeDef",
+    "CmfcSettingsOutputTypeDef",
     "CmfcSettingsTypeDef",
+    "Hdr10MetadataOutputTypeDef",
     "Hdr10MetadataTypeDef",
-    "F4vSettingsTypeDef",
+    "F4vSettingsOutputTypeDef",
     "M3u8SettingsOutputTypeDef",
+    "MovSettingsOutputTypeDef",
+    "Mp4SettingsOutputTypeDef",
+    "MpdSettingsOutputTypeDef",
+    "F4vSettingsTypeDef",
+    "M3u8SettingsTypeDef",
     "MovSettingsTypeDef",
     "Mp4SettingsTypeDef",
     "MpdSettingsTypeDef",
-    "M3u8SettingsTypeDef",
     "HopDestinationTypeDef",
     "ResponseMetadataTypeDef",
     "ReservationPlanSettingsTypeDef",
     "DashAdditionalManifestOutputTypeDef",
     "DashAdditionalManifestTypeDef",
     "SpekeKeyProviderOutputTypeDef",
     "SpekeKeyProviderTypeDef",
+    "DashIsoImageBasedTrickPlaySettingsOutputTypeDef",
     "DashIsoImageBasedTrickPlaySettingsTypeDef",
+    "DeinterlacerOutputTypeDef",
     "DeinterlacerTypeDef",
     "DeleteJobTemplateRequestRequestTypeDef",
     "DeletePresetRequestRequestTypeDef",
     "DeleteQueueRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeEndpointsRequestRequestTypeDef",
     "EndpointTypeDef",
     "DisassociateCertificateRequestRequestTypeDef",
+    "DolbyVisionLevel6MetadataOutputTypeDef",
     "DolbyVisionLevel6MetadataTypeDef",
+    "DvbNitSettingsOutputTypeDef",
     "DvbNitSettingsTypeDef",
+    "DvbSdtSettingsOutputTypeDef",
     "DvbSdtSettingsTypeDef",
+    "DvbTdtSettingsOutputTypeDef",
     "DvbTdtSettingsTypeDef",
+    "EsamManifestConfirmConditionNotificationOutputTypeDef",
     "EsamManifestConfirmConditionNotificationTypeDef",
+    "EsamSignalProcessingNotificationOutputTypeDef",
     "EsamSignalProcessingNotificationTypeDef",
+    "ExtendedDataServicesOutputTypeDef",
     "ExtendedDataServicesTypeDef",
+    "FrameCaptureSettingsOutputTypeDef",
     "FrameCaptureSettingsTypeDef",
     "GetJobRequestRequestTypeDef",
     "GetJobTemplateRequestRequestTypeDef",
-    "PolicyTypeDef",
+    "PolicyOutputTypeDef",
     "GetPresetRequestRequestTypeDef",
     "GetQueueRequestRequestTypeDef",
+    "H264QvbrSettingsOutputTypeDef",
     "H264QvbrSettingsTypeDef",
+    "H265QvbrSettingsOutputTypeDef",
     "H265QvbrSettingsTypeDef",
+    "Hdr10PlusOutputTypeDef",
     "Hdr10PlusTypeDef",
     "HlsAdditionalManifestOutputTypeDef",
     "HlsAdditionalManifestTypeDef",
+    "HlsCaptionLanguageMappingOutputTypeDef",
     "HlsCaptionLanguageMappingTypeDef",
+    "HlsImageBasedTrickPlaySettingsOutputTypeDef",
     "HlsImageBasedTrickPlaySettingsTypeDef",
-    "HlsSettingsTypeDef",
+    "HlsSettingsOutputTypeDef",
+    "HopDestinationOutputTypeDef",
+    "Id3InsertionOutputTypeDef",
     "Id3InsertionTypeDef",
+    "InsertableImageOutputTypeDef",
     "InsertableImageTypeDef",
+    "InputClippingOutputTypeDef",
     "InputClippingTypeDef",
+    "InputDecryptionSettingsOutputTypeDef",
     "InputDecryptionSettingsTypeDef",
-    "InputVideoGeneratorTypeDef",
+    "InputVideoGeneratorOutputTypeDef",
+    "RectangleOutputTypeDef",
     "RectangleTypeDef",
+    "InputVideoGeneratorTypeDef",
     "JobMessagesTypeDef",
+    "KantarWatermarkSettingsOutputTypeDef",
+    "NielsenConfigurationOutputTypeDef",
+    "NielsenNonLinearWatermarkSettingsOutputTypeDef",
+    "TimecodeConfigOutputTypeDef",
     "KantarWatermarkSettingsTypeDef",
     "NielsenConfigurationTypeDef",
     "NielsenNonLinearWatermarkSettingsTypeDef",
     "TimecodeConfigTypeDef",
     "QueueTransitionTypeDef",
     "TimingTypeDef",
     "WarningGroupTypeDef",
     "ListJobTemplatesRequestRequestTypeDef",
     "ListJobsRequestRequestTypeDef",
     "ListPresetsRequestRequestTypeDef",
     "ListQueuesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ResourceTagsTypeDef",
+    "M2tsScte35EsamOutputTypeDef",
     "M2tsScte35EsamTypeDef",
+    "MotionImageInsertionFramerateOutputTypeDef",
+    "MotionImageInsertionOffsetOutputTypeDef",
     "MotionImageInsertionFramerateTypeDef",
     "MotionImageInsertionOffsetTypeDef",
+    "Mpeg2SettingsOutputTypeDef",
     "Mpeg2SettingsTypeDef",
     "MsSmoothAdditionalManifestOutputTypeDef",
     "MsSmoothAdditionalManifestTypeDef",
+    "MxfXavcProfileSettingsOutputTypeDef",
     "MxfXavcProfileSettingsTypeDef",
+    "NexGuardFileMarkerSettingsOutputTypeDef",
     "NexGuardFileMarkerSettingsTypeDef",
+    "NoiseReducerFilterSettingsOutputTypeDef",
     "NoiseReducerFilterSettingsTypeDef",
+    "NoiseReducerSpatialFilterSettingsOutputTypeDef",
+    "NoiseReducerTemporalFilterSettingsOutputTypeDef",
     "NoiseReducerSpatialFilterSettingsTypeDef",
     "NoiseReducerTemporalFilterSettingsTypeDef",
     "VideoDetailTypeDef",
+    "PolicyTypeDef",
+    "ProresSettingsOutputTypeDef",
     "ProresSettingsTypeDef",
     "ReservationPlanTypeDef",
+    "S3DestinationAccessControlOutputTypeDef",
     "S3DestinationAccessControlTypeDef",
+    "S3EncryptionSettingsOutputTypeDef",
     "S3EncryptionSettingsTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "TimecodeBurninOutputTypeDef",
     "TimecodeBurninTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "Vc3SettingsOutputTypeDef",
     "Vc3SettingsTypeDef",
+    "Vp8SettingsOutputTypeDef",
+    "Vp9SettingsOutputTypeDef",
     "Vp8SettingsTypeDef",
     "Vp9SettingsTypeDef",
+    "Xavc4kIntraCbgProfileSettingsOutputTypeDef",
     "Xavc4kIntraCbgProfileSettingsTypeDef",
+    "Xavc4kIntraVbrProfileSettingsOutputTypeDef",
     "Xavc4kIntraVbrProfileSettingsTypeDef",
+    "Xavc4kProfileSettingsOutputTypeDef",
     "Xavc4kProfileSettingsTypeDef",
+    "XavcHdIntraCbgProfileSettingsOutputTypeDef",
     "XavcHdIntraCbgProfileSettingsTypeDef",
+    "XavcHdProfileSettingsOutputTypeDef",
     "XavcHdProfileSettingsTypeDef",
+    "AudioCodecSettingsOutputTypeDef",
     "AudioCodecSettingsTypeDef",
     "AutomatedAbrRuleOutputTypeDef",
     "AutomatedAbrRuleTypeDef",
+    "Av1SettingsOutputTypeDef",
     "Av1SettingsTypeDef",
+    "AvcIntraSettingsOutputTypeDef",
     "AvcIntraSettingsTypeDef",
     "CaptionDestinationSettingsOutputTypeDef",
     "CaptionDestinationSettingsTypeDef",
+    "FileSourceSettingsOutputTypeDef",
     "FileSourceSettingsTypeDef",
     "ChannelMappingOutputTypeDef",
     "ChannelMappingTypeDef",
     "CmafEncryptionSettingsOutputTypeDef",
     "CmafEncryptionSettingsTypeDef",
+    "ColorCorrectorOutputTypeDef",
+    "VideoSelectorOutputTypeDef",
     "ColorCorrectorTypeDef",
     "VideoSelectorTypeDef",
     "CreateQueueRequestRequestTypeDef",
     "UpdateQueueRequestRequestTypeDef",
     "DashIsoEncryptionSettingsOutputTypeDef",
     "HlsEncryptionSettingsOutputTypeDef",
     "MsSmoothEncryptionSettingsOutputTypeDef",
@@ -600,113 +701,140 @@
     "MsSmoothEncryptionSettingsTypeDef",
     "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
     "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
     "ListPresetsRequestListPresetsPaginateTypeDef",
     "ListQueuesRequestListQueuesPaginateTypeDef",
     "DescribeEndpointsResponseTypeDef",
+    "DolbyVisionOutputTypeDef",
     "DolbyVisionTypeDef",
+    "EsamSettingsOutputTypeDef",
     "EsamSettingsTypeDef",
     "GetPolicyResponseTypeDef",
-    "PutPolicyRequestRequestTypeDef",
     "PutPolicyResponseTypeDef",
+    "H264SettingsOutputTypeDef",
     "H264SettingsTypeDef",
+    "H265SettingsOutputTypeDef",
     "H265SettingsTypeDef",
-    "OutputSettingsTypeDef",
+    "OutputSettingsOutputTypeDef",
     "TimedMetadataInsertionOutputTypeDef",
     "TimedMetadataInsertionTypeDef",
     "ImageInserterOutputTypeDef",
     "ImageInserterTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "M2tsSettingsOutputTypeDef",
     "M2tsSettingsTypeDef",
+    "MotionImageInserterOutputTypeDef",
     "MotionImageInserterTypeDef",
+    "MxfSettingsOutputTypeDef",
     "MxfSettingsTypeDef",
+    "PartnerWatermarkingOutputTypeDef",
     "PartnerWatermarkingTypeDef",
+    "NoiseReducerOutputTypeDef",
     "NoiseReducerTypeDef",
     "OutputDetailTypeDef",
+    "PutPolicyRequestRequestTypeDef",
     "QueueTypeDef",
+    "S3DestinationSettingsOutputTypeDef",
     "S3DestinationSettingsTypeDef",
+    "XavcSettingsOutputTypeDef",
     "XavcSettingsTypeDef",
     "AutomatedAbrSettingsOutputTypeDef",
     "AutomatedAbrSettingsTypeDef",
+    "CaptionDescriptionOutputTypeDef",
     "CaptionDescriptionPresetOutputTypeDef",
     "CaptionDescriptionPresetTypeDef",
-    "CaptionDescriptionTypeDef",
+    "CaptionSourceSettingsOutputTypeDef",
     "CaptionSourceSettingsTypeDef",
     "RemixSettingsOutputTypeDef",
     "RemixSettingsTypeDef",
     "ContainerSettingsOutputTypeDef",
     "ContainerSettingsTypeDef",
     "VideoPreprocessorOutputTypeDef",
     "VideoPreprocessorTypeDef",
     "OutputGroupDetailTypeDef",
     "CreateQueueResponseTypeDef",
     "GetQueueResponseTypeDef",
     "ListQueuesResponseTypeDef",
     "UpdateQueueResponseTypeDef",
+    "DestinationSettingsOutputTypeDef",
     "DestinationSettingsTypeDef",
+    "VideoCodecSettingsOutputTypeDef",
     "VideoCodecSettingsTypeDef",
     "AutomatedEncodingSettingsOutputTypeDef",
     "AutomatedEncodingSettingsTypeDef",
+    "CaptionSelectorOutputTypeDef",
     "CaptionSelectorTypeDef",
     "AudioDescriptionOutputTypeDef",
     "AudioSelectorOutputTypeDef",
     "AudioDescriptionTypeDef",
     "AudioSelectorTypeDef",
     "CmafGroupSettingsOutputTypeDef",
-    "CmafGroupSettingsTypeDef",
     "DashIsoGroupSettingsOutputTypeDef",
+    "FileGroupSettingsOutputTypeDef",
+    "HlsGroupSettingsOutputTypeDef",
+    "MsSmoothGroupSettingsOutputTypeDef",
+    "CmafGroupSettingsTypeDef",
     "DashIsoGroupSettingsTypeDef",
     "FileGroupSettingsTypeDef",
-    "HlsGroupSettingsOutputTypeDef",
     "HlsGroupSettingsTypeDef",
-    "MsSmoothGroupSettingsOutputTypeDef",
     "MsSmoothGroupSettingsTypeDef",
     "VideoDescriptionOutputTypeDef",
     "VideoDescriptionTypeDef",
     "InputOutputTypeDef",
     "InputTemplateOutputTypeDef",
     "InputTemplateTypeDef",
     "InputTypeDef",
     "OutputGroupSettingsOutputTypeDef",
     "OutputGroupSettingsTypeDef",
-    "PresetSettingsOutputTypeDef",
     "OutputTypeDef",
+    "PresetSettingsOutputTypeDef",
     "PresetSettingsTypeDef",
-    "PresetTypeDef",
     "OutputGroupOutputTypeDef",
     "OutputGroupTypeDef",
+    "PresetTypeDef",
     "CreatePresetRequestRequestTypeDef",
-    "PresetSettingsUnionTypeDef",
     "UpdatePresetRequestRequestTypeDef",
-    "CreatePresetResponseTypeDef",
-    "GetPresetResponseTypeDef",
-    "ListPresetsResponseTypeDef",
-    "UpdatePresetResponseTypeDef",
     "JobSettingsOutputTypeDef",
     "JobTemplateSettingsOutputTypeDef",
     "JobSettingsTypeDef",
     "JobTemplateSettingsTypeDef",
+    "CreatePresetResponseTypeDef",
+    "GetPresetResponseTypeDef",
+    "ListPresetsResponseTypeDef",
+    "UpdatePresetResponseTypeDef",
     "JobTypeDef",
     "JobTemplateTypeDef",
     "CreateJobRequestRequestTypeDef",
-    "JobSettingsUnionTypeDef",
     "CreateJobTemplateRequestRequestTypeDef",
-    "JobTemplateSettingsUnionTypeDef",
     "UpdateJobTemplateRequestRequestTypeDef",
     "CreateJobResponseTypeDef",
     "GetJobResponseTypeDef",
     "ListJobsResponseTypeDef",
     "CreateJobTemplateResponseTypeDef",
     "GetJobTemplateResponseTypeDef",
     "ListJobTemplatesResponseTypeDef",
     "UpdateJobTemplateResponseTypeDef",
 )
 
+AacSettingsOutputTypeDef = TypedDict(
+    "AacSettingsOutputTypeDef",
+    {
+        "AudioDescriptionBroadcasterMix": AacAudioDescriptionBroadcasterMixType,
+        "Bitrate": int,
+        "CodecProfile": AacCodecProfileType,
+        "CodingMode": AacCodingModeType,
+        "RateControlMode": AacRateControlModeType,
+        "RawFormat": AacRawFormatType,
+        "SampleRate": int,
+        "Specification": AacSpecificationType,
+        "VbrQuality": AacVbrQualityType,
+    },
+)
+
 AacSettingsTypeDef = TypedDict(
     "AacSettingsTypeDef",
     {
         "AudioDescriptionBroadcasterMix": AacAudioDescriptionBroadcasterMixType,
         "Bitrate": int,
         "CodecProfile": AacCodecProfileType,
         "CodingMode": AacCodingModeType,
@@ -715,14 +843,30 @@
         "SampleRate": int,
         "Specification": AacSpecificationType,
         "VbrQuality": AacVbrQualityType,
     },
     total=False,
 )
 
+Ac3SettingsOutputTypeDef = TypedDict(
+    "Ac3SettingsOutputTypeDef",
+    {
+        "Bitrate": int,
+        "BitstreamMode": Ac3BitstreamModeType,
+        "CodingMode": Ac3CodingModeType,
+        "Dialnorm": int,
+        "DynamicRangeCompressionLine": Ac3DynamicRangeCompressionLineType,
+        "DynamicRangeCompressionProfile": Ac3DynamicRangeCompressionProfileType,
+        "DynamicRangeCompressionRf": Ac3DynamicRangeCompressionRfType,
+        "LfeFilter": Ac3LfeFilterType,
+        "MetadataControl": Ac3MetadataControlType,
+        "SampleRate": int,
+    },
+)
+
 Ac3SettingsTypeDef = TypedDict(
     "Ac3SettingsTypeDef",
     {
         "Bitrate": int,
         "BitstreamMode": Ac3BitstreamModeType,
         "CodingMode": Ac3CodingModeType,
         "Dialnorm": int,
@@ -732,50 +876,92 @@
         "LfeFilter": Ac3LfeFilterType,
         "MetadataControl": Ac3MetadataControlType,
         "SampleRate": int,
     },
     total=False,
 )
 
+AccelerationSettingsOutputTypeDef = TypedDict(
+    "AccelerationSettingsOutputTypeDef",
+    {
+        "Mode": AccelerationModeType,
+    },
+)
+
 AccelerationSettingsTypeDef = TypedDict(
     "AccelerationSettingsTypeDef",
     {
         "Mode": AccelerationModeType,
     },
 )
 
+AdvancedInputFilterSettingsOutputTypeDef = TypedDict(
+    "AdvancedInputFilterSettingsOutputTypeDef",
+    {
+        "AddTexture": AdvancedInputFilterAddTextureType,
+        "Sharpening": AdvancedInputFilterSharpenType,
+    },
+)
+
 AdvancedInputFilterSettingsTypeDef = TypedDict(
     "AdvancedInputFilterSettingsTypeDef",
     {
         "AddTexture": AdvancedInputFilterAddTextureType,
         "Sharpening": AdvancedInputFilterSharpenType,
     },
     total=False,
 )
 
+AiffSettingsOutputTypeDef = TypedDict(
+    "AiffSettingsOutputTypeDef",
+    {
+        "BitDepth": int,
+        "Channels": int,
+        "SampleRate": int,
+    },
+)
+
 AiffSettingsTypeDef = TypedDict(
     "AiffSettingsTypeDef",
     {
         "BitDepth": int,
         "Channels": int,
         "SampleRate": int,
     },
     total=False,
 )
 
+AllowedRenditionSizeOutputTypeDef = TypedDict(
+    "AllowedRenditionSizeOutputTypeDef",
+    {
+        "Height": int,
+        "Required": RequiredFlagType,
+        "Width": int,
+    },
+)
+
 AllowedRenditionSizeTypeDef = TypedDict(
     "AllowedRenditionSizeTypeDef",
     {
         "Height": int,
         "Required": RequiredFlagType,
         "Width": int,
     },
     total=False,
 )
 
+AncillarySourceSettingsOutputTypeDef = TypedDict(
+    "AncillarySourceSettingsOutputTypeDef",
+    {
+        "Convert608To708": AncillaryConvert608To708Type,
+        "SourceAncillaryChannelNumber": int,
+        "TerminateCaptions": AncillaryTerminateCaptionsType,
+    },
+)
+
 AncillarySourceSettingsTypeDef = TypedDict(
     "AncillarySourceSettingsTypeDef",
     {
         "Convert608To708": AncillaryConvert608To708Type,
         "SourceAncillaryChannelNumber": int,
         "TerminateCaptions": AncillaryTerminateCaptionsType,
     },
@@ -785,22 +971,127 @@
 AssociateCertificateRequestRequestTypeDef = TypedDict(
     "AssociateCertificateRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
+AudioChannelTaggingSettingsOutputTypeDef = TypedDict(
+    "AudioChannelTaggingSettingsOutputTypeDef",
+    {
+        "ChannelTag": AudioChannelTagType,
+    },
+)
+
 AudioChannelTaggingSettingsTypeDef = TypedDict(
     "AudioChannelTaggingSettingsTypeDef",
     {
         "ChannelTag": AudioChannelTagType,
     },
     total=False,
 )
 
+Eac3AtmosSettingsOutputTypeDef = TypedDict(
+    "Eac3AtmosSettingsOutputTypeDef",
+    {
+        "Bitrate": int,
+        "BitstreamMode": Literal["COMPLETE_MAIN"],
+        "CodingMode": Eac3AtmosCodingModeType,
+        "DialogueIntelligence": Eac3AtmosDialogueIntelligenceType,
+        "DownmixControl": Eac3AtmosDownmixControlType,
+        "DynamicRangeCompressionLine": Eac3AtmosDynamicRangeCompressionLineType,
+        "DynamicRangeCompressionRf": Eac3AtmosDynamicRangeCompressionRfType,
+        "DynamicRangeControl": Eac3AtmosDynamicRangeControlType,
+        "LoRoCenterMixLevel": float,
+        "LoRoSurroundMixLevel": float,
+        "LtRtCenterMixLevel": float,
+        "LtRtSurroundMixLevel": float,
+        "MeteringMode": Eac3AtmosMeteringModeType,
+        "SampleRate": int,
+        "SpeechThreshold": int,
+        "StereoDownmix": Eac3AtmosStereoDownmixType,
+        "SurroundExMode": Eac3AtmosSurroundExModeType,
+    },
+)
+
+Eac3SettingsOutputTypeDef = TypedDict(
+    "Eac3SettingsOutputTypeDef",
+    {
+        "AttenuationControl": Eac3AttenuationControlType,
+        "Bitrate": int,
+        "BitstreamMode": Eac3BitstreamModeType,
+        "CodingMode": Eac3CodingModeType,
+        "DcFilter": Eac3DcFilterType,
+        "Dialnorm": int,
+        "DynamicRangeCompressionLine": Eac3DynamicRangeCompressionLineType,
+        "DynamicRangeCompressionRf": Eac3DynamicRangeCompressionRfType,
+        "LfeControl": Eac3LfeControlType,
+        "LfeFilter": Eac3LfeFilterType,
+        "LoRoCenterMixLevel": float,
+        "LoRoSurroundMixLevel": float,
+        "LtRtCenterMixLevel": float,
+        "LtRtSurroundMixLevel": float,
+        "MetadataControl": Eac3MetadataControlType,
+        "PassthroughControl": Eac3PassthroughControlType,
+        "PhaseControl": Eac3PhaseControlType,
+        "SampleRate": int,
+        "StereoDownmix": Eac3StereoDownmixType,
+        "SurroundExMode": Eac3SurroundExModeType,
+        "SurroundMode": Eac3SurroundModeType,
+    },
+)
+
+Mp2SettingsOutputTypeDef = TypedDict(
+    "Mp2SettingsOutputTypeDef",
+    {
+        "Bitrate": int,
+        "Channels": int,
+        "SampleRate": int,
+    },
+)
+
+Mp3SettingsOutputTypeDef = TypedDict(
+    "Mp3SettingsOutputTypeDef",
+    {
+        "Bitrate": int,
+        "Channels": int,
+        "RateControlMode": Mp3RateControlModeType,
+        "SampleRate": int,
+        "VbrQuality": int,
+    },
+)
+
+OpusSettingsOutputTypeDef = TypedDict(
+    "OpusSettingsOutputTypeDef",
+    {
+        "Bitrate": int,
+        "Channels": int,
+        "SampleRate": int,
+    },
+)
+
+VorbisSettingsOutputTypeDef = TypedDict(
+    "VorbisSettingsOutputTypeDef",
+    {
+        "Channels": int,
+        "SampleRate": int,
+        "VbrQuality": int,
+    },
+)
+
+WavSettingsOutputTypeDef = TypedDict(
+    "WavSettingsOutputTypeDef",
+    {
+        "BitDepth": int,
+        "Channels": int,
+        "Format": WavFormatType,
+        "SampleRate": int,
+    },
+)
+
 Eac3AtmosSettingsTypeDef = TypedDict(
     "Eac3AtmosSettingsTypeDef",
     {
         "Bitrate": int,
         "BitstreamMode": Literal["COMPLETE_MAIN"],
         "CodingMode": Eac3AtmosCodingModeType,
         "DialogueIntelligence": Eac3AtmosDialogueIntelligenceType,
@@ -898,14 +1189,27 @@
         "Channels": int,
         "Format": WavFormatType,
         "SampleRate": int,
     },
     total=False,
 )
 
+AudioNormalizationSettingsOutputTypeDef = TypedDict(
+    "AudioNormalizationSettingsOutputTypeDef",
+    {
+        "Algorithm": AudioNormalizationAlgorithmType,
+        "AlgorithmControl": AudioNormalizationAlgorithmControlType,
+        "CorrectionGateLevel": int,
+        "LoudnessLogging": AudioNormalizationLoudnessLoggingType,
+        "PeakCalculation": AudioNormalizationPeakCalculationType,
+        "TargetLkfs": float,
+        "TruePeakLimiterThreshold": float,
+    },
+)
+
 AudioNormalizationSettingsTypeDef = TypedDict(
     "AudioNormalizationSettingsTypeDef",
     {
         "Algorithm": AudioNormalizationAlgorithmType,
         "AlgorithmControl": AudioNormalizationAlgorithmControlType,
         "CorrectionGateLevel": int,
         "LoudnessLogging": AudioNormalizationLoudnessLoggingType,
@@ -917,35 +1221,67 @@
 )
 
 AudioSelectorGroupOutputTypeDef = TypedDict(
     "AudioSelectorGroupOutputTypeDef",
     {
         "AudioSelectorNames": List[str],
     },
-    total=False,
 )
 
 AudioSelectorGroupTypeDef = TypedDict(
     "AudioSelectorGroupTypeDef",
     {
         "AudioSelectorNames": Sequence[str],
     },
     total=False,
 )
 
+HlsRenditionGroupSettingsOutputTypeDef = TypedDict(
+    "HlsRenditionGroupSettingsOutputTypeDef",
+    {
+        "RenditionGroupId": str,
+        "RenditionLanguageCode": LanguageCodeType,
+        "RenditionName": str,
+    },
+)
+
 HlsRenditionGroupSettingsTypeDef = TypedDict(
     "HlsRenditionGroupSettingsTypeDef",
     {
         "RenditionGroupId": str,
         "RenditionLanguageCode": LanguageCodeType,
         "RenditionName": str,
     },
     total=False,
 )
 
+ForceIncludeRenditionSizeOutputTypeDef = TypedDict(
+    "ForceIncludeRenditionSizeOutputTypeDef",
+    {
+        "Height": int,
+        "Width": int,
+    },
+)
+
+MinBottomRenditionSizeOutputTypeDef = TypedDict(
+    "MinBottomRenditionSizeOutputTypeDef",
+    {
+        "Height": int,
+        "Width": int,
+    },
+)
+
+MinTopRenditionSizeOutputTypeDef = TypedDict(
+    "MinTopRenditionSizeOutputTypeDef",
+    {
+        "Height": int,
+        "Width": int,
+    },
+)
+
 ForceIncludeRenditionSizeTypeDef = TypedDict(
     "ForceIncludeRenditionSizeTypeDef",
     {
         "Height": int,
         "Width": int,
     },
     total=False,
@@ -965,48 +1301,105 @@
     {
         "Height": int,
         "Width": int,
     },
     total=False,
 )
 
+Av1QvbrSettingsOutputTypeDef = TypedDict(
+    "Av1QvbrSettingsOutputTypeDef",
+    {
+        "QvbrQualityLevel": int,
+        "QvbrQualityLevelFineTune": float,
+    },
+)
+
 Av1QvbrSettingsTypeDef = TypedDict(
     "Av1QvbrSettingsTypeDef",
     {
         "QvbrQualityLevel": int,
         "QvbrQualityLevelFineTune": float,
     },
     total=False,
 )
 
+AvailBlankingOutputTypeDef = TypedDict(
+    "AvailBlankingOutputTypeDef",
+    {
+        "AvailBlankingImage": str,
+    },
+)
+
 AvailBlankingTypeDef = TypedDict(
     "AvailBlankingTypeDef",
     {
         "AvailBlankingImage": str,
     },
     total=False,
 )
 
+AvcIntraUhdSettingsOutputTypeDef = TypedDict(
+    "AvcIntraUhdSettingsOutputTypeDef",
+    {
+        "QualityTuningLevel": AvcIntraUhdQualityTuningLevelType,
+    },
+)
+
 AvcIntraUhdSettingsTypeDef = TypedDict(
     "AvcIntraUhdSettingsTypeDef",
     {
         "QualityTuningLevel": AvcIntraUhdQualityTuningLevelType,
     },
     total=False,
 )
 
+BandwidthReductionFilterOutputTypeDef = TypedDict(
+    "BandwidthReductionFilterOutputTypeDef",
+    {
+        "Sharpening": BandwidthReductionFilterSharpeningType,
+        "Strength": BandwidthReductionFilterStrengthType,
+    },
+)
+
 BandwidthReductionFilterTypeDef = TypedDict(
     "BandwidthReductionFilterTypeDef",
     {
         "Sharpening": BandwidthReductionFilterSharpeningType,
         "Strength": BandwidthReductionFilterStrengthType,
     },
     total=False,
 )
 
+BurninDestinationSettingsOutputTypeDef = TypedDict(
+    "BurninDestinationSettingsOutputTypeDef",
+    {
+        "Alignment": BurninSubtitleAlignmentType,
+        "ApplyFontColor": BurninSubtitleApplyFontColorType,
+        "BackgroundColor": BurninSubtitleBackgroundColorType,
+        "BackgroundOpacity": int,
+        "FallbackFont": BurninSubtitleFallbackFontType,
+        "FontColor": BurninSubtitleFontColorType,
+        "FontOpacity": int,
+        "FontResolution": int,
+        "FontScript": FontScriptType,
+        "FontSize": int,
+        "HexFontColor": str,
+        "OutlineColor": BurninSubtitleOutlineColorType,
+        "OutlineSize": int,
+        "ShadowColor": BurninSubtitleShadowColorType,
+        "ShadowOpacity": int,
+        "ShadowXOffset": int,
+        "ShadowYOffset": int,
+        "StylePassthrough": BurnInSubtitleStylePassthroughType,
+        "TeletextSpacing": BurninSubtitleTeletextSpacingType,
+        "XPosition": int,
+        "YPosition": int,
+    },
+)
+
 BurninDestinationSettingsTypeDef = TypedDict(
     "BurninDestinationSettingsTypeDef",
     {
         "Alignment": BurninSubtitleAlignmentType,
         "ApplyFontColor": BurninSubtitleApplyFontColorType,
         "BackgroundColor": BurninSubtitleBackgroundColorType,
         "BackgroundOpacity": int,
@@ -1034,14 +1427,100 @@
 CancelJobRequestRequestTypeDef = TypedDict(
     "CancelJobRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+DvbSubDestinationSettingsOutputTypeDef = TypedDict(
+    "DvbSubDestinationSettingsOutputTypeDef",
+    {
+        "Alignment": DvbSubtitleAlignmentType,
+        "ApplyFontColor": DvbSubtitleApplyFontColorType,
+        "BackgroundColor": DvbSubtitleBackgroundColorType,
+        "BackgroundOpacity": int,
+        "DdsHandling": DvbddsHandlingType,
+        "DdsXCoordinate": int,
+        "DdsYCoordinate": int,
+        "FallbackFont": DvbSubSubtitleFallbackFontType,
+        "FontColor": DvbSubtitleFontColorType,
+        "FontOpacity": int,
+        "FontResolution": int,
+        "FontScript": FontScriptType,
+        "FontSize": int,
+        "Height": int,
+        "HexFontColor": str,
+        "OutlineColor": DvbSubtitleOutlineColorType,
+        "OutlineSize": int,
+        "ShadowColor": DvbSubtitleShadowColorType,
+        "ShadowOpacity": int,
+        "ShadowXOffset": int,
+        "ShadowYOffset": int,
+        "StylePassthrough": DvbSubtitleStylePassthroughType,
+        "SubtitlingType": DvbSubtitlingTypeType,
+        "TeletextSpacing": DvbSubtitleTeletextSpacingType,
+        "Width": int,
+        "XPosition": int,
+        "YPosition": int,
+    },
+)
+
+EmbeddedDestinationSettingsOutputTypeDef = TypedDict(
+    "EmbeddedDestinationSettingsOutputTypeDef",
+    {
+        "Destination608ChannelNumber": int,
+        "Destination708ServiceNumber": int,
+    },
+)
+
+ImscDestinationSettingsOutputTypeDef = TypedDict(
+    "ImscDestinationSettingsOutputTypeDef",
+    {
+        "Accessibility": ImscAccessibilitySubsType,
+        "StylePassthrough": ImscStylePassthroughType,
+    },
+)
+
+SccDestinationSettingsOutputTypeDef = TypedDict(
+    "SccDestinationSettingsOutputTypeDef",
+    {
+        "Framerate": SccDestinationFramerateType,
+    },
+)
+
+SrtDestinationSettingsOutputTypeDef = TypedDict(
+    "SrtDestinationSettingsOutputTypeDef",
+    {
+        "StylePassthrough": SrtStylePassthroughType,
+    },
+)
+
+TeletextDestinationSettingsOutputTypeDef = TypedDict(
+    "TeletextDestinationSettingsOutputTypeDef",
+    {
+        "PageNumber": str,
+        "PageTypes": List[TeletextPageTypeType],
+    },
+)
+
+TtmlDestinationSettingsOutputTypeDef = TypedDict(
+    "TtmlDestinationSettingsOutputTypeDef",
+    {
+        "StylePassthrough": TtmlStylePassthroughType,
+    },
+)
+
+WebvttDestinationSettingsOutputTypeDef = TypedDict(
+    "WebvttDestinationSettingsOutputTypeDef",
+    {
+        "Accessibility": WebvttAccessibilitySubsType,
+        "StylePassthrough": WebvttStylePassthroughType,
+    },
+)
+
 DvbSubDestinationSettingsTypeDef = TypedDict(
     "DvbSubDestinationSettingsTypeDef",
     {
         "Alignment": DvbSubtitleAlignmentType,
         "ApplyFontColor": DvbSubtitleApplyFontColorType,
         "BackgroundColor": DvbSubtitleBackgroundColorType,
         "BackgroundOpacity": int,
@@ -1102,19 +1581,19 @@
     "SrtDestinationSettingsTypeDef",
     {
         "StylePassthrough": SrtStylePassthroughType,
     },
     total=False,
 )
 
-TeletextDestinationSettingsOutputTypeDef = TypedDict(
-    "TeletextDestinationSettingsOutputTypeDef",
+TeletextDestinationSettingsTypeDef = TypedDict(
+    "TeletextDestinationSettingsTypeDef",
     {
         "PageNumber": str,
-        "PageTypes": List[TeletextPageTypeType],
+        "PageTypes": Sequence[TeletextPageTypeType],
     },
     total=False,
 )
 
 TtmlDestinationSettingsTypeDef = TypedDict(
     "TtmlDestinationSettingsTypeDef",
     {
@@ -1128,32 +1607,71 @@
     {
         "Accessibility": WebvttAccessibilitySubsType,
         "StylePassthrough": WebvttStylePassthroughType,
     },
     total=False,
 )
 
-TeletextDestinationSettingsTypeDef = TypedDict(
-    "TeletextDestinationSettingsTypeDef",
+CaptionSourceFramerateOutputTypeDef = TypedDict(
+    "CaptionSourceFramerateOutputTypeDef",
     {
-        "PageNumber": str,
-        "PageTypes": Sequence[TeletextPageTypeType],
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
     },
-    total=False,
 )
 
 CaptionSourceFramerateTypeDef = TypedDict(
     "CaptionSourceFramerateTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
     },
     total=False,
 )
 
+DvbSubSourceSettingsOutputTypeDef = TypedDict(
+    "DvbSubSourceSettingsOutputTypeDef",
+    {
+        "Pid": int,
+    },
+)
+
+EmbeddedSourceSettingsOutputTypeDef = TypedDict(
+    "EmbeddedSourceSettingsOutputTypeDef",
+    {
+        "Convert608To708": EmbeddedConvert608To708Type,
+        "Source608ChannelNumber": int,
+        "Source608TrackNumber": int,
+        "TerminateCaptions": EmbeddedTerminateCaptionsType,
+    },
+)
+
+TeletextSourceSettingsOutputTypeDef = TypedDict(
+    "TeletextSourceSettingsOutputTypeDef",
+    {
+        "PageNumber": str,
+    },
+)
+
+TrackSourceSettingsOutputTypeDef = TypedDict(
+    "TrackSourceSettingsOutputTypeDef",
+    {
+        "TrackNumber": int,
+    },
+)
+
+WebvttHlsSourceSettingsOutputTypeDef = TypedDict(
+    "WebvttHlsSourceSettingsOutputTypeDef",
+    {
+        "RenditionGroupId": str,
+        "RenditionLanguageCode": LanguageCodeType,
+        "RenditionName": str,
+    },
+)
+
 DvbSubSourceSettingsTypeDef = TypedDict(
     "DvbSubSourceSettingsTypeDef",
     {
         "Pid": int,
     },
     total=False,
 )
@@ -1197,26 +1715,35 @@
 
 OutputChannelMappingOutputTypeDef = TypedDict(
     "OutputChannelMappingOutputTypeDef",
     {
         "InputChannels": List[int],
         "InputChannelsFineTune": List[float],
     },
-    total=False,
 )
 
 OutputChannelMappingTypeDef = TypedDict(
     "OutputChannelMappingTypeDef",
     {
         "InputChannels": Sequence[int],
         "InputChannelsFineTune": Sequence[float],
     },
     total=False,
 )
 
+ClipLimitsOutputTypeDef = TypedDict(
+    "ClipLimitsOutputTypeDef",
+    {
+        "MaximumRGBTolerance": int,
+        "MaximumYUV": int,
+        "MinimumRGBTolerance": int,
+        "MinimumYUV": int,
+    },
+)
+
 ClipLimitsTypeDef = TypedDict(
     "ClipLimitsTypeDef",
     {
         "MaximumRGBTolerance": int,
         "MaximumYUV": int,
         "MinimumRGBTolerance": int,
         "MinimumYUV": int,
@@ -1226,15 +1753,14 @@
 
 CmafAdditionalManifestOutputTypeDef = TypedDict(
     "CmafAdditionalManifestOutputTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": List[str],
     },
-    total=False,
 )
 
 CmafAdditionalManifestTypeDef = TypedDict(
     "CmafAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
@@ -1247,53 +1773,94 @@
     {
         "CertificateArn": str,
         "DashSignaledSystemIds": List[str],
         "HlsSignaledSystemIds": List[str],
         "ResourceId": str,
         "Url": str,
     },
-    total=False,
 )
 
-StaticKeyProviderTypeDef = TypedDict(
-    "StaticKeyProviderTypeDef",
+StaticKeyProviderOutputTypeDef = TypedDict(
+    "StaticKeyProviderOutputTypeDef",
     {
         "KeyFormat": str,
         "KeyFormatVersions": str,
         "StaticKeyValue": str,
         "Url": str,
     },
-    total=False,
 )
 
 SpekeKeyProviderCmafTypeDef = TypedDict(
     "SpekeKeyProviderCmafTypeDef",
     {
         "CertificateArn": str,
         "DashSignaledSystemIds": Sequence[str],
         "HlsSignaledSystemIds": Sequence[str],
         "ResourceId": str,
         "Url": str,
     },
     total=False,
 )
 
+StaticKeyProviderTypeDef = TypedDict(
+    "StaticKeyProviderTypeDef",
+    {
+        "KeyFormat": str,
+        "KeyFormatVersions": str,
+        "StaticKeyValue": str,
+        "Url": str,
+    },
+    total=False,
+)
+
+CmafImageBasedTrickPlaySettingsOutputTypeDef = TypedDict(
+    "CmafImageBasedTrickPlaySettingsOutputTypeDef",
+    {
+        "IntervalCadence": CmafIntervalCadenceType,
+        "ThumbnailHeight": int,
+        "ThumbnailInterval": float,
+        "ThumbnailWidth": int,
+        "TileHeight": int,
+        "TileWidth": int,
+    },
+)
+
 CmafImageBasedTrickPlaySettingsTypeDef = TypedDict(
     "CmafImageBasedTrickPlaySettingsTypeDef",
     {
         "IntervalCadence": CmafIntervalCadenceType,
         "ThumbnailHeight": int,
         "ThumbnailInterval": float,
         "ThumbnailWidth": int,
         "TileHeight": int,
         "TileWidth": int,
     },
     total=False,
 )
 
+CmfcSettingsOutputTypeDef = TypedDict(
+    "CmfcSettingsOutputTypeDef",
+    {
+        "AudioDuration": CmfcAudioDurationType,
+        "AudioGroupId": str,
+        "AudioRenditionSets": str,
+        "AudioTrackType": CmfcAudioTrackTypeType,
+        "DescriptiveVideoServiceFlag": CmfcDescriptiveVideoServiceFlagType,
+        "IFrameOnlyManifest": CmfcIFrameOnlyManifestType,
+        "KlvMetadata": CmfcKlvMetadataType,
+        "ManifestMetadataSignaling": CmfcManifestMetadataSignalingType,
+        "Scte35Esam": CmfcScte35EsamType,
+        "Scte35Source": CmfcScte35SourceType,
+        "TimedMetadata": CmfcTimedMetadataType,
+        "TimedMetadataBoxVersion": CmfcTimedMetadataBoxVersionType,
+        "TimedMetadataSchemeIdUri": str,
+        "TimedMetadataValue": str,
+    },
+)
+
 CmfcSettingsTypeDef = TypedDict(
     "CmfcSettingsTypeDef",
     {
         "AudioDuration": CmfcAudioDurationType,
         "AudioGroupId": str,
         "AudioRenditionSets": str,
         "AudioTrackType": CmfcAudioTrackTypeType,
@@ -1307,14 +1874,32 @@
         "TimedMetadataBoxVersion": CmfcTimedMetadataBoxVersionType,
         "TimedMetadataSchemeIdUri": str,
         "TimedMetadataValue": str,
     },
     total=False,
 )
 
+Hdr10MetadataOutputTypeDef = TypedDict(
+    "Hdr10MetadataOutputTypeDef",
+    {
+        "BluePrimaryX": int,
+        "BluePrimaryY": int,
+        "GreenPrimaryX": int,
+        "GreenPrimaryY": int,
+        "MaxContentLightLevel": int,
+        "MaxFrameAverageLightLevel": int,
+        "MaxLuminance": int,
+        "MinLuminance": int,
+        "RedPrimaryX": int,
+        "RedPrimaryY": int,
+        "WhitePointX": int,
+        "WhitePointY": int,
+    },
+)
+
 Hdr10MetadataTypeDef = TypedDict(
     "Hdr10MetadataTypeDef",
     {
         "BluePrimaryX": int,
         "BluePrimaryY": int,
         "GreenPrimaryX": int,
         "GreenPrimaryY": int,
@@ -1326,20 +1911,19 @@
         "RedPrimaryY": int,
         "WhitePointX": int,
         "WhitePointY": int,
     },
     total=False,
 )
 
-F4vSettingsTypeDef = TypedDict(
-    "F4vSettingsTypeDef",
+F4vSettingsOutputTypeDef = TypedDict(
+    "F4vSettingsOutputTypeDef",
     {
         "MoovPlacement": F4vMoovPlacementType,
     },
-    total=False,
 )
 
 M3u8SettingsOutputTypeDef = TypedDict(
     "M3u8SettingsOutputTypeDef",
     {
         "AudioDuration": M3u8AudioDurationType,
         "AudioFramesPerPes": int,
@@ -1357,57 +1941,61 @@
         "Scte35Pid": int,
         "Scte35Source": M3u8Scte35SourceType,
         "TimedMetadata": TimedMetadataType,
         "TimedMetadataPid": int,
         "TransportStreamId": int,
         "VideoPid": int,
     },
-    total=False,
 )
 
-MovSettingsTypeDef = TypedDict(
-    "MovSettingsTypeDef",
+MovSettingsOutputTypeDef = TypedDict(
+    "MovSettingsOutputTypeDef",
     {
         "ClapAtom": MovClapAtomType,
         "CslgAtom": MovCslgAtomType,
         "Mpeg2FourCCControl": MovMpeg2FourCCControlType,
         "PaddingControl": MovPaddingControlType,
         "Reference": MovReferenceType,
     },
-    total=False,
 )
 
-Mp4SettingsTypeDef = TypedDict(
-    "Mp4SettingsTypeDef",
+Mp4SettingsOutputTypeDef = TypedDict(
+    "Mp4SettingsOutputTypeDef",
     {
         "AudioDuration": CmfcAudioDurationType,
         "CslgAtom": Mp4CslgAtomType,
         "CttsVersion": int,
         "FreeSpaceBox": Mp4FreeSpaceBoxType,
         "MoovPlacement": Mp4MoovPlacementType,
         "Mp4MajorBrand": str,
     },
-    total=False,
 )
 
-MpdSettingsTypeDef = TypedDict(
-    "MpdSettingsTypeDef",
+MpdSettingsOutputTypeDef = TypedDict(
+    "MpdSettingsOutputTypeDef",
     {
         "AccessibilityCaptionHints": MpdAccessibilityCaptionHintsType,
         "AudioDuration": MpdAudioDurationType,
         "CaptionContainerType": MpdCaptionContainerTypeType,
         "KlvMetadata": MpdKlvMetadataType,
         "ManifestMetadataSignaling": MpdManifestMetadataSignalingType,
         "Scte35Esam": MpdScte35EsamType,
         "Scte35Source": MpdScte35SourceType,
         "TimedMetadata": MpdTimedMetadataType,
         "TimedMetadataBoxVersion": MpdTimedMetadataBoxVersionType,
         "TimedMetadataSchemeIdUri": str,
         "TimedMetadataValue": str,
     },
+)
+
+F4vSettingsTypeDef = TypedDict(
+    "F4vSettingsTypeDef",
+    {
+        "MoovPlacement": F4vMoovPlacementType,
+    },
     total=False,
 )
 
 M3u8SettingsTypeDef = TypedDict(
     "M3u8SettingsTypeDef",
     {
         "AudioDuration": M3u8AudioDurationType,
@@ -1429,14 +2017,57 @@
         "TimedMetadataPid": int,
         "TransportStreamId": int,
         "VideoPid": int,
     },
     total=False,
 )
 
+MovSettingsTypeDef = TypedDict(
+    "MovSettingsTypeDef",
+    {
+        "ClapAtom": MovClapAtomType,
+        "CslgAtom": MovCslgAtomType,
+        "Mpeg2FourCCControl": MovMpeg2FourCCControlType,
+        "PaddingControl": MovPaddingControlType,
+        "Reference": MovReferenceType,
+    },
+    total=False,
+)
+
+Mp4SettingsTypeDef = TypedDict(
+    "Mp4SettingsTypeDef",
+    {
+        "AudioDuration": CmfcAudioDurationType,
+        "CslgAtom": Mp4CslgAtomType,
+        "CttsVersion": int,
+        "FreeSpaceBox": Mp4FreeSpaceBoxType,
+        "MoovPlacement": Mp4MoovPlacementType,
+        "Mp4MajorBrand": str,
+    },
+    total=False,
+)
+
+MpdSettingsTypeDef = TypedDict(
+    "MpdSettingsTypeDef",
+    {
+        "AccessibilityCaptionHints": MpdAccessibilityCaptionHintsType,
+        "AudioDuration": MpdAudioDurationType,
+        "CaptionContainerType": MpdCaptionContainerTypeType,
+        "KlvMetadata": MpdKlvMetadataType,
+        "ManifestMetadataSignaling": MpdManifestMetadataSignalingType,
+        "Scte35Esam": MpdScte35EsamType,
+        "Scte35Source": MpdScte35SourceType,
+        "TimedMetadata": MpdTimedMetadataType,
+        "TimedMetadataBoxVersion": MpdTimedMetadataBoxVersionType,
+        "TimedMetadataSchemeIdUri": str,
+        "TimedMetadataValue": str,
+    },
+    total=False,
+)
+
 HopDestinationTypeDef = TypedDict(
     "HopDestinationTypeDef",
     {
         "Priority": int,
         "Queue": str,
         "WaitMinutes": int,
     },
@@ -1465,15 +2096,14 @@
 
 DashAdditionalManifestOutputTypeDef = TypedDict(
     "DashAdditionalManifestOutputTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": List[str],
     },
-    total=False,
 )
 
 DashAdditionalManifestTypeDef = TypedDict(
     "DashAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
@@ -1485,41 +2115,61 @@
     "SpekeKeyProviderOutputTypeDef",
     {
         "CertificateArn": str,
         "ResourceId": str,
         "SystemIds": List[str],
         "Url": str,
     },
-    total=False,
 )
 
 SpekeKeyProviderTypeDef = TypedDict(
     "SpekeKeyProviderTypeDef",
     {
         "CertificateArn": str,
         "ResourceId": str,
         "SystemIds": Sequence[str],
         "Url": str,
     },
     total=False,
 )
 
+DashIsoImageBasedTrickPlaySettingsOutputTypeDef = TypedDict(
+    "DashIsoImageBasedTrickPlaySettingsOutputTypeDef",
+    {
+        "IntervalCadence": DashIsoIntervalCadenceType,
+        "ThumbnailHeight": int,
+        "ThumbnailInterval": float,
+        "ThumbnailWidth": int,
+        "TileHeight": int,
+        "TileWidth": int,
+    },
+)
+
 DashIsoImageBasedTrickPlaySettingsTypeDef = TypedDict(
     "DashIsoImageBasedTrickPlaySettingsTypeDef",
     {
         "IntervalCadence": DashIsoIntervalCadenceType,
         "ThumbnailHeight": int,
         "ThumbnailInterval": float,
         "ThumbnailWidth": int,
         "TileHeight": int,
         "TileWidth": int,
     },
     total=False,
 )
 
+DeinterlacerOutputTypeDef = TypedDict(
+    "DeinterlacerOutputTypeDef",
+    {
+        "Algorithm": DeinterlaceAlgorithmType,
+        "Control": DeinterlacerControlType,
+        "Mode": DeinterlacerModeType,
+    },
+)
+
 DeinterlacerTypeDef = TypedDict(
     "DeinterlacerTypeDef",
     {
         "Algorithm": DeinterlaceAlgorithmType,
         "Control": DeinterlacerControlType,
         "Mode": DeinterlacerModeType,
     },
@@ -1568,87 +2218,152 @@
 )
 
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "Url": str,
     },
-    total=False,
 )
 
 DisassociateCertificateRequestRequestTypeDef = TypedDict(
     "DisassociateCertificateRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
+DolbyVisionLevel6MetadataOutputTypeDef = TypedDict(
+    "DolbyVisionLevel6MetadataOutputTypeDef",
+    {
+        "MaxCll": int,
+        "MaxFall": int,
+    },
+)
+
 DolbyVisionLevel6MetadataTypeDef = TypedDict(
     "DolbyVisionLevel6MetadataTypeDef",
     {
         "MaxCll": int,
         "MaxFall": int,
     },
     total=False,
 )
 
+DvbNitSettingsOutputTypeDef = TypedDict(
+    "DvbNitSettingsOutputTypeDef",
+    {
+        "NetworkId": int,
+        "NetworkName": str,
+        "NitInterval": int,
+    },
+)
+
 DvbNitSettingsTypeDef = TypedDict(
     "DvbNitSettingsTypeDef",
     {
         "NetworkId": int,
         "NetworkName": str,
         "NitInterval": int,
     },
     total=False,
 )
 
+DvbSdtSettingsOutputTypeDef = TypedDict(
+    "DvbSdtSettingsOutputTypeDef",
+    {
+        "OutputSdt": OutputSdtType,
+        "SdtInterval": int,
+        "ServiceName": str,
+        "ServiceProviderName": str,
+    },
+)
+
 DvbSdtSettingsTypeDef = TypedDict(
     "DvbSdtSettingsTypeDef",
     {
         "OutputSdt": OutputSdtType,
         "SdtInterval": int,
         "ServiceName": str,
         "ServiceProviderName": str,
     },
     total=False,
 )
 
+DvbTdtSettingsOutputTypeDef = TypedDict(
+    "DvbTdtSettingsOutputTypeDef",
+    {
+        "TdtInterval": int,
+    },
+)
+
 DvbTdtSettingsTypeDef = TypedDict(
     "DvbTdtSettingsTypeDef",
     {
         "TdtInterval": int,
     },
     total=False,
 )
 
+EsamManifestConfirmConditionNotificationOutputTypeDef = TypedDict(
+    "EsamManifestConfirmConditionNotificationOutputTypeDef",
+    {
+        "MccXml": str,
+    },
+)
+
 EsamManifestConfirmConditionNotificationTypeDef = TypedDict(
     "EsamManifestConfirmConditionNotificationTypeDef",
     {
         "MccXml": str,
     },
     total=False,
 )
 
+EsamSignalProcessingNotificationOutputTypeDef = TypedDict(
+    "EsamSignalProcessingNotificationOutputTypeDef",
+    {
+        "SccXml": str,
+    },
+)
+
 EsamSignalProcessingNotificationTypeDef = TypedDict(
     "EsamSignalProcessingNotificationTypeDef",
     {
         "SccXml": str,
     },
     total=False,
 )
 
+ExtendedDataServicesOutputTypeDef = TypedDict(
+    "ExtendedDataServicesOutputTypeDef",
+    {
+        "CopyProtectionAction": CopyProtectionActionType,
+        "VchipAction": VchipActionType,
+    },
+)
+
 ExtendedDataServicesTypeDef = TypedDict(
     "ExtendedDataServicesTypeDef",
     {
         "CopyProtectionAction": CopyProtectionActionType,
         "VchipAction": VchipActionType,
     },
     total=False,
 )
 
+FrameCaptureSettingsOutputTypeDef = TypedDict(
+    "FrameCaptureSettingsOutputTypeDef",
+    {
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "MaxCaptures": int,
+        "Quality": int,
+    },
+)
+
 FrameCaptureSettingsTypeDef = TypedDict(
     "FrameCaptureSettingsTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
         "MaxCaptures": int,
         "Quality": int,
@@ -1666,22 +2381,21 @@
 GetJobTemplateRequestRequestTypeDef = TypedDict(
     "GetJobTemplateRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-PolicyTypeDef = TypedDict(
-    "PolicyTypeDef",
+PolicyOutputTypeDef = TypedDict(
+    "PolicyOutputTypeDef",
     {
         "HttpInputs": InputPolicyType,
         "HttpsInputs": InputPolicyType,
         "S3Inputs": InputPolicyType,
     },
-    total=False,
 )
 
 GetPresetRequestRequestTypeDef = TypedDict(
     "GetPresetRequestRequestTypeDef",
     {
         "Name": str,
     },
@@ -1690,34 +2404,60 @@
 GetQueueRequestRequestTypeDef = TypedDict(
     "GetQueueRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+H264QvbrSettingsOutputTypeDef = TypedDict(
+    "H264QvbrSettingsOutputTypeDef",
+    {
+        "MaxAverageBitrate": int,
+        "QvbrQualityLevel": int,
+        "QvbrQualityLevelFineTune": float,
+    },
+)
+
 H264QvbrSettingsTypeDef = TypedDict(
     "H264QvbrSettingsTypeDef",
     {
         "MaxAverageBitrate": int,
         "QvbrQualityLevel": int,
         "QvbrQualityLevelFineTune": float,
     },
     total=False,
 )
 
+H265QvbrSettingsOutputTypeDef = TypedDict(
+    "H265QvbrSettingsOutputTypeDef",
+    {
+        "MaxAverageBitrate": int,
+        "QvbrQualityLevel": int,
+        "QvbrQualityLevelFineTune": float,
+    },
+)
+
 H265QvbrSettingsTypeDef = TypedDict(
     "H265QvbrSettingsTypeDef",
     {
         "MaxAverageBitrate": int,
         "QvbrQualityLevel": int,
         "QvbrQualityLevelFineTune": float,
     },
     total=False,
 )
 
+Hdr10PlusOutputTypeDef = TypedDict(
+    "Hdr10PlusOutputTypeDef",
+    {
+        "MasteringMonitorNits": int,
+        "TargetMonitorNits": int,
+    },
+)
+
 Hdr10PlusTypeDef = TypedDict(
     "Hdr10PlusTypeDef",
     {
         "MasteringMonitorNits": int,
         "TargetMonitorNits": int,
     },
     total=False,
@@ -1725,73 +2465,127 @@
 
 HlsAdditionalManifestOutputTypeDef = TypedDict(
     "HlsAdditionalManifestOutputTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": List[str],
     },
-    total=False,
 )
 
 HlsAdditionalManifestTypeDef = TypedDict(
     "HlsAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
     },
     total=False,
 )
 
+HlsCaptionLanguageMappingOutputTypeDef = TypedDict(
+    "HlsCaptionLanguageMappingOutputTypeDef",
+    {
+        "CaptionChannel": int,
+        "CustomLanguageCode": str,
+        "LanguageCode": LanguageCodeType,
+        "LanguageDescription": str,
+    },
+)
+
 HlsCaptionLanguageMappingTypeDef = TypedDict(
     "HlsCaptionLanguageMappingTypeDef",
     {
         "CaptionChannel": int,
         "CustomLanguageCode": str,
         "LanguageCode": LanguageCodeType,
         "LanguageDescription": str,
     },
     total=False,
 )
 
+HlsImageBasedTrickPlaySettingsOutputTypeDef = TypedDict(
+    "HlsImageBasedTrickPlaySettingsOutputTypeDef",
+    {
+        "IntervalCadence": HlsIntervalCadenceType,
+        "ThumbnailHeight": int,
+        "ThumbnailInterval": float,
+        "ThumbnailWidth": int,
+        "TileHeight": int,
+        "TileWidth": int,
+    },
+)
+
 HlsImageBasedTrickPlaySettingsTypeDef = TypedDict(
     "HlsImageBasedTrickPlaySettingsTypeDef",
     {
         "IntervalCadence": HlsIntervalCadenceType,
         "ThumbnailHeight": int,
         "ThumbnailInterval": float,
         "ThumbnailWidth": int,
         "TileHeight": int,
         "TileWidth": int,
     },
     total=False,
 )
 
-HlsSettingsTypeDef = TypedDict(
-    "HlsSettingsTypeDef",
+HlsSettingsOutputTypeDef = TypedDict(
+    "HlsSettingsOutputTypeDef",
     {
         "AudioGroupId": str,
         "AudioOnlyContainer": HlsAudioOnlyContainerType,
         "AudioRenditionSets": str,
         "AudioTrackType": HlsAudioTrackTypeType,
         "DescriptiveVideoServiceFlag": HlsDescriptiveVideoServiceFlagType,
         "IFrameOnlyManifest": HlsIFrameOnlyManifestType,
         "SegmentModifier": str,
     },
-    total=False,
+)
+
+HopDestinationOutputTypeDef = TypedDict(
+    "HopDestinationOutputTypeDef",
+    {
+        "Priority": int,
+        "Queue": str,
+        "WaitMinutes": int,
+    },
+)
+
+Id3InsertionOutputTypeDef = TypedDict(
+    "Id3InsertionOutputTypeDef",
+    {
+        "Id3": str,
+        "Timecode": str,
+    },
 )
 
 Id3InsertionTypeDef = TypedDict(
     "Id3InsertionTypeDef",
     {
         "Id3": str,
         "Timecode": str,
     },
     total=False,
 )
 
+InsertableImageOutputTypeDef = TypedDict(
+    "InsertableImageOutputTypeDef",
+    {
+        "Duration": int,
+        "FadeIn": int,
+        "FadeOut": int,
+        "Height": int,
+        "ImageInserterInput": str,
+        "ImageX": int,
+        "ImageY": int,
+        "Layer": int,
+        "Opacity": int,
+        "StartTime": str,
+        "Width": int,
+    },
+)
+
 InsertableImageTypeDef = TypedDict(
     "InsertableImageTypeDef",
     {
         "Duration": int,
         "FadeIn": int,
         "FadeOut": int,
         "Height": int,
@@ -1802,60 +2596,148 @@
         "Opacity": int,
         "StartTime": str,
         "Width": int,
     },
     total=False,
 )
 
+InputClippingOutputTypeDef = TypedDict(
+    "InputClippingOutputTypeDef",
+    {
+        "EndTimecode": str,
+        "StartTimecode": str,
+    },
+)
+
 InputClippingTypeDef = TypedDict(
     "InputClippingTypeDef",
     {
         "EndTimecode": str,
         "StartTimecode": str,
     },
     total=False,
 )
 
+InputDecryptionSettingsOutputTypeDef = TypedDict(
+    "InputDecryptionSettingsOutputTypeDef",
+    {
+        "DecryptionMode": DecryptionModeType,
+        "EncryptedDecryptionKey": str,
+        "InitializationVector": str,
+        "KmsKeyRegion": str,
+    },
+)
+
 InputDecryptionSettingsTypeDef = TypedDict(
     "InputDecryptionSettingsTypeDef",
     {
         "DecryptionMode": DecryptionModeType,
         "EncryptedDecryptionKey": str,
         "InitializationVector": str,
         "KmsKeyRegion": str,
     },
     total=False,
 )
 
-InputVideoGeneratorTypeDef = TypedDict(
-    "InputVideoGeneratorTypeDef",
+InputVideoGeneratorOutputTypeDef = TypedDict(
+    "InputVideoGeneratorOutputTypeDef",
     {
         "Duration": int,
     },
-    total=False,
+)
+
+RectangleOutputTypeDef = TypedDict(
+    "RectangleOutputTypeDef",
+    {
+        "Height": int,
+        "Width": int,
+        "X": int,
+        "Y": int,
+    },
 )
 
 RectangleTypeDef = TypedDict(
     "RectangleTypeDef",
     {
         "Height": int,
         "Width": int,
         "X": int,
         "Y": int,
     },
     total=False,
 )
 
+InputVideoGeneratorTypeDef = TypedDict(
+    "InputVideoGeneratorTypeDef",
+    {
+        "Duration": int,
+    },
+    total=False,
+)
+
 JobMessagesTypeDef = TypedDict(
     "JobMessagesTypeDef",
     {
         "Info": List[str],
         "Warning": List[str],
     },
-    total=False,
+)
+
+KantarWatermarkSettingsOutputTypeDef = TypedDict(
+    "KantarWatermarkSettingsOutputTypeDef",
+    {
+        "ChannelName": str,
+        "ContentReference": str,
+        "CredentialsSecretName": str,
+        "FileOffset": float,
+        "KantarLicenseId": int,
+        "KantarServerUrl": str,
+        "LogDestination": str,
+        "Metadata3": str,
+        "Metadata4": str,
+        "Metadata5": str,
+        "Metadata6": str,
+        "Metadata7": str,
+        "Metadata8": str,
+    },
+)
+
+NielsenConfigurationOutputTypeDef = TypedDict(
+    "NielsenConfigurationOutputTypeDef",
+    {
+        "BreakoutCode": int,
+        "DistributorId": str,
+    },
+)
+
+NielsenNonLinearWatermarkSettingsOutputTypeDef = TypedDict(
+    "NielsenNonLinearWatermarkSettingsOutputTypeDef",
+    {
+        "ActiveWatermarkProcess": NielsenActiveWatermarkProcessTypeType,
+        "AdiFilename": str,
+        "AssetId": str,
+        "AssetName": str,
+        "CbetSourceId": str,
+        "EpisodeId": str,
+        "MetadataDestination": str,
+        "SourceId": int,
+        "SourceWatermarkStatus": NielsenSourceWatermarkStatusTypeType,
+        "TicServerUrl": str,
+        "UniqueTicPerAudioTrack": NielsenUniqueTicPerAudioTrackTypeType,
+    },
+)
+
+TimecodeConfigOutputTypeDef = TypedDict(
+    "TimecodeConfigOutputTypeDef",
+    {
+        "Anchor": str,
+        "Source": TimecodeSourceType,
+        "Start": str,
+        "TimestampOffset": str,
+    },
 )
 
 KantarWatermarkSettingsTypeDef = TypedDict(
     "KantarWatermarkSettingsTypeDef",
     {
         "ChannelName": str,
         "ContentReference": str,
@@ -1915,25 +2797,23 @@
 QueueTransitionTypeDef = TypedDict(
     "QueueTransitionTypeDef",
     {
         "DestinationQueue": str,
         "SourceQueue": str,
         "Timestamp": datetime,
     },
-    total=False,
 )
 
 TimingTypeDef = TypedDict(
     "TimingTypeDef",
     {
         "FinishTime": datetime,
         "StartTime": datetime,
         "SubmitTime": datetime,
     },
-    total=False,
 )
 
 WarningGroupTypeDef = TypedDict(
     "WarningGroupTypeDef",
     {
         "Code": int,
         "Count": int,
@@ -1996,25 +2876,47 @@
 
 ResourceTagsTypeDef = TypedDict(
     "ResourceTagsTypeDef",
     {
         "Arn": str,
         "Tags": Dict[str, str],
     },
-    total=False,
+)
+
+M2tsScte35EsamOutputTypeDef = TypedDict(
+    "M2tsScte35EsamOutputTypeDef",
+    {
+        "Scte35EsamPid": int,
+    },
 )
 
 M2tsScte35EsamTypeDef = TypedDict(
     "M2tsScte35EsamTypeDef",
     {
         "Scte35EsamPid": int,
     },
     total=False,
 )
 
+MotionImageInsertionFramerateOutputTypeDef = TypedDict(
+    "MotionImageInsertionFramerateOutputTypeDef",
+    {
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+    },
+)
+
+MotionImageInsertionOffsetOutputTypeDef = TypedDict(
+    "MotionImageInsertionOffsetOutputTypeDef",
+    {
+        "ImageX": int,
+        "ImageY": int,
+    },
+)
+
 MotionImageInsertionFramerateTypeDef = TypedDict(
     "MotionImageInsertionFramerateTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
     },
     total=False,
@@ -2025,14 +2927,53 @@
     {
         "ImageX": int,
         "ImageY": int,
     },
     total=False,
 )
 
+Mpeg2SettingsOutputTypeDef = TypedDict(
+    "Mpeg2SettingsOutputTypeDef",
+    {
+        "AdaptiveQuantization": Mpeg2AdaptiveQuantizationType,
+        "Bitrate": int,
+        "CodecLevel": Mpeg2CodecLevelType,
+        "CodecProfile": Mpeg2CodecProfileType,
+        "DynamicSubGop": Mpeg2DynamicSubGopType,
+        "FramerateControl": Mpeg2FramerateControlType,
+        "FramerateConversionAlgorithm": Mpeg2FramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "GopClosedCadence": int,
+        "GopSize": float,
+        "GopSizeUnits": Mpeg2GopSizeUnitsType,
+        "HrdBufferFinalFillPercentage": int,
+        "HrdBufferInitialFillPercentage": int,
+        "HrdBufferSize": int,
+        "InterlaceMode": Mpeg2InterlaceModeType,
+        "IntraDcPrecision": Mpeg2IntraDcPrecisionType,
+        "MaxBitrate": int,
+        "MinIInterval": int,
+        "NumberBFramesBetweenReferenceFrames": int,
+        "ParControl": Mpeg2ParControlType,
+        "ParDenominator": int,
+        "ParNumerator": int,
+        "QualityTuningLevel": Mpeg2QualityTuningLevelType,
+        "RateControlMode": Mpeg2RateControlModeType,
+        "ScanTypeConversionMode": Mpeg2ScanTypeConversionModeType,
+        "SceneChangeDetect": Mpeg2SceneChangeDetectType,
+        "SlowPal": Mpeg2SlowPalType,
+        "Softness": int,
+        "SpatialAdaptiveQuantization": Mpeg2SpatialAdaptiveQuantizationType,
+        "Syntax": Mpeg2SyntaxType,
+        "Telecine": Mpeg2TelecineType,
+        "TemporalAdaptiveQuantization": Mpeg2TemporalAdaptiveQuantizationType,
+    },
+)
+
 Mpeg2SettingsTypeDef = TypedDict(
     "Mpeg2SettingsTypeDef",
     {
         "AdaptiveQuantization": Mpeg2AdaptiveQuantizationType,
         "Bitrate": int,
         "CodecLevel": Mpeg2CodecLevelType,
         "CodecProfile": Mpeg2CodecProfileType,
@@ -2071,54 +3012,98 @@
 
 MsSmoothAdditionalManifestOutputTypeDef = TypedDict(
     "MsSmoothAdditionalManifestOutputTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": List[str],
     },
-    total=False,
 )
 
 MsSmoothAdditionalManifestTypeDef = TypedDict(
     "MsSmoothAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
     },
     total=False,
 )
 
+MxfXavcProfileSettingsOutputTypeDef = TypedDict(
+    "MxfXavcProfileSettingsOutputTypeDef",
+    {
+        "DurationMode": MxfXavcDurationModeType,
+        "MaxAncDataSize": int,
+    },
+)
+
 MxfXavcProfileSettingsTypeDef = TypedDict(
     "MxfXavcProfileSettingsTypeDef",
     {
         "DurationMode": MxfXavcDurationModeType,
         "MaxAncDataSize": int,
     },
     total=False,
 )
 
+NexGuardFileMarkerSettingsOutputTypeDef = TypedDict(
+    "NexGuardFileMarkerSettingsOutputTypeDef",
+    {
+        "License": str,
+        "Payload": int,
+        "Preset": str,
+        "Strength": WatermarkingStrengthType,
+    },
+)
+
 NexGuardFileMarkerSettingsTypeDef = TypedDict(
     "NexGuardFileMarkerSettingsTypeDef",
     {
         "License": str,
         "Payload": int,
         "Preset": str,
         "Strength": WatermarkingStrengthType,
     },
     total=False,
 )
 
+NoiseReducerFilterSettingsOutputTypeDef = TypedDict(
+    "NoiseReducerFilterSettingsOutputTypeDef",
+    {
+        "Strength": int,
+    },
+)
+
 NoiseReducerFilterSettingsTypeDef = TypedDict(
     "NoiseReducerFilterSettingsTypeDef",
     {
         "Strength": int,
     },
     total=False,
 )
 
+NoiseReducerSpatialFilterSettingsOutputTypeDef = TypedDict(
+    "NoiseReducerSpatialFilterSettingsOutputTypeDef",
+    {
+        "PostFilterSharpenStrength": int,
+        "Speed": int,
+        "Strength": int,
+    },
+)
+
+NoiseReducerTemporalFilterSettingsOutputTypeDef = TypedDict(
+    "NoiseReducerTemporalFilterSettingsOutputTypeDef",
+    {
+        "AggressiveMode": int,
+        "PostTemporalSharpening": NoiseFilterPostTemporalSharpeningType,
+        "PostTemporalSharpeningStrength": NoiseFilterPostTemporalSharpeningStrengthType,
+        "Speed": int,
+        "Strength": int,
+    },
+)
+
 NoiseReducerSpatialFilterSettingsTypeDef = TypedDict(
     "NoiseReducerSpatialFilterSettingsTypeDef",
     {
         "PostFilterSharpenStrength": int,
         "Speed": int,
         "Strength": int,
     },
@@ -2139,17 +3124,45 @@
 
 VideoDetailTypeDef = TypedDict(
     "VideoDetailTypeDef",
     {
         "HeightInPx": int,
         "WidthInPx": int,
     },
+)
+
+PolicyTypeDef = TypedDict(
+    "PolicyTypeDef",
+    {
+        "HttpInputs": InputPolicyType,
+        "HttpsInputs": InputPolicyType,
+        "S3Inputs": InputPolicyType,
+    },
     total=False,
 )
 
+ProresSettingsOutputTypeDef = TypedDict(
+    "ProresSettingsOutputTypeDef",
+    {
+        "ChromaSampling": ProresChromaSamplingType,
+        "CodecProfile": ProresCodecProfileType,
+        "FramerateControl": ProresFramerateControlType,
+        "FramerateConversionAlgorithm": ProresFramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "InterlaceMode": ProresInterlaceModeType,
+        "ParControl": ProresParControlType,
+        "ParDenominator": int,
+        "ParNumerator": int,
+        "ScanTypeConversionMode": ProresScanTypeConversionModeType,
+        "SlowPal": ProresSlowPalType,
+        "Telecine": ProresTelecineType,
+    },
+)
+
 ProresSettingsTypeDef = TypedDict(
     "ProresSettingsTypeDef",
     {
         "ChromaSampling": ProresChromaSamplingType,
         "CodecProfile": ProresCodecProfileType,
         "FramerateControl": ProresFramerateControlType,
         "FramerateConversionAlgorithm": ProresFramerateConversionAlgorithmType,
@@ -2172,25 +3185,40 @@
         "Commitment": Literal["ONE_YEAR"],
         "ExpiresAt": datetime,
         "PurchasedAt": datetime,
         "RenewalType": RenewalTypeType,
         "ReservedSlots": int,
         "Status": ReservationPlanStatusType,
     },
-    total=False,
+)
+
+S3DestinationAccessControlOutputTypeDef = TypedDict(
+    "S3DestinationAccessControlOutputTypeDef",
+    {
+        "CannedAcl": S3ObjectCannedAclType,
+    },
 )
 
 S3DestinationAccessControlTypeDef = TypedDict(
     "S3DestinationAccessControlTypeDef",
     {
         "CannedAcl": S3ObjectCannedAclType,
     },
     total=False,
 )
 
+S3EncryptionSettingsOutputTypeDef = TypedDict(
+    "S3EncryptionSettingsOutputTypeDef",
+    {
+        "EncryptionType": S3ServerSideEncryptionTypeType,
+        "KmsEncryptionContext": str,
+        "KmsKeyArn": str,
+    },
+)
+
 S3EncryptionSettingsTypeDef = TypedDict(
     "S3EncryptionSettingsTypeDef",
     {
         "EncryptionType": S3ServerSideEncryptionTypeType,
         "KmsEncryptionContext": str,
         "KmsKeyArn": str,
     },
@@ -2201,14 +3229,23 @@
     "TagResourceRequestRequestTypeDef",
     {
         "Arn": str,
         "Tags": Mapping[str, str],
     },
 )
 
+TimecodeBurninOutputTypeDef = TypedDict(
+    "TimecodeBurninOutputTypeDef",
+    {
+        "FontSize": int,
+        "Position": TimecodeBurninPositionType,
+        "Prefix": str,
+    },
+)
+
 TimecodeBurninTypeDef = TypedDict(
     "TimecodeBurninTypeDef",
     {
         "FontSize": int,
         "Position": TimecodeBurninPositionType,
         "Prefix": str,
     },
@@ -2230,14 +3267,29 @@
 )
 
 class UntagResourceRequestRequestTypeDef(
     _RequiredUntagResourceRequestRequestTypeDef, _OptionalUntagResourceRequestRequestTypeDef
 ):
     pass
 
+Vc3SettingsOutputTypeDef = TypedDict(
+    "Vc3SettingsOutputTypeDef",
+    {
+        "FramerateControl": Vc3FramerateControlType,
+        "FramerateConversionAlgorithm": Vc3FramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "InterlaceMode": Vc3InterlaceModeType,
+        "ScanTypeConversionMode": Vc3ScanTypeConversionModeType,
+        "SlowPal": Vc3SlowPalType,
+        "Telecine": Vc3TelecineType,
+        "Vc3Class": Vc3ClassType,
+    },
+)
+
 Vc3SettingsTypeDef = TypedDict(
     "Vc3SettingsTypeDef",
     {
         "FramerateControl": Vc3FramerateControlType,
         "FramerateConversionAlgorithm": Vc3FramerateConversionAlgorithmType,
         "FramerateDenominator": int,
         "FramerateNumerator": int,
@@ -2246,14 +3298,52 @@
         "SlowPal": Vc3SlowPalType,
         "Telecine": Vc3TelecineType,
         "Vc3Class": Vc3ClassType,
     },
     total=False,
 )
 
+Vp8SettingsOutputTypeDef = TypedDict(
+    "Vp8SettingsOutputTypeDef",
+    {
+        "Bitrate": int,
+        "FramerateControl": Vp8FramerateControlType,
+        "FramerateConversionAlgorithm": Vp8FramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "GopSize": float,
+        "HrdBufferSize": int,
+        "MaxBitrate": int,
+        "ParControl": Vp8ParControlType,
+        "ParDenominator": int,
+        "ParNumerator": int,
+        "QualityTuningLevel": Vp8QualityTuningLevelType,
+        "RateControlMode": Literal["VBR"],
+    },
+)
+
+Vp9SettingsOutputTypeDef = TypedDict(
+    "Vp9SettingsOutputTypeDef",
+    {
+        "Bitrate": int,
+        "FramerateControl": Vp9FramerateControlType,
+        "FramerateConversionAlgorithm": Vp9FramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "GopSize": float,
+        "HrdBufferSize": int,
+        "MaxBitrate": int,
+        "ParControl": Vp9ParControlType,
+        "ParDenominator": int,
+        "ParNumerator": int,
+        "QualityTuningLevel": Vp9QualityTuningLevelType,
+        "RateControlMode": Literal["VBR"],
+    },
+)
+
 Vp8SettingsTypeDef = TypedDict(
     "Vp8SettingsTypeDef",
     {
         "Bitrate": int,
         "FramerateControl": Vp8FramerateControlType,
         "FramerateConversionAlgorithm": Vp8FramerateConversionAlgorithmType,
         "FramerateDenominator": int,
@@ -2286,30 +3376,58 @@
         "ParNumerator": int,
         "QualityTuningLevel": Vp9QualityTuningLevelType,
         "RateControlMode": Literal["VBR"],
     },
     total=False,
 )
 
+Xavc4kIntraCbgProfileSettingsOutputTypeDef = TypedDict(
+    "Xavc4kIntraCbgProfileSettingsOutputTypeDef",
+    {
+        "XavcClass": Xavc4kIntraCbgProfileClassType,
+    },
+)
+
 Xavc4kIntraCbgProfileSettingsTypeDef = TypedDict(
     "Xavc4kIntraCbgProfileSettingsTypeDef",
     {
         "XavcClass": Xavc4kIntraCbgProfileClassType,
     },
     total=False,
 )
 
+Xavc4kIntraVbrProfileSettingsOutputTypeDef = TypedDict(
+    "Xavc4kIntraVbrProfileSettingsOutputTypeDef",
+    {
+        "XavcClass": Xavc4kIntraVbrProfileClassType,
+    },
+)
+
 Xavc4kIntraVbrProfileSettingsTypeDef = TypedDict(
     "Xavc4kIntraVbrProfileSettingsTypeDef",
     {
         "XavcClass": Xavc4kIntraVbrProfileClassType,
     },
     total=False,
 )
 
+Xavc4kProfileSettingsOutputTypeDef = TypedDict(
+    "Xavc4kProfileSettingsOutputTypeDef",
+    {
+        "BitrateClass": Xavc4kProfileBitrateClassType,
+        "CodecProfile": Xavc4kProfileCodecProfileType,
+        "FlickerAdaptiveQuantization": XavcFlickerAdaptiveQuantizationType,
+        "GopBReference": XavcGopBReferenceType,
+        "GopClosedCadence": int,
+        "HrdBufferSize": int,
+        "QualityTuningLevel": Xavc4kProfileQualityTuningLevelType,
+        "Slices": int,
+    },
+)
+
 Xavc4kProfileSettingsTypeDef = TypedDict(
     "Xavc4kProfileSettingsTypeDef",
     {
         "BitrateClass": Xavc4kProfileBitrateClassType,
         "CodecProfile": Xavc4kProfileCodecProfileType,
         "FlickerAdaptiveQuantization": XavcFlickerAdaptiveQuantizationType,
         "GopBReference": XavcGopBReferenceType,
@@ -2317,22 +3435,44 @@
         "HrdBufferSize": int,
         "QualityTuningLevel": Xavc4kProfileQualityTuningLevelType,
         "Slices": int,
     },
     total=False,
 )
 
+XavcHdIntraCbgProfileSettingsOutputTypeDef = TypedDict(
+    "XavcHdIntraCbgProfileSettingsOutputTypeDef",
+    {
+        "XavcClass": XavcHdIntraCbgProfileClassType,
+    },
+)
+
 XavcHdIntraCbgProfileSettingsTypeDef = TypedDict(
     "XavcHdIntraCbgProfileSettingsTypeDef",
     {
         "XavcClass": XavcHdIntraCbgProfileClassType,
     },
     total=False,
 )
 
+XavcHdProfileSettingsOutputTypeDef = TypedDict(
+    "XavcHdProfileSettingsOutputTypeDef",
+    {
+        "BitrateClass": XavcHdProfileBitrateClassType,
+        "FlickerAdaptiveQuantization": XavcFlickerAdaptiveQuantizationType,
+        "GopBReference": XavcGopBReferenceType,
+        "GopClosedCadence": int,
+        "HrdBufferSize": int,
+        "InterlaceMode": XavcInterlaceModeType,
+        "QualityTuningLevel": XavcHdProfileQualityTuningLevelType,
+        "Slices": int,
+        "Telecine": XavcHdProfileTelecineType,
+    },
+)
+
 XavcHdProfileSettingsTypeDef = TypedDict(
     "XavcHdProfileSettingsTypeDef",
     {
         "BitrateClass": XavcHdProfileBitrateClassType,
         "FlickerAdaptiveQuantization": XavcFlickerAdaptiveQuantizationType,
         "GopBReference": XavcGopBReferenceType,
         "GopClosedCadence": int,
@@ -2341,14 +3481,31 @@
         "QualityTuningLevel": XavcHdProfileQualityTuningLevelType,
         "Slices": int,
         "Telecine": XavcHdProfileTelecineType,
     },
     total=False,
 )
 
+AudioCodecSettingsOutputTypeDef = TypedDict(
+    "AudioCodecSettingsOutputTypeDef",
+    {
+        "AacSettings": AacSettingsOutputTypeDef,
+        "Ac3Settings": Ac3SettingsOutputTypeDef,
+        "AiffSettings": AiffSettingsOutputTypeDef,
+        "Codec": AudioCodecType,
+        "Eac3AtmosSettings": Eac3AtmosSettingsOutputTypeDef,
+        "Eac3Settings": Eac3SettingsOutputTypeDef,
+        "Mp2Settings": Mp2SettingsOutputTypeDef,
+        "Mp3Settings": Mp3SettingsOutputTypeDef,
+        "OpusSettings": OpusSettingsOutputTypeDef,
+        "VorbisSettings": VorbisSettingsOutputTypeDef,
+        "WavSettings": WavSettingsOutputTypeDef,
+    },
+)
+
 AudioCodecSettingsTypeDef = TypedDict(
     "AudioCodecSettingsTypeDef",
     {
         "AacSettings": AacSettingsTypeDef,
         "Ac3Settings": Ac3SettingsTypeDef,
         "AiffSettings": AiffSettingsTypeDef,
         "Codec": AudioCodecType,
@@ -2362,35 +3519,53 @@
     },
     total=False,
 )
 
 AutomatedAbrRuleOutputTypeDef = TypedDict(
     "AutomatedAbrRuleOutputTypeDef",
     {
-        "AllowedRenditions": List[AllowedRenditionSizeTypeDef],
-        "ForceIncludeRenditions": List[ForceIncludeRenditionSizeTypeDef],
-        "MinBottomRenditionSize": MinBottomRenditionSizeTypeDef,
-        "MinTopRenditionSize": MinTopRenditionSizeTypeDef,
+        "AllowedRenditions": List[AllowedRenditionSizeOutputTypeDef],
+        "ForceIncludeRenditions": List[ForceIncludeRenditionSizeOutputTypeDef],
+        "MinBottomRenditionSize": MinBottomRenditionSizeOutputTypeDef,
+        "MinTopRenditionSize": MinTopRenditionSizeOutputTypeDef,
         "Type": RuleTypeType,
     },
-    total=False,
 )
 
 AutomatedAbrRuleTypeDef = TypedDict(
     "AutomatedAbrRuleTypeDef",
     {
         "AllowedRenditions": Sequence[AllowedRenditionSizeTypeDef],
         "ForceIncludeRenditions": Sequence[ForceIncludeRenditionSizeTypeDef],
         "MinBottomRenditionSize": MinBottomRenditionSizeTypeDef,
         "MinTopRenditionSize": MinTopRenditionSizeTypeDef,
         "Type": RuleTypeType,
     },
     total=False,
 )
 
+Av1SettingsOutputTypeDef = TypedDict(
+    "Av1SettingsOutputTypeDef",
+    {
+        "AdaptiveQuantization": Av1AdaptiveQuantizationType,
+        "BitDepth": Av1BitDepthType,
+        "FramerateControl": Av1FramerateControlType,
+        "FramerateConversionAlgorithm": Av1FramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "GopSize": float,
+        "MaxBitrate": int,
+        "NumberBFramesBetweenReferenceFrames": int,
+        "QvbrSettings": Av1QvbrSettingsOutputTypeDef,
+        "RateControlMode": Literal["QVBR"],
+        "Slices": int,
+        "SpatialAdaptiveQuantization": Av1SpatialAdaptiveQuantizationType,
+    },
+)
+
 Av1SettingsTypeDef = TypedDict(
     "Av1SettingsTypeDef",
     {
         "AdaptiveQuantization": Av1AdaptiveQuantizationType,
         "BitDepth": Av1BitDepthType,
         "FramerateControl": Av1FramerateControlType,
         "FramerateConversionAlgorithm": Av1FramerateConversionAlgorithmType,
@@ -2403,14 +3578,30 @@
         "RateControlMode": Literal["QVBR"],
         "Slices": int,
         "SpatialAdaptiveQuantization": Av1SpatialAdaptiveQuantizationType,
     },
     total=False,
 )
 
+AvcIntraSettingsOutputTypeDef = TypedDict(
+    "AvcIntraSettingsOutputTypeDef",
+    {
+        "AvcIntraClass": AvcIntraClassType,
+        "AvcIntraUhdSettings": AvcIntraUhdSettingsOutputTypeDef,
+        "FramerateControl": AvcIntraFramerateControlType,
+        "FramerateConversionAlgorithm": AvcIntraFramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "InterlaceMode": AvcIntraInterlaceModeType,
+        "ScanTypeConversionMode": AvcIntraScanTypeConversionModeType,
+        "SlowPal": AvcIntraSlowPalType,
+        "Telecine": AvcIntraTelecineType,
+    },
+)
+
 AvcIntraSettingsTypeDef = TypedDict(
     "AvcIntraSettingsTypeDef",
     {
         "AvcIntraClass": AvcIntraClassType,
         "AvcIntraUhdSettings": AvcIntraUhdSettingsTypeDef,
         "FramerateControl": AvcIntraFramerateControlType,
         "FramerateConversionAlgorithm": AvcIntraFramerateConversionAlgorithmType,
@@ -2423,26 +3614,25 @@
     },
     total=False,
 )
 
 CaptionDestinationSettingsOutputTypeDef = TypedDict(
     "CaptionDestinationSettingsOutputTypeDef",
     {
-        "BurninDestinationSettings": BurninDestinationSettingsTypeDef,
+        "BurninDestinationSettings": BurninDestinationSettingsOutputTypeDef,
         "DestinationType": CaptionDestinationTypeType,
-        "DvbSubDestinationSettings": DvbSubDestinationSettingsTypeDef,
-        "EmbeddedDestinationSettings": EmbeddedDestinationSettingsTypeDef,
-        "ImscDestinationSettings": ImscDestinationSettingsTypeDef,
-        "SccDestinationSettings": SccDestinationSettingsTypeDef,
-        "SrtDestinationSettings": SrtDestinationSettingsTypeDef,
+        "DvbSubDestinationSettings": DvbSubDestinationSettingsOutputTypeDef,
+        "EmbeddedDestinationSettings": EmbeddedDestinationSettingsOutputTypeDef,
+        "ImscDestinationSettings": ImscDestinationSettingsOutputTypeDef,
+        "SccDestinationSettings": SccDestinationSettingsOutputTypeDef,
+        "SrtDestinationSettings": SrtDestinationSettingsOutputTypeDef,
         "TeletextDestinationSettings": TeletextDestinationSettingsOutputTypeDef,
-        "TtmlDestinationSettings": TtmlDestinationSettingsTypeDef,
-        "WebvttDestinationSettings": WebvttDestinationSettingsTypeDef,
+        "TtmlDestinationSettings": TtmlDestinationSettingsOutputTypeDef,
+        "WebvttDestinationSettings": WebvttDestinationSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 CaptionDestinationSettingsTypeDef = TypedDict(
     "CaptionDestinationSettingsTypeDef",
     {
         "BurninDestinationSettings": BurninDestinationSettingsTypeDef,
         "DestinationType": CaptionDestinationTypeType,
@@ -2454,14 +3644,26 @@
         "TeletextDestinationSettings": TeletextDestinationSettingsTypeDef,
         "TtmlDestinationSettings": TtmlDestinationSettingsTypeDef,
         "WebvttDestinationSettings": WebvttDestinationSettingsTypeDef,
     },
     total=False,
 )
 
+FileSourceSettingsOutputTypeDef = TypedDict(
+    "FileSourceSettingsOutputTypeDef",
+    {
+        "Convert608To708": FileSourceConvert608To708Type,
+        "ConvertPaintToPop": CaptionSourceConvertPaintOnToPopOnType,
+        "Framerate": CaptionSourceFramerateOutputTypeDef,
+        "SourceFile": str,
+        "TimeDelta": int,
+        "TimeDeltaUnits": FileSourceTimeDeltaUnitsType,
+    },
+)
+
 FileSourceSettingsTypeDef = TypedDict(
     "FileSourceSettingsTypeDef",
     {
         "Convert608To708": FileSourceConvert608To708Type,
         "ConvertPaintToPop": CaptionSourceConvertPaintOnToPopOnType,
         "Framerate": CaptionSourceFramerateTypeDef,
         "SourceFile": str,
@@ -2472,15 +3674,14 @@
 )
 
 ChannelMappingOutputTypeDef = TypedDict(
     "ChannelMappingOutputTypeDef",
     {
         "OutputChannels": List[OutputChannelMappingOutputTypeDef],
     },
-    total=False,
 )
 
 ChannelMappingTypeDef = TypedDict(
     "ChannelMappingTypeDef",
     {
         "OutputChannels": Sequence[OutputChannelMappingTypeDef],
     },
@@ -2490,18 +3691,17 @@
 CmafEncryptionSettingsOutputTypeDef = TypedDict(
     "CmafEncryptionSettingsOutputTypeDef",
     {
         "ConstantInitializationVector": str,
         "EncryptionMethod": CmafEncryptionTypeType,
         "InitializationVectorInManifest": CmafInitializationVectorInManifestType,
         "SpekeKeyProvider": SpekeKeyProviderCmafOutputTypeDef,
-        "StaticKeyProvider": StaticKeyProviderTypeDef,
+        "StaticKeyProvider": StaticKeyProviderOutputTypeDef,
         "Type": CmafKeyProviderTypeType,
     },
-    total=False,
 )
 
 CmafEncryptionSettingsTypeDef = TypedDict(
     "CmafEncryptionSettingsTypeDef",
     {
         "ConstantInitializationVector": str,
         "EncryptionMethod": CmafEncryptionTypeType,
@@ -2509,14 +3709,46 @@
         "SpekeKeyProvider": SpekeKeyProviderCmafTypeDef,
         "StaticKeyProvider": StaticKeyProviderTypeDef,
         "Type": CmafKeyProviderTypeType,
     },
     total=False,
 )
 
+ColorCorrectorOutputTypeDef = TypedDict(
+    "ColorCorrectorOutputTypeDef",
+    {
+        "Brightness": int,
+        "ClipLimits": ClipLimitsOutputTypeDef,
+        "ColorSpaceConversion": ColorSpaceConversionType,
+        "Contrast": int,
+        "Hdr10Metadata": Hdr10MetadataOutputTypeDef,
+        "HdrToSdrToneMapper": HDRToSDRToneMapperType,
+        "Hue": int,
+        "SampleRangeConversion": SampleRangeConversionType,
+        "Saturation": int,
+        "SdrReferenceWhiteLevel": int,
+    },
+)
+
+VideoSelectorOutputTypeDef = TypedDict(
+    "VideoSelectorOutputTypeDef",
+    {
+        "AlphaBehavior": AlphaBehaviorType,
+        "ColorSpace": ColorSpaceType,
+        "ColorSpaceUsage": ColorSpaceUsageType,
+        "EmbeddedTimecodeOverride": EmbeddedTimecodeOverrideType,
+        "Hdr10Metadata": Hdr10MetadataOutputTypeDef,
+        "PadVideo": PadVideoType,
+        "Pid": int,
+        "ProgramNumber": int,
+        "Rotate": InputRotateType,
+        "SampleRange": InputSampleRangeType,
+    },
+)
+
 ColorCorrectorTypeDef = TypedDict(
     "ColorCorrectorTypeDef",
     {
         "Brightness": int,
         "ClipLimits": ClipLimitsTypeDef,
         "ColorSpaceConversion": ColorSpaceConversionType,
         "Contrast": int,
@@ -2593,37 +3825,34 @@
 
 DashIsoEncryptionSettingsOutputTypeDef = TypedDict(
     "DashIsoEncryptionSettingsOutputTypeDef",
     {
         "PlaybackDeviceCompatibility": DashIsoPlaybackDeviceCompatibilityType,
         "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
     },
-    total=False,
 )
 
 HlsEncryptionSettingsOutputTypeDef = TypedDict(
     "HlsEncryptionSettingsOutputTypeDef",
     {
         "ConstantInitializationVector": str,
         "EncryptionMethod": HlsEncryptionTypeType,
         "InitializationVectorInManifest": HlsInitializationVectorInManifestType,
         "OfflineEncrypted": HlsOfflineEncryptedType,
         "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
-        "StaticKeyProvider": StaticKeyProviderTypeDef,
+        "StaticKeyProvider": StaticKeyProviderOutputTypeDef,
         "Type": HlsKeyProviderTypeType,
     },
-    total=False,
 )
 
 MsSmoothEncryptionSettingsOutputTypeDef = TypedDict(
     "MsSmoothEncryptionSettingsOutputTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
     },
-    total=False,
 )
 
 DashIsoEncryptionSettingsTypeDef = TypedDict(
     "DashIsoEncryptionSettingsTypeDef",
     {
         "PlaybackDeviceCompatibility": DashIsoPlaybackDeviceCompatibilityType,
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
@@ -2710,55 +3939,117 @@
     {
         "Endpoints": List[EndpointTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DolbyVisionOutputTypeDef = TypedDict(
+    "DolbyVisionOutputTypeDef",
+    {
+        "L6Metadata": DolbyVisionLevel6MetadataOutputTypeDef,
+        "L6Mode": DolbyVisionLevel6ModeType,
+        "Mapping": DolbyVisionMappingType,
+        "Profile": DolbyVisionProfileType,
+    },
+)
+
 DolbyVisionTypeDef = TypedDict(
     "DolbyVisionTypeDef",
     {
         "L6Metadata": DolbyVisionLevel6MetadataTypeDef,
         "L6Mode": DolbyVisionLevel6ModeType,
         "Mapping": DolbyVisionMappingType,
         "Profile": DolbyVisionProfileType,
     },
     total=False,
 )
 
+EsamSettingsOutputTypeDef = TypedDict(
+    "EsamSettingsOutputTypeDef",
+    {
+        "ManifestConfirmConditionNotification": (
+            EsamManifestConfirmConditionNotificationOutputTypeDef
+        ),
+        "ResponseSignalPreroll": int,
+        "SignalProcessingNotification": EsamSignalProcessingNotificationOutputTypeDef,
+    },
+)
+
 EsamSettingsTypeDef = TypedDict(
     "EsamSettingsTypeDef",
     {
         "ManifestConfirmConditionNotification": EsamManifestConfirmConditionNotificationTypeDef,
         "ResponseSignalPreroll": int,
         "SignalProcessingNotification": EsamSignalProcessingNotificationTypeDef,
     },
     total=False,
 )
 
 GetPolicyResponseTypeDef = TypedDict(
     "GetPolicyResponseTypeDef",
     {
-        "Policy": PolicyTypeDef,
+        "Policy": PolicyOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutPolicyRequestRequestTypeDef = TypedDict(
-    "PutPolicyRequestRequestTypeDef",
+PutPolicyResponseTypeDef = TypedDict(
+    "PutPolicyResponseTypeDef",
     {
-        "Policy": PolicyTypeDef,
+        "Policy": PolicyOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutPolicyResponseTypeDef = TypedDict(
-    "PutPolicyResponseTypeDef",
+H264SettingsOutputTypeDef = TypedDict(
+    "H264SettingsOutputTypeDef",
     {
-        "Policy": PolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AdaptiveQuantization": H264AdaptiveQuantizationType,
+        "BandwidthReductionFilter": BandwidthReductionFilterOutputTypeDef,
+        "Bitrate": int,
+        "CodecLevel": H264CodecLevelType,
+        "CodecProfile": H264CodecProfileType,
+        "DynamicSubGop": H264DynamicSubGopType,
+        "EntropyEncoding": H264EntropyEncodingType,
+        "FieldEncoding": H264FieldEncodingType,
+        "FlickerAdaptiveQuantization": H264FlickerAdaptiveQuantizationType,
+        "FramerateControl": H264FramerateControlType,
+        "FramerateConversionAlgorithm": H264FramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "GopBReference": H264GopBReferenceType,
+        "GopClosedCadence": int,
+        "GopSize": float,
+        "GopSizeUnits": H264GopSizeUnitsType,
+        "HrdBufferFinalFillPercentage": int,
+        "HrdBufferInitialFillPercentage": int,
+        "HrdBufferSize": int,
+        "InterlaceMode": H264InterlaceModeType,
+        "MaxBitrate": int,
+        "MinIInterval": int,
+        "NumberBFramesBetweenReferenceFrames": int,
+        "NumberReferenceFrames": int,
+        "ParControl": H264ParControlType,
+        "ParDenominator": int,
+        "ParNumerator": int,
+        "QualityTuningLevel": H264QualityTuningLevelType,
+        "QvbrSettings": H264QvbrSettingsOutputTypeDef,
+        "RateControlMode": H264RateControlModeType,
+        "RepeatPps": H264RepeatPpsType,
+        "ScanTypeConversionMode": H264ScanTypeConversionModeType,
+        "SceneChangeDetect": H264SceneChangeDetectType,
+        "Slices": int,
+        "SlowPal": H264SlowPalType,
+        "Softness": int,
+        "SpatialAdaptiveQuantization": H264SpatialAdaptiveQuantizationType,
+        "Syntax": H264SyntaxType,
+        "Telecine": H264TelecineType,
+        "TemporalAdaptiveQuantization": H264TemporalAdaptiveQuantizationType,
+        "UnregisteredSeiTimecode": H264UnregisteredSeiTimecodeType,
     },
 )
 
 H264SettingsTypeDef = TypedDict(
     "H264SettingsTypeDef",
     {
         "AdaptiveQuantization": H264AdaptiveQuantizationType,
@@ -2803,14 +4094,62 @@
         "Telecine": H264TelecineType,
         "TemporalAdaptiveQuantization": H264TemporalAdaptiveQuantizationType,
         "UnregisteredSeiTimecode": H264UnregisteredSeiTimecodeType,
     },
     total=False,
 )
 
+H265SettingsOutputTypeDef = TypedDict(
+    "H265SettingsOutputTypeDef",
+    {
+        "AdaptiveQuantization": H265AdaptiveQuantizationType,
+        "AlternateTransferFunctionSei": H265AlternateTransferFunctionSeiType,
+        "BandwidthReductionFilter": BandwidthReductionFilterOutputTypeDef,
+        "Bitrate": int,
+        "CodecLevel": H265CodecLevelType,
+        "CodecProfile": H265CodecProfileType,
+        "DynamicSubGop": H265DynamicSubGopType,
+        "FlickerAdaptiveQuantization": H265FlickerAdaptiveQuantizationType,
+        "FramerateControl": H265FramerateControlType,
+        "FramerateConversionAlgorithm": H265FramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "GopBReference": H265GopBReferenceType,
+        "GopClosedCadence": int,
+        "GopSize": float,
+        "GopSizeUnits": H265GopSizeUnitsType,
+        "HrdBufferFinalFillPercentage": int,
+        "HrdBufferInitialFillPercentage": int,
+        "HrdBufferSize": int,
+        "InterlaceMode": H265InterlaceModeType,
+        "MaxBitrate": int,
+        "MinIInterval": int,
+        "NumberBFramesBetweenReferenceFrames": int,
+        "NumberReferenceFrames": int,
+        "ParControl": H265ParControlType,
+        "ParDenominator": int,
+        "ParNumerator": int,
+        "QualityTuningLevel": H265QualityTuningLevelType,
+        "QvbrSettings": H265QvbrSettingsOutputTypeDef,
+        "RateControlMode": H265RateControlModeType,
+        "SampleAdaptiveOffsetFilterMode": H265SampleAdaptiveOffsetFilterModeType,
+        "ScanTypeConversionMode": H265ScanTypeConversionModeType,
+        "SceneChangeDetect": H265SceneChangeDetectType,
+        "Slices": int,
+        "SlowPal": H265SlowPalType,
+        "SpatialAdaptiveQuantization": H265SpatialAdaptiveQuantizationType,
+        "Telecine": H265TelecineType,
+        "TemporalAdaptiveQuantization": H265TemporalAdaptiveQuantizationType,
+        "TemporalIds": H265TemporalIdsType,
+        "Tiles": H265TilesType,
+        "UnregisteredSeiTimecode": H265UnregisteredSeiTimecodeType,
+        "WriteMp4PackagingType": H265WriteMp4PackagingTypeType,
+    },
+)
+
 H265SettingsTypeDef = TypedDict(
     "H265SettingsTypeDef",
     {
         "AdaptiveQuantization": H265AdaptiveQuantizationType,
         "AlternateTransferFunctionSei": H265AlternateTransferFunctionSeiType,
         "BandwidthReductionFilter": BandwidthReductionFilterTypeDef,
         "Bitrate": int,
@@ -2852,45 +4191,42 @@
         "Tiles": H265TilesType,
         "UnregisteredSeiTimecode": H265UnregisteredSeiTimecodeType,
         "WriteMp4PackagingType": H265WriteMp4PackagingTypeType,
     },
     total=False,
 )
 
-OutputSettingsTypeDef = TypedDict(
-    "OutputSettingsTypeDef",
+OutputSettingsOutputTypeDef = TypedDict(
+    "OutputSettingsOutputTypeDef",
     {
-        "HlsSettings": HlsSettingsTypeDef,
+        "HlsSettings": HlsSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 TimedMetadataInsertionOutputTypeDef = TypedDict(
     "TimedMetadataInsertionOutputTypeDef",
     {
-        "Id3Insertions": List[Id3InsertionTypeDef],
+        "Id3Insertions": List[Id3InsertionOutputTypeDef],
     },
-    total=False,
 )
 
 TimedMetadataInsertionTypeDef = TypedDict(
     "TimedMetadataInsertionTypeDef",
     {
         "Id3Insertions": Sequence[Id3InsertionTypeDef],
     },
     total=False,
 )
 
 ImageInserterOutputTypeDef = TypedDict(
     "ImageInserterOutputTypeDef",
     {
-        "InsertableImages": List[InsertableImageTypeDef],
+        "InsertableImages": List[InsertableImageOutputTypeDef],
         "SdrReferenceWhiteLevel": int,
     },
-    total=False,
 )
 
 ImageInserterTypeDef = TypedDict(
     "ImageInserterTypeDef",
     {
         "InsertableImages": Sequence[InsertableImageTypeDef],
         "SdrReferenceWhiteLevel": int,
@@ -2912,18 +4248,18 @@
         "AudioBufferModel": M2tsAudioBufferModelType,
         "AudioDuration": M2tsAudioDurationType,
         "AudioFramesPerPes": int,
         "AudioPids": List[int],
         "Bitrate": int,
         "BufferModel": M2tsBufferModelType,
         "DataPTSControl": M2tsDataPtsControlType,
-        "DvbNitSettings": DvbNitSettingsTypeDef,
-        "DvbSdtSettings": DvbSdtSettingsTypeDef,
+        "DvbNitSettings": DvbNitSettingsOutputTypeDef,
+        "DvbSdtSettings": DvbSdtSettingsOutputTypeDef,
         "DvbSubPids": List[int],
-        "DvbTdtSettings": DvbTdtSettingsTypeDef,
+        "DvbTdtSettings": DvbTdtSettingsOutputTypeDef,
         "DvbTeletextPid": int,
         "EbpAudioInterval": M2tsEbpAudioIntervalType,
         "EbpPlacement": M2tsEbpPlacementType,
         "EsRateInPes": M2tsEsRateInPesType,
         "ForceTsVideoEbpOrder": M2tsForceTsVideoEbpOrderType,
         "FragmentTime": float,
         "KlvMetadata": M2tsKlvMetadataType,
@@ -2935,25 +4271,24 @@
         "PcrControl": M2tsPcrControlType,
         "PcrPid": int,
         "PmtInterval": int,
         "PmtPid": int,
         "PrivateMetadataPid": int,
         "ProgramNumber": int,
         "RateMode": M2tsRateModeType,
-        "Scte35Esam": M2tsScte35EsamTypeDef,
+        "Scte35Esam": M2tsScte35EsamOutputTypeDef,
         "Scte35Pid": int,
         "Scte35Source": M2tsScte35SourceType,
         "SegmentationMarkers": M2tsSegmentationMarkersType,
         "SegmentationStyle": M2tsSegmentationStyleType,
         "SegmentationTime": float,
         "TimedMetadataPid": int,
         "TransportStreamId": int,
         "VideoPid": int,
     },
-    total=False,
 )
 
 M2tsSettingsTypeDef = TypedDict(
     "M2tsSettingsTypeDef",
     {
         "AudioBufferModel": M2tsAudioBufferModelType,
         "AudioDuration": M2tsAudioDurationType,
@@ -2994,45 +4329,83 @@
         "TimedMetadataPid": int,
         "TransportStreamId": int,
         "VideoPid": int,
     },
     total=False,
 )
 
+MotionImageInserterOutputTypeDef = TypedDict(
+    "MotionImageInserterOutputTypeDef",
+    {
+        "Framerate": MotionImageInsertionFramerateOutputTypeDef,
+        "Input": str,
+        "InsertionMode": MotionImageInsertionModeType,
+        "Offset": MotionImageInsertionOffsetOutputTypeDef,
+        "Playback": MotionImagePlaybackType,
+        "StartTime": str,
+    },
+)
+
 MotionImageInserterTypeDef = TypedDict(
     "MotionImageInserterTypeDef",
     {
         "Framerate": MotionImageInsertionFramerateTypeDef,
         "Input": str,
         "InsertionMode": MotionImageInsertionModeType,
         "Offset": MotionImageInsertionOffsetTypeDef,
         "Playback": MotionImagePlaybackType,
         "StartTime": str,
     },
     total=False,
 )
 
+MxfSettingsOutputTypeDef = TypedDict(
+    "MxfSettingsOutputTypeDef",
+    {
+        "AfdSignaling": MxfAfdSignalingType,
+        "Profile": MxfProfileType,
+        "XavcProfileSettings": MxfXavcProfileSettingsOutputTypeDef,
+    },
+)
+
 MxfSettingsTypeDef = TypedDict(
     "MxfSettingsTypeDef",
     {
         "AfdSignaling": MxfAfdSignalingType,
         "Profile": MxfProfileType,
         "XavcProfileSettings": MxfXavcProfileSettingsTypeDef,
     },
     total=False,
 )
 
+PartnerWatermarkingOutputTypeDef = TypedDict(
+    "PartnerWatermarkingOutputTypeDef",
+    {
+        "NexguardFileMarkerSettings": NexGuardFileMarkerSettingsOutputTypeDef,
+    },
+)
+
 PartnerWatermarkingTypeDef = TypedDict(
     "PartnerWatermarkingTypeDef",
     {
         "NexguardFileMarkerSettings": NexGuardFileMarkerSettingsTypeDef,
     },
     total=False,
 )
 
+NoiseReducerOutputTypeDef = TypedDict(
+    "NoiseReducerOutputTypeDef",
+    {
+        "Filter": NoiseReducerFilterType,
+        "FilterSettings": NoiseReducerFilterSettingsOutputTypeDef,
+        "SpatialFilterSettings": NoiseReducerSpatialFilterSettingsOutputTypeDef,
+        "TemporalFilterSettings": NoiseReducerTemporalFilterSettingsOutputTypeDef,
+    },
+)
+
 NoiseReducerTypeDef = TypedDict(
     "NoiseReducerTypeDef",
     {
         "Filter": NoiseReducerFilterType,
         "FilterSettings": NoiseReducerFilterSettingsTypeDef,
         "SpatialFilterSettings": NoiseReducerSpatialFilterSettingsTypeDef,
         "TemporalFilterSettings": NoiseReducerTemporalFilterSettingsTypeDef,
@@ -3042,52 +4415,79 @@
 
 OutputDetailTypeDef = TypedDict(
     "OutputDetailTypeDef",
     {
         "DurationInMs": int,
         "VideoDetails": VideoDetailTypeDef,
     },
-    total=False,
 )
 
-_RequiredQueueTypeDef = TypedDict(
-    "_RequiredQueueTypeDef",
+PutPolicyRequestRequestTypeDef = TypedDict(
+    "PutPolicyRequestRequestTypeDef",
     {
-        "Name": str,
+        "Policy": PolicyTypeDef,
     },
 )
-_OptionalQueueTypeDef = TypedDict(
-    "_OptionalQueueTypeDef",
+
+QueueTypeDef = TypedDict(
+    "QueueTypeDef",
     {
         "Arn": str,
         "CreatedAt": datetime,
         "Description": str,
         "LastUpdated": datetime,
+        "Name": str,
         "PricingPlan": PricingPlanType,
         "ProgressingJobsCount": int,
         "ReservationPlan": ReservationPlanTypeDef,
         "Status": QueueStatusType,
         "SubmittedJobsCount": int,
         "Type": TypeType,
     },
-    total=False,
 )
 
-class QueueTypeDef(_RequiredQueueTypeDef, _OptionalQueueTypeDef):
-    pass
+S3DestinationSettingsOutputTypeDef = TypedDict(
+    "S3DestinationSettingsOutputTypeDef",
+    {
+        "AccessControl": S3DestinationAccessControlOutputTypeDef,
+        "Encryption": S3EncryptionSettingsOutputTypeDef,
+    },
+)
 
 S3DestinationSettingsTypeDef = TypedDict(
     "S3DestinationSettingsTypeDef",
     {
         "AccessControl": S3DestinationAccessControlTypeDef,
         "Encryption": S3EncryptionSettingsTypeDef,
     },
     total=False,
 )
 
+XavcSettingsOutputTypeDef = TypedDict(
+    "XavcSettingsOutputTypeDef",
+    {
+        "AdaptiveQuantization": XavcAdaptiveQuantizationType,
+        "EntropyEncoding": XavcEntropyEncodingType,
+        "FramerateControl": XavcFramerateControlType,
+        "FramerateConversionAlgorithm": XavcFramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "Profile": XavcProfileType,
+        "SlowPal": XavcSlowPalType,
+        "Softness": int,
+        "SpatialAdaptiveQuantization": XavcSpatialAdaptiveQuantizationType,
+        "TemporalAdaptiveQuantization": XavcTemporalAdaptiveQuantizationType,
+        "Xavc4kIntraCbgProfileSettings": Xavc4kIntraCbgProfileSettingsOutputTypeDef,
+        "Xavc4kIntraVbrProfileSettings": Xavc4kIntraVbrProfileSettingsOutputTypeDef,
+        "Xavc4kProfileSettings": Xavc4kProfileSettingsOutputTypeDef,
+        "XavcHdIntraCbgProfileSettings": XavcHdIntraCbgProfileSettingsOutputTypeDef,
+        "XavcHdProfileSettings": XavcHdProfileSettingsOutputTypeDef,
+    },
+)
+
 XavcSettingsTypeDef = TypedDict(
     "XavcSettingsTypeDef",
     {
         "AdaptiveQuantization": XavcAdaptiveQuantizationType,
         "EntropyEncoding": XavcEntropyEncodingType,
         "FramerateControl": XavcFramerateControlType,
         "FramerateConversionAlgorithm": XavcFramerateConversionAlgorithmType,
@@ -3111,60 +4511,71 @@
     "AutomatedAbrSettingsOutputTypeDef",
     {
         "MaxAbrBitrate": int,
         "MaxRenditions": int,
         "MinAbrBitrate": int,
         "Rules": List[AutomatedAbrRuleOutputTypeDef],
     },
-    total=False,
 )
 
 AutomatedAbrSettingsTypeDef = TypedDict(
     "AutomatedAbrSettingsTypeDef",
     {
         "MaxAbrBitrate": int,
         "MaxRenditions": int,
         "MinAbrBitrate": int,
         "Rules": Sequence[AutomatedAbrRuleTypeDef],
     },
     total=False,
 )
 
+CaptionDescriptionOutputTypeDef = TypedDict(
+    "CaptionDescriptionOutputTypeDef",
+    {
+        "CaptionSelectorName": str,
+        "CustomLanguageCode": str,
+        "DestinationSettings": CaptionDestinationSettingsOutputTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "LanguageDescription": str,
+    },
+)
+
 CaptionDescriptionPresetOutputTypeDef = TypedDict(
     "CaptionDescriptionPresetOutputTypeDef",
     {
         "CustomLanguageCode": str,
         "DestinationSettings": CaptionDestinationSettingsOutputTypeDef,
         "LanguageCode": LanguageCodeType,
         "LanguageDescription": str,
     },
-    total=False,
 )
 
 CaptionDescriptionPresetTypeDef = TypedDict(
     "CaptionDescriptionPresetTypeDef",
     {
         "CustomLanguageCode": str,
         "DestinationSettings": CaptionDestinationSettingsTypeDef,
         "LanguageCode": LanguageCodeType,
         "LanguageDescription": str,
     },
     total=False,
 )
 
-CaptionDescriptionTypeDef = TypedDict(
-    "CaptionDescriptionTypeDef",
+CaptionSourceSettingsOutputTypeDef = TypedDict(
+    "CaptionSourceSettingsOutputTypeDef",
     {
-        "CaptionSelectorName": str,
-        "CustomLanguageCode": str,
-        "DestinationSettings": CaptionDestinationSettingsTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "LanguageDescription": str,
+        "AncillarySourceSettings": AncillarySourceSettingsOutputTypeDef,
+        "DvbSubSourceSettings": DvbSubSourceSettingsOutputTypeDef,
+        "EmbeddedSourceSettings": EmbeddedSourceSettingsOutputTypeDef,
+        "FileSourceSettings": FileSourceSettingsOutputTypeDef,
+        "SourceType": CaptionSourceTypeType,
+        "TeletextSourceSettings": TeletextSourceSettingsOutputTypeDef,
+        "TrackSourceSettings": TrackSourceSettingsOutputTypeDef,
+        "WebvttHlsSourceSettings": WebvttHlsSourceSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 CaptionSourceSettingsTypeDef = TypedDict(
     "CaptionSourceSettingsTypeDef",
     {
         "AncillarySourceSettings": AncillarySourceSettingsTypeDef,
         "DvbSubSourceSettings": DvbSubSourceSettingsTypeDef,
@@ -3181,15 +4592,14 @@
 RemixSettingsOutputTypeDef = TypedDict(
     "RemixSettingsOutputTypeDef",
     {
         "ChannelMapping": ChannelMappingOutputTypeDef,
         "ChannelsIn": int,
         "ChannelsOut": int,
     },
-    total=False,
 )
 
 RemixSettingsTypeDef = TypedDict(
     "RemixSettingsTypeDef",
     {
         "ChannelMapping": ChannelMappingTypeDef,
         "ChannelsIn": int,
@@ -3197,25 +4607,24 @@
     },
     total=False,
 )
 
 ContainerSettingsOutputTypeDef = TypedDict(
     "ContainerSettingsOutputTypeDef",
     {
-        "CmfcSettings": CmfcSettingsTypeDef,
+        "CmfcSettings": CmfcSettingsOutputTypeDef,
         "Container": ContainerTypeType,
-        "F4vSettings": F4vSettingsTypeDef,
+        "F4vSettings": F4vSettingsOutputTypeDef,
         "M2tsSettings": M2tsSettingsOutputTypeDef,
         "M3u8Settings": M3u8SettingsOutputTypeDef,
-        "MovSettings": MovSettingsTypeDef,
-        "Mp4Settings": Mp4SettingsTypeDef,
-        "MpdSettings": MpdSettingsTypeDef,
-        "MxfSettings": MxfSettingsTypeDef,
+        "MovSettings": MovSettingsOutputTypeDef,
+        "Mp4Settings": Mp4SettingsOutputTypeDef,
+        "MpdSettings": MpdSettingsOutputTypeDef,
+        "MxfSettings": MxfSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 ContainerSettingsTypeDef = TypedDict(
     "ContainerSettingsTypeDef",
     {
         "CmfcSettings": CmfcSettingsTypeDef,
         "Container": ContainerTypeType,
@@ -3229,24 +4638,23 @@
     },
     total=False,
 )
 
 VideoPreprocessorOutputTypeDef = TypedDict(
     "VideoPreprocessorOutputTypeDef",
     {
-        "ColorCorrector": ColorCorrectorTypeDef,
-        "Deinterlacer": DeinterlacerTypeDef,
-        "DolbyVision": DolbyVisionTypeDef,
-        "Hdr10Plus": Hdr10PlusTypeDef,
+        "ColorCorrector": ColorCorrectorOutputTypeDef,
+        "Deinterlacer": DeinterlacerOutputTypeDef,
+        "DolbyVision": DolbyVisionOutputTypeDef,
+        "Hdr10Plus": Hdr10PlusOutputTypeDef,
         "ImageInserter": ImageInserterOutputTypeDef,
-        "NoiseReducer": NoiseReducerTypeDef,
-        "PartnerWatermarking": PartnerWatermarkingTypeDef,
-        "TimecodeBurnin": TimecodeBurninTypeDef,
+        "NoiseReducer": NoiseReducerOutputTypeDef,
+        "PartnerWatermarking": PartnerWatermarkingOutputTypeDef,
+        "TimecodeBurnin": TimecodeBurninOutputTypeDef,
     },
-    total=False,
 )
 
 VideoPreprocessorTypeDef = TypedDict(
     "VideoPreprocessorTypeDef",
     {
         "ColorCorrector": ColorCorrectorTypeDef,
         "Deinterlacer": DeinterlacerTypeDef,
@@ -3261,15 +4669,14 @@
 )
 
 OutputGroupDetailTypeDef = TypedDict(
     "OutputGroupDetailTypeDef",
     {
         "OutputDetails": List[OutputDetailTypeDef],
     },
-    total=False,
 )
 
 CreateQueueResponseTypeDef = TypedDict(
     "CreateQueueResponseTypeDef",
     {
         "Queue": QueueTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3297,22 +4704,47 @@
     "UpdateQueueResponseTypeDef",
     {
         "Queue": QueueTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DestinationSettingsOutputTypeDef = TypedDict(
+    "DestinationSettingsOutputTypeDef",
+    {
+        "S3Settings": S3DestinationSettingsOutputTypeDef,
+    },
+)
+
 DestinationSettingsTypeDef = TypedDict(
     "DestinationSettingsTypeDef",
     {
         "S3Settings": S3DestinationSettingsTypeDef,
     },
     total=False,
 )
 
+VideoCodecSettingsOutputTypeDef = TypedDict(
+    "VideoCodecSettingsOutputTypeDef",
+    {
+        "Av1Settings": Av1SettingsOutputTypeDef,
+        "AvcIntraSettings": AvcIntraSettingsOutputTypeDef,
+        "Codec": VideoCodecType,
+        "FrameCaptureSettings": FrameCaptureSettingsOutputTypeDef,
+        "H264Settings": H264SettingsOutputTypeDef,
+        "H265Settings": H265SettingsOutputTypeDef,
+        "Mpeg2Settings": Mpeg2SettingsOutputTypeDef,
+        "ProresSettings": ProresSettingsOutputTypeDef,
+        "Vc3Settings": Vc3SettingsOutputTypeDef,
+        "Vp8Settings": Vp8SettingsOutputTypeDef,
+        "Vp9Settings": Vp9SettingsOutputTypeDef,
+        "XavcSettings": XavcSettingsOutputTypeDef,
+    },
+)
+
 VideoCodecSettingsTypeDef = TypedDict(
     "VideoCodecSettingsTypeDef",
     {
         "Av1Settings": Av1SettingsTypeDef,
         "AvcIntraSettings": AvcIntraSettingsTypeDef,
         "Codec": VideoCodecType,
         "FrameCaptureSettings": FrameCaptureSettingsTypeDef,
@@ -3329,70 +4761,76 @@
 )
 
 AutomatedEncodingSettingsOutputTypeDef = TypedDict(
     "AutomatedEncodingSettingsOutputTypeDef",
     {
         "AbrSettings": AutomatedAbrSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 AutomatedEncodingSettingsTypeDef = TypedDict(
     "AutomatedEncodingSettingsTypeDef",
     {
         "AbrSettings": AutomatedAbrSettingsTypeDef,
     },
     total=False,
 )
 
+CaptionSelectorOutputTypeDef = TypedDict(
+    "CaptionSelectorOutputTypeDef",
+    {
+        "CustomLanguageCode": str,
+        "LanguageCode": LanguageCodeType,
+        "SourceSettings": CaptionSourceSettingsOutputTypeDef,
+    },
+)
+
 CaptionSelectorTypeDef = TypedDict(
     "CaptionSelectorTypeDef",
     {
         "CustomLanguageCode": str,
         "LanguageCode": LanguageCodeType,
         "SourceSettings": CaptionSourceSettingsTypeDef,
     },
     total=False,
 )
 
 AudioDescriptionOutputTypeDef = TypedDict(
     "AudioDescriptionOutputTypeDef",
     {
-        "AudioChannelTaggingSettings": AudioChannelTaggingSettingsTypeDef,
-        "AudioNormalizationSettings": AudioNormalizationSettingsTypeDef,
+        "AudioChannelTaggingSettings": AudioChannelTaggingSettingsOutputTypeDef,
+        "AudioNormalizationSettings": AudioNormalizationSettingsOutputTypeDef,
         "AudioSourceName": str,
         "AudioType": int,
         "AudioTypeControl": AudioTypeControlType,
-        "CodecSettings": AudioCodecSettingsTypeDef,
+        "CodecSettings": AudioCodecSettingsOutputTypeDef,
         "CustomLanguageCode": str,
         "LanguageCode": LanguageCodeType,
         "LanguageCodeControl": AudioLanguageCodeControlType,
         "RemixSettings": RemixSettingsOutputTypeDef,
         "StreamName": str,
     },
-    total=False,
 )
 
 AudioSelectorOutputTypeDef = TypedDict(
     "AudioSelectorOutputTypeDef",
     {
         "AudioDurationCorrection": AudioDurationCorrectionType,
         "CustomLanguageCode": str,
         "DefaultSelection": AudioDefaultSelectionType,
         "ExternalAudioFileInput": str,
-        "HlsRenditionGroupSettings": HlsRenditionGroupSettingsTypeDef,
+        "HlsRenditionGroupSettings": HlsRenditionGroupSettingsOutputTypeDef,
         "LanguageCode": LanguageCodeType,
         "Offset": int,
         "Pids": List[int],
         "ProgramSelection": int,
         "RemixSettings": RemixSettingsOutputTypeDef,
         "SelectorType": AudioSelectorTypeType,
         "Tracks": List[int],
     },
-    total=False,
 )
 
 AudioDescriptionTypeDef = TypedDict(
     "AudioDescriptionTypeDef",
     {
         "AudioChannelTaggingSettings": AudioChannelTaggingSettingsTypeDef,
         "AudioNormalizationSettings": AudioNormalizationSettingsTypeDef,
@@ -3433,19 +4871,19 @@
     {
         "AdditionalManifests": List[CmafAdditionalManifestOutputTypeDef],
         "BaseUrl": str,
         "ClientCache": CmafClientCacheType,
         "CodecSpecification": CmafCodecSpecificationType,
         "DashManifestStyle": DashManifestStyleType,
         "Destination": str,
-        "DestinationSettings": DestinationSettingsTypeDef,
+        "DestinationSettings": DestinationSettingsOutputTypeDef,
         "Encryption": CmafEncryptionSettingsOutputTypeDef,
         "FragmentLength": int,
         "ImageBasedTrickPlay": CmafImageBasedTrickPlayType,
-        "ImageBasedTrickPlaySettings": CmafImageBasedTrickPlaySettingsTypeDef,
+        "ImageBasedTrickPlaySettings": CmafImageBasedTrickPlaySettingsOutputTypeDef,
         "ManifestCompression": CmafManifestCompressionType,
         "ManifestDurationFormat": CmafManifestDurationFormatType,
         "MinBufferTime": int,
         "MinFinalSegmentLength": float,
         "MpdManifestBandwidthType": CmafMpdManifestBandwidthTypeType,
         "MpdProfile": CmafMpdProfileType,
         "PtsOffsetHandlingForBFrames": CmafPtsOffsetHandlingForBFramesType,
@@ -3455,15 +4893,101 @@
         "StreamInfResolution": CmafStreamInfResolutionType,
         "TargetDurationCompatibilityMode": CmafTargetDurationCompatibilityModeType,
         "VideoCompositionOffsets": CmafVideoCompositionOffsetsType,
         "WriteDashManifest": CmafWriteDASHManifestType,
         "WriteHlsManifest": CmafWriteHLSManifestType,
         "WriteSegmentTimelineInRepresentation": CmafWriteSegmentTimelineInRepresentationType,
     },
-    total=False,
+)
+
+DashIsoGroupSettingsOutputTypeDef = TypedDict(
+    "DashIsoGroupSettingsOutputTypeDef",
+    {
+        "AdditionalManifests": List[DashAdditionalManifestOutputTypeDef],
+        "AudioChannelConfigSchemeIdUri": DashIsoGroupAudioChannelConfigSchemeIdUriType,
+        "BaseUrl": str,
+        "DashManifestStyle": DashManifestStyleType,
+        "Destination": str,
+        "DestinationSettings": DestinationSettingsOutputTypeDef,
+        "Encryption": DashIsoEncryptionSettingsOutputTypeDef,
+        "FragmentLength": int,
+        "HbbtvCompliance": DashIsoHbbtvComplianceType,
+        "ImageBasedTrickPlay": DashIsoImageBasedTrickPlayType,
+        "ImageBasedTrickPlaySettings": DashIsoImageBasedTrickPlaySettingsOutputTypeDef,
+        "MinBufferTime": int,
+        "MinFinalSegmentLength": float,
+        "MpdManifestBandwidthType": DashIsoMpdManifestBandwidthTypeType,
+        "MpdProfile": DashIsoMpdProfileType,
+        "PtsOffsetHandlingForBFrames": DashIsoPtsOffsetHandlingForBFramesType,
+        "SegmentControl": DashIsoSegmentControlType,
+        "SegmentLength": int,
+        "SegmentLengthControl": DashIsoSegmentLengthControlType,
+        "VideoCompositionOffsets": DashIsoVideoCompositionOffsetsType,
+        "WriteSegmentTimelineInRepresentation": DashIsoWriteSegmentTimelineInRepresentationType,
+    },
+)
+
+FileGroupSettingsOutputTypeDef = TypedDict(
+    "FileGroupSettingsOutputTypeDef",
+    {
+        "Destination": str,
+        "DestinationSettings": DestinationSettingsOutputTypeDef,
+    },
+)
+
+HlsGroupSettingsOutputTypeDef = TypedDict(
+    "HlsGroupSettingsOutputTypeDef",
+    {
+        "AdMarkers": List[HlsAdMarkersType],
+        "AdditionalManifests": List[HlsAdditionalManifestOutputTypeDef],
+        "AudioOnlyHeader": HlsAudioOnlyHeaderType,
+        "BaseUrl": str,
+        "CaptionLanguageMappings": List[HlsCaptionLanguageMappingOutputTypeDef],
+        "CaptionLanguageSetting": HlsCaptionLanguageSettingType,
+        "CaptionSegmentLengthControl": HlsCaptionSegmentLengthControlType,
+        "ClientCache": HlsClientCacheType,
+        "CodecSpecification": HlsCodecSpecificationType,
+        "Destination": str,
+        "DestinationSettings": DestinationSettingsOutputTypeDef,
+        "DirectoryStructure": HlsDirectoryStructureType,
+        "Encryption": HlsEncryptionSettingsOutputTypeDef,
+        "ImageBasedTrickPlay": HlsImageBasedTrickPlayType,
+        "ImageBasedTrickPlaySettings": HlsImageBasedTrickPlaySettingsOutputTypeDef,
+        "ManifestCompression": HlsManifestCompressionType,
+        "ManifestDurationFormat": HlsManifestDurationFormatType,
+        "MinFinalSegmentLength": float,
+        "MinSegmentLength": int,
+        "OutputSelection": HlsOutputSelectionType,
+        "ProgramDateTime": HlsProgramDateTimeType,
+        "ProgramDateTimePeriod": int,
+        "ProgressiveWriteHlsManifest": HlsProgressiveWriteHlsManifestType,
+        "SegmentControl": HlsSegmentControlType,
+        "SegmentLength": int,
+        "SegmentLengthControl": HlsSegmentLengthControlType,
+        "SegmentsPerSubdirectory": int,
+        "StreamInfResolution": HlsStreamInfResolutionType,
+        "TargetDurationCompatibilityMode": HlsTargetDurationCompatibilityModeType,
+        "TimedMetadataId3Frame": HlsTimedMetadataId3FrameType,
+        "TimedMetadataId3Period": int,
+        "TimestampDeltaMilliseconds": int,
+    },
+)
+
+MsSmoothGroupSettingsOutputTypeDef = TypedDict(
+    "MsSmoothGroupSettingsOutputTypeDef",
+    {
+        "AdditionalManifests": List[MsSmoothAdditionalManifestOutputTypeDef],
+        "AudioDeduplication": MsSmoothAudioDeduplicationType,
+        "Destination": str,
+        "DestinationSettings": DestinationSettingsOutputTypeDef,
+        "Encryption": MsSmoothEncryptionSettingsOutputTypeDef,
+        "FragmentLength": int,
+        "FragmentLengthControl": MsSmoothFragmentLengthControlType,
+        "ManifestEncoding": MsSmoothManifestEncodingType,
+    },
 )
 
 CmafGroupSettingsTypeDef = TypedDict(
     "CmafGroupSettingsTypeDef",
     {
         "AdditionalManifests": Sequence[CmafAdditionalManifestTypeDef],
         "BaseUrl": str,
@@ -3492,42 +5016,14 @@
         "WriteDashManifest": CmafWriteDASHManifestType,
         "WriteHlsManifest": CmafWriteHLSManifestType,
         "WriteSegmentTimelineInRepresentation": CmafWriteSegmentTimelineInRepresentationType,
     },
     total=False,
 )
 
-DashIsoGroupSettingsOutputTypeDef = TypedDict(
-    "DashIsoGroupSettingsOutputTypeDef",
-    {
-        "AdditionalManifests": List[DashAdditionalManifestOutputTypeDef],
-        "AudioChannelConfigSchemeIdUri": DashIsoGroupAudioChannelConfigSchemeIdUriType,
-        "BaseUrl": str,
-        "DashManifestStyle": DashManifestStyleType,
-        "Destination": str,
-        "DestinationSettings": DestinationSettingsTypeDef,
-        "Encryption": DashIsoEncryptionSettingsOutputTypeDef,
-        "FragmentLength": int,
-        "HbbtvCompliance": DashIsoHbbtvComplianceType,
-        "ImageBasedTrickPlay": DashIsoImageBasedTrickPlayType,
-        "ImageBasedTrickPlaySettings": DashIsoImageBasedTrickPlaySettingsTypeDef,
-        "MinBufferTime": int,
-        "MinFinalSegmentLength": float,
-        "MpdManifestBandwidthType": DashIsoMpdManifestBandwidthTypeType,
-        "MpdProfile": DashIsoMpdProfileType,
-        "PtsOffsetHandlingForBFrames": DashIsoPtsOffsetHandlingForBFramesType,
-        "SegmentControl": DashIsoSegmentControlType,
-        "SegmentLength": int,
-        "SegmentLengthControl": DashIsoSegmentLengthControlType,
-        "VideoCompositionOffsets": DashIsoVideoCompositionOffsetsType,
-        "WriteSegmentTimelineInRepresentation": DashIsoWriteSegmentTimelineInRepresentationType,
-    },
-    total=False,
-)
-
 DashIsoGroupSettingsTypeDef = TypedDict(
     "DashIsoGroupSettingsTypeDef",
     {
         "AdditionalManifests": Sequence[DashAdditionalManifestTypeDef],
         "AudioChannelConfigSchemeIdUri": DashIsoGroupAudioChannelConfigSchemeIdUriType,
         "BaseUrl": str,
         "DashManifestStyle": DashManifestStyleType,
@@ -3557,53 +5053,14 @@
     {
         "Destination": str,
         "DestinationSettings": DestinationSettingsTypeDef,
     },
     total=False,
 )
 
-HlsGroupSettingsOutputTypeDef = TypedDict(
-    "HlsGroupSettingsOutputTypeDef",
-    {
-        "AdMarkers": List[HlsAdMarkersType],
-        "AdditionalManifests": List[HlsAdditionalManifestOutputTypeDef],
-        "AudioOnlyHeader": HlsAudioOnlyHeaderType,
-        "BaseUrl": str,
-        "CaptionLanguageMappings": List[HlsCaptionLanguageMappingTypeDef],
-        "CaptionLanguageSetting": HlsCaptionLanguageSettingType,
-        "CaptionSegmentLengthControl": HlsCaptionSegmentLengthControlType,
-        "ClientCache": HlsClientCacheType,
-        "CodecSpecification": HlsCodecSpecificationType,
-        "Destination": str,
-        "DestinationSettings": DestinationSettingsTypeDef,
-        "DirectoryStructure": HlsDirectoryStructureType,
-        "Encryption": HlsEncryptionSettingsOutputTypeDef,
-        "ImageBasedTrickPlay": HlsImageBasedTrickPlayType,
-        "ImageBasedTrickPlaySettings": HlsImageBasedTrickPlaySettingsTypeDef,
-        "ManifestCompression": HlsManifestCompressionType,
-        "ManifestDurationFormat": HlsManifestDurationFormatType,
-        "MinFinalSegmentLength": float,
-        "MinSegmentLength": int,
-        "OutputSelection": HlsOutputSelectionType,
-        "ProgramDateTime": HlsProgramDateTimeType,
-        "ProgramDateTimePeriod": int,
-        "ProgressiveWriteHlsManifest": HlsProgressiveWriteHlsManifestType,
-        "SegmentControl": HlsSegmentControlType,
-        "SegmentLength": int,
-        "SegmentLengthControl": HlsSegmentLengthControlType,
-        "SegmentsPerSubdirectory": int,
-        "StreamInfResolution": HlsStreamInfResolutionType,
-        "TargetDurationCompatibilityMode": HlsTargetDurationCompatibilityModeType,
-        "TimedMetadataId3Frame": HlsTimedMetadataId3FrameType,
-        "TimedMetadataId3Period": int,
-        "TimestampDeltaMilliseconds": int,
-    },
-    total=False,
-)
-
 HlsGroupSettingsTypeDef = TypedDict(
     "HlsGroupSettingsTypeDef",
     {
         "AdMarkers": Sequence[HlsAdMarkersType],
         "AdditionalManifests": Sequence[HlsAdditionalManifestTypeDef],
         "AudioOnlyHeader": HlsAudioOnlyHeaderType,
         "BaseUrl": str,
@@ -3635,29 +5092,14 @@
         "TimedMetadataId3Frame": HlsTimedMetadataId3FrameType,
         "TimedMetadataId3Period": int,
         "TimestampDeltaMilliseconds": int,
     },
     total=False,
 )
 
-MsSmoothGroupSettingsOutputTypeDef = TypedDict(
-    "MsSmoothGroupSettingsOutputTypeDef",
-    {
-        "AdditionalManifests": List[MsSmoothAdditionalManifestOutputTypeDef],
-        "AudioDeduplication": MsSmoothAudioDeduplicationType,
-        "Destination": str,
-        "DestinationSettings": DestinationSettingsTypeDef,
-        "Encryption": MsSmoothEncryptionSettingsOutputTypeDef,
-        "FragmentLength": int,
-        "FragmentLengthControl": MsSmoothFragmentLengthControlType,
-        "ManifestEncoding": MsSmoothManifestEncodingType,
-    },
-    total=False,
-)
-
 MsSmoothGroupSettingsTypeDef = TypedDict(
     "MsSmoothGroupSettingsTypeDef",
     {
         "AdditionalManifests": Sequence[MsSmoothAdditionalManifestTypeDef],
         "AudioDeduplication": MsSmoothAudioDeduplicationType,
         "Destination": str,
         "DestinationSettings": DestinationSettingsTypeDef,
@@ -3670,29 +5112,28 @@
 )
 
 VideoDescriptionOutputTypeDef = TypedDict(
     "VideoDescriptionOutputTypeDef",
     {
         "AfdSignaling": AfdSignalingType,
         "AntiAlias": AntiAliasType,
-        "CodecSettings": VideoCodecSettingsTypeDef,
+        "CodecSettings": VideoCodecSettingsOutputTypeDef,
         "ColorMetadata": ColorMetadataType,
-        "Crop": RectangleTypeDef,
+        "Crop": RectangleOutputTypeDef,
         "DropFrameTimecode": DropFrameTimecodeType,
         "FixedAfd": int,
         "Height": int,
-        "Position": RectangleTypeDef,
+        "Position": RectangleOutputTypeDef,
         "RespondToAfd": RespondToAfdType,
         "ScalingBehavior": ScalingBehaviorType,
         "Sharpness": int,
         "TimecodeInsertion": VideoTimecodeInsertionType,
         "VideoPreprocessors": VideoPreprocessorOutputTypeDef,
         "Width": int,
     },
-    total=False,
 )
 
 VideoDescriptionTypeDef = TypedDict(
     "VideoDescriptionTypeDef",
     {
         "AfdSignaling": AfdSignalingType,
         "AntiAlias": AntiAliasType,
@@ -3713,66 +5154,64 @@
     total=False,
 )
 
 InputOutputTypeDef = TypedDict(
     "InputOutputTypeDef",
     {
         "AdvancedInputFilter": AdvancedInputFilterType,
-        "AdvancedInputFilterSettings": AdvancedInputFilterSettingsTypeDef,
+        "AdvancedInputFilterSettings": AdvancedInputFilterSettingsOutputTypeDef,
         "AudioSelectorGroups": Dict[str, AudioSelectorGroupOutputTypeDef],
         "AudioSelectors": Dict[str, AudioSelectorOutputTypeDef],
-        "CaptionSelectors": Dict[str, CaptionSelectorTypeDef],
-        "Crop": RectangleTypeDef,
+        "CaptionSelectors": Dict[str, CaptionSelectorOutputTypeDef],
+        "Crop": RectangleOutputTypeDef,
         "DeblockFilter": InputDeblockFilterType,
-        "DecryptionSettings": InputDecryptionSettingsTypeDef,
+        "DecryptionSettings": InputDecryptionSettingsOutputTypeDef,
         "DenoiseFilter": InputDenoiseFilterType,
         "DolbyVisionMetadataXml": str,
         "FileInput": str,
         "FilterEnable": InputFilterEnableType,
         "FilterStrength": int,
         "ImageInserter": ImageInserterOutputTypeDef,
-        "InputClippings": List[InputClippingTypeDef],
+        "InputClippings": List[InputClippingOutputTypeDef],
         "InputScanType": InputScanTypeType,
-        "Position": RectangleTypeDef,
+        "Position": RectangleOutputTypeDef,
         "ProgramNumber": int,
         "PsiControl": InputPsiControlType,
         "SupplementalImps": List[str],
         "TimecodeSource": InputTimecodeSourceType,
         "TimecodeStart": str,
-        "VideoGenerator": InputVideoGeneratorTypeDef,
-        "VideoSelector": VideoSelectorTypeDef,
+        "VideoGenerator": InputVideoGeneratorOutputTypeDef,
+        "VideoSelector": VideoSelectorOutputTypeDef,
     },
-    total=False,
 )
 
 InputTemplateOutputTypeDef = TypedDict(
     "InputTemplateOutputTypeDef",
     {
         "AdvancedInputFilter": AdvancedInputFilterType,
-        "AdvancedInputFilterSettings": AdvancedInputFilterSettingsTypeDef,
+        "AdvancedInputFilterSettings": AdvancedInputFilterSettingsOutputTypeDef,
         "AudioSelectorGroups": Dict[str, AudioSelectorGroupOutputTypeDef],
         "AudioSelectors": Dict[str, AudioSelectorOutputTypeDef],
-        "CaptionSelectors": Dict[str, CaptionSelectorTypeDef],
-        "Crop": RectangleTypeDef,
+        "CaptionSelectors": Dict[str, CaptionSelectorOutputTypeDef],
+        "Crop": RectangleOutputTypeDef,
         "DeblockFilter": InputDeblockFilterType,
         "DenoiseFilter": InputDenoiseFilterType,
         "DolbyVisionMetadataXml": str,
         "FilterEnable": InputFilterEnableType,
         "FilterStrength": int,
         "ImageInserter": ImageInserterOutputTypeDef,
-        "InputClippings": List[InputClippingTypeDef],
+        "InputClippings": List[InputClippingOutputTypeDef],
         "InputScanType": InputScanTypeType,
-        "Position": RectangleTypeDef,
+        "Position": RectangleOutputTypeDef,
         "ProgramNumber": int,
         "PsiControl": InputPsiControlType,
         "TimecodeSource": InputTimecodeSourceType,
         "TimecodeStart": str,
-        "VideoSelector": VideoSelectorTypeDef,
+        "VideoSelector": VideoSelectorOutputTypeDef,
     },
-    total=False,
 )
 
 InputTemplateTypeDef = TypedDict(
     "InputTemplateTypeDef",
     {
         "AdvancedInputFilter": AdvancedInputFilterType,
         "AdvancedInputFilterSettings": AdvancedInputFilterSettingsTypeDef,
@@ -3830,20 +5269,19 @@
 )
 
 OutputGroupSettingsOutputTypeDef = TypedDict(
     "OutputGroupSettingsOutputTypeDef",
     {
         "CmafGroupSettings": CmafGroupSettingsOutputTypeDef,
         "DashIsoGroupSettings": DashIsoGroupSettingsOutputTypeDef,
-        "FileGroupSettings": FileGroupSettingsTypeDef,
+        "FileGroupSettings": FileGroupSettingsOutputTypeDef,
         "HlsGroupSettings": HlsGroupSettingsOutputTypeDef,
         "MsSmoothGroupSettings": MsSmoothGroupSettingsOutputTypeDef,
         "Type": OutputGroupTypeType,
     },
-    total=False,
 )
 
 OutputGroupSettingsTypeDef = TypedDict(
     "OutputGroupSettingsTypeDef",
     {
         "CmafGroupSettings": CmafGroupSettingsTypeDef,
         "DashIsoGroupSettings": DashIsoGroupSettingsTypeDef,
@@ -3851,98 +5289,86 @@
         "HlsGroupSettings": HlsGroupSettingsTypeDef,
         "MsSmoothGroupSettings": MsSmoothGroupSettingsTypeDef,
         "Type": OutputGroupTypeType,
     },
     total=False,
 )
 
-PresetSettingsOutputTypeDef = TypedDict(
-    "PresetSettingsOutputTypeDef",
+OutputTypeDef = TypedDict(
+    "OutputTypeDef",
     {
         "AudioDescriptions": List[AudioDescriptionOutputTypeDef],
-        "CaptionDescriptions": List[CaptionDescriptionPresetOutputTypeDef],
+        "CaptionDescriptions": List[CaptionDescriptionOutputTypeDef],
         "ContainerSettings": ContainerSettingsOutputTypeDef,
+        "Extension": str,
+        "NameModifier": str,
+        "OutputSettings": OutputSettingsOutputTypeDef,
+        "Preset": str,
         "VideoDescription": VideoDescriptionOutputTypeDef,
     },
-    total=False,
 )
 
-OutputTypeDef = TypedDict(
-    "OutputTypeDef",
+PresetSettingsOutputTypeDef = TypedDict(
+    "PresetSettingsOutputTypeDef",
     {
-        "AudioDescriptions": Sequence[AudioDescriptionTypeDef],
-        "CaptionDescriptions": Sequence[CaptionDescriptionTypeDef],
-        "ContainerSettings": ContainerSettingsTypeDef,
-        "Extension": str,
-        "NameModifier": str,
-        "OutputSettings": OutputSettingsTypeDef,
-        "Preset": str,
-        "VideoDescription": VideoDescriptionTypeDef,
+        "AudioDescriptions": List[AudioDescriptionOutputTypeDef],
+        "CaptionDescriptions": List[CaptionDescriptionPresetOutputTypeDef],
+        "ContainerSettings": ContainerSettingsOutputTypeDef,
+        "VideoDescription": VideoDescriptionOutputTypeDef,
     },
-    total=False,
 )
 
 PresetSettingsTypeDef = TypedDict(
     "PresetSettingsTypeDef",
     {
         "AudioDescriptions": Sequence[AudioDescriptionTypeDef],
         "CaptionDescriptions": Sequence[CaptionDescriptionPresetTypeDef],
         "ContainerSettings": ContainerSettingsTypeDef,
         "VideoDescription": VideoDescriptionTypeDef,
     },
     total=False,
 )
 
-_RequiredPresetTypeDef = TypedDict(
-    "_RequiredPresetTypeDef",
-    {
-        "Name": str,
-        "Settings": PresetSettingsOutputTypeDef,
-    },
-)
-_OptionalPresetTypeDef = TypedDict(
-    "_OptionalPresetTypeDef",
-    {
-        "Arn": str,
-        "Category": str,
-        "CreatedAt": datetime,
-        "Description": str,
-        "LastUpdated": datetime,
-        "Type": TypeType,
-    },
-    total=False,
-)
-
-class PresetTypeDef(_RequiredPresetTypeDef, _OptionalPresetTypeDef):
-    pass
-
 OutputGroupOutputTypeDef = TypedDict(
     "OutputGroupOutputTypeDef",
     {
         "AutomatedEncodingSettings": AutomatedEncodingSettingsOutputTypeDef,
         "CustomName": str,
         "Name": str,
         "OutputGroupSettings": OutputGroupSettingsOutputTypeDef,
         "Outputs": List[OutputTypeDef],
     },
-    total=False,
 )
 
 OutputGroupTypeDef = TypedDict(
     "OutputGroupTypeDef",
     {
         "AutomatedEncodingSettings": AutomatedEncodingSettingsTypeDef,
         "CustomName": str,
         "Name": str,
         "OutputGroupSettings": OutputGroupSettingsTypeDef,
         "Outputs": Sequence[OutputTypeDef],
     },
     total=False,
 )
 
+PresetTypeDef = TypedDict(
+    "PresetTypeDef",
+    {
+        "Arn": str,
+        "Category": str,
+        "CreatedAt": datetime,
+        "Description": str,
+        "LastUpdated": datetime,
+        "Name": str,
+        "Settings": PresetSettingsOutputTypeDef,
+        "Type": TypeType,
+    },
+)
+
 _RequiredCreatePresetRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePresetRequestRequestTypeDef",
     {
         "Name": str,
         "Settings": PresetSettingsTypeDef,
     },
 )
@@ -3957,15 +5383,14 @@
 )
 
 class CreatePresetRequestRequestTypeDef(
     _RequiredCreatePresetRequestRequestTypeDef, _OptionalCreatePresetRequestRequestTypeDef
 ):
     pass
 
-PresetSettingsUnionTypeDef = Union[PresetSettingsTypeDef, PresetSettingsOutputTypeDef]
 _RequiredUpdatePresetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePresetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdatePresetRequestRequestTypeDef = TypedDict(
@@ -3979,83 +5404,48 @@
 )
 
 class UpdatePresetRequestRequestTypeDef(
     _RequiredUpdatePresetRequestRequestTypeDef, _OptionalUpdatePresetRequestRequestTypeDef
 ):
     pass
 
-CreatePresetResponseTypeDef = TypedDict(
-    "CreatePresetResponseTypeDef",
-    {
-        "Preset": PresetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPresetResponseTypeDef = TypedDict(
-    "GetPresetResponseTypeDef",
-    {
-        "Preset": PresetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListPresetsResponseTypeDef = TypedDict(
-    "ListPresetsResponseTypeDef",
-    {
-        "NextToken": str,
-        "Presets": List[PresetTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdatePresetResponseTypeDef = TypedDict(
-    "UpdatePresetResponseTypeDef",
-    {
-        "Preset": PresetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 JobSettingsOutputTypeDef = TypedDict(
     "JobSettingsOutputTypeDef",
     {
         "AdAvailOffset": int,
-        "AvailBlanking": AvailBlankingTypeDef,
-        "Esam": EsamSettingsTypeDef,
-        "ExtendedDataServices": ExtendedDataServicesTypeDef,
+        "AvailBlanking": AvailBlankingOutputTypeDef,
+        "Esam": EsamSettingsOutputTypeDef,
+        "ExtendedDataServices": ExtendedDataServicesOutputTypeDef,
         "Inputs": List[InputOutputTypeDef],
-        "KantarWatermark": KantarWatermarkSettingsTypeDef,
-        "MotionImageInserter": MotionImageInserterTypeDef,
-        "NielsenConfiguration": NielsenConfigurationTypeDef,
-        "NielsenNonLinearWatermark": NielsenNonLinearWatermarkSettingsTypeDef,
+        "KantarWatermark": KantarWatermarkSettingsOutputTypeDef,
+        "MotionImageInserter": MotionImageInserterOutputTypeDef,
+        "NielsenConfiguration": NielsenConfigurationOutputTypeDef,
+        "NielsenNonLinearWatermark": NielsenNonLinearWatermarkSettingsOutputTypeDef,
         "OutputGroups": List[OutputGroupOutputTypeDef],
-        "TimecodeConfig": TimecodeConfigTypeDef,
+        "TimecodeConfig": TimecodeConfigOutputTypeDef,
         "TimedMetadataInsertion": TimedMetadataInsertionOutputTypeDef,
     },
-    total=False,
 )
 
 JobTemplateSettingsOutputTypeDef = TypedDict(
     "JobTemplateSettingsOutputTypeDef",
     {
         "AdAvailOffset": int,
-        "AvailBlanking": AvailBlankingTypeDef,
-        "Esam": EsamSettingsTypeDef,
-        "ExtendedDataServices": ExtendedDataServicesTypeDef,
+        "AvailBlanking": AvailBlankingOutputTypeDef,
+        "Esam": EsamSettingsOutputTypeDef,
+        "ExtendedDataServices": ExtendedDataServicesOutputTypeDef,
         "Inputs": List[InputTemplateOutputTypeDef],
-        "KantarWatermark": KantarWatermarkSettingsTypeDef,
-        "MotionImageInserter": MotionImageInserterTypeDef,
-        "NielsenConfiguration": NielsenConfigurationTypeDef,
-        "NielsenNonLinearWatermark": NielsenNonLinearWatermarkSettingsTypeDef,
+        "KantarWatermark": KantarWatermarkSettingsOutputTypeDef,
+        "MotionImageInserter": MotionImageInserterOutputTypeDef,
+        "NielsenConfiguration": NielsenConfigurationOutputTypeDef,
+        "NielsenNonLinearWatermark": NielsenNonLinearWatermarkSettingsOutputTypeDef,
         "OutputGroups": List[OutputGroupOutputTypeDef],
-        "TimecodeConfig": TimecodeConfigTypeDef,
+        "TimecodeConfig": TimecodeConfigOutputTypeDef,
         "TimedMetadataInsertion": TimedMetadataInsertionOutputTypeDef,
     },
-    total=False,
 )
 
 JobSettingsTypeDef = TypedDict(
     "JobSettingsTypeDef",
     {
         "AdAvailOffset": int,
         "AvailBlanking": AvailBlankingTypeDef,
@@ -4088,84 +5478,99 @@
         "OutputGroups": Sequence[OutputGroupTypeDef],
         "TimecodeConfig": TimecodeConfigTypeDef,
         "TimedMetadataInsertion": TimedMetadataInsertionTypeDef,
     },
     total=False,
 )
 
-_RequiredJobTypeDef = TypedDict(
-    "_RequiredJobTypeDef",
+CreatePresetResponseTypeDef = TypedDict(
+    "CreatePresetResponseTypeDef",
+    {
+        "Preset": PresetTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPresetResponseTypeDef = TypedDict(
+    "GetPresetResponseTypeDef",
     {
-        "Role": str,
-        "Settings": JobSettingsOutputTypeDef,
+        "Preset": PresetTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalJobTypeDef = TypedDict(
-    "_OptionalJobTypeDef",
+
+ListPresetsResponseTypeDef = TypedDict(
+    "ListPresetsResponseTypeDef",
     {
-        "AccelerationSettings": AccelerationSettingsTypeDef,
+        "NextToken": str,
+        "Presets": List[PresetTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePresetResponseTypeDef = TypedDict(
+    "UpdatePresetResponseTypeDef",
+    {
+        "Preset": PresetTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+JobTypeDef = TypedDict(
+    "JobTypeDef",
+    {
+        "AccelerationSettings": AccelerationSettingsOutputTypeDef,
         "AccelerationStatus": AccelerationStatusType,
         "Arn": str,
         "BillingTagsSource": BillingTagsSourceType,
         "ClientRequestToken": str,
         "CreatedAt": datetime,
         "CurrentPhase": JobPhaseType,
         "ErrorCode": int,
         "ErrorMessage": str,
-        "HopDestinations": List[HopDestinationTypeDef],
+        "HopDestinations": List[HopDestinationOutputTypeDef],
         "Id": str,
         "JobPercentComplete": int,
         "JobTemplate": str,
         "Messages": JobMessagesTypeDef,
         "OutputGroupDetails": List[OutputGroupDetailTypeDef],
         "Priority": int,
         "Queue": str,
         "QueueTransitions": List[QueueTransitionTypeDef],
         "RetryCount": int,
+        "Role": str,
+        "Settings": JobSettingsOutputTypeDef,
         "SimulateReservedQueue": SimulateReservedQueueType,
         "Status": JobStatusType,
         "StatusUpdateInterval": StatusUpdateIntervalType,
         "Timing": TimingTypeDef,
         "UserMetadata": Dict[str, str],
         "Warnings": List[WarningGroupTypeDef],
     },
-    total=False,
 )
 
-class JobTypeDef(_RequiredJobTypeDef, _OptionalJobTypeDef):
-    pass
-
-_RequiredJobTemplateTypeDef = TypedDict(
-    "_RequiredJobTemplateTypeDef",
-    {
-        "Name": str,
-        "Settings": JobTemplateSettingsOutputTypeDef,
-    },
-)
-_OptionalJobTemplateTypeDef = TypedDict(
-    "_OptionalJobTemplateTypeDef",
+JobTemplateTypeDef = TypedDict(
+    "JobTemplateTypeDef",
     {
-        "AccelerationSettings": AccelerationSettingsTypeDef,
+        "AccelerationSettings": AccelerationSettingsOutputTypeDef,
         "Arn": str,
         "Category": str,
         "CreatedAt": datetime,
         "Description": str,
-        "HopDestinations": List[HopDestinationTypeDef],
+        "HopDestinations": List[HopDestinationOutputTypeDef],
         "LastUpdated": datetime,
+        "Name": str,
         "Priority": int,
         "Queue": str,
+        "Settings": JobTemplateSettingsOutputTypeDef,
         "StatusUpdateInterval": StatusUpdateIntervalType,
         "Type": TypeType,
     },
-    total=False,
 )
 
-class JobTemplateTypeDef(_RequiredJobTemplateTypeDef, _OptionalJobTemplateTypeDef):
-    pass
-
 _RequiredCreateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobRequestRequestTypeDef",
     {
         "Role": str,
         "Settings": JobSettingsTypeDef,
     },
 )
@@ -4188,15 +5593,14 @@
 )
 
 class CreateJobRequestRequestTypeDef(
     _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
 ):
     pass
 
-JobSettingsUnionTypeDef = Union[JobSettingsTypeDef, JobSettingsOutputTypeDef]
 _RequiredCreateJobTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobTemplateRequestRequestTypeDef",
     {
         "Name": str,
         "Settings": JobTemplateSettingsTypeDef,
     },
 )
@@ -4216,17 +5620,14 @@
 )
 
 class CreateJobTemplateRequestRequestTypeDef(
     _RequiredCreateJobTemplateRequestRequestTypeDef, _OptionalCreateJobTemplateRequestRequestTypeDef
 ):
     pass
 
-JobTemplateSettingsUnionTypeDef = Union[
-    JobTemplateSettingsTypeDef, JobTemplateSettingsOutputTypeDef
-]
 _RequiredUpdateJobTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateJobTemplateRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateJobTemplateRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-mediaconvert-1.28.16/mypy_boto3_mediaconvert.egg-info/PKG-INFO` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediaconvert
-Version: 1.28.16
-Summary: Type annotations for boto3.MediaConvert 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.9
+Summary: Type annotations for boto3.MediaConvert 1.28.9 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 mediaconvert type-annotations botocore mypy typeshed autocomplete
+Keywords: boto3 mediaconvert type-annotations boto3-stubs mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-mediaconvert"></a>
 
 # mypy-boto3-mediaconvert
 
 [![PyPI - mypy-boto3-mediaconvert](https://img.shields.io/pypi/v/mypy-boto3-mediaconvert.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconvert)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediaconvert.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconvert)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediaconvert)](https://pepy.tech/project/mypy-boto3-mediaconvert)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediaconvert?color=blue)](https://pypistats.org/packages/mypy-boto3-mediaconvert)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaConvert 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
+[boto3.MediaConvert 1.28.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-mediaconvert docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +74,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
-    - [Type definitions](#type-definitions)
+    - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -734,180 +734,281 @@
 )
 
 
 def check_value(value: AacAudioDescriptionBroadcasterMixType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_mediaconvert.type_defs` module contains structures and shapes
-assembled to typed dictionaries and unions for additional type checking.
+assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediaconvert.type_defs import (
+    AacSettingsOutputTypeDef,
     AacSettingsTypeDef,
+    Ac3SettingsOutputTypeDef,
     Ac3SettingsTypeDef,
+    AccelerationSettingsOutputTypeDef,
     AccelerationSettingsTypeDef,
+    AdvancedInputFilterSettingsOutputTypeDef,
     AdvancedInputFilterSettingsTypeDef,
+    AiffSettingsOutputTypeDef,
     AiffSettingsTypeDef,
+    AllowedRenditionSizeOutputTypeDef,
     AllowedRenditionSizeTypeDef,
+    AncillarySourceSettingsOutputTypeDef,
     AncillarySourceSettingsTypeDef,
     AssociateCertificateRequestRequestTypeDef,
+    AudioChannelTaggingSettingsOutputTypeDef,
     AudioChannelTaggingSettingsTypeDef,
+    Eac3AtmosSettingsOutputTypeDef,
+    Eac3SettingsOutputTypeDef,
+    Mp2SettingsOutputTypeDef,
+    Mp3SettingsOutputTypeDef,
+    OpusSettingsOutputTypeDef,
+    VorbisSettingsOutputTypeDef,
+    WavSettingsOutputTypeDef,
     Eac3AtmosSettingsTypeDef,
     Eac3SettingsTypeDef,
     Mp2SettingsTypeDef,
     Mp3SettingsTypeDef,
     OpusSettingsTypeDef,
     VorbisSettingsTypeDef,
     WavSettingsTypeDef,
+    AudioNormalizationSettingsOutputTypeDef,
     AudioNormalizationSettingsTypeDef,
     AudioSelectorGroupOutputTypeDef,
     AudioSelectorGroupTypeDef,
+    HlsRenditionGroupSettingsOutputTypeDef,
     HlsRenditionGroupSettingsTypeDef,
+    ForceIncludeRenditionSizeOutputTypeDef,
+    MinBottomRenditionSizeOutputTypeDef,
+    MinTopRenditionSizeOutputTypeDef,
     ForceIncludeRenditionSizeTypeDef,
     MinBottomRenditionSizeTypeDef,
     MinTopRenditionSizeTypeDef,
+    Av1QvbrSettingsOutputTypeDef,
     Av1QvbrSettingsTypeDef,
+    AvailBlankingOutputTypeDef,
     AvailBlankingTypeDef,
+    AvcIntraUhdSettingsOutputTypeDef,
     AvcIntraUhdSettingsTypeDef,
+    BandwidthReductionFilterOutputTypeDef,
     BandwidthReductionFilterTypeDef,
+    BurninDestinationSettingsOutputTypeDef,
     BurninDestinationSettingsTypeDef,
     CancelJobRequestRequestTypeDef,
+    DvbSubDestinationSettingsOutputTypeDef,
+    EmbeddedDestinationSettingsOutputTypeDef,
+    ImscDestinationSettingsOutputTypeDef,
+    SccDestinationSettingsOutputTypeDef,
+    SrtDestinationSettingsOutputTypeDef,
+    TeletextDestinationSettingsOutputTypeDef,
+    TtmlDestinationSettingsOutputTypeDef,
+    WebvttDestinationSettingsOutputTypeDef,
     DvbSubDestinationSettingsTypeDef,
     EmbeddedDestinationSettingsTypeDef,
     ImscDestinationSettingsTypeDef,
     SccDestinationSettingsTypeDef,
     SrtDestinationSettingsTypeDef,
-    TeletextDestinationSettingsOutputTypeDef,
+    TeletextDestinationSettingsTypeDef,
     TtmlDestinationSettingsTypeDef,
     WebvttDestinationSettingsTypeDef,
-    TeletextDestinationSettingsTypeDef,
+    CaptionSourceFramerateOutputTypeDef,
     CaptionSourceFramerateTypeDef,
+    DvbSubSourceSettingsOutputTypeDef,
+    EmbeddedSourceSettingsOutputTypeDef,
+    TeletextSourceSettingsOutputTypeDef,
+    TrackSourceSettingsOutputTypeDef,
+    WebvttHlsSourceSettingsOutputTypeDef,
     DvbSubSourceSettingsTypeDef,
     EmbeddedSourceSettingsTypeDef,
     TeletextSourceSettingsTypeDef,
     TrackSourceSettingsTypeDef,
     WebvttHlsSourceSettingsTypeDef,
     OutputChannelMappingOutputTypeDef,
     OutputChannelMappingTypeDef,
+    ClipLimitsOutputTypeDef,
     ClipLimitsTypeDef,
     CmafAdditionalManifestOutputTypeDef,
     CmafAdditionalManifestTypeDef,
     SpekeKeyProviderCmafOutputTypeDef,
-    StaticKeyProviderTypeDef,
+    StaticKeyProviderOutputTypeDef,
     SpekeKeyProviderCmafTypeDef,
+    StaticKeyProviderTypeDef,
+    CmafImageBasedTrickPlaySettingsOutputTypeDef,
     CmafImageBasedTrickPlaySettingsTypeDef,
+    CmfcSettingsOutputTypeDef,
     CmfcSettingsTypeDef,
+    Hdr10MetadataOutputTypeDef,
     Hdr10MetadataTypeDef,
-    F4vSettingsTypeDef,
+    F4vSettingsOutputTypeDef,
     M3u8SettingsOutputTypeDef,
+    MovSettingsOutputTypeDef,
+    Mp4SettingsOutputTypeDef,
+    MpdSettingsOutputTypeDef,
+    F4vSettingsTypeDef,
+    M3u8SettingsTypeDef,
     MovSettingsTypeDef,
     Mp4SettingsTypeDef,
     MpdSettingsTypeDef,
-    M3u8SettingsTypeDef,
     HopDestinationTypeDef,
     ResponseMetadataTypeDef,
     ReservationPlanSettingsTypeDef,
     DashAdditionalManifestOutputTypeDef,
     DashAdditionalManifestTypeDef,
     SpekeKeyProviderOutputTypeDef,
     SpekeKeyProviderTypeDef,
+    DashIsoImageBasedTrickPlaySettingsOutputTypeDef,
     DashIsoImageBasedTrickPlaySettingsTypeDef,
+    DeinterlacerOutputTypeDef,
     DeinterlacerTypeDef,
     DeleteJobTemplateRequestRequestTypeDef,
     DeletePresetRequestRequestTypeDef,
     DeleteQueueRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeEndpointsRequestRequestTypeDef,
     EndpointTypeDef,
     DisassociateCertificateRequestRequestTypeDef,
+    DolbyVisionLevel6MetadataOutputTypeDef,
     DolbyVisionLevel6MetadataTypeDef,
+    DvbNitSettingsOutputTypeDef,
     DvbNitSettingsTypeDef,
+    DvbSdtSettingsOutputTypeDef,
     DvbSdtSettingsTypeDef,
+    DvbTdtSettingsOutputTypeDef,
     DvbTdtSettingsTypeDef,
+    EsamManifestConfirmConditionNotificationOutputTypeDef,
     EsamManifestConfirmConditionNotificationTypeDef,
+    EsamSignalProcessingNotificationOutputTypeDef,
     EsamSignalProcessingNotificationTypeDef,
+    ExtendedDataServicesOutputTypeDef,
     ExtendedDataServicesTypeDef,
+    FrameCaptureSettingsOutputTypeDef,
     FrameCaptureSettingsTypeDef,
     GetJobRequestRequestTypeDef,
     GetJobTemplateRequestRequestTypeDef,
-    PolicyTypeDef,
+    PolicyOutputTypeDef,
     GetPresetRequestRequestTypeDef,
     GetQueueRequestRequestTypeDef,
+    H264QvbrSettingsOutputTypeDef,
     H264QvbrSettingsTypeDef,
+    H265QvbrSettingsOutputTypeDef,
     H265QvbrSettingsTypeDef,
+    Hdr10PlusOutputTypeDef,
     Hdr10PlusTypeDef,
     HlsAdditionalManifestOutputTypeDef,
     HlsAdditionalManifestTypeDef,
+    HlsCaptionLanguageMappingOutputTypeDef,
     HlsCaptionLanguageMappingTypeDef,
+    HlsImageBasedTrickPlaySettingsOutputTypeDef,
     HlsImageBasedTrickPlaySettingsTypeDef,
-    HlsSettingsTypeDef,
+    HlsSettingsOutputTypeDef,
+    HopDestinationOutputTypeDef,
+    Id3InsertionOutputTypeDef,
     Id3InsertionTypeDef,
+    InsertableImageOutputTypeDef,
     InsertableImageTypeDef,
+    InputClippingOutputTypeDef,
     InputClippingTypeDef,
+    InputDecryptionSettingsOutputTypeDef,
     InputDecryptionSettingsTypeDef,
-    InputVideoGeneratorTypeDef,
+    InputVideoGeneratorOutputTypeDef,
+    RectangleOutputTypeDef,
     RectangleTypeDef,
+    InputVideoGeneratorTypeDef,
     JobMessagesTypeDef,
+    KantarWatermarkSettingsOutputTypeDef,
+    NielsenConfigurationOutputTypeDef,
+    NielsenNonLinearWatermarkSettingsOutputTypeDef,
+    TimecodeConfigOutputTypeDef,
     KantarWatermarkSettingsTypeDef,
     NielsenConfigurationTypeDef,
     NielsenNonLinearWatermarkSettingsTypeDef,
     TimecodeConfigTypeDef,
     QueueTransitionTypeDef,
     TimingTypeDef,
     WarningGroupTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListPresetsRequestRequestTypeDef,
     ListQueuesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ResourceTagsTypeDef,
+    M2tsScte35EsamOutputTypeDef,
     M2tsScte35EsamTypeDef,
+    MotionImageInsertionFramerateOutputTypeDef,
+    MotionImageInsertionOffsetOutputTypeDef,
     MotionImageInsertionFramerateTypeDef,
     MotionImageInsertionOffsetTypeDef,
+    Mpeg2SettingsOutputTypeDef,
     Mpeg2SettingsTypeDef,
     MsSmoothAdditionalManifestOutputTypeDef,
     MsSmoothAdditionalManifestTypeDef,
+    MxfXavcProfileSettingsOutputTypeDef,
     MxfXavcProfileSettingsTypeDef,
+    NexGuardFileMarkerSettingsOutputTypeDef,
     NexGuardFileMarkerSettingsTypeDef,
+    NoiseReducerFilterSettingsOutputTypeDef,
     NoiseReducerFilterSettingsTypeDef,
+    NoiseReducerSpatialFilterSettingsOutputTypeDef,
+    NoiseReducerTemporalFilterSettingsOutputTypeDef,
     NoiseReducerSpatialFilterSettingsTypeDef,
     NoiseReducerTemporalFilterSettingsTypeDef,
     VideoDetailTypeDef,
+    PolicyTypeDef,
+    ProresSettingsOutputTypeDef,
     ProresSettingsTypeDef,
     ReservationPlanTypeDef,
+    S3DestinationAccessControlOutputTypeDef,
     S3DestinationAccessControlTypeDef,
+    S3EncryptionSettingsOutputTypeDef,
     S3EncryptionSettingsTypeDef,
     TagResourceRequestRequestTypeDef,
+    TimecodeBurninOutputTypeDef,
     TimecodeBurninTypeDef,
     UntagResourceRequestRequestTypeDef,
+    Vc3SettingsOutputTypeDef,
     Vc3SettingsTypeDef,
+    Vp8SettingsOutputTypeDef,
+    Vp9SettingsOutputTypeDef,
     Vp8SettingsTypeDef,
     Vp9SettingsTypeDef,
+    Xavc4kIntraCbgProfileSettingsOutputTypeDef,
     Xavc4kIntraCbgProfileSettingsTypeDef,
+    Xavc4kIntraVbrProfileSettingsOutputTypeDef,
     Xavc4kIntraVbrProfileSettingsTypeDef,
+    Xavc4kProfileSettingsOutputTypeDef,
     Xavc4kProfileSettingsTypeDef,
+    XavcHdIntraCbgProfileSettingsOutputTypeDef,
     XavcHdIntraCbgProfileSettingsTypeDef,
+    XavcHdProfileSettingsOutputTypeDef,
     XavcHdProfileSettingsTypeDef,
+    AudioCodecSettingsOutputTypeDef,
     AudioCodecSettingsTypeDef,
     AutomatedAbrRuleOutputTypeDef,
     AutomatedAbrRuleTypeDef,
+    Av1SettingsOutputTypeDef,
     Av1SettingsTypeDef,
+    AvcIntraSettingsOutputTypeDef,
     AvcIntraSettingsTypeDef,
     CaptionDestinationSettingsOutputTypeDef,
     CaptionDestinationSettingsTypeDef,
+    FileSourceSettingsOutputTypeDef,
     FileSourceSettingsTypeDef,
     ChannelMappingOutputTypeDef,
     ChannelMappingTypeDef,
     CmafEncryptionSettingsOutputTypeDef,
     CmafEncryptionSettingsTypeDef,
+    ColorCorrectorOutputTypeDef,
+    VideoSelectorOutputTypeDef,
     ColorCorrectorTypeDef,
     VideoSelectorTypeDef,
     CreateQueueRequestRequestTypeDef,
     UpdateQueueRequestRequestTypeDef,
     DashIsoEncryptionSettingsOutputTypeDef,
     HlsEncryptionSettingsOutputTypeDef,
     MsSmoothEncryptionSettingsOutputTypeDef,
@@ -916,115 +1017,127 @@
     MsSmoothEncryptionSettingsTypeDef,
     DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef,
     ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
     ListPresetsRequestListPresetsPaginateTypeDef,
     ListQueuesRequestListQueuesPaginateTypeDef,
     DescribeEndpointsResponseTypeDef,
+    DolbyVisionOutputTypeDef,
     DolbyVisionTypeDef,
+    EsamSettingsOutputTypeDef,
     EsamSettingsTypeDef,
     GetPolicyResponseTypeDef,
-    PutPolicyRequestRequestTypeDef,
     PutPolicyResponseTypeDef,
+    H264SettingsOutputTypeDef,
     H264SettingsTypeDef,
+    H265SettingsOutputTypeDef,
     H265SettingsTypeDef,
-    OutputSettingsTypeDef,
+    OutputSettingsOutputTypeDef,
     TimedMetadataInsertionOutputTypeDef,
     TimedMetadataInsertionTypeDef,
     ImageInserterOutputTypeDef,
     ImageInserterTypeDef,
     ListTagsForResourceResponseTypeDef,
     M2tsSettingsOutputTypeDef,
     M2tsSettingsTypeDef,
+    MotionImageInserterOutputTypeDef,
     MotionImageInserterTypeDef,
+    MxfSettingsOutputTypeDef,
     MxfSettingsTypeDef,
+    PartnerWatermarkingOutputTypeDef,
     PartnerWatermarkingTypeDef,
+    NoiseReducerOutputTypeDef,
     NoiseReducerTypeDef,
     OutputDetailTypeDef,
+    PutPolicyRequestRequestTypeDef,
     QueueTypeDef,
+    S3DestinationSettingsOutputTypeDef,
     S3DestinationSettingsTypeDef,
+    XavcSettingsOutputTypeDef,
     XavcSettingsTypeDef,
     AutomatedAbrSettingsOutputTypeDef,
     AutomatedAbrSettingsTypeDef,
+    CaptionDescriptionOutputTypeDef,
     CaptionDescriptionPresetOutputTypeDef,
     CaptionDescriptionPresetTypeDef,
-    CaptionDescriptionTypeDef,
+    CaptionSourceSettingsOutputTypeDef,
     CaptionSourceSettingsTypeDef,
     RemixSettingsOutputTypeDef,
     RemixSettingsTypeDef,
     ContainerSettingsOutputTypeDef,
     ContainerSettingsTypeDef,
     VideoPreprocessorOutputTypeDef,
     VideoPreprocessorTypeDef,
     OutputGroupDetailTypeDef,
     CreateQueueResponseTypeDef,
     GetQueueResponseTypeDef,
     ListQueuesResponseTypeDef,
     UpdateQueueResponseTypeDef,
+    DestinationSettingsOutputTypeDef,
     DestinationSettingsTypeDef,
+    VideoCodecSettingsOutputTypeDef,
     VideoCodecSettingsTypeDef,
     AutomatedEncodingSettingsOutputTypeDef,
     AutomatedEncodingSettingsTypeDef,
+    CaptionSelectorOutputTypeDef,
     CaptionSelectorTypeDef,
     AudioDescriptionOutputTypeDef,
     AudioSelectorOutputTypeDef,
     AudioDescriptionTypeDef,
     AudioSelectorTypeDef,
     CmafGroupSettingsOutputTypeDef,
-    CmafGroupSettingsTypeDef,
     DashIsoGroupSettingsOutputTypeDef,
+    FileGroupSettingsOutputTypeDef,
+    HlsGroupSettingsOutputTypeDef,
+    MsSmoothGroupSettingsOutputTypeDef,
+    CmafGroupSettingsTypeDef,
     DashIsoGroupSettingsTypeDef,
     FileGroupSettingsTypeDef,
-    HlsGroupSettingsOutputTypeDef,
     HlsGroupSettingsTypeDef,
-    MsSmoothGroupSettingsOutputTypeDef,
     MsSmoothGroupSettingsTypeDef,
     VideoDescriptionOutputTypeDef,
     VideoDescriptionTypeDef,
     InputOutputTypeDef,
     InputTemplateOutputTypeDef,
     InputTemplateTypeDef,
     InputTypeDef,
     OutputGroupSettingsOutputTypeDef,
     OutputGroupSettingsTypeDef,
-    PresetSettingsOutputTypeDef,
     OutputTypeDef,
+    PresetSettingsOutputTypeDef,
     PresetSettingsTypeDef,
-    PresetTypeDef,
     OutputGroupOutputTypeDef,
     OutputGroupTypeDef,
+    PresetTypeDef,
     CreatePresetRequestRequestTypeDef,
-    PresetSettingsUnionTypeDef,
     UpdatePresetRequestRequestTypeDef,
-    CreatePresetResponseTypeDef,
-    GetPresetResponseTypeDef,
-    ListPresetsResponseTypeDef,
-    UpdatePresetResponseTypeDef,
     JobSettingsOutputTypeDef,
     JobTemplateSettingsOutputTypeDef,
     JobSettingsTypeDef,
     JobTemplateSettingsTypeDef,
+    CreatePresetResponseTypeDef,
+    GetPresetResponseTypeDef,
+    ListPresetsResponseTypeDef,
+    UpdatePresetResponseTypeDef,
     JobTypeDef,
     JobTemplateTypeDef,
     CreateJobRequestRequestTypeDef,
-    JobSettingsUnionTypeDef,
     CreateJobTemplateRequestRequestTypeDef,
-    JobTemplateSettingsUnionTypeDef,
     UpdateJobTemplateRequestRequestTypeDef,
     CreateJobResponseTypeDef,
     GetJobResponseTypeDef,
     ListJobsResponseTypeDef,
     CreateJobTemplateResponseTypeDef,
     GetJobTemplateResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
     UpdateJobTemplateResponseTypeDef,
 )
 
 
-def get_value() -> AacSettingsTypeDef:
+def get_structure() -> AacSettingsOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mediaconvert-1.28.16/mypy_boto3_mediaconvert.egg-info/SOURCES.txt` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.28.16/setup.py` & `mypy-boto3-mediaconvert-1.28.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediaconvert",
-    version="1.28.16",
+    version="1.28.9",
     packages=["mypy_boto3_mediaconvert"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MediaConvert 1.28.16 service generated with mypy-boto3-builder"
-        " 7.17.1"
+        "Type annotations for boto3.MediaConvert 1.28.9 service generated with mypy-boto3-builder"
+        " 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -34,15 +34,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
-    keywords="boto3 mediaconvert type-annotations botocore mypy typeshed autocomplete",
+    keywords="boto3 mediaconvert type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_mediaconvert": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

