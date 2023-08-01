# Comparing `tmp/camunda_external_task_client_python3-4.3.0.tar.gz` & `tmp/camunda_external_task_client_python3-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camunda_external_task_client_python3-4.3.0.tar", last modified: Tue Feb 22 05:49:56 2022, max compression
+gzip compressed data, was "camunda_external_task_client_python3-4.4.0.tar", last modified: Tue Aug  1 04:18:13 2023, max compression
```

## Comparing `camunda_external_task_client_python3-4.3.0.tar` & `camunda_external_task_client_python3-4.4.0.tar`

### file list

```diff
@@ -1,67 +1,70 @@
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-02-22 05:49:56.773007 camunda_external_task_client_python3-4.3.0/
--rw-r--r--   0 apple      (501) staff       (20)    11357 2021-10-31 14:47:44.000000 camunda_external_task_client_python3-4.3.0/LICENSE
--rw-r--r--   0 apple      (501) staff       (20)    10960 2022-02-22 05:49:56.773180 camunda_external_task_client_python3-4.3.0/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)    10102 2022-01-25 10:41:23.000000 camunda_external_task_client_python3-4.3.0/README.md
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-02-22 05:49:56.716444 camunda_external_task_client_python3-4.3.0/camunda/
--rw-r--r--   0 apple      (501) staff       (20)        0 2021-10-31 14:47:44.000000 camunda_external_task_client_python3-4.3.0/camunda/__init__.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-02-22 05:49:56.717542 camunda_external_task_client_python3-4.3.0/camunda/client/
--rw-r--r--   0 apple      (501) staff       (20)        0 2021-10-31 14:47:44.000000 camunda_external_task_client_python3-4.3.0/camunda/client/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     6408 2022-01-25 10:41:23.000000 camunda_external_task_client_python3-4.3.0/camunda/client/engine_client.py
--rw-r--r--   0 apple      (501) staff       (20)     6151 2022-02-16 04:14:55.000000 camunda_external_task_client_python3-4.3.0/camunda/client/external_task_client.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-02-22 05:49:56.720910 camunda_external_task_client_python3-4.3.0/camunda/client/tests/
--rw-r--r--   0 apple      (501) staff       (20)        0 2021-10-31 14:47:44.000000 camunda_external_task_client_python3-4.3.0/camunda/client/tests/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)    11639 2022-01-25 10:41:23.000000 camunda_external_task_client_python3-4.3.0/camunda/client/tests/test_engine_client.py
--rw-r--r--   0 apple      (501) staff       (20)    12104 2022-01-25 10:41:23.000000 camunda_external_task_client_python3-4.3.0/camunda/client/tests/test_engine_client_auth.py
--rw-r--r--   0 apple      (501) staff       (20)      641 2021-10-31 14:47:44.000000 camunda_external_task_client_python3-4.3.0/camunda/client/tests/test_external_task_client.py
--rw-r--r--   0 apple      (501) staff       (20)      798 2022-01-25 10:41:23.000000 camunda_external_task_client_python3-4.3.0/camunda/client/tests/test_external_task_client_auth.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-02-22 05:49:56.723269 camunda_external_task_client_python3-4.3.0/camunda/external_task/
--rw-r--r--   0 apple      (501) staff       (20)        0 2021-10-31 14:47:44.000000 camunda_external_task_client_python3-4.3.0/camunda/external_task/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     5467 2021-10-31 14:52:48.000000 camunda_external_task_client_python3-4.3.0/camunda/external_task/external_task.py
--rw-r--r--   0 apple      (501) staff       (20)     4785 2021-10-31 14:47:44.000000 camunda_external_task_client_python3-4.3.0/camunda/external_task/external_task_executor.py
--rw-r--r--   0 apple      (501) staff       (20)     4462 2022-02-16 04:14:55.000000 camunda_external_task_client_python3-4.3.0/camunda/external_task/external_task_worker.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-02-22 05:49:56.725652 camunda_external_task_client_python3-4.3.0/camunda/external_task/tests/
--rw-r--r--   0 apple      (501) staff       (20)        0 2021-10-31 14:47:44.000000 camunda_external_task_client_python3-4.3.0/camunda/external_task/tests/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     4562 2021-10-31 14:47:44.000000 camunda_external_task_client_python3-4.3.0/camunda/external_task/tests/test_external_task.py
--rw-r--r--   0 apple      (501) staff       (20)     8673 2022-01-25 10:41:23.000000 camunda_external_task_client_python3-4.3.0/camunda/external_task/tests/test_external_task_executor.py
--rw-r--r--   0 apple      (501) staff       (20)     6178 2022-01-25 10:41:23.000000 camunda_external_task_client_python3-4.3.0/camunda/external_task/tests/test_external_task_worker.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-02-22 05:49:56.759827 camunda_external_task_client_python3-4.3.0/camunda/process_definition/
--rw-r--r--   0 apple      (501) staff       (20)        0 2021-10-31 14:47:44.000000 camunda_external_task_client_python3-4.3.0/camunda/process_definition/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     4354 2022-01-25 10:41:23.000000 camunda_external_task_client_python3-4.3.0/camunda/process_definition/process_definition_client.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-02-22 05:49:56.760758 camunda_external_task_client_python3-4.3.0/camunda/process_definition/tests/
--rw-r--r--   0 apple      (501) staff       (20)        0 2021-10-31 14:47:44.000000 camunda_external_task_client_python3-4.3.0/camunda/process_definition/tests/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     7208 2021-10-31 14:52:48.000000 camunda_external_task_client_python3-4.3.0/camunda/process_definition/tests/test_process_definition_client.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-02-22 05:49:56.763589 camunda_external_task_client_python3-4.3.0/camunda/utils/
--rw-r--r--   0 apple      (501) staff       (20)        0 2021-10-31 14:47:44.000000 camunda_external_task_client_python3-4.3.0/camunda/utils/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)      812 2022-02-16 04:14:55.000000 camunda_external_task_client_python3-4.3.0/camunda/utils/auth_basic.py
--rw-r--r--   0 apple      (501) staff       (20)      834 2021-10-31 14:47:44.000000 camunda_external_task_client_python3-4.3.0/camunda/utils/log_utils.py
--rw-r--r--   0 apple      (501) staff       (20)      774 2021-10-31 14:47:44.000000 camunda_external_task_client_python3-4.3.0/camunda/utils/response_utils.py
--rw-r--r--   0 apple      (501) staff       (20)      327 2021-10-31 14:47:44.000000 camunda_external_task_client_python3-4.3.0/camunda/utils/utils.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-02-22 05:49:56.764875 camunda_external_task_client_python3-4.3.0/camunda/variables/
--rw-r--r--   0 apple      (501) staff       (20)        0 2021-10-31 14:47:44.000000 camunda_external_task_client_python3-4.3.0/camunda/variables/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)      883 2021-10-31 14:47:44.000000 camunda_external_task_client_python3-4.3.0/camunda/variables/properties.py
--rw-r--r--   0 apple      (501) staff       (20)     1333 2022-02-22 05:47:55.000000 camunda_external_task_client_python3-4.3.0/camunda/variables/variables.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-02-22 05:49:56.766487 camunda_external_task_client_python3-4.3.0/camunda_external_task_client_python3.egg-info/
--rw-r--r--   0 apple      (501) staff       (20)    10960 2022-02-22 05:49:56.000000 camunda_external_task_client_python3-4.3.0/camunda_external_task_client_python3.egg-info/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)     2032 2022-02-22 05:49:56.000000 camunda_external_task_client_python3-4.3.0/camunda_external_task_client_python3.egg-info/SOURCES.txt
--rw-r--r--   0 apple      (501) staff       (20)        1 2022-02-22 05:49:56.000000 camunda_external_task_client_python3-4.3.0/camunda_external_task_client_python3.egg-info/dependency_links.txt
--rw-r--r--   0 apple      (501) staff       (20)       17 2022-02-22 05:49:56.000000 camunda_external_task_client_python3-4.3.0/camunda_external_task_client_python3.egg-info/requires.txt
--rw-r--r--   0 apple      (501) staff       (20)       17 2022-02-22 05:49:56.000000 camunda_external_task_client_python3-4.3.0/camunda_external_task_client_python3.egg-info/top_level.txt
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-02-22 05:49:56.770683 camunda_external_task_client_python3-4.3.0/examples/
--rw-r--r--   0 apple      (501) staff       (20)        0 2022-01-25 10:41:23.000000 camunda_external_task_client_python3-4.3.0/examples/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     2793 2021-10-31 14:47:44.000000 camunda_external_task_client_python3-4.3.0/examples/bpmn_error_example.py
--rw-r--r--   0 apple      (501) staff       (20)      269 2021-10-31 14:47:44.000000 camunda_external_task_client_python3-4.3.0/examples/correlate_message.py
--rw-r--r--   0 apple      (501) staff       (20)     1500 2021-10-31 14:47:44.000000 camunda_external_task_client_python3-4.3.0/examples/event_subprocess_example.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-02-22 05:49:56.772578 camunda_external_task_client_python3-4.3.0/examples/examples_auth_basic/
--rw-r--r--   0 apple      (501) staff       (20)        0 2022-01-25 10:41:23.000000 camunda_external_task_client_python3-4.3.0/examples/examples_auth_basic/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)      901 2022-01-25 10:41:23.000000 camunda_external_task_client_python3-4.3.0/examples/examples_auth_basic/fetch_and_execute.py
--rw-r--r--   0 apple      (501) staff       (20)      412 2022-01-25 10:41:23.000000 camunda_external_task_client_python3-4.3.0/examples/examples_auth_basic/get_process_instance.py
--rw-r--r--   0 apple      (501) staff       (20)      453 2022-01-25 10:41:23.000000 camunda_external_task_client_python3-4.3.0/examples/examples_auth_basic/start_process.py
--rw-r--r--   0 apple      (501) staff       (20)     1649 2022-01-25 10:41:23.000000 camunda_external_task_client_python3-4.3.0/examples/examples_auth_basic/task_handler_example.py
--rw-r--r--   0 apple      (501) staff       (20)      850 2021-10-31 14:47:44.000000 camunda_external_task_client_python3-4.3.0/examples/fetch_and_execute.py
--rw-r--r--   0 apple      (501) staff       (20)      349 2021-10-31 14:47:44.000000 camunda_external_task_client_python3-4.3.0/examples/get_process_instance.py
--rw-r--r--   0 apple      (501) staff       (20)     1780 2021-10-31 14:47:44.000000 camunda_external_task_client_python3-4.3.0/examples/retry_task_example.py
--rw-r--r--   0 apple      (501) staff       (20)      410 2021-10-31 14:47:44.000000 camunda_external_task_client_python3-4.3.0/examples/start_process.py
--rw-r--r--   0 apple      (501) staff       (20)     1649 2021-10-31 14:47:44.000000 camunda_external_task_client_python3-4.3.0/examples/task_handler_example.py
--rw-r--r--   0 apple      (501) staff       (20)     1049 2021-10-31 14:47:44.000000 camunda_external_task_client_python3-4.3.0/examples/tasks_example.py
--rw-r--r--   0 apple      (501) staff       (20)      964 2022-02-22 05:49:56.773873 camunda_external_task_client_python3-4.3.0/setup.cfg
--rw-r--r--   0 apple      (501) staff       (20)       36 2021-10-31 14:47:44.000000 camunda_external_task_client_python3-4.3.0/setup.py
+drwxr-xr-x   0 yogeshnaik   (502) staff       (20)        0 2023-08-01 04:18:13.986538 camunda_external_task_client_python3-4.4.0/
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)    11357 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/LICENSE
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)    10940 2023-08-01 04:18:13.986652 camunda_external_task_client_python3-4.4.0/PKG-INFO
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)    10102 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/README.md
+drwxr-xr-x   0 yogeshnaik   (502) staff       (20)        0 2023-08-01 04:18:13.975026 camunda_external_task_client_python3-4.4.0/camunda/
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)        0 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/camunda/__init__.py
+drwxr-xr-x   0 yogeshnaik   (502) staff       (20)        0 2023-08-01 04:18:13.975633 camunda_external_task_client_python3-4.4.0/camunda/client/
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)        0 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/camunda/client/__init__.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)     6827 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/camunda/client/engine_client.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)     6889 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/camunda/client/external_task_client.py
+drwxr-xr-x   0 yogeshnaik   (502) staff       (20)        0 2023-08-01 04:18:13.976941 camunda_external_task_client_python3-4.4.0/camunda/client/tests/
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)        0 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/camunda/client/tests/__init__.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)    11639 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/camunda/client/tests/test_engine_client.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)    12104 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/camunda/client/tests/test_engine_client_auth.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)    12653 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/camunda/client/tests/test_engine_client_bearer.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)      641 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/camunda/client/tests/test_external_task_client.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)      798 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/camunda/client/tests/test_external_task_client_auth.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)     1063 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/camunda/client/tests/test_external_task_client_bearer.py
+drwxr-xr-x   0 yogeshnaik   (502) staff       (20)        0 2023-08-01 04:18:13.977742 camunda_external_task_client_python3-4.4.0/camunda/external_task/
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)        0 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/camunda/external_task/__init__.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)     5467 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/camunda/external_task/external_task.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)     4785 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/camunda/external_task/external_task_executor.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)     4584 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/camunda/external_task/external_task_worker.py
+drwxr-xr-x   0 yogeshnaik   (502) staff       (20)        0 2023-08-01 04:18:13.978461 camunda_external_task_client_python3-4.4.0/camunda/external_task/tests/
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)        0 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/camunda/external_task/tests/__init__.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)     4562 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/camunda/external_task/tests/test_external_task.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)     8673 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/camunda/external_task/tests/test_external_task_executor.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)     6178 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/camunda/external_task/tests/test_external_task_worker.py
+drwxr-xr-x   0 yogeshnaik   (502) staff       (20)        0 2023-08-01 04:18:13.978789 camunda_external_task_client_python3-4.4.0/camunda/process_definition/
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)        0 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/camunda/process_definition/__init__.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)     4354 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/camunda/process_definition/process_definition_client.py
+drwxr-xr-x   0 yogeshnaik   (502) staff       (20)        0 2023-08-01 04:18:13.979214 camunda_external_task_client_python3-4.4.0/camunda/process_definition/tests/
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)        0 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/camunda/process_definition/tests/__init__.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)     7208 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/camunda/process_definition/tests/test_process_definition_client.py
+drwxr-xr-x   0 yogeshnaik   (502) staff       (20)        0 2023-08-01 04:18:13.980716 camunda_external_task_client_python3-4.4.0/camunda/utils/
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)        0 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/camunda/utils/__init__.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)      812 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/camunda/utils/auth_basic.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)      850 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/camunda/utils/auth_bearer.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)      834 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/camunda/utils/log_utils.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)      774 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/camunda/utils/response_utils.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)      327 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/camunda/utils/utils.py
+drwxr-xr-x   0 yogeshnaik   (502) staff       (20)        0 2023-08-01 04:18:13.981848 camunda_external_task_client_python3-4.4.0/camunda/variables/
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)        0 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/camunda/variables/__init__.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)      883 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/camunda/variables/properties.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)     1333 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/camunda/variables/variables.py
+drwxr-xr-x   0 yogeshnaik   (502) staff       (20)        0 2023-08-01 04:18:13.982783 camunda_external_task_client_python3-4.4.0/camunda_external_task_client_python3.egg-info/
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)    10940 2023-08-01 04:18:13.000000 camunda_external_task_client_python3-4.4.0/camunda_external_task_client_python3.egg-info/PKG-INFO
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)     2168 2023-08-01 04:18:13.000000 camunda_external_task_client_python3-4.4.0/camunda_external_task_client_python3.egg-info/SOURCES.txt
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)        1 2023-08-01 04:18:13.000000 camunda_external_task_client_python3-4.4.0/camunda_external_task_client_python3.egg-info/dependency_links.txt
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)       17 2023-08-01 04:18:13.000000 camunda_external_task_client_python3-4.4.0/camunda_external_task_client_python3.egg-info/requires.txt
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)       17 2023-08-01 04:18:13.000000 camunda_external_task_client_python3-4.4.0/camunda_external_task_client_python3.egg-info/top_level.txt
+drwxr-xr-x   0 yogeshnaik   (502) staff       (20)        0 2023-08-01 04:18:13.985245 camunda_external_task_client_python3-4.4.0/examples/
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)        0 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/examples/__init__.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)     2793 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/examples/bpmn_error_example.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)      269 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/examples/correlate_message.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)     1500 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/examples/event_subprocess_example.py
+drwxr-xr-x   0 yogeshnaik   (502) staff       (20)        0 2023-08-01 04:18:13.986330 camunda_external_task_client_python3-4.4.0/examples/examples_auth_basic/
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)        0 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/examples/examples_auth_basic/__init__.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)      901 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/examples/examples_auth_basic/fetch_and_execute.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)      412 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/examples/examples_auth_basic/get_process_instance.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)      453 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/examples/examples_auth_basic/start_process.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)     1649 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/examples/examples_auth_basic/task_handler_example.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)      850 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/examples/fetch_and_execute.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)      349 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/examples/get_process_instance.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)     1780 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/examples/retry_task_example.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)      410 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/examples/start_process.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)     1649 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/examples/task_handler_example.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)     1049 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/examples/tasks_example.py
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)      964 2023-08-01 04:18:13.988286 camunda_external_task_client_python3-4.4.0/setup.cfg
+-rw-r--r--   0 yogeshnaik   (502) staff       (20)       36 2023-08-01 04:08:36.000000 camunda_external_task_client_python3-4.4.0/setup.py
```

### Comparing `camunda_external_task_client_python3-4.3.0/LICENSE` & `camunda_external_task_client_python3-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `camunda_external_task_client_python3-4.3.0/PKG-INFO` & `camunda_external_task_client_python3-4.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: camunda_external_task_client_python3
-Version: 4.3.0
+Version: 4.4.0
 Summary: Camunda External Task Client for Python 3
 Home-page: https://github.com/yogeshrnaik/camunda-external-task-client-python3
 Author: Deserve Labs
 Author-email: devteam@deserve.com
 License: Apache-2.0
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -247,9 +246,7 @@
     return task.complete({"var1": 1, "var2": "value"})
 
 ExternalTaskWorker(worker_id="1", config=config).subscribe("topicName", handle_task)
 ```
 
 ## License
 The source files in this repository are made available under the [Apache License Version 2.0](./LICENSE).
-
-
```

### Comparing `camunda_external_task_client_python3-4.3.0/README.md` & `camunda_external_task_client_python3-4.4.0/README.md`

 * *Files identical despite different names*

### Comparing `camunda_external_task_client_python3-4.3.0/camunda/client/engine_client.py` & `camunda_external_task_client_python3-4.4.0/camunda/client/engine_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from http import HTTPStatus
 
 import requests
 
 from camunda.utils.response_utils import raise_exception_if_not_ok
 from camunda.utils.utils import join
 from camunda.utils.auth_basic import AuthBasic
+from camunda.utils.auth_bearer import AuthBearer
 from camunda.variables.variables import Variables
 
 logger = logging.getLogger(__name__)
 
 ENGINE_LOCAL_BASE_URL = "http://localhost:8080/engine-rest"
 
 
@@ -69,20 +70,29 @@
     @property
     def auth_basic(self) -> dict:
         if not self.config.get("auth_basic") or not isinstance(self.config.get("auth_basic"), dict):
             return {}
         token = AuthBasic(**self.config.get("auth_basic").copy()).token
         return {"Authorization": token}
 
+    @property
+    def auth_bearer(self) -> dict:
+        if not self.config.get("auth_bearer") or not isinstance(self.config.get("auth_bearer"), dict):
+            return {}
+        token = AuthBearer(access_token=self.config["auth_bearer"]).access_token
+        return {"Authorization": token}
+
     def _get_headers(self):
         headers = {
             "Content-Type": "application/json"
         }
         if self.auth_basic:
             headers.update(self.auth_basic)
+        if self.auth_bearer:
+            headers.update(self.auth_bearer)
         return headers
 
     def correlate_message(self, message_name, process_instance_id=None, tenant_id=None, business_key=None,
                           process_variables=None):
         """
         Correlates a message to the process engine to either trigger a message start event or
         an intermediate message catching event.
```

### Comparing `camunda_external_task_client_python3-4.3.0/camunda/client/external_task_client.py` & `camunda_external_task_client_python3-4.4.0/camunda/client/external_task_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,29 +4,32 @@
 import requests
 
 from camunda.client.engine_client import ENGINE_LOCAL_BASE_URL
 from camunda.utils.log_utils import log_with_context
 from camunda.utils.response_utils import raise_exception_if_not_ok
 from camunda.utils.utils import str_to_list
 from camunda.utils.auth_basic import AuthBasic, obfuscate_password
+from camunda.utils.auth_bearer import AuthBearer
 from camunda.variables.variables import Variables
 
 logger = logging.getLogger(__name__)
 
 
 class ExternalTaskClient:
     default_config = {
         "maxTasks": 1,
         "lockDuration": 300000,  # in milliseconds
         "asyncResponseTimeout": 30000,
         "retries": 3,
         "retryTimeout": 300000,
         "httpTimeoutMillis": 30000,
         "timeoutDeltaMillis": 5000,
-        "includeExtensionProperties": True  # enables Camunda Extension Properties
+        "includeExtensionProperties": True,  # enables Camunda Extension Properties
+        "deserializeValues": True,  # deserialize values when fetch a task by default
+        "usePriority": False
     }
 
     def __init__(self, worker_id, engine_base_url=ENGINE_LOCAL_BASE_URL, config=None):
         config = config if config is not None else {}
         self.worker_id = worker_id
         self.external_task_base_url = engine_base_url + "/external-task"
         self.config = type(self).default_config.copy()
@@ -34,21 +37,22 @@
         self.is_debug = config.get('isDebug', False)
         self.http_timeout_seconds = self.config.get('httpTimeoutMillis') / 1000
         self._log_with_context(f"Created External Task client with config: {obfuscate_password(self.config)}")
 
     def get_fetch_and_lock_url(self):
         return f"{self.external_task_base_url}/fetchAndLock"
 
-    def fetch_and_lock(self, topic_names, process_variables=None):
+    def fetch_and_lock(self, topic_names, process_variables=None, variables=None):
         url = self.get_fetch_and_lock_url()
         body = {
             "workerId": str(self.worker_id),  # convert to string to make it JSON serializable
             "maxTasks": self.config["maxTasks"],
-            "topics": self._get_topics(topic_names, process_variables),
-            "asyncResponseTimeout": self.config["asyncResponseTimeout"]
+            "topics": self._get_topics(topic_names, process_variables, variables),
+            "asyncResponseTimeout": self.config["asyncResponseTimeout"],
+            "usePriority": self.config["usePriority"]
         }
 
         if self.is_debug:
             self._log_with_context(f"trying to fetch and lock with request payload: {body}")
         http_timeout_seconds = self.__get_fetch_and_lock_http_timeout_seconds()
         response = requests.post(url, headers=self._get_headers(), json=body, timeout=http_timeout_seconds)
         raise_exception_if_not_ok(response)
@@ -58,24 +62,25 @@
             self._log_with_context(f"fetch and lock response json: {resp_json} for request: {body}")
         return response.json()
 
     def __get_fetch_and_lock_http_timeout_seconds(self):
         # use HTTP timeout slightly more than async Response / long polling timeout
         return (self.config["timeoutDeltaMillis"] + self.config["asyncResponseTimeout"]) / 1000
 
-    def _get_topics(self, topic_names, process_variables):
+    def _get_topics(self, topic_names, process_variables, variables):
         topics = []
         for topic in str_to_list(topic_names):
             topics.append({
                 "topicName": topic,
                 "lockDuration": self.config["lockDuration"],
                 "processVariables": process_variables if process_variables else {},
                 # enables Camunda Extension Properties
-                "includeExtensionProperties": self.config.get("includeExtensionProperties") or False
-
+                "includeExtensionProperties": self.config.get("includeExtensionProperties") or False,
+                "deserializeValues": self.config["deserializeValues"],
+                "variables": variables
             })
         return topics
 
     def complete(self, task_id, global_variables, local_variables=None):
         url = self.get_task_complete_url(task_id)
 
         body = {
@@ -133,18 +138,27 @@
     @property
     def auth_basic(self) -> dict:
         if not self.config.get("auth_basic") or not isinstance(self.config.get("auth_basic"), dict):
             return {}
         token = AuthBasic(**self.config.get("auth_basic").copy()).token
         return {"Authorization": token}
 
+    @property
+    def auth_bearer(self) -> dict:
+        if not self.config.get("auth_bearer") or not isinstance(self.config.get("auth_bearer"), dict):
+            return {}
+        token = AuthBearer(access_token=self.config["auth_bearer"]).access_token
+        return {"Authorization": token}
+
     def _get_headers(self):
         headers = {
             "Content-Type": "application/json"
         }
         if self.auth_basic:
             headers.update(self.auth_basic)
+        if self.auth_bearer:
+            headers.update(self.auth_bearer)
         return headers
 
     def _log_with_context(self, msg, log_level='info', **kwargs):
         context = {"WORKER_ID": self.worker_id}
         log_with_context(msg, context=context, log_level=log_level, **kwargs)
```

### Comparing `camunda_external_task_client_python3-4.3.0/camunda/client/tests/test_engine_client.py` & `camunda_external_task_client_python3-4.4.0/camunda/client/tests/test_engine_client.py`

 * *Files identical despite different names*

### Comparing `camunda_external_task_client_python3-4.3.0/camunda/client/tests/test_engine_client_auth.py` & `camunda_external_task_client_python3-4.4.0/camunda/client/tests/test_engine_client_auth.py`

 * *Files identical despite different names*

### Comparing `camunda_external_task_client_python3-4.3.0/camunda/client/tests/test_external_task_client.py` & `camunda_external_task_client_python3-4.4.0/camunda/client/tests/test_external_task_client.py`

 * *Files identical despite different names*

### Comparing `camunda_external_task_client_python3-4.3.0/camunda/client/tests/test_external_task_client_auth.py` & `camunda_external_task_client_python3-4.4.0/camunda/client/tests/test_external_task_client_auth.py`

 * *Files identical despite different names*

### Comparing `camunda_external_task_client_python3-4.3.0/camunda/external_task/external_task.py` & `camunda_external_task_client_python3-4.4.0/camunda/external_task/external_task.py`

 * *Files identical despite different names*

### Comparing `camunda_external_task_client_python3-4.3.0/camunda/external_task/external_task_executor.py` & `camunda_external_task_client_python3-4.4.0/camunda/external_task/external_task_executor.py`

 * *Files identical despite different names*

### Comparing `camunda_external_task_client_python3-4.3.0/camunda/external_task/external_task_worker.py` & `camunda_external_task_client_python3-4.4.0/camunda/external_task/external_task_worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,47 +15,49 @@
         config = config if config is not None else {}  # To avoid to have a mutable default for a parameter
         self.worker_id = worker_id
         self.client = ExternalTaskClient(self.worker_id, base_url, config)
         self.executor = ExternalTaskExecutor(self.worker_id, self.client)
         self.config = config
         self._log_with_context(f"Created new External Task Worker with config: {obfuscate_password(self.config)}")
 
-    def subscribe(self, topic_names, action, process_variables=None):
+    def subscribe(self, topic_names, action, process_variables=None, variables=None):
         while True:
-            self._fetch_and_execute_safe(topic_names, action, process_variables)
+            self._fetch_and_execute_safe(topic_names, action, process_variables, variables)
 
         self._log_with_context("Stopping worker")  # Fixme: This code seems to be unreachable?
 
-    def _fetch_and_execute_safe(self, topic_names, action, process_variables=None):
+    def _fetch_and_execute_safe(
+        self, topic_names, action, process_variables=None, variables=None
+    ):
         try:
-            self.fetch_and_execute(topic_names, action, process_variables)
+            self.fetch_and_execute(topic_names, action, process_variables, variables)
         except NoExternalTaskFound:
             self._log_with_context(f"no External Task found for Topics: {topic_names}, "
                                    f"Process variables: {process_variables}", topic=topic_names)
         except BaseException as e:
             sleep_seconds = self._get_sleep_seconds()
             self._log_with_context(f'error fetching and executing tasks: {get_exception_detail(e)} '
                                    f'for topic(s)={topic_names} with Process variables: {process_variables}. '
                                    f'retrying after {sleep_seconds} seconds', exc_info=True)
             time.sleep(sleep_seconds)
 
-    def fetch_and_execute(self, topic_names, action, process_variables=None):
+    def fetch_and_execute(self, topic_names, action, process_variables=None, variables=None):
         self._log_with_context(f"Fetching and Executing external tasks for Topics: {topic_names} "
                                f"with Process variables: {process_variables}")
-        resp_json = self._fetch_and_lock(topic_names, process_variables)
+        resp_json = self._fetch_and_lock(topic_names, process_variables, variables)
         tasks = self._parse_response(resp_json, topic_names, process_variables)
         if len(tasks) == 0:
             raise NoExternalTaskFound(f"no External Task found for Topics: {topic_names}, "
                                       f"Process variables: {process_variables}")
         self._execute_tasks(tasks, action)
 
-    def _fetch_and_lock(self, topic_names, process_variables=None):
+    def _fetch_and_lock(self, topic_names, process_variables=None, variables=None):
         self._log_with_context(f"Fetching and Locking external tasks for Topics: {topic_names} "
                                f"with Process variables: {process_variables}")
-        return self.client.fetch_and_lock(topic_names, process_variables)
+        return self.client.fetch_and_lock(topic_names, process_variables, variables)
 
     def _parse_response(self, resp_json, topic_names, process_variables):
         tasks = []
         if resp_json:
             for context in resp_json:
                 task = ExternalTask(context)
                 tasks.append(task)
```

### Comparing `camunda_external_task_client_python3-4.3.0/camunda/external_task/tests/test_external_task.py` & `camunda_external_task_client_python3-4.4.0/camunda/external_task/tests/test_external_task.py`

 * *Files identical despite different names*

### Comparing `camunda_external_task_client_python3-4.3.0/camunda/external_task/tests/test_external_task_executor.py` & `camunda_external_task_client_python3-4.4.0/camunda/external_task/tests/test_external_task_executor.py`

 * *Files identical despite different names*

### Comparing `camunda_external_task_client_python3-4.3.0/camunda/external_task/tests/test_external_task_worker.py` & `camunda_external_task_client_python3-4.4.0/camunda/external_task/tests/test_external_task_worker.py`

 * *Files identical despite different names*

### Comparing `camunda_external_task_client_python3-4.3.0/camunda/process_definition/process_definition_client.py` & `camunda_external_task_client_python3-4.4.0/camunda/process_definition/process_definition_client.py`

 * *Files identical despite different names*

### Comparing `camunda_external_task_client_python3-4.3.0/camunda/process_definition/tests/test_process_definition_client.py` & `camunda_external_task_client_python3-4.4.0/camunda/process_definition/tests/test_process_definition_client.py`

 * *Files identical despite different names*

### Comparing `camunda_external_task_client_python3-4.3.0/camunda/utils/auth_basic.py` & `camunda_external_task_client_python3-4.4.0/camunda/utils/auth_basic.py`

 * *Files identical despite different names*

### Comparing `camunda_external_task_client_python3-4.3.0/camunda/utils/log_utils.py` & `camunda_external_task_client_python3-4.4.0/camunda/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `camunda_external_task_client_python3-4.3.0/camunda/utils/response_utils.py` & `camunda_external_task_client_python3-4.4.0/camunda/utils/response_utils.py`

 * *Files identical despite different names*

### Comparing `camunda_external_task_client_python3-4.3.0/camunda/variables/properties.py` & `camunda_external_task_client_python3-4.4.0/camunda/variables/properties.py`

 * *Files identical despite different names*

### Comparing `camunda_external_task_client_python3-4.3.0/camunda/variables/variables.py` & `camunda_external_task_client_python3-4.4.0/camunda/variables/variables.py`

 * *Files identical despite different names*

### Comparing `camunda_external_task_client_python3-4.3.0/camunda_external_task_client_python3.egg-info/PKG-INFO` & `camunda_external_task_client_python3-4.4.0/camunda_external_task_client_python3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: camunda-external-task-client-python3
-Version: 4.3.0
+Version: 4.4.0
 Summary: Camunda External Task Client for Python 3
 Home-page: https://github.com/yogeshrnaik/camunda-external-task-client-python3
 Author: Deserve Labs
 Author-email: devteam@deserve.com
 License: Apache-2.0
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -247,9 +246,7 @@
     return task.complete({"var1": 1, "var2": "value"})
 
 ExternalTaskWorker(worker_id="1", config=config).subscribe("topicName", handle_task)
 ```
 
 ## License
 The source files in this repository are made available under the [Apache License Version 2.0](./LICENSE).
-
-
```

### Comparing `camunda_external_task_client_python3-4.3.0/camunda_external_task_client_python3.egg-info/SOURCES.txt` & `camunda_external_task_client_python3-4.4.0/camunda_external_task_client_python3.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,30 +5,33 @@
 camunda/__init__.py
 camunda/client/__init__.py
 camunda/client/engine_client.py
 camunda/client/external_task_client.py
 camunda/client/tests/__init__.py
 camunda/client/tests/test_engine_client.py
 camunda/client/tests/test_engine_client_auth.py
+camunda/client/tests/test_engine_client_bearer.py
 camunda/client/tests/test_external_task_client.py
 camunda/client/tests/test_external_task_client_auth.py
+camunda/client/tests/test_external_task_client_bearer.py
 camunda/external_task/__init__.py
 camunda/external_task/external_task.py
 camunda/external_task/external_task_executor.py
 camunda/external_task/external_task_worker.py
 camunda/external_task/tests/__init__.py
 camunda/external_task/tests/test_external_task.py
 camunda/external_task/tests/test_external_task_executor.py
 camunda/external_task/tests/test_external_task_worker.py
 camunda/process_definition/__init__.py
 camunda/process_definition/process_definition_client.py
 camunda/process_definition/tests/__init__.py
 camunda/process_definition/tests/test_process_definition_client.py
 camunda/utils/__init__.py
 camunda/utils/auth_basic.py
+camunda/utils/auth_bearer.py
 camunda/utils/log_utils.py
 camunda/utils/response_utils.py
 camunda/utils/utils.py
 camunda/variables/__init__.py
 camunda/variables/properties.py
 camunda/variables/variables.py
 camunda_external_task_client_python3.egg-info/PKG-INFO
```

### Comparing `camunda_external_task_client_python3-4.3.0/examples/bpmn_error_example.py` & `camunda_external_task_client_python3-4.4.0/examples/bpmn_error_example.py`

 * *Files identical despite different names*

### Comparing `camunda_external_task_client_python3-4.3.0/examples/event_subprocess_example.py` & `camunda_external_task_client_python3-4.4.0/examples/event_subprocess_example.py`

 * *Files identical despite different names*

### Comparing `camunda_external_task_client_python3-4.3.0/examples/examples_auth_basic/fetch_and_execute.py` & `camunda_external_task_client_python3-4.4.0/examples/examples_auth_basic/fetch_and_execute.py`

 * *Files identical despite different names*

### Comparing `camunda_external_task_client_python3-4.3.0/examples/examples_auth_basic/task_handler_example.py` & `camunda_external_task_client_python3-4.4.0/examples/examples_auth_basic/task_handler_example.py`

 * *Files identical despite different names*

### Comparing `camunda_external_task_client_python3-4.3.0/examples/fetch_and_execute.py` & `camunda_external_task_client_python3-4.4.0/examples/fetch_and_execute.py`

 * *Files identical despite different names*

### Comparing `camunda_external_task_client_python3-4.3.0/examples/retry_task_example.py` & `camunda_external_task_client_python3-4.4.0/examples/retry_task_example.py`

 * *Files identical despite different names*

### Comparing `camunda_external_task_client_python3-4.3.0/examples/task_handler_example.py` & `camunda_external_task_client_python3-4.4.0/examples/task_handler_example.py`

 * *Files identical despite different names*

### Comparing `camunda_external_task_client_python3-4.3.0/examples/tasks_example.py` & `camunda_external_task_client_python3-4.4.0/examples/tasks_example.py`

 * *Files identical despite different names*

### Comparing `camunda_external_task_client_python3-4.3.0/setup.cfg` & `camunda_external_task_client_python3-4.4.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = camunda_external_task_client_python3
-version = 4.3.0
+version = 4.4.0
 description = Camunda External Task Client for Python 3
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/yogeshrnaik/camunda-external-task-client-python3
 author = Deserve Labs
 author_email = devteam@deserve.com
 license = Apache-2.0
@@ -19,15 +19,15 @@
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: Software Development :: Libraries
 
 [options]
 packages = find:
 install_requires = 
-	requests==2.24.0
+	requests>=2.24.0
 python_requires = >=3.7
 include_package_data = True
 
 [options.packages.find]
 exclude = tests
 
 [egg_info]
```

