# Comparing `tmp/testflows.github.runners-1.3.230731.1223752.tar.gz` & `tmp/testflows.github.runners-1.3.230801.1034814.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.3.230731.1223752.tar", last modified: Mon Jul 31 22:37:52 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.3.230801.1034814.tar", last modified: Tue Aug  1 03:48:14 2023, max compression
```

## Comparing `testflows.github.runners-1.3.230731.1223752.tar` & `testflows.github.runners-1.3.230801.1034814.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 22:37:52.540387 testflows.github.runners-1.3.230731.1223752/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1223752/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    57204 2023-07-31 22:37:52.536387 testflows.github.runners-1.3.230731.1223752/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    56612 2023-07-31 22:37:49.000000 testflows.github.runners-1.3.230731.1223752/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-31 22:37:52.540387 testflows.github.runners-1.3.230731.1223752/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-31 22:37:52.000000 testflows.github.runners-1.3.230731.1223752/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 22:37:52.536387 testflows.github.runners-1.3.230731.1223752/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 22:37:52.536387 testflows.github.runners-1.3.230731.1223752/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 22:37:52.536387 testflows.github.runners-1.3.230731.1223752/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-31 22:37:52.000000 testflows.github.runners-1.3.230731.1223752/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1615 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1223752/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     2599 2023-07-31 15:05:55.000000 testflows.github.runners-1.3.230731.1223752/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 22:37:52.536387 testflows.github.runners-1.3.230731.1223752/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    23381 2023-07-31 15:15:18.000000 testflows.github.runners-1.3.230731.1223752/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)    13607 2023-07-29 23:57:40.000000 testflows.github.runners-1.3.230731.1223752/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     4164 2023-07-31 15:16:54.000000 testflows.github.runners-1.3.230731.1223752/testflows/github/runners/config.py
--rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.3.230731.1223752/testflows/github/runners/delete.py
--rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1223752/testflows/github/runners/logger.py
--rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.3.230731.1223752/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)    10814 2023-07-29 23:14:39.000000 testflows.github.runners-1.3.230731.1223752/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    16903 2023-07-31 15:02:38.000000 testflows.github.runners-1.3.230731.1223752/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 22:37:52.536387 testflows.github.runners-1.3.230731.1223752/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1223752/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 22:37:52.536387 testflows.github.runners-1.3.230731.1223752/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1223752/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1223752/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.3.230731.1223752/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.3.230731.1223752/testflows/github/runners/scripts/setup_docker.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1223752/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1223752/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1223752/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     5158 2023-07-31 17:30:38.000000 testflows.github.runners-1.3.230731.1223752/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1223752/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 22:37:52.536387 testflows.github.runners-1.3.230731.1223752/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    57204 2023-07-31 22:37:52.000000 testflows.github.runners-1.3.230731.1223752/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1154 2023-07-31 22:37:52.000000 testflows.github.runners-1.3.230731.1223752/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-31 22:37:52.000000 testflows.github.runners-1.3.230731.1223752/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.3.230731.1223752/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-31 22:37:52.000000 testflows.github.runners-1.3.230731.1223752/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-31 22:37:52.000000 testflows.github.runners-1.3.230731.1223752/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 03:48:14.471269 testflows.github.runners-1.3.230801.1034814/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1034814/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    57192 2023-08-01 03:48:14.467269 testflows.github.runners-1.3.230801.1034814/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    56600 2023-07-31 22:43:07.000000 testflows.github.runners-1.3.230801.1034814/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-08-01 03:48:14.471269 testflows.github.runners-1.3.230801.1034814/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2043 2023-08-01 03:48:14.000000 testflows.github.runners-1.3.230801.1034814/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 03:48:14.467269 testflows.github.runners-1.3.230801.1034814/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 03:48:14.467269 testflows.github.runners-1.3.230801.1034814/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 03:48:14.467269 testflows.github.runners-1.3.230801.1034814/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-08-01 03:48:14.000000 testflows.github.runners-1.3.230801.1034814/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1615 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1034814/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1951 2023-08-01 03:44:03.000000 testflows.github.runners-1.3.230801.1034814/testflows/github/runners/api_watch.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2599 2023-07-31 15:05:55.000000 testflows.github.runners-1.3.230801.1034814/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 03:48:14.467269 testflows.github.runners-1.3.230801.1034814/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    24374 2023-08-01 03:43:45.000000 testflows.github.runners-1.3.230801.1034814/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)    13607 2023-07-29 23:57:40.000000 testflows.github.runners-1.3.230801.1034814/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4164 2023-08-01 01:08:42.000000 testflows.github.runners-1.3.230801.1034814/testflows/github/runners/config.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.3.230801.1034814/testflows/github/runners/delete.py
+-rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1034814/testflows/github/runners/logger.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.3.230801.1034814/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11279 2023-08-01 03:43:12.000000 testflows.github.runners-1.3.230801.1034814/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    17362 2023-08-01 03:14:02.000000 testflows.github.runners-1.3.230801.1034814/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 03:48:14.467269 testflows.github.runners-1.3.230801.1034814/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1034814/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 03:48:14.467269 testflows.github.runners-1.3.230801.1034814/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1034814/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1034814/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.3.230801.1034814/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.3.230801.1034814/testflows/github/runners/scripts/setup_docker.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1034814/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1034814/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1034814/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5158 2023-07-31 17:30:38.000000 testflows.github.runners-1.3.230801.1034814/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1034814/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 03:48:14.467269 testflows.github.runners-1.3.230801.1034814/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    57192 2023-08-01 03:48:14.000000 testflows.github.runners-1.3.230801.1034814/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1192 2023-08-01 03:48:14.000000 testflows.github.runners-1.3.230801.1034814/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-01 03:48:14.000000 testflows.github.runners-1.3.230801.1034814/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.3.230801.1034814/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       61 2023-08-01 03:48:14.000000 testflows.github.runners-1.3.230801.1034814/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-08-01 03:48:14.000000 testflows.github.runners-1.3.230801.1034814/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.3.230731.1223752/LICENSE` & `testflows.github.runners-1.3.230801.1034814/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1223752/PKG-INFO` & `testflows.github.runners-1.3.230801.1034814/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.3.230731.1223752
+Version: 1.3.230801.1034814
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -230,18 +230,19 @@
 
 The repository name will have the following format:
 
 ::
 
    <username>/demo-testflows-github-runners
 
-:For me, my GitHub repository is:
-   ::
+For me, my GitHub repository is:
+
+::
 
-      vzakaznikov/demo-testflows-github-runners
+   vzakaznikov/demo-testflows-github-runners
 
 ❷ Now, create an example GitHub Actions workflow as described in the `Quickstart for GitHub Actions <https://docs.github.com/en/actions/quickstart>`_ article.
 Note that we need to modify the example YAML configuration and specify that our job will run on a runner with the **self-hosted** and the **type-cpx21**
 labels.
 
 .. code-block:: yaml
 
@@ -272,18 +273,19 @@
               run: |
                 ls ${{ github.workspace }}
             - run: echo "🍏 This job's status is ${{ job.status }}."
 
 
 ❸ Finally, you will need to create a GitHub API token with the **workflow** privileges. Make sure to save the token!
 
-:For me, my *demo* GitHub token is:
-   ::
+For me, my *demo* GitHub token is:
+
+::
 
-      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
+   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
 
 You should now have your GitHub repository ready.
 
 See these steps in action:
 
 .. image:: https://raw.githubusercontent.com/testflows/TestFlows-GitHub-Runners/master/docs/images/github_create_repo_and_token.gif
    :align: center
@@ -296,18 +298,19 @@
 
 Next you will need to create a Hetzner Cloud project and an API token that we can use to create an manage Hetzner Cloud server instances.
 
 ❶ Create new Hetzner Cloud project **Demo GitHub Runners**.
 
 ❷ Now, create an API token and save it.
 
-:For me, the Hetzner Cloud token for my *Demo GitHub Runners* project is:
-   ::
-
-      5Up04IHuY8mC7l0JxKwh3Aps4ghGIyL0NJ9rGlhyAmmkddzuRreR1YstTSTFCG0N
+For me, the Hetzner Cloud token for my *Demo GitHub Runners* project is:
+   
+::
+   
+   5Up04IHuY8mC7l0JxKwh3Aps4ghGIyL0NJ9rGlhyAmmkddzuRreR1YstTSTFCG0N
 
 You should now have your Hetzner Cloud project ready.
 
 See these steps in action:
 
 .. image:: https://raw.githubusercontent.com/testflows/TestFlows-GitHub-Runners/master/docs/images/hetzner_create_project_and_token.gif
    :align: center
@@ -337,15 +340,15 @@
 
 You should now have the cloud service up and running.
 
 See these steps in action:
 
 .. image:: https://raw.githubusercontent.com/testflows/TestFlows-GitHub-Runners/master/docs/images/cloud_deploy.gif
    :align: center
-   :width: 790px
+   :width: 625px
    :alt: Deploying Cloud Service
 
 ------------------------------------------
 Waiting for GitHub Actions Job to Complete
 ------------------------------------------
 
 ❶ The **github-runners** cloud service is now running. So, now you can just seat back and wait until **github-runners**
```

### Comparing `testflows.github.runners-1.3.230731.1223752/README.rst` & `testflows.github.runners-1.3.230801.1034814/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: testflows.github.runners
+Version: 1.3.230801.1034814
+Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
+Home-page: https://github.com/testflows/github-runners
+Author: Vitaliy Zakaznikov
+Author-email: vzakaznikov@testflows.com
+License: Apache-2.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
+License-File: LICENSE
+
 .. image:: https://raw.githubusercontent.com/testflows/TestFlows-ArtWork/master/images/logo.png
    :width: 300px
    :align: center
    :target: https://testflows.com
    :alt: TestFlows Open-source Testing Framework
 
 ----
@@ -213,18 +230,19 @@
 
 The repository name will have the following format:
 
 ::
 
    <username>/demo-testflows-github-runners
 
-:For me, my GitHub repository is:
-   ::
+For me, my GitHub repository is:
+
+::
 
-      vzakaznikov/demo-testflows-github-runners
+   vzakaznikov/demo-testflows-github-runners
 
 ❷ Now, create an example GitHub Actions workflow as described in the `Quickstart for GitHub Actions <https://docs.github.com/en/actions/quickstart>`_ article.
 Note that we need to modify the example YAML configuration and specify that our job will run on a runner with the **self-hosted** and the **type-cpx21**
 labels.
 
 .. code-block:: yaml
 
@@ -255,18 +273,19 @@
               run: |
                 ls ${{ github.workspace }}
             - run: echo "🍏 This job's status is ${{ job.status }}."
 
 
 ❸ Finally, you will need to create a GitHub API token with the **workflow** privileges. Make sure to save the token!
 
-:For me, my *demo* GitHub token is:
-   ::
+For me, my *demo* GitHub token is:
 
-      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
+::
+
+   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
 
 You should now have your GitHub repository ready.
 
 See these steps in action:
 
 .. image:: https://raw.githubusercontent.com/testflows/TestFlows-GitHub-Runners/master/docs/images/github_create_repo_and_token.gif
    :align: center
@@ -279,18 +298,19 @@
 
 Next you will need to create a Hetzner Cloud project and an API token that we can use to create an manage Hetzner Cloud server instances.
 
 ❶ Create new Hetzner Cloud project **Demo GitHub Runners**.
 
 ❷ Now, create an API token and save it.
 
-:For me, the Hetzner Cloud token for my *Demo GitHub Runners* project is:
-   ::
-
-      5Up04IHuY8mC7l0JxKwh3Aps4ghGIyL0NJ9rGlhyAmmkddzuRreR1YstTSTFCG0N
+For me, the Hetzner Cloud token for my *Demo GitHub Runners* project is:
+   
+::
+   
+   5Up04IHuY8mC7l0JxKwh3Aps4ghGIyL0NJ9rGlhyAmmkddzuRreR1YstTSTFCG0N
 
 You should now have your Hetzner Cloud project ready.
 
 See these steps in action:
 
 .. image:: https://raw.githubusercontent.com/testflows/TestFlows-GitHub-Runners/master/docs/images/hetzner_create_project_and_token.gif
    :align: center
@@ -320,15 +340,15 @@
 
 You should now have the cloud service up and running.
 
 See these steps in action:
 
 .. image:: https://raw.githubusercontent.com/testflows/TestFlows-GitHub-Runners/master/docs/images/cloud_deploy.gif
    :align: center
-   :width: 790px
+   :width: 625px
    :alt: Deploying Cloud Service
 
 ------------------------------------------
 Waiting for GitHub Actions Job to Complete
 ------------------------------------------
 
 ❶ The **github-runners** cloud service is now running. So, now you can just seat back and wait until **github-runners**
```

### Comparing `testflows.github.runners-1.3.230731.1223752/setup.py` & `testflows.github.runners-1.3.230801.1034814/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.3.230731.1223752",
+    version="1.3.230801.1034814",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
@@ -45,10 +45,10 @@
     package_data={
         "testflows.github.runners.scripts": ["*.sh"],
         "testflows.github.runners.scripts.deploy": ["*.sh"],
         "testflows.github.runners.bin": ["github-runners"],
     },
     scripts=["testflows/github/runners/bin/github-runners"],
     zip_safe=False,
-    install_requires=["PyGithub==1.59.0", "hcloud==1.26.0"],
+    install_requires=["PyGithub==1.59.0", "hcloud==1.26.0", "requests-cache==1.1.0"],
     extras_require={"dev": []},
 )
```

### Comparing `testflows.github.runners-1.3.230731.1223752/testflows/github/runners/__init__.py` & `testflows.github.runners-1.3.230801.1034814/testflows/github/runners/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.3.230731.1223752"
+__version__ = "1.3.230801.1034814"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.3.230731.1223752/testflows/github/runners/actions.py` & `testflows.github.runners-1.3.230801.1034814/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1223752/testflows/github/runners/args.py` & `testflows.github.runners-1.3.230801.1034814/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1223752/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.3.230801.1034814/testflows/github/runners/bin/github-runners`

 * *Files 2% similar despite different names*

```diff
@@ -30,23 +30,33 @@
 
 from argparse import ArgumentParser, RawTextHelpFormatter
 
 from testflows.github.runners import __version__, __license__
 from testflows.github.runners.actions import Action
 from testflows.github.runners.scale_up import scale_up
 from testflows.github.runners.scale_down import scale_down
+from testflows.github.runners.api_watch import api_watch
 from testflows.github.runners.scripts import Scripts, scripts
 from testflows.github.runners.logger import logger
 from testflows.github.runners.config import Config, check_image
 
 import testflows.github.runners.args as args
 import testflows.github.runners.cloud as cloud
 import testflows.github.runners.service as service
 import testflows.github.runners.delete as delete
 
+from requests_cache import DO_NOT_CACHE, EXPIRE_IMMEDIATELY, install_cache
+
+install_cache(
+    cache_control=True,
+    urls_expire_after={
+        '*.github.com': EXPIRE_IMMEDIATELY,
+        '*': DO_NOT_CACHE,
+    },
+)
 
 description = """Auto-scaling GitHub Actions runners service using Hetzner Cloud.
 
     Service that starts and monitors queued up GitHub Actions workflows.
     When a new job is queued up, it creates new Hetzner Cloud server instance
     that provides an ephemeral GitHub Actions runner. Server is automatically
     powered off when job completes and then powered off servers are
@@ -579,15 +589,15 @@
     terminate = threading.Event()
 
     try:
         with Action("Logging in to Hetzner Cloud"):
             client = Client(token=config.hetzner_token)
 
         with Action("Logging in to GitHub"):
-            github = Github(login_or_token=config.github_token)
+            github = Github(login_or_token=config.github_token, per_page=100)
 
         with Action(f"Getting repository {config.github_repository}"):
             repo: Repository = github.get_repo(config.github_repository)
 
         with Action("Checking if default image exists"):
             config.default_image = check_image(
                 client=client, image=config.default_image
@@ -606,68 +616,84 @@
                     )
 
         try:
             with Action("Creating scale up service"):
                 scale_up_service: Future = worker_pool.submit(
                     scale_up,
                     terminate=terminate,
-                    repo=repo,
-                    client=client,
                     scripts=scripts,
                     ssh_key=ssh_key,
                     default_server_type=config.default_server_type,
                     default_image=config.default_image,
                     default_location=config.default_location,
                     worker_pool=worker_pool,
+                    hetzner_token=config.hetzner_token,
                     github_token=config.github_token,
                     github_repository=config.github_repository,
                     interval=config.scale_up_interval,
                     max_servers=config.max_runners,
                     max_server_ready_time=config.max_server_ready_time,
                     debug=config.debug,
                     standby_runners=config.standby_runners,
                 )
 
             with Action("Creating scale down service"):
                 scale_down_service: Future = worker_pool.submit(
                     scale_down,
+                    hetzner_token=config.hetzner_token,
+                    github_token=config.github_token,
+                    github_repository=config.github_repository,
                     terminate=terminate,
-                    repo=repo,
-                    client=client,
                     max_powered_off_time=config.max_powered_off_time,
                     max_unused_runner_time=config.max_unused_runner_time,
                     max_runner_registration_time=config.max_runner_registration_time,
                     interval=config.scale_down_interval,
                     debug=config.debug,
                     standby_runners=config.standby_runners,
                 )
 
+            with Action("Creating GitHub API calls watch service"):
+                api_watch_service: Future = worker_pool.submit(
+                    api_watch,
+                    terminate=terminate,
+                    github_token=config.github_token,
+                )
+
             while True:
                 time.sleep(1)
 
                 if scale_up_service.done():
                     raise RuntimeError("scale-up service exited")
 
                 if scale_down_service.done():
                     raise RuntimeError("scale-down service exited")
 
+                if api_watch_service.done():
+                    raise RuntimeError("GitHub API calls watch service exited")
+
         except BaseException:
             with Action("Requesting all services to terminate"):
                 terminate.set()
             raise
 
         finally:
             with Action("Waiting for scale up service to terminate", ignore_fail=True):
                 scale_down_service.result(timeout=terminate_timeout)
 
             with Action(
                 "Waiting for scale down service to terminate", ignore_fail=True
             ):
                 scale_up_service.result(timeout=terminate_timeout)
 
+            with Action(
+                "Waiting for GitHub API calls watch service to terminate", ignore_fail=True
+            ):
+                api_watch_service.result(timeout=terminate_timeout)
+
+
     except KeyboardInterrupt as exc:
         msg = "❗ KeyboardInterrupt"
         if config.debug:
             logger.exception(f"{msg}\n{exc}")
         else:
             logger.error(msg)
         sys.exit(1)
@@ -729,10 +755,10 @@
                 raise
             logger.fatal(f"❗ Error: {exc}")
 
     else:
         config.check()
 
         with ThreadPoolExecutor(
-            max_workers=config.workers + 2, thread_name_prefix="worker"
+            max_workers=config.workers + 3, thread_name_prefix="worker"
         ) as worker_pool:
             main(config=config, scripts=scripts, worker_pool=worker_pool)
```

### Comparing `testflows.github.runners-1.3.230731.1223752/testflows/github/runners/cloud.py` & `testflows.github.runners-1.3.230801.1034814/testflows/github/runners/cloud.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1223752/testflows/github/runners/config.py` & `testflows.github.runners-1.3.230801.1034814/testflows/github/runners/config.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1223752/testflows/github/runners/delete.py` & `testflows.github.runners-1.3.230801.1034814/testflows/github/runners/delete.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1223752/testflows/github/runners/logger.py` & `testflows.github.runners-1.3.230801.1034814/testflows/github/runners/logger.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1223752/testflows/github/runners/request.py` & `testflows.github.runners-1.3.230801.1034814/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1223752/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.3.230801.1034814/testflows/github/runners/scale_down.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     server_name_prefix,
     runner_name_prefix,
     standby_runner_name_prefix,
     StandbyRunner,
 )
 from .logger import logger
 
+from github import Github
 from github.Repository import Repository
 from github.SelfHostedActionsRunner import SelfHostedActionsRunner
 
 from hcloud import Client
 from hcloud.servers.client import BoundServer
 
 
@@ -60,16 +61,17 @@
     time: float
     runner: SelfHostedActionsRunner
     observed_interval: float
 
 
 def scale_down(
     terminate: threading.Event,
-    repo: Repository,
-    client: Client,
+    hetzner_token: str,
+    github_token: str,
+    github_repository: str,
     max_powered_off_time: int,
     max_unused_runner_time: int,
     max_runner_registration_time: int,
     interval: int,
     debug: bool = False,
     standby_runners: list[StandbyRunner] = None,
 ):
@@ -77,14 +79,23 @@
     any server that has unused runner, or any server that failed to register its
     runner (zombie server).
     """
     powered_off_servers: dict[str, PoweredOffServer] = {}
     unused_runners: dict[str, UnusedRunner] = {}
     zombie_servers: dict[str, ZombieServer] = {}
 
+    with Action("Logging in to Hetzner Cloud"):
+        client = Client(token=hetzner_token)
+
+    with Action("Logging in to GitHub"):
+        github = Github(login_or_token=github_token, per_page=100)
+
+    with Action(f"Getting repository {github_repository}"):
+        repo: Repository = github.get_repo(github_repository)
+
     while True:
         current_interval = time.time()
 
         if terminate.is_set():
             with Action("Terminating scale down service"):
                 break
 
@@ -135,15 +146,17 @@
 
                         else:
                             zombie_servers.pop(server.name, None)
 
             with Action("Looking for unused runners", level=logging.DEBUG):
                 _standby_runners = copy.deepcopy(standby_runners)
                 for runner in runners:
-                    if runner.status == "online" and not runner.busy:
+                    if (runner.status == "online" and not runner.busy) or (
+                        runner.status == "offline"
+                    ):
                         if runner.name.startswith(runner_name_prefix):
                             # skip any specified standby runners
                             if runner.name.startswith(standby_runner_name_prefix):
                                 found = False
                                 for standby_runner in _standby_runners:
                                     if set(standby_runner.labels).issubset(
                                         set(
```

### Comparing `testflows.github.runners-1.3.230731.1223752/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.3.230801.1034814/testflows/github/runners/scale_up.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 from hcloud.server_types.domain import ServerType
 from hcloud.locations.domain import Location
 from hcloud.servers.client import BoundServer
 from hcloud.servers.domain import Server
 from hcloud.images.domain import Image
 from hcloud.helpers.labels import LabelValidator
 
+from github import Github
 from github.Repository import Repository
 from github.WorkflowJob import WorkflowJob
 from github.WorkflowRun import WorkflowRun
 from github.SelfHostedActionsRunner import SelfHostedActionsRunner
 
 from concurrent.futures import ThreadPoolExecutor, Future
 
@@ -169,29 +170,31 @@
     if server_type.name.lower().startswith("ca"):
         return scripts.startup_arm64
 
     return scripts.startup_x64
 
 
 def create_server(
+    hetzner_token: str,
     setup_worker_pool: ThreadPoolExecutor,
-    client: Client,
     labels: set[str],
     name: str,
     default_server_type: ServerType,
     default_location: Location,
     default_image: Image,
     scripts: Scripts,
     github_token: str,
     github_repository: str,
     ssh_key: SSHKey,
     timeout=60,
 ):
     """Create specified number of server instances."""
 
+    client = Client(token=hetzner_token)
+
     server_type = get_server_type(labels=labels, default=default_server_type)
     server_location = get_server_location(labels=labels, default=default_location)
     server_image = get_server_image(client=client, labels=labels, default=default_image)
     startup_script = get_startup_script(server_type=server_type, scripts=scripts)
 
     server_labels = {
         f"github-runner-label-{i}": value for i, value in enumerate(labels)
@@ -257,20 +260,19 @@
             count += 1
 
     return count
 
 
 def scale_up(
     terminate: threading.Event,
-    repo: Repository,
-    client: Client,
     scripts: Scripts,
     worker_pool: ThreadPoolExecutor,
     github_token: str,
     github_repository: str,
+    hetzner_token: str,
     ssh_key: SSHKey,
     default_server_type: ServerType,
     default_location: Location,
     default_image: Image,
     interval: int,
     max_servers: int,
     max_server_ready_time: int,
@@ -292,16 +294,16 @@
                 with Action(
                     f"Maximum number of servers {max_servers} has been reached"
                 ):
                     raise StopIteration("maximum number of servers reached")
 
         future = worker_pool.submit(
             create_server,
+            hetzner_token=hetzner_token,
             setup_worker_pool=setup_worker_pool,
-            client=client,
             labels=labels,
             name=name,
             default_server_type=default_server_type,
             default_location=default_location,
             default_image=default_image,
             scripts=scripts,
             github_token=github_token,
@@ -310,26 +312,37 @@
             timeout=max_server_ready_time,
         )
         future.server_name = name
 
         futures.append(future)
         servers.append(RunnerServer(name=name, labels=labels))
 
+    with Action("Logging in to Hetzner Cloud"):
+        client = Client(token=hetzner_token)
+
+    with Action("Logging in to GitHub"):
+        github = Github(login_or_token=github_token, per_page=100)
+
+    with Action(f"Getting repository {github_repository}"):
+        repo: Repository = github.get_repo(github_repository)
+
     with ThreadPoolExecutor(
         max_workers=worker_pool._max_workers, thread_name_prefix=f"setup-worker"
     ) as setup_worker_pool:
 
         while True:
             if terminate.is_set():
                 with Action("Terminating scale up service"):
                     break
 
             try:
                 with Action("Getting workflow runs", level=logging.DEBUG):
-                    workflow_runs = repo.get_workflow_runs(status="queued")
+                    workflow_runs: list[WorkflowRun] = repo.get_workflow_runs(
+                        status="queued"
+                    )
 
                 futures: list[Future] = []
 
                 with Action("Getting list of servers", level=logging.DEBUG):
                     servers = [
                         RunnerServer(
                             name=server.name,
```

### Comparing `testflows.github.runners-1.3.230731.1223752/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.3.230801.1034814/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1223752/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.3.230801.1034814/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1223752/testflows/github/runners/scripts/deploy/setup.sh` & `testflows.github.runners-1.3.230801.1034814/testflows/github/runners/scripts/deploy/setup.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1223752/testflows/github/runners/scripts/setup_docker.sh` & `testflows.github.runners-1.3.230801.1034814/testflows/github/runners/scripts/setup_docker.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1223752/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.3.230801.1034814/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1223752/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.3.230801.1034814/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1223752/testflows/github/runners/server.py` & `testflows.github.runners-1.3.230801.1034814/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1223752/testflows/github/runners/service.py` & `testflows.github.runners-1.3.230801.1034814/testflows/github/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1223752/testflows/github/runners/shell.py` & `testflows.github.runners-1.3.230801.1034814/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1223752/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.3.230801.1034814/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: testflows.github.runners
-Version: 1.3.230731.1223752
-Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
-Home-page: https://github.com/testflows/github-runners
-Author: Vitaliy Zakaznikov
-Author-email: vzakaznikov@testflows.com
-License: Apache-2.0
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-Provides-Extra: dev
-License-File: LICENSE
-
 .. image:: https://raw.githubusercontent.com/testflows/TestFlows-ArtWork/master/images/logo.png
    :width: 300px
    :align: center
    :target: https://testflows.com
    :alt: TestFlows Open-source Testing Framework
 
 ----
@@ -230,18 +213,19 @@
 
 The repository name will have the following format:
 
 ::
 
    <username>/demo-testflows-github-runners
 
-:For me, my GitHub repository is:
-   ::
+For me, my GitHub repository is:
+
+::
 
-      vzakaznikov/demo-testflows-github-runners
+   vzakaznikov/demo-testflows-github-runners
 
 ❷ Now, create an example GitHub Actions workflow as described in the `Quickstart for GitHub Actions <https://docs.github.com/en/actions/quickstart>`_ article.
 Note that we need to modify the example YAML configuration and specify that our job will run on a runner with the **self-hosted** and the **type-cpx21**
 labels.
 
 .. code-block:: yaml
 
@@ -272,18 +256,19 @@
               run: |
                 ls ${{ github.workspace }}
             - run: echo "🍏 This job's status is ${{ job.status }}."
 
 
 ❸ Finally, you will need to create a GitHub API token with the **workflow** privileges. Make sure to save the token!
 
-:For me, my *demo* GitHub token is:
-   ::
+For me, my *demo* GitHub token is:
 
-      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
+::
+
+   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
 
 You should now have your GitHub repository ready.
 
 See these steps in action:
 
 .. image:: https://raw.githubusercontent.com/testflows/TestFlows-GitHub-Runners/master/docs/images/github_create_repo_and_token.gif
    :align: center
@@ -296,18 +281,19 @@
 
 Next you will need to create a Hetzner Cloud project and an API token that we can use to create an manage Hetzner Cloud server instances.
 
 ❶ Create new Hetzner Cloud project **Demo GitHub Runners**.
 
 ❷ Now, create an API token and save it.
 
-:For me, the Hetzner Cloud token for my *Demo GitHub Runners* project is:
-   ::
-
-      5Up04IHuY8mC7l0JxKwh3Aps4ghGIyL0NJ9rGlhyAmmkddzuRreR1YstTSTFCG0N
+For me, the Hetzner Cloud token for my *Demo GitHub Runners* project is:
+   
+::
+   
+   5Up04IHuY8mC7l0JxKwh3Aps4ghGIyL0NJ9rGlhyAmmkddzuRreR1YstTSTFCG0N
 
 You should now have your Hetzner Cloud project ready.
 
 See these steps in action:
 
 .. image:: https://raw.githubusercontent.com/testflows/TestFlows-GitHub-Runners/master/docs/images/hetzner_create_project_and_token.gif
    :align: center
@@ -337,15 +323,15 @@
 
 You should now have the cloud service up and running.
 
 See these steps in action:
 
 .. image:: https://raw.githubusercontent.com/testflows/TestFlows-GitHub-Runners/master/docs/images/cloud_deploy.gif
    :align: center
-   :width: 790px
+   :width: 625px
    :alt: Deploying Cloud Service
 
 ------------------------------------------
 Waiting for GitHub Actions Job to Complete
 ------------------------------------------
 
 ❶ The **github-runners** cloud service is now running. So, now you can just seat back and wait until **github-runners**
```

### Comparing `testflows.github.runners-1.3.230731.1223752/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.3.230801.1034814/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 testflows.github.runners.egg-info/SOURCES.txt
 testflows.github.runners.egg-info/dependency_links.txt
 testflows.github.runners.egg-info/not-zip-safe
 testflows.github.runners.egg-info/requires.txt
 testflows.github.runners.egg-info/top_level.txt
 testflows/github/runners/__init__.py
 testflows/github/runners/actions.py
+testflows/github/runners/api_watch.py
 testflows/github/runners/args.py
 testflows/github/runners/cloud.py
 testflows/github/runners/config.py
 testflows/github/runners/delete.py
 testflows/github/runners/logger.py
 testflows/github/runners/request.py
 testflows/github/runners/scale_down.py
```

