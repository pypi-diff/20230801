# Comparing `tmp/optipack-0.0.21.dev0.tar.gz` & `tmp/optipack-0.0.22.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optipack-0.0.21.dev0.tar", max compression
+gzip compressed data, was "optipack-0.0.22.dev0.tar", max compression
```

## Comparing `optipack-0.0.21.dev0.tar` & `optipack-0.0.22.dev0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1072 2023-02-02 02:52:49.676807 optipack-0.0.21.dev0/LICENSE
--rw-r--r--   0        0        0      795 2023-02-22 03:50:53.157490 optipack-0.0.21.dev0/README.md
--rw-r--r--   0        0        0     8196 2023-02-09 02:34:16.755095 optipack-0.0.21.dev0/optipack/.DS_Store
--rw-r--r--   0        0        0      393 2023-02-23 04:45:57.676772 optipack-0.0.21.dev0/optipack/.config/app_start.yaml
--rw-r--r--   0        0        0     1152 2023-03-28 07:59:00.285290 optipack-0.0.21.dev0/optipack/.config/connection_config.yaml
--rw-r--r--   0        0        0     1105 2023-02-10 10:14:39.318351 optipack-0.0.21.dev0/optipack/.config/hyperparam_config.yaml
--rw-r--r--   0        0        0      182 2023-02-15 09:40:56.333654 optipack-0.0.21.dev0/optipack/.config/project_structure.yaml
--rw-r--r--   0        0        0      193 2023-02-10 10:47:35.669118 optipack-0.0.21.dev0/optipack/.config/run_config.yaml
--rw-r--r--   0        0        0      174 2023-04-11 04:35:43.491296 optipack-0.0.21.dev0/optipack/__init__.py
--rw-r--r--   0        0        0      487 2023-04-11 04:17:56.303032 optipack-0.0.21.dev0/optipack/__main__.py
--rw-r--r--   0        0        0     6148 2023-02-08 11:02:11.605877 optipack-0.0.21.dev0/optipack/asset/.DS_Store
--rw-r--r--   0        0        0    64098 2023-02-09 02:35:39.601968 optipack-0.0.21.dev0/optipack/asset/logo-large.png
--rw-r--r--   0        0        0    14305 2023-02-09 02:35:39.602667 optipack-0.0.21.dev0/optipack/asset/logo-small.png
--rw-r--r--   0        0        0      473 2023-02-10 10:23:56.503936 optipack-0.0.21.dev0/optipack/asset/message.txt
--rw-r--r--   0        0        0       98 2023-02-10 12:04:37.999291 optipack-0.0.21.dev0/optipack/asset/tree_vis.yaml
--rw-r--r--   0        0        0     1216 2023-03-20 02:22:23.786659 optipack-0.0.21.dev0/optipack/cli.py
--rw-r--r--   0        0        0      257 2023-04-19 04:49:17.885432 optipack-0.0.21.dev0/optipack/core/automl/builder/__init__.py
--rw-r--r--   0        0        0     3380 2023-04-05 08:46:46.918861 optipack-0.0.21.dev0/optipack/core/automl/builder/base.py
--rw-r--r--   0        0        0     3057 2023-08-01 08:01:50.431976 optipack-0.0.21.dev0/optipack/core/automl/builder/data_builder.py
--rw-r--r--   0        0        0     1252 2023-04-19 04:50:50.124725 optipack-0.0.21.dev0/optipack/core/automl/builder/metric_builder.py
--rw-r--r--   0        0        0     2100 2023-04-19 04:51:13.529341 optipack-0.0.21.dev0/optipack/core/automl/builder/model_builder.py
--rw-r--r--   0        0        0       51 2023-04-19 04:52:13.961098 optipack-0.0.21.dev0/optipack/core/automl/runner/__init__.py
--rw-r--r--   0        0        0      984 2023-04-06 08:45:17.640576 optipack-0.0.21.dev0/optipack/core/automl/runner/base.py
--rw-r--r--   0        0        0        0 2023-04-04 02:51:40.046557 optipack-0.0.21.dev0/optipack/core/automl/runner/evaluator_runner.py
--rw-r--r--   0        0        0        0 2023-04-04 02:51:40.046843 optipack-0.0.21.dev0/optipack/core/automl/runner/runner_config.py
--rw-r--r--   0        0        0      181 2023-04-06 08:45:17.641026 optipack-0.0.21.dev0/optipack/core/automl/runner/trainer_runner.py
--rw-r--r--   0        0        0     1012 2023-04-07 10:48:16.828004 optipack-0.0.21.dev0/optipack/core/fileio/reader_misc.py
--rw-r--r--   0        0        0     8409 2023-04-21 09:49:56.923568 optipack-0.0.21.dev0/optipack/core/fileio/storage_io.py
--rw-r--r--   0        0        0      741 2023-04-07 08:35:16.155017 optipack-0.0.21.dev0/optipack/core/fileio/writer_misc.py
--rw-r--r--   0        0        0      140 2023-04-19 04:41:50.728393 optipack-0.0.21.dev0/optipack/core/logger/__init__.py
--rw-r--r--   0        0        0      746 2023-04-11 04:01:15.541303 optipack-0.0.21.dev0/optipack/core/logger/base.py
--rw-r--r--   0        0        0      394 2023-08-01 08:01:50.434127 optipack-0.0.21.dev0/optipack/core/logger/logger.cfg
--rw-r--r--   0        0        0     1893 2023-04-20 10:49:19.728342 optipack-0.0.21.dev0/optipack/core/logger/otp_logger.py
--rw-r--r--   0        0        0     1076 2023-04-19 08:02:11.226814 optipack-0.0.21.dev0/optipack/core/manager/automl_manager.py
--rw-r--r--   0        0        0     3745 2023-04-19 08:02:42.526653 optipack-0.0.21.dev0/optipack/core/manager/automodel_manager.py
--rw-r--r--   0        0        0      554 2023-04-19 08:03:49.436991 optipack-0.0.21.dev0/optipack/core/manager/run_manager.py
--rw-r--r--   0        0        0     2317 2023-08-01 08:01:50.435301 optipack-0.0.21.dev0/optipack/core/typing.py
--rw-r--r--   0        0        0      143 2023-04-19 08:04:07.778785 optipack-0.0.21.dev0/optipack/core/visualizer/__init__.py
--rw-r--r--   0        0        0      250 2023-03-30 10:37:47.836408 optipack-0.0.21.dev0/optipack/core/visualizer/base.py
--rw-r--r--   0        0        0     4532 2023-08-01 08:01:50.436583 optipack-0.0.21.dev0/optipack/core/visualizer/otp_visualizer.py
--rw-r--r--   0        0        0     1040 2023-04-19 08:04:46.367924 optipack-0.0.21.dev0/optipack/internal_utils/file_util.py
--rw-r--r--   0        0        0     3784 2023-08-01 08:01:50.438031 optipack-0.0.21.dev0/optipack/internal_utils/terminal_util.py
--rw-r--r--   0        0        0      155 2023-04-10 10:17:01.113759 optipack-0.0.21.dev0/optipack/sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-02-10 05:14:38.498269 optipack-0.0.21.dev0/optipack/sdk/optipack_env_controller.py
--rw-r--r--   0        0        0     1062 2023-04-19 04:45:25.414500 optipack-0.0.21.dev0/optipack/sdk/optipack_init.py
--rw-r--r--   0        0        0     4110 2023-08-01 08:01:50.439521 optipack-0.0.21.dev0/optipack/sdk/optipack_logger.py
--rw-r--r--   0        0        0     6091 2023-08-01 08:04:26.180138 optipack-0.0.21.dev0/optipack/sdk/optipack_project_generator.py
--rw-r--r--   0        0        0      158 2023-02-23 08:07:04.463928 optipack-0.0.21.dev0/optipack/sdk/optipack_run.py
--rw-r--r--   0        0        0      249 2023-04-19 04:47:24.388598 optipack-0.0.21.dev0/optipack/sdk/optipack_utils.py
--rw-r--r--   0        0        0      535 2023-08-01 08:06:57.384075 optipack-0.0.21.dev0/pyproject.toml
--rw-r--r--   0        0        0     1966 1970-01-01 00:00:00.000000 optipack-0.0.21.dev0/setup.py
--rw-r--r--   0        0        0     1523 1970-01-01 00:00:00.000000 optipack-0.0.21.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-02-02 02:52:49.676807 optipack-0.0.22.dev0/LICENSE
+-rw-r--r--   0        0        0      795 2023-02-22 03:50:53.157490 optipack-0.0.22.dev0/README.md
+-rw-r--r--   0        0        0     8196 2023-02-09 02:34:16.755095 optipack-0.0.22.dev0/optipack/.DS_Store
+-rw-r--r--   0        0        0      393 2023-02-23 04:45:57.676772 optipack-0.0.22.dev0/optipack/.config/app_start.yaml
+-rw-r--r--   0        0        0     1152 2023-03-28 07:59:00.285290 optipack-0.0.22.dev0/optipack/.config/connection_config.yaml
+-rw-r--r--   0        0        0     1105 2023-02-10 10:14:39.318351 optipack-0.0.22.dev0/optipack/.config/hyperparam_config.yaml
+-rw-r--r--   0        0        0      182 2023-02-15 09:40:56.333654 optipack-0.0.22.dev0/optipack/.config/project_structure.yaml
+-rw-r--r--   0        0        0      193 2023-02-10 10:47:35.669118 optipack-0.0.22.dev0/optipack/.config/run_config.yaml
+-rw-r--r--   0        0        0      174 2023-04-11 04:35:43.491296 optipack-0.0.22.dev0/optipack/__init__.py
+-rw-r--r--   0        0        0      487 2023-04-11 04:17:56.303032 optipack-0.0.22.dev0/optipack/__main__.py
+-rw-r--r--   0        0        0     6148 2023-02-08 11:02:11.605877 optipack-0.0.22.dev0/optipack/asset/.DS_Store
+-rw-r--r--   0        0        0    64098 2023-02-09 02:35:39.601968 optipack-0.0.22.dev0/optipack/asset/logo-large.png
+-rw-r--r--   0        0        0    14305 2023-02-09 02:35:39.602667 optipack-0.0.22.dev0/optipack/asset/logo-small.png
+-rw-r--r--   0        0        0      473 2023-02-10 10:23:56.503936 optipack-0.0.22.dev0/optipack/asset/message.txt
+-rw-r--r--   0        0        0       98 2023-02-10 12:04:37.999291 optipack-0.0.22.dev0/optipack/asset/tree_vis.yaml
+-rw-r--r--   0        0        0     1216 2023-03-20 02:22:23.786659 optipack-0.0.22.dev0/optipack/cli.py
+-rw-r--r--   0        0        0      257 2023-04-19 04:49:17.885432 optipack-0.0.22.dev0/optipack/core/automl/builder/__init__.py
+-rw-r--r--   0        0        0     3380 2023-04-05 08:46:46.918861 optipack-0.0.22.dev0/optipack/core/automl/builder/base.py
+-rw-r--r--   0        0        0     3057 2023-08-01 08:01:50.431976 optipack-0.0.22.dev0/optipack/core/automl/builder/data_builder.py
+-rw-r--r--   0        0        0     1252 2023-04-19 04:50:50.124725 optipack-0.0.22.dev0/optipack/core/automl/builder/metric_builder.py
+-rw-r--r--   0        0        0     2100 2023-04-19 04:51:13.529341 optipack-0.0.22.dev0/optipack/core/automl/builder/model_builder.py
+-rw-r--r--   0        0        0       51 2023-04-19 04:52:13.961098 optipack-0.0.22.dev0/optipack/core/automl/runner/__init__.py
+-rw-r--r--   0        0        0      984 2023-04-06 08:45:17.640576 optipack-0.0.22.dev0/optipack/core/automl/runner/base.py
+-rw-r--r--   0        0        0        0 2023-04-04 02:51:40.046557 optipack-0.0.22.dev0/optipack/core/automl/runner/evaluator_runner.py
+-rw-r--r--   0        0        0        0 2023-04-04 02:51:40.046843 optipack-0.0.22.dev0/optipack/core/automl/runner/runner_config.py
+-rw-r--r--   0        0        0      181 2023-04-06 08:45:17.641026 optipack-0.0.22.dev0/optipack/core/automl/runner/trainer_runner.py
+-rw-r--r--   0        0        0     1012 2023-04-07 10:48:16.828004 optipack-0.0.22.dev0/optipack/core/fileio/reader_misc.py
+-rw-r--r--   0        0        0     8409 2023-04-21 09:49:56.923568 optipack-0.0.22.dev0/optipack/core/fileio/storage_io.py
+-rw-r--r--   0        0        0      741 2023-04-07 08:35:16.155017 optipack-0.0.22.dev0/optipack/core/fileio/writer_misc.py
+-rw-r--r--   0        0        0      140 2023-04-19 04:41:50.728393 optipack-0.0.22.dev0/optipack/core/logger/__init__.py
+-rw-r--r--   0        0        0      746 2023-04-11 04:01:15.541303 optipack-0.0.22.dev0/optipack/core/logger/base.py
+-rw-r--r--   0        0        0      394 2023-08-01 08:01:50.434127 optipack-0.0.22.dev0/optipack/core/logger/logger.cfg
+-rw-r--r--   0        0        0     1893 2023-04-20 10:49:19.728342 optipack-0.0.22.dev0/optipack/core/logger/otp_logger.py
+-rw-r--r--   0        0        0     1076 2023-04-19 08:02:11.226814 optipack-0.0.22.dev0/optipack/core/manager/automl_manager.py
+-rw-r--r--   0        0        0     3745 2023-04-19 08:02:42.526653 optipack-0.0.22.dev0/optipack/core/manager/automodel_manager.py
+-rw-r--r--   0        0        0      554 2023-04-19 08:03:49.436991 optipack-0.0.22.dev0/optipack/core/manager/run_manager.py
+-rw-r--r--   0        0        0     2317 2023-08-01 08:01:50.435301 optipack-0.0.22.dev0/optipack/core/typing.py
+-rw-r--r--   0        0        0      143 2023-04-19 08:04:07.778785 optipack-0.0.22.dev0/optipack/core/visualizer/__init__.py
+-rw-r--r--   0        0        0      250 2023-03-30 10:37:47.836408 optipack-0.0.22.dev0/optipack/core/visualizer/base.py
+-rw-r--r--   0        0        0     4532 2023-08-01 08:01:50.436583 optipack-0.0.22.dev0/optipack/core/visualizer/otp_visualizer.py
+-rw-r--r--   0        0        0     1040 2023-04-19 08:04:46.367924 optipack-0.0.22.dev0/optipack/internal_utils/file_util.py
+-rw-r--r--   0        0        0     3793 2023-08-01 08:11:06.079853 optipack-0.0.22.dev0/optipack/internal_utils/terminal_util.py
+-rw-r--r--   0        0        0      155 2023-04-10 10:17:01.113759 optipack-0.0.22.dev0/optipack/sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-10 05:14:38.498269 optipack-0.0.22.dev0/optipack/sdk/optipack_env_controller.py
+-rw-r--r--   0        0        0     1062 2023-04-19 04:45:25.414500 optipack-0.0.22.dev0/optipack/sdk/optipack_init.py
+-rw-r--r--   0        0        0     4110 2023-08-01 08:01:50.439521 optipack-0.0.22.dev0/optipack/sdk/optipack_logger.py
+-rw-r--r--   0        0        0     6091 2023-08-01 08:04:26.180138 optipack-0.0.22.dev0/optipack/sdk/optipack_project_generator.py
+-rw-r--r--   0        0        0      158 2023-02-23 08:07:04.463928 optipack-0.0.22.dev0/optipack/sdk/optipack_run.py
+-rw-r--r--   0        0        0      249 2023-04-19 04:47:24.388598 optipack-0.0.22.dev0/optipack/sdk/optipack_utils.py
+-rw-r--r--   0        0        0      535 2023-08-01 08:10:26.545782 optipack-0.0.22.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1966 1970-01-01 00:00:00.000000 optipack-0.0.22.dev0/setup.py
+-rw-r--r--   0        0        0     1523 1970-01-01 00:00:00.000000 optipack-0.0.22.dev0/PKG-INFO
```

### Comparing `optipack-0.0.21.dev0/LICENSE` & `optipack-0.0.22.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `optipack-0.0.21.dev0/README.md` & `optipack-0.0.22.dev0/README.md`

 * *Files identical despite different names*

### Comparing `optipack-0.0.21.dev0/optipack/.DS_Store` & `optipack-0.0.22.dev0/optipack/.DS_Store`

 * *Files identical despite different names*

### Comparing `optipack-0.0.21.dev0/optipack/.config/connection_config.yaml` & `optipack-0.0.22.dev0/optipack/.config/connection_config.yaml`

 * *Files identical despite different names*

### Comparing `optipack-0.0.21.dev0/optipack/.config/hyperparam_config.yaml` & `optipack-0.0.22.dev0/optipack/.config/hyperparam_config.yaml`

 * *Files identical despite different names*

### Comparing `optipack-0.0.21.dev0/optipack/asset/.DS_Store` & `optipack-0.0.22.dev0/optipack/asset/.DS_Store`

 * *Files identical despite different names*

### Comparing `optipack-0.0.21.dev0/optipack/asset/logo-large.png` & `optipack-0.0.22.dev0/optipack/asset/logo-large.png`

 * *Files identical despite different names*

### Comparing `optipack-0.0.21.dev0/optipack/asset/logo-small.png` & `optipack-0.0.22.dev0/optipack/asset/logo-small.png`

 * *Files identical despite different names*

### Comparing `optipack-0.0.21.dev0/optipack/cli.py` & `optipack-0.0.22.dev0/optipack/cli.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.21.dev0/optipack/core/automl/builder/base.py` & `optipack-0.0.22.dev0/optipack/core/automl/builder/base.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.21.dev0/optipack/core/automl/builder/data_builder.py` & `optipack-0.0.22.dev0/optipack/core/automl/builder/data_builder.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.21.dev0/optipack/core/automl/builder/metric_builder.py` & `optipack-0.0.22.dev0/optipack/core/automl/builder/metric_builder.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.21.dev0/optipack/core/automl/builder/model_builder.py` & `optipack-0.0.22.dev0/optipack/core/automl/builder/model_builder.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.21.dev0/optipack/core/automl/runner/base.py` & `optipack-0.0.22.dev0/optipack/core/automl/runner/base.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.21.dev0/optipack/core/fileio/reader_misc.py` & `optipack-0.0.22.dev0/optipack/core/fileio/reader_misc.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.21.dev0/optipack/core/fileio/storage_io.py` & `optipack-0.0.22.dev0/optipack/core/fileio/storage_io.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.21.dev0/optipack/core/fileio/writer_misc.py` & `optipack-0.0.22.dev0/optipack/core/fileio/writer_misc.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.21.dev0/optipack/core/logger/base.py` & `optipack-0.0.22.dev0/optipack/core/logger/base.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.21.dev0/optipack/core/logger/otp_logger.py` & `optipack-0.0.22.dev0/optipack/core/logger/otp_logger.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.21.dev0/optipack/core/manager/automl_manager.py` & `optipack-0.0.22.dev0/optipack/core/manager/automl_manager.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.21.dev0/optipack/core/manager/automodel_manager.py` & `optipack-0.0.22.dev0/optipack/core/manager/automodel_manager.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.21.dev0/optipack/core/manager/run_manager.py` & `optipack-0.0.22.dev0/optipack/core/manager/run_manager.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.21.dev0/optipack/core/typing.py` & `optipack-0.0.22.dev0/optipack/core/typing.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.21.dev0/optipack/core/visualizer/otp_visualizer.py` & `optipack-0.0.22.dev0/optipack/core/visualizer/otp_visualizer.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.21.dev0/optipack/internal_utils/file_util.py` & `optipack-0.0.22.dev0/optipack/internal_utils/file_util.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.21.dev0/optipack/internal_utils/terminal_util.py` & `optipack-0.0.22.dev0/optipack/internal_utils/terminal_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         return 
     
     rich_console.rule('Welcome to Optip⍙ck')
     msg = read_text(message_path)
     rich_console.print(Align.center(Panel.fit(msg), style= 'bold yellow'))
 
 def visualize_folder_tree(parent_dir, project_name): 
-    from core.fileio.reader_misc import read_yaml
+    from optipack.core.fileio.reader_misc import read_yaml
     tree_vis_dir = os.path.join(
         os.environ.get('OPTIPACK_PATH'), 
         os.environ.get('TREE_VIS_PATH')
     )
     global tree_vis
     tree_vis = read_yaml(tree_vis_dir)
     tree = Tree(f'{project_name} structure')
```

### Comparing `optipack-0.0.21.dev0/optipack/sdk/optipack_init.py` & `optipack-0.0.22.dev0/optipack/sdk/optipack_init.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.21.dev0/optipack/sdk/optipack_logger.py` & `optipack-0.0.22.dev0/optipack/sdk/optipack_logger.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.21.dev0/optipack/sdk/optipack_project_generator.py` & `optipack-0.0.22.dev0/optipack/sdk/optipack_project_generator.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.21.dev0/pyproject.toml` & `optipack-0.0.22.dev0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "optipack"
-version = "0.0.21-dev"
+version = "0.0.22-dev"
 description = "The optimal ML package"
 authors = ["indigoYoshimaru"]
 readme = "README.md"
 include = ["optipack/.config/project_structure.yaml"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `optipack-0.0.21.dev0/setup.py` & `optipack-0.0.22.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
  'typer>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['optipack = optipack.__main__:start']}
 
 setup_kwargs = {
     'name': 'optipack',
-    'version': '0.0.21.dev0',
+    'version': '0.0.22.dev0',
     'description': 'The optimal ML package',
     'long_description': "![optipack](asset/image/logo.png)\n\n# What optipack do: \n- Workspace management: \n    - Generate folder structure for ML project \n    - Generate files following the given environment in yaml format, including: \n        - tool connection configuration \n        - hyperparameter configuration \n        - model run config\n-  Logging: 🔥 all-in-one logger\n    - Support console/file logger for users' log! 🔥 No more uggly print, no more terminal scrolling\n    - Support tensorboard metric log. \n\n# Installation:  \n## 1. Installation from PYPI: \n- Run `pip install optipack`\n## 2. Installation from source: \n- Clone this repo \n- Change directory to optipack\n- Run `pip install . `\n\n# How to use: \n## 1. Use as CLI \n- All you need is running `optipack` on terminal :) \n\n## 2. Use as library\n- ... ",
     'author': 'indigoYoshimaru',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `optipack-0.0.21.dev0/PKG-INFO` & `optipack-0.0.22.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optipack
-Version: 0.0.21.dev0
+Version: 0.0.22.dev0
 Summary: The optimal ML package
 Author: indigoYoshimaru
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

