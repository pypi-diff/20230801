# Comparing `tmp/responsibleai_vision-0.2.3.tar.gz` & `tmp/responsibleai_vision-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "responsibleai_vision-0.2.3.tar", last modified: Mon Jul  3 20:08:22 2023, max compression
+gzip compressed data, was "responsibleai_vision-0.2.4.tar", last modified: Tue Aug  1 06:49:58 2023, max compression
```

## Comparing `responsibleai_vision-0.2.3.tar` & `responsibleai_vision-0.2.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:08:22.212848 responsibleai_vision-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-03 20:08:22.212848 responsibleai_vision-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:08:22.208848 responsibleai_vision-0.2.3/responsibleai_vision/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/responsibleai_vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:08:22.208848 responsibleai_vision-0.2.3/responsibleai_vision/common/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/responsibleai_vision/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/responsibleai_vision/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/responsibleai_vision/common/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:08:22.208848 responsibleai_vision-0.2.3/responsibleai_vision/managers/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/responsibleai_vision/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14054 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/responsibleai_vision/managers/error_analysis_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    27682 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/responsibleai_vision/managers/explainer_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:08:22.212848 responsibleai_vision-0.2.3/responsibleai_vision/rai_vision_insights/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/responsibleai_vision/rai_vision_insights/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47582 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/responsibleai_vision/rai_vision_insights/rai_vision_insights.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:08:22.212848 responsibleai_vision-0.2.3/responsibleai_vision/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/responsibleai_vision/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/responsibleai_vision/utils/feature_extractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/responsibleai_vision/utils/image_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/responsibleai_vision/utils/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/responsibleai_vision/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:08:22.208848 responsibleai_vision-0.2.3/responsibleai_vision.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-03 20:08:22.000000 responsibleai_vision-0.2.3/responsibleai_vision.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-03 20:08:22.000000 responsibleai_vision-0.2.3/responsibleai_vision.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 20:08:22.000000 responsibleai_vision-0.2.3/responsibleai_vision.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-03 20:08:22.000000 responsibleai_vision-0.2.3/responsibleai_vision.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 20:08:22.000000 responsibleai_vision-0.2.3/responsibleai_vision.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 20:08:22.212848 responsibleai_vision-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:08:22.212848 responsibleai_vision-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/tests/test_image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/tests/test_rai_vision_automl_images_insights.py
--rw-r--r--   0 runner    (1001) docker     (123)    13696 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/tests/test_rai_vision_insights.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/tests/test_rai_vision_insights_save_and_load_scenarios.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:49:58.915818 responsibleai_vision-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-08-01 06:49:58.915818 responsibleai_vision-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-08-01 06:39:53.000000 responsibleai_vision-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:49:58.895819 responsibleai_vision-0.2.4/responsibleai_vision/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-08-01 06:39:53.000000 responsibleai_vision-0.2.4/responsibleai_vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:49:58.899819 responsibleai_vision-0.2.4/responsibleai_vision/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-01 06:39:53.000000 responsibleai_vision-0.2.4/responsibleai_vision/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-08-01 06:39:53.000000 responsibleai_vision-0.2.4/responsibleai_vision/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-08-01 06:39:53.000000 responsibleai_vision-0.2.4/responsibleai_vision/common/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:49:58.903818 responsibleai_vision-0.2.4/responsibleai_vision/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-01 06:39:53.000000 responsibleai_vision-0.2.4/responsibleai_vision/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14054 2023-08-01 06:39:53.000000 responsibleai_vision-0.2.4/responsibleai_vision/managers/error_analysis_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27970 2023-08-01 06:39:53.000000 responsibleai_vision-0.2.4/responsibleai_vision/managers/explainer_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:49:58.907818 responsibleai_vision-0.2.4/responsibleai_vision/rai_vision_insights/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-08-01 06:39:53.000000 responsibleai_vision-0.2.4/responsibleai_vision/rai_vision_insights/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48168 2023-08-01 06:39:53.000000 responsibleai_vision-0.2.4/responsibleai_vision/rai_vision_insights/rai_vision_insights.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:49:58.911818 responsibleai_vision-0.2.4/responsibleai_vision/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-01 06:39:53.000000 responsibleai_vision-0.2.4/responsibleai_vision/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-08-01 06:39:53.000000 responsibleai_vision-0.2.4/responsibleai_vision/utils/feature_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-08-01 06:39:53.000000 responsibleai_vision-0.2.4/responsibleai_vision/utils/image_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-08-01 06:39:53.000000 responsibleai_vision-0.2.4/responsibleai_vision/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-01 06:39:53.000000 responsibleai_vision-0.2.4/responsibleai_vision/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:49:58.895819 responsibleai_vision-0.2.4/responsibleai_vision.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-08-01 06:49:58.000000 responsibleai_vision-0.2.4/responsibleai_vision.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-01 06:49:58.000000 responsibleai_vision-0.2.4/responsibleai_vision.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 06:49:58.000000 responsibleai_vision-0.2.4/responsibleai_vision.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-01 06:49:58.000000 responsibleai_vision-0.2.4/responsibleai_vision.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 06:49:58.000000 responsibleai_vision-0.2.4/responsibleai_vision.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 06:49:58.915818 responsibleai_vision-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-08-01 06:39:53.000000 responsibleai_vision-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:49:58.915818 responsibleai_vision-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-08-01 06:39:53.000000 responsibleai_vision-0.2.4/tests/test_image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-08-01 06:39:53.000000 responsibleai_vision-0.2.4/tests/test_rai_vision_automl_images_insights.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13696 2023-08-01 06:39:53.000000 responsibleai_vision-0.2.4/tests/test_rai_vision_insights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-08-01 06:39:53.000000 responsibleai_vision-0.2.4/tests/test_rai_vision_insights_save_and_load_scenarios.py
```

### Comparing `responsibleai_vision-0.2.3/PKG-INFO` & `responsibleai_vision-0.2.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: responsibleai_vision
-Version: 0.2.3
+Version: 0.2.4
 Summary: SDK API to assess image Machine Learning models.
 Home-page: https://github.com/microsoft/responsible-ai-toolbox
 Author: Roman Lutz, Ilya Matiach, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `responsibleai_vision-0.2.3/README.md` & `responsibleai_vision-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.2.3/responsibleai_vision/common/constants.py` & `responsibleai_vision-0.2.4/responsibleai_vision/common/constants.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.2.3/responsibleai_vision/managers/error_analysis_manager.py` & `responsibleai_vision-0.2.4/responsibleai_vision/managers/error_analysis_manager.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.2.3/responsibleai_vision/managers/explainer_manager.py` & `responsibleai_vision-0.2.4/responsibleai_vision/managers/explainer_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -262,22 +262,31 @@
 
                 # calling DRISE to generate saliency maps for all objects
                 mask_res_tuple = (self._mask_res, self._mask_res)
                 device = self._device
                 # get_drise_saliency_map only recognizes GPU and CPU
                 if device == Device.AUTO.value:
                     device = None
-                fl, _, _, = get_drise_saliency_map(img,
-                                                   self._model,
-                                                   len(self._classes),
-                                                   savename=str(index),
-                                                   nummasks=self._num_masks,
-                                                   maskres=mask_res_tuple,
-                                                   devicechoice=device,
-                                                   max_figures=5000)
+                try:
+                    fl, _, _, = get_drise_saliency_map(
+                        img,
+                        self._model,
+                        len(self._classes),
+                        savename=str(index),
+                        nummasks=self._num_masks,
+                        maskres=mask_res_tuple,
+                        devicechoice=device,
+                        max_figures=5000)
+                except ValueError as ve:
+                    if str(ve) == 'No detections found':
+                        raise UserConfigValidationException(
+                            "No detections found in image. "
+                            "Please increase num_masks or mask_res.")
+                    else:
+                        raise ve
                 if object_index is None:
                     return fl
                 b64_string = fl[object_index]
             except BaseException:
                 if object_index is None:
                     return [self._get_fail_str()]
                 b64_string = self._get_fail_str()
@@ -573,19 +582,21 @@
 
         :return: True if the task is an object detection task.
         :rtype: bool
         """
         return self._task_type == ModelTask.OBJECT_DETECTION
 
     def _get_fail_str(self):
-        fail = Image.new('RGB', (100, 100))
+        fail = Image.new('RGB', (250, 250))
         draw = ImageDraw.Draw(fail)
         font = ImageFont.load_default()
         text = "saliency map could not be created"
-        textwidth, textheight = draw.textsize(text, font)
+        left, top, right, bottom = draw.textbbox((0, 0), text, font)
+        textwidth = right - left
+        textheight = bottom - top
         x = (fail.width - textwidth) // 2
         y = (fail.height - textheight) // 2
         draw.text((x, y), text, fill="white", font=font)
         fail.show()
         fail.save('fail.jpg')
         image = get_image_from_path("fail.jpg", "RGB")
         jpg_img = cv2.imencode('.jpg', image)
```

### Comparing `responsibleai_vision-0.2.3/responsibleai_vision/rai_vision_insights/rai_vision_insights.py` & `responsibleai_vision-0.2.4/responsibleai_vision/rai_vision_insights/rai_vision_insights.py`

 * *Files 2% similar despite different names*

```diff
@@ -1082,28 +1082,35 @@
         return inst
 
     def compute_object_detection_metrics(
             self,
             selection_indexes,
             aggregate_method,
             class_name,
-            iou_thresh):
+            iou_threshold,
+            object_detection_cache):
         dashboard_dataset = self.get_data().dataset
         true_y = dashboard_dataset.object_detection_true_y
         predicted_y = dashboard_dataset.object_detection_predicted_y
         dashboard_dataset = self.get_data().dataset
         true_y = dashboard_dataset.object_detection_true_y
         predicted_y = dashboard_dataset.object_detection_predicted_y
 
-        iou_thresh = [iou_thresh / 100.0]
+        normalized_iou_threshold = [iou_threshold / 100.0]
         all_cohort_metrics = []
         for cohort_indices in selection_indexes:
+            key = ','.join([str(cid) for cid in cohort_indices] +
+                           [aggregate_method, class_name, str(iou_threshold)])
+            if key in object_detection_cache:
+                all_cohort_metrics.append(object_detection_cache[key])
+                continue
+
             metric_OD = MeanAveragePrecision(
                 class_metrics=True,
-                iou_thresholds=iou_thresh,
+                iou_thresholds=normalized_iou_threshold,
                 average=aggregate_method)
             true_y_cohort = [true_y[cohort_index] for cohort_index
                              in cohort_indices]
             predicted_y_cohort = [predicted_y[cohort_index] for cohort_index
                                   in cohort_indices]
 
             pred_boxes, pred_labels, pred_scores = [], [], []
@@ -1136,26 +1143,31 @@
             # this is to find the class index given
             # that there might not all classes in the cohort to predict or gt
             classes = self._classes
             classes = list(classes)
             cohort_classes = list(set([classes[i - 1]
                                   for i in pred_labels + gt_labels]))
             cohort_classes.sort(
-                key=lambda class_name: classes.index(class_name))
+                key=lambda cname: classes.index(cname))
             # to catch if the class is not in the cohort
-            try:
-                index = cohort_classes.index(class_name)
-            except ValueError:
+            if class_name not in cohort_classes:
                 all_cohort_metrics.append([-1, -1, -1])
             else:
                 metric_OD.update(cohort_pred,
                                  cohort_gt)
                 object_detection_values = metric_OD.compute()
                 mAP = round(object_detection_values
                             ['map'].item(), 2)
-                AP = round(object_detection_values
-                           ['map_per_class'][index].item(), 2)
-                AR = round(object_detection_values
-                           ['mar_100_per_class'][index].item(), 2)
-                all_cohort_metrics.append([mAP, AP, AR])
+                APs = [round(value, 2) for value in
+                       object_detection_values['map_per_class']
+                       .detach().tolist()]
+                ARs = [round(value, 2) for value in
+                       object_detection_values['mar_100_per_class']
+                       .detach().tolist()]
+
+                assert len(APs) == len(ARs) == len(cohort_classes)
+
+                all_submetrics = [[mAP, APs[i], ARs[i]]
+                                  for i in range(len(APs))]
+                all_cohort_metrics.append(all_submetrics)
 
-        return all_cohort_metrics
+        return [all_cohort_metrics, cohort_classes]
```

### Comparing `responsibleai_vision-0.2.3/responsibleai_vision/utils/feature_extractors.py` & `responsibleai_vision-0.2.4/responsibleai_vision/utils/feature_extractors.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.2.3/responsibleai_vision/utils/image_reader.py` & `responsibleai_vision-0.2.4/responsibleai_vision/utils/image_reader.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.2.3/responsibleai_vision/utils/image_utils.py` & `responsibleai_vision-0.2.4/responsibleai_vision/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.2.3/responsibleai_vision.egg-info/PKG-INFO` & `responsibleai_vision-0.2.4/responsibleai_vision.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: responsibleai-vision
-Version: 0.2.3
+Version: 0.2.4
 Summary: SDK API to assess image Machine Learning models.
 Home-page: https://github.com/microsoft/responsible-ai-toolbox
 Author: Roman Lutz, Ilya Matiach, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `responsibleai_vision-0.2.3/responsibleai_vision.egg-info/SOURCES.txt` & `responsibleai_vision-0.2.4/responsibleai_vision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.2.3/setup.py` & `responsibleai_vision-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.2.3/tests/test_image_utils.py` & `responsibleai_vision-0.2.4/tests/test_image_utils.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.2.3/tests/test_rai_vision_automl_images_insights.py` & `responsibleai_vision-0.2.4/tests/test_rai_vision_automl_images_insights.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.2.3/tests/test_rai_vision_insights.py` & `responsibleai_vision-0.2.4/tests/test_rai_vision_insights.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.2.3/tests/test_rai_vision_insights_save_and_load_scenarios.py` & `responsibleai_vision-0.2.4/tests/test_rai_vision_insights_save_and_load_scenarios.py`

 * *Files identical despite different names*

