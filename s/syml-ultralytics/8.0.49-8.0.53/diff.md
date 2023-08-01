# Comparing `tmp/syml_ultralytics-8.0.49.tar.gz` & `tmp/syml_ultralytics-8.0.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syml_ultralytics-8.0.49.tar", last modified: Fri Mar  3 14:31:59 2023, max compression
+gzip compressed data, was "syml_ultralytics-8.0.53.tar", last modified: Tue Mar 14 13:27:12 2023, max compression
```

## Comparing `syml_ultralytics-8.0.49.tar` & `syml_ultralytics-8.0.53.tar`

### file list

```diff
@@ -1,155 +1,164 @@
-drwxrwxrwx   0        0        0        0 2023-03-03 14:31:59.597694 syml_ultralytics-8.0.49/
--rw-rw-rw-   0        0        0     5729 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    35823 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/LICENSE
--rw-rw-rw-   0        0        0      146 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/MANIFEST.in
--rw-rw-rw-   0        0        0    23205 2023-03-03 14:31:59.597694 syml_ultralytics-8.0.49/PKG-INFO
--rw-rw-rw-   0        0        0    21770 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/README.md
--rw-rw-rw-   0        0        0    20649 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/README.zh-CN.md
--rw-rw-rw-   0        0        0     1204 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/requirements.txt
--rw-rw-rw-   0        0        0      723 2023-03-03 14:31:59.599695 syml_ultralytics-8.0.49/setup.cfg
--rw-rw-rw-   0        0        0     2743 2023-03-03 14:31:51.000000 syml_ultralytics-8.0.49/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:31:59.513557 syml_ultralytics-8.0.49/syml_ultralytics.egg-info/
--rw-rw-rw-   0        0        0    23205 2023-03-03 14:31:59.000000 syml_ultralytics-8.0.49/syml_ultralytics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4442 2023-03-03 14:31:59.000000 syml_ultralytics-8.0.49/syml_ultralytics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-03 14:31:59.000000 syml_ultralytics-8.0.49/syml_ultralytics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2023-03-03 14:31:59.000000 syml_ultralytics-8.0.49/syml_ultralytics.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      451 2023-03-03 14:31:59.000000 syml_ultralytics-8.0.49/syml_ultralytics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-03 14:31:59.000000 syml_ultralytics-8.0.49/syml_ultralytics.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-03 14:31:59.514555 syml_ultralytics-8.0.49/ultralytics/
--rw-rw-rw-   0        0        0      251 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:31:59.525558 syml_ultralytics-8.0.49/ultralytics/datasets/
--rw-rw-rw-   0        0        0     2818 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/datasets/Argoverse.yaml
--rw-rw-rw-   0        0        0     1966 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/datasets/GlobalWheat2020.yaml
--rw-rw-rw-   0        0        0    44458 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/datasets/ImageNet.yaml
--rw-rw-rw-   0        0        0     9707 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/datasets/Objects365.yaml
--rw-rw-rw-   0        0        0     2489 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/datasets/SKU-110K.yaml
--rw-rw-rw-   0        0        0     3606 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/datasets/VOC.yaml
--rw-rw-rw-   0        0        0     3081 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/datasets/VisDrone.yaml
--rw-rw-rw-   0        0        0     2635 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/datasets/coco.yaml
--rw-rw-rw-   0        0        0     1957 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/datasets/coco128-seg.yaml
--rw-rw-rw-   0        0        0     1941 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/datasets/coco128.yaml
--rw-rw-rw-   0        0        0     1892 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/datasets/coco8-seg.yaml
--rw-rw-rw-   0        0        0     1872 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/datasets/coco8.yaml
--rw-rw-rw-   0        0        0     5325 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/datasets/xView.yaml
-drwxrwxrwx   0        0        0        0 2023-03-03 14:31:59.528084 syml_ultralytics-8.0.49/ultralytics/hub/
--rw-rw-rw-   0        0        0     3512 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/hub/__init__.py
--rw-rw-rw-   0        0        0     2553 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/hub/auth.py
--rw-rw-rw-   0        0        0     5599 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/hub/session.py
--rw-rw-rw-   0        0        0     9639 2023-03-03 14:04:52.000000 syml_ultralytics-8.0.49/ultralytics/hub/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:31:59.487035 syml_ultralytics-8.0.49/ultralytics/models/
-drwxrwxrwx   0        0        0        0 2023-03-03 14:31:59.530099 syml_ultralytics-8.0.49/ultralytics/models/v3/
--rw-rw-rw-   0        0        0     1481 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/models/v3/yolov3-sppu.yaml
--rw-rw-rw-   0        0        0     1173 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/models/v3/yolov3-tinyu.yaml
--rw-rw-rw-   0        0        0     1472 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/models/v3/yolov3u.yaml
-drwxrwxrwx   0        0        0        0 2023-03-03 14:31:59.534047 syml_ultralytics-8.0.49/ultralytics/models/v5/
--rw-rw-rw-   0        0        0     1312 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/models/v5/yolov5lu.yaml
--rw-rw-rw-   0        0        0     1314 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/models/v5/yolov5mu.yaml
--rw-rw-rw-   0        0        0     1314 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/models/v5/yolov5nu.yaml
--rw-rw-rw-   0        0        0     1316 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/models/v5/yolov5su.yaml
--rw-rw-rw-   0        0        0     1314 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/models/v5/yolov5xu.yaml
-drwxrwxrwx   0        0        0        0 2023-03-03 14:31:59.538046 syml_ultralytics-8.0.49/ultralytics/models/v8/
-drwxrwxrwx   0        0        0        0 2023-03-03 14:31:59.542046 syml_ultralytics-8.0.49/ultralytics/models/v8/cls/
--rw-rw-rw-   0        0        0      652 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/models/v8/cls/yolov8l-cls.yaml
--rw-rw-rw-   0        0        0      652 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/models/v8/cls/yolov8m-cls.yaml
--rw-rw-rw-   0        0        0      652 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/models/v8/cls/yolov8n-cls.yaml
--rw-rw-rw-   0        0        0      652 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/models/v8/cls/yolov8s-cls.yaml
--rw-rw-rw-   0        0        0      652 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/models/v8/cls/yolov8x-cls.yaml
-drwxrwxrwx   0        0        0        0 2023-03-03 14:31:59.546047 syml_ultralytics-8.0.49/ultralytics/models/v8/seg/
--rw-rw-rw-   0        0        0     1249 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/models/v8/seg/yolov8l-seg.yaml
--rw-rw-rw-   0        0        0     1249 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/models/v8/seg/yolov8m-seg.yaml
--rw-rw-rw-   0        0        0     1253 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/models/v8/seg/yolov8n-seg.yaml
--rw-rw-rw-   0        0        0     1253 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/models/v8/seg/yolov8s-seg.yaml
--rw-rw-rw-   0        0        0     1249 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/models/v8/seg/yolov8x-seg.yaml
--rw-rw-rw-   0        0        0     1239 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/models/v8/yolov8l.yaml
--rw-rw-rw-   0        0        0     1239 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/models/v8/yolov8m.yaml
--rw-rw-rw-   0        0        0     1243 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/models/v8/yolov8n.yaml
--rw-rw-rw-   0        0        0     1243 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/models/v8/yolov8s.yaml
--rw-rw-rw-   0        0        0     1239 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/models/v8/yolov8x.yaml
--rw-rw-rw-   0        0        0     1619 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/models/v8/yolov8x6.yaml
-drwxrwxrwx   0        0        0        0 2023-03-03 14:31:59.549047 syml_ultralytics-8.0.49/ultralytics/nn/
--rw-rw-rw-   0        0        0        0 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/nn/__init__.py
--rw-rw-rw-   0        0        0    23742 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/nn/autobackend.py
--rw-rw-rw-   0        0        0    12067 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/nn/autoshape.py
--rw-rw-rw-   0        0        0    19097 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/nn/modules.py
--rw-rw-rw-   0        0        0    24802 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/nn/tasks.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:31:59.551047 syml_ultralytics-8.0.49/ultralytics/tracker/
--rw-rw-rw-   0        0        0      207 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/tracker/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:31:59.552048 syml_ultralytics-8.0.49/ultralytics/tracker/cfg/
--rw-rw-rw-   0        0        0      907 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/tracker/cfg/botsort.yaml
--rw-rw-rw-   0        0        0      704 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/tracker/cfg/bytetrack.yaml
--rw-rw-rw-   0        0        0     1698 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/tracker/track.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:31:59.555045 syml_ultralytics-8.0.49/ultralytics/tracker/trackers/
--rw-rw-rw-   0        0        0      176 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/tracker/trackers/__init__.py
--rw-rw-rw-   0        0        0     1033 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/tracker/trackers/basetrack.py
--rw-rw-rw-   0        0        0     4801 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/tracker/trackers/bot_sort.py
--rw-rw-rw-   0        0        0    13019 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/tracker/trackers/byte_tracker.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:31:59.557048 syml_ultralytics-8.0.49/ultralytics/tracker/utils/
--rw-rw-rw-   0        0        0        0 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/tracker/utils/__init__.py
--rw-rw-rw-   0        0        0    12205 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/tracker/utils/gmc.py
--rw-rw-rw-   0        0        0    18679 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/tracker/utils/kalman_filter.py
--rw-rw-rw-   0        0        0     6925 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/tracker/utils/matching.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:31:59.558048 syml_ultralytics-8.0.49/ultralytics/yolo/
--rw-rw-rw-   0        0        0       98 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:31:59.559391 syml_ultralytics-8.0.49/ultralytics/yolo/cfg/
--rw-rw-rw-   0        0        0    15367 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/cfg/__init__.py
--rw-rw-rw-   0        0        0     6281 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/cfg/default.yaml
-drwxrwxrwx   0        0        0        0 2023-03-03 14:31:59.564694 syml_ultralytics-8.0.49/ultralytics/yolo/data/
--rw-rw-rw-   0        0        0      492 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/data/__init__.py
--rw-rw-rw-   0        0        0    31601 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/data/augment.py
--rw-rw-rw-   0        0        0     8958 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/data/base.py
--rw-rw-rw-   0        0        0     7874 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/data/build.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:31:59.567693 syml_ultralytics-8.0.49/ultralytics/yolo/data/dataloaders/
--rw-rw-rw-   0        0        0        0 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/data/dataloaders/__init__.py
--rw-rw-rw-   0        0        0    15068 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/data/dataloaders/stream_loaders.py
--rw-rw-rw-   0        0        0    17628 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/data/dataloaders/v5augmentations.py
--rw-rw-rw-   0        0        0    50919 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/data/dataloaders/v5loader.py
--rw-rw-rw-   0        0        0    12331 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/data/dataset.py
--rw-rw-rw-   0        0        0     1369 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/data/dataset_wrappers.py
--rw-rw-rw-   0        0        0    19870 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/data/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:31:59.573696 syml_ultralytics-8.0.49/ultralytics/yolo/engine/
--rw-rw-rw-   0        0        0        0 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/engine/__init__.py
--rw-rw-rw-   0        0        0    42707 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/engine/exporter.py
--rw-rw-rw-   0        0        0    15691 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/engine/model.py
--rw-rw-rw-   0        0        0    12489 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/engine/predictor.py
--rw-rw-rw-   0        0        0    14113 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/engine/results.py
--rw-rw-rw-   0        0        0    27666 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/engine/trainer.py
--rw-rw-rw-   0        0        0    10482 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/engine/validator.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:31:59.582696 syml_ultralytics-8.0.49/ultralytics/yolo/utils/
--rw-rw-rw-   0        0        0    22243 2023-03-03 14:05:53.000000 syml_ultralytics-8.0.49/ultralytics/yolo/utils/__init__.py
--rw-rw-rw-   0        0        0     3221 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/utils/autobatch.py
--rw-rw-rw-   0        0        0     5330 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/utils/benchmarks.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:31:59.586694 syml_ultralytics-8.0.49/ultralytics/yolo/utils/callbacks/
--rw-rw-rw-   0        0        0      126 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/utils/callbacks/__init__.py
--rw-rw-rw-   0        0        0     3594 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/utils/callbacks/base.py
--rw-rw-rw-   0        0        0     2193 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/utils/callbacks/clearml.py
--rw-rw-rw-   0        0        0     2096 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/utils/callbacks/comet.py
--rw-rw-rw-   0        0        0     3237 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/utils/callbacks/hub.py
--rw-rw-rw-   0        0        0     1112 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/utils/callbacks/tensorboard.py
--rw-rw-rw-   0        0        0    13558 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/utils/checks.py
--rw-rw-rw-   0        0        0     2476 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/utils/dist.py
--rw-rw-rw-   0        0        0     9747 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/utils/downloads.py
--rw-rw-rw-   0        0        0     3498 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/utils/files.py
--rw-rw-rw-   0        0        0    11715 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/utils/instance.py
--rw-rw-rw-   0        0        0     2317 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/utils/loss.py
--rw-rw-rw-   0        0        0    31915 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/utils/metrics.py
--rw-rw-rw-   0        0        0    29038 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/utils/ops.py
--rw-rw-rw-   0        0        0    17062 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/utils/plotting.py
--rw-rw-rw-   0        0        0    11583 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/utils/tal.py
--rw-rw-rw-   0        0        0    20325 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/utils/torch_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:31:59.587696 syml_ultralytics-8.0.49/ultralytics/yolo/v8/
--rw-rw-rw-   0        0        0      148 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/v8/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:31:59.590696 syml_ultralytics-8.0.49/ultralytics/yolo/v8/classify/
--rw-rw-rw-   0        0        0      397 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/v8/classify/__init__.py
--rw-rw-rw-   0        0        0     3257 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/v8/classify/predict.py
--rw-rw-rw-   0        0        0     6518 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/v8/classify/train.py
--rw-rw-rw-   0        0        0     2392 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/v8/classify/val.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:31:59.593699 syml_ultralytics-8.0.49/ultralytics/yolo/v8/detect/
--rw-rw-rw-   0        0        0      283 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/v8/detect/__init__.py
--rw-rw-rw-   0        0        0     4523 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/v8/detect/predict.py
--rw-rw-rw-   0        0        0    10376 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/v8/detect/train.py
--rw-rw-rw-   0        0        0    12131 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/v8/detect/val.py
-drwxrwxrwx   0        0        0        0 2023-03-03 14:31:59.596697 syml_ultralytics-8.0.49/ultralytics/yolo/v8/segment/
--rw-rw-rw-   0        0        0      301 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/v8/segment/__init__.py
--rw-rw-rw-   0        0        0     5550 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/v8/segment/predict.py
--rw-rw-rw-   0        0        0     7670 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/v8/segment/train.py
--rw-rw-rw-   0        0        0    12203 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.49/ultralytics/yolo/v8/segment/val.py
+drwxrwxrwx   0        0        0        0 2023-03-14 13:27:12.518577 syml_ultralytics-8.0.53/
+-rw-rw-rw-   0        0        0     5729 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.53/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    35823 2023-03-03 13:47:43.000000 syml_ultralytics-8.0.53/LICENSE
+-rw-rw-rw-   0        0        0      221 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/MANIFEST.in
+-rw-rw-rw-   0        0        0     1516 2023-03-14 13:27:12.518577 syml_ultralytics-8.0.53/PKG-INFO
+-rw-rw-rw-   0        0        0       81 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/README.md
+-rw-rw-rw-   0        0        0    20672 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/README.zh-CN.md
+-rw-rw-rw-   0        0        0     1122 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/requirements.txt
+-rw-rw-rw-   0        0        0      723 2023-03-14 13:27:12.521576 syml_ultralytics-8.0.53/setup.cfg
+-rw-rw-rw-   0        0        0     2743 2023-03-14 13:25:47.000000 syml_ultralytics-8.0.53/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-14 13:27:11.330381 syml_ultralytics-8.0.53/syml_ultralytics.egg-info/
+-rw-rw-rw-   0        0        0     1516 2023-03-14 13:27:11.000000 syml_ultralytics-8.0.53/syml_ultralytics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4716 2023-03-14 13:27:11.000000 syml_ultralytics-8.0.53/syml_ultralytics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-14 13:27:11.000000 syml_ultralytics-8.0.53/syml_ultralytics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2023-03-14 13:27:11.000000 syml_ultralytics-8.0.53/syml_ultralytics.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      413 2023-03-14 13:27:11.000000 syml_ultralytics-8.0.53/syml_ultralytics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-03-14 13:27:11.000000 syml_ultralytics-8.0.53/syml_ultralytics.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-03-14 13:27:11.331381 syml_ultralytics-8.0.53/ultralytics/
+-rw-rw-rw-   0        0        0      251 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-14 13:27:11.340382 syml_ultralytics-8.0.53/ultralytics/assets/
+-rw-rw-rw-   0        0        0   137419 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/assets/bus.jpg
+-rw-rw-rw-   0        0        0    50427 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/assets/zidane.jpg
+drwxrwxrwx   0        0        0        0 2023-03-14 13:27:11.426382 syml_ultralytics-8.0.53/ultralytics/datasets/
+-rw-rw-rw-   0        0        0     2823 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/datasets/Argoverse.yaml
+-rw-rw-rw-   0        0        0     1971 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/datasets/GlobalWheat2020.yaml
+-rw-rw-rw-   0        0        0    44463 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/datasets/ImageNet.yaml
+-rw-rw-rw-   0        0        0     9712 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/datasets/Objects365.yaml
+-rw-rw-rw-   0        0        0     2494 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/datasets/SKU-110K.yaml
+-rw-rw-rw-   0        0        0     3611 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/datasets/VOC.yaml
+-rw-rw-rw-   0        0        0     3086 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/datasets/VisDrone.yaml
+-rw-rw-rw-   0        0        0     2640 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/datasets/coco.yaml
+-rw-rw-rw-   0        0        0     1962 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/datasets/coco128-seg.yaml
+-rw-rw-rw-   0        0        0     1946 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/datasets/coco128.yaml
+-rw-rw-rw-   0        0        0     1897 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/datasets/coco8-seg.yaml
+-rw-rw-rw-   0        0        0     1877 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/datasets/coco8.yaml
+-rw-rw-rw-   0        0        0     5330 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/datasets/xView.yaml
+drwxrwxrwx   0        0        0        0 2023-03-14 13:27:11.458383 syml_ultralytics-8.0.53/ultralytics/hub/
+-rw-rw-rw-   0        0        0     3563 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/hub/__init__.py
+-rw-rw-rw-   0        0        0     2553 2023-03-03 15:05:02.000000 syml_ultralytics-8.0.53/ultralytics/hub/auth.py
+-rw-rw-rw-   0        0        0     5599 2023-03-03 15:05:02.000000 syml_ultralytics-8.0.53/ultralytics/hub/session.py
+-rw-rw-rw-   0        0        0     9639 2023-03-03 15:05:02.000000 syml_ultralytics-8.0.53/ultralytics/hub/utils - Copy.py
+-rw-rw-rw-   0        0        0     9639 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/hub/utils.py
+drwxrwxrwx   0        0        0        0 2023-03-14 13:27:11.262381 syml_ultralytics-8.0.53/ultralytics/models/
+drwxrwxrwx   0        0        0        0 2023-03-14 13:27:11.478383 syml_ultralytics-8.0.53/ultralytics/models/v3/
+-rw-rw-rw-   0        0        0     1481 2023-03-03 15:05:02.000000 syml_ultralytics-8.0.53/ultralytics/models/v3/yolov3-sppu.yaml
+-rw-rw-rw-   0        0        0     1173 2023-03-03 15:05:02.000000 syml_ultralytics-8.0.53/ultralytics/models/v3/yolov3-tinyu.yaml
+-rw-rw-rw-   0        0        0     1472 2023-03-03 15:05:02.000000 syml_ultralytics-8.0.53/ultralytics/models/v3/yolov3u.yaml
+drwxrwxrwx   0        0        0        0 2023-03-14 13:27:11.602383 syml_ultralytics-8.0.53/ultralytics/models/v5/
+-rw-rw-rw-   0        0        0     1690 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/models/v5/yolov5l6u.yaml
+-rw-rw-rw-   0        0        0     1312 2023-03-03 15:05:02.000000 syml_ultralytics-8.0.53/ultralytics/models/v5/yolov5lu.yaml
+-rw-rw-rw-   0        0        0     1692 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/models/v5/yolov5m6u.yaml
+-rw-rw-rw-   0        0        0     1314 2023-03-03 15:05:02.000000 syml_ultralytics-8.0.53/ultralytics/models/v5/yolov5mu.yaml
+-rw-rw-rw-   0        0        0     1692 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/models/v5/yolov5n6u.yaml
+-rw-rw-rw-   0        0        0     1314 2023-03-03 15:05:02.000000 syml_ultralytics-8.0.53/ultralytics/models/v5/yolov5nu.yaml
+-rw-rw-rw-   0        0        0     1692 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/models/v5/yolov5s6u.yaml
+-rw-rw-rw-   0        0        0     1314 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/models/v5/yolov5su.yaml
+-rw-rw-rw-   0        0        0     1692 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/models/v5/yolov5x6u.yaml
+-rw-rw-rw-   0        0        0     1314 2023-03-03 15:05:01.000000 syml_ultralytics-8.0.53/ultralytics/models/v5/yolov5xu.yaml
+drwxrwxrwx   0        0        0        0 2023-03-14 13:27:11.675385 syml_ultralytics-8.0.53/ultralytics/models/v8/
+drwxrwxrwx   0        0        0        0 2023-03-14 13:27:11.720385 syml_ultralytics-8.0.53/ultralytics/models/v8/cls/
+-rw-rw-rw-   0        0        0      652 2023-03-03 15:05:01.000000 syml_ultralytics-8.0.53/ultralytics/models/v8/cls/yolov8l-cls.yaml
+-rw-rw-rw-   0        0        0      652 2023-03-03 15:05:01.000000 syml_ultralytics-8.0.53/ultralytics/models/v8/cls/yolov8m-cls.yaml
+-rw-rw-rw-   0        0        0      652 2023-03-03 15:05:01.000000 syml_ultralytics-8.0.53/ultralytics/models/v8/cls/yolov8n-cls.yaml
+-rw-rw-rw-   0        0        0      652 2023-03-03 15:05:01.000000 syml_ultralytics-8.0.53/ultralytics/models/v8/cls/yolov8s-cls.yaml
+-rw-rw-rw-   0        0        0      652 2023-03-03 15:05:01.000000 syml_ultralytics-8.0.53/ultralytics/models/v8/cls/yolov8x-cls.yaml
+drwxrwxrwx   0        0        0        0 2023-03-14 13:27:11.771385 syml_ultralytics-8.0.53/ultralytics/models/v8/seg/
+-rw-rw-rw-   0        0        0     1249 2023-03-03 15:05:01.000000 syml_ultralytics-8.0.53/ultralytics/models/v8/seg/yolov8l-seg.yaml
+-rw-rw-rw-   0        0        0     1249 2023-03-03 15:05:01.000000 syml_ultralytics-8.0.53/ultralytics/models/v8/seg/yolov8m-seg.yaml
+-rw-rw-rw-   0        0        0     1253 2023-03-03 15:05:01.000000 syml_ultralytics-8.0.53/ultralytics/models/v8/seg/yolov8n-seg.yaml
+-rw-rw-rw-   0        0        0     1253 2023-03-03 15:05:01.000000 syml_ultralytics-8.0.53/ultralytics/models/v8/seg/yolov8s-seg.yaml
+-rw-rw-rw-   0        0        0     1249 2023-03-03 15:05:01.000000 syml_ultralytics-8.0.53/ultralytics/models/v8/seg/yolov8x-seg.yaml
+-rw-rw-rw-   0        0        0     1239 2023-03-03 15:05:01.000000 syml_ultralytics-8.0.53/ultralytics/models/v8/yolov8l.yaml
+-rw-rw-rw-   0        0        0     1239 2023-03-03 15:05:00.000000 syml_ultralytics-8.0.53/ultralytics/models/v8/yolov8m.yaml
+-rw-rw-rw-   0        0        0     1243 2023-03-03 15:05:00.000000 syml_ultralytics-8.0.53/ultralytics/models/v8/yolov8n.yaml
+-rw-rw-rw-   0        0        0     1243 2023-03-03 15:05:00.000000 syml_ultralytics-8.0.53/ultralytics/models/v8/yolov8s.yaml
+-rw-rw-rw-   0        0        0     1239 2023-03-03 15:05:00.000000 syml_ultralytics-8.0.53/ultralytics/models/v8/yolov8x.yaml
+-rw-rw-rw-   0        0        0     1619 2023-03-03 15:05:00.000000 syml_ultralytics-8.0.53/ultralytics/models/v8/yolov8x6.yaml
+drwxrwxrwx   0        0        0        0 2023-03-14 13:27:11.850387 syml_ultralytics-8.0.53/ultralytics/nn/
+-rw-rw-rw-   0        0        0        0 2023-03-03 15:05:00.000000 syml_ultralytics-8.0.53/ultralytics/nn/__init__.py
+-rw-rw-rw-   0        0        0    24271 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/nn/autobackend.py
+-rw-rw-rw-   0        0        0    12073 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/nn/autoshape.py
+-rw-rw-rw-   0        0        0    19104 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/nn/modules.py
+-rw-rw-rw-   0        0        0    24862 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/nn/tasks.py
+drwxrwxrwx   0        0        0        0 2023-03-14 13:27:11.880386 syml_ultralytics-8.0.53/ultralytics/tracker/
+-rw-rw-rw-   0        0        0      207 2023-03-03 15:05:00.000000 syml_ultralytics-8.0.53/ultralytics/tracker/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-14 13:27:11.904387 syml_ultralytics-8.0.53/ultralytics/tracker/cfg/
+-rw-rw-rw-   0        0        0      907 2023-03-03 15:05:00.000000 syml_ultralytics-8.0.53/ultralytics/tracker/cfg/botsort.yaml
+-rw-rw-rw-   0        0        0      704 2023-03-03 15:04:59.000000 syml_ultralytics-8.0.53/ultralytics/tracker/cfg/bytetrack.yaml
+-rw-rw-rw-   0        0        0     1698 2023-03-03 15:04:59.000000 syml_ultralytics-8.0.53/ultralytics/tracker/track.py
+drwxrwxrwx   0        0        0        0 2023-03-14 13:27:11.954414 syml_ultralytics-8.0.53/ultralytics/tracker/trackers/
+-rw-rw-rw-   0        0        0      176 2023-03-03 15:04:59.000000 syml_ultralytics-8.0.53/ultralytics/tracker/trackers/__init__.py
+-rw-rw-rw-   0        0        0     1033 2023-03-03 15:04:59.000000 syml_ultralytics-8.0.53/ultralytics/tracker/trackers/basetrack.py
+-rw-rw-rw-   0        0        0     4801 2023-03-03 15:04:59.000000 syml_ultralytics-8.0.53/ultralytics/tracker/trackers/bot_sort.py
+-rw-rw-rw-   0        0        0    13019 2023-03-03 15:04:59.000000 syml_ultralytics-8.0.53/ultralytics/tracker/trackers/byte_tracker.py
+drwxrwxrwx   0        0        0        0 2023-03-14 13:27:11.999408 syml_ultralytics-8.0.53/ultralytics/tracker/utils/
+-rw-rw-rw-   0        0        0        0 2023-03-03 15:04:59.000000 syml_ultralytics-8.0.53/ultralytics/tracker/utils/__init__.py
+-rw-rw-rw-   0        0        0    12205 2023-03-03 15:04:59.000000 syml_ultralytics-8.0.53/ultralytics/tracker/utils/gmc.py
+-rw-rw-rw-   0        0        0    18679 2023-03-03 15:04:59.000000 syml_ultralytics-8.0.53/ultralytics/tracker/utils/kalman_filter.py
+-rw-rw-rw-   0        0        0     7434 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/tracker/utils/matching.py
+drwxrwxrwx   0        0        0        0 2023-03-14 13:27:12.009404 syml_ultralytics-8.0.53/ultralytics/yolo/
+-rw-rw-rw-   0        0        0       98 2023-03-03 15:04:59.000000 syml_ultralytics-8.0.53/ultralytics/yolo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-14 13:27:12.033408 syml_ultralytics-8.0.53/ultralytics/yolo/cfg/
+-rw-rw-rw-   0        0        0    15577 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/yolo/cfg/__init__.py
+-rw-rw-rw-   0        0        0     6218 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/yolo/cfg/default.yaml
+drwxrwxrwx   0        0        0        0 2023-03-14 13:27:12.106406 syml_ultralytics-8.0.53/ultralytics/yolo/data/
+-rw-rw-rw-   0        0        0      492 2023-03-03 15:04:58.000000 syml_ultralytics-8.0.53/ultralytics/yolo/data/__init__.py
+-rw-rw-rw-   0        0        0    31673 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/yolo/data/augment.py
+-rw-rw-rw-   0        0        0     9044 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/yolo/data/base.py
+-rw-rw-rw-   0        0        0     8068 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/yolo/data/build.py
+drwxrwxrwx   0        0        0        0 2023-03-14 13:27:12.149406 syml_ultralytics-8.0.53/ultralytics/yolo/data/dataloaders/
+-rw-rw-rw-   0        0        0        0 2023-03-03 15:04:58.000000 syml_ultralytics-8.0.53/ultralytics/yolo/data/dataloaders/__init__.py
+-rw-rw-rw-   0        0        0    15491 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/yolo/data/dataloaders/stream_loaders.py
+-rw-rw-rw-   0        0        0    17628 2023-03-03 15:04:58.000000 syml_ultralytics-8.0.53/ultralytics/yolo/data/dataloaders/v5augmentations.py
+-rw-rw-rw-   0        0        0    50957 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/yolo/data/dataloaders/v5loader.py
+-rw-rw-rw-   0        0        0    12398 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/yolo/data/dataset.py
+-rw-rw-rw-   0        0        0     1369 2023-03-03 15:04:58.000000 syml_ultralytics-8.0.53/ultralytics/yolo/data/dataset_wrappers.py
+-rw-rw-rw-   0        0        0    19801 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/yolo/data/utils.py
+drwxrwxrwx   0        0        0        0 2023-03-14 13:27:12.211045 syml_ultralytics-8.0.53/ultralytics/yolo/engine/
+-rw-rw-rw-   0        0        0        0 2023-03-03 15:04:57.000000 syml_ultralytics-8.0.53/ultralytics/yolo/engine/__init__.py
+-rw-rw-rw-   0        0        0    42021 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/yolo/engine/exporter.py
+-rw-rw-rw-   0        0        0    15807 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/yolo/engine/model.py
+-rw-rw-rw-   0        0        0    12845 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/yolo/engine/predictor.py
+-rw-rw-rw-   0        0        0    14375 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/yolo/engine/results.py
+-rw-rw-rw-   0        0        0    30300 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/yolo/engine/trainer.py
+-rw-rw-rw-   0        0        0    10482 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/yolo/engine/validator.py
+drwxrwxrwx   0        0        0        0 2023-03-14 13:27:12.362577 syml_ultralytics-8.0.53/ultralytics/yolo/utils/
+-rw-rw-rw-   0        0        0    21916 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/yolo/utils/__init__.py
+-rw-rw-rw-   0        0        0     3221 2023-03-03 15:04:56.000000 syml_ultralytics-8.0.53/ultralytics/yolo/utils/autobatch.py
+-rw-rw-rw-   0        0        0     5530 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/yolo/utils/benchmarks.py
+drwxrwxrwx   0        0        0        0 2023-03-14 13:27:12.419575 syml_ultralytics-8.0.53/ultralytics/yolo/utils/callbacks/
+-rw-rw-rw-   0        0        0      126 2023-03-03 15:04:56.000000 syml_ultralytics-8.0.53/ultralytics/yolo/utils/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     3594 2023-03-03 15:04:56.000000 syml_ultralytics-8.0.53/ultralytics/yolo/utils/callbacks/base.py
+-rw-rw-rw-   0        0        0     2193 2023-03-03 15:04:56.000000 syml_ultralytics-8.0.53/ultralytics/yolo/utils/callbacks/clearml.py
+-rw-rw-rw-   0        0        0     2096 2023-03-03 15:04:56.000000 syml_ultralytics-8.0.53/ultralytics/yolo/utils/callbacks/comet.py
+-rw-rw-rw-   0        0        0     3237 2023-03-03 15:04:56.000000 syml_ultralytics-8.0.53/ultralytics/yolo/utils/callbacks/hub.py
+-rw-rw-rw-   0        0        0     1112 2023-03-03 15:04:56.000000 syml_ultralytics-8.0.53/ultralytics/yolo/utils/callbacks/tensorboard.py
+-rw-rw-rw-   0        0        0    13909 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/yolo/utils/checks.py
+-rw-rw-rw-   0        0        0     2476 2023-03-03 15:04:56.000000 syml_ultralytics-8.0.53/ultralytics/yolo/utils/dist.py
+-rw-rw-rw-   0        0        0     9747 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/yolo/utils/downloads.py
+-rw-rw-rw-   0        0        0     3498 2023-03-03 15:04:56.000000 syml_ultralytics-8.0.53/ultralytics/yolo/utils/files.py
+-rw-rw-rw-   0        0        0    11715 2023-03-03 15:04:55.000000 syml_ultralytics-8.0.53/ultralytics/yolo/utils/instance.py
+-rw-rw-rw-   0        0        0     2317 2023-03-03 15:04:55.000000 syml_ultralytics-8.0.53/ultralytics/yolo/utils/loss.py
+-rw-rw-rw-   0        0        0    31915 2023-03-03 15:04:55.000000 syml_ultralytics-8.0.53/ultralytics/yolo/utils/metrics.py
+-rw-rw-rw-   0        0        0    29038 2023-03-03 15:04:55.000000 syml_ultralytics-8.0.53/ultralytics/yolo/utils/ops.py
+-rw-rw-rw-   0        0        0    17093 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/yolo/utils/plotting.py
+-rw-rw-rw-   0        0        0    10455 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/yolo/utils/tal.py
+-rw-rw-rw-   0        0        0    20378 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/yolo/utils/torch_utils.py
+drwxrwxrwx   0        0        0        0 2023-03-14 13:27:12.424575 syml_ultralytics-8.0.53/ultralytics/yolo/v8/
+-rw-rw-rw-   0        0        0      148 2023-03-03 15:04:55.000000 syml_ultralytics-8.0.53/ultralytics/yolo/v8/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-14 13:27:12.454574 syml_ultralytics-8.0.53/ultralytics/yolo/v8/classify/
+-rw-rw-rw-   0        0        0      397 2023-03-03 15:04:55.000000 syml_ultralytics-8.0.53/ultralytics/yolo/v8/classify/__init__.py
+-rw-rw-rw-   0        0        0     3246 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/yolo/v8/classify/predict.py
+-rw-rw-rw-   0        0        0     6518 2023-03-03 15:04:55.000000 syml_ultralytics-8.0.53/ultralytics/yolo/v8/classify/train.py
+-rw-rw-rw-   0        0        0     2623 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/yolo/v8/classify/val.py
+drwxrwxrwx   0        0        0        0 2023-03-14 13:27:12.488575 syml_ultralytics-8.0.53/ultralytics/yolo/v8/detect/
+-rw-rw-rw-   0        0        0      283 2023-03-03 15:04:55.000000 syml_ultralytics-8.0.53/ultralytics/yolo/v8/detect/__init__.py
+-rw-rw-rw-   0        0        0     4557 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/yolo/v8/detect/predict.py
+-rw-rw-rw-   0        0        0    10064 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/yolo/v8/detect/train.py
+-rw-rw-rw-   0        0        0    12194 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/yolo/v8/detect/val.py
+drwxrwxrwx   0        0        0        0 2023-03-14 13:27:12.517577 syml_ultralytics-8.0.53/ultralytics/yolo/v8/segment/
+-rw-rw-rw-   0        0        0      301 2023-03-03 15:04:54.000000 syml_ultralytics-8.0.53/ultralytics/yolo/v8/segment/__init__.py
+-rw-rw-rw-   0        0        0     5646 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/yolo/v8/segment/predict.py
+-rw-rw-rw-   0        0        0     7670 2023-03-03 15:04:54.000000 syml_ultralytics-8.0.53/ultralytics/yolo/v8/segment/train.py
+-rw-rw-rw-   0        0        0    12266 2023-03-14 13:23:33.000000 syml_ultralytics-8.0.53/ultralytics/yolo/v8/segment/val.py
```

### Comparing `syml_ultralytics-8.0.49/CONTRIBUTING.md` & `syml_ultralytics-8.0.53/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/LICENSE` & `syml_ultralytics-8.0.53/LICENSE`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/PKG-INFO` & `syml_ultralytics-8.0.53/README.zh-CN.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,70 +1,32 @@
-Metadata-Version: 2.1
-Name: syml_ultralytics
-Version: 8.0.49
-Summary: Syml Ultralytics YOLOv8
-Home-page: 
-Download-URL: https://github.com/its-jd/syml_ultralytics/archive/refs/tags/8.0.49.tar.gz
-Author: syml_ultralytics
-License: GPL-3.0
-Keywords: machine-learning,deep-learning,vision,ML,DL,AI,YOLO,YOLOv3,YOLOv5,YOLOv8,HUB,Ultralytics
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Image Recognition
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: export
-Provides-Extra: tf
-License-File: LICENSE
-
 <div align="center">
   <p>
     <a href="https://ultralytics.com/yolov8" target="_blank">
-      <img width="100%" src="https://raw.githubusercontent.com/ultralytics/assets/main/yolov8/banner-yolov8.png"></a>
+      <img width="850" src="https://raw.githubusercontent.com/ultralytics/assets/main/yolov8/banner-yolov8.png"></a>
   </p>
 
 [English](README.md) | [简体中文](README.zh-CN.md)
 <br>
 
 <div>
     <a href="https://github.com/ultralytics/ultralytics/actions/workflows/ci.yaml"><img src="https://github.com/ultralytics/ultralytics/actions/workflows/ci.yaml/badge.svg" alt="Ultralytics CI"></a>
     <a href="https://zenodo.org/badge/latestdoi/264818686"><img src="https://zenodo.org/badge/264818686.svg" alt="YOLOv8 Citation"></a>
-    <a href="https://hub.docker.com/r/ultralytics/ultralytics"><img src="https://img.shields.io/docker/pulls/ultralytics/ultralytics?logo=docker" alt="Docker Pulls"></a>
+    <a href="https://hub.docker.com/r/ultralytics/yolov5"><img src="https://img.shields.io/docker/pulls/ultralytics/yolov5?logo=docker" alt="Docker Pulls"></a>
     <br>
     <a href="https://console.paperspace.com/github/ultralytics/ultralytics"><img src="https://assets.paperspace.io/img/gradient-badge.svg" alt="Run on Gradient"/></a>
     <a href="https://colab.research.google.com/github/ultralytics/ultralytics/blob/main/examples/tutorial.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a>
     <a href="https://www.kaggle.com/ultralytics/yolov8"><img src="https://kaggle.com/static/images/open-in-kaggle.svg" alt="Open In Kaggle"></a>
   </div>
   <br>
 
-[Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics), developed by [Ultralytics](https://ultralytics.com),
-is a cutting-edge, state-of-the-art (SOTA) model that builds upon the success of previous YOLO versions and introduces
-new features and improvements to further boost performance and flexibility. YOLOv8 is designed to be fast, accurate, and
-easy to use, making it an excellent choice for a wide range of object detection, image segmentation and image
-classification tasks.
-
-To request an Enterprise License please complete the form at [Ultralytics Licensing](https://ultralytics.com/license).
+[Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics) 是由 [Ultralytics](https://ultralytics.com) 开发的一个前沿的
+SOTA 模型。它在以前成功的 YOLO 版本基础上，引入了新的功能和改进，进一步提升了其性能和灵活性。YOLOv8
+基于快速、准确和易于使用的设计理念，使其成为广泛的目标检测、图像分割和图像分类任务的绝佳选择。
 
-<img width="100%" src="https://raw.githubusercontent.com/ultralytics/assets/main/yolov8/yolo-comparison-plots.png"></a>
+如果要申请企业许可证，请填写 [Ultralytics 许可](https://ultralytics.com/license)。
 
 <div align="center">
     <a href="https://github.com/ultralytics" style="text-decoration:none;">
       <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-github.png" width="2%" alt="" /></a>
     <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
     <a href="https://www.linkedin.com/company/ultralytics" style="text-decoration:none;">
       <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-linkedin.png" width="2%" alt="" /></a>
@@ -82,157 +44,142 @@
       <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-facebook.png" width="2%" alt="" /></a>
     <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
     <a href="https://www.instagram.com/ultralytics/" style="text-decoration:none;">
       <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-instagram.png" width="2%" alt="" /></a>
   </div>
 </div>
 
-## <div align="center">Documentation</div>
+## <div align="center">文档</div>
 
-See below for a quickstart installation and usage example, and see the [YOLOv8 Docs](https://docs.ultralytics.com) for
-full documentation on training, validation, prediction and deployment.
+有关训练、测试和部署的完整文档见[YOLOv8 Docs](https://docs.ultralytics.com)。请参阅下面的快速入门示例。
 
 <details open>
-<summary>Install</summary>
+<summary>安装</summary>
 
-Pip install the ultralytics package including
-all [requirements.txt](https://github.com/ultralytics/ultralytics/blob/main/requirements.txt) in a
-[**Python>=3.7**](https://www.python.org/) environment with
-[**PyTorch>=1.7**](https://pytorch.org/get-started/locally/).
+Pip 安装包含所有 [requirements.txt](https://github.com/ultralytics/ultralytics/blob/main/requirements.txt) 的
+ultralytics 包，环境要求 [**Python>=3.7**](https://www.python.org/)，且 [\*\*PyTorch>=1.7
+\*\*](https://pytorch.org/get-started/locally/)。
 
 ```bash
 pip install ultralytics
 ```
 
 </details>
 
 <details open>
-<summary>Usage</summary>
+<summary>使用方法</summary>
 
-#### CLI
-
-YOLOv8 may be used directly in the Command Line Interface (CLI) with a `yolo` command:
+YOLOv8 可以直接在命令行界面（CLI）中使用 `yolo` 命令运行：
 
 ```bash
 yolo predict model=yolov8n.pt source="https://ultralytics.com/images/bus.jpg"
 ```
 
-`yolo` can be used for a variety of tasks and modes and accepts additional arguments, i.e. `imgsz=640`. See the YOLOv8
-[CLI Docs](https://docs.ultralytics.com/cli) for examples.
+`yolo`可以用于各种任务和模式，并接受额外的参数，例如 `imgsz=640`。参见 YOLOv8 [文档](https://docs.ultralytics.com)
+中可用`yolo`[参数](https://docs.ultralytics.com/usage/cfg/)的完整列表。
 
-#### Python
+```bash
+yolo task=detect    mode=train    model=yolov8n.pt        args...
+          classify       predict        yolov8n-cls.yaml  args...
+          segment        val            yolov8n-seg.yaml  args...
+                         export         yolov8n.pt        format=onnx  args...
+```
 
-YOLOv8 may also be used directly in a Python environment, and accepts the
-same [arguments](https://docs.ultralytics.com/cfg/) as in the CLI example above:
+YOLOv8 也可以在 Python 环境中直接使用，并接受与上面 CLI 例子中相同的[参数](https://docs.ultralytics.com/usage/cfg/)：
 
 ```python
 from ultralytics import YOLO
 
-# Load a model
-model = YOLO("yolov8n.yaml")  # build a new model from scratch
-model = YOLO("yolov8n.pt")  # load a pretrained model (recommended for training)
+# 加载模型
+model = YOLO("yolov8n.yaml")  # 从头开始构建新模型
+model = YOLO("yolov8n.pt")  # 加载预训练模型（推荐用于训练）
 
 # Use the model
-model.train(data="coco128.yaml", epochs=3)  # train the model
-metrics = model.val()  # evaluate model performance on the validation set
-results = model("https://ultralytics.com/images/bus.jpg")  # predict on an image
-success = model.export(format="onnx")  # export the model to ONNX format
+results = model.train(data="coco128.yaml", epochs=3)  # 训练模型
+results = model.val()  # 在验证集上评估模型性能
+results = model("https://ultralytics.com/images/bus.jpg")  # 预测图像
+success = model.export(format="onnx")  # 将模型导出为 ONNX 格式
 ```
 
-[Models](https://github.com/ultralytics/ultralytics/tree/main/ultralytics/models) download automatically from the latest
-Ultralytics [release](https://github.com/ultralytics/assets/releases). See
-YOLOv8 [Python Docs](https://docs.ultralytics.com/python) for more examples.
-
-#### Model Architectures
-
-⭐ **NEW** YOLOv5u anchor free models are now available.
+[模型](https://github.com/ultralytics/ultralytics/tree/main/ultralytics/models) 会从
+Ultralytics [发布页](https://github.com/ultralytics/ultralytics/releases) 自动下载。
 
-All supported model architectures can be found in the [Models](./ultralytics/models/) section.
+### 已知问题 / 待办事项
 
-#### Known Issues / TODOs
+我们仍在努力完善 YOLOv8 的几个部分！我们的目标是尽快完成这些工作，使 YOLOv8 的功能设置达到YOLOv5
+的水平，包括对所有相同格式的导出和推理。我们还在写一篇 YOLOv8 的论文，一旦完成，我们将提交给 [arxiv.org](https://arxiv.org)。
 
-We are still working on several parts of YOLOv8! We aim to have these completed soon to bring the YOLOv8 feature set up
-to par with YOLOv5, including export and inference to all the same formats. We are also writing a YOLOv8 paper which we
-will submit to [arxiv.org](https://arxiv.org) once complete.
-
-- [x] TensorFlow exports
-- [x] DDP resume
-- [ ] [arxiv.org](https://arxiv.org) paper
+- [x] TensorFlow 导出
+- [x] DDP 恢复训练
+- [ ] [arxiv.org](https://arxiv.org) 论文
 
 </details>
 
-## <div align="center">Models</div>
+## <div align="center">模型</div>
 
-All YOLOv8 pretrained models are available here. Detection and Segmentation models are pretrained on the COCO dataset,
-while Classification models are pretrained on the ImageNet dataset.
+所有 YOLOv8 的预训练模型都可以在这里找到。目标检测和分割模型是在 COCO 数据集上预训练的，而分类模型是在 ImageNet 数据集上预训练的。
 
-[Models](https://github.com/ultralytics/ultralytics/tree/main/ultralytics/models) download automatically from the latest
-Ultralytics [release](https://github.com/ultralytics/assets/releases) on first use.
+第一次使用时，[模型](https://github.com/ultralytics/ultralytics/tree/main/ultralytics/models) 会从
+Ultralytics [发布页](https://github.com/ultralytics/ultralytics/releases) 自动下载。
 
-<details open><summary>Detection</summary>
-
-See [Detection Docs](https://docs.ultralytics.com/tasks/detection/) for usage examples with these models.
-
-| Model                                                                                | size<br><sup>(pixels) | mAP<sup>val<br>50-95 | Speed<br><sup>CPU ONNX<br>(ms) | Speed<br><sup>A100 TensorRT<br>(ms) | params<br><sup>(M) | FLOPs<br><sup>(B) |
-| ------------------------------------------------------------------------------------ | --------------------- | -------------------- | ------------------------------ | ----------------------------------- | ------------------ | ----------------- |
-| [YOLOv8n](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n.pt) | 640                   | 37.3                 | 80.4                           | 0.99                                | 3.2                | 8.7               |
-| [YOLOv8s](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s.pt) | 640                   | 44.9                 | 128.4                          | 1.20                                | 11.2               | 28.6              |
-| [YOLOv8m](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m.pt) | 640                   | 50.2                 | 234.7                          | 1.83                                | 25.9               | 78.9              |
-| [YOLOv8l](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8l.pt) | 640                   | 52.9                 | 375.2                          | 2.39                                | 43.7               | 165.2             |
-| [YOLOv8x](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x.pt) | 640                   | 53.9                 | 479.1                          | 3.53                                | 68.2               | 257.8             |
-
-- **mAP<sup>val</sup>** values are for single-model single-scale on [COCO val2017](http://cocodataset.org) dataset.
-  <br>Reproduce by `yolo val detect data=coco.yaml device=0`
-- **Speed** averaged over COCO val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/)
-  instance.
-  <br>Reproduce by `yolo val detect data=coco128.yaml batch=1 device=0/cpu`
+<details open><summary>目标检测</summary>
 
-</details>
+| 模型                                                                                   | 尺寸<br><sup>（像素） | mAP<sup>val<br>50-95 | 推理速度<br><sup>CPU ONNX<br>(ms) | 推理速度<br><sup>A100 TensorRT<br>(ms) | 参数量<br><sup>(M) | FLOPs<br><sup>(B) |
+| ------------------------------------------------------------------------------------ | --------------- | -------------------- | ----------------------------- | ---------------------------------- | --------------- | ----------------- |
+| [YOLOv8n](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n.pt) | 640             | 37.3                 | 80.4                          | 0.99                               | 3.2             | 8.7               |
+| [YOLOv8s](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s.pt) | 640             | 44.9                 | 128.4                         | 1.20                               | 11.2            | 28.6              |
+| [YOLOv8m](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m.pt) | 640             | 50.2                 | 234.7                         | 1.83                               | 25.9            | 78.9              |
+| [YOLOv8l](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8l.pt) | 640             | 52.9                 | 375.2                         | 2.39                               | 43.7            | 165.2             |
+| [YOLOv8x](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x.pt) | 640             | 53.9                 | 479.1                         | 3.53                               | 68.2            | 257.8             |
+
+- **mAP<sup>val</sup>** 结果都在 [COCO val2017](http://cocodataset.org) 数据集上，使用单模型单尺度测试得到。
+  <br>复现命令 `yolo val detect data=coco.yaml device=0`
+- **推理速度**使用 COCO
+  验证集图片推理时间进行平均得到，测试环境使用 [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/) 实例。
+  <br>复现命令 `yolo val detect data=coco128.yaml batch=1 device=0/cpu`
 
-<details><summary>Segmentation</summary>
+</details>
 
-See [Segmentation Docs](https://docs.ultralytics.com/tasks/segmentation/) for usage examples with these models.
+<details><summary>实例分割</summary>
 
-| Model                                                                                        | size<br><sup>(pixels) | mAP<sup>box<br>50-95 | mAP<sup>mask<br>50-95 | Speed<br><sup>CPU ONNX<br>(ms) | Speed<br><sup>A100 TensorRT<br>(ms) | params<br><sup>(M) | FLOPs<br><sup>(B) |
-| -------------------------------------------------------------------------------------------- | --------------------- | -------------------- | --------------------- | ------------------------------ | ----------------------------------- | ------------------ | ----------------- |
-| [YOLOv8n-seg](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n-seg.pt) | 640                   | 36.7                 | 30.5                  | 96.1                           | 1.21                                | 3.4                | 12.6              |
-| [YOLOv8s-seg](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s-seg.pt) | 640                   | 44.6                 | 36.8                  | 155.7                          | 1.47                                | 11.8               | 42.6              |
-| [YOLOv8m-seg](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m-seg.pt) | 640                   | 49.9                 | 40.8                  | 317.0                          | 2.18                                | 27.3               | 110.2             |
-| [YOLOv8l-seg](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8l-seg.pt) | 640                   | 52.3                 | 42.6                  | 572.4                          | 2.79                                | 46.0               | 220.5             |
-| [YOLOv8x-seg](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x-seg.pt) | 640                   | 53.4                 | 43.4                  | 712.1                          | 4.02                                | 71.8               | 344.1             |
-
-- **mAP<sup>val</sup>** values are for single-model single-scale on [COCO val2017](http://cocodataset.org) dataset.
-  <br>Reproduce by `yolo val segment data=coco.yaml device=0`
-- **Speed** averaged over COCO val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/)
-  instance.
-  <br>Reproduce by `yolo val segment data=coco128-seg.yaml batch=1 device=0/cpu`
+| 模型                                                                                           | 尺寸<br><sup>（像素） | mAP<sup>box<br>50-95 | mAP<sup>mask<br>50-95 | 推理速度<br><sup>CPU ONNX<br>(ms) | 推理速度<br><sup>A100 TensorRT<br>(ms) | 参数量<br><sup>(M) | FLOPs<br><sup>(B) |
+| -------------------------------------------------------------------------------------------- | --------------- | -------------------- | --------------------- | ----------------------------- | ---------------------------------- | --------------- | ----------------- |
+| [YOLOv8n-seg](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n-seg.pt) | 640             | 36.7                 | 30.5                  | 96.1                          | 1.21                               | 3.4             | 12.6              |
+| [YOLOv8s-seg](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s-seg.pt) | 640             | 44.6                 | 36.8                  | 155.7                         | 1.47                               | 11.8            | 42.6              |
+| [YOLOv8m-seg](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m-seg.pt) | 640             | 49.9                 | 40.8                  | 317.0                         | 2.18                               | 27.3            | 110.2             |
+| [YOLOv8l-seg](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8l-seg.pt) | 640             | 52.3                 | 42.6                  | 572.4                         | 2.79                               | 46.0            | 220.5             |
+| [YOLOv8x-seg](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x-seg.pt) | 640             | 53.4                 | 43.4                  | 712.1                         | 4.02                               | 71.8            | 344.1             |
+
+- **mAP<sup>val</sup>**  结果都在 [COCO val2017](http://cocodataset.org) 数据集上，使用单模型单尺度测试得到。
+  <br>复现命令 `yolo val segment data=coco.yaml device=0`
+- **推理速度**使用 COCO
+  验证集图片推理时间进行平均得到，测试环境使用 [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/) 实例。
+  <br>复现命令 `yolo val segment data=coco128-seg.yaml batch=1 device=0/cpu`
 
 </details>
 
-<details><summary>Classification</summary>
+<details><summary>分类</summary>
 
-See [Classification Docs](https://docs.ultralytics.com/tasks/classification/) for usage examples with these models.
-
-| Model                                                                                        | size<br><sup>(pixels) | acc<br><sup>top1 | acc<br><sup>top5 | Speed<br><sup>CPU ONNX<br>(ms) | Speed<br><sup>A100 TensorRT<br>(ms) | params<br><sup>(M) | FLOPs<br><sup>(B) at 640 |
-| -------------------------------------------------------------------------------------------- | --------------------- | ---------------- | ---------------- | ------------------------------ | ----------------------------------- | ------------------ | ------------------------ |
-| [YOLOv8n-cls](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n-cls.pt) | 224                   | 66.6             | 87.0             | 12.9                           | 0.31                                | 2.7                | 4.3                      |
-| [YOLOv8s-cls](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s-cls.pt) | 224                   | 72.3             | 91.1             | 23.4                           | 0.35                                | 6.4                | 13.5                     |
-| [YOLOv8m-cls](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m-cls.pt) | 224                   | 76.4             | 93.2             | 85.4                           | 0.62                                | 17.0               | 42.7                     |
-| [YOLOv8l-cls](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8l-cls.pt) | 224                   | 78.0             | 94.1             | 163.0                          | 0.87                                | 37.5               | 99.7                     |
-| [YOLOv8x-cls](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x-cls.pt) | 224                   | 78.4             | 94.3             | 232.0                          | 1.01                                | 57.4               | 154.8                    |
-
-- **acc** values are model accuracies on the [ImageNet](https://www.image-net.org/) dataset validation set.
-  <br>Reproduce by `yolo val classify data=path/to/ImageNet device=0`
-- **Speed** averaged over ImageNet val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/)
-  instance.
-  <br>Reproduce by `yolo val classify data=path/to/ImageNet batch=1 device=0/cpu`
+| 模型                                                                                           | 尺寸<br><sup>（像素） | acc<br><sup>top1 | acc<br><sup>top5 | 推理速度<br><sup>CPU ONNX<br>(ms) | 推理速度<br><sup>A100 TensorRT<br>(ms) | 参数量<br><sup>(M) | FLOPs<br><sup>(B) at 640 |
+| -------------------------------------------------------------------------------------------- | --------------- | ---------------- | ---------------- | ----------------------------- | ---------------------------------- | --------------- | ------------------------ |
+| [YOLOv8n-cls](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n-cls.pt) | 224             | 66.6             | 87.0             | 12.9                          | 0.31                               | 2.7             | 4.3                      |
+| [YOLOv8s-cls](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s-cls.pt) | 224             | 72.3             | 91.1             | 23.4                          | 0.35                               | 6.4             | 13.5                     |
+| [YOLOv8m-cls](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m-cls.pt) | 224             | 76.4             | 93.2             | 85.4                          | 0.62                               | 17.0            | 42.7                     |
+| [YOLOv8l-cls](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8l-cls.pt) | 224             | 78.0             | 94.1             | 163.0                         | 0.87                               | 37.5            | 99.7                     |
+| [YOLOv8x-cls](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x-cls.pt) | 224             | 78.4             | 94.3             | 232.0                         | 1.01                               | 57.4            | 154.8                    |
+
+- **acc** 都在 [ImageNet](https://www.image-net.org/) 数据集上，使用单模型单尺度测试得到。
+  <br>复现命令 `yolo val classify data=path/to/ImageNet device=0`
+- **推理速度**使用 ImageNet
+  验证集图片推理时间进行平均得到，测试环境使用 [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/) 实例。
+  <br>复现命令 `yolo val classify data=path/to/ImageNet batch=1 device=0/cpu`
 
 </details>
 
-## <div align="center">Integrations</div>
+## <div align="center">模块集成</div>
 
 <br>
 <a href="https://bit.ly/ultralytics_hub" target="_blank">
 <img width="100%" src="https://github.com/ultralytics/assets/raw/main/yolov8/banner-integrations.png"></a>
 <br>
 <br>
 
@@ -246,54 +193,50 @@
   <a href="https://bit.ly/yolov5-readme-comet2">
     <img src="https://github.com/ultralytics/assets/raw/main/partners/logo-comet.png" width="10%" /></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="15%" height="0" alt="" />
   <a href="https://bit.ly/yolov5-neuralmagic">
     <img src="https://github.com/ultralytics/assets/raw/main/partners/logo-neuralmagic.png" width="10%" /></a>
 </div>
 
-|                                                           Roboflow                                                           |                                                            ClearML ⭐ NEW                                                            |                                                                        Comet ⭐ NEW                                                                         |                                           Neural Magic ⭐ NEW                                           |
-| :--------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------: |
-| Label and export your custom datasets directly to YOLOv8 for training with [Roboflow](https://roboflow.com/?ref=ultralytics) | Automatically track, visualize and even remotely train YOLOv8 using [ClearML](https://cutt.ly/yolov5-readme-clearml) (open-source!) | Free forever, [Comet](https://bit.ly/yolov5-readme-comet2) lets you save YOLOv8 models, resume training, and interactively visualize and debug predictions | Run YOLOv8 inference up to 6x faster with [Neural Magic DeepSparse](https://bit.ly/yolov5-neuralmagic) |
+|                                      Roboflow                                      |                                 ClearML ⭐ 新                                 |                                     Comet ⭐ 新                                      |                                    Neural Magic ⭐ 新                                    |
+| :--------------------------------------------------------------------------------: | :-------------------------------------------------------------------------: | :--------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------: |
+| 将您的自定义数据集进行标注并直接导出到 YOLOv8 以进行训练 [Roboflow](https://roboflow.com/?ref=ultralytics) | 自动跟踪、可视化甚至远程训练 YOLOv8 [ClearML](https://cutt.ly/yolov5-readme-clearml)（开源！） | 永远免费，[Comet](https://bit.ly/yolov5-readme-comet2)可让您保存 YOLOv8 模型、恢复训练以及交互式可视化和调试预测 | 使用 [Neural Magic DeepSparse](https://bit.ly/yolov5-neuralmagic)，运行 YOLOv8 推理的速度最高可提高6倍 |
 
 ## <div align="center">Ultralytics HUB</div>
 
-Experience seamless AI with [Ultralytics HUB](https://bit.ly/ultralytics_hub) ⭐, the all-in-one solution for data
-visualization, YOLOv5 and YOLOv8 (coming soon) 🚀 model training and deployment, without any coding. Transform images
-into actionable insights and bring your AI visions to life with ease using our cutting-edge platform and
-user-friendly [Ultralytics App](https://ultralytics.com/app_install). Start your journey for **Free** now!
+[Ultralytics HUB](https://bit.ly/ultralytics_hub) 是我们⭐ **新**的无代码解决方案，用于可视化数据集，训练 YOLOv8🚀
+模型，并以无缝体验方式部署到现实世界。现在开始**免费**!
+还可以通过下载 [Ultralytics App](https://ultralytics.com/app_install) 在你的 iOS 或 Android 设备上运行 YOLOv8 模型!
 
 <a href="https://bit.ly/ultralytics_hub" target="_blank">
 <img width="100%" src="https://github.com/ultralytics/assets/raw/main/im/ultralytics-hub.png"></a>
 
-## <div align="center">Contribute</div>
+## <div align="center">贡献</div>
 
-We love your input! YOLOv5 and YOLOv8 would not be possible without help from our community. Please see
-our [Contributing Guide](CONTRIBUTING.md) to get started, and fill out
-our [Survey](https://ultralytics.com/survey?utm_source=github&utm_medium=social&utm_campaign=Survey) to send us feedback
-on your experience. Thank you 🙏 to all our contributors!
+我们喜欢您的意见或建议！我们希望尽可能简单和透明地为 YOLOv8 做出贡献。请看我们的 [贡献指南](CONTRIBUTING.md)
+，并填写 [调查问卷](https://ultralytics.com/survey?utm_source=github&utm_medium=social&utm_campaign=Survey)
+向我们发送您的体验反馈。感谢我们所有的贡献者！
 
 <!-- SVG image from https://opencollective.com/ultralytics/contributors.svg?width=990 -->
 
 <a href="https://github.com/ultralytics/yolov5/graphs/contributors">
-<img src="https://github.com/ultralytics/assets/raw/main/im/image-contributors.png" /></a>
+<img width="100%" src="https://github.com/ultralytics/assets/raw/main/im/image-contributors.png"></a>
 
 ## <div align="center">License</div>
 
-YOLOv8 is available under two different licenses:
+YOLOv8 在两种不同的 License 下可用：
+
+- **GPL-3.0 License**： 查看 [License](https://github.com/ultralytics/ultralytics/blob/main/LICENSE) 文件的详细信息。
+- **企业License**：在没有 GPL-3.0 开源要求的情况下为商业产品开发提供更大的灵活性。典型用例是将 Ultralytics 软件和 AI
+  模型嵌入到商业产品和应用程序中。在以下位置申请企业许可证 [Ultralytics 许可](https://ultralytics.com/license) 。
+
+## <div align="center">联系我们</div>
 
-- **GPL-3.0 License**: See [LICENSE](https://github.com/ultralytics/ultralytics/blob/main/LICENSE) file for details.
-- **Enterprise License**: Provides greater flexibility for commercial product development without the open-source
-  requirements of GPL-3.0. Typical use cases are embedding Ultralytics software and AI models in commercial products and
-  applications. Request an Enterprise License at [Ultralytics Licensing](https://ultralytics.com/license).
-
-## <div align="center">Contact</div>
-
-For YOLOv8 bug reports and feature requests please
-visit [GitHub Issues](https://github.com/ultralytics/ultralytics/issues) or
-the [Ultralytics Community Forum](https://community.ultralytics.com/).
+请访问 [GitHub Issues](https://github.com/ultralytics/ultralytics/issues)
+或 [Ultralytics Community Forum](https://community.ultralytis.com) 以报告 YOLOv8 错误和请求功能。
 
 <br>
 <div align="center">
   <a href="https://github.com/ultralytics" style="text-decoration:none;">
     <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-github.png" width="3%" alt="" /></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="" />
   <a href="https://www.linkedin.com/company/ultralytics" style="text-decoration:none;">
```

#### html2text {}

```diff
@@ -1,213 +1,189 @@
-Metadata-Version: 2.1 Name: syml_ultralytics Version: 8.0.49 Summary: Syml
-Ultralytics YOLOv8 Home-page: Download-URL: https://github.com/its-jd/
-syml_ultralytics/archive/refs/tags/8.0.49.tar.gz Author: syml_ultralytics
-License: GPL-3.0 Keywords: machine-learning,deep-
-learning,vision,ML,DL,AI,YOLO,YOLOv3,YOLOv5,YOLOv8,HUB,Ultralytics Classifier:
-Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education Classifier: Intended Audience ::
-Science/Research Classifier: License :: OSI Approved :: GNU General Public
-License v3 (GPLv3) Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Topic :: Software Development Classifier: Topic ::
-Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
-Artificial Intelligence Classifier: Topic :: Scientific/Engineering :: Image
-Recognition Classifier: Operating System :: POSIX :: Linux Classifier:
-Operating System :: MacOS Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra:
-dev Provides-Extra: export Provides-Extra: tf License-File: LICENSE
    [https://raw.githubusercontent.com/ultralytics/assets/main/yolov8/banner-
                                   yolov8.png]
             [English](README.md) | [ç®ä½ä¸­æ](README.zh-CN.md)
               [Ultralytics_CI] [YOLOv8_Citation] [Docker_Pulls]
               [Run_on_Gradient] [Open_In_Colab] [Open_In_Kaggle]
 
-[Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics), developed by
- [Ultralytics](https://ultralytics.com), is a cutting-edge, state-of-the-art
-    (SOTA) model that builds upon the success of previous YOLO versions and
-   introduces new features and improvements to further boost performance and
- flexibility. YOLOv8 is designed to be fast, accurate, and easy to use, making
-it an excellent choice for a wide range of object detection, image segmentation
-    and image classification tasks. To request an Enterprise License please
-complete the form at [Ultralytics Licensing](https://ultralytics.com/license).
-    [https://raw.githubusercontent.com/ultralytics/assets/main/yolov8/yolo-
-                             comparison-plots.png]
+   [Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics) æ¯ç±
+     [Ultralytics](https://ultralytics.com) å¼åçä¸ä¸ªåæ²¿ç SOTA
+                      æ¨¡åãå®å¨ä»¥åæåç YOLO
+çæ¬åºç¡ä¸ï¼å¼å¥äºæ°çåè½åæ¹è¿ï¼è¿ä¸æ­¥æåäºå¶æ§è½åçµæ´»æ§ãYOLOv8
+åºäºå¿«éãåç¡®åæäºä½¿ç¨çè®¾è®¡çå¿µï¼ä½¿å¶æä¸ºå¹¿æ³çç®æ æ£æµãå¾ååå²åå¾ååç±»ä»»å¡çç»ä½³éæ©ã
+   å¦æè¦ç³è¯·ä¼ä¸è®¸å¯è¯ï¼è¯·å¡«å [Ultralytics è®¸å¯](https://
+                          ultralytics.com/license)ã
 
 ##
-                                 Documentation
-See below for a quickstart installation and usage example, and see the [YOLOv8
-Docs](https://docs.ultralytics.com) for full documentation on training,
-validation, prediction and deployment.  Install Pip install the ultralytics
-package including all [requirements.txt](https://github.com/ultralytics/
-ultralytics/blob/main/requirements.txt) in a [**Python>=3.7**](https://
-www.python.org/) environment with [**PyTorch>=1.7**](https://pytorch.org/get-
-started/locally/). ```bash pip install ultralytics ```   Usage #### CLI YOLOv8
-may be used directly in the Command Line Interface (CLI) with a `yolo` command:
-```bash yolo predict model=yolov8n.pt source="https://ultralytics.com/images/
-bus.jpg" ``` `yolo` can be used for a variety of tasks and modes and accepts
-additional arguments, i.e. `imgsz=640`. See the YOLOv8 [CLI Docs](https://
-docs.ultralytics.com/cli) for examples. #### Python YOLOv8 may also be used
-directly in a Python environment, and accepts the same [arguments](https://
-docs.ultralytics.com/cfg/) as in the CLI example above: ```python from
-ultralytics import YOLO # Load a model model = YOLO("yolov8n.yaml") # build a
-new model from scratch model = YOLO("yolov8n.pt") # load a pretrained model
-(recommended for training) # Use the model model.train(data="coco128.yaml",
-epochs=3) # train the model metrics = model.val() # evaluate model performance
-on the validation set results = model("https://ultralytics.com/images/bus.jpg")
-# predict on an image success = model.export(format="onnx") # export the model
-to ONNX format ``` [Models](https://github.com/ultralytics/ultralytics/tree/
-main/ultralytics/models) download automatically from the latest Ultralytics
-[release](https://github.com/ultralytics/assets/releases). See YOLOv8 [Python
-Docs](https://docs.ultralytics.com/python) for more examples. #### Model
-Architectures â­ **NEW** YOLOv5u anchor free models are now available. All
-supported model architectures can be found in the [Models](./ultralytics/
-models/) section. #### Known Issues / TODOs We are still working on several
-parts of YOLOv8! We aim to have these completed soon to bring the YOLOv8
-feature set up to par with YOLOv5, including export and inference to all the
-same formats. We are also writing a YOLOv8 paper which we will submit to
-[arxiv.org](https://arxiv.org) once complete. - [x] TensorFlow exports - [x]
-DDP resume - [ ] [arxiv.org](https://arxiv.org) paper  ##
-                                    Models
-All YOLOv8 pretrained models are available here. Detection and Segmentation
-models are pretrained on the COCO dataset, while Classification models are
-pretrained on the ImageNet dataset. [Models](https://github.com/ultralytics/
-ultralytics/tree/main/ultralytics/models) download automatically from the
-latest Ultralytics [release](https://github.com/ultralytics/assets/releases) on
-first use. Detection See [Detection Docs](https://docs.ultralytics.com/tasks/
-detection/) for usage examples with these models. | Model | size
-(pixels) | mAPval
-50-95 | Speed
+                                    ææ¡£
+æå³è®­ç»ãæµè¯åé¨ç½²çå®æ´ææ¡£è§[YOLOv8 Docs](https://
+docs.ultralytics.com)ãè¯·åéä¸é¢çå¿«éå¥é¨ç¤ºä¾ã  å®è£ Pip
+å®è£åå«ææ [requirements.txt](https://github.com/ultralytics/
+ultralytics/blob/main/requirements.txt) ç ultralytics åï¼ç¯å¢è¦æ±
+[**Python>=3.7**](https://www.python.org/)ï¼ä¸ [\*\*PyTorch>=1.7 \*\*](https:
+//pytorch.org/get-started/locally/)ã ```bash pip install ultralytics ```
+ä½¿ç¨æ¹æ³ YOLOv8 å¯ä»¥ç´æ¥å¨å½ä»¤è¡çé¢ï¼CLIï¼ä¸­ä½¿ç¨ `yolo`
+å½ä»¤è¿è¡ï¼ ```bash yolo predict model=yolov8n.pt source="https://
+ultralytics.com/images/bus.jpg" ```
+`yolo`å¯ä»¥ç¨äºåç§ä»»å¡åæ¨¡å¼ï¼å¹¶æ¥åé¢å¤çåæ°ï¼ä¾å¦
+`imgsz=640`ãåè§ YOLOv8 [ææ¡£](https://docs.ultralytics.com)
+ä¸­å¯ç¨`yolo`[åæ°](https://docs.ultralytics.com/usage/cfg/
+)çå®æ´åè¡¨ã ```bash yolo task=detect mode=train model=yolov8n.pt
+args... classify predict yolov8n-cls.yaml args... segment val yolov8n-seg.yaml
+args... export yolov8n.pt format=onnx args... ``` YOLOv8 ä¹å¯ä»¥å¨ Python
+ç¯å¢ä¸­ç´æ¥ä½¿ç¨ï¼å¹¶æ¥åä¸ä¸é¢ CLI ä¾å­ä¸­ç¸åç[åæ°]
+(https://docs.ultralytics.com/usage/cfg/)ï¼ ```python from ultralytics import
+YOLO # å è½½æ¨¡å model = YOLO("yolov8n.yaml") # ä»å¤´å¼å§æå»ºæ°æ¨¡å
+model = YOLO("yolov8n.pt") # å è½½é¢è®­ç»æ¨¡åï¼æ¨èç¨äºè®­ç»ï¼ #
+Use the model results = model.train(data="coco128.yaml", epochs=3) #
+è®­ç»æ¨¡å results = model.val() # å¨éªè¯éä¸è¯ä¼°æ¨¡åæ§è½ results
+= model("https://ultralytics.com/images/bus.jpg") # é¢æµå¾å success =
+model.export(format="onnx") # å°æ¨¡åå¯¼åºä¸º ONNX æ ¼å¼ ``` [æ¨¡å]
+(https://github.com/ultralytics/ultralytics/tree/main/ultralytics/models)
+ä¼ä» Ultralytics [åå¸é¡µ](https://github.com/ultralytics/ultralytics/
+releases) èªå¨ä¸è½½ã ### å·²ç¥é®é¢ / å¾åäºé¡¹
+æä»¬ä»å¨åªåå®å YOLOv8
+çå ä¸ªé¨åï¼æä»¬çç®æ æ¯å°½å¿«å®æè¿äºå·¥ä½ï¼ä½¿ YOLOv8
+çåè½è®¾ç½®è¾¾å°YOLOv5
+çæ°´å¹³ï¼åæ¬å¯¹ææç¸åæ ¼å¼çå¯¼åºåæ¨çãæä»¬è¿å¨åä¸ç¯
+YOLOv8 çè®ºæï¼ä¸æ¦å®æï¼æä»¬å°æäº¤ç» [arxiv.org](https://
+arxiv.org)ã - [x] TensorFlow å¯¼åº - [x] DDP æ¢å¤è®­ç» - [ ] [arxiv.org]
+(https://arxiv.org) è®ºæ  ##
+                                    æ¨¡å
+ææ YOLOv8
+çé¢è®­ç»æ¨¡åé½å¯ä»¥å¨è¿éæ¾å°ãç®æ æ£æµååå²æ¨¡åæ¯å¨
+COCO æ°æ®éä¸é¢è®­ç»çï¼èåç±»æ¨¡åæ¯å¨ ImageNet
+æ°æ®éä¸é¢è®­ç»çã ç¬¬ä¸æ¬¡ä½¿ç¨æ¶ï¼[æ¨¡å](https://github.com/
+ultralytics/ultralytics/tree/main/ultralytics/models) ä¼ä» Ultralytics
+[åå¸é¡µ](https://github.com/ultralytics/ultralytics/releases)
+èªå¨ä¸è½½ã ç®æ æ£æµ | æ¨¡å | å°ºå¯¸
+ï¼åç´ ï¼ | mAPval
+50-95 | æ¨çéåº¦
 CPU ONNX
-(ms) | Speed
+(ms) | æ¨çéåº¦
 A100 TensorRT
-(ms) | params
+(ms) | åæ°é
 (M) | FLOPs
 (B) | | -----------------------------------------------------------------------
-------------- | --------------------- | -------------------- | ----------------
--------------- | ----------------------------------- | ------------------ | ---
--------------- | | [YOLOv8n](https://github.com/ultralytics/assets/releases/
-download/v0.0.0/yolov8n.pt) | 640 | 37.3 | 80.4 | 0.99 | 3.2 | 8.7 | |
-[YOLOv8s](https://github.com/ultralytics/assets/releases/download/v0.0.0/
-yolov8s.pt) | 640 | 44.9 | 128.4 | 1.20 | 11.2 | 28.6 | | [YOLOv8m](https://
-github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m.pt) | 640 | 50.2
-| 234.7 | 1.83 | 25.9 | 78.9 | | [YOLOv8l](https://github.com/ultralytics/
-assets/releases/download/v0.0.0/yolov8l.pt) | 640 | 52.9 | 375.2 | 2.39 | 43.7
-| 165.2 | | [YOLOv8x](https://github.com/ultralytics/assets/releases/download/
-v0.0.0/yolov8x.pt) | 640 | 53.9 | 479.1 | 3.53 | 68.2 | 257.8 | - **mAPval**
-values are for single-model single-scale on [COCO val2017](http://
-cocodataset.org) dataset.
-Reproduce by `yolo val detect data=coco.yaml device=0` - **Speed** averaged
-over COCO val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/
-instance-types/p4/) instance.
-Reproduce by `yolo val detect data=coco128.yaml batch=1 device=0/cpu`
-Segmentation See [Segmentation Docs](https://docs.ultralytics.com/tasks/
-segmentation/) for usage examples with these models. | Model | size
-(pixels) | mAPbox
+------------- | --------------- | -------------------- | ----------------------
+------- | ---------------------------------- | --------------- | --------------
+--- | | [YOLOv8n](https://github.com/ultralytics/assets/releases/download/
+v0.0.0/yolov8n.pt) | 640 | 37.3 | 80.4 | 0.99 | 3.2 | 8.7 | | [YOLOv8s](https:/
+/github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s.pt) | 640 |
+44.9 | 128.4 | 1.20 | 11.2 | 28.6 | | [YOLOv8m](https://github.com/ultralytics/
+assets/releases/download/v0.0.0/yolov8m.pt) | 640 | 50.2 | 234.7 | 1.83 | 25.9
+| 78.9 | | [YOLOv8l](https://github.com/ultralytics/assets/releases/download/
+v0.0.0/yolov8l.pt) | 640 | 52.9 | 375.2 | 2.39 | 43.7 | 165.2 | | [YOLOv8x]
+(https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x.pt) |
+640 | 53.9 | 479.1 | 3.53 | 68.2 | 257.8 | - **mAPval** ç»æé½å¨ [COCO
+val2017](http://cocodataset.org)
+æ°æ®éä¸ï¼ä½¿ç¨åæ¨¡ååå°ºåº¦æµè¯å¾å°ã
+å¤ç°å½ä»¤ `yolo val detect data=coco.yaml device=0` - **æ¨çéåº¦**ä½¿ç¨
+COCO éªè¯éå¾çæ¨çæ¶é´è¿è¡å¹³åå¾å°ï¼æµè¯ç¯å¢ä½¿ç¨ [Amazon
+EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/) å®ä¾ã
+å¤ç°å½ä»¤ `yolo val detect data=coco128.yaml batch=1 device=0/cpu`
+å®ä¾åå² | æ¨¡å | å°ºå¯¸
+ï¼åç´ ï¼ | mAPbox
 50-95 | mAPmask
-50-95 | Speed
+50-95 | æ¨çéåº¦
 CPU ONNX
-(ms) | Speed
+(ms) | æ¨çéåº¦
 A100 TensorRT
-(ms) | params
+(ms) | åæ°é
 (M) | FLOPs
 (B) | | -----------------------------------------------------------------------
---------------------- | --------------------- | -------------------- | --------
-------------- | ------------------------------ | ------------------------------
------ | ------------------ | ----------------- | | [YOLOv8n-seg](https://
-github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n-seg.pt) | 640 |
-36.7 | 30.5 | 96.1 | 1.21 | 3.4 | 12.6 | | [YOLOv8s-seg](https://github.com/
-ultralytics/assets/releases/download/v0.0.0/yolov8s-seg.pt) | 640 | 44.6 | 36.8
-| 155.7 | 1.47 | 11.8 | 42.6 | | [YOLOv8m-seg](https://github.com/ultralytics/
-assets/releases/download/v0.0.0/yolov8m-seg.pt) | 640 | 49.9 | 40.8 | 317.0 |
-2.18 | 27.3 | 110.2 | | [YOLOv8l-seg](https://github.com/ultralytics/assets/
-releases/download/v0.0.0/yolov8l-seg.pt) | 640 | 52.3 | 42.6 | 572.4 | 2.79 |
-46.0 | 220.5 | | [YOLOv8x-seg](https://github.com/ultralytics/assets/releases/
+--------------------- | --------------- | -------------------- | --------------
+------- | ----------------------------- | ---------------------------------- |
+--------------- | ----------------- | | [YOLOv8n-seg](https://github.com/
+ultralytics/assets/releases/download/v0.0.0/yolov8n-seg.pt) | 640 | 36.7 | 30.5
+| 96.1 | 1.21 | 3.4 | 12.6 | | [YOLOv8s-seg](https://github.com/ultralytics/
+assets/releases/download/v0.0.0/yolov8s-seg.pt) | 640 | 44.6 | 36.8 | 155.7 |
+1.47 | 11.8 | 42.6 | | [YOLOv8m-seg](https://github.com/ultralytics/assets/
+releases/download/v0.0.0/yolov8m-seg.pt) | 640 | 49.9 | 40.8 | 317.0 | 2.18 |
+27.3 | 110.2 | | [YOLOv8l-seg](https://github.com/ultralytics/assets/releases/
+download/v0.0.0/yolov8l-seg.pt) | 640 | 52.3 | 42.6 | 572.4 | 2.79 | 46.0 |
+220.5 | | [YOLOv8x-seg](https://github.com/ultralytics/assets/releases/
 download/v0.0.0/yolov8x-seg.pt) | 640 | 53.4 | 43.4 | 712.1 | 4.02 | 71.8 |
-344.1 | - **mAPval** values are for single-model single-scale on [COCO val2017]
-(http://cocodataset.org) dataset.
-Reproduce by `yolo val segment data=coco.yaml device=0` - **Speed** averaged
-over COCO val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/
-instance-types/p4/) instance.
-Reproduce by `yolo val segment data=coco128-seg.yaml batch=1 device=0/cpu`
-Classification See [Classification Docs](https://docs.ultralytics.com/tasks/
-classification/) for usage examples with these models. | Model | size
-(pixels) | acc
+344.1 | - **mAPval** ç»æé½å¨ [COCO val2017](http://cocodataset.org)
+æ°æ®éä¸ï¼ä½¿ç¨åæ¨¡ååå°ºåº¦æµè¯å¾å°ã
+å¤ç°å½ä»¤ `yolo val segment data=coco.yaml device=0` -
+**æ¨çéåº¦**ä½¿ç¨ COCO
+éªè¯éå¾çæ¨çæ¶é´è¿è¡å¹³åå¾å°ï¼æµè¯ç¯å¢ä½¿ç¨ [Amazon EC2
+P4d](https://aws.amazon.com/ec2/instance-types/p4/) å®ä¾ã
+å¤ç°å½ä»¤ `yolo val segment data=coco128-seg.yaml batch=1 device=0/cpu`
+åç±» | æ¨¡å | å°ºå¯¸
+ï¼åç´ ï¼ | acc
 top1 | acc
-top5 | Speed
+top5 | æ¨çéåº¦
 CPU ONNX
-(ms) | Speed
+(ms) | æ¨çéåº¦
 A100 TensorRT
-(ms) | params
+(ms) | åæ°é
 (M) | FLOPs
 (B) at 640 | | ----------------------------------------------------------------
----------------------------- | --------------------- | ---------------- | -----
------------ | ------------------------------ | --------------------------------
---- | ------------------ | ------------------------ | | [YOLOv8n-cls](https://
-github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n-cls.pt) | 224 |
-66.6 | 87.0 | 12.9 | 0.31 | 2.7 | 4.3 | | [YOLOv8s-cls](https://github.com/
-ultralytics/assets/releases/download/v0.0.0/yolov8s-cls.pt) | 224 | 72.3 | 91.1
-| 23.4 | 0.35 | 6.4 | 13.5 | | [YOLOv8m-cls](https://github.com/ultralytics/
-assets/releases/download/v0.0.0/yolov8m-cls.pt) | 224 | 76.4 | 93.2 | 85.4 |
-0.62 | 17.0 | 42.7 | | [YOLOv8l-cls](https://github.com/ultralytics/assets/
-releases/download/v0.0.0/yolov8l-cls.pt) | 224 | 78.0 | 94.1 | 163.0 | 0.87 |
-37.5 | 99.7 | | [YOLOv8x-cls](https://github.com/ultralytics/assets/releases/
-download/v0.0.0/yolov8x-cls.pt) | 224 | 78.4 | 94.3 | 232.0 | 1.01 | 57.4 |
-154.8 | - **acc** values are model accuracies on the [ImageNet](https://
-www.image-net.org/) dataset validation set.
-Reproduce by `yolo val classify data=path/to/ImageNet device=0` - **Speed**
-averaged over ImageNet val images using an [Amazon EC2 P4d](https://
-aws.amazon.com/ec2/instance-types/p4/) instance.
-Reproduce by `yolo val classify data=path/to/ImageNet batch=1 device=0/cpu`  ##
-                                 Integrations
+---------------------------- | --------------- | ---------------- | -----------
+----- | ----------------------------- | ---------------------------------- | --
+------------- | ------------------------ | | [YOLOv8n-cls](https://github.com/
+ultralytics/assets/releases/download/v0.0.0/yolov8n-cls.pt) | 224 | 66.6 | 87.0
+| 12.9 | 0.31 | 2.7 | 4.3 | | [YOLOv8s-cls](https://github.com/ultralytics/
+assets/releases/download/v0.0.0/yolov8s-cls.pt) | 224 | 72.3 | 91.1 | 23.4 |
+0.35 | 6.4 | 13.5 | | [YOLOv8m-cls](https://github.com/ultralytics/assets/
+releases/download/v0.0.0/yolov8m-cls.pt) | 224 | 76.4 | 93.2 | 85.4 | 0.62 |
+17.0 | 42.7 | | [YOLOv8l-cls](https://github.com/ultralytics/assets/releases/
+download/v0.0.0/yolov8l-cls.pt) | 224 | 78.0 | 94.1 | 163.0 | 0.87 | 37.5 |
+99.7 | | [YOLOv8x-cls](https://github.com/ultralytics/assets/releases/download/
+v0.0.0/yolov8x-cls.pt) | 224 | 78.4 | 94.3 | 232.0 | 1.01 | 57.4 | 154.8 | -
+**acc** é½å¨ [ImageNet](https://www.image-net.org/
+) æ°æ®éä¸ï¼ä½¿ç¨åæ¨¡ååå°ºåº¦æµè¯å¾å°ã
+å¤ç°å½ä»¤ `yolo val classify data=path/to/ImageNet device=0` -
+**æ¨çéåº¦**ä½¿ç¨ ImageNet
+éªè¯éå¾çæ¨çæ¶é´è¿è¡å¹³åå¾å°ï¼æµè¯ç¯å¢ä½¿ç¨ [Amazon EC2
+P4d](https://aws.amazon.com/ec2/instance-types/p4/) å®ä¾ã
+å¤ç°å½ä»¤ `yolo val classify data=path/to/ImageNet batch=1 device=0/cpu`  ##
+                                 æ¨¡åéæ
 
 [https://github.com/ultralytics/assets/raw/main/yolov8/banner-integrations.png]
 
 
  [https://github.com/ultralytics/assets/raw/main/partners/logo-roboflow.png]
  [https://github.com/ultralytics/assets/raw/main/partners/logo-clearml.png]
   [https://github.com/ultralytics/assets/raw/main/partners/logo-comet.png]
 [https://github.com/ultralytics/assets/raw/main/partners/logo-neuralmagic.png]
-| Roboflow | ClearML â­ NEW | Comet â­ NEW | Neural Magic â­ NEW | | :------
--------------------------------------------------------------------------------
--------------------------------------: | :-------------------------------------
--------------------------------------------------------------------------------
--------------: | :-------------------------------------------------------------
--------------------------------------------------------------------------------
-------------: | :--------------------------------------------------------------
---------------------------------------: | | Label and export your custom
-datasets directly to YOLOv8 for training with [Roboflow](https://roboflow.com/
-?ref=ultralytics) | Automatically track, visualize and even remotely train
-YOLOv8 using [ClearML](https://cutt.ly/yolov5-readme-clearml) (open-source!) |
-Free forever, [Comet](https://bit.ly/yolov5-readme-comet2) lets you save YOLOv8
-models, resume training, and interactively visualize and debug predictions |
-Run YOLOv8 inference up to 6x faster with [Neural Magic DeepSparse](https://
-bit.ly/yolov5-neuralmagic) | ##
+| Roboflow | ClearML â­ æ° | Comet â­ æ° | Neural Magic â­ æ° | | :------
+--------------------------------------------------------------------------: | :
+-------------------------------------------------------------------------: | :-
+------------------------------------------------------------------------------
+-: | :-------------------------------------------------------------------------
+-----------: | | å°æ¨çèªå®ä¹æ°æ®éè¿è¡æ æ³¨å¹¶ç´æ¥å¯¼åºå°
+YOLOv8 ä»¥è¿è¡è®­ç» [Roboflow](https://roboflow.com/?ref=ultralytics) |
+èªå¨è·è¸ªãå¯è§åçè³è¿ç¨è®­ç» YOLOv8 [ClearML](https://cutt.ly/
+yolov5-readme-clearml)ï¼å¼æºï¼ï¼ | æ°¸è¿åè´¹ï¼[Comet](https://bit.ly/
+yolov5-readme-comet2)å¯è®©æ¨ä¿å­ YOLOv8
+æ¨¡åãæ¢å¤è®­ç»ä»¥åäº¤äºå¼å¯è§ååè°è¯é¢æµ | ä½¿ç¨ [Neural
+Magic DeepSparse](https://bit.ly/yolov5-neuralmagic)ï¼è¿è¡ YOLOv8
+æ¨ççéåº¦æé«å¯æé«6å | ##
                                 Ultralytics HUB
-Experience seamless AI with [Ultralytics HUB](https://bit.ly/ultralytics_hub)
-â­, the all-in-one solution for data visualization, YOLOv5 and YOLOv8 (coming
-soon) ð model training and deployment, without any coding. Transform images
-into actionable insights and bring your AI visions to life with ease using our
-cutting-edge platform and user-friendly [Ultralytics App](https://
-ultralytics.com/app_install). Start your journey for **Free** now! [https://
-github.com/ultralytics/assets/raw/main/im/ultralytics-hub.png] ##
-                                  Contribute
-We love your input! YOLOv5 and YOLOv8 would not be possible without help from
-our community. Please see our [Contributing Guide](CONTRIBUTING.md) to get
-started, and fill out our [Survey](https://ultralytics.com/
-survey?utm_source=github&utm_medium=social&utm_campaign=Survey) to send us
-feedback on your experience. Thank you ð to all our contributors!  [https://
-github.com/ultralytics/assets/raw/main/im/image-contributors.png] ##
+[Ultralytics HUB](https://bit.ly/ultralytics_hub) æ¯æä»¬â­
+**æ°**çæ ä»£ç è§£å³æ¹æ¡ï¼ç¨äºå¯è§åæ°æ®éï¼è®­ç» YOLOv8ð
+æ¨¡åï¼å¹¶ä»¥æ ç¼ä½éªæ¹å¼é¨ç½²å°ç°å®ä¸çãç°å¨å¼å§**åè´¹**!
+è¿å¯ä»¥éè¿ä¸è½½ [Ultralytics App](https://ultralytics.com/app_install)
+å¨ä½ ç iOS æ Android è®¾å¤ä¸è¿è¡ YOLOv8 æ¨¡å! [https://github.com/
+ultralytics/assets/raw/main/im/ultralytics-hub.png] ##
+                                    è´¡ç®
+æä»¬åæ¬¢æ¨çæè§æå»ºè®®ï¼æä»¬å¸æå°½å¯è½ç®ååéæå°ä¸º
+YOLOv8 ååºè´¡ç®ãè¯·çæä»¬ç [è´¡ç®æå](CONTRIBUTING.md)
+ï¼å¹¶å¡«å [è°æ¥é®å·](https://ultralytics.com/
+survey?utm_source=github&utm_medium=social&utm_campaign=Survey)
+åæä»¬åéæ¨çä½éªåé¦ãæè°¢æä»¬ææçè´¡ç®èï¼  [https:/
+/github.com/ultralytics/assets/raw/main/im/image-contributors.png] ##
                                     License
-YOLOv8 is available under two different licenses: - **GPL-3.0 License**: See
-[LICENSE](https://github.com/ultralytics/ultralytics/blob/main/LICENSE) file
-for details. - **Enterprise License**: Provides greater flexibility for
-commercial product development without the open-source requirements of GPL-3.0.
-Typical use cases are embedding Ultralytics software and AI models in
-commercial products and applications. Request an Enterprise License at
-[Ultralytics Licensing](https://ultralytics.com/license). ##
-                                    Contact
-For YOLOv8 bug reports and feature requests please visit [GitHub Issues](https:
-//github.com/ultralytics/ultralytics/issues) or the [Ultralytics Community
-Forum](https://community.ultralytics.com/).
+YOLOv8 å¨ä¸¤ç§ä¸åç License ä¸å¯ç¨ï¼ - **GPL-3.0 License**ï¼ æ¥ç
+[License](https://github.com/ultralytics/ultralytics/blob/main/LICENSE)
+æä»¶çè¯¦ç»ä¿¡æ¯ã - **ä¼ä¸License**ï¼å¨æ²¡æ GPL-3.0
+å¼æºè¦æ±çæåµä¸ä¸ºåä¸äº§åå¼åæä¾æ´å¤§ççµæ´»æ§ãå¸åç¨ä¾æ¯å°
+Ultralytics è½¯ä»¶å AI
+æ¨¡ååµå¥å°åä¸äº§åååºç¨ç¨åºä¸­ãå¨ä»¥ä¸ä½ç½®ç³è¯·ä¼ä¸è®¸å¯è¯
+[Ultralytics è®¸å¯](https://ultralytics.com/license) ã ##
+                                 èç³»æä»¬
+è¯·è®¿é® [GitHub Issues](https://github.com/ultralytics/ultralytics/issues)
+æ [Ultralytics Community Forum](https://community.ultralytis.com) ä»¥æ¥å
+YOLOv8 éè¯¯åè¯·æ±åè½ã
```

### Comparing `syml_ultralytics-8.0.49/requirements.txt` & `syml_ultralytics-8.0.53/requirements.txt`

 * *Files 15% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 requests>=2.23.0
 scipy>=1.4.1
 torch>=1.7.0
 torchvision>=0.8.1
 tqdm>=4.64.0
 
 # Logging -------------------------------------
-tensorboard>=2.4.1
+# tensorboard>=2.4.1
 # clearml
 # comet
 
 # Plotting ------------------------------------
 pandas>=1.1.4
 seaborn>=0.11.0
 
@@ -37,8 +37,7 @@
 # Extras --------------------------------------
 psutil  # system utilization
 thop>=0.1.1  # FLOPs computation
 # ipython  # interactive notebook
 # albumentations>=1.0.3
 # pycocotools>=2.0.6  # COCO mAP
 # roboflow
-certifi>=2022.12.7 # not directly required, pinned by Snyk to avoid a vulnerability
```

### Comparing `syml_ultralytics-8.0.49/setup.cfg` & `syml_ultralytics-8.0.53/setup.cfg`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/setup.py` & `syml_ultralytics-8.0.53/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     version=get_version(),  # version of pypi package
     python_requires='>=3.7',
     license='GPL-3.0',
     description='Syml Ultralytics YOLOv8',
     long_description=README,
     long_description_content_type='text/markdown',
     url='',
+    download_url="https://github.com/its-jd/syml_ultralytics/archive/refs/tags/8.0.53.tar.gz",
     author='syml_ultralytics',
-    download_url='https://github.com/its-jd/syml_ultralytics/archive/refs/tags/8.0.49.tar.gz',
     packages=find_packages(),  # required
     include_package_data=True,
     install_requires=REQUIREMENTS + PKG_REQUIREMENTS,
     extras_require={
         'dev': ['check-manifest', 'pytest', 'pytest-cov', 'coverage', 'mkdocs-material', 'mkdocstrings[python]'],
         'export': ['coremltools>=6.0', 'onnx', 'onnxsim', 'onnxruntime', 'openvino-dev>=2022.3'],
         'tf': ['onnx2tf', 'sng4onnx', 'tflite_support', 'tensorflow']},
```

### Comparing `syml_ultralytics-8.0.49/syml_ultralytics.egg-info/SOURCES.txt` & `syml_ultralytics-8.0.53/syml_ultralytics.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 syml_ultralytics.egg-info/PKG-INFO
 syml_ultralytics.egg-info/SOURCES.txt
 syml_ultralytics.egg-info/dependency_links.txt
 syml_ultralytics.egg-info/entry_points.txt
 syml_ultralytics.egg-info/requires.txt
 syml_ultralytics.egg-info/top_level.txt
 ultralytics/__init__.py
+ultralytics/assets/bus.jpg
+ultralytics/assets/zidane.jpg
 ultralytics/datasets/Argoverse.yaml
 ultralytics/datasets/GlobalWheat2020.yaml
 ultralytics/datasets/ImageNet.yaml
 ultralytics/datasets/Objects365.yaml
 ultralytics/datasets/SKU-110K.yaml
 ultralytics/datasets/VOC.yaml
 ultralytics/datasets/VisDrone.yaml
@@ -25,22 +27,28 @@
 ultralytics/datasets/coco128.yaml
 ultralytics/datasets/coco8-seg.yaml
 ultralytics/datasets/coco8.yaml
 ultralytics/datasets/xView.yaml
 ultralytics/hub/__init__.py
 ultralytics/hub/auth.py
 ultralytics/hub/session.py
+ultralytics/hub/utils - Copy.py
 ultralytics/hub/utils.py
 ultralytics/models/v3/yolov3-sppu.yaml
 ultralytics/models/v3/yolov3-tinyu.yaml
 ultralytics/models/v3/yolov3u.yaml
+ultralytics/models/v5/yolov5l6u.yaml
 ultralytics/models/v5/yolov5lu.yaml
+ultralytics/models/v5/yolov5m6u.yaml
 ultralytics/models/v5/yolov5mu.yaml
+ultralytics/models/v5/yolov5n6u.yaml
 ultralytics/models/v5/yolov5nu.yaml
+ultralytics/models/v5/yolov5s6u.yaml
 ultralytics/models/v5/yolov5su.yaml
+ultralytics/models/v5/yolov5x6u.yaml
 ultralytics/models/v5/yolov5xu.yaml
 ultralytics/models/v8/yolov8l.yaml
 ultralytics/models/v8/yolov8m.yaml
 ultralytics/models/v8/yolov8n.yaml
 ultralytics/models/v8/yolov8s.yaml
 ultralytics/models/v8/yolov8x.yaml
 ultralytics/models/v8/yolov8x6.yaml
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/datasets/Argoverse.yaml` & `syml_ultralytics-8.0.53/ultralytics/datasets/Argoverse.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Ultralytics YOLO 🚀, GPL-3.0 license
 # Argoverse-HD dataset (ring-front-center camera) http://www.cs.cmu.edu/~mengtial/proj/streaming/ by Argo AI
 # Example usage: yolo train data=Argoverse.yaml
 # parent
-# ├── yolov5
+# ├── ultralytics
 # └── datasets
 #     └── Argoverse  ← downloads here (31.3 GB)
 
 
 # Train/val/test sets as 1) dir: path/to/imgs, 2) file: path/to/imgs.txt, or 3) list: [path/to/imgs1, path/to/imgs2, ..]
 path: ../datasets/Argoverse  # dataset root dir
 train: Argoverse-1.1/images/train/  # train images (relative to 'path') 39384 images
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/datasets/GlobalWheat2020.yaml` & `syml_ultralytics-8.0.53/ultralytics/datasets/GlobalWheat2020.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Ultralytics YOLO 🚀, GPL-3.0 license
 # Global Wheat 2020 dataset http://www.global-wheat.com/ by University of Saskatchewan
 # Example usage: yolo train data=GlobalWheat2020.yaml
 # parent
-# ├── yolov5
+# ├── ultralytics
 # └── datasets
 #     └── GlobalWheat2020  ← downloads here (7.0 GB)
 
 
 # Train/val/test sets as 1) dir: path/to/imgs, 2) file: path/to/imgs.txt, or 3) list: [path/to/imgs1, path/to/imgs2, ..]
 path: ../datasets/GlobalWheat2020  # dataset root dir
 train: # train images (relative to 'path') 3422 images
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/datasets/ImageNet.yaml` & `syml_ultralytics-8.0.53/ultralytics/datasets/ImageNet.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Ultralytics YOLO 🚀, GPL-3.0 license
 # ImageNet-1k dataset https://www.image-net.org/index.php by Stanford University
 # Simplified class names from https://github.com/anishathalye/imagenet-simple-labels
 # Example usage: yolo train task=classify data=imagenet
 # parent
-# ├── yolov5
+# ├── ultralytics
 # └── datasets
 #     └── imagenet  ← downloads here (144 GB)
 
 
 # Train/val/test sets as 1) dir: path/to/imgs, 2) file: path/to/imgs.txt, or 3) list: [path/to/imgs1, path/to/imgs2, ..]
 path: ../datasets/imagenet  # dataset root dir
 train: train  # train images (relative to 'path') 1281167 images
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/datasets/Objects365.yaml` & `syml_ultralytics-8.0.53/ultralytics/datasets/Objects365.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Ultralytics YOLO 🚀, GPL-3.0 license
 # Objects365 dataset https://www.objects365.org/ by Megvii
 # Example usage: yolo train data=Objects365.yaml
 # parent
-# ├── yolov5
+# ├── ultralytics
 # └── datasets
 #     └── Objects365  ← downloads here (712 GB = 367G data + 345G zips)
 
 
 # Train/val/test sets as 1) dir: path/to/imgs, 2) file: path/to/imgs.txt, or 3) list: [path/to/imgs1, path/to/imgs2, ..]
 path: ../datasets/Objects365  # dataset root dir
 train: images/train  # train images (relative to 'path') 1742289 images
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/datasets/SKU-110K.yaml` & `syml_ultralytics-8.0.53/ultralytics/datasets/SKU-110K.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Ultralytics YOLO 🚀, GPL-3.0 license
 # SKU-110K retail items dataset https://github.com/eg4000/SKU110K_CVPR19 by Trax Retail
 # Example usage: yolo train data=SKU-110K.yaml
 # parent
-# ├── yolov5
+# ├── ultralytics
 # └── datasets
 #     └── SKU-110K  ← downloads here (13.6 GB)
 
 
 # Train/val/test sets as 1) dir: path/to/imgs, 2) file: path/to/imgs.txt, or 3) list: [path/to/imgs1, path/to/imgs2, ..]
 path: ../datasets/SKU-110K  # dataset root dir
 train: train.txt  # train images (relative to 'path')  8219 images
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/datasets/VOC.yaml` & `syml_ultralytics-8.0.53/ultralytics/datasets/VOC.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Ultralytics YOLO 🚀, GPL-3.0 license
 # PASCAL VOC dataset http://host.robots.ox.ac.uk/pascal/VOC by University of Oxford
 # Example usage: yolo train data=VOC.yaml
 # parent
-# ├── yolov5
+# ├── ultralytics
 # └── datasets
 #     └── VOC  ← downloads here (2.8 GB)
 
 
 # Train/val/test sets as 1) dir: path/to/imgs, 2) file: path/to/imgs.txt, or 3) list: [path/to/imgs1, path/to/imgs2, ..]
 path: ../datasets/VOC
 train: # train images (relative to 'path')  16551 images
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/datasets/VisDrone.yaml` & `syml_ultralytics-8.0.53/ultralytics/datasets/VisDrone.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Ultralytics YOLO 🚀, GPL-3.0 license
 # VisDrone2019-DET dataset https://github.com/VisDrone/VisDrone-Dataset by Tianjin University
 # Example usage: yolo train data=VisDrone.yaml
 # parent
-# ├── yolov5
+# ├── ultralytics
 # └── datasets
 #     └── VisDrone  ← downloads here (2.3 GB)
 
 
 # Train/val/test sets as 1) dir: path/to/imgs, 2) file: path/to/imgs.txt, or 3) list: [path/to/imgs1, path/to/imgs2, ..]
 path: ../datasets/VisDrone  # dataset root dir
 train: VisDrone2019-DET-train/images  # train images (relative to 'path')  6471 images
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/datasets/coco.yaml` & `syml_ultralytics-8.0.53/ultralytics/datasets/coco.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Ultralytics YOLO 🚀, GPL-3.0 license
 # COCO 2017 dataset http://cocodataset.org by Microsoft
 # Example usage: yolo train data=coco.yaml
 # parent
-# ├── yolov5
+# ├── ultralytics
 # └── datasets
 #     └── coco  ← downloads here (20.1 GB)
 
 
 # Train/val/test sets as 1) dir: path/to/imgs, 2) file: path/to/imgs.txt, or 3) list: [path/to/imgs1, path/to/imgs2, ..]
 path: ../datasets/coco  # dataset root dir
 train: train2017.txt  # train images (relative to 'path') 118287 images
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/datasets/coco128-seg.yaml` & `syml_ultralytics-8.0.53/ultralytics/datasets/coco128-seg.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Ultralytics YOLO 🚀, GPL-3.0 license
 # COCO128-seg dataset https://www.kaggle.com/ultralytics/coco128 (first 128 images from COCO train2017) by Ultralytics
 # Example usage: yolo train data=coco128.yaml
 # parent
-# ├── yolov5
+# ├── ultralytics
 # └── datasets
 #     └── coco128-seg  ← downloads here (7 MB)
 
 
 # Train/val/test sets as 1) dir: path/to/imgs, 2) file: path/to/imgs.txt, or 3) list: [path/to/imgs1, path/to/imgs2, ..]
 path: ../datasets/coco128-seg  # dataset root dir
 train: images/train2017  # train images (relative to 'path') 128 images
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/datasets/coco128.yaml` & `syml_ultralytics-8.0.53/ultralytics/datasets/coco128.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Ultralytics YOLO 🚀, GPL-3.0 license
 # COCO128 dataset https://www.kaggle.com/ultralytics/coco128 (first 128 images from COCO train2017) by Ultralytics
 # Example usage: yolo train data=coco128.yaml
 # parent
-# ├── yolov5
+# ├── ultralytics
 # └── datasets
 #     └── coco128  ← downloads here (7 MB)
 
 
 # Train/val/test sets as 1) dir: path/to/imgs, 2) file: path/to/imgs.txt, or 3) list: [path/to/imgs1, path/to/imgs2, ..]
 path: ../datasets/coco128  # dataset root dir
 train: images/train2017  # train images (relative to 'path') 128 images
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/datasets/coco8-seg.yaml` & `syml_ultralytics-8.0.53/ultralytics/datasets/coco8-seg.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Ultralytics YOLO 🚀, GPL-3.0 license
 # COCO8-seg dataset (first 8 images from COCO train2017) by Ultralytics
 # Example usage: yolo train data=coco8-seg.yaml
 # parent
-# ├── yolov5
+# ├── ultralytics
 # └── datasets
 #     └── coco8-seg  ← downloads here (1 MB)
 
 
 # Train/val/test sets as 1) dir: path/to/imgs, 2) file: path/to/imgs.txt, or 3) list: [path/to/imgs1, path/to/imgs2, ..]
 path: ../datasets/coco8-seg  # dataset root dir
 train: images/train  # train images (relative to 'path') 4 images
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/datasets/coco8.yaml` & `syml_ultralytics-8.0.53/ultralytics/datasets/coco8.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Ultralytics YOLO 🚀, GPL-3.0 license
 # COCO8 dataset (first 8 images from COCO train2017) by Ultralytics
 # Example usage: yolo train data=coco8.yaml
 # parent
-# ├── yolov5
+# ├── ultralytics
 # └── datasets
 #     └── coco8  ← downloads here (1 MB)
 
 
 # Train/val/test sets as 1) dir: path/to/imgs, 2) file: path/to/imgs.txt, or 3) list: [path/to/imgs1, path/to/imgs2, ..]
 path: ../datasets/coco8  # dataset root dir
 train: images/train  # train images (relative to 'path') 4 images
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/datasets/xView.yaml` & `syml_ultralytics-8.0.53/ultralytics/datasets/xView.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Ultralytics YOLO 🚀, GPL-3.0 license
 # DIUx xView 2018 Challenge https://challenge.xviewdataset.org by U.S. National Geospatial-Intelligence Agency (NGA)
 # --------  DOWNLOAD DATA MANUALLY and jar xf val_images.zip to 'datasets/xView' before running train command!  --------
 # Example usage: yolo train data=xView.yaml
 # parent
-# ├── yolov5
+# ├── ultralytics
 # └── datasets
 #     └── xView  ← downloads here (20.7 GB)
 
 
 # Train/val/test sets as 1) dir: path/to/imgs, 2) file: path/to/imgs.txt, or 3) list: [path/to/imgs1, path/to/imgs2, ..]
 path: ../datasets/xView  # dataset root dir
 train: images/autosplit_train.txt  # train images (relative to 'path') 90% of 847 train images
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/hub/__init__.py` & `syml_ultralytics-8.0.53/ultralytics/hub/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 # Ultralytics YOLO 🚀, GPL-3.0 license
 
 import requests
 
 from ultralytics.hub.auth import Auth
 from ultralytics.hub.session import HUBTrainingSession
 from ultralytics.hub.utils import PREFIX, split_key
-from ultralytics.yolo.engine.exporter import EXPORT_FORMATS_LIST
 from ultralytics.yolo.engine.model import YOLO
 from ultralytics.yolo.utils import LOGGER, emojis
 
-# Define all export formats
-EXPORT_FORMATS_HUB = EXPORT_FORMATS_LIST + ['ultralytics_tflite', 'ultralytics_coreml']
-
 
 def start(key=''):
     """
     Start training models with Ultralytics HUB. Usage: from ultralytics.hub import start; start('API_KEY')
     """
     auth = Auth(key)
     if not auth.get_state():
@@ -59,30 +55,36 @@
 
     if r.status_code == 200:
         LOGGER.info(f'{PREFIX}Model reset successfully')
         return
     LOGGER.warning(f'{PREFIX}Model reset failure {r.status_code} {r.reason}')
 
 
+def export_fmts_hub():
+    # Returns a list of HUB-supported export formats
+    from ultralytics.yolo.engine.exporter import export_formats
+    return list(export_formats()['Argument'][1:]) + ['ultralytics_tflite', 'ultralytics_coreml']
+
+
 def export_model(key='', format='torchscript'):
     # Export a model to all formats
-    assert format in EXPORT_FORMATS_HUB, f"Unsupported export format '{format}', valid formats are {EXPORT_FORMATS_HUB}"
+    assert format in export_fmts_hub(), f"Unsupported export format '{format}', valid formats are {export_fmts_hub()}"
     api_key, model_id = split_key(key)
     r = requests.post('https://api.ultralytics.com/export',
                       json={
                           'apiKey': api_key,
                           'modelId': model_id,
                           'format': format})
     assert r.status_code == 200, f'{PREFIX}{format} export failure {r.status_code} {r.reason}'
     LOGGER.info(f'{PREFIX}{format} export started ✅')
 
 
 def get_export(key='', format='torchscript'):
     # Get an exported model dictionary with download URL
-    assert format in EXPORT_FORMATS_HUB, f"Unsupported export format '{format}', valid formats are {EXPORT_FORMATS_HUB}"
+    assert format in export_fmts_hub, f"Unsupported export format '{format}', valid formats are {export_fmts_hub}"
     api_key, model_id = split_key(key)
     r = requests.post('https://api.ultralytics.com/get-export',
                       json={
                           'apiKey': api_key,
                           'modelId': model_id,
                           'format': format})
     assert r.status_code == 200, f'{PREFIX}{format} get_export failure {r.status_code} {r.reason}'
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/hub/auth.py` & `syml_ultralytics-8.0.53/ultralytics/hub/auth.py`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/hub/session.py` & `syml_ultralytics-8.0.53/ultralytics/hub/session.py`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/hub/utils.py` & `syml_ultralytics-8.0.53/ultralytics/hub/utils - Copy.py`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/models/v3/yolov3-sppu.yaml` & `syml_ultralytics-8.0.53/ultralytics/models/v3/yolov3-sppu.yaml`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/models/v3/yolov3-tinyu.yaml` & `syml_ultralytics-8.0.53/ultralytics/models/v3/yolov3-tinyu.yaml`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/models/v3/yolov3u.yaml` & `syml_ultralytics-8.0.53/ultralytics/models/v3/yolov3u.yaml`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/models/v5/yolov5lu.yaml` & `syml_ultralytics-8.0.53/ultralytics/models/v5/yolov5lu.yaml`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/models/v5/yolov5mu.yaml` & `syml_ultralytics-8.0.53/ultralytics/models/v5/yolov5mu.yaml`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/models/v5/yolov5nu.yaml` & `syml_ultralytics-8.0.53/ultralytics/models/v5/yolov5nu.yaml`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/models/v5/yolov5su.yaml` & `syml_ultralytics-8.0.53/ultralytics/models/v5/yolov5su.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Ultralytics YOLO 🚀, GPL-3.0 license
 
 # Parameters
 nc: 80  # number of classes
 depth_multiple: 0.33  # model depth multiple
 width_multiple: 0.50  # layer channel multiple
 
-
 # YOLOv5 v6.0 backbone
 backbone:
   # [from, number, module, args]
   [[-1, 1, Conv, [64, 6, 2, 2]],  # 0-P1/2
    [-1, 1, Conv, [128, 3, 2]],  # 1-P2/4
    [-1, 3, C3, [128]],
    [-1, 1, Conv, [256, 3, 2]],  # 3-P3/8
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/models/v5/yolov5xu.yaml` & `syml_ultralytics-8.0.53/ultralytics/models/v5/yolov5xu.yaml`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/models/v8/cls/yolov8l-cls.yaml` & `syml_ultralytics-8.0.53/ultralytics/models/v8/cls/yolov8l-cls.yaml`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/models/v8/cls/yolov8m-cls.yaml` & `syml_ultralytics-8.0.53/ultralytics/models/v8/cls/yolov8m-cls.yaml`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/models/v8/cls/yolov8n-cls.yaml` & `syml_ultralytics-8.0.53/ultralytics/models/v8/cls/yolov8n-cls.yaml`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/models/v8/cls/yolov8s-cls.yaml` & `syml_ultralytics-8.0.53/ultralytics/models/v8/cls/yolov8s-cls.yaml`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/models/v8/cls/yolov8x-cls.yaml` & `syml_ultralytics-8.0.53/ultralytics/models/v8/cls/yolov8x-cls.yaml`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/models/v8/seg/yolov8l-seg.yaml` & `syml_ultralytics-8.0.53/ultralytics/models/v8/seg/yolov8l-seg.yaml`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/models/v8/seg/yolov8m-seg.yaml` & `syml_ultralytics-8.0.53/ultralytics/models/v8/seg/yolov8m-seg.yaml`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/models/v8/seg/yolov8n-seg.yaml` & `syml_ultralytics-8.0.53/ultralytics/models/v8/seg/yolov8n-seg.yaml`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/models/v8/seg/yolov8s-seg.yaml` & `syml_ultralytics-8.0.53/ultralytics/models/v8/seg/yolov8s-seg.yaml`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/models/v8/seg/yolov8x-seg.yaml` & `syml_ultralytics-8.0.53/ultralytics/models/v8/seg/yolov8x-seg.yaml`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/models/v8/yolov8l.yaml` & `syml_ultralytics-8.0.53/ultralytics/models/v8/yolov8l.yaml`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/models/v8/yolov8m.yaml` & `syml_ultralytics-8.0.53/ultralytics/models/v8/yolov8m.yaml`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/models/v8/yolov8n.yaml` & `syml_ultralytics-8.0.53/ultralytics/models/v8/yolov8n.yaml`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/models/v8/yolov8s.yaml` & `syml_ultralytics-8.0.53/ultralytics/models/v8/yolov8s.yaml`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/models/v8/yolov8x.yaml` & `syml_ultralytics-8.0.53/ultralytics/models/v8/yolov8x.yaml`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/models/v8/yolov8x6.yaml` & `syml_ultralytics-8.0.53/ultralytics/models/v8/yolov8x6.yaml`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/nn/autobackend.py` & `syml_ultralytics-8.0.53/ultralytics/nn/autobackend.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,51 +10,58 @@
 
 import cv2
 import numpy as np
 import torch
 import torch.nn as nn
 from PIL import Image
 
-from ultralytics.yolo.utils import LOGGER, ROOT, yaml_load
+from ultralytics.yolo.utils import LINUX, LOGGER, ROOT, yaml_load
 from ultralytics.yolo.utils.checks import check_requirements, check_suffix, check_version, check_yaml
 from ultralytics.yolo.utils.downloads import attempt_download_asset, is_url
 from ultralytics.yolo.utils.ops import xywh2xyxy
 
 
 def check_class_names(names):
     # Check class names. Map imagenet class codes to human-readable names if required. Convert lists to dicts.
     if isinstance(names, list):  # names is a list
         names = dict(enumerate(names))  # convert to dict
     if isinstance(names, dict):
         if not all(isinstance(k, int) for k in names.keys()):  # convert string keys to int, i.e. '0' to 0
             names = {int(k): v for k, v in names.items()}
+        n = len(names)
+        if max(names.keys()) >= n:
+            raise KeyError(f'{n}-class dataset requires class indices 0-{n - 1}, but you have invalid class indices '
+                           f'{min(names.keys())}-{max(names.keys())} defined in your dataset YAML.')
         if isinstance(names[0], str) and names[0].startswith('n0'):  # imagenet class codes, i.e. 'n01440764'
             map = yaml_load(ROOT / 'datasets/ImageNet.yaml')['map']  # human-readable names
             names = {k: map[v] for k, v in names.items()}
     return names
 
 
 class AutoBackend(nn.Module):
 
-    def _apply_default_class_names(self, data):
-        with contextlib.suppress(Exception):
-            return yaml_load(check_yaml(data))['names']
-        return {i: f'class{i}' for i in range(999)}  # return default if above errors
-
-    def __init__(self, weights='yolov8n.pt', device=torch.device('cpu'), dnn=False, data=None, fp16=False, fuse=True):
+    def __init__(self,
+                 weights='yolov8n.pt',
+                 device=torch.device('cpu'),
+                 dnn=False,
+                 data=None,
+                 fp16=False,
+                 fuse=True,
+                 verbose=True):
         """
         MultiBackend class for python inference on various platforms using Ultralytics YOLO.
 
         Args:
             weights (str): The path to the weights file. Default: 'yolov8n.pt'
             device (torch.device): The device to run the model on.
             dnn (bool): Use OpenCV's DNN module for inference if True, defaults to False.
             data (str), (Path): Additional data.yaml file for class names, optional
             fp16 (bool): If True, use half precision. Default: False
             fuse (bool): Whether to fuse the model or not. Default: True
+            verbose (bool): Whether to run in verbose mode or not. Default: True
 
         Supported formats and their naming conventions:
             | Format                | Suffix           |
             |-----------------------|------------------|
             | PyTorch               | *.pt             |
             | TorchScript           | *.torchscript    |
             | ONNX Runtime          | *.onnx           |
@@ -79,15 +86,15 @@
         cuda = torch.cuda.is_available() and device.type != 'cpu'  # use CUDA
         if not (pt or triton or nn_module):
             w = attempt_download_asset(w)  # download if not local
 
         # NOTE: special case: in-memory pytorch model
         if nn_module:
             model = weights.to(device)
-            model = model.fuse() if fuse else model
+            model = model.fuse(verbose=verbose) if fuse else model
             names = model.module.names if hasattr(model, 'module') else model.names  # get class names
             stride = max(int(model.stride.max()), 32)  # model stride
             model.half() if fp16 else model.float()
             self.model = model  # explicitly assign for to(), cpu(), cuda(), half()
             pt = True
         elif pt:  # PyTorch
             from ultralytics.nn.tasks import attempt_load_weights
@@ -132,15 +139,20 @@
             batch_dim = get_batch(network)
             if batch_dim.is_static:
                 batch_size = batch_dim.get_length()
             executable_network = ie.compile_model(network, device_name='CPU')  # device_name="MYRIAD" for NCS2
             metadata = w.parent / 'metadata.yaml'
         elif engine:  # TensorRT
             LOGGER.info(f'Loading {w} for TensorRT inference...')
-            import tensorrt as trt  # https://developer.nvidia.com/nvidia-tensorrt-download
+            try:
+                import tensorrt as trt  # noqa https://developer.nvidia.com/nvidia-tensorrt-download
+            except ImportError:
+                if LINUX:
+                    check_requirements('nvidia-tensorrt', cmds='-U --index-url https://pypi.ngc.nvidia.com')
+                import tensorrt as trt  # noqa
             check_version(trt.__version__, '7.0.0', hard=True)  # require tensorrt>=7.0.0
             if device.type == 'cpu':
                 device = torch.device('cuda:0')
             Binding = namedtuple('Binding', ('name', 'dtype', 'shape', 'data', 'ptr'))
             logger = trt.Logger(trt.Logger.INFO)
             # Read file
             with open(w, 'rb') as f, trt.Runtime(logger) as runtime:
@@ -168,15 +180,15 @@
                 bindings[name] = Binding(name, dtype, shape, im, int(im.data_ptr()))
             binding_addrs = OrderedDict((n, d.ptr) for n, d in bindings.items())
             batch_size = bindings['images'].shape[0]  # if dynamic, this is instead max batch size
         elif coreml:  # CoreML
             LOGGER.info(f'Loading {w} for CoreML inference...')
             import coremltools as ct
             model = ct.models.MLModel(w)
-            metadata = model.user_defined_metadata
+            metadata = dict(model.user_defined_metadata)
         elif saved_model:  # TF SavedModel
             LOGGER.info(f'Loading {w} for TensorFlow SavedModel inference...')
             import tensorflow as tf
             keras = False  # assume TF1 saved_model
             model = tf.keras.models.load_model(w) if keras else tf.saved_model.load(w)
             metadata = Path(w) / 'metadata.yaml'
         elif pb:  # GraphDef https://www.tensorflow.org/guide/migrate#a_graphpb_or_graphpbtxt
@@ -219,15 +231,15 @@
                     meta_file = model.namelist()[0]
                     metadata = ast.literal_eval(model.read(meta_file).decode('utf-8'))
         elif tfjs:  # TF.js
             raise NotImplementedError('YOLOv8 TF.js inference is not supported')
         elif paddle:  # PaddlePaddle
             LOGGER.info(f'Loading {w} for PaddlePaddle inference...')
             check_requirements('paddlepaddle-gpu' if cuda else 'paddlepaddle')
-            import paddle.inference as pdi
+            import paddle.inference as pdi  # noqa
             w = Path(w)
             if not w.is_file():  # if not *.pdmodel
                 w = next(w.rglob('*.pdmodel'))  # get *.pdmodel file from *_paddle_model dir
             config = pdi.Config(str(w), str(w.with_suffix('.pdiparams')))
             if cuda:
                 config.enable_use_gpu(memory_pool_init_size_mb=2048, device_id=0)
             predictor = pdi.create_predictor(config)
@@ -240,28 +252,33 @@
             TODO:
             check_requirements('tritonclient[all]')
             from utils.triton import TritonRemoteModel
             model = TritonRemoteModel(url=w)
             nhwc = model.runtime.startswith("tensorflow")
             '''
         else:
-            from ultralytics.yolo.engine.exporter import EXPORT_FORMATS_TABLE
+            from ultralytics.yolo.engine.exporter import export_formats
             raise TypeError(f"model='{w}' is not a supported model format. "
                             'See https://docs.ultralytics.com/tasks/detection/#export for help.'
-                            f'\n\n{EXPORT_FORMATS_TABLE}')
+                            f'\n\n{export_formats()}')
 
         # Load external metadata YAML
         if isinstance(metadata, (str, Path)) and Path(metadata).exists():
             metadata = yaml_load(metadata)
         if metadata:
-            stride = int(metadata['stride'])
+            for k, v in metadata.items():
+                if k in ('stride', 'batch'):
+                    metadata[k] = int(v)
+                elif k in ('imgsz', 'names') and isinstance(v, str):
+                    metadata[k] = eval(v)
+            stride = metadata['stride']
             task = metadata['task']
-            batch = int(metadata['batch'])
-            imgsz = eval(metadata['imgsz']) if isinstance(metadata['imgsz'], str) else metadata['imgsz']
-            names = eval(metadata['names']) if isinstance(metadata['names'], str) else metadata['names']
+            batch = metadata['batch']
+            imgsz = metadata['imgsz']
+            names = metadata['names']
         elif not (pt or triton or nn_module):
             LOGGER.warning(f"WARNING ⚠️ Metadata not found for 'model={weights}'")
 
         # Check names
         if 'names' not in locals():  # names missing
             names = self._apply_default_class_names(data)
         names = check_class_names(names)
@@ -274,15 +291,15 @@
 
         Args:
             im (torch.Tensor): The image tensor to perform inference on.
             augment (bool): whether to perform data augmentation during inference, defaults to False
             visualize (bool): whether to visualize the output predictions, defaults to False
 
         Returns:
-            (tuple): Tuple containing the raw output tensor, and the processed output for visualization (if visualize=True)
+            (tuple): Tuple containing the raw output tensor, and processed output for visualization (if visualize=True)
         """
         b, ch, h, w = im.shape  # batch, channel, height, width
         if self.fp16 and im.dtype != torch.float16:
             im = im.half()  # to FP16
         if self.nhwc:
             im = im.permute(0, 2, 3, 1)  # torch BCHW to numpy BHWC shape(1,320,192,3)
 
@@ -311,21 +328,14 @@
             s = self.bindings['images'].shape
             assert im.shape == s, f"input size {im.shape} {'>' if self.dynamic else 'not equal to'} max model size {s}"
             self.binding_addrs['images'] = int(im.data_ptr())
             self.context.execute_v2(list(self.binding_addrs.values()))
             y = [self.bindings[x].data for x in sorted(self.output_names)]
         elif self.coreml:  # CoreML
             im = im[0].cpu().numpy()
-            if self.task == 'classify':
-                from ultralytics.yolo.data.utils import IMAGENET_MEAN, IMAGENET_STD
-
-                # im_pil = Image.fromarray(((im / 6 + 0.5) * 255).astype('uint8'))
-                for i in range(3):
-                    im[..., i] *= IMAGENET_STD[i]
-                    im[..., i] += IMAGENET_MEAN[i]
             im_pil = Image.fromarray((im * 255).astype('uint8'))
             # im = im.resize((192, 320), Image.ANTIALIAS)
             y = self.model.predict({'image': im_pil})  # coordinates are xywh normalized
             if 'confidence' in y:
                 box = xywh2xyxy(y['coordinates'] * [[w, h, w, h]])  # xyxy pixels
                 conf, cls = y['confidence'].max(1), y['confidence'].argmax(1).astype(np.float)
                 y = np.concatenate((box, conf.reshape(-1, 1), cls.reshape(-1, 1)), 1)
@@ -350,18 +360,18 @@
                 y = self.frozen_func(x=self.tf.constant(im))
                 if len(y) == 2 and len(self.names) == 999:  # segments and names not defined
                     ip, ib = (0, 1) if len(y[0].shape) == 4 else (1, 0)  # index of protos, boxes
                     nc = y[ib].shape[1] - y[ip].shape[3] - 4  # y = (1, 160, 160, 32), (1, 116, 8400)
                     self.names = {i: f'class{i}' for i in range(nc)}
             else:  # Lite or Edge TPU
                 input = self.input_details[0]
-                int8 = input['dtype'] == np.uint8  # is TFLite quantized uint8 model
+                int8 = input['dtype'] == np.int8  # is TFLite quantized int8 model
                 if int8:
                     scale, zero_point = input['quantization']
-                    im = (im / scale + zero_point).astype(np.uint8)  # de-scale
+                    im = (im / scale + zero_point).astype(np.int8)  # de-scale
                 self.interpreter.set_tensor(input['index'], im)
                 self.interpreter.invoke()
                 y = []
                 for output in self.output_details:
                     x = self.interpreter.get_tensor(output['index'])
                     if int8:
                         scale, zero_point = output['quantization']
@@ -407,14 +417,20 @@
         warmup_types = self.pt, self.jit, self.onnx, self.engine, self.saved_model, self.pb, self.triton, self.nn_module
         if any(warmup_types) and (self.device.type != 'cpu' or self.triton):
             im = torch.empty(*imgsz, dtype=torch.half if self.fp16 else torch.float, device=self.device)  # input
             for _ in range(2 if self.jit else 1):  #
                 self.forward(im)  # warmup
 
     @staticmethod
+    def _apply_default_class_names(data):
+        with contextlib.suppress(Exception):
+            return yaml_load(check_yaml(data))['names']
+        return {i: f'class{i}' for i in range(999)}  # return default if above errors
+
+    @staticmethod
     def _model_type(p='path/to/model.pt'):
         """
         This function takes a path to a model file and returns the model type
 
         Args:
             p: path to the model file. Defaults to path/to/model.pt
         """
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/nn/autoshape.py` & `syml_ultralytics-8.0.53/ultralytics/nn/autoshape.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 """
 
 from copy import copy
 from pathlib import Path
 
 import cv2
 import numpy as np
-import pandas as pd
 import requests
 import torch
 import torch.nn as nn
 from PIL import Image, ImageOps
 from torch.cuda import amp
 
 from ultralytics.nn.autobackend import AutoBackend
@@ -200,20 +199,21 @@
 
     def render(self, labels=True):
         self._run(render=True, labels=labels)  # render results
         return self.ims
 
     def pandas(self):
         # return detections as pandas DataFrames, i.e. print(results.pandas().xyxy[0])
+        import pandas
         new = copy(self)  # return copy
         ca = 'xmin', 'ymin', 'xmax', 'ymax', 'confidence', 'class', 'name'  # xyxy columns
         cb = 'xcenter', 'ycenter', 'width', 'height', 'confidence', 'class', 'name'  # xywh columns
         for k, c in zip(['xyxy', 'xyxyn', 'xywh', 'xywhn'], [ca, ca, cb, cb]):
             a = [[x[:5] + [int(x[5]), self.names[int(x[5])]] for x in x.tolist()] for x in getattr(self, k)]  # update
-            setattr(new, k, [pd.DataFrame(x, columns=c) for x in a])
+            setattr(new, k, [pandas.DataFrame(x, columns=c) for x in a])
         return new
 
     def tolist(self):
         # return a list of Detections objects, i.e. 'for result in results.tolist():'
         r = range(self.n)  # iterable
         x = [Detections([self.ims[i]], [self.pred[i]], [self.files[i]], self.times, self.names, self.s) for i in r]
         # for d in x:
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/nn/modules.py` & `syml_ultralytics-8.0.53/ultralytics/nn/modules.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,16 @@
         return self.act(self.bn(self.conv_transpose(x)))
 
     def forward_fuse(self, x):
         return self.act(self.conv_transpose(x))
 
 
 class DFL(nn.Module):
-    # Integral module of Distribution Focal Loss (DFL) proposed in Generalized Focal Loss https://ieeexplore.ieee.org/document/9792391
+    # Integral module of Distribution Focal Loss (DFL)
+    # Proposed in Generalized Focal Loss https://ieeexplore.ieee.org/document/9792391
     def __init__(self, c1=16):
         super().__init__()
         self.conv = nn.Conv2d(c1, 1, 1, bias=False).requires_grad_(False)
         x = torch.arange(c1, dtype=torch.float)
         self.conv.weight.data[:] = nn.Parameter(x.view(1, c1, 1, 1))
         self.c1 = c1
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/nn/tasks.py` & `syml_ultralytics-8.0.53/ultralytics/nn/tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         dt.append((time_sync() - t) * 100)
         if m == self.model[0]:
             LOGGER.info(f"{'time (ms)':>10s} {'GFLOPs':>10s} {'params':>10s}  module")
         LOGGER.info(f'{dt[-1]:10.2f} {o:10.2f} {m.np:10.0f}  {m.type}')
         if c:
             LOGGER.info(f"{sum(dt):10.2f} {'-':>10s} {'-':>10s}  Total")
 
-    def fuse(self):
+    def fuse(self, verbose=True):
         """
         Fuse the `Conv2d()` and `BatchNorm2d()` layers of the model into a single layer, in order to improve the
         computation efficiency.
 
         Returns:
             (nn.Module): The fused model is returned.
         """
@@ -101,15 +101,15 @@
                     m.conv = fuse_conv_and_bn(m.conv, m.bn)  # update conv
                     delattr(m, 'bn')  # remove batchnorm
                     m.forward = m.forward_fuse  # update forward
                 if isinstance(m, ConvTranspose) and hasattr(m, 'bn'):
                     m.conv_transpose = fuse_deconv_and_bn(m.conv_transpose, m.bn)
                     delattr(m, 'bn')  # remove batchnorm
                     m.forward = m.forward_fuse  # update forward
-            self.info()
+            self.info(verbose=verbose)
 
         return self
 
     def is_fused(self, thresh=10):
         """
         Check if the model has less than a certain threshold of BatchNorm layers.
 
@@ -118,23 +118,23 @@
 
         Returns:
             (bool): True if the number of BatchNorm layers in the model is less than the threshold, False otherwise.
         """
         bn = tuple(v for k, v in nn.__dict__.items() if 'Norm' in k)  # normalization layers, i.e. BatchNorm2d()
         return sum(isinstance(v, bn) for v in self.modules()) < thresh  # True if < 'thresh' BatchNorm layers in model
 
-    def info(self, verbose=False, imgsz=640):
+    def info(self, verbose=True, imgsz=640):
         """
         Prints model information
 
         Args:
             verbose (bool): if True, prints out the model information. Defaults to False
             imgsz (int): the size of the image that the model will be trained on. Defaults to 640
         """
-        model_info(self, verbose, imgsz)
+        model_info(self, verbose=verbose, imgsz=imgsz)
 
     def _apply(self, fn):
         """
         `_apply()` is a function that applies a function to all the tensors in the model that are not
         parameters or registered buffers
 
         Args:
@@ -322,17 +322,17 @@
 
 
 # Functions ------------------------------------------------------------------------------------------------------------
 
 
 def torch_safe_load(weight):
     """
-    This function attempts to load a PyTorch model with the torch.load() function. If a ModuleNotFoundError is raised, it
-    catches the error, logs a warning message, and attempts to install the missing module via the check_requirements()
-    function. After installation, the function again attempts to load the model using torch.load().
+    This function attempts to load a PyTorch model with the torch.load() function. If a ModuleNotFoundError is raised,
+    it catches the error, logs a warning message, and attempts to install the missing module via the
+    check_requirements() function. After installation, the function again attempts to load the model using torch.load().
 
     Args:
         weight (str): The file path of the PyTorch model.
 
     Returns:
         The loaded PyTorch model.
     """
@@ -433,15 +433,15 @@
     if act:
         Conv.default_act = eval(act)  # redefine default activation, i.e. Conv.default_act = nn.SiLU()
         if verbose:
             LOGGER.info(f"{colorstr('activation:')} {act}")  # print
     ch = [ch]
     layers, save, c2 = [], [], ch[-1]  # layers, savelist, ch out
     for i, (f, n, m, args) in enumerate(d['backbone'] + d['head']):  # from, number, module, args
-        m = eval(m) if isinstance(m, str) else m  # eval strings
+        m = getattr(torch.nn, m[3:]) if 'nn.' in m else globals()[m]  # get module
         for j, a in enumerate(args):
             # TODO: re-implement with eval() removal if possible
             # args[j] = (locals()[a] if a in locals() else ast.literal_eval(a)) if isinstance(a, str) else a
             with contextlib.suppress(NameError):
                 args[j] = eval(a) if isinstance(a, str) else a  # eval strings
 
         n = n_ = max(round(n * gd), 1) if n > 1 else n  # depth gain
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/tracker/cfg/botsort.yaml` & `syml_ultralytics-8.0.53/ultralytics/tracker/cfg/botsort.yaml`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/tracker/cfg/bytetrack.yaml` & `syml_ultralytics-8.0.53/ultralytics/tracker/cfg/bytetrack.yaml`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/tracker/track.py` & `syml_ultralytics-8.0.53/ultralytics/tracker/track.py`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/tracker/trackers/basetrack.py` & `syml_ultralytics-8.0.53/ultralytics/tracker/trackers/basetrack.py`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/tracker/trackers/bot_sort.py` & `syml_ultralytics-8.0.53/ultralytics/tracker/trackers/bot_sort.py`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/tracker/trackers/byte_tracker.py` & `syml_ultralytics-8.0.53/ultralytics/tracker/trackers/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/tracker/utils/gmc.py` & `syml_ultralytics-8.0.53/ultralytics/tracker/utils/gmc.py`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/tracker/utils/kalman_filter.py` & `syml_ultralytics-8.0.53/ultralytics/tracker/utils/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/tracker/utils/matching.py` & `syml_ultralytics-8.0.53/ultralytics/tracker/utils/matching.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,23 +32,34 @@
     matches = indices[matched_mask]
     unmatched_a = tuple(set(range(cost_matrix.shape[0])) - set(matches[:, 0]))
     unmatched_b = tuple(set(range(cost_matrix.shape[1])) - set(matches[:, 1]))
 
     return matches, unmatched_a, unmatched_b
 
 
-def linear_assignment(cost_matrix, thresh):
+def linear_assignment(cost_matrix, thresh, use_lap=True):
+    # Linear assignment implementations with scipy and lap.lapjv
     if cost_matrix.size == 0:
         return np.empty((0, 2), dtype=int), tuple(range(cost_matrix.shape[0])), tuple(range(cost_matrix.shape[1]))
-    matches, unmatched_a, unmatched_b = [], [], []
-    cost, x, y = lap.lapjv(cost_matrix, extend_cost=True, cost_limit=thresh)
-    matches.extend([ix, mx] for ix, mx in enumerate(x) if mx >= 0)
-    unmatched_a = np.where(x < 0)[0]
-    unmatched_b = np.where(y < 0)[0]
-    matches = np.asarray(matches)
+
+    if use_lap:
+        _, x, y = lap.lapjv(cost_matrix, extend_cost=True, cost_limit=thresh)
+        matches = [[ix, mx] for ix, mx in enumerate(x) if mx >= 0]
+        unmatched_a = np.where(x < 0)[0]
+        unmatched_b = np.where(y < 0)[0]
+    else:
+        # Scipy linear sum assignment is NOT working correctly, DO NOT USE
+        y, x = scipy.optimize.linear_sum_assignment(cost_matrix)  # row y, col x
+        matches = np.asarray([[i, x] for i, x in enumerate(x) if cost_matrix[i, x] <= thresh])
+        unmatched = np.ones(cost_matrix.shape)
+        for i, xi in matches:
+            unmatched[i, xi] = 0.0
+        unmatched_a = np.where(unmatched.all(1))[0]
+        unmatched_b = np.where(unmatched.all(0))[0]
+
     return matches, unmatched_a, unmatched_b
 
 
 def ious(atlbrs, btlbrs):
     """
     Compute cost based on IoU
     :type atlbrs: list[tlbr] | np.ndarray
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/cfg/__init__.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/cfg/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,16 +57,18 @@
 CFG_BOOL_KEYS = ('save', 'exist_ok', 'pretrained', 'verbose', 'deterministic', 'single_cls', 'image_weights', 'rect',
                  'cos_lr', 'overlap_mask', 'val', 'save_json', 'save_hybrid', 'half', 'dnn', 'plots', 'show',
                  'save_txt', 'save_conf', 'save_crop', 'hide_labels', 'hide_conf', 'visualize', 'augment',
                  'agnostic_nms', 'retina_masks', 'boxes', 'keras', 'optimize', 'int8', 'dynamic', 'simplify', 'nms',
                  'v5loader')
 
 # Define valid tasks and modes
-TASKS = 'detect', 'segment', 'classify'
 MODES = 'train', 'val', 'predict', 'export', 'track', 'benchmark'
+TASKS = 'detect', 'segment', 'classify'
+TASK2DATA = {'detect': 'coco128.yaml', 'segment': 'coco128-seg.yaml', 'classify': 'imagenet100'}
+TASK2MODEL = {'detect': 'yolov8n.pt', 'segment': 'yolov8n-seg.pt', 'classify': 'yolov8n-cls.pt'}
 
 
 def cfg2dict(cfg):
     """
     Convert a configuration object to a dictionary, whether it is a file path, a string, or a SimpleNamespace object.
 
     Inputs:
@@ -270,41 +272,44 @@
             raise ValueError(f"Invalid 'mode={mode}'. Valid modes are {MODES}.\n{CLI_HELP_MSG}")
         LOGGER.warning("WARNING ⚠️ 'yolo mode=checks' is deprecated. Use 'yolo checks' instead.")
         checks.check_yolo()
         return
 
     # Task
     task = overrides.pop('task', None)
-    if task and task not in TASKS:
-        raise ValueError(f"Invalid 'task={task}'. Valid tasks are {TASKS}.\n{CLI_HELP_MSG}")
+    if task:
+        if task not in TASKS:
+            raise ValueError(f"Invalid 'task={task}'. Valid tasks are {TASKS}.\n{CLI_HELP_MSG}")
+        if 'model' not in overrides:
+            overrides['model'] = TASK2MODEL[task]
 
     # Model
     model = overrides.pop('model', DEFAULT_CFG.model)
     if model is None:
         model = 'yolov8n.pt'
         LOGGER.warning(f"WARNING ⚠️ 'model' is missing. Using default 'model={model}'.")
     from ultralytics.yolo.engine.model import YOLO
     overrides['model'] = model
     model = YOLO(model, task=task)
 
     # Task Update
-    if task and task != model.task:
-        LOGGER.warning(f"WARNING ⚠️ conflicting 'task={task}' passed with 'task={model.task}' model. "
-                       f"Ignoring 'task={task}' and updating to 'task={model.task}' to match model.")
+    if task != model.task:
+        if task:
+            LOGGER.warning(f"WARNING ⚠️ conflicting 'task={task}' passed with 'task={model.task}' model. "
+                           f"Ignoring 'task={task}' and updating to 'task={model.task}' to match model.")
         task = model.task
 
     # Mode
-    if mode in {'predict', 'track'} and 'source' not in overrides:
+    if mode in ('predict', 'track') and 'source' not in overrides:
         overrides['source'] = DEFAULT_CFG.source or ROOT / 'assets' if (ROOT / 'assets').exists() \
             else 'https://ultralytics.com/images/bus.jpg'
         LOGGER.warning(f"WARNING ⚠️ 'source' is missing. Using default 'source={overrides['source']}'.")
     elif mode in ('train', 'val'):
         if 'data' not in overrides:
-            task2data = dict(detect='coco128.yaml', segment='coco128-seg.yaml', classify='imagenet100')
-            overrides['data'] = task2data.get(task or DEFAULT_CFG.task, DEFAULT_CFG.data)
+            overrides['data'] = TASK2DATA.get(task or DEFAULT_CFG.task, DEFAULT_CFG.data)
             LOGGER.warning(f"WARNING ⚠️ 'data' is missing. Using default 'data={overrides['data']}'.")
     elif mode == 'export':
         if 'format' not in overrides:
             overrides['format'] = DEFAULT_CFG.format or 'torchscript'
             LOGGER.warning(f"WARNING ⚠️ 'format' is missing. Using default 'format={overrides['format']}'.")
 
     # Run command in python
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/cfg/default.yaml` & `syml_ultralytics-8.0.53/ultralytics/yolo/cfg/default.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -2,39 +2,38 @@
 # Default training settings and hyperparameters for medium-augmentation COCO training
 
 task: detect  # inference task, i.e. detect, segment, classify
 mode: train  # YOLO mode, i.e. train, val, predict, export
 
 # Train settings -------------------------------------------------------------------------------------------------------
 model:  # path to model file, i.e. yolov8n.pt, yolov8n.yaml
-data:  # path to data file, i.e. i.e. coco128.yaml
+data:  # path to data file, i.e. coco128.yaml
 epochs: 100  # number of epochs to train for
 patience: 50  # epochs to wait for no observable improvement for early stopping of training
 batch: 16  # number of images per batch (-1 for AutoBatch)
 imgsz: 640  # size of input images as integer or w,h
 save: True  # save train checkpoints and predict results
 save_period: -1 # Save checkpoint every x epochs (disabled if < 1)
 cache: False  # True/ram, disk or False. Use cache for data loading
 device:  # device to run on, i.e. cuda device=0 or device=0,1,2,3 or device=cpu
 workers: 8  # number of worker threads for data loading (per RANK if DDP)
 project:  # project name
-name:  # experiment name
+name:  # experiment name, results saved to 'project/name' directory
 exist_ok: False  # whether to overwrite existing experiment
 pretrained: False  # whether to use a pretrained model
 optimizer: SGD  # optimizer to use, choices=['SGD', 'Adam', 'AdamW', 'RMSProp']
 verbose: True  # whether to print verbose output
 seed: 0  # random seed for reproducibility
 deterministic: True  # whether to enable deterministic mode
 single_cls: False  # train multi-class data as single-class
 image_weights: False  # use weighted image selection for training
 rect: False  # support rectangular training if mode='train', support rectangular evaluation if mode='val'
 cos_lr: False  # use cosine learning rate scheduler
 close_mosaic: 10  # disable mosaic augmentation for final 10 epochs
 resume: False  # resume training from last checkpoint
-min_memory: False  # minimize memory footprint loss function, choices=[False, True, <roll_out_thr>]
 # Segmentation
 overlap_mask: True  # masks should overlap during training (segment train only)
 mask_ratio: 4  # mask downsample ratio (segment train only)
 # Classification
 dropout: 0.0  # use dropout regularization (classify train only)
 
 # Val/Test settings ----------------------------------------------------------------------------------------------------
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/data/augment.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/data/augment.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import torchvision.transforms as T
 
 from ..utils import LOGGER, colorstr
 from ..utils.checks import check_version
 from ..utils.instance import Instances
 from ..utils.metrics import bbox_ioa
 from ..utils.ops import segment2box
-from .utils import IMAGENET_MEAN, IMAGENET_STD, polygons2masks, polygons2masks_overlap
+from .utils import polygons2masks, polygons2masks_overlap
 
 
 # TODO: we might need a BaseTransform to make all these augments be compatible with both classification and semantic
 class BaseTransform:
 
     def __init__(self) -> None:
         pass
@@ -678,31 +678,33 @@
         Albumentations(p=1.0),
         RandomHSV(hgain=hyp.hsv_h, sgain=hyp.hsv_s, vgain=hyp.hsv_v),
         RandomFlip(direction='vertical', p=hyp.flipud),
         RandomFlip(direction='horizontal', p=hyp.fliplr)])  # transforms
 
 
 # Classification augmentations -----------------------------------------------------------------------------------------
-def classify_transforms(size=224):
+def classify_transforms(size=224, mean=(0.0, 0.0, 0.0), std=(1.0, 1.0, 1.0)):  # IMAGENET_MEAN, IMAGENET_STD
     # Transforms to apply if albumentations not installed
     if not isinstance(size, int):
         raise TypeError(f'classify_transforms() size {size} must be integer, not (list, tuple)')
-    # T.Compose([T.ToTensor(), T.Resize(size), T.CenterCrop(size), T.Normalize(IMAGENET_MEAN, IMAGENET_STD)])
-    return T.Compose([CenterCrop(size), ToTensor(), T.Normalize(IMAGENET_MEAN, IMAGENET_STD)])
+    if any(mean) or any(std):
+        return T.Compose([CenterCrop(size), ToTensor(), T.Normalize(mean, std, inplace=True)])
+    else:
+        return T.Compose([CenterCrop(size), ToTensor()])
 
 
 def classify_albumentations(
         augment=True,
         size=224,
         scale=(0.08, 1.0),
         hflip=0.5,
         vflip=0.0,
         jitter=0.4,
-        mean=IMAGENET_MEAN,
-        std=IMAGENET_STD,
+        mean=(0.0, 0.0, 0.0),  # IMAGENET_MEAN
+        std=(1.0, 1.0, 1.0),  # IMAGENET_STD
         auto_aug=False,
 ):
     # YOLOv8 classification Albumentations (optional, only used if package is installed)
     prefix = colorstr('albumentations: ')
     try:
         import albumentations as A
         from albumentations.pytorch import ToTensorV2
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/data/base.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/data/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,26 +31,26 @@
                  augment=True,
                  hyp=None,
                  prefix='',
                  rect=False,
                  batch_size=None,
                  stride=32,
                  pad=0.5,
-                 single_cls=False):
+                 single_cls=False,
+                 classes=None):
         super().__init__()
         self.img_path = img_path
         self.imgsz = imgsz
         self.augment = augment
         self.single_cls = single_cls
         self.prefix = prefix
 
         self.im_files = self.get_img_files(self.img_path)
         self.labels = self.get_labels()
-        if self.single_cls:
-            self.update_labels(include_class=[])
+        self.update_labels(include_class=classes)  # single_cls and include_class
 
         self.ni = len(self.labels)
 
         # rect stuff
         self.rect = rect
         self.batch_size = batch_size
         self.stride = stride
@@ -92,23 +92,23 @@
             raise FileNotFoundError(f'{self.prefix}Error loading data from {img_path}\n{HELP_URL}') from e
         return im_files
 
     def update_labels(self, include_class: Optional[list]):
         """include_class, filter labels to include only these classes (optional)"""
         include_class_array = np.array(include_class).reshape(1, -1)
         for i in range(len(self.labels)):
-            if include_class:
+            if include_class is not None:
                 cls = self.labels[i]['cls']
                 bboxes = self.labels[i]['bboxes']
                 segments = self.labels[i]['segments']
                 j = (cls == include_class_array).any(1)
                 self.labels[i]['cls'] = cls[j]
                 self.labels[i]['bboxes'] = bboxes[j]
                 if segments:
-                    self.labels[i]['segments'] = segments[j]
+                    self.labels[i]['segments'] = [segments[si] for si, idx in enumerate(j) if idx]
             if self.single_cls:
                 self.labels[i]['cls'][:, 0] = 0
 
     def load_image(self, i):
         # Loads 1 image from dataset index 'i', returns (im, resized hw)
         im, f, fn = self.ims[i], self.im_files[i], self.npy_files[i]
         if im is None:  # not cached in RAM
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/data/build.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/data/build.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import numpy as np
 import torch
 from PIL import Image
 from torch.utils.data import DataLoader, dataloader, distributed
 
 from ultralytics.yolo.data.dataloaders.stream_loaders import (LOADERS, LoadImages, LoadPilAndNumpy, LoadScreenshots,
-                                                              LoadStreams, SourceTypes, autocast_list)
+                                                              LoadStreams, LoadTensor, SourceTypes, autocast_list)
 from ultralytics.yolo.data.utils import IMG_FORMATS, VID_FORMATS
 from ultralytics.yolo.utils.checks import check_file
 
 from ..utils import LOGGER, colorstr
 from ..utils.torch_utils import torch_distributed_zero_first
 from .dataset import ClassificationDataset, YOLODataset
 from .utils import PIN_MEMORY, RANK
@@ -78,15 +78,16 @@
             cache=cfg.cache or None,
             single_cls=cfg.single_cls or False,
             stride=int(stride),
             pad=0.0 if mode == 'train' else 0.5,
             prefix=colorstr(f'{mode}: '),
             use_segments=cfg.task == 'segment',
             use_keypoints=cfg.task == 'keypoint',
-            names=names)
+            names=names,
+            classes=cfg.classes)
 
     batch = min(batch, len(dataset))
     nd = torch.cuda.device_count()  # number of CUDA devices
     workers = cfg.workers if mode == 'train' else cfg.workers * 2
     nw = min([os.cpu_count() // max(nd, 1), batch if batch > 1 else 0, workers])  # number of workers
     sampler = None if rank == -1 else distributed.DistributedSampler(dataset, shuffle=shuffle)
     loader = DataLoader if cfg.image_weights or cfg.close_mosaic else InfiniteDataLoader  # allow attribute updates
@@ -129,15 +130,15 @@
                               sampler=sampler,
                               pin_memory=PIN_MEMORY,
                               worker_init_fn=seed_worker,
                               generator=generator)  # or DataLoader(persistent_workers=True)
 
 
 def check_source(source):
-    webcam, screenshot, from_img, in_memory = False, False, False, False
+    webcam, screenshot, from_img, in_memory, tensor = False, False, False, False, False
     if isinstance(source, (str, int, Path)):  # int for local usb camera
         source = str(source)
         is_file = Path(source).suffix[1:] in (IMG_FORMATS + VID_FORMATS)
         is_url = source.lower().startswith(('https://', 'http://', 'rtsp://', 'rtmp://'))
         webcam = source.isnumeric() or source.endswith('.streams') or (is_url and not is_file)
         screenshot = source.lower().startswith('screen')
         if is_url and is_file:
@@ -145,30 +146,33 @@
     elif isinstance(source, tuple(LOADERS)):
         in_memory = True
     elif isinstance(source, (list, tuple)):
         source = autocast_list(source)  # convert all list elements to PIL or np arrays
         from_img = True
     elif isinstance(source, (Image.Image, np.ndarray)):
         from_img = True
+    elif isinstance(source, torch.Tensor):
+        tensor = True
     else:
         raise TypeError('Unsupported image type. See docs for supported types https://docs.ultralytics.com/predict')
 
-    return source, webcam, screenshot, from_img, in_memory
+    return source, webcam, screenshot, from_img, in_memory, tensor
 
 
 def load_inference_source(source=None, transforms=None, imgsz=640, vid_stride=1, stride=32, auto=True):
     """
     TODO: docs
     """
-    # source
-    source, webcam, screenshot, from_img, in_memory = check_source(source)
-    source_type = source.source_type if in_memory else SourceTypes(webcam, screenshot, from_img)
+    source, webcam, screenshot, from_img, in_memory, tensor = check_source(source)
+    source_type = source.source_type if in_memory else SourceTypes(webcam, screenshot, from_img, tensor)
 
     # Dataloader
-    if in_memory:
+    if tensor:
+        dataset = LoadTensor(source)
+    elif in_memory:
         dataset = source
     elif webcam:
         dataset = LoadStreams(source,
                               imgsz=imgsz,
                               stride=stride,
                               auto=auto,
                               transforms=transforms,
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/data/dataloaders/stream_loaders.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/data/dataloaders/stream_loaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 
 @dataclass
 class SourceTypes:
     webcam: bool = False
     screenshot: bool = False
     from_img: bool = False
+    tensor: bool = False
 
 
 class LoadStreams:
     # YOLOv8 streamloader, i.e. `yolo predict source='rtsp://example.com/media.mp4'  # RTSP, RTMP, HTTP streams`
     def __init__(self, sources='file.streams', imgsz=640, stride=32, auto=True, transforms=None, vid_stride=1):
         torch.backends.cudnn.benchmark = True  # faster for fixed-size inference
         self.mode = 'stream'
@@ -325,14 +326,31 @@
         return self.paths, im, self.im0, None, ''
 
     def __iter__(self):
         self.count = 0
         return self
 
 
+class LoadTensor:
+
+    def __init__(self, imgs) -> None:
+        self.im0 = imgs
+        self.bs = imgs.shape[0]
+
+    def __iter__(self):
+        self.count = 0
+        return self
+
+    def __next__(self):
+        if self.count == 1:
+            raise StopIteration
+        self.count += 1
+        return None, self.im0, self.im0, None, ''  # self.paths, im, self.im0, None, ''
+
+
 def autocast_list(source):
     """
     Merges a list of source of different types into a list of numpy arrays or PIL images
     """
     files = []
     for im in source:
         if isinstance(im, (str, Path)):  # filename or uri
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/data/dataloaders/v5augmentations.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/data/dataloaders/v5augmentations.py`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/data/dataloaders/v5loader.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/data/dataloaders/v5loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -492,15 +492,15 @@
             assert cache['version'] == self.cache_version  # matches current version
             assert cache['hash'] == get_hash(self.label_files + self.im_files)  # identical hash
         except (FileNotFoundError, AssertionError, AttributeError):
             cache, exists = self.cache_labels(cache_path, prefix), False  # run cache ops
 
         # Display cache
         nf, nm, ne, nc, n = cache.pop('results')  # found, missing, empty, corrupt, total
-        if exists and LOCAL_RANK in {-1, 0}:
+        if exists and LOCAL_RANK in (-1, 0):
             d = f'Scanning {cache_path}... {nf} images, {nm + ne} backgrounds, {nc} corrupt'
             tqdm(None, desc=prefix + d, total=n, initial=n, bar_format=TQDM_BAR_FORMAT)  # display cache results
             if cache['msgs']:
                 LOGGER.info('\n'.join(cache['msgs']))  # display warnings
         assert nf > 0 or not augment, f'{prefix}No labels found in {cache_path}, can not start training. {HELP_URL}'
 
         # Read cache
@@ -535,15 +535,15 @@
         include_class = []  # filter labels to include only these classes (optional)
         include_class_array = np.array(include_class).reshape(1, -1)
         for i, (label, segment) in enumerate(zip(self.labels, self.segments)):
             if include_class:
                 j = (label[:, 0:1] == include_class_array).any(1)
                 self.labels[i] = label[j]
                 if segment:
-                    self.segments[i] = segment[j]
+                    self.segments[i] = [segment[si] for si, idx in enumerate(j) if idx]
             if single_cls:  # single-class training, merge all classes into 0
                 self.labels[i][:, 0] = 0
 
         # Rectangular Training
         if self.rect:
             # Sort by aspect ratio
             s = self.shapes  # wh
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/data/dataset.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/data/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,20 +53,22 @@
                  rect=False,
                  batch_size=None,
                  stride=32,
                  pad=0.0,
                  single_cls=False,
                  use_segments=False,
                  use_keypoints=False,
-                 names=None):
+                 names=None,
+                 classes=None):
         self.use_segments = use_segments
         self.use_keypoints = use_keypoints
         self.names = names
         assert not (self.use_segments and self.use_keypoints), 'Can not use both segments and keypoints.'
-        super().__init__(img_path, imgsz, cache, augment, hyp, prefix, rect, batch_size, stride, pad, single_cls)
+        super().__init__(img_path, imgsz, cache, augment, hyp, prefix, rect, batch_size, stride, pad, single_cls,
+                         classes)
 
     def cache_labels(self, path=Path('./labels.cache')):
         """Cache dataset labels, check images and read shapes.
         Args:
             path (Path): path where to save the cache file (default: Path('./labels.cache')).
         Returns:
             (dict): labels.
@@ -127,15 +129,15 @@
             assert cache['version'] == self.cache_version  # matches current version
             assert cache['hash'] == get_hash(self.label_files + self.im_files)  # identical hash
         except (FileNotFoundError, AssertionError, AttributeError):
             cache, exists = self.cache_labels(cache_path), False  # run cache ops
 
         # Display cache
         nf, nm, ne, nc, n = cache.pop('results')  # found, missing, empty, corrupt, total
-        if exists and LOCAL_RANK in {-1, 0}:
+        if exists and LOCAL_RANK in (-1, 0):
             d = f'Scanning {cache_path}... {nf} images, {nm + ne} backgrounds, {nc} corrupt'
             tqdm(None, desc=self.prefix + d, total=n, initial=n, bar_format=TQDM_BAR_FORMAT)  # display cache results
             if cache['msgs']:
                 LOGGER.info('\n'.join(cache['msgs']))  # display warnings
         if nf == 0:  # number of labels found
             raise FileNotFoundError(f'{self.prefix}No labels found in {cache_path}, can not start training. {HELP_URL}')
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/data/dataset_wrappers.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/data/dataset_wrappers.py`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/data/utils.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/data/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,22 +12,23 @@
 from zipfile import is_zipfile
 
 import cv2
 import numpy as np
 from PIL import ExifTags, Image, ImageOps
 from tqdm import tqdm
 
+from ultralytics.nn.autobackend import check_class_names
 from ultralytics.yolo.utils import DATASETS_DIR, LOGGER, NUM_THREADS, ROOT, colorstr, emojis, yaml_load
 from ultralytics.yolo.utils.checks import check_file, check_font, is_ascii
 from ultralytics.yolo.utils.downloads import download, safe_download, unzip_file
 from ultralytics.yolo.utils.ops import segments2boxes
 
 HELP_URL = 'See https://github.com/ultralytics/yolov5/wiki/Train-Custom-Data'
-IMG_FORMATS = 'bmp', 'dng', 'jpeg', 'jpg', 'mpo', 'png', 'tif', 'tiff', 'webp', 'pfm'  # include image suffixes
-VID_FORMATS = 'asf', 'avi', 'gif', 'm4v', 'mkv', 'mov', 'mp4', 'mpeg', 'mpg', 'ts', 'wmv'  # include video suffixes
+IMG_FORMATS = 'bmp', 'dng', 'jpeg', 'jpg', 'mpo', 'png', 'tif', 'tiff', 'webp', 'pfm'  # image suffixes
+VID_FORMATS = 'asf', 'avi', 'gif', 'm4v', 'mkv', 'mov', 'mp4', 'mpeg', 'mpg', 'ts', 'wmv', 'webm'  # video suffixes
 LOCAL_RANK = int(os.getenv('LOCAL_RANK', -1))  # https://pytorch.org/docs/stable/elastic/run.html
 RANK = int(os.getenv('RANK', -1))
 PIN_MEMORY = str(os.getenv('PIN_MEMORY', True)).lower() == 'true'  # global pin_memory for dataloaders
 IMAGENET_MEAN = 0.485, 0.456, 0.406  # RGB mean
 IMAGENET_STD = 0.229, 0.224, 0.225  # RGB standard deviation
 
 # Get orientation exif tag
@@ -205,18 +206,16 @@
     if isinstance(data, (str, Path)):
         data = yaml_load(data, append_filename=True)  # dictionary
 
     # Checks
     for k in 'train', 'val', 'names':
         if k not in data:
             raise SyntaxError(
-                emojis(f"{dataset} '{k}:' key missing ❌.\n"
-                       f"'train', 'val' and 'names' are required in data.yaml files."))
-    if isinstance(data['names'], (list, tuple)):  # old array format
-        data['names'] = dict(enumerate(data['names']))  # convert to dict
+                emojis(f"{dataset} '{k}:' key missing ❌.\n'train', 'val' and 'names' are required in all data YAMLs."))
+    data['names'] = check_class_names(data['names'])
     data['nc'] = len(data['names'])
 
     # Resolve paths
     path = Path(extract_dir or data.get('path') or Path(data.get('yaml_file', '')).parent)  # dataset root
 
     if not path.is_absolute():
         path = (DATASETS_DIR / path).resolve()
@@ -232,19 +231,19 @@
                 data[k] = [str((path / x).resolve()) for x in data[k]]
 
     # Parse yaml
     train, val, test, s = (data.get(x) for x in ('train', 'val', 'test', 'download'))
     if val:
         val = [Path(x).resolve() for x in (val if isinstance(val, list) else [val])]  # val path
         if not all(x.exists() for x in val):
-            msg = f"\nDataset '{dataset}' not found ⚠️, missing paths %s" % [str(x) for x in val if not x.exists()]
+            m = f"\nDataset '{dataset}' images not found ⚠️, missing paths %s" % [str(x) for x in val if not x.exists()]
             if s and autodownload:
-                LOGGER.warning(msg)
+                LOGGER.warning(m)
             else:
-                raise FileNotFoundError(msg)
+                raise FileNotFoundError(m)
             t = time.time()
             if s.startswith('http') and s.endswith('.zip'):  # URL
                 safe_download(url=s, dir=DATASETS_DIR, delete=True)
                 r = None  # success
             elif s.startswith('bash '):  # bash script
                 LOGGER.info(f'Running {s} ...')
                 r = os.system(s)
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/engine/exporter.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/engine/exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,54 +53,47 @@
 import subprocess
 import time
 import warnings
 from collections import defaultdict
 from copy import deepcopy
 from pathlib import Path
 
-import numpy as np
-import pandas as pd
 import torch
 
 from ultralytics.nn.autobackend import check_class_names
 from ultralytics.nn.modules import C2f, Detect, Segment
 from ultralytics.nn.tasks import DetectionModel, SegmentationModel
 from ultralytics.yolo.cfg import get_cfg
-from ultralytics.yolo.data.dataloaders.stream_loaders import LoadImages
-from ultralytics.yolo.data.utils import IMAGENET_MEAN, IMAGENET_STD, check_det_dataset
 from ultralytics.yolo.utils import (DEFAULT_CFG, LINUX, LOGGER, MACOS, __version__, callbacks, colorstr,
                                     get_default_args, yaml_save)
-from ultralytics.yolo.utils.checks import check_imgsz, check_requirements, check_version, check_yaml
+from ultralytics.yolo.utils.checks import check_imgsz, check_requirements, check_version
 from ultralytics.yolo.utils.files import file_size
 from ultralytics.yolo.utils.ops import Profile
 from ultralytics.yolo.utils.torch_utils import get_latest_opset, select_device, smart_inference_mode
 
 ARM64 = platform.machine() in ('arm64', 'aarch64')
 
 
 def export_formats():
     # YOLOv8 export formats
+    import pandas
     x = [
         ['PyTorch', '-', '.pt', True, True],
         ['TorchScript', 'torchscript', '.torchscript', True, True],
         ['ONNX', 'onnx', '.onnx', True, True],
         ['OpenVINO', 'openvino', '_openvino_model', True, False],
         ['TensorRT', 'engine', '.engine', False, True],
         ['CoreML', 'coreml', '.mlmodel', True, False],
         ['TensorFlow SavedModel', 'saved_model', '_saved_model', True, True],
         ['TensorFlow GraphDef', 'pb', '.pb', True, True],
         ['TensorFlow Lite', 'tflite', '.tflite', True, False],
         ['TensorFlow Edge TPU', 'edgetpu', '_edgetpu.tflite', True, False],
         ['TensorFlow.js', 'tfjs', '_web_model', True, False],
         ['PaddlePaddle', 'paddle', '_paddle_model', True, True], ]
-    return pd.DataFrame(x, columns=['Format', 'Argument', 'Suffix', 'CPU', 'GPU'])
-
-
-EXPORT_FORMATS_LIST = list(export_formats()['Argument'][1:])
-EXPORT_FORMATS_TABLE = str(export_formats())
+    return pandas.DataFrame(x, columns=['Format', 'Argument', 'Suffix', 'CPU', 'GPU'])
 
 
 def gd_outputs(gd):
     # TensorFlow GraphDef model output node names
     name_list, input_list = [], []
     for node in gd.node:  # tensorflow.core.framework.node_def_pb2.NodeDef
         name_list.append(node.name)
@@ -150,15 +143,15 @@
         callbacks.add_integration_callbacks(self)
 
     @smart_inference_mode()
     def __call__(self, model=None):
         self.run_callbacks('on_export_start')
         t = time.time()
         format = self.args.format.lower()  # to lowercase
-        if format in {'tensorrt', 'trt'}:  # engine aliases
+        if format in ('tensorrt', 'trt'):  # engine aliases
             format = 'engine'
         fmts = tuple(export_formats()['Argument'][1:])  # available export formats
         flags = [x == format for x in fmts]
         if sum(flags) != 1:
             raise ValueError(f"Invalid export format='{format}'. Valid formats are {fmts}")
         jit, onnx, xml, engine, coreml, saved_model, pb, tflite, edgetpu, tfjs, paddle = flags  # export booleans
 
@@ -410,16 +403,14 @@
         LOGGER.info(f'\n{prefix} starting export with coremltools {ct.__version__}...')
         f = self.file.with_suffix('.mlmodel')
 
         bias = [0.0, 0.0, 0.0]
         scale = 1 / 255
         classifier_config = None
         if self.model.task == 'classify':
-            bias = [-x for x in IMAGENET_MEAN]
-            scale = 1 / 255 / (sum(IMAGENET_STD) / 3)
             classifier_config = ct.ClassifierConfig(list(self.model.names.values())) if self.args.nms else None
             model = self.model
         elif self.model.task == 'detect':
             model = iOSDetectModel(self.model, self.im) if self.args.nms else self.model
         elif self.model.task == 'segment':
             # TODO CoreML Segmentation model pipelining
             model = self.model
@@ -533,15 +524,15 @@
         # Export to ONNX
         self.args.simplify = True
         f_onnx, _ = self._export_onnx()
 
         # Export to TF
         int8 = '-oiqt -qt per-tensor' if self.args.int8 else ''
         cmd = f'onnx2tf -i {f_onnx} -o {f} -nuo --non_verbose {int8}'
-        LOGGER.info(f'\n{prefix} running {cmd}')
+        LOGGER.info(f"\n{prefix} running '{cmd.strip()}'")
         subprocess.run(cmd, shell=True)
         yaml_save(f / 'metadata.yaml', self.metadata)  # add metadata.yaml
 
         # Add TFLite metadata
         for file in f.rglob('*.tflite'):
             self._add_tflite_metadata(file)
 
@@ -570,55 +561,55 @@
     def _export_tflite(self, keras_model, nms, agnostic_nms, prefix=colorstr('TensorFlow Lite:')):
         # YOLOv8 TensorFlow Lite export
         import tensorflow as tf  # noqa
 
         LOGGER.info(f'\n{prefix} starting export with tensorflow {tf.__version__}...')
         saved_model = Path(str(self.file).replace(self.file.suffix, '_saved_model'))
         if self.args.int8:
-            f = saved_model / (self.file.stem + 'yolov8n_integer_quant.tflite')  # fp32 in/out
+            f = saved_model / f'{self.file.stem}_integer_quant.tflite'  # fp32 in/out
         elif self.args.half:
-            f = saved_model / (self.file.stem + '_float16.tflite')
+            f = saved_model / f'{self.file.stem}_float16.tflite'
         else:
-            f = saved_model / (self.file.stem + '_float32.tflite')
-        return str(f), None  # noqa
-
-        # OLD VERSION BELOW ---------------------------------------------------------------
-        batch_size, ch, *imgsz = list(self.im.shape)  # BCHW
-        f = str(self.file).replace(self.file.suffix, '-fp16.tflite')
-
-        converter = tf.lite.TFLiteConverter.from_keras_model(keras_model)
-        converter.target_spec.supported_ops = [tf.lite.OpsSet.TFLITE_BUILTINS]
-        converter.target_spec.supported_types = [tf.float16]
-        converter.optimizations = [tf.lite.Optimize.DEFAULT]
-        if self.args.int8:
+            f = saved_model / f'{self.file.stem}_float32.tflite'
+        return str(f), None
 
-            def representative_dataset_gen(dataset, n_images=100):
-                # Dataset generator for use with converter.representative_dataset, returns a generator of np arrays
-                for n, (path, img, im0s, vid_cap, string) in enumerate(dataset):
-                    im = np.transpose(img, [1, 2, 0])
-                    im = np.expand_dims(im, axis=0).astype(np.float32)
-                    im /= 255
-                    yield [im]
-                    if n >= n_images:
-                        break
-
-            dataset = LoadImages(check_det_dataset(check_yaml(self.args.data))['train'], imgsz=imgsz, auto=False)
-            converter.representative_dataset = lambda: representative_dataset_gen(dataset, n_images=100)
-            converter.target_spec.supported_ops = [tf.lite.OpsSet.TFLITE_BUILTINS_INT8]
-            converter.target_spec.supported_types = []
-            converter.inference_input_type = tf.uint8  # or tf.int8
-            converter.inference_output_type = tf.uint8  # or tf.int8
-            converter.experimental_new_quantizer = True
-            f = str(self.file).replace(self.file.suffix, '-int8.tflite')
-        if nms or agnostic_nms:
-            converter.target_spec.supported_ops.append(tf.lite.OpsSet.SELECT_TF_OPS)
-
-        tflite_model = converter.convert()
-        open(f, 'wb').write(tflite_model)
-        return f, None
+        # # OLD TFLITE EXPORT CODE BELOW -------------------------------------------------------------------------------
+        # batch_size, ch, *imgsz = list(self.im.shape)  # BCHW
+        # f = str(self.file).replace(self.file.suffix, '-fp16.tflite')
+        #
+        # converter = tf.lite.TFLiteConverter.from_keras_model(keras_model)
+        # converter.target_spec.supported_ops = [tf.lite.OpsSet.TFLITE_BUILTINS]
+        # converter.target_spec.supported_types = [tf.float16]
+        # converter.optimizations = [tf.lite.Optimize.DEFAULT]
+        # if self.args.int8:
+        #
+        #     def representative_dataset_gen(dataset, n_images=100):
+        #         # Dataset generator for use with converter.representative_dataset, returns a generator of np arrays
+        #         for n, (path, img, im0s, vid_cap, string) in enumerate(dataset):
+        #             im = np.transpose(img, [1, 2, 0])
+        #             im = np.expand_dims(im, axis=0).astype(np.float32)
+        #             im /= 255
+        #             yield [im]
+        #             if n >= n_images:
+        #                 break
+        #
+        #     dataset = LoadImages(check_det_dataset(self.args.data)['train'], imgsz=imgsz, auto=False)
+        #     converter.representative_dataset = lambda: representative_dataset_gen(dataset, n_images=100)
+        #     converter.target_spec.supported_ops = [tf.lite.OpsSet.TFLITE_BUILTINS_INT8]
+        #     converter.target_spec.supported_types = []
+        #     converter.inference_input_type = tf.uint8  # or tf.int8
+        #     converter.inference_output_type = tf.uint8  # or tf.int8
+        #     converter.experimental_new_quantizer = True
+        #     f = str(self.file).replace(self.file.suffix, '-int8.tflite')
+        # if nms or agnostic_nms:
+        #     converter.target_spec.supported_ops.append(tf.lite.OpsSet.SELECT_TF_OPS)
+        #
+        # tflite_model = converter.convert()
+        # open(f, 'wb').write(tflite_model)
+        # return f, None
 
     @try_export
     def _export_edgetpu(self, tflite_model='', prefix=colorstr('Edge TPU:')):
         # YOLOv8 Edge TPU export https://coral.ai/docs/edgetpu/models-intro/
         LOGGER.warning(f'{prefix} WARNING ⚠️ Edge TPU known bug https://github.com/ultralytics/ultralytics/issues/1185')
 
         cmd = 'edgetpu_compiler --version'
@@ -634,14 +625,15 @@
                 subprocess.run(c if sudo else c.replace('sudo ', ''), shell=True, check=True)
         ver = subprocess.run(cmd, shell=True, capture_output=True, check=True).stdout.decode().split()[-1]
 
         LOGGER.info(f'\n{prefix} starting export with Edge TPU compiler {ver}...')
         f = str(tflite_model).replace('.tflite', '_edgetpu.tflite')  # Edge TPU model
 
         cmd = f'edgetpu_compiler -s -d -k 10 --out_dir {Path(f).parent} {tflite_model}'
+        LOGGER.info(f"{prefix} running '{cmd}'")
         subprocess.run(cmd.split(), check=True)
         self._add_tflite_metadata(f)
         return f, None
 
     @try_export
     def _export_tfjs(self, prefix=colorstr('TensorFlow.js:')):
         # YOLOv8 TensorFlow.js export
@@ -859,26 +851,14 @@
             callback(self)
 
 
 def export(cfg=DEFAULT_CFG):
     cfg.model = cfg.model or 'yolov8n.yaml'
     cfg.format = cfg.format or 'torchscript'
 
-    # exporter = Exporter(cfg)
-    #
-    # model = None
-    # if isinstance(cfg.model, (str, Path)):
-    #     if Path(cfg.model).suffix == '.yaml':
-    #         model = DetectionModel(cfg.model)
-    #     elif Path(cfg.model).suffix == '.pt':
-    #         model = attempt_load_weights(cfg.model, fuse=True)
-    #     else:
-    #         TypeError(f'Unsupported model type {cfg.model}')
-    # exporter(model=model)
-
     from ultralytics import YOLO
     model = YOLO(cfg.model)
     model.export(**vars(cfg))
 
 
 if __name__ == '__main__':
     """
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/engine/model.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/engine/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ultralytics import yolo  # noqa
 from ultralytics.nn.tasks import (ClassificationModel, DetectionModel, SegmentationModel, attempt_load_one_weight,
                                   guess_model_task, nn)
 from ultralytics.yolo.cfg import get_cfg
 from ultralytics.yolo.engine.exporter import Exporter
 from ultralytics.yolo.utils import (DEFAULT_CFG, DEFAULT_CFG_DICT, DEFAULT_CFG_KEYS, LOGGER, ONLINE, RANK, ROOT,
                                     callbacks, is_git_dir, is_pip_package, yaml_load)
-from ultralytics.yolo.utils.checks import check_file, check_imgsz, check_pip_update, check_yaml
+from ultralytics.yolo.utils.checks import check_file, check_imgsz, check_pip_update_available, check_yaml
 from ultralytics.yolo.utils.downloads import GITHUB_ASSET_STEMS
 from ultralytics.yolo.utils.torch_utils import smart_inference_mode
 
 # Map head to model, trainer, validator, and predictor classes
 TASK_MAP = {
     'classify': [
         ClassificationModel, yolo.v8.classify.ClassificationTrainer, yolo.v8.classify.ClassificationValidator,
@@ -154,15 +154,15 @@
                             f"support 'predict' and 'val' modes, i.e. 'yolo predict model=yolov8n.onnx'.")
 
     def _check_pip_update(self):
         """
         Inform user of ultralytics package update availability
         """
         if ONLINE and is_pip_package():
-            check_pip_update()
+            check_pip_update_available()
 
     def reset(self):
         """
         Resets the model modules.
         """
         self._check_is_pytorch_model()
         for m in self.model.modules():
@@ -199,28 +199,29 @@
 
         Returns:
             (List[ultralytics.yolo.engine.results.Results]): The prediction results.
         """
         if source is None:
             source = ROOT / 'assets' if is_git_dir() else 'https://ultralytics.com/images/bus.jpg'
             LOGGER.warning(f"WARNING ⚠️ 'source' is missing. Using 'source={source}'.")
+        is_cli = (sys.argv[0].endswith('yolo') or sys.argv[0].endswith('ultralytics')) and \
+                 ('predict' in sys.argv or 'mode=predict' in sys.argv)
 
         overrides = self.overrides.copy()
         overrides['conf'] = 0.25
         overrides.update(kwargs)  # prefer kwargs
         overrides['mode'] = kwargs.get('mode', 'predict')
         assert overrides['mode'] in ['track', 'predict']
         overrides['save'] = kwargs.get('save', False)  # not save files by default
         if not self.predictor:
             self.task = overrides.get('task') or self.task
             self.predictor = TASK_MAP[self.task][3](overrides=overrides)
-            self.predictor.setup_model(model=self.model)
+            self.predictor.setup_model(model=self.model, verbose=is_cli)
         else:  # only update args if predictor is already setup
             self.predictor.args = get_cfg(self.predictor.args, overrides)
-        is_cli = sys.argv[0].endswith('yolo') or sys.argv[0].endswith('ultralytics')
         return self.predictor.predict_cli(source=source) if is_cli else self.predictor(source=source, stream=stream)
 
     def track(self, source=None, stream=False, **kwargs):
         from ultralytics.tracker import register_tracker
         register_tracker(self)
         # ByteTrack-based method needs low confidence predictions as input
         conf = kwargs.get('conf') or 0.1
@@ -314,15 +315,15 @@
         self.trainer = TASK_MAP[self.task][1](overrides=overrides)
         if not overrides.get('resume'):  # manually set model only if not resuming
             self.trainer.model = self.trainer.get_model(weights=self.model if self.ckpt else None, cfg=self.model.yaml)
             self.model = self.trainer.model
         self.trainer.hub_session = self.session  # attach optional HUB session
         self.trainer.train()
         # update model and cfg after training
-        if RANK in {0, -1}:
+        if RANK in (-1, 0):
             self.model, _ = attempt_load_one_weight(str(self.trainer.best))
             self.overrides = self.model.args
             self.metrics = getattr(self.trainer.validator, 'metrics', None)  # TODO: no metrics returned by DDP
 
     def to(self, device):
         """
         Sends the model to the given device.
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/engine/predictor.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/engine/predictor.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,14 +179,16 @@
             # visualize, save, write results
             n = len(im)
             for i in range(n):
                 self.results[i].speed = {
                     'preprocess': self.dt[0].dt * 1E3 / n,
                     'inference': self.dt[1].dt * 1E3 / n,
                     'postprocess': self.dt[2].dt * 1E3 / n}
+                if self.source_type.tensor:  # skip write, show and plot operations if input is raw tensor
+                    continue
                 p, im0 = (path[i], im0s[i].copy()) if self.source_type.webcam or self.source_type.from_img \
                     else (path, im0s.copy())
                 p = Path(p)
 
                 if self.args.verbose or self.args.save or self.args.save_txt or self.args.show:
                     s += self.write_results(i, self.results, (p, im, im0))
 
@@ -214,19 +216,24 @@
         if self.args.save or self.args.save_txt or self.args.save_crop:
             nl = len(list(self.save_dir.glob('labels/*.txt')))  # number of labels
             s = f"\n{nl} label{'s' * (nl > 1)} saved to {self.save_dir / 'labels'}" if self.args.save_txt else ''
             LOGGER.info(f"Results saved to {colorstr('bold', self.save_dir)}{s}")
 
         self.run_callbacks('on_predict_end')
 
-    def setup_model(self, model):
-        device = select_device(self.args.device)
+    def setup_model(self, model, verbose=True):
+        device = select_device(self.args.device, verbose=verbose)
         model = model or self.args.model
         self.args.half &= device.type != 'cpu'  # half precision only supported on CUDA
-        self.model = AutoBackend(model, device=device, dnn=self.args.dnn, data=self.args.data, fp16=self.args.half)
+        self.model = AutoBackend(model,
+                                 device=device,
+                                 dnn=self.args.dnn,
+                                 data=self.args.data,
+                                 fp16=self.args.half,
+                                 verbose=verbose)
         self.device = device
         self.model.eval()
 
     def show(self, p):
         im0 = self.annotator.result()
         if platform.system() == 'Linux' and p not in self.windows:
             self.windows.append(p)
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/engine/results.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/engine/results.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Ultralytics YOLO 🚀, GPL-3.0 license
 """
 Ultralytics Results, Boxes and Masks classes for handling inference results
 
-Usage: See https://docs.ultralytics.com/predict/
+Usage: See https://docs.ultralytics.com/modes/predict/
 """
 
 import pprint
 from copy import deepcopy
 from functools import lru_cache
 
 import numpy as np
@@ -44,15 +44,15 @@
         self.orig_img = orig_img
         self.orig_shape = orig_img.shape[:2]
         self.boxes = Boxes(boxes, self.orig_shape) if boxes is not None else None  # native size boxes
         self.masks = Masks(masks, self.orig_shape) if masks is not None else None  # native size or imgsz masks
         self.probs = probs if probs is not None else None
         self.names = names
         self.path = path
-        self._keys = (k for k in ('boxes', 'masks', 'probs') if getattr(self, k) is not None)
+        self._keys = [k for k in ('boxes', 'masks', 'probs') if getattr(self, k) is not None]
 
     def pandas(self):
         pass
         # TODO masks.pandas + boxes.pandas + cls.pandas
 
     def __getitem__(self, idx):
         r = Results(orig_img=self.orig_img, path=self.path, names=self.names)
@@ -118,39 +118,38 @@
             font (str): The font to use for the text.
             pil (bool): Whether to return the image as a PIL Image.
             example (str): An example string to display. Useful for indicating the expected format of the output.
 
         Returns:
             (None) or (PIL.Image): If `pil` is True, a PIL Image is returned. Otherwise, nothing is returned.
         """
-        img = deepcopy(self.orig_img)
-        annotator = Annotator(img, line_width, font_size, font, pil, example)
+        annotator = Annotator(deepcopy(self.orig_img), line_width, font_size, font, pil, example)
         boxes = self.boxes
         masks = self.masks
         logits = self.probs
         names = self.names
         if boxes is not None:
             for d in reversed(boxes):
                 cls, conf = d.cls.squeeze(), d.conf.squeeze()
                 c = int(cls)
                 label = (f'{names[c]}' if names else f'{c}') + (f'{conf:.2f}' if show_conf else '')
                 annotator.box_label(d.xyxy.squeeze(), label, color=colors(c, True))
 
         if masks is not None:
-            im = torch.as_tensor(img, dtype=torch.float16, device=masks.data.device).permute(2, 0, 1).flip(0)
+            im = torch.as_tensor(annotator.im, dtype=torch.float16, device=masks.data.device).permute(2, 0, 1).flip(0)
             im = F.resize(im.contiguous(), masks.data.shape[1:]) / 255
             annotator.masks(masks.data, colors=[colors(x, True) for x in boxes.cls], im_gpu=im)
 
         if logits is not None:
             n5 = min(len(self.names), 5)
             top5i = logits.argsort(0, descending=True)[:n5].tolist()  # top 5 indices
             text = f"{', '.join(f'{names[j] if names else j} {logits[j]:.2f}' for j in top5i)}, "
             annotator.text((32, 32), text, txt_color=(255, 255, 255))  # TODO: allow setting colors
 
-        return img
+        return np.asarray(annotator.im) if annotator.pil else annotator.im
 
 
 class Boxes:
     """
     A class for storing and manipulating detection boxes.
 
     Args:
@@ -182,15 +181,15 @@
         pandas(): Convert the object to a pandas DataFrame (not yet implemented).
     """
 
     def __init__(self, boxes, orig_shape) -> None:
         if boxes.ndim == 1:
             boxes = boxes[None, :]
         n = boxes.shape[-1]
-        assert n in {6, 7}, f'expected `n` in [6, 7], but got {n}'  # xyxy, (track_id), conf, cls
+        assert n in (6, 7), f'expected `n` in [6, 7], but got {n}'  # xyxy, (track_id), conf, cls
         # TODO
         self.is_track = n == 7
         self.boxes = boxes
         self.orig_shape = torch.as_tensor(orig_shape, device=boxes.device) if isinstance(boxes, torch.Tensor) \
             else np.asarray(orig_shape)
 
     @property
@@ -259,16 +258,19 @@
     def __len__(self):  # override len(results)
         return len(self.boxes)
 
     def __str__(self):
         return self.boxes.__str__()
 
     def __repr__(self):
-        return (f'Ultralytics YOLO {self.__class__.__name__}\n' + f'type: {type(self.boxes)}\n' +
-                f'shape: {self.boxes.shape}\n' + f'dtype: {self.boxes.dtype}\n + {self.boxes.__repr__()}')
+        return (f'{self.__class__.__module__}.{self.__class__.__name__}\n'
+                f'type:  {self.boxes.__class__.__module__}.{self.boxes.__class__.__name__}\n'
+                f'shape: {self.boxes.shape}\n'
+                f'dtype: {self.boxes.dtype}\n'
+                f'{self.boxes.__repr__()}')
 
     def __getitem__(self, idx):
         return Boxes(self.boxes[idx], self.orig_shape)
 
     def __getattr__(self, attr):
         name = self.__class__.__name__
         raise AttributeError(f"'{name}' object has no attribute '{attr}'. See valid attributes below.\n{self.__doc__}")
@@ -335,16 +337,19 @@
     def __len__(self):  # override len(results)
         return len(self.masks)
 
     def __str__(self):
         return self.masks.__str__()
 
     def __repr__(self):
-        return (f'Ultralytics YOLO {self.__class__.__name__}\n' + f'type: {type(self.masks)}\n' +
-                f'shape: {self.masks.shape}\n' + f'dtype: {self.masks.dtype}\n + {self.masks.__repr__()}')
+        return (f'{self.__class__.__module__}.{self.__class__.__name__}\n'
+                f'type:  {self.masks.__class__.__module__}.{self.masks.__class__.__name__}\n'
+                f'shape: {self.masks.shape}\n'
+                f'dtype: {self.masks.dtype}\n'
+                f'{self.masks.__repr__()}')
 
     def __getitem__(self, idx):
         return Masks(self.masks[idx], self.orig_shape)
 
     def __getattr__(self, attr):
         name = self.__class__.__name__
         raise AttributeError(f"'{name}' object has no attribute '{attr}'. See valid attributes below.\n{self.__doc__}")
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/engine/trainer.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/engine/trainer.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 from torch.nn.parallel import DistributedDataParallel as DDP
 from torch.optim import lr_scheduler
 from tqdm import tqdm
 
 from ultralytics.nn.tasks import attempt_load_one_weight, attempt_load_weights
 from ultralytics.yolo.cfg import get_cfg
 from ultralytics.yolo.data.utils import check_cls_dataset, check_det_dataset
-from ultralytics.yolo.utils import (DEFAULT_CFG, LOGGER, RANK, SETTINGS, TQDM_BAR_FORMAT, __version__, callbacks,
-                                    colorstr, emojis, yaml_save)
+from ultralytics.yolo.utils import (DEFAULT_CFG, LOGGER, ONLINE, RANK, ROOT, SETTINGS, TQDM_BAR_FORMAT, __version__,
+                                    callbacks, colorstr, emojis, yaml_save)
 from ultralytics.yolo.utils.autobatch import check_train_batch_size
 from ultralytics.yolo.utils.checks import check_file, check_imgsz, print_args
 from ultralytics.yolo.utils.dist import ddp_cleanup, generate_ddp_command
 from ultralytics.yolo.utils.files import get_latest_run, increment_path
 from ultralytics.yolo.utils.torch_utils import (EarlyStopping, ModelEMA, de_parallel, init_seeds, one_cycle,
                                                 select_device, strip_optimizer)
 
@@ -91,46 +91,44 @@
         # Dirs
         project = self.args.project or Path(SETTINGS['runs_dir']) / self.args.task
         name = self.args.name or f'{self.args.mode}'
         if hasattr(self.args, 'save_dir'):
             self.save_dir = Path(self.args.save_dir)
         else:
             self.save_dir = Path(
-                increment_path(Path(project) / name, exist_ok=self.args.exist_ok if RANK in {-1, 0} else True))
+                increment_path(Path(project) / name, exist_ok=self.args.exist_ok if RANK in (-1, 0) else True))
         self.wdir = self.save_dir / 'weights'  # weights dir
-        if RANK in {-1, 0}:
+        if RANK in (-1, 0):
             self.wdir.mkdir(parents=True, exist_ok=True)  # make dir
             self.args.save_dir = str(self.save_dir)
             yaml_save(self.save_dir / 'args.yaml', vars(self.args))  # save run args
         self.last, self.best = self.wdir / 'last.pt', self.wdir / 'best.pt'  # checkpoint paths
         self.save_period = self.args.save_period
 
         self.batch_size = self.args.batch
         self.epochs = self.args.epochs
         self.start_epoch = 0
         if RANK == -1:
             print_args(vars(self.args))
 
         # Device
-        self.amp = self.device.type != 'cpu'
-        self.scaler = amp.GradScaler(enabled=self.amp)
         if self.device.type == 'cpu':
             self.args.workers = 0  # faster CPU training as time dominated by inference, not dataloading
 
         # Model and Dataloaders.
         self.model = self.args.model
         try:
             if self.args.task == 'classify':
                 self.data = check_cls_dataset(self.args.data)
             elif self.args.data.endswith('.yaml') or self.args.task in ('detect', 'segment'):
                 self.data = check_det_dataset(self.args.data)
                 if 'yaml_file' in self.data:
                     self.args.data = self.data['yaml_file']  # for validating 'yolo train data=url.zip' usage
         except Exception as e:
-            raise FileNotFoundError(emojis(f"Dataset '{self.args.data}' error ❌ {e}")) from e
+            raise RuntimeError(emojis(f"Dataset '{self.args.data}' error ❌ {e}")) from e
 
         self.trainset, self.testset = self.get_dataset(self.data)
         self.ema = None
 
         # Optimization utils init
         self.lf = None
         self.scheduler = None
@@ -142,15 +140,15 @@
         self.tloss = None
         self.loss_names = ['Loss']
         self.csv = self.save_dir / 'results.csv'
         self.plot_idx = [0, 1, 2]
 
         # Callbacks
         self.callbacks = defaultdict(list, callbacks.default_callbacks)  # add callbacks
-        if RANK in {0, -1}:
+        if RANK in (-1, 0):
             callbacks.add_integration_callbacks(self)
 
     def add_callback(self, event: str, callback):
         """
         Appends the given callback.
         """
         self.callbacks[event].append(callback)
@@ -195,19 +193,29 @@
         LOGGER.info(f'DDP settings: RANK {rank}, WORLD_SIZE {world_size}, DEVICE {self.device}')
         dist.init_process_group('nccl' if dist.is_nccl_available() else 'gloo', rank=rank, world_size=world_size)
 
     def _setup_train(self, rank, world_size):
         """
         Builds dataloaders and optimizer on correct rank process.
         """
-        # model
+        # Model
         self.run_callbacks('on_pretrain_routine_start')
         ckpt = self.setup_model()
         self.model = self.model.to(self.device)
         self.set_model_attributes()
+        # Check AMP
+        self.amp = torch.tensor(True).to(self.device)
+        if RANK in (-1, 0):  # Single-GPU and DDP
+            callbacks_backup = callbacks.default_callbacks.copy()  # backup callbacks as check_amp() resets them
+            self.amp = torch.tensor(check_amp(self.model), device=self.device)
+            callbacks.default_callbacks = callbacks_backup  # restore callbacks
+        if RANK > -1:  # DDP
+            dist.broadcast(self.amp, src=0)  # broadcast the tensor from rank 0 to all other ranks (returns None)
+        self.amp = bool(self.amp)  # as boolean
+        self.scaler = amp.GradScaler(enabled=self.amp)
         if world_size > 1:
             self.model = DDP(self.model, device_ids=[rank])
         # Check imgsz
         gs = max(int(self.model.stride.max() if hasattr(self.model, 'stride') else 32), 32)  # grid size (max stride)
         self.args.imgsz = check_imgsz(self.args.imgsz, stride=gs, floor=gs, max_dim=1)
         # Batch size
         if self.batch_size == -1:
@@ -232,15 +240,15 @@
             self.lf = lambda x: (1 - x / self.epochs) * (1.0 - self.args.lrf) + self.args.lrf  # linear
         self.scheduler = lr_scheduler.LambdaLR(self.optimizer, lr_lambda=self.lf)
         self.stopper, self.stop = EarlyStopping(patience=self.args.patience), False
 
         # dataloaders
         batch_size = self.batch_size // world_size if world_size > 1 else self.batch_size
         self.train_loader = self.get_dataloader(self.trainset, batch_size=batch_size, rank=rank, mode='train')
-        if rank in {0, -1}:
+        if rank in (-1, 0):
             self.test_loader = self.get_dataloader(self.testset, batch_size=batch_size * 2, rank=-1, mode='val')
             self.validator = self.get_validator()
             metric_keys = self.validator.metrics.keys + self.label_loss_items(prefix='val')
             self.metrics = dict(zip(metric_keys, [0] * len(metric_keys)))  # TODO: init metrics for plot_results()?
             self.ema = ModelEMA(self.model)
             if self.args.plots and not self.args.v5loader:
                 self.plot_training_labels()
@@ -279,15 +287,15 @@
             if epoch == (self.epochs - self.args.close_mosaic):
                 LOGGER.info('Closing dataloader mosaic')
                 if hasattr(self.train_loader.dataset, 'mosaic'):
                     self.train_loader.dataset.mosaic = False
                 if hasattr(self.train_loader.dataset, 'close_mosaic'):
                     self.train_loader.dataset.close_mosaic(hyp=self.args)
 
-            if rank in {-1, 0}:
+            if rank in (-1, 0):
                 LOGGER.info(self.progress_string())
                 pbar = tqdm(enumerate(self.train_loader), total=nb, bar_format=TQDM_BAR_FORMAT)
             self.tloss = None
             self.optimizer.zero_grad()
             for i, batch in pbar:
                 self.run_callbacks('on_train_batch_start')
                 # Warmup
@@ -320,30 +328,30 @@
                     self.optimizer_step()
                     last_opt_step = ni
 
                 # Log
                 mem = f'{torch.cuda.memory_reserved() / 1E9 if torch.cuda.is_available() else 0:.3g}G'  # (GB)
                 loss_len = self.tloss.shape[0] if len(self.tloss.size()) else 1
                 losses = self.tloss if loss_len > 1 else torch.unsqueeze(self.tloss, 0)
-                if rank in {-1, 0}:
+                if rank in (-1, 0):
                     pbar.set_description(
                         ('%11s' * 2 + '%11.4g' * (2 + loss_len)) %
                         (f'{epoch + 1}/{self.epochs}', mem, *losses, batch['cls'].shape[0], batch['img'].shape[-1]))
                     self.run_callbacks('on_batch_end')
                     if self.args.plots and ni in self.plot_idx:
                         self.plot_training_samples(batch, ni)
 
                 self.run_callbacks('on_train_batch_end')
 
             self.lr = {f'lr/pg{ir}': x['lr'] for ir, x in enumerate(self.optimizer.param_groups)}  # for loggers
 
             self.scheduler.step()
             self.run_callbacks('on_train_epoch_end')
 
-            if rank in {-1, 0}:
+            if rank in (-1, 0):
 
                 # Validation
                 self.ema.update_attr(self.model, include=['yaml', 'nc', 'args', 'names', 'stride', 'class_weights'])
                 final_epoch = (epoch + 1 == self.epochs) or self.stopper.possible_stop
 
                 if self.args.val or final_epoch:
                     self.metrics, self.fitness = self.validate()
@@ -365,15 +373,15 @@
                 broadcast_list = [self.stop if RANK == 0 else None]
                 dist.broadcast_object_list(broadcast_list, 0)  # broadcast 'stop' to all ranks
                 if RANK != 0:
                     self.stop = broadcast_list[0]
             if self.stop:
                 break  # must break all DDP ranks
 
-        if rank in {-1, 0}:
+        if rank in (-1, 0):
             # Do final val with best.pt
             LOGGER.info(f'\n{epoch - self.start_epoch + 1} epochs completed in '
                         f'{(time.time() - self.train_time_start) / 3600:.3f} hours.')
             self.final_eval()
             if self.args.plots:
                 self.plot_metrics()
             self.run_callbacks('on_train_end')
@@ -593,7 +601,51 @@
             raise NotImplementedError(f'Optimizer {name} not implemented.')
 
         optimizer.add_param_group({'params': g[0], 'weight_decay': decay})  # add g0 with weight_decay
         optimizer.add_param_group({'params': g[1], 'weight_decay': 0.0})  # add g1 (BatchNorm2d weights)
         LOGGER.info(f"{colorstr('optimizer:')} {type(optimizer).__name__}(lr={lr}) with parameter groups "
                     f'{len(g[1])} weight(decay=0.0), {len(g[0])} weight(decay={decay}), {len(g[2])} bias')
         return optimizer
+
+
+def check_amp(model):
+    """
+    This function checks the PyTorch Automatic Mixed Precision (AMP) functionality of a YOLOv8 model.
+    If the checks fail, it means there are anomalies with AMP on the system that may cause NaN losses or zero-mAP
+    results, so AMP will be disabled during training.
+
+    Args:
+        model (nn.Module): A YOLOv8 model instance.
+
+    Returns:
+        bool: Returns True if the AMP functionality works correctly with YOLOv8 model, else False.
+
+    Raises:
+        AssertionError: If the AMP checks fail, indicating anomalies with the AMP functionality on the system.
+    """
+    device = next(model.parameters()).device  # get model device
+    if device.type in ('cpu', 'mps'):
+        return False  # AMP only used on CUDA devices
+
+    def amp_allclose(m, im):
+        # All close FP32 vs AMP results
+        a = m(im, device=device, verbose=False)[0].boxes.boxes  # FP32 inference
+        with torch.cuda.amp.autocast(True):
+            b = m(im, device=device, verbose=False)[0].boxes.boxes  # AMP inference
+        del m
+        return a.shape == b.shape and torch.allclose(a, b.float(), atol=0.5)  # close to 0.5 absolute tolerance
+
+    f = ROOT / 'assets/bus.jpg'  # image to check
+    im = f if f.exists() else 'https://ultralytics.com/images/bus.jpg' if ONLINE else np.ones((640, 640, 3))
+    prefix = colorstr('AMP: ')
+    LOGGER.info(f'{prefix}running Automatic Mixed Precision (AMP) checks with YOLOv8n...')
+    try:
+        from ultralytics import YOLO
+        assert amp_allclose(YOLO('yolov8n.pt'), im)
+        LOGGER.info(f'{prefix}checks passed ✅')
+    except ConnectionError:
+        LOGGER.warning(f"{prefix}checks skipped ⚠️, offline and unable to download YOLOv8n. Setting 'amp=True'.")
+    except AssertionError:
+        LOGGER.warning(f'{prefix}checks failed ❌. Anomalies were detected with AMP on your system that may lead to '
+                       f'NaN losses or zero-mAP results, so AMP will be disabled during training.')
+        return False
+    return True
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/engine/validator.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/engine/validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         self.training = True
         self.speed = {'preprocess': 0.0, 'inference': 0.0, 'loss': 0.0, 'postprocess': 0.0}
         self.jdict = None
 
         project = self.args.project or Path(SETTINGS['runs_dir']) / self.args.task
         name = self.args.name or f'{self.args.mode}'
         self.save_dir = save_dir or increment_path(Path(project) / name,
-                                                   exist_ok=self.args.exist_ok if RANK in {-1, 0} else True)
+                                                   exist_ok=self.args.exist_ok if RANK in (-1, 0) else True)
         (self.save_dir / 'labels' if self.args.save_txt else self.save_dir).mkdir(parents=True, exist_ok=True)
 
         if self.args.conf is None:
             self.args.conf = 0.001  # default conf=0.001
 
         self.callbacks = defaultdict(list, callbacks.default_callbacks)  # add callbacks
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/utils/__init__.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/utils/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 import uuid
 from pathlib import Path
 from types import SimpleNamespace
 from typing import Union
 
 import cv2
 import numpy as np
-import pandas as pd
 import torch
 import yaml
 
 from ultralytics import __version__
 
 # Constants
 FILE = Path(__file__).resolve()
@@ -91,16 +90,14 @@
     Community: https://community.ultralytics.com
     GitHub: https://github.com/ultralytics/ultralytics
     """
 
 # Settings
 torch.set_printoptions(linewidth=320, precision=5, profile='long')
 np.set_printoptions(linewidth=320, formatter={'float_kind': '{:11.5g}'.format})  # format short g, %precision=5
-pd.options.display.max_columns = 10
-pd.options.display.width = 120
 cv2.setNumThreads(0)  # prevent OpenCV from multithreading (incompatible with PyTorch DataLoader)
 os.environ['NUMEXPR_MAX_THREADS'] = str(NUM_THREADS)  # NumExpr max threads
 os.environ['CUBLAS_WORKSPACE_CONFIG'] = ':4096:8'  # for deterministic training
 
 
 class IterableSimpleNamespace(SimpleNamespace):
     """
@@ -122,14 +119,45 @@
             https://github.com/ultralytics/ultralytics/blob/main/ultralytics/yolo/cfg/default.yaml
             """)
 
     def get(self, key, default=None):
         return getattr(self, key, default)
 
 
+def set_logging(name=LOGGING_NAME, verbose=True):
+    # sets up logging for the given name
+    rank = int(os.getenv('RANK', -1))  # rank in world for Multi-GPU trainings
+    level = logging.INFO if verbose and rank in (-1, 0) else logging.ERROR
+    logging.config.dictConfig({
+        'version': 1,
+        'disable_existing_loggers': False,
+        'formatters': {
+            name: {
+                'format': '%(message)s'}},
+        'handlers': {
+            name: {
+                'class': 'logging.StreamHandler',
+                'formatter': name,
+                'level': level}},
+        'loggers': {
+            name: {
+                'level': level,
+                'handlers': [name],
+                'propagate': False}}})
+
+
+# Set logger
+set_logging(LOGGING_NAME, verbose=VERBOSE)  # run before defining LOGGER
+LOGGER = logging.getLogger(LOGGING_NAME)  # define globally (used in train.py, val.py, detect.py, etc.)
+if WINDOWS:  # emoji-safe logging
+    info_fn, warning_fn = LOGGER.info, LOGGER.warning
+    setattr(LOGGER, info_fn.__name__, lambda x: info_fn(emojis(x)))
+    setattr(LOGGER, warning_fn.__name__, lambda x: warning_fn(emojis(x)))
+
+
 def yaml_save(file='data.yaml', data=None):
     """
     Save YAML data to a file.
 
     Args:
         file (str, optional): File name. Default is 'data.yaml'.
         data (dict, optional): Data to save in YAML format. Default is None.
@@ -159,18 +187,21 @@
         file (str, optional): File name. Default is 'data.yaml'.
         append_filename (bool): Add the YAML filename to the YAML dictionary. Default is False.
 
     Returns:
         dict: YAML data and file name.
     """
     with open(file, errors='ignore', encoding='utf-8') as f:
-        # Add YAML filename to dict and return
         s = f.read()  # string
-        if not s.isprintable():  # remove special characters
+
+        # Remove special characters
+        if not s.isprintable():
             s = re.sub(r'[^\x09\x0A\x0D\x20-\x7E\x85\xA0-\uD7FF\uE000-\uFFFD\U00010000-\U0010ffff]+', '', s)
+
+        # Add YAML filename to dict and return
         return {**yaml.safe_load(s), 'yaml_file': str(file)} if append_filename else yaml.safe_load(s)
 
 
 def yaml_print(yaml_file: Union[str, Path, dict]) -> None:
     """
     Pretty prints a yaml file or a yaml-formatted dictionary.
 
@@ -246,19 +277,19 @@
 def is_online() -> bool:
     """
     Check internet connectivity by attempting to connect to a known online host.
 
     Returns:
         bool: True if connection is successful, False otherwise.
     """
-    import socket
-    with contextlib.suppress(Exception):
-        host = socket.gethostbyname('www.github.com')
-        socket.create_connection((host, 80), timeout=2)
-        return True
+#     import socket
+#     with contextlib.suppress(Exception):
+#         host = socket.gethostbyname('www.github.com')
+#         socket.create_connection((host, 80), timeout=2)
+#         return True
     return False
 
 
 ONLINE = is_online()
 
 
 def is_pip_package(filepath: str = __name__) -> bool:
@@ -444,49 +475,14 @@
         'bright_white': '\033[97m',
         'end': '\033[0m',  # misc
         'bold': '\033[1m',
         'underline': '\033[4m'}
     return ''.join(colors[x] for x in args) + f'{string}' + colors['end']
 
 
-def remove_ansi_codes(string):
-    """
-    Remove ANSI escape sequences from a string.
-
-    Args:
-        string (str): The input string that may contain ANSI escape sequences.
-
-    Returns:
-        str: The input string with ANSI escape sequences removed.
-    """
-    return re.sub(r'\x1B\[([0-9]{1,2}(;[0-9]{1,2})?)?[m|K]', '', string)
-
-
-def set_logging(name=LOGGING_NAME, verbose=True):
-    # sets up logging for the given name
-    rank = int(os.getenv('RANK', -1))  # rank in world for Multi-GPU trainings
-    level = logging.INFO if verbose and rank in {-1, 0} else logging.ERROR
-    logging.config.dictConfig({
-        'version': 1,
-        'disable_existing_loggers': False,
-        'formatters': {
-            name: {
-                'format': '%(message)s'}},
-        'handlers': {
-            name: {
-                'class': 'logging.StreamHandler',
-                'formatter': name,
-                'level': level}},
-        'loggers': {
-            name: {
-                'level': level,
-                'handlers': [name],
-                'propagate': False}}})
-
-
 class TryExcept(contextlib.ContextDecorator):
     # YOLOv8 TryExcept class. Usage: @TryExcept() decorator or 'with TryExcept():' context manager
     def __init__(self, msg='', verbose=True):
         self.msg = msg
         self.verbose = verbose
 
     def __enter__(self):
@@ -524,15 +520,15 @@
             'sys_argv': sys.argv[0],
             'sys_argv_name': Path(sys.argv[0]).name,
             'install': 'git' if is_git_dir() else 'pip' if is_pip_package() else 'other',
             'os': ENVIRONMENT}
         return event
 
     if SETTINGS['sync'] and \
-            RANK in {-1, 0} and \
+            RANK in (-1, 0) and \
             Path(sys.argv[0]).name == 'yolo' and \
             not TESTS_RUNNING and \
             ONLINE and \
             ((is_pip_package() and not is_git_dir()) or
              (get_git_origin_url() == 'https://github.com/ultralytics/ultralytics.git' and get_git_branch() == 'main')):
 
         import sentry_sdk  # noqa
@@ -605,21 +601,14 @@
     """
     SETTINGS.update(kwargs)
     yaml_save(file, SETTINGS)
 
 
 # Run below code on yolo/utils init ------------------------------------------------------------------------------------
 
-# Set logger
-set_logging(LOGGING_NAME, verbose=VERBOSE)  # run before defining LOGGER
-LOGGER = logging.getLogger(LOGGING_NAME)  # define globally (used in train.py, val.py, detect.py, etc.)
-if WINDOWS:
-    for fn in LOGGER.info, LOGGER.warning:
-        setattr(LOGGER, fn.__name__, lambda x: fn(emojis(x)))  # emoji safe logging
-
 # Check first-install steps
 PREFIX = colorstr('Ultralytics: ')
 SETTINGS = get_settings()
 DATASETS_DIR = Path(SETTINGS['datasets_dir'])  # global datasets directory
 ENVIRONMENT = 'Colab' if is_colab() else 'Kaggle' if is_kaggle() else 'Jupyter' if is_jupyter() else \
     'Docker' if is_docker() else platform.system()
 TESTS_RUNNING = is_pytest_running() or is_github_actions_ci()
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/utils/autobatch.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/utils/benchmarks.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/utils/benchmarks.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,38 +22,41 @@
 PaddlePaddle            | `paddle`                  | yolov8n_paddle_model/
 """
 
 import platform
 import time
 from pathlib import Path
 
-import pandas as pd
-
 from ultralytics import YOLO
 from ultralytics.yolo.engine.exporter import export_formats
-from ultralytics.yolo.utils import LINUX, LOGGER, ROOT, SETTINGS
+from ultralytics.yolo.utils import LINUX, LOGGER, MACOS, ROOT, SETTINGS
 from ultralytics.yolo.utils.checks import check_yolo
 from ultralytics.yolo.utils.downloads import download
 from ultralytics.yolo.utils.files import file_size
 from ultralytics.yolo.utils.torch_utils import select_device
 
 
 def benchmark(model=Path(SETTINGS['weights_dir']) / 'yolov8n.pt', imgsz=160, half=False, device='cpu', hard_fail=False):
+    import pandas as pd
+    pd.options.display.max_columns = 10
+    pd.options.display.width = 120
     device = select_device(device, verbose=False)
     if isinstance(model, (str, Path)):
         model = YOLO(model)
 
     y = []
     t0 = time.time()
     for i, (name, format, suffix, cpu, gpu) in export_formats().iterrows():  # index, (name, format, suffix, CPU, GPU)
         emoji, filename = '❌', None  # export defaults
         try:
             if model.task == 'classify':
                 assert i != 11, 'paddle cls exports coming soon'
             assert i != 9 or LINUX, 'Edge TPU export only supported on Linux'
+            if i == 10:
+                assert MACOS or LINUX, 'TF.js export only supported on macOS and Linux'
             if 'cpu' in device.type:
                 assert cpu, 'inference not supported on CPU'
             if 'cuda' in device.type:
                 assert gpu, 'inference not supported on GPU'
 
             # Export
             if format == '-':
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/utils/callbacks/base.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/utils/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/utils/callbacks/clearml.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/utils/callbacks/clearml.py`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/utils/callbacks/comet.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/utils/callbacks/comet.py`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/utils/callbacks/hub.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/utils/callbacks/hub.py`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/utils/callbacks/tensorboard.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/utils/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/utils/checks.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/utils/checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,20 +130,28 @@
     """
     response = requests.get(f'https://pypi.org/pypi/{package_name}/json')
     if response.status_code == 200:
         return response.json()['info']['version']
     return None
 
 
-def check_pip_update():
+def check_pip_update_available():
+    """
+    Checks if a new version of the ultralytics package is available on PyPI.
+
+    Returns:
+        bool: True if an update is available, False otherwise.
+    """
     from ultralytics import __version__
     latest = check_latest_pypi_version()
-    if pkg.parse_version(__version__) < pkg.parse_version(latest):
+    if pkg.parse_version(__version__) < pkg.parse_version(latest):  # update is available
         LOGGER.info(f'New https://pypi.org/project/ultralytics/{latest} available 😃 '
                     f"Update with 'pip install -U ultralytics'")
+        return True
+    return False
 
 
 def check_font(font='Arial.ttf'):
     """
     Find font locally or download to user's configuration directory if it does not already exist.
 
     Args:
@@ -232,17 +240,18 @@
             s = Path(f).suffix.lower()  # file suffix
             if len(s):
                 assert s in suffix, f'{msg}{f} acceptable suffix is {suffix}'
 
 
 def check_yolov5u_filename(file: str, verbose: bool = True):
     # Replace legacy YOLOv5 filenames with updated YOLOv5u filenames
-    if 'yolov3' in file or 'yolov5' in file and 'u' not in file:
+    if ('yolov3' in file or 'yolov5' in file) and 'u' not in file:
         original_file = file
         file = re.sub(r'(.*yolov5([nsmlx]))\.', '\\1u.', file)  # i.e. yolov5n.pt -> yolov5nu.pt
+        file = re.sub(r'(.*yolov5([nsmlx])6)\.', '\\1u.', file)  # i.e. yolov5n6.pt -> yolov5n6u.pt
         file = re.sub(r'(.*yolov3(|-tiny|-spp))\.', '\\1u.', file)  # i.e. yolov3-spp.pt -> yolov3-sppu.pt
         if file != original_file and verbose:
             LOGGER.info(f"PRO TIP 💡 Replace 'model={original_file}' with new 'model={file}'.\nYOLOv5 'u' models are "
                         f'trained with https://github.com/ultralytics/ultralytics and feature improved performance vs '
                         f'standard YOLOv5 models trained with https://github.com/ultralytics/yolov5.\n')
     return file
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/utils/dist.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/utils/dist.py`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/utils/downloads.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/utils/downloads.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
             except Exception as e:
                 if i == 0 and not is_online():
                     raise ConnectionError(f'❌  Download failure for {url}. Environment is not online.') from e
                 elif i >= retry:
                     raise ConnectionError(f'❌  Download failure for {url}. Retry limit reached.') from e
                 LOGGER.warning(f'⚠️ Download failure, retrying {i + 1}/{retry} {url}...')
 
-    if unzip and f.exists() and f.suffix in {'.zip', '.tar', '.gz'}:
+    if unzip and f.exists() and f.suffix in ('.zip', '.tar', '.gz'):
         unzip_dir = dir or f.parent  # unzip to dir if provided else unzip in place
         LOGGER.info(f'Unzipping {f} to {unzip_dir}...')
         if f.suffix == '.zip':
             unzip_dir = unzip_file(file=f, path=unzip_dir)  # unzip
         elif f.suffix == '.tar':
             subprocess.run(['tar', 'xf', f, '--directory', unzip_dir], check=True)  # unzip
         elif f.suffix == '.gz':
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/utils/files.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/utils/files.py`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/utils/instance.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/utils/instance.py`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/utils/loss.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/utils/loss.py`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/utils/metrics.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/utils/ops.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/utils/ops.py`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/utils/plotting.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/utils/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 import math
 from pathlib import Path
 
 import cv2
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
-import pandas as pd
-import seaborn as sn
 import torch
 from PIL import Image, ImageDraw, ImageFont
 from PIL import __version__ as pil_version
 
 from ultralytics.yolo.utils import LOGGER, TryExcept, threaded
 
 from .checks import check_font, check_version, is_ascii
@@ -157,14 +155,17 @@
     def result(self):
         # Return annotated image as array
         return np.asarray(self.im)
 
 
 @TryExcept()  # known issue https://github.com/ultralytics/yolov5/issues/5395
 def plot_labels(boxes, cls, names=(), save_dir=Path('')):
+    import pandas as pd
+    import seaborn as sn
+
     # plot dataset labels
     LOGGER.info(f"Plotting labels to {save_dir / 'labels.jpg'}... ")
     b = boxes.transpose()  # classes, boxes
     nc = int(cls.max() + 1)  # number of classes
     x = pd.DataFrame(b.transpose(), columns=['x', 'y', 'width', 'height'])
 
     # seaborn correlogram
@@ -270,15 +271,15 @@
     # Annotate
     fs = int((h + w) * ns * 0.01)  # font size
     annotator = Annotator(mosaic, line_width=round(fs / 10), font_size=fs, pil=True, example=names)
     for i in range(i + 1):
         x, y = int(w * (i // ns)), int(h * (i % ns))  # block origin
         annotator.rectangle([x, y, x + w, y + h], None, (255, 255, 255), width=2)  # borders
         if paths:
-            annotator.text((x + 5, y + 5 + h), text=Path(paths[i]).name[:40], txt_color=(220, 220, 220))  # filenames
+            annotator.text((x + 5, y + 5), text=Path(paths[i]).name[:40], txt_color=(220, 220, 220))  # filenames
         if len(cls) > 0:
             idx = batch_idx == i
 
             boxes = xywh2xyxy(bboxes[idx, :4]).T
             classes = cls[idx].astype('int')
             labels = bboxes.shape[1] == 4  # labels if no conf column
             conf = None if labels else bboxes[idx, 4]  # check for confidence presence (label vs pred)
@@ -325,14 +326,15 @@
                             im[y:y + h, x:x + w, :][mask] = im[y:y + h, x:x + w, :][mask] * 0.4 + np.array(color) * 0.6
                 annotator.fromarray(im)
     annotator.im.save(fname)  # save
 
 
 def plot_results(file='path/to/results.csv', dir='', segment=False):
     # Plot training results.csv. Usage: from utils.plots import *; plot_results('path/to/results.csv')
+    import pandas as pd
     save_dir = Path(file).parent if file else Path(dir)
     if segment:
         fig, ax = plt.subplots(2, 8, figsize=(18, 6), tight_layout=True)
         index = [1, 2, 3, 4, 5, 6, 9, 10, 13, 14, 15, 16, 7, 8, 11, 12]
     else:
         fig, ax = plt.subplots(2, 5, figsize=(12, 6), tight_layout=True)
         index = [1, 2, 3, 4, 5, 8, 9, 10, 6, 7]
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/utils/tal.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/utils/tal.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,37 +6,29 @@
 
 from .checks import check_version
 from .metrics import bbox_iou
 
 TORCH_1_10 = check_version(torch.__version__, '1.10.0')
 
 
-def select_candidates_in_gts(xy_centers, gt_bboxes, eps=1e-9, roll_out=False):
+def select_candidates_in_gts(xy_centers, gt_bboxes, eps=1e-9):
     """select the positive anchor center in gt
 
     Args:
         xy_centers (Tensor): shape(h*w, 4)
         gt_bboxes (Tensor): shape(b, n_boxes, 4)
     Return:
         (Tensor): shape(b, n_boxes, h*w)
     """
     n_anchors = xy_centers.shape[0]
     bs, n_boxes, _ = gt_bboxes.shape
-    if roll_out:
-        bbox_deltas = torch.empty((bs, n_boxes, n_anchors), device=gt_bboxes.device)
-        for b in range(bs):
-            lt, rb = gt_bboxes[b].view(-1, 1, 4).chunk(2, 2)  # left-top, right-bottom
-            bbox_deltas[b] = torch.cat((xy_centers[None] - lt, rb - xy_centers[None]),
-                                       dim=2).view(n_boxes, n_anchors, -1).amin(2).gt_(eps)
-        return bbox_deltas
-    else:
-        lt, rb = gt_bboxes.view(-1, 1, 4).chunk(2, 2)  # left-top, right-bottom
-        bbox_deltas = torch.cat((xy_centers[None] - lt, rb - xy_centers[None]), dim=2).view(bs, n_boxes, n_anchors, -1)
-        # return (bbox_deltas.min(3)[0] > eps).to(gt_bboxes.dtype)
-        return bbox_deltas.amin(3).gt_(eps)
+    lt, rb = gt_bboxes.view(-1, 1, 4).chunk(2, 2)  # left-top, right-bottom
+    bbox_deltas = torch.cat((xy_centers[None] - lt, rb - xy_centers[None]), dim=2).view(bs, n_boxes, n_anchors, -1)
+    # return (bbox_deltas.min(3)[0] > eps).to(gt_bboxes.dtype)
+    return bbox_deltas.amin(3).gt_(eps)
 
 
 def select_highest_overlaps(mask_pos, overlaps, n_max_boxes):
     """if an anchor box is assigned to multiple gts,
         the one with the highest iou will be selected.
 
     Args:
@@ -59,23 +51,22 @@
     # find each grid serve which gt(index)
     target_gt_idx = mask_pos.argmax(-2)  # (b, h*w)
     return target_gt_idx, fg_mask, mask_pos
 
 
 class TaskAlignedAssigner(nn.Module):
 
-    def __init__(self, topk=13, num_classes=80, alpha=1.0, beta=6.0, eps=1e-9, roll_out_thr=0):
+    def __init__(self, topk=13, num_classes=80, alpha=1.0, beta=6.0, eps=1e-9):
         super().__init__()
         self.topk = topk
         self.num_classes = num_classes
         self.bg_idx = num_classes
         self.alpha = alpha
         self.beta = beta
         self.eps = eps
-        self.roll_out_thr = roll_out_thr
 
     @torch.no_grad()
     def forward(self, pd_scores, pd_bboxes, anc_points, gt_labels, gt_bboxes, mask_gt):
         """This code referenced to
            https://github.com/Nioolek/PPYOLOE_pytorch/blob/master/ppyoloe/assigner/tal_assigner.py
 
         Args:
@@ -89,15 +80,14 @@
             target_labels (Tensor): shape(bs, num_total_anchors)
             target_bboxes (Tensor): shape(bs, num_total_anchors, 4)
             target_scores (Tensor): shape(bs, num_total_anchors, num_classes)
             fg_mask (Tensor): shape(bs, num_total_anchors)
         """
         self.bs = pd_scores.size(0)
         self.n_max_boxes = gt_bboxes.size(1)
-        self.roll_out = self.n_max_boxes > self.roll_out_thr if self.roll_out_thr else False
 
         if self.n_max_boxes == 0:
             device = gt_bboxes.device
             return (torch.full_like(pd_scores[..., 0], self.bg_idx).to(device), torch.zeros_like(pd_bboxes).to(device),
                     torch.zeros_like(pd_scores).to(device), torch.zeros_like(pd_scores[..., 0]).to(device),
                     torch.zeros_like(pd_scores[..., 0]).to(device))
 
@@ -115,48 +105,43 @@
         pos_overlaps = (overlaps * mask_pos).amax(axis=-1, keepdim=True)  # b, max_num_obj
         norm_align_metric = (align_metric * pos_overlaps / (pos_align_metrics + self.eps)).amax(-2).unsqueeze(-1)
         target_scores = target_scores * norm_align_metric
 
         return target_labels, target_bboxes, target_scores, fg_mask.bool(), target_gt_idx
 
     def get_pos_mask(self, pd_scores, pd_bboxes, gt_labels, gt_bboxes, anc_points, mask_gt):
-        # get anchor_align metric, (b, max_num_obj, h*w)
-        align_metric, overlaps = self.get_box_metrics(pd_scores, pd_bboxes, gt_labels, gt_bboxes)
         # get in_gts mask, (b, max_num_obj, h*w)
-        mask_in_gts = select_candidates_in_gts(anc_points, gt_bboxes, roll_out=self.roll_out)
+        mask_in_gts = select_candidates_in_gts(anc_points, gt_bboxes)
+        # get anchor_align metric, (b, max_num_obj, h*w)
+        align_metric, overlaps = self.get_box_metrics(pd_scores, pd_bboxes, gt_labels, gt_bboxes, mask_in_gts * mask_gt)
         # get topk_metric mask, (b, max_num_obj, h*w)
-        mask_topk = self.select_topk_candidates(align_metric * mask_in_gts,
-                                                topk_mask=mask_gt.repeat([1, 1, self.topk]).bool())
+        mask_topk = self.select_topk_candidates(align_metric, topk_mask=mask_gt.repeat([1, 1, self.topk]).bool())
         # merge all mask to a final mask, (b, max_num_obj, h*w)
         mask_pos = mask_topk * mask_in_gts * mask_gt
 
         return mask_pos, align_metric, overlaps
 
-    def get_box_metrics(self, pd_scores, pd_bboxes, gt_labels, gt_bboxes):
-        if self.roll_out:
-            align_metric = torch.empty((self.bs, self.n_max_boxes, pd_scores.shape[1]), device=pd_scores.device)
-            overlaps = torch.empty((self.bs, self.n_max_boxes, pd_scores.shape[1]), device=pd_scores.device)
-            ind_0 = torch.empty(self.n_max_boxes, dtype=torch.long)
-            for b in range(self.bs):
-                ind_0[:], ind_2 = b, gt_labels[b].squeeze(-1).long()
-                # get the scores of each grid for each gt cls
-                bbox_scores = pd_scores[ind_0, :, ind_2]  # b, max_num_obj, h*w
-                overlaps[b] = bbox_iou(gt_bboxes[b].unsqueeze(1), pd_bboxes[b].unsqueeze(0), xywh=False,
-                                       CIoU=True).squeeze(2).clamp(0)
-                align_metric[b] = bbox_scores.pow(self.alpha) * overlaps[b].pow(self.beta)
-        else:
-            ind = torch.zeros([2, self.bs, self.n_max_boxes], dtype=torch.long)  # 2, b, max_num_obj
-            ind[0] = torch.arange(end=self.bs).view(-1, 1).repeat(1, self.n_max_boxes)  # b, max_num_obj
-            ind[1] = gt_labels.long().squeeze(-1)  # b, max_num_obj
-            # get the scores of each grid for each gt cls
-            bbox_scores = pd_scores[ind[0], :, ind[1]]  # b, max_num_obj, h*w
-
-            overlaps = bbox_iou(gt_bboxes.unsqueeze(2), pd_bboxes.unsqueeze(1), xywh=False,
-                                CIoU=True).squeeze(3).clamp(0)
-            align_metric = bbox_scores.pow(self.alpha) * overlaps.pow(self.beta)
+    def get_box_metrics(self, pd_scores, pd_bboxes, gt_labels, gt_bboxes, mask_gt):
+        na = pd_bboxes.shape[-2]
+        mask_gt = mask_gt.bool()  # b, max_num_obj, h*w
+        overlaps = torch.zeros([self.bs, self.n_max_boxes, na], dtype=pd_bboxes.dtype, device=pd_bboxes.device)
+        bbox_scores = torch.zeros([self.bs, self.n_max_boxes, na], dtype=pd_scores.dtype, device=pd_scores.device)
+
+        ind = torch.zeros([2, self.bs, self.n_max_boxes], dtype=torch.long)  # 2, b, max_num_obj
+        ind[0] = torch.arange(end=self.bs).view(-1, 1).repeat(1, self.n_max_boxes)  # b, max_num_obj
+        ind[1] = gt_labels.long().squeeze(-1)  # b, max_num_obj
+        # get the scores of each grid for each gt cls
+        bbox_scores[mask_gt] = pd_scores[ind[0], :, ind[1]][mask_gt]  # b, max_num_obj, h*w
+
+        # (b, max_num_obj, 1, 4), (b, 1, h*w, 4)
+        pd_boxes = pd_bboxes.unsqueeze(1).repeat(1, self.n_max_boxes, 1, 1)[mask_gt]
+        gt_boxes = gt_bboxes.unsqueeze(2).repeat(1, 1, na, 1)[mask_gt]
+        overlaps[mask_gt] = bbox_iou(gt_boxes, pd_boxes, xywh=False, CIoU=True).squeeze(-1).clamp(0)
+
+        align_metric = bbox_scores.pow(self.alpha) * overlaps.pow(self.beta)
         return align_metric, overlaps
 
     def select_topk_candidates(self, metrics, largest=True, topk_mask=None):
         """
         Args:
             metrics: (b, max_num_obj, h*w).
             topk_mask: (b, max_num_obj, topk) or None
@@ -166,20 +151,18 @@
         # (b, max_num_obj, topk)
         topk_metrics, topk_idxs = torch.topk(metrics, self.topk, dim=-1, largest=largest)
         if topk_mask is None:
             topk_mask = (topk_metrics.max(-1, keepdim=True) > self.eps).tile([1, 1, self.topk])
         # (b, max_num_obj, topk)
         topk_idxs[~topk_mask] = 0
         # (b, max_num_obj, topk, h*w) -> (b, max_num_obj, h*w)
-        if self.roll_out:
-            is_in_topk = torch.empty(metrics.shape, dtype=torch.long, device=metrics.device)
-            for b in range(len(topk_idxs)):
-                is_in_topk[b] = F.one_hot(topk_idxs[b], num_anchors).sum(-2)
-        else:
-            is_in_topk = F.one_hot(topk_idxs, num_anchors).sum(-2)
+        is_in_topk = torch.zeros(metrics.shape, dtype=torch.long, device=metrics.device)
+        for it in range(self.topk):
+            is_in_topk += F.one_hot(topk_idxs[:, :, it], num_anchors)
+        # is_in_topk = F.one_hot(topk_idxs, num_anchors).sum(-2)
         # filter invalid bboxes
         is_in_topk = torch.where(is_in_topk > 1, 0, is_in_topk)
         return is_in_topk.to(metrics.dtype)
 
     def get_targets(self, gt_labels, gt_bboxes, target_gt_idx, fg_mask):
         """
         Args:
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/utils/torch_utils.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/utils/torch_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 TORCH_1_12 = check_version(torch.__version__, '1.12.0')
 
 
 @contextmanager
 def torch_distributed_zero_first(local_rank: int):
     # Decorator to make all processes in distributed training wait for each local_master to do something
     initialized = torch.distributed.is_available() and torch.distributed.is_initialized()
-    if initialized and local_rank not in {-1, 0}:
+    if initialized and local_rank not in (-1, 0):
         dist.barrier(device_ids=[local_rank])
     yield
     if initialized and local_rank == 0:
         dist.barrier(device_ids=[0])
 
 
 def smart_inference_mode():
@@ -158,19 +158,21 @@
     b_conv = torch.zeros(deconv.weight.size(1), device=deconv.weight.device) if deconv.bias is None else deconv.bias
     b_bn = bn.bias - bn.weight.mul(bn.running_mean).div(torch.sqrt(bn.running_var + bn.eps))
     fuseddconv.bias.copy_(torch.mm(w_bn, b_conv.reshape(-1, 1)).reshape(-1) + b_bn)
 
     return fuseddconv
 
 
-def model_info(model, verbose=False, imgsz=640):
+def model_info(model, detailed=False, verbose=True, imgsz=640):
     # Model information. imgsz may be int or list, i.e. imgsz=640 or imgsz=[640, 320]
+    if not verbose:
+        return
     n_p = get_num_params(model)
     n_g = get_num_gradients(model)  # number gradients
-    if verbose:
+    if detailed:
         LOGGER.info(
             f"{'layer':>5} {'name':>40} {'gradient':>9} {'parameters':>12} {'shape':>20} {'mu':>10} {'sigma':>10}")
         for i, (name, p) in enumerate(model.named_parameters()):
             name = name.replace('module_list.', '')
             LOGGER.info('%5g %40s %9s %12g %20s %10.3g %10.3g' %
                         (i, name, p.requires_grad, p.numel(), list(p.shape), p.mean(), p.std()))
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/v8/classify/predict.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/v8/classify/predict.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,22 +10,21 @@
 
 class ClassificationPredictor(BasePredictor):
 
     def get_annotator(self, img):
         return Annotator(img, example=str(self.model.names), pil=True)
 
     def preprocess(self, img):
-        img = (img if isinstance(img, torch.Tensor) else torch.Tensor(img)).to(self.model.device)
-        img = img.half() if self.model.fp16 else img.float()  # uint8 to fp16/32
-        return img
+        img = (img if isinstance(img, torch.Tensor) else torch.from_numpy(img)).to(self.model.device)
+        return img.half() if self.model.fp16 else img.float()  # uint8 to fp16/32
 
-    def postprocess(self, preds, img, orig_img):
+    def postprocess(self, preds, img, orig_imgs):
         results = []
         for i, pred in enumerate(preds):
-            orig_img = orig_img[i] if isinstance(orig_img, list) else orig_img
+            orig_img = orig_imgs[i] if isinstance(orig_imgs, list) else orig_imgs
             path, _, _, _, _ = self.batch
             img_path = path[i] if isinstance(path, list) else path
             results.append(Results(orig_img=orig_img, path=img_path, names=self.model.names, probs=pred))
 
         return results
 
     def write_results(self, idx, results, batch):
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/v8/classify/train.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/v8/classify/train.py`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/v8/classify/val.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/v8/classify/val.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,23 +29,26 @@
     def update_metrics(self, preds, batch):
         n5 = min(len(self.model.names), 5)
         self.pred.append(preds.argsort(1, descending=True)[:, :n5])
         self.targets.append(batch['cls'])
 
     def finalize_metrics(self, *args, **kwargs):
         self.metrics.speed = self.speed
+        # self.metrics.confusion_matrix = self.confusion_matrix  # TODO: classification ConfusionMatrix
 
     def get_stats(self):
         self.metrics.process(self.targets, self.pred)
         return self.metrics.results_dict
 
     def get_dataloader(self, dataset_path, batch_size):
         return build_classification_dataloader(path=dataset_path,
                                                imgsz=self.args.imgsz,
                                                batch_size=batch_size,
+                                               augment=False,
+                                               shuffle=False,
                                                workers=self.args.workers)
 
     def print_results(self):
         pf = '%22s' + '%11.3g' * len(self.metrics.keys)  # print format
         LOGGER.info(pf % ('all', self.metrics.top1, self.metrics.top5))
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/v8/detect/predict.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/v8/detect/predict.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,32 +10,32 @@
 
 class DetectionPredictor(BasePredictor):
 
     def get_annotator(self, img):
         return Annotator(img, line_width=self.args.line_thickness, example=str(self.model.names))
 
     def preprocess(self, img):
-        img = torch.from_numpy(img).to(self.model.device)
+        img = (img if isinstance(img, torch.Tensor) else torch.from_numpy(img)).to(self.model.device)
         img = img.half() if self.model.fp16 else img.float()  # uint8 to fp16/32
         img /= 255  # 0 - 255 to 0.0 - 1.0
         return img
 
-    def postprocess(self, preds, img, orig_img):
+    def postprocess(self, preds, img, orig_imgs):
         preds = ops.non_max_suppression(preds,
                                         self.args.conf,
                                         self.args.iou,
                                         agnostic=self.args.agnostic_nms,
                                         max_det=self.args.max_det,
                                         classes=self.args.classes)
 
         results = []
         for i, pred in enumerate(preds):
-            orig_img = orig_img[i] if isinstance(orig_img, list) else orig_img
-            shape = orig_img.shape
-            pred[:, :4] = ops.scale_boxes(img.shape[2:], pred[:, :4], shape).round()
+            orig_img = orig_imgs[i] if isinstance(orig_imgs, list) else orig_imgs
+            if not isinstance(orig_imgs, torch.Tensor):
+                pred[:, :4] = ops.scale_boxes(img.shape[2:], pred[:, :4], orig_img.shape)
             path, _, _, _, _ = self.batch
             img_path = path[i] if isinstance(path, list) else path
             results.append(Results(orig_img=orig_img, path=img_path, names=self.model.names, boxes=pred))
         return results
 
     def write_results(self, idx, results, batch):
         p, im, im0 = batch
@@ -59,23 +59,22 @@
             return f'{log_string}(no detections), '
         for c in det.cls.unique():
             n = (det.cls == c).sum()  # detections per class
             log_string += f"{n} {self.model.names[int(c)]}{'s' * (n > 1)}, "
 
         # write
         for d in reversed(det):
-            cls, conf = d.cls.squeeze(), d.conf.squeeze()
+            cls, conf, id = d.cls.squeeze(), d.conf.squeeze(), None if d.id is None else int(d.id.item())
             if self.args.save_txt:  # Write to file
-                line = (cls, *(d.xywhn.view(-1).tolist()), conf) \
-                    if self.args.save_conf else (cls, *(d.xywhn.view(-1).tolist()))  # label format
+                line = (cls, *d.xywhn.view(-1)) + (conf, ) * self.args.save_conf + (() if id is None else (id, ))
                 with open(f'{self.txt_path}.txt', 'a') as f:
                     f.write(('%g ' * len(line)).rstrip() % line + '\n')
             if self.args.save or self.args.save_crop or self.args.show:  # Add bbox to image
                 c = int(cls)  # integer class
-                name = f'id:{int(d.id.item())} {self.model.names[c]}' if d.id is not None else self.model.names[c]
+                name = ('' if id is None else f'id:{id} ') + self.model.names[c]
                 label = None if self.args.hide_labels else (name if self.args.hide_conf else f'{name} {conf:.2f}')
                 self.annotator.box_label(d.xyxy.squeeze(), label, color=colors(c, True))
             if self.args.save_crop:
                 save_one_box(d.xyxy,
                              imc,
                              file=self.save_dir / 'crops' / self.model.model.names[c] / f'{self.data_path.stem}.jpg',
                              BGR=True)
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/v8/detect/train.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/v8/detect/train.py`

 * *Files 5% similar despite different names*

```diff
@@ -120,21 +120,16 @@
         self.stride = m.stride  # model strides
         self.nc = m.nc  # number of classes
         self.no = m.no
         self.reg_max = m.reg_max
         self.device = device
 
         self.use_dfl = m.reg_max > 1
-        roll_out_thr = h.min_memory if h.min_memory > 1 else 64 if h.min_memory else 0  # 64 is default
 
-        self.assigner = TaskAlignedAssigner(topk=10,
-                                            num_classes=self.nc,
-                                            alpha=0.5,
-                                            beta=6.0,
-                                            roll_out_thr=roll_out_thr)
+        self.assigner = TaskAlignedAssigner(topk=10, num_classes=self.nc, alpha=0.5, beta=6.0)
         self.bbox_loss = BboxLoss(m.reg_max - 1, use_dfl=self.use_dfl).to(device)
         self.proj = torch.arange(m.reg_max, dtype=torch.float, device=device)
 
     def preprocess(self, targets, batch_size, scale_tensor):
         if targets.shape[0] == 0:
             out = torch.zeros(batch_size, 0, 5, device=self.device)
         else:
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/v8/detect/val.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/v8/detect/val.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,15 @@
             if self.args.save_json:
                 self.pred_to_json(predn, batch['im_file'][si])
             # if self.args.save_txt:
             #    save_one_txt(predn, save_conf, shape, file=save_dir / 'labels' / f'{path.stem}.txt')
 
     def finalize_metrics(self, *args, **kwargs):
         self.metrics.speed = self.speed
+        self.metrics.confusion_matrix = self.confusion_matrix
 
     def get_stats(self):
         stats = [torch.cat(x, 0).cpu().numpy() for x in zip(*self.stats)]  # to numpy
         if len(stats) and stats[0].any():
             self.metrics.process(*stats)
         self.nt_per_class = np.bincount(stats[-1].astype(int), minlength=self.nc)  # number of targets per class
         return self.metrics.results_dict
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/v8/segment/predict.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/v8/segment/predict.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,39 +6,40 @@
 from ultralytics.yolo.utils import DEFAULT_CFG, ROOT, ops
 from ultralytics.yolo.utils.plotting import colors, save_one_box
 from ultralytics.yolo.v8.detect.predict import DetectionPredictor
 
 
 class SegmentationPredictor(DetectionPredictor):
 
-    def postprocess(self, preds, img, orig_img):
+    def postprocess(self, preds, img, orig_imgs):
         # TODO: filter by classes
         p = ops.non_max_suppression(preds[0],
                                     self.args.conf,
                                     self.args.iou,
                                     agnostic=self.args.agnostic_nms,
                                     max_det=self.args.max_det,
                                     nc=len(self.model.names),
                                     classes=self.args.classes)
         results = []
         proto = preds[1][-1] if len(preds[1]) == 3 else preds[1]  # second output is len 3 if pt, but only 1 if exported
         for i, pred in enumerate(p):
-            orig_img = orig_img[i] if isinstance(orig_img, list) else orig_img
-            shape = orig_img.shape
+            orig_img = orig_imgs[i] if isinstance(orig_imgs, list) else orig_imgs
             path, _, _, _, _ = self.batch
             img_path = path[i] if isinstance(path, list) else path
             if not len(pred):  # save empty boxes
                 results.append(Results(orig_img=orig_img, path=img_path, names=self.model.names, boxes=pred[:, :6]))
                 continue
             if self.args.retina_masks:
-                pred[:, :4] = ops.scale_boxes(img.shape[2:], pred[:, :4], shape).round()
-                masks = ops.process_mask_native(proto[i], pred[:, 6:], pred[:, :4], shape[:2])  # HWC
+                if not isinstance(orig_imgs, torch.Tensor):
+                    pred[:, :4] = ops.scale_boxes(img.shape[2:], pred[:, :4], orig_img.shape)
+                masks = ops.process_mask_native(proto[i], pred[:, 6:], pred[:, :4], orig_img.shape[:2])  # HWC
             else:
                 masks = ops.process_mask(proto[i], pred[:, 6:], pred[:, :4], img.shape[2:], upsample=True)  # HWC
-                pred[:, :4] = ops.scale_boxes(img.shape[2:], pred[:, :4], shape).round()
+                if not isinstance(orig_imgs, torch.Tensor):
+                    pred[:, :4] = ops.scale_boxes(img.shape[2:], pred[:, :4], orig_img.shape)
             results.append(
                 Results(orig_img=orig_img, path=img_path, names=self.model.names, boxes=pred[:, :6], masks=masks))
         return results
 
     def write_results(self, idx, results, batch):
         p, im, im0 = batch
         log_string = ''
@@ -71,25 +72,23 @@
         if self.args.save or self.args.show:
             im_gpu = torch.as_tensor(im0, dtype=torch.float16, device=mask.masks.device).permute(
                 2, 0, 1).flip(0).contiguous() / 255 if self.args.retina_masks else im[idx]
             self.annotator.masks(masks=mask.masks, colors=[colors(x, True) for x in det.cls], im_gpu=im_gpu)
 
         # Write results
         for j, d in enumerate(reversed(det)):
-            cls, conf = d.cls.squeeze(), d.conf.squeeze()
+            cls, conf, id = d.cls.squeeze(), d.conf.squeeze(), None if d.id is None else int(d.id.item())
             if self.args.save_txt:  # Write to file
-                seg = mask.segments[len(det) - j - 1].copy()  # reversed mask.segments
-                seg = seg.reshape(-1)  # (n,2) to (n*2)
-                line = (cls, *seg, conf) if self.args.save_conf else (cls, *seg)  # label format
+                seg = mask.segments[len(det) - j - 1].copy().reshape(-1)  # reversed mask.segments, (n,2) to (n*2)
+                line = (cls, *seg) + (conf, ) * self.args.save_conf + (() if id is None else (id, ))
                 with open(f'{self.txt_path}.txt', 'a') as f:
                     f.write(('%g ' * len(line)).rstrip() % line + '\n')
-
             if self.args.save or self.args.save_crop or self.args.show:  # Add bbox to image
                 c = int(cls)  # integer class
-                name = f'id:{int(d.id.item())} {self.model.names[c]}' if d.id is not None else self.model.names[c]
+                name = ('' if id is None else f'id:{id} ') + self.model.names[c]
                 label = None if self.args.hide_labels else (name if self.args.hide_conf else f'{name} {conf:.2f}')
                 self.annotator.box_label(d.xyxy.squeeze(), label, color=colors(c, True)) if self.args.boxes else None
             if self.args.save_crop:
                 save_one_box(d.xyxy,
                              imc,
                              file=self.save_dir / 'crops' / self.model.model.names[c] / f'{self.data_path.stem}.jpg',
                              BGR=True)
```

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/v8/segment/train.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/v8/segment/train.py`

 * *Files identical despite different names*

### Comparing `syml_ultralytics-8.0.49/ultralytics/yolo/v8/segment/val.py` & `syml_ultralytics-8.0.53/ultralytics/yolo/v8/segment/val.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,14 +117,15 @@
                                              ratio_pad=batch['ratio_pad'][si])
                 self.pred_to_json(predn, batch['im_file'][si], pred_masks)
             # if self.args.save_txt:
             #    save_one_txt(predn, save_conf, shape, file=save_dir / 'labels' / f'{path.stem}.txt')
 
     def finalize_metrics(self, *args, **kwargs):
         self.metrics.speed = self.speed
+        self.metrics.confusion_matrix = self.confusion_matrix
 
     def _process_batch(self, detections, labels, pred_masks=None, gt_masks=None, overlap=False, masks=False):
         """
         Return correct prediction matrix
         Arguments:
             detections (array[N, 6]), x1, y1, x2, y2, conf, class
             labels (array[M, 5]), class, x1, y1, x2, y2
```

