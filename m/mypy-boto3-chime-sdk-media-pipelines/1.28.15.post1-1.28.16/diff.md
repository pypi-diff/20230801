# Comparing `tmp/mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-chime-sdk-media-pipelines-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:38 2023, max compression
+gzip compressed data, was "mypy-boto3-chime-sdk-media-pipelines-1.28.16.tar", last modified: Tue Aug  1 11:36:18 2023, max compression
```

## Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1.tar` & `mypy-boto3-chime-sdk-media-pipelines-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:38.237037 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:39:27.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19103 2023-07-29 10:02:38.237037 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17541 2023-07-29 09:39:27.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:38.237037 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-29 09:39:27.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-29 09:39:27.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-29 09:39:27.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18846 2023-07-29 09:39:27.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18820 2023-07-29 09:39:27.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-07-29 09:39:28.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-07-29 09:39:27.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:39:27.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    49063 2023-07-29 09:39:30.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    49006 2023-07-29 09:39:29.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:39:27.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:38.237037 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19103 2023-07-29 10:02:37.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-29 10:02:38.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:37.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:37.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:37.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-29 10:02:37.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:38.237037 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-29 09:39:27.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:18.896939 mypy-boto3-chime-sdk-media-pipelines-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:12:01.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19447 2023-08-01 11:36:18.896939 mypy-boto3-chime-sdk-media-pipelines-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-08-01 11:12:01.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:18.880939 mypy-boto3-chime-sdk-media-pipelines-1.28.16/mypy_boto3_chime_sdk_media_pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-08-01 11:12:01.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.16/mypy_boto3_chime_sdk_media_pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-08-01 11:12:01.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.16/mypy_boto3_chime_sdk_media_pipelines/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-01 11:12:01.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.16/mypy_boto3_chime_sdk_media_pipelines/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17761 2023-08-01 11:12:01.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.16/mypy_boto3_chime_sdk_media_pipelines/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17735 2023-08-01 11:12:01.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.16/mypy_boto3_chime_sdk_media_pipelines/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-08-01 11:12:01.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.16/mypy_boto3_chime_sdk_media_pipelines/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-08-01 11:12:01.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.16/mypy_boto3_chime_sdk_media_pipelines/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:12:01.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.16/mypy_boto3_chime_sdk_media_pipelines/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    50082 2023-08-01 11:12:02.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.16/mypy_boto3_chime_sdk_media_pipelines/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50025 2023-08-01 11:12:02.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.16/mypy_boto3_chime_sdk_media_pipelines/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:12:01.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.16/mypy_boto3_chime_sdk_media_pipelines/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:18.896939 mypy-boto3-chime-sdk-media-pipelines-1.28.16/mypy_boto3_chime_sdk_media_pipelines.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19447 2023-08-01 11:36:18.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.16/mypy_boto3_chime_sdk_media_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-08-01 11:36:18.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.16/mypy_boto3_chime_sdk_media_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:18.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.16/mypy_boto3_chime_sdk_media_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:18.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.16/mypy_boto3_chime_sdk_media_pipelines.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:18.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.16/mypy_boto3_chime_sdk_media_pipelines.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-01 11:36:18.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.16/mypy_boto3_chime_sdk_media_pipelines.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:18.896939 mypy-boto3-chime-sdk-media-pipelines-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-08-01 11:12:01.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.16/setup.py
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/LICENSE` & `mypy-boto3-chime-sdk-media-pipelines-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/PKG-INFO` & `mypy-boto3-chime-sdk-media-pipelines-1.28.16/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-media-pipelines
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ChimeSDKMediaPipelines 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ChimeSDKMediaPipelines 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 chime-sdk-media-pipelines type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 chime-sdk-media-pipelines type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-media-pipelines)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime-sdk-media-pipelines)](https://pepy.tech/project/mypy-boto3-chime-sdk-media-pipelines)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMediaPipelines 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
+[boto3.ChimeSDKMediaPipelines 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-chime-sdk-media-pipelines docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +73,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Literals](#literals)
-    - [Typed dictionaries](#typed-dictionaries)
+    - [Type definitions](#type-definitions)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -328,20 +328,20 @@
 )
 
 
 def check_value(value: ActiveSpeakerPositionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_chime_sdk_media_pipelines.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_chime_sdk_media_pipelines.type_defs import (
     ActiveSpeakerOnlyConfigurationTypeDef,
     PostCallAnalyticsSettingsTypeDef,
     AmazonTranscribeProcessorConfigurationTypeDef,
     AudioConcatenationConfigurationTypeDef,
@@ -359,15 +359,14 @@
     TagTypeDef,
     ResponseMetadataTypeDef,
     S3RecordingSinkRuntimeConfigurationTypeDef,
     DeleteMediaCapturePipelineRequestRequestTypeDef,
     DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     DeleteMediaPipelineRequestRequestTypeDef,
     TimestampRangeOutputTypeDef,
-    TimestampRangeTypeDef,
     GetMediaCapturePipelineRequestRequestTypeDef,
     GetMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     GetMediaPipelineRequestRequestTypeDef,
     HorizontalLayoutConfigurationTypeDef,
     PresenterOnlyConfigurationTypeDef,
     VerticalLayoutConfigurationTypeDef,
     VideoAttributeTypeDef,
@@ -388,82 +387,90 @@
     S3RecordingSinkConfigurationTypeDef,
     SnsTopicSinkConfigurationTypeDef,
     SqsQueueSinkConfigurationTypeDef,
     VoiceAnalyticsProcessorConfigurationTypeDef,
     SentimentConfigurationTypeDef,
     SelectedVideoStreamsOutputTypeDef,
     SelectedVideoStreamsTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateMediaInsightsPipelineStatusRequestRequestTypeDef,
     AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
     AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
     ArtifactsConcatenationConfigurationTypeDef,
     StreamChannelDefinitionOutputTypeDef,
     StreamChannelDefinitionTypeDef,
     ConcatenationSinkTypeDef,
     TagResourceRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
     FragmentSelectorOutputTypeDef,
-    FragmentSelectorTypeDef,
     GridViewConfigurationTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
     ListMediaInsightsPipelineConfigurationsResponseTypeDef,
     ListMediaPipelinesResponseTypeDef,
     LiveConnectorSinkConfigurationTypeDef,
     RealTimeAlertRuleOutputTypeDef,
     RealTimeAlertRuleTypeDef,
     SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
+    TimestampRangeTypeDef,
     MediaInsightsPipelineConfigurationElementOutputTypeDef,
     MediaInsightsPipelineConfigurationElementTypeDef,
     ChimeSdkMeetingConcatenationConfigurationTypeDef,
     StreamConfigurationOutputTypeDef,
     StreamConfigurationTypeDef,
     KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef,
-    KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
     CompositedVideoArtifactsConfigurationTypeDef,
     RealTimeAlertConfigurationOutputTypeDef,
     RealTimeAlertConfigurationTypeDef,
+    FragmentSelectorTypeDef,
+    MediaInsightsPipelineConfigurationElementUnionTypeDef,
     MediaCapturePipelineSourceConfigurationTypeDef,
     KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef,
     KinesisVideoStreamSourceRuntimeConfigurationTypeDef,
     ArtifactsConfigurationTypeDef,
     ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
     ChimeSdkMeetingLiveConnectorConfigurationTypeDef,
     MediaInsightsPipelineConfigurationTypeDef,
+    RealTimeAlertConfigurationUnionTypeDef,
+    KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
     CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     ConcatenationSourceTypeDef,
     MediaInsightsPipelineTypeDef,
-    CreateMediaInsightsPipelineRequestRequestTypeDef,
+    KinesisVideoStreamSourceRuntimeConfigurationUnionTypeDef,
     ChimeSdkMeetingConfigurationOutputTypeDef,
     ChimeSdkMeetingConfigurationTypeDef,
     LiveConnectorSourceConfigurationOutputTypeDef,
     LiveConnectorSourceConfigurationTypeDef,
     CreateMediaInsightsPipelineConfigurationResponseTypeDef,
     GetMediaInsightsPipelineConfigurationResponseTypeDef,
     UpdateMediaInsightsPipelineConfigurationResponseTypeDef,
+    CreateMediaInsightsPipelineRequestRequestTypeDef,
+    KinesisVideoStreamRecordingSourceRuntimeConfigurationUnionTypeDef,
     CreateMediaConcatenationPipelineRequestRequestTypeDef,
     MediaConcatenationPipelineTypeDef,
     CreateMediaInsightsPipelineResponseTypeDef,
     MediaCapturePipelineTypeDef,
+    ChimeSdkMeetingConfigurationUnionTypeDef,
     CreateMediaCapturePipelineRequestRequestTypeDef,
     MediaLiveConnectorPipelineTypeDef,
-    CreateMediaLiveConnectorPipelineRequestRequestTypeDef,
+    LiveConnectorSourceConfigurationUnionTypeDef,
     CreateMediaConcatenationPipelineResponseTypeDef,
     CreateMediaCapturePipelineResponseTypeDef,
     GetMediaCapturePipelineResponseTypeDef,
     CreateMediaLiveConnectorPipelineResponseTypeDef,
     MediaPipelineTypeDef,
+    CreateMediaLiveConnectorPipelineRequestRequestTypeDef,
     GetMediaPipelineResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveSpeakerOnlyConfigurationTypeDef:
+def get_value() -> ActiveSpeakerOnlyConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/README.md` & `mypy-boto3-chime-sdk-media-pipelines-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-media-pipelines)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime-sdk-media-pipelines)](https://pepy.tech/project/mypy-boto3-chime-sdk-media-pipelines)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMediaPipelines 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
+[boto3.ChimeSDKMediaPipelines 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-chime-sdk-media-pipelines docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/).
 
 See how it helps to find and fix potential bugs:
 
@@ -41,15 +41,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Literals](#literals)
-    - [Typed dictionaries](#typed-dictionaries)
+    - [Type definitions](#type-definitions)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -296,20 +296,20 @@
 )
 
 
 def check_value(value: ActiveSpeakerPositionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_chime_sdk_media_pipelines.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_chime_sdk_media_pipelines.type_defs import (
     ActiveSpeakerOnlyConfigurationTypeDef,
     PostCallAnalyticsSettingsTypeDef,
     AmazonTranscribeProcessorConfigurationTypeDef,
     AudioConcatenationConfigurationTypeDef,
@@ -327,15 +327,14 @@
     TagTypeDef,
     ResponseMetadataTypeDef,
     S3RecordingSinkRuntimeConfigurationTypeDef,
     DeleteMediaCapturePipelineRequestRequestTypeDef,
     DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     DeleteMediaPipelineRequestRequestTypeDef,
     TimestampRangeOutputTypeDef,
-    TimestampRangeTypeDef,
     GetMediaCapturePipelineRequestRequestTypeDef,
     GetMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     GetMediaPipelineRequestRequestTypeDef,
     HorizontalLayoutConfigurationTypeDef,
     PresenterOnlyConfigurationTypeDef,
     VerticalLayoutConfigurationTypeDef,
     VideoAttributeTypeDef,
@@ -356,82 +355,90 @@
     S3RecordingSinkConfigurationTypeDef,
     SnsTopicSinkConfigurationTypeDef,
     SqsQueueSinkConfigurationTypeDef,
     VoiceAnalyticsProcessorConfigurationTypeDef,
     SentimentConfigurationTypeDef,
     SelectedVideoStreamsOutputTypeDef,
     SelectedVideoStreamsTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateMediaInsightsPipelineStatusRequestRequestTypeDef,
     AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
     AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
     ArtifactsConcatenationConfigurationTypeDef,
     StreamChannelDefinitionOutputTypeDef,
     StreamChannelDefinitionTypeDef,
     ConcatenationSinkTypeDef,
     TagResourceRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
     FragmentSelectorOutputTypeDef,
-    FragmentSelectorTypeDef,
     GridViewConfigurationTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
     ListMediaInsightsPipelineConfigurationsResponseTypeDef,
     ListMediaPipelinesResponseTypeDef,
     LiveConnectorSinkConfigurationTypeDef,
     RealTimeAlertRuleOutputTypeDef,
     RealTimeAlertRuleTypeDef,
     SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
+    TimestampRangeTypeDef,
     MediaInsightsPipelineConfigurationElementOutputTypeDef,
     MediaInsightsPipelineConfigurationElementTypeDef,
     ChimeSdkMeetingConcatenationConfigurationTypeDef,
     StreamConfigurationOutputTypeDef,
     StreamConfigurationTypeDef,
     KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef,
-    KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
     CompositedVideoArtifactsConfigurationTypeDef,
     RealTimeAlertConfigurationOutputTypeDef,
     RealTimeAlertConfigurationTypeDef,
+    FragmentSelectorTypeDef,
+    MediaInsightsPipelineConfigurationElementUnionTypeDef,
     MediaCapturePipelineSourceConfigurationTypeDef,
     KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef,
     KinesisVideoStreamSourceRuntimeConfigurationTypeDef,
     ArtifactsConfigurationTypeDef,
     ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
     ChimeSdkMeetingLiveConnectorConfigurationTypeDef,
     MediaInsightsPipelineConfigurationTypeDef,
+    RealTimeAlertConfigurationUnionTypeDef,
+    KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
     CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     ConcatenationSourceTypeDef,
     MediaInsightsPipelineTypeDef,
-    CreateMediaInsightsPipelineRequestRequestTypeDef,
+    KinesisVideoStreamSourceRuntimeConfigurationUnionTypeDef,
     ChimeSdkMeetingConfigurationOutputTypeDef,
     ChimeSdkMeetingConfigurationTypeDef,
     LiveConnectorSourceConfigurationOutputTypeDef,
     LiveConnectorSourceConfigurationTypeDef,
     CreateMediaInsightsPipelineConfigurationResponseTypeDef,
     GetMediaInsightsPipelineConfigurationResponseTypeDef,
     UpdateMediaInsightsPipelineConfigurationResponseTypeDef,
+    CreateMediaInsightsPipelineRequestRequestTypeDef,
+    KinesisVideoStreamRecordingSourceRuntimeConfigurationUnionTypeDef,
     CreateMediaConcatenationPipelineRequestRequestTypeDef,
     MediaConcatenationPipelineTypeDef,
     CreateMediaInsightsPipelineResponseTypeDef,
     MediaCapturePipelineTypeDef,
+    ChimeSdkMeetingConfigurationUnionTypeDef,
     CreateMediaCapturePipelineRequestRequestTypeDef,
     MediaLiveConnectorPipelineTypeDef,
-    CreateMediaLiveConnectorPipelineRequestRequestTypeDef,
+    LiveConnectorSourceConfigurationUnionTypeDef,
     CreateMediaConcatenationPipelineResponseTypeDef,
     CreateMediaCapturePipelineResponseTypeDef,
     GetMediaCapturePipelineResponseTypeDef,
     CreateMediaLiveConnectorPipelineResponseTypeDef,
     MediaPipelineTypeDef,
+    CreateMediaLiveConnectorPipelineRequestRequestTypeDef,
     GetMediaPipelineResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveSpeakerOnlyConfigurationTypeDef:
+def get_value() -> ActiveSpeakerOnlyConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/__main__.py` & `mypy-boto3-chime-sdk-media-pipelines-1.28.16/mypy_boto3_chime_sdk_media_pipelines/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ChimeSDKMediaPipelines 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.ChimeSDKMediaPipelines 1.28.16\nVersion:        "
+        " 1.28.16\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.15.post1")
+    print("1.28.16")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/client.py` & `mypy-boto3-chime-sdk-media-pipelines-1.28.16/mypy_boto3_chime_sdk_media_pipelines/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,48 +10,42 @@
     from mypy_boto3_chime_sdk_media_pipelines.client import ChimeSDKMediaPipelinesClient
 
     session = Session()
     client: ChimeSDKMediaPipelinesClient = session.client("chime-sdk-media-pipelines")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import MediaPipelineStatusUpdateType
 from .type_defs import (
-    ChimeSdkMeetingConfigurationOutputTypeDef,
-    ChimeSdkMeetingConfigurationTypeDef,
+    ChimeSdkMeetingConfigurationUnionTypeDef,
     ConcatenationSinkTypeDef,
     ConcatenationSourceTypeDef,
     CreateMediaCapturePipelineResponseTypeDef,
     CreateMediaConcatenationPipelineResponseTypeDef,
     CreateMediaInsightsPipelineConfigurationResponseTypeDef,
     CreateMediaInsightsPipelineResponseTypeDef,
     CreateMediaLiveConnectorPipelineResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetMediaCapturePipelineResponseTypeDef,
     GetMediaInsightsPipelineConfigurationResponseTypeDef,
     GetMediaPipelineResponseTypeDef,
-    KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef,
-    KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
-    KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef,
-    KinesisVideoStreamSourceRuntimeConfigurationTypeDef,
+    KinesisVideoStreamRecordingSourceRuntimeConfigurationUnionTypeDef,
+    KinesisVideoStreamSourceRuntimeConfigurationUnionTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
     ListMediaInsightsPipelineConfigurationsResponseTypeDef,
     ListMediaPipelinesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     LiveConnectorSinkConfigurationTypeDef,
-    LiveConnectorSourceConfigurationOutputTypeDef,
-    LiveConnectorSourceConfigurationTypeDef,
-    MediaInsightsPipelineConfigurationElementOutputTypeDef,
-    MediaInsightsPipelineConfigurationElementTypeDef,
-    RealTimeAlertConfigurationOutputTypeDef,
-    RealTimeAlertConfigurationTypeDef,
+    LiveConnectorSourceConfigurationUnionTypeDef,
+    MediaInsightsPipelineConfigurationElementUnionTypeDef,
+    RealTimeAlertConfigurationUnionTypeDef,
     S3RecordingSinkRuntimeConfigurationTypeDef,
     TagTypeDef,
     UpdateMediaInsightsPipelineConfigurationResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -120,17 +114,15 @@
         self,
         *,
         SourceType: Literal["ChimeSdkMeeting"],
         SourceArn: str,
         SinkType: Literal["S3Bucket"],
         SinkArn: str,
         ClientRequestToken: str = ...,
-        ChimeSdkMeetingConfiguration: Union[
-            ChimeSdkMeetingConfigurationTypeDef, ChimeSdkMeetingConfigurationOutputTypeDef
-        ] = ...,
+        ChimeSdkMeetingConfiguration: ChimeSdkMeetingConfigurationUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateMediaCapturePipelineResponseTypeDef:
         """
         Creates a media pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_capture_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/client/#create_media_capture_pipeline)
@@ -151,23 +143,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/client/#create_media_concatenation_pipeline)
         """
 
     def create_media_insights_pipeline(
         self,
         *,
         MediaInsightsPipelineConfigurationArn: str,
-        KinesisVideoStreamSourceRuntimeConfiguration: Union[
-            KinesisVideoStreamSourceRuntimeConfigurationTypeDef,
-            KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef,
-        ] = ...,
+        KinesisVideoStreamSourceRuntimeConfiguration: KinesisVideoStreamSourceRuntimeConfigurationUnionTypeDef = ...,
         MediaInsightsRuntimeMetadata: Mapping[str, str] = ...,
-        KinesisVideoStreamRecordingSourceRuntimeConfiguration: Union[
-            KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
-            KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef,
-        ] = ...,
+        KinesisVideoStreamRecordingSourceRuntimeConfiguration: KinesisVideoStreamRecordingSourceRuntimeConfigurationUnionTypeDef = ...,
         S3RecordingSinkRuntimeConfiguration: S3RecordingSinkRuntimeConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...
     ) -> CreateMediaInsightsPipelineResponseTypeDef:
         """
         Creates a media insights pipeline.
 
@@ -176,43 +162,31 @@
         """
 
     def create_media_insights_pipeline_configuration(
         self,
         *,
         MediaInsightsPipelineConfigurationName: str,
         ResourceAccessRoleArn: str,
-        Elements: Sequence[
-            Union[
-                MediaInsightsPipelineConfigurationElementTypeDef,
-                MediaInsightsPipelineConfigurationElementOutputTypeDef,
-            ]
-        ],
-        RealTimeAlertConfiguration: Union[
-            RealTimeAlertConfigurationTypeDef, RealTimeAlertConfigurationOutputTypeDef
-        ] = ...,
+        Elements: Sequence[MediaInsightsPipelineConfigurationElementUnionTypeDef],
+        RealTimeAlertConfiguration: RealTimeAlertConfigurationUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...
     ) -> CreateMediaInsightsPipelineConfigurationResponseTypeDef:
         """
         A structure that contains the static configurations for a media insights
         pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_insights_pipeline_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/client/#create_media_insights_pipeline_configuration)
         """
 
     def create_media_live_connector_pipeline(
         self,
         *,
-        Sources: Sequence[
-            Union[
-                LiveConnectorSourceConfigurationTypeDef,
-                LiveConnectorSourceConfigurationOutputTypeDef,
-            ]
-        ],
+        Sources: Sequence[LiveConnectorSourceConfigurationUnionTypeDef],
         Sinks: Sequence[LiveConnectorSinkConfigurationTypeDef],
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateMediaLiveConnectorPipelineResponseTypeDef:
         """
         Creates a media live connector pipeline in an Amazon Chime SDK meeting.
 
@@ -345,23 +319,16 @@
         """
 
     def update_media_insights_pipeline_configuration(
         self,
         *,
         Identifier: str,
         ResourceAccessRoleArn: str,
-        Elements: Sequence[
-            Union[
-                MediaInsightsPipelineConfigurationElementTypeDef,
-                MediaInsightsPipelineConfigurationElementOutputTypeDef,
-            ]
-        ],
-        RealTimeAlertConfiguration: Union[
-            RealTimeAlertConfigurationTypeDef, RealTimeAlertConfigurationOutputTypeDef
-        ] = ...
+        Elements: Sequence[MediaInsightsPipelineConfigurationElementUnionTypeDef],
+        RealTimeAlertConfiguration: RealTimeAlertConfigurationUnionTypeDef = ...
     ) -> UpdateMediaInsightsPipelineConfigurationResponseTypeDef:
         """
         Updates the media insights pipeline's configuration settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.update_media_insights_pipeline_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/client/#update_media_insights_pipeline_configuration)
         """
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/client.pyi` & `mypy-boto3-chime-sdk-media-pipelines-1.28.16/mypy_boto3_chime_sdk_media_pipelines/client.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -10,48 +10,42 @@
     from mypy_boto3_chime_sdk_media_pipelines.client import ChimeSDKMediaPipelinesClient
 
     session = Session()
     client: ChimeSDKMediaPipelinesClient = session.client("chime-sdk-media-pipelines")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import MediaPipelineStatusUpdateType
 from .type_defs import (
-    ChimeSdkMeetingConfigurationOutputTypeDef,
-    ChimeSdkMeetingConfigurationTypeDef,
+    ChimeSdkMeetingConfigurationUnionTypeDef,
     ConcatenationSinkTypeDef,
     ConcatenationSourceTypeDef,
     CreateMediaCapturePipelineResponseTypeDef,
     CreateMediaConcatenationPipelineResponseTypeDef,
     CreateMediaInsightsPipelineConfigurationResponseTypeDef,
     CreateMediaInsightsPipelineResponseTypeDef,
     CreateMediaLiveConnectorPipelineResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetMediaCapturePipelineResponseTypeDef,
     GetMediaInsightsPipelineConfigurationResponseTypeDef,
     GetMediaPipelineResponseTypeDef,
-    KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef,
-    KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
-    KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef,
-    KinesisVideoStreamSourceRuntimeConfigurationTypeDef,
+    KinesisVideoStreamRecordingSourceRuntimeConfigurationUnionTypeDef,
+    KinesisVideoStreamSourceRuntimeConfigurationUnionTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
     ListMediaInsightsPipelineConfigurationsResponseTypeDef,
     ListMediaPipelinesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     LiveConnectorSinkConfigurationTypeDef,
-    LiveConnectorSourceConfigurationOutputTypeDef,
-    LiveConnectorSourceConfigurationTypeDef,
-    MediaInsightsPipelineConfigurationElementOutputTypeDef,
-    MediaInsightsPipelineConfigurationElementTypeDef,
-    RealTimeAlertConfigurationOutputTypeDef,
-    RealTimeAlertConfigurationTypeDef,
+    LiveConnectorSourceConfigurationUnionTypeDef,
+    MediaInsightsPipelineConfigurationElementUnionTypeDef,
+    RealTimeAlertConfigurationUnionTypeDef,
     S3RecordingSinkRuntimeConfigurationTypeDef,
     TagTypeDef,
     UpdateMediaInsightsPipelineConfigurationResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -113,17 +107,15 @@
         self,
         *,
         SourceType: Literal["ChimeSdkMeeting"],
         SourceArn: str,
         SinkType: Literal["S3Bucket"],
         SinkArn: str,
         ClientRequestToken: str = ...,
-        ChimeSdkMeetingConfiguration: Union[
-            ChimeSdkMeetingConfigurationTypeDef, ChimeSdkMeetingConfigurationOutputTypeDef
-        ] = ...,
+        ChimeSdkMeetingConfiguration: ChimeSdkMeetingConfigurationUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateMediaCapturePipelineResponseTypeDef:
         """
         Creates a media pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_capture_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/client/#create_media_capture_pipeline)
@@ -142,23 +134,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_concatenation_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/client/#create_media_concatenation_pipeline)
         """
     def create_media_insights_pipeline(
         self,
         *,
         MediaInsightsPipelineConfigurationArn: str,
-        KinesisVideoStreamSourceRuntimeConfiguration: Union[
-            KinesisVideoStreamSourceRuntimeConfigurationTypeDef,
-            KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef,
-        ] = ...,
+        KinesisVideoStreamSourceRuntimeConfiguration: KinesisVideoStreamSourceRuntimeConfigurationUnionTypeDef = ...,
         MediaInsightsRuntimeMetadata: Mapping[str, str] = ...,
-        KinesisVideoStreamRecordingSourceRuntimeConfiguration: Union[
-            KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
-            KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef,
-        ] = ...,
+        KinesisVideoStreamRecordingSourceRuntimeConfiguration: KinesisVideoStreamRecordingSourceRuntimeConfigurationUnionTypeDef = ...,
         S3RecordingSinkRuntimeConfiguration: S3RecordingSinkRuntimeConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...
     ) -> CreateMediaInsightsPipelineResponseTypeDef:
         """
         Creates a media insights pipeline.
 
@@ -166,42 +152,30 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/client/#create_media_insights_pipeline)
         """
     def create_media_insights_pipeline_configuration(
         self,
         *,
         MediaInsightsPipelineConfigurationName: str,
         ResourceAccessRoleArn: str,
-        Elements: Sequence[
-            Union[
-                MediaInsightsPipelineConfigurationElementTypeDef,
-                MediaInsightsPipelineConfigurationElementOutputTypeDef,
-            ]
-        ],
-        RealTimeAlertConfiguration: Union[
-            RealTimeAlertConfigurationTypeDef, RealTimeAlertConfigurationOutputTypeDef
-        ] = ...,
+        Elements: Sequence[MediaInsightsPipelineConfigurationElementUnionTypeDef],
+        RealTimeAlertConfiguration: RealTimeAlertConfigurationUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...
     ) -> CreateMediaInsightsPipelineConfigurationResponseTypeDef:
         """
         A structure that contains the static configurations for a media insights
         pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_insights_pipeline_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/client/#create_media_insights_pipeline_configuration)
         """
     def create_media_live_connector_pipeline(
         self,
         *,
-        Sources: Sequence[
-            Union[
-                LiveConnectorSourceConfigurationTypeDef,
-                LiveConnectorSourceConfigurationOutputTypeDef,
-            ]
-        ],
+        Sources: Sequence[LiveConnectorSourceConfigurationUnionTypeDef],
         Sinks: Sequence[LiveConnectorSinkConfigurationTypeDef],
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateMediaLiveConnectorPipelineResponseTypeDef:
         """
         Creates a media live connector pipeline in an Amazon Chime SDK meeting.
 
@@ -320,23 +294,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/client/#untag_resource)
         """
     def update_media_insights_pipeline_configuration(
         self,
         *,
         Identifier: str,
         ResourceAccessRoleArn: str,
-        Elements: Sequence[
-            Union[
-                MediaInsightsPipelineConfigurationElementTypeDef,
-                MediaInsightsPipelineConfigurationElementOutputTypeDef,
-            ]
-        ],
-        RealTimeAlertConfiguration: Union[
-            RealTimeAlertConfigurationTypeDef, RealTimeAlertConfigurationOutputTypeDef
-        ] = ...
+        Elements: Sequence[MediaInsightsPipelineConfigurationElementUnionTypeDef],
+        RealTimeAlertConfiguration: RealTimeAlertConfigurationUnionTypeDef = ...
     ) -> UpdateMediaInsightsPipelineConfigurationResponseTypeDef:
         """
         Updates the media insights pipeline's configuration settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.update_media_insights_pipeline_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/client/#update_media_insights_pipeline_configuration)
         """
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/literals.py` & `mypy-boto3-chime-sdk-media-pipelines-1.28.16/mypy_boto3_chime_sdk_media_pipelines/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/literals.pyi` & `mypy-boto3-chime-sdk-media-pipelines-1.28.16/mypy_boto3_chime_sdk_media_pipelines/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/type_defs.py` & `mypy-boto3-chime-sdk-media-pipelines-1.28.16/mypy_boto3_chime_sdk_media_pipelines/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_chime_sdk_media_pipelines.type_defs import ActiveSpeakerOnlyConfigurationTypeDef
 
-    data: ActiveSpeakerOnlyConfigurationTypeDef = {...}
+    data: ActiveSpeakerOnlyConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -50,15 +50,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActiveSpeakerOnlyConfigurationTypeDef",
     "PostCallAnalyticsSettingsTypeDef",
     "AmazonTranscribeProcessorConfigurationTypeDef",
     "AudioConcatenationConfigurationTypeDef",
     "CompositedVideoConcatenationConfigurationTypeDef",
     "ContentConcatenationConfigurationTypeDef",
@@ -74,15 +73,14 @@
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "S3RecordingSinkRuntimeConfigurationTypeDef",
     "DeleteMediaCapturePipelineRequestRequestTypeDef",
     "DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "DeleteMediaPipelineRequestRequestTypeDef",
     "TimestampRangeOutputTypeDef",
-    "TimestampRangeTypeDef",
     "GetMediaCapturePipelineRequestRequestTypeDef",
     "GetMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "GetMediaPipelineRequestRequestTypeDef",
     "HorizontalLayoutConfigurationTypeDef",
     "PresenterOnlyConfigurationTypeDef",
     "VerticalLayoutConfigurationTypeDef",
     "VideoAttributeTypeDef",
@@ -103,77 +101,85 @@
     "S3RecordingSinkConfigurationTypeDef",
     "SnsTopicSinkConfigurationTypeDef",
     "SqsQueueSinkConfigurationTypeDef",
     "VoiceAnalyticsProcessorConfigurationTypeDef",
     "SentimentConfigurationTypeDef",
     "SelectedVideoStreamsOutputTypeDef",
     "SelectedVideoStreamsTypeDef",
+    "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateMediaInsightsPipelineStatusRequestRequestTypeDef",
     "AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef",
     "AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef",
     "ArtifactsConcatenationConfigurationTypeDef",
     "StreamChannelDefinitionOutputTypeDef",
     "StreamChannelDefinitionTypeDef",
     "ConcatenationSinkTypeDef",
     "TagResourceRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "FragmentSelectorOutputTypeDef",
-    "FragmentSelectorTypeDef",
     "GridViewConfigurationTypeDef",
     "ListMediaCapturePipelinesResponseTypeDef",
     "ListMediaInsightsPipelineConfigurationsResponseTypeDef",
     "ListMediaPipelinesResponseTypeDef",
     "LiveConnectorSinkConfigurationTypeDef",
     "RealTimeAlertRuleOutputTypeDef",
     "RealTimeAlertRuleTypeDef",
     "SourceConfigurationOutputTypeDef",
     "SourceConfigurationTypeDef",
+    "TimestampRangeTypeDef",
     "MediaInsightsPipelineConfigurationElementOutputTypeDef",
     "MediaInsightsPipelineConfigurationElementTypeDef",
     "ChimeSdkMeetingConcatenationConfigurationTypeDef",
     "StreamConfigurationOutputTypeDef",
     "StreamConfigurationTypeDef",
     "KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef",
-    "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
     "CompositedVideoArtifactsConfigurationTypeDef",
     "RealTimeAlertConfigurationOutputTypeDef",
     "RealTimeAlertConfigurationTypeDef",
+    "FragmentSelectorTypeDef",
+    "MediaInsightsPipelineConfigurationElementUnionTypeDef",
     "MediaCapturePipelineSourceConfigurationTypeDef",
     "KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef",
     "KinesisVideoStreamSourceRuntimeConfigurationTypeDef",
     "ArtifactsConfigurationTypeDef",
     "ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
     "ChimeSdkMeetingLiveConnectorConfigurationTypeDef",
     "MediaInsightsPipelineConfigurationTypeDef",
+    "RealTimeAlertConfigurationUnionTypeDef",
+    "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
     "CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "ConcatenationSourceTypeDef",
     "MediaInsightsPipelineTypeDef",
-    "CreateMediaInsightsPipelineRequestRequestTypeDef",
+    "KinesisVideoStreamSourceRuntimeConfigurationUnionTypeDef",
     "ChimeSdkMeetingConfigurationOutputTypeDef",
     "ChimeSdkMeetingConfigurationTypeDef",
     "LiveConnectorSourceConfigurationOutputTypeDef",
     "LiveConnectorSourceConfigurationTypeDef",
     "CreateMediaInsightsPipelineConfigurationResponseTypeDef",
     "GetMediaInsightsPipelineConfigurationResponseTypeDef",
     "UpdateMediaInsightsPipelineConfigurationResponseTypeDef",
+    "CreateMediaInsightsPipelineRequestRequestTypeDef",
+    "KinesisVideoStreamRecordingSourceRuntimeConfigurationUnionTypeDef",
     "CreateMediaConcatenationPipelineRequestRequestTypeDef",
     "MediaConcatenationPipelineTypeDef",
     "CreateMediaInsightsPipelineResponseTypeDef",
     "MediaCapturePipelineTypeDef",
+    "ChimeSdkMeetingConfigurationUnionTypeDef",
     "CreateMediaCapturePipelineRequestRequestTypeDef",
     "MediaLiveConnectorPipelineTypeDef",
-    "CreateMediaLiveConnectorPipelineRequestRequestTypeDef",
+    "LiveConnectorSourceConfigurationUnionTypeDef",
     "CreateMediaConcatenationPipelineResponseTypeDef",
     "CreateMediaCapturePipelineResponseTypeDef",
     "GetMediaCapturePipelineResponseTypeDef",
     "CreateMediaLiveConnectorPipelineResponseTypeDef",
     "MediaPipelineTypeDef",
+    "CreateMediaLiveConnectorPipelineRequestRequestTypeDef",
     "GetMediaPipelineResponseTypeDef",
 )
 
 ActiveSpeakerOnlyConfigurationTypeDef = TypedDict(
     "ActiveSpeakerOnlyConfigurationTypeDef",
     {
         "ActiveSpeakerPosition": ActiveSpeakerPositionType,
@@ -193,21 +199,19 @@
     {
         "ContentRedactionOutput": ContentRedactionOutputType,
         "OutputEncryptionKMSKeyId": str,
     },
     total=False,
 )
 
-
 class PostCallAnalyticsSettingsTypeDef(
     _RequiredPostCallAnalyticsSettingsTypeDef, _OptionalPostCallAnalyticsSettingsTypeDef
 ):
     pass
 
-
 AmazonTranscribeProcessorConfigurationTypeDef = TypedDict(
     "AmazonTranscribeProcessorConfigurationTypeDef",
     {
         "LanguageCode": CallAnalyticsLanguageCodeType,
         "VocabularyName": str,
         "VocabularyFilterName": str,
         "VocabularyFilterMethod": VocabularyFilterMethodType,
@@ -294,63 +298,57 @@
     "_OptionalContentArtifactsConfigurationTypeDef",
     {
         "MuxType": Literal["ContentOnly"],
     },
     total=False,
 )
 
-
 class ContentArtifactsConfigurationTypeDef(
     _RequiredContentArtifactsConfigurationTypeDef, _OptionalContentArtifactsConfigurationTypeDef
 ):
     pass
 
-
 _RequiredVideoArtifactsConfigurationTypeDef = TypedDict(
     "_RequiredVideoArtifactsConfigurationTypeDef",
     {
         "State": ArtifactsStateType,
     },
 )
 _OptionalVideoArtifactsConfigurationTypeDef = TypedDict(
     "_OptionalVideoArtifactsConfigurationTypeDef",
     {
         "MuxType": Literal["VideoOnly"],
     },
     total=False,
 )
 
-
 class VideoArtifactsConfigurationTypeDef(
     _RequiredVideoArtifactsConfigurationTypeDef, _OptionalVideoArtifactsConfigurationTypeDef
 ):
     pass
 
-
 _RequiredChannelDefinitionTypeDef = TypedDict(
     "_RequiredChannelDefinitionTypeDef",
     {
         "ChannelId": int,
     },
 )
 _OptionalChannelDefinitionTypeDef = TypedDict(
     "_OptionalChannelDefinitionTypeDef",
     {
         "ParticipantRole": ParticipantRoleType,
     },
     total=False,
 )
 
-
 class ChannelDefinitionTypeDef(
     _RequiredChannelDefinitionTypeDef, _OptionalChannelDefinitionTypeDef
 ):
     pass
 
-
 S3BucketSinkConfigurationTypeDef = TypedDict(
     "S3BucketSinkConfigurationTypeDef",
     {
         "Destination": str,
     },
 )
 
@@ -406,22 +404,14 @@
     "TimestampRangeOutputTypeDef",
     {
         "StartTimestamp": datetime,
         "EndTimestamp": datetime,
     },
 )
 
-TimestampRangeTypeDef = TypedDict(
-    "TimestampRangeTypeDef",
-    {
-        "StartTimestamp": Union[datetime, str],
-        "EndTimestamp": Union[datetime, str],
-    },
-)
-
 GetMediaCapturePipelineRequestRequestTypeDef = TypedDict(
     "GetMediaCapturePipelineRequestRequestTypeDef",
     {
         "MediaPipelineId": str,
     },
 )
 
@@ -498,21 +488,19 @@
     "_OptionalKeywordMatchConfigurationOutputTypeDef",
     {
         "Negate": bool,
     },
     total=False,
 )
 
-
 class KeywordMatchConfigurationOutputTypeDef(
     _RequiredKeywordMatchConfigurationOutputTypeDef, _OptionalKeywordMatchConfigurationOutputTypeDef
 ):
     pass
 
-
 _RequiredKeywordMatchConfigurationTypeDef = TypedDict(
     "_RequiredKeywordMatchConfigurationTypeDef",
     {
         "RuleName": str,
         "Keywords": Sequence[str],
     },
 )
@@ -520,21 +508,19 @@
     "_OptionalKeywordMatchConfigurationTypeDef",
     {
         "Negate": bool,
     },
     total=False,
 )
 
-
 class KeywordMatchConfigurationTypeDef(
     _RequiredKeywordMatchConfigurationTypeDef, _OptionalKeywordMatchConfigurationTypeDef
 ):
     pass
 
-
 KinesisDataStreamSinkConfigurationTypeDef = TypedDict(
     "KinesisDataStreamSinkConfigurationTypeDef",
     {
         "InsightsTarget": str,
     },
     total=False,
 )
@@ -628,21 +614,19 @@
     {
         "AudioChannels": AudioChannelsOptionType,
         "AudioSampleRate": str,
     },
     total=False,
 )
 
-
 class LiveConnectorRTMPConfigurationTypeDef(
     _RequiredLiveConnectorRTMPConfigurationTypeDef, _OptionalLiveConnectorRTMPConfigurationTypeDef
 ):
     pass
 
-
 S3RecordingSinkConfigurationTypeDef = TypedDict(
     "S3RecordingSinkConfigurationTypeDef",
     {
         "Destination": str,
         "RecordingFileFormat": RecordingFileFormatType,
     },
     total=False,
@@ -696,14 +680,15 @@
     {
         "AttendeeIds": Sequence[str],
         "ExternalUserIds": Sequence[str],
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -737,22 +722,20 @@
         "FilterPartialResults": bool,
         "PostCallAnalyticsSettings": PostCallAnalyticsSettingsTypeDef,
         "CallAnalyticsStreamCategories": List[str],
     },
     total=False,
 )
 
-
 class AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef(
     _RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
     _OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
 ):
     pass
 
-
 _RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef = TypedDict(
     "_RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef",
     {
         "LanguageCode": CallAnalyticsLanguageCodeType,
     },
 )
 _OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef = TypedDict(
@@ -770,22 +753,20 @@
         "FilterPartialResults": bool,
         "PostCallAnalyticsSettings": PostCallAnalyticsSettingsTypeDef,
         "CallAnalyticsStreamCategories": Sequence[str],
     },
     total=False,
 )
 
-
 class AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef(
     _RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
     _OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
 ):
     pass
 
-
 ArtifactsConcatenationConfigurationTypeDef = TypedDict(
     "ArtifactsConcatenationConfigurationTypeDef",
     {
         "Audio": AudioConcatenationConfigurationTypeDef,
         "Video": VideoConcatenationConfigurationTypeDef,
         "Content": ContentConcatenationConfigurationTypeDef,
         "DataChannel": DataChannelConcatenationConfigurationTypeDef,
@@ -805,42 +786,38 @@
     "_OptionalStreamChannelDefinitionOutputTypeDef",
     {
         "ChannelDefinitions": List[ChannelDefinitionTypeDef],
     },
     total=False,
 )
 
-
 class StreamChannelDefinitionOutputTypeDef(
     _RequiredStreamChannelDefinitionOutputTypeDef, _OptionalStreamChannelDefinitionOutputTypeDef
 ):
     pass
 
-
 _RequiredStreamChannelDefinitionTypeDef = TypedDict(
     "_RequiredStreamChannelDefinitionTypeDef",
     {
         "NumberOfChannels": int,
     },
 )
 _OptionalStreamChannelDefinitionTypeDef = TypedDict(
     "_OptionalStreamChannelDefinitionTypeDef",
     {
         "ChannelDefinitions": Sequence[ChannelDefinitionTypeDef],
     },
     total=False,
 )
 
-
 class StreamChannelDefinitionTypeDef(
     _RequiredStreamChannelDefinitionTypeDef, _OptionalStreamChannelDefinitionTypeDef
 ):
     pass
 
-
 ConcatenationSinkTypeDef = TypedDict(
     "ConcatenationSinkTypeDef",
     {
         "Type": Literal["S3Bucket"],
         "S3BucketSinkConfiguration": S3BucketSinkConfigurationTypeDef,
     },
 )
@@ -872,22 +849,14 @@
     "FragmentSelectorOutputTypeDef",
     {
         "FragmentSelectorType": FragmentSelectorTypeType,
         "TimestampRange": TimestampRangeOutputTypeDef,
     },
 )
 
-FragmentSelectorTypeDef = TypedDict(
-    "FragmentSelectorTypeDef",
-    {
-        "FragmentSelectorType": FragmentSelectorTypeType,
-        "TimestampRange": TimestampRangeTypeDef,
-    },
-)
-
 _RequiredGridViewConfigurationTypeDef = TypedDict(
     "_RequiredGridViewConfigurationTypeDef",
     {
         "ContentShareLayout": ContentShareLayoutOptionType,
     },
 )
 _OptionalGridViewConfigurationTypeDef = TypedDict(
@@ -899,21 +868,19 @@
         "VerticalLayoutConfiguration": VerticalLayoutConfigurationTypeDef,
         "VideoAttribute": VideoAttributeTypeDef,
         "CanvasOrientation": CanvasOrientationType,
     },
     total=False,
 )
 
-
 class GridViewConfigurationTypeDef(
     _RequiredGridViewConfigurationTypeDef, _OptionalGridViewConfigurationTypeDef
 ):
     pass
 
-
 ListMediaCapturePipelinesResponseTypeDef = TypedDict(
     "ListMediaCapturePipelinesResponseTypeDef",
     {
         "MediaCapturePipelines": List[MediaCapturePipelineSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -959,21 +926,19 @@
         "KeywordMatchConfiguration": KeywordMatchConfigurationOutputTypeDef,
         "SentimentConfiguration": SentimentConfigurationTypeDef,
         "IssueDetectionConfiguration": IssueDetectionConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class RealTimeAlertRuleOutputTypeDef(
     _RequiredRealTimeAlertRuleOutputTypeDef, _OptionalRealTimeAlertRuleOutputTypeDef
 ):
     pass
 
-
 _RequiredRealTimeAlertRuleTypeDef = TypedDict(
     "_RequiredRealTimeAlertRuleTypeDef",
     {
         "Type": RealTimeAlertRuleTypeType,
     },
 )
 _OptionalRealTimeAlertRuleTypeDef = TypedDict(
@@ -982,21 +947,19 @@
         "KeywordMatchConfiguration": KeywordMatchConfigurationTypeDef,
         "SentimentConfiguration": SentimentConfigurationTypeDef,
         "IssueDetectionConfiguration": IssueDetectionConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class RealTimeAlertRuleTypeDef(
     _RequiredRealTimeAlertRuleTypeDef, _OptionalRealTimeAlertRuleTypeDef
 ):
     pass
 
-
 SourceConfigurationOutputTypeDef = TypedDict(
     "SourceConfigurationOutputTypeDef",
     {
         "SelectedVideoStreams": SelectedVideoStreamsOutputTypeDef,
     },
     total=False,
 )
@@ -1005,14 +968,22 @@
     "SourceConfigurationTypeDef",
     {
         "SelectedVideoStreams": SelectedVideoStreamsTypeDef,
     },
     total=False,
 )
 
+TimestampRangeTypeDef = TypedDict(
+    "TimestampRangeTypeDef",
+    {
+        "StartTimestamp": TimestampTypeDef,
+        "EndTimestamp": TimestampTypeDef,
+    },
+)
+
 _RequiredMediaInsightsPipelineConfigurationElementOutputTypeDef = TypedDict(
     "_RequiredMediaInsightsPipelineConfigurationElementOutputTypeDef",
     {
         "Type": MediaInsightsPipelineConfigurationElementTypeType,
     },
 )
 _OptionalMediaInsightsPipelineConfigurationElementOutputTypeDef = TypedDict(
@@ -1028,22 +999,20 @@
         "LambdaFunctionSinkConfiguration": LambdaFunctionSinkConfigurationTypeDef,
         "SqsQueueSinkConfiguration": SqsQueueSinkConfigurationTypeDef,
         "SnsTopicSinkConfiguration": SnsTopicSinkConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class MediaInsightsPipelineConfigurationElementOutputTypeDef(
     _RequiredMediaInsightsPipelineConfigurationElementOutputTypeDef,
     _OptionalMediaInsightsPipelineConfigurationElementOutputTypeDef,
 ):
     pass
 
-
 _RequiredMediaInsightsPipelineConfigurationElementTypeDef = TypedDict(
     "_RequiredMediaInsightsPipelineConfigurationElementTypeDef",
     {
         "Type": MediaInsightsPipelineConfigurationElementTypeType,
     },
 )
 _OptionalMediaInsightsPipelineConfigurationElementTypeDef = TypedDict(
@@ -1059,22 +1028,20 @@
         "LambdaFunctionSinkConfiguration": LambdaFunctionSinkConfigurationTypeDef,
         "SqsQueueSinkConfiguration": SqsQueueSinkConfigurationTypeDef,
         "SnsTopicSinkConfiguration": SnsTopicSinkConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class MediaInsightsPipelineConfigurationElementTypeDef(
     _RequiredMediaInsightsPipelineConfigurationElementTypeDef,
     _OptionalMediaInsightsPipelineConfigurationElementTypeDef,
 ):
     pass
 
-
 ChimeSdkMeetingConcatenationConfigurationTypeDef = TypedDict(
     "ChimeSdkMeetingConcatenationConfigurationTypeDef",
     {
         "ArtifactsConfiguration": ArtifactsConcatenationConfigurationTypeDef,
     },
 )
 
@@ -1089,21 +1056,19 @@
     "_OptionalStreamConfigurationOutputTypeDef",
     {
         "FragmentNumber": str,
     },
     total=False,
 )
 
-
 class StreamConfigurationOutputTypeDef(
     _RequiredStreamConfigurationOutputTypeDef, _OptionalStreamConfigurationOutputTypeDef
 ):
     pass
 
-
 _RequiredStreamConfigurationTypeDef = TypedDict(
     "_RequiredStreamConfigurationTypeDef",
     {
         "StreamArn": str,
         "StreamChannelDefinition": StreamChannelDefinitionTypeDef,
     },
 )
@@ -1111,37 +1076,27 @@
     "_OptionalStreamConfigurationTypeDef",
     {
         "FragmentNumber": str,
     },
     total=False,
 )
 
-
 class StreamConfigurationTypeDef(
     _RequiredStreamConfigurationTypeDef, _OptionalStreamConfigurationTypeDef
 ):
     pass
 
-
 KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef = TypedDict(
     "KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef",
     {
         "Streams": List[RecordingStreamConfigurationTypeDef],
         "FragmentSelector": FragmentSelectorOutputTypeDef,
     },
 )
 
-KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef = TypedDict(
-    "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
-    {
-        "Streams": Sequence[RecordingStreamConfigurationTypeDef],
-        "FragmentSelector": FragmentSelectorTypeDef,
-    },
-)
-
 _RequiredCompositedVideoArtifactsConfigurationTypeDef = TypedDict(
     "_RequiredCompositedVideoArtifactsConfigurationTypeDef",
     {
         "GridViewConfiguration": GridViewConfigurationTypeDef,
     },
 )
 _OptionalCompositedVideoArtifactsConfigurationTypeDef = TypedDict(
@@ -1149,22 +1104,20 @@
     {
         "Layout": Literal["GridView"],
         "Resolution": ResolutionOptionType,
     },
     total=False,
 )
 
-
 class CompositedVideoArtifactsConfigurationTypeDef(
     _RequiredCompositedVideoArtifactsConfigurationTypeDef,
     _OptionalCompositedVideoArtifactsConfigurationTypeDef,
 ):
     pass
 
-
 RealTimeAlertConfigurationOutputTypeDef = TypedDict(
     "RealTimeAlertConfigurationOutputTypeDef",
     {
         "Disabled": bool,
         "Rules": List[RealTimeAlertRuleOutputTypeDef],
     },
     total=False,
@@ -1175,14 +1128,26 @@
     {
         "Disabled": bool,
         "Rules": Sequence[RealTimeAlertRuleTypeDef],
     },
     total=False,
 )
 
+FragmentSelectorTypeDef = TypedDict(
+    "FragmentSelectorTypeDef",
+    {
+        "FragmentSelectorType": FragmentSelectorTypeType,
+        "TimestampRange": TimestampRangeTypeDef,
+    },
+)
+
+MediaInsightsPipelineConfigurationElementUnionTypeDef = Union[
+    MediaInsightsPipelineConfigurationElementTypeDef,
+    MediaInsightsPipelineConfigurationElementOutputTypeDef,
+]
 MediaCapturePipelineSourceConfigurationTypeDef = TypedDict(
     "MediaCapturePipelineSourceConfigurationTypeDef",
     {
         "MediaPipelineArn": str,
         "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConcatenationConfigurationTypeDef,
     },
 )
@@ -1217,21 +1182,19 @@
     "_OptionalArtifactsConfigurationTypeDef",
     {
         "CompositedVideo": CompositedVideoArtifactsConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class ArtifactsConfigurationTypeDef(
     _RequiredArtifactsConfigurationTypeDef, _OptionalArtifactsConfigurationTypeDef
 ):
     pass
 
-
 _RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef = TypedDict(
     "_RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
     {
         "Arn": str,
         "MuxType": LiveConnectorMuxTypeType,
     },
 )
@@ -1240,22 +1203,20 @@
     {
         "CompositedVideo": CompositedVideoArtifactsConfigurationTypeDef,
         "SourceConfiguration": SourceConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-
 class ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef(
     _RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
     _OptionalChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
 ):
     pass
 
-
 _RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef = TypedDict(
     "_RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef",
     {
         "Arn": str,
         "MuxType": LiveConnectorMuxTypeType,
     },
 )
@@ -1264,22 +1225,20 @@
     {
         "CompositedVideo": CompositedVideoArtifactsConfigurationTypeDef,
         "SourceConfiguration": SourceConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class ChimeSdkMeetingLiveConnectorConfigurationTypeDef(
     _RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef,
     _OptionalChimeSdkMeetingLiveConnectorConfigurationTypeDef,
 ):
     pass
 
-
 MediaInsightsPipelineConfigurationTypeDef = TypedDict(
     "MediaInsightsPipelineConfigurationTypeDef",
     {
         "MediaInsightsPipelineConfigurationName": str,
         "MediaInsightsPipelineConfigurationArn": str,
         "ResourceAccessRoleArn": str,
         "RealTimeAlertConfiguration": RealTimeAlertConfigurationOutputTypeDef,
@@ -1287,74 +1246,71 @@
         "MediaInsightsPipelineConfigurationId": str,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
     },
     total=False,
 )
 
+RealTimeAlertConfigurationUnionTypeDef = Union[
+    RealTimeAlertConfigurationTypeDef, RealTimeAlertConfigurationOutputTypeDef
+]
+KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef = TypedDict(
+    "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
+    {
+        "Streams": Sequence[RecordingStreamConfigurationTypeDef],
+        "FragmentSelector": FragmentSelectorTypeDef,
+    },
+)
+
 _RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "MediaInsightsPipelineConfigurationName": str,
         "ResourceAccessRoleArn": str,
-        "Elements": Sequence[
-            Union[
-                MediaInsightsPipelineConfigurationElementTypeDef,
-                MediaInsightsPipelineConfigurationElementOutputTypeDef,
-            ]
-        ],
+        "Elements": Sequence[MediaInsightsPipelineConfigurationElementUnionTypeDef],
     },
 )
 _OptionalCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "RealTimeAlertConfiguration": RealTimeAlertConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef(
     _RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     _OptionalCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "Identifier": str,
         "ResourceAccessRoleArn": str,
-        "Elements": Sequence[
-            Union[
-                MediaInsightsPipelineConfigurationElementTypeDef,
-                MediaInsightsPipelineConfigurationElementOutputTypeDef,
-            ]
-        ],
+        "Elements": Sequence[MediaInsightsPipelineConfigurationElementUnionTypeDef],
     },
 )
 _OptionalUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "RealTimeAlertConfiguration": RealTimeAlertConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef(
     _RequiredUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     _OptionalUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 ConcatenationSourceTypeDef = TypedDict(
     "ConcatenationSourceTypeDef",
     {
         "Type": Literal["MediaCapturePipeline"],
         "MediaCapturePipelineSourceConfiguration": MediaCapturePipelineSourceConfigurationTypeDef,
     },
 )
@@ -1375,45 +1331,18 @@
         ),
         "S3RecordingSinkRuntimeConfiguration": S3RecordingSinkRuntimeConfigurationTypeDef,
         "CreatedTimestamp": datetime,
     },
     total=False,
 )
 
-_RequiredCreateMediaInsightsPipelineRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateMediaInsightsPipelineRequestRequestTypeDef",
-    {
-        "MediaInsightsPipelineConfigurationArn": str,
-    },
-)
-_OptionalCreateMediaInsightsPipelineRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateMediaInsightsPipelineRequestRequestTypeDef",
-    {
-        "KinesisVideoStreamSourceRuntimeConfiguration": (
-            KinesisVideoStreamSourceRuntimeConfigurationTypeDef
-        ),
-        "MediaInsightsRuntimeMetadata": Mapping[str, str],
-        "KinesisVideoStreamRecordingSourceRuntimeConfiguration": (
-            KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef
-        ),
-        "S3RecordingSinkRuntimeConfiguration": S3RecordingSinkRuntimeConfigurationTypeDef,
-        "Tags": Sequence[TagTypeDef],
-        "ClientRequestToken": str,
-    },
-    total=False,
-)
-
-
-class CreateMediaInsightsPipelineRequestRequestTypeDef(
-    _RequiredCreateMediaInsightsPipelineRequestRequestTypeDef,
-    _OptionalCreateMediaInsightsPipelineRequestRequestTypeDef,
-):
-    pass
-
-
+KinesisVideoStreamSourceRuntimeConfigurationUnionTypeDef = Union[
+    KinesisVideoStreamSourceRuntimeConfigurationTypeDef,
+    KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef,
+]
 ChimeSdkMeetingConfigurationOutputTypeDef = TypedDict(
     "ChimeSdkMeetingConfigurationOutputTypeDef",
     {
         "SourceConfiguration": SourceConfigurationOutputTypeDef,
         "ArtifactsConfiguration": ArtifactsConfigurationTypeDef,
     },
     total=False,
@@ -1468,14 +1397,47 @@
     "UpdateMediaInsightsPipelineConfigurationResponseTypeDef",
     {
         "MediaInsightsPipelineConfiguration": MediaInsightsPipelineConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateMediaInsightsPipelineRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateMediaInsightsPipelineRequestRequestTypeDef",
+    {
+        "MediaInsightsPipelineConfigurationArn": str,
+    },
+)
+_OptionalCreateMediaInsightsPipelineRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateMediaInsightsPipelineRequestRequestTypeDef",
+    {
+        "KinesisVideoStreamSourceRuntimeConfiguration": (
+            KinesisVideoStreamSourceRuntimeConfigurationTypeDef
+        ),
+        "MediaInsightsRuntimeMetadata": Mapping[str, str],
+        "KinesisVideoStreamRecordingSourceRuntimeConfiguration": (
+            KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef
+        ),
+        "S3RecordingSinkRuntimeConfiguration": S3RecordingSinkRuntimeConfigurationTypeDef,
+        "Tags": Sequence[TagTypeDef],
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+class CreateMediaInsightsPipelineRequestRequestTypeDef(
+    _RequiredCreateMediaInsightsPipelineRequestRequestTypeDef,
+    _OptionalCreateMediaInsightsPipelineRequestRequestTypeDef,
+):
+    pass
+
+KinesisVideoStreamRecordingSourceRuntimeConfigurationUnionTypeDef = Union[
+    KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
+    KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef,
+]
 _RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef",
     {
         "Sources": Sequence[ConcatenationSourceTypeDef],
         "Sinks": Sequence[ConcatenationSinkTypeDef],
     },
 )
@@ -1484,22 +1446,20 @@
     {
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateMediaConcatenationPipelineRequestRequestTypeDef(
     _RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef,
     _OptionalCreateMediaConcatenationPipelineRequestRequestTypeDef,
 ):
     pass
 
-
 MediaConcatenationPipelineTypeDef = TypedDict(
     "MediaConcatenationPipelineTypeDef",
     {
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
         "Sources": List[ConcatenationSourceTypeDef],
         "Sinks": List[ConcatenationSinkTypeDef],
@@ -1531,14 +1491,17 @@
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationOutputTypeDef,
     },
     total=False,
 )
 
+ChimeSdkMeetingConfigurationUnionTypeDef = Union[
+    ChimeSdkMeetingConfigurationTypeDef, ChimeSdkMeetingConfigurationOutputTypeDef
+]
 _RequiredCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaCapturePipelineRequestRequestTypeDef",
     {
         "SourceType": Literal["ChimeSdkMeeting"],
         "SourceArn": str,
         "SinkType": Literal["S3Bucket"],
         "SinkArn": str,
@@ -1550,65 +1513,37 @@
         "ClientRequestToken": str,
         "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateMediaCapturePipelineRequestRequestTypeDef(
     _RequiredCreateMediaCapturePipelineRequestRequestTypeDef,
     _OptionalCreateMediaCapturePipelineRequestRequestTypeDef,
 ):
     pass
 
-
 MediaLiveConnectorPipelineTypeDef = TypedDict(
     "MediaLiveConnectorPipelineTypeDef",
     {
         "Sources": List[LiveConnectorSourceConfigurationOutputTypeDef],
         "Sinks": List[LiveConnectorSinkConfigurationTypeDef],
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
         "Status": MediaPipelineStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
     },
     total=False,
 )
 
-_RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef",
-    {
-        "Sources": Sequence[
-            Union[
-                LiveConnectorSourceConfigurationTypeDef,
-                LiveConnectorSourceConfigurationOutputTypeDef,
-            ]
-        ],
-        "Sinks": Sequence[LiveConnectorSinkConfigurationTypeDef],
-    },
-)
-_OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateMediaLiveConnectorPipelineRequestRequestTypeDef(
-    _RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
-    _OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
-):
-    pass
-
-
+LiveConnectorSourceConfigurationUnionTypeDef = Union[
+    LiveConnectorSourceConfigurationTypeDef, LiveConnectorSourceConfigurationOutputTypeDef
+]
 CreateMediaConcatenationPipelineResponseTypeDef = TypedDict(
     "CreateMediaConcatenationPipelineResponseTypeDef",
     {
         "MediaConcatenationPipeline": MediaConcatenationPipelineTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1644,14 +1579,36 @@
         "MediaLiveConnectorPipeline": MediaLiveConnectorPipelineTypeDef,
         "MediaConcatenationPipeline": MediaConcatenationPipelineTypeDef,
         "MediaInsightsPipeline": MediaInsightsPipelineTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef",
+    {
+        "Sources": Sequence[LiveConnectorSourceConfigurationUnionTypeDef],
+        "Sinks": Sequence[LiveConnectorSinkConfigurationTypeDef],
+    },
+)
+_OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateMediaLiveConnectorPipelineRequestRequestTypeDef(
+    _RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
+    _OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
+):
+    pass
+
 GetMediaPipelineResponseTypeDef = TypedDict(
     "GetMediaPipelineResponseTypeDef",
     {
         "MediaPipeline": MediaPipelineTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/type_defs.pyi` & `mypy-boto3-chime-sdk-media-pipelines-1.28.16/mypy_boto3_chime_sdk_media_pipelines/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_chime_sdk_media_pipelines.type_defs import ActiveSpeakerOnlyConfigurationTypeDef
 
-    data: ActiveSpeakerOnlyConfigurationTypeDef = {...}
+    data: ActiveSpeakerOnlyConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -50,14 +50,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ActiveSpeakerOnlyConfigurationTypeDef",
     "PostCallAnalyticsSettingsTypeDef",
     "AmazonTranscribeProcessorConfigurationTypeDef",
     "AudioConcatenationConfigurationTypeDef",
     "CompositedVideoConcatenationConfigurationTypeDef",
     "ContentConcatenationConfigurationTypeDef",
@@ -73,15 +74,14 @@
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "S3RecordingSinkRuntimeConfigurationTypeDef",
     "DeleteMediaCapturePipelineRequestRequestTypeDef",
     "DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "DeleteMediaPipelineRequestRequestTypeDef",
     "TimestampRangeOutputTypeDef",
-    "TimestampRangeTypeDef",
     "GetMediaCapturePipelineRequestRequestTypeDef",
     "GetMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "GetMediaPipelineRequestRequestTypeDef",
     "HorizontalLayoutConfigurationTypeDef",
     "PresenterOnlyConfigurationTypeDef",
     "VerticalLayoutConfigurationTypeDef",
     "VideoAttributeTypeDef",
@@ -102,77 +102,85 @@
     "S3RecordingSinkConfigurationTypeDef",
     "SnsTopicSinkConfigurationTypeDef",
     "SqsQueueSinkConfigurationTypeDef",
     "VoiceAnalyticsProcessorConfigurationTypeDef",
     "SentimentConfigurationTypeDef",
     "SelectedVideoStreamsOutputTypeDef",
     "SelectedVideoStreamsTypeDef",
+    "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateMediaInsightsPipelineStatusRequestRequestTypeDef",
     "AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef",
     "AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef",
     "ArtifactsConcatenationConfigurationTypeDef",
     "StreamChannelDefinitionOutputTypeDef",
     "StreamChannelDefinitionTypeDef",
     "ConcatenationSinkTypeDef",
     "TagResourceRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "FragmentSelectorOutputTypeDef",
-    "FragmentSelectorTypeDef",
     "GridViewConfigurationTypeDef",
     "ListMediaCapturePipelinesResponseTypeDef",
     "ListMediaInsightsPipelineConfigurationsResponseTypeDef",
     "ListMediaPipelinesResponseTypeDef",
     "LiveConnectorSinkConfigurationTypeDef",
     "RealTimeAlertRuleOutputTypeDef",
     "RealTimeAlertRuleTypeDef",
     "SourceConfigurationOutputTypeDef",
     "SourceConfigurationTypeDef",
+    "TimestampRangeTypeDef",
     "MediaInsightsPipelineConfigurationElementOutputTypeDef",
     "MediaInsightsPipelineConfigurationElementTypeDef",
     "ChimeSdkMeetingConcatenationConfigurationTypeDef",
     "StreamConfigurationOutputTypeDef",
     "StreamConfigurationTypeDef",
     "KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef",
-    "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
     "CompositedVideoArtifactsConfigurationTypeDef",
     "RealTimeAlertConfigurationOutputTypeDef",
     "RealTimeAlertConfigurationTypeDef",
+    "FragmentSelectorTypeDef",
+    "MediaInsightsPipelineConfigurationElementUnionTypeDef",
     "MediaCapturePipelineSourceConfigurationTypeDef",
     "KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef",
     "KinesisVideoStreamSourceRuntimeConfigurationTypeDef",
     "ArtifactsConfigurationTypeDef",
     "ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
     "ChimeSdkMeetingLiveConnectorConfigurationTypeDef",
     "MediaInsightsPipelineConfigurationTypeDef",
+    "RealTimeAlertConfigurationUnionTypeDef",
+    "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
     "CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "ConcatenationSourceTypeDef",
     "MediaInsightsPipelineTypeDef",
-    "CreateMediaInsightsPipelineRequestRequestTypeDef",
+    "KinesisVideoStreamSourceRuntimeConfigurationUnionTypeDef",
     "ChimeSdkMeetingConfigurationOutputTypeDef",
     "ChimeSdkMeetingConfigurationTypeDef",
     "LiveConnectorSourceConfigurationOutputTypeDef",
     "LiveConnectorSourceConfigurationTypeDef",
     "CreateMediaInsightsPipelineConfigurationResponseTypeDef",
     "GetMediaInsightsPipelineConfigurationResponseTypeDef",
     "UpdateMediaInsightsPipelineConfigurationResponseTypeDef",
+    "CreateMediaInsightsPipelineRequestRequestTypeDef",
+    "KinesisVideoStreamRecordingSourceRuntimeConfigurationUnionTypeDef",
     "CreateMediaConcatenationPipelineRequestRequestTypeDef",
     "MediaConcatenationPipelineTypeDef",
     "CreateMediaInsightsPipelineResponseTypeDef",
     "MediaCapturePipelineTypeDef",
+    "ChimeSdkMeetingConfigurationUnionTypeDef",
     "CreateMediaCapturePipelineRequestRequestTypeDef",
     "MediaLiveConnectorPipelineTypeDef",
-    "CreateMediaLiveConnectorPipelineRequestRequestTypeDef",
+    "LiveConnectorSourceConfigurationUnionTypeDef",
     "CreateMediaConcatenationPipelineResponseTypeDef",
     "CreateMediaCapturePipelineResponseTypeDef",
     "GetMediaCapturePipelineResponseTypeDef",
     "CreateMediaLiveConnectorPipelineResponseTypeDef",
     "MediaPipelineTypeDef",
+    "CreateMediaLiveConnectorPipelineRequestRequestTypeDef",
     "GetMediaPipelineResponseTypeDef",
 )
 
 ActiveSpeakerOnlyConfigurationTypeDef = TypedDict(
     "ActiveSpeakerOnlyConfigurationTypeDef",
     {
         "ActiveSpeakerPosition": ActiveSpeakerPositionType,
@@ -192,19 +200,21 @@
     {
         "ContentRedactionOutput": ContentRedactionOutputType,
         "OutputEncryptionKMSKeyId": str,
     },
     total=False,
 )
 
+
 class PostCallAnalyticsSettingsTypeDef(
     _RequiredPostCallAnalyticsSettingsTypeDef, _OptionalPostCallAnalyticsSettingsTypeDef
 ):
     pass
 
+
 AmazonTranscribeProcessorConfigurationTypeDef = TypedDict(
     "AmazonTranscribeProcessorConfigurationTypeDef",
     {
         "LanguageCode": CallAnalyticsLanguageCodeType,
         "VocabularyName": str,
         "VocabularyFilterName": str,
         "VocabularyFilterMethod": VocabularyFilterMethodType,
@@ -291,57 +301,63 @@
     "_OptionalContentArtifactsConfigurationTypeDef",
     {
         "MuxType": Literal["ContentOnly"],
     },
     total=False,
 )
 
+
 class ContentArtifactsConfigurationTypeDef(
     _RequiredContentArtifactsConfigurationTypeDef, _OptionalContentArtifactsConfigurationTypeDef
 ):
     pass
 
+
 _RequiredVideoArtifactsConfigurationTypeDef = TypedDict(
     "_RequiredVideoArtifactsConfigurationTypeDef",
     {
         "State": ArtifactsStateType,
     },
 )
 _OptionalVideoArtifactsConfigurationTypeDef = TypedDict(
     "_OptionalVideoArtifactsConfigurationTypeDef",
     {
         "MuxType": Literal["VideoOnly"],
     },
     total=False,
 )
 
+
 class VideoArtifactsConfigurationTypeDef(
     _RequiredVideoArtifactsConfigurationTypeDef, _OptionalVideoArtifactsConfigurationTypeDef
 ):
     pass
 
+
 _RequiredChannelDefinitionTypeDef = TypedDict(
     "_RequiredChannelDefinitionTypeDef",
     {
         "ChannelId": int,
     },
 )
 _OptionalChannelDefinitionTypeDef = TypedDict(
     "_OptionalChannelDefinitionTypeDef",
     {
         "ParticipantRole": ParticipantRoleType,
     },
     total=False,
 )
 
+
 class ChannelDefinitionTypeDef(
     _RequiredChannelDefinitionTypeDef, _OptionalChannelDefinitionTypeDef
 ):
     pass
 
+
 S3BucketSinkConfigurationTypeDef = TypedDict(
     "S3BucketSinkConfigurationTypeDef",
     {
         "Destination": str,
     },
 )
 
@@ -397,22 +413,14 @@
     "TimestampRangeOutputTypeDef",
     {
         "StartTimestamp": datetime,
         "EndTimestamp": datetime,
     },
 )
 
-TimestampRangeTypeDef = TypedDict(
-    "TimestampRangeTypeDef",
-    {
-        "StartTimestamp": Union[datetime, str],
-        "EndTimestamp": Union[datetime, str],
-    },
-)
-
 GetMediaCapturePipelineRequestRequestTypeDef = TypedDict(
     "GetMediaCapturePipelineRequestRequestTypeDef",
     {
         "MediaPipelineId": str,
     },
 )
 
@@ -489,19 +497,21 @@
     "_OptionalKeywordMatchConfigurationOutputTypeDef",
     {
         "Negate": bool,
     },
     total=False,
 )
 
+
 class KeywordMatchConfigurationOutputTypeDef(
     _RequiredKeywordMatchConfigurationOutputTypeDef, _OptionalKeywordMatchConfigurationOutputTypeDef
 ):
     pass
 
+
 _RequiredKeywordMatchConfigurationTypeDef = TypedDict(
     "_RequiredKeywordMatchConfigurationTypeDef",
     {
         "RuleName": str,
         "Keywords": Sequence[str],
     },
 )
@@ -509,19 +519,21 @@
     "_OptionalKeywordMatchConfigurationTypeDef",
     {
         "Negate": bool,
     },
     total=False,
 )
 
+
 class KeywordMatchConfigurationTypeDef(
     _RequiredKeywordMatchConfigurationTypeDef, _OptionalKeywordMatchConfigurationTypeDef
 ):
     pass
 
+
 KinesisDataStreamSinkConfigurationTypeDef = TypedDict(
     "KinesisDataStreamSinkConfigurationTypeDef",
     {
         "InsightsTarget": str,
     },
     total=False,
 )
@@ -615,19 +627,21 @@
     {
         "AudioChannels": AudioChannelsOptionType,
         "AudioSampleRate": str,
     },
     total=False,
 )
 
+
 class LiveConnectorRTMPConfigurationTypeDef(
     _RequiredLiveConnectorRTMPConfigurationTypeDef, _OptionalLiveConnectorRTMPConfigurationTypeDef
 ):
     pass
 
+
 S3RecordingSinkConfigurationTypeDef = TypedDict(
     "S3RecordingSinkConfigurationTypeDef",
     {
         "Destination": str,
         "RecordingFileFormat": RecordingFileFormatType,
     },
     total=False,
@@ -681,14 +695,15 @@
     {
         "AttendeeIds": Sequence[str],
         "ExternalUserIds": Sequence[str],
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -722,20 +737,22 @@
         "FilterPartialResults": bool,
         "PostCallAnalyticsSettings": PostCallAnalyticsSettingsTypeDef,
         "CallAnalyticsStreamCategories": List[str],
     },
     total=False,
 )
 
+
 class AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef(
     _RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
     _OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
 ):
     pass
 
+
 _RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef = TypedDict(
     "_RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef",
     {
         "LanguageCode": CallAnalyticsLanguageCodeType,
     },
 )
 _OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef = TypedDict(
@@ -753,20 +770,22 @@
         "FilterPartialResults": bool,
         "PostCallAnalyticsSettings": PostCallAnalyticsSettingsTypeDef,
         "CallAnalyticsStreamCategories": Sequence[str],
     },
     total=False,
 )
 
+
 class AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef(
     _RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
     _OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
 ):
     pass
 
+
 ArtifactsConcatenationConfigurationTypeDef = TypedDict(
     "ArtifactsConcatenationConfigurationTypeDef",
     {
         "Audio": AudioConcatenationConfigurationTypeDef,
         "Video": VideoConcatenationConfigurationTypeDef,
         "Content": ContentConcatenationConfigurationTypeDef,
         "DataChannel": DataChannelConcatenationConfigurationTypeDef,
@@ -786,38 +805,42 @@
     "_OptionalStreamChannelDefinitionOutputTypeDef",
     {
         "ChannelDefinitions": List[ChannelDefinitionTypeDef],
     },
     total=False,
 )
 
+
 class StreamChannelDefinitionOutputTypeDef(
     _RequiredStreamChannelDefinitionOutputTypeDef, _OptionalStreamChannelDefinitionOutputTypeDef
 ):
     pass
 
+
 _RequiredStreamChannelDefinitionTypeDef = TypedDict(
     "_RequiredStreamChannelDefinitionTypeDef",
     {
         "NumberOfChannels": int,
     },
 )
 _OptionalStreamChannelDefinitionTypeDef = TypedDict(
     "_OptionalStreamChannelDefinitionTypeDef",
     {
         "ChannelDefinitions": Sequence[ChannelDefinitionTypeDef],
     },
     total=False,
 )
 
+
 class StreamChannelDefinitionTypeDef(
     _RequiredStreamChannelDefinitionTypeDef, _OptionalStreamChannelDefinitionTypeDef
 ):
     pass
 
+
 ConcatenationSinkTypeDef = TypedDict(
     "ConcatenationSinkTypeDef",
     {
         "Type": Literal["S3Bucket"],
         "S3BucketSinkConfiguration": S3BucketSinkConfigurationTypeDef,
     },
 )
@@ -849,22 +872,14 @@
     "FragmentSelectorOutputTypeDef",
     {
         "FragmentSelectorType": FragmentSelectorTypeType,
         "TimestampRange": TimestampRangeOutputTypeDef,
     },
 )
 
-FragmentSelectorTypeDef = TypedDict(
-    "FragmentSelectorTypeDef",
-    {
-        "FragmentSelectorType": FragmentSelectorTypeType,
-        "TimestampRange": TimestampRangeTypeDef,
-    },
-)
-
 _RequiredGridViewConfigurationTypeDef = TypedDict(
     "_RequiredGridViewConfigurationTypeDef",
     {
         "ContentShareLayout": ContentShareLayoutOptionType,
     },
 )
 _OptionalGridViewConfigurationTypeDef = TypedDict(
@@ -876,19 +891,21 @@
         "VerticalLayoutConfiguration": VerticalLayoutConfigurationTypeDef,
         "VideoAttribute": VideoAttributeTypeDef,
         "CanvasOrientation": CanvasOrientationType,
     },
     total=False,
 )
 
+
 class GridViewConfigurationTypeDef(
     _RequiredGridViewConfigurationTypeDef, _OptionalGridViewConfigurationTypeDef
 ):
     pass
 
+
 ListMediaCapturePipelinesResponseTypeDef = TypedDict(
     "ListMediaCapturePipelinesResponseTypeDef",
     {
         "MediaCapturePipelines": List[MediaCapturePipelineSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -934,19 +951,21 @@
         "KeywordMatchConfiguration": KeywordMatchConfigurationOutputTypeDef,
         "SentimentConfiguration": SentimentConfigurationTypeDef,
         "IssueDetectionConfiguration": IssueDetectionConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class RealTimeAlertRuleOutputTypeDef(
     _RequiredRealTimeAlertRuleOutputTypeDef, _OptionalRealTimeAlertRuleOutputTypeDef
 ):
     pass
 
+
 _RequiredRealTimeAlertRuleTypeDef = TypedDict(
     "_RequiredRealTimeAlertRuleTypeDef",
     {
         "Type": RealTimeAlertRuleTypeType,
     },
 )
 _OptionalRealTimeAlertRuleTypeDef = TypedDict(
@@ -955,19 +974,21 @@
         "KeywordMatchConfiguration": KeywordMatchConfigurationTypeDef,
         "SentimentConfiguration": SentimentConfigurationTypeDef,
         "IssueDetectionConfiguration": IssueDetectionConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class RealTimeAlertRuleTypeDef(
     _RequiredRealTimeAlertRuleTypeDef, _OptionalRealTimeAlertRuleTypeDef
 ):
     pass
 
+
 SourceConfigurationOutputTypeDef = TypedDict(
     "SourceConfigurationOutputTypeDef",
     {
         "SelectedVideoStreams": SelectedVideoStreamsOutputTypeDef,
     },
     total=False,
 )
@@ -976,14 +997,22 @@
     "SourceConfigurationTypeDef",
     {
         "SelectedVideoStreams": SelectedVideoStreamsTypeDef,
     },
     total=False,
 )
 
+TimestampRangeTypeDef = TypedDict(
+    "TimestampRangeTypeDef",
+    {
+        "StartTimestamp": TimestampTypeDef,
+        "EndTimestamp": TimestampTypeDef,
+    },
+)
+
 _RequiredMediaInsightsPipelineConfigurationElementOutputTypeDef = TypedDict(
     "_RequiredMediaInsightsPipelineConfigurationElementOutputTypeDef",
     {
         "Type": MediaInsightsPipelineConfigurationElementTypeType,
     },
 )
 _OptionalMediaInsightsPipelineConfigurationElementOutputTypeDef = TypedDict(
@@ -999,20 +1028,22 @@
         "LambdaFunctionSinkConfiguration": LambdaFunctionSinkConfigurationTypeDef,
         "SqsQueueSinkConfiguration": SqsQueueSinkConfigurationTypeDef,
         "SnsTopicSinkConfiguration": SnsTopicSinkConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class MediaInsightsPipelineConfigurationElementOutputTypeDef(
     _RequiredMediaInsightsPipelineConfigurationElementOutputTypeDef,
     _OptionalMediaInsightsPipelineConfigurationElementOutputTypeDef,
 ):
     pass
 
+
 _RequiredMediaInsightsPipelineConfigurationElementTypeDef = TypedDict(
     "_RequiredMediaInsightsPipelineConfigurationElementTypeDef",
     {
         "Type": MediaInsightsPipelineConfigurationElementTypeType,
     },
 )
 _OptionalMediaInsightsPipelineConfigurationElementTypeDef = TypedDict(
@@ -1028,20 +1059,22 @@
         "LambdaFunctionSinkConfiguration": LambdaFunctionSinkConfigurationTypeDef,
         "SqsQueueSinkConfiguration": SqsQueueSinkConfigurationTypeDef,
         "SnsTopicSinkConfiguration": SnsTopicSinkConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class MediaInsightsPipelineConfigurationElementTypeDef(
     _RequiredMediaInsightsPipelineConfigurationElementTypeDef,
     _OptionalMediaInsightsPipelineConfigurationElementTypeDef,
 ):
     pass
 
+
 ChimeSdkMeetingConcatenationConfigurationTypeDef = TypedDict(
     "ChimeSdkMeetingConcatenationConfigurationTypeDef",
     {
         "ArtifactsConfiguration": ArtifactsConcatenationConfigurationTypeDef,
     },
 )
 
@@ -1056,19 +1089,21 @@
     "_OptionalStreamConfigurationOutputTypeDef",
     {
         "FragmentNumber": str,
     },
     total=False,
 )
 
+
 class StreamConfigurationOutputTypeDef(
     _RequiredStreamConfigurationOutputTypeDef, _OptionalStreamConfigurationOutputTypeDef
 ):
     pass
 
+
 _RequiredStreamConfigurationTypeDef = TypedDict(
     "_RequiredStreamConfigurationTypeDef",
     {
         "StreamArn": str,
         "StreamChannelDefinition": StreamChannelDefinitionTypeDef,
     },
 )
@@ -1076,35 +1111,29 @@
     "_OptionalStreamConfigurationTypeDef",
     {
         "FragmentNumber": str,
     },
     total=False,
 )
 
+
 class StreamConfigurationTypeDef(
     _RequiredStreamConfigurationTypeDef, _OptionalStreamConfigurationTypeDef
 ):
     pass
 
+
 KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef = TypedDict(
     "KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef",
     {
         "Streams": List[RecordingStreamConfigurationTypeDef],
         "FragmentSelector": FragmentSelectorOutputTypeDef,
     },
 )
 
-KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef = TypedDict(
-    "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
-    {
-        "Streams": Sequence[RecordingStreamConfigurationTypeDef],
-        "FragmentSelector": FragmentSelectorTypeDef,
-    },
-)
-
 _RequiredCompositedVideoArtifactsConfigurationTypeDef = TypedDict(
     "_RequiredCompositedVideoArtifactsConfigurationTypeDef",
     {
         "GridViewConfiguration": GridViewConfigurationTypeDef,
     },
 )
 _OptionalCompositedVideoArtifactsConfigurationTypeDef = TypedDict(
@@ -1112,20 +1141,22 @@
     {
         "Layout": Literal["GridView"],
         "Resolution": ResolutionOptionType,
     },
     total=False,
 )
 
+
 class CompositedVideoArtifactsConfigurationTypeDef(
     _RequiredCompositedVideoArtifactsConfigurationTypeDef,
     _OptionalCompositedVideoArtifactsConfigurationTypeDef,
 ):
     pass
 
+
 RealTimeAlertConfigurationOutputTypeDef = TypedDict(
     "RealTimeAlertConfigurationOutputTypeDef",
     {
         "Disabled": bool,
         "Rules": List[RealTimeAlertRuleOutputTypeDef],
     },
     total=False,
@@ -1136,14 +1167,26 @@
     {
         "Disabled": bool,
         "Rules": Sequence[RealTimeAlertRuleTypeDef],
     },
     total=False,
 )
 
+FragmentSelectorTypeDef = TypedDict(
+    "FragmentSelectorTypeDef",
+    {
+        "FragmentSelectorType": FragmentSelectorTypeType,
+        "TimestampRange": TimestampRangeTypeDef,
+    },
+)
+
+MediaInsightsPipelineConfigurationElementUnionTypeDef = Union[
+    MediaInsightsPipelineConfigurationElementTypeDef,
+    MediaInsightsPipelineConfigurationElementOutputTypeDef,
+]
 MediaCapturePipelineSourceConfigurationTypeDef = TypedDict(
     "MediaCapturePipelineSourceConfigurationTypeDef",
     {
         "MediaPipelineArn": str,
         "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConcatenationConfigurationTypeDef,
     },
 )
@@ -1178,19 +1221,21 @@
     "_OptionalArtifactsConfigurationTypeDef",
     {
         "CompositedVideo": CompositedVideoArtifactsConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class ArtifactsConfigurationTypeDef(
     _RequiredArtifactsConfigurationTypeDef, _OptionalArtifactsConfigurationTypeDef
 ):
     pass
 
+
 _RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef = TypedDict(
     "_RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
     {
         "Arn": str,
         "MuxType": LiveConnectorMuxTypeType,
     },
 )
@@ -1199,20 +1244,22 @@
     {
         "CompositedVideo": CompositedVideoArtifactsConfigurationTypeDef,
         "SourceConfiguration": SourceConfigurationOutputTypeDef,
     },
     total=False,
 )
 
+
 class ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef(
     _RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
     _OptionalChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
 ):
     pass
 
+
 _RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef = TypedDict(
     "_RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef",
     {
         "Arn": str,
         "MuxType": LiveConnectorMuxTypeType,
     },
 )
@@ -1221,20 +1268,22 @@
     {
         "CompositedVideo": CompositedVideoArtifactsConfigurationTypeDef,
         "SourceConfiguration": SourceConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class ChimeSdkMeetingLiveConnectorConfigurationTypeDef(
     _RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef,
     _OptionalChimeSdkMeetingLiveConnectorConfigurationTypeDef,
 ):
     pass
 
+
 MediaInsightsPipelineConfigurationTypeDef = TypedDict(
     "MediaInsightsPipelineConfigurationTypeDef",
     {
         "MediaInsightsPipelineConfigurationName": str,
         "MediaInsightsPipelineConfigurationArn": str,
         "ResourceAccessRoleArn": str,
         "RealTimeAlertConfiguration": RealTimeAlertConfigurationOutputTypeDef,
@@ -1242,70 +1291,75 @@
         "MediaInsightsPipelineConfigurationId": str,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
     },
     total=False,
 )
 
+RealTimeAlertConfigurationUnionTypeDef = Union[
+    RealTimeAlertConfigurationTypeDef, RealTimeAlertConfigurationOutputTypeDef
+]
+KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef = TypedDict(
+    "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
+    {
+        "Streams": Sequence[RecordingStreamConfigurationTypeDef],
+        "FragmentSelector": FragmentSelectorTypeDef,
+    },
+)
+
 _RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "MediaInsightsPipelineConfigurationName": str,
         "ResourceAccessRoleArn": str,
-        "Elements": Sequence[
-            Union[
-                MediaInsightsPipelineConfigurationElementTypeDef,
-                MediaInsightsPipelineConfigurationElementOutputTypeDef,
-            ]
-        ],
+        "Elements": Sequence[MediaInsightsPipelineConfigurationElementUnionTypeDef],
     },
 )
 _OptionalCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "RealTimeAlertConfiguration": RealTimeAlertConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef(
     _RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     _OptionalCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "Identifier": str,
         "ResourceAccessRoleArn": str,
-        "Elements": Sequence[
-            Union[
-                MediaInsightsPipelineConfigurationElementTypeDef,
-                MediaInsightsPipelineConfigurationElementOutputTypeDef,
-            ]
-        ],
+        "Elements": Sequence[MediaInsightsPipelineConfigurationElementUnionTypeDef],
     },
 )
 _OptionalUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "RealTimeAlertConfiguration": RealTimeAlertConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef(
     _RequiredUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     _OptionalUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 ConcatenationSourceTypeDef = TypedDict(
     "ConcatenationSourceTypeDef",
     {
         "Type": Literal["MediaCapturePipeline"],
         "MediaCapturePipelineSourceConfiguration": MediaCapturePipelineSourceConfigurationTypeDef,
     },
 )
@@ -1326,43 +1380,18 @@
         ),
         "S3RecordingSinkRuntimeConfiguration": S3RecordingSinkRuntimeConfigurationTypeDef,
         "CreatedTimestamp": datetime,
     },
     total=False,
 )
 
-_RequiredCreateMediaInsightsPipelineRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateMediaInsightsPipelineRequestRequestTypeDef",
-    {
-        "MediaInsightsPipelineConfigurationArn": str,
-    },
-)
-_OptionalCreateMediaInsightsPipelineRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateMediaInsightsPipelineRequestRequestTypeDef",
-    {
-        "KinesisVideoStreamSourceRuntimeConfiguration": (
-            KinesisVideoStreamSourceRuntimeConfigurationTypeDef
-        ),
-        "MediaInsightsRuntimeMetadata": Mapping[str, str],
-        "KinesisVideoStreamRecordingSourceRuntimeConfiguration": (
-            KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef
-        ),
-        "S3RecordingSinkRuntimeConfiguration": S3RecordingSinkRuntimeConfigurationTypeDef,
-        "Tags": Sequence[TagTypeDef],
-        "ClientRequestToken": str,
-    },
-    total=False,
-)
-
-class CreateMediaInsightsPipelineRequestRequestTypeDef(
-    _RequiredCreateMediaInsightsPipelineRequestRequestTypeDef,
-    _OptionalCreateMediaInsightsPipelineRequestRequestTypeDef,
-):
-    pass
-
+KinesisVideoStreamSourceRuntimeConfigurationUnionTypeDef = Union[
+    KinesisVideoStreamSourceRuntimeConfigurationTypeDef,
+    KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef,
+]
 ChimeSdkMeetingConfigurationOutputTypeDef = TypedDict(
     "ChimeSdkMeetingConfigurationOutputTypeDef",
     {
         "SourceConfiguration": SourceConfigurationOutputTypeDef,
         "ArtifactsConfiguration": ArtifactsConfigurationTypeDef,
     },
     total=False,
@@ -1417,14 +1446,49 @@
     "UpdateMediaInsightsPipelineConfigurationResponseTypeDef",
     {
         "MediaInsightsPipelineConfiguration": MediaInsightsPipelineConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateMediaInsightsPipelineRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateMediaInsightsPipelineRequestRequestTypeDef",
+    {
+        "MediaInsightsPipelineConfigurationArn": str,
+    },
+)
+_OptionalCreateMediaInsightsPipelineRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateMediaInsightsPipelineRequestRequestTypeDef",
+    {
+        "KinesisVideoStreamSourceRuntimeConfiguration": (
+            KinesisVideoStreamSourceRuntimeConfigurationTypeDef
+        ),
+        "MediaInsightsRuntimeMetadata": Mapping[str, str],
+        "KinesisVideoStreamRecordingSourceRuntimeConfiguration": (
+            KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef
+        ),
+        "S3RecordingSinkRuntimeConfiguration": S3RecordingSinkRuntimeConfigurationTypeDef,
+        "Tags": Sequence[TagTypeDef],
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+
+class CreateMediaInsightsPipelineRequestRequestTypeDef(
+    _RequiredCreateMediaInsightsPipelineRequestRequestTypeDef,
+    _OptionalCreateMediaInsightsPipelineRequestRequestTypeDef,
+):
+    pass
+
+
+KinesisVideoStreamRecordingSourceRuntimeConfigurationUnionTypeDef = Union[
+    KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
+    KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef,
+]
 _RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef",
     {
         "Sources": Sequence[ConcatenationSourceTypeDef],
         "Sinks": Sequence[ConcatenationSinkTypeDef],
     },
 )
@@ -1433,20 +1497,22 @@
     {
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateMediaConcatenationPipelineRequestRequestTypeDef(
     _RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef,
     _OptionalCreateMediaConcatenationPipelineRequestRequestTypeDef,
 ):
     pass
 
+
 MediaConcatenationPipelineTypeDef = TypedDict(
     "MediaConcatenationPipelineTypeDef",
     {
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
         "Sources": List[ConcatenationSourceTypeDef],
         "Sinks": List[ConcatenationSinkTypeDef],
@@ -1478,14 +1544,17 @@
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationOutputTypeDef,
     },
     total=False,
 )
 
+ChimeSdkMeetingConfigurationUnionTypeDef = Union[
+    ChimeSdkMeetingConfigurationTypeDef, ChimeSdkMeetingConfigurationOutputTypeDef
+]
 _RequiredCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaCapturePipelineRequestRequestTypeDef",
     {
         "SourceType": Literal["ChimeSdkMeeting"],
         "SourceArn": str,
         "SinkType": Literal["S3Bucket"],
         "SinkArn": str,
@@ -1497,61 +1566,39 @@
         "ClientRequestToken": str,
         "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateMediaCapturePipelineRequestRequestTypeDef(
     _RequiredCreateMediaCapturePipelineRequestRequestTypeDef,
     _OptionalCreateMediaCapturePipelineRequestRequestTypeDef,
 ):
     pass
 
+
 MediaLiveConnectorPipelineTypeDef = TypedDict(
     "MediaLiveConnectorPipelineTypeDef",
     {
         "Sources": List[LiveConnectorSourceConfigurationOutputTypeDef],
         "Sinks": List[LiveConnectorSinkConfigurationTypeDef],
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
         "Status": MediaPipelineStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
     },
     total=False,
 )
 
-_RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef",
-    {
-        "Sources": Sequence[
-            Union[
-                LiveConnectorSourceConfigurationTypeDef,
-                LiveConnectorSourceConfigurationOutputTypeDef,
-            ]
-        ],
-        "Sinks": Sequence[LiveConnectorSinkConfigurationTypeDef],
-    },
-)
-_OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateMediaLiveConnectorPipelineRequestRequestTypeDef(
-    _RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
-    _OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
-):
-    pass
-
+LiveConnectorSourceConfigurationUnionTypeDef = Union[
+    LiveConnectorSourceConfigurationTypeDef, LiveConnectorSourceConfigurationOutputTypeDef
+]
 CreateMediaConcatenationPipelineResponseTypeDef = TypedDict(
     "CreateMediaConcatenationPipelineResponseTypeDef",
     {
         "MediaConcatenationPipeline": MediaConcatenationPipelineTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1587,14 +1634,38 @@
         "MediaLiveConnectorPipeline": MediaLiveConnectorPipelineTypeDef,
         "MediaConcatenationPipeline": MediaConcatenationPipelineTypeDef,
         "MediaInsightsPipeline": MediaInsightsPipelineTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef",
+    {
+        "Sources": Sequence[LiveConnectorSourceConfigurationUnionTypeDef],
+        "Sinks": Sequence[LiveConnectorSinkConfigurationTypeDef],
+    },
+)
+_OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateMediaLiveConnectorPipelineRequestRequestTypeDef(
+    _RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
+    _OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
+):
+    pass
+
+
 GetMediaPipelineResponseTypeDef = TypedDict(
     "GetMediaPipelineResponseTypeDef",
     {
         "MediaPipeline": MediaPipelineTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines.egg-info/PKG-INFO` & `mypy-boto3-chime-sdk-media-pipelines-1.28.16/mypy_boto3_chime_sdk_media_pipelines.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-media-pipelines
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ChimeSDKMediaPipelines 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ChimeSDKMediaPipelines 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 chime-sdk-media-pipelines type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 chime-sdk-media-pipelines type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-media-pipelines)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime-sdk-media-pipelines)](https://pepy.tech/project/mypy-boto3-chime-sdk-media-pipelines)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMediaPipelines 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
+[boto3.ChimeSDKMediaPipelines 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-chime-sdk-media-pipelines docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +73,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Literals](#literals)
-    - [Typed dictionaries](#typed-dictionaries)
+    - [Type definitions](#type-definitions)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -328,20 +328,20 @@
 )
 
 
 def check_value(value: ActiveSpeakerPositionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_chime_sdk_media_pipelines.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_chime_sdk_media_pipelines.type_defs import (
     ActiveSpeakerOnlyConfigurationTypeDef,
     PostCallAnalyticsSettingsTypeDef,
     AmazonTranscribeProcessorConfigurationTypeDef,
     AudioConcatenationConfigurationTypeDef,
@@ -359,15 +359,14 @@
     TagTypeDef,
     ResponseMetadataTypeDef,
     S3RecordingSinkRuntimeConfigurationTypeDef,
     DeleteMediaCapturePipelineRequestRequestTypeDef,
     DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     DeleteMediaPipelineRequestRequestTypeDef,
     TimestampRangeOutputTypeDef,
-    TimestampRangeTypeDef,
     GetMediaCapturePipelineRequestRequestTypeDef,
     GetMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     GetMediaPipelineRequestRequestTypeDef,
     HorizontalLayoutConfigurationTypeDef,
     PresenterOnlyConfigurationTypeDef,
     VerticalLayoutConfigurationTypeDef,
     VideoAttributeTypeDef,
@@ -388,82 +387,90 @@
     S3RecordingSinkConfigurationTypeDef,
     SnsTopicSinkConfigurationTypeDef,
     SqsQueueSinkConfigurationTypeDef,
     VoiceAnalyticsProcessorConfigurationTypeDef,
     SentimentConfigurationTypeDef,
     SelectedVideoStreamsOutputTypeDef,
     SelectedVideoStreamsTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateMediaInsightsPipelineStatusRequestRequestTypeDef,
     AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
     AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
     ArtifactsConcatenationConfigurationTypeDef,
     StreamChannelDefinitionOutputTypeDef,
     StreamChannelDefinitionTypeDef,
     ConcatenationSinkTypeDef,
     TagResourceRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
     FragmentSelectorOutputTypeDef,
-    FragmentSelectorTypeDef,
     GridViewConfigurationTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
     ListMediaInsightsPipelineConfigurationsResponseTypeDef,
     ListMediaPipelinesResponseTypeDef,
     LiveConnectorSinkConfigurationTypeDef,
     RealTimeAlertRuleOutputTypeDef,
     RealTimeAlertRuleTypeDef,
     SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
+    TimestampRangeTypeDef,
     MediaInsightsPipelineConfigurationElementOutputTypeDef,
     MediaInsightsPipelineConfigurationElementTypeDef,
     ChimeSdkMeetingConcatenationConfigurationTypeDef,
     StreamConfigurationOutputTypeDef,
     StreamConfigurationTypeDef,
     KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef,
-    KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
     CompositedVideoArtifactsConfigurationTypeDef,
     RealTimeAlertConfigurationOutputTypeDef,
     RealTimeAlertConfigurationTypeDef,
+    FragmentSelectorTypeDef,
+    MediaInsightsPipelineConfigurationElementUnionTypeDef,
     MediaCapturePipelineSourceConfigurationTypeDef,
     KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef,
     KinesisVideoStreamSourceRuntimeConfigurationTypeDef,
     ArtifactsConfigurationTypeDef,
     ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
     ChimeSdkMeetingLiveConnectorConfigurationTypeDef,
     MediaInsightsPipelineConfigurationTypeDef,
+    RealTimeAlertConfigurationUnionTypeDef,
+    KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
     CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     ConcatenationSourceTypeDef,
     MediaInsightsPipelineTypeDef,
-    CreateMediaInsightsPipelineRequestRequestTypeDef,
+    KinesisVideoStreamSourceRuntimeConfigurationUnionTypeDef,
     ChimeSdkMeetingConfigurationOutputTypeDef,
     ChimeSdkMeetingConfigurationTypeDef,
     LiveConnectorSourceConfigurationOutputTypeDef,
     LiveConnectorSourceConfigurationTypeDef,
     CreateMediaInsightsPipelineConfigurationResponseTypeDef,
     GetMediaInsightsPipelineConfigurationResponseTypeDef,
     UpdateMediaInsightsPipelineConfigurationResponseTypeDef,
+    CreateMediaInsightsPipelineRequestRequestTypeDef,
+    KinesisVideoStreamRecordingSourceRuntimeConfigurationUnionTypeDef,
     CreateMediaConcatenationPipelineRequestRequestTypeDef,
     MediaConcatenationPipelineTypeDef,
     CreateMediaInsightsPipelineResponseTypeDef,
     MediaCapturePipelineTypeDef,
+    ChimeSdkMeetingConfigurationUnionTypeDef,
     CreateMediaCapturePipelineRequestRequestTypeDef,
     MediaLiveConnectorPipelineTypeDef,
-    CreateMediaLiveConnectorPipelineRequestRequestTypeDef,
+    LiveConnectorSourceConfigurationUnionTypeDef,
     CreateMediaConcatenationPipelineResponseTypeDef,
     CreateMediaCapturePipelineResponseTypeDef,
     GetMediaCapturePipelineResponseTypeDef,
     CreateMediaLiveConnectorPipelineResponseTypeDef,
     MediaPipelineTypeDef,
+    CreateMediaLiveConnectorPipelineRequestRequestTypeDef,
     GetMediaPipelineResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveSpeakerOnlyConfigurationTypeDef:
+def get_value() -> ActiveSpeakerOnlyConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines.egg-info/SOURCES.txt` & `mypy-boto3-chime-sdk-media-pipelines-1.28.16/mypy_boto3_chime_sdk_media_pipelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/setup.py` & `mypy-boto3-chime-sdk-media-pipelines-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-chime-sdk-media-pipelines",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_chime_sdk_media_pipelines"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ChimeSDKMediaPipelines 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.ChimeSDKMediaPipelines 1.28.16 service generated with"
+        " mypy-boto3-builder 7.17.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -34,17 +34,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
-    keywords=(
-        "boto3 chime-sdk-media-pipelines type-annotations boto3-stubs mypy typeshed autocomplete"
-    ),
+    keywords="boto3 chime-sdk-media-pipelines type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_chime_sdk_media_pipelines": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/"
```

