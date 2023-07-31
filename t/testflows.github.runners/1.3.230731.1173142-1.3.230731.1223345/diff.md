# Comparing `tmp/testflows.github.runners-1.3.230731.1173142.tar.gz` & `tmp/testflows.github.runners-1.3.230731.1223345.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.3.230731.1173142.tar", last modified: Mon Jul 31 17:31:42 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.3.230731.1223345.tar", last modified: Mon Jul 31 22:33:45 2023, max compression
```

## Comparing `testflows.github.runners-1.3.230731.1173142.tar` & `testflows.github.runners-1.3.230731.1223345.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 17:31:42.332390 testflows.github.runners-1.3.230731.1173142/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1173142/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    49039 2023-07-31 17:31:42.332390 testflows.github.runners-1.3.230731.1173142/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    48447 2023-07-31 15:49:25.000000 testflows.github.runners-1.3.230731.1173142/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-31 17:31:42.332390 testflows.github.runners-1.3.230731.1173142/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-31 17:31:42.000000 testflows.github.runners-1.3.230731.1173142/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 17:31:42.328390 testflows.github.runners-1.3.230731.1173142/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 17:31:42.328390 testflows.github.runners-1.3.230731.1173142/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 17:31:42.332390 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-31 17:31:42.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1615 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     2599 2023-07-31 15:05:55.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 17:31:42.332390 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    23381 2023-07-31 15:15:18.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)    13607 2023-07-29 23:57:40.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     4164 2023-07-31 15:16:54.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/config.py
--rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/delete.py
--rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/logger.py
--rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)    10814 2023-07-29 23:14:39.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    16903 2023-07-31 15:02:38.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 17:31:42.332390 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 17:31:42.332390 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scripts/setup_docker.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     5158 2023-07-31 17:30:38.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 17:31:42.332390 testflows.github.runners-1.3.230731.1173142/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    49039 2023-07-31 17:31:42.000000 testflows.github.runners-1.3.230731.1173142/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1154 2023-07-31 17:31:42.000000 testflows.github.runners-1.3.230731.1173142/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-31 17:31:42.000000 testflows.github.runners-1.3.230731.1173142/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.3.230731.1173142/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-31 17:31:42.000000 testflows.github.runners-1.3.230731.1173142/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-31 17:31:42.000000 testflows.github.runners-1.3.230731.1173142/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 22:33:45.440139 testflows.github.runners-1.3.230731.1223345/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1223345/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    57136 2023-07-31 22:33:45.440139 testflows.github.runners-1.3.230731.1223345/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    56544 2023-07-31 22:33:14.000000 testflows.github.runners-1.3.230731.1223345/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-31 22:33:45.440139 testflows.github.runners-1.3.230731.1223345/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-31 22:33:45.000000 testflows.github.runners-1.3.230731.1223345/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 22:33:45.436138 testflows.github.runners-1.3.230731.1223345/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 22:33:45.436138 testflows.github.runners-1.3.230731.1223345/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 22:33:45.436138 testflows.github.runners-1.3.230731.1223345/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-31 22:33:45.000000 testflows.github.runners-1.3.230731.1223345/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1615 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1223345/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2599 2023-07-31 15:05:55.000000 testflows.github.runners-1.3.230731.1223345/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 22:33:45.436138 testflows.github.runners-1.3.230731.1223345/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    23381 2023-07-31 15:15:18.000000 testflows.github.runners-1.3.230731.1223345/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)    13607 2023-07-29 23:57:40.000000 testflows.github.runners-1.3.230731.1223345/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4164 2023-07-31 15:16:54.000000 testflows.github.runners-1.3.230731.1223345/testflows/github/runners/config.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.3.230731.1223345/testflows/github/runners/delete.py
+-rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1223345/testflows/github/runners/logger.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.3.230731.1223345/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10814 2023-07-29 23:14:39.000000 testflows.github.runners-1.3.230731.1223345/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16903 2023-07-31 15:02:38.000000 testflows.github.runners-1.3.230731.1223345/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 22:33:45.436138 testflows.github.runners-1.3.230731.1223345/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1223345/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 22:33:45.436138 testflows.github.runners-1.3.230731.1223345/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1223345/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1223345/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.3.230731.1223345/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.3.230731.1223345/testflows/github/runners/scripts/setup_docker.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1223345/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1223345/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1223345/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5158 2023-07-31 17:30:38.000000 testflows.github.runners-1.3.230731.1223345/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1223345/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 22:33:45.436138 testflows.github.runners-1.3.230731.1223345/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    57136 2023-07-31 22:33:45.000000 testflows.github.runners-1.3.230731.1223345/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1154 2023-07-31 22:33:45.000000 testflows.github.runners-1.3.230731.1223345/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-31 22:33:45.000000 testflows.github.runners-1.3.230731.1223345/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.3.230731.1223345/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-31 22:33:45.000000 testflows.github.runners-1.3.230731.1223345/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-31 22:33:45.000000 testflows.github.runners-1.3.230731.1223345/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.3.230731.1173142/LICENSE` & `testflows.github.runners-1.3.230731.1223345/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1173142/PKG-INFO` & `testflows.github.runners-1.3.230731.1223345/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.3.230731.1173142
+Version: 1.3.230731.1223345
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -30,22 +30,26 @@
 
 ======================================================
 Autoscaling GitHub Actions Runners Using Hetzner Cloud
 ======================================================
 
 A simple alternative to Github's `Recommended autoscaling solutions <https://docs.github.com/en/actions/hosting-your-own-runners/managing-self-hosted-runners/autoscaling-with-self-hosted-runners#recommended-autoscaling-solutions>`_.
 
+:🔍 Tip:
+   You can easily navigate this documentation page by clicking on any title to jump to the `Table of Contents`_.
+   Try it out, and remember, if you get lost just click any title!
+
 The **github-runners** service program starts and monitors queued up jobs for GitHub Actions workflows.
 When a new job is queued up, it creates a new Hetzner Cloud server instance
 that provides an ephemeral GitHub Actions runner. Each server instance is automatically
 powered off when job completes and then powered off servers are
 automatically deleted. Both **x64** (*x86*) and **arm64** (*arm*) runners are supported.
 See `Features`_ and `Limitations`_ for more details.
 
-.. image:: https://raw.githubusercontent.com/testflows/TestFlows-GitHub-Runners/master/intro.gif
+.. image:: https://raw.githubusercontent.com/testflows/TestFlows-GitHub-Runners/master/docs/images/intro.gif
    :align: center
    :alt: TestFlows GitHub Runners
 
 
 :❗Warning:
    This program is provided on "AS IS" basis without warranties or conditions of any kind. See LICENSE.
    Use it at your own risk. Manual monitoring is required to make sure server instances are cleaned up properly
@@ -55,86 +59,95 @@
 to avoid any cleanup. Server instances are not shared between any jobs.
 
 :✋ Note:
    Currently Hetzner Cloud server instances are billed on hourly basis. So a job that takes 1 min will be billed
    the same way as for a job that takes 59 minutes. Therefore, the minimal cost
    for any job is the cost of the server for 1 hour plus the cost for one public IPv4 address.
 
-----
-
-:🔍 Tip:
-   You can easily navigate this documentation page by clicking on any title to jump to the `Table of Contents`_.
-   Try it out, and remember, if you get lost just click any title!
-
-----
-
---------
+========
 Features
---------
+========
 
 * cost efficient on-demand runners using `Hetzner Cloud <https://www.hetzner.com/cloud>`_
 * simple configuration, no Webhooks, no need for AWS lambdas, and no need to setup any GitHub application
 * supports specifying custom runner server types, images, and locations using job labels
 * self-contained program that you can use to deploy, redeploy, and manage the service on a cloud instance
 * supports x64 (x86) and ARM64 (arm) runners
 * supports using any Hetzner Cloud server types
 * supports runners with pre-installed Docker
 * supports using any standard Hetzner Cloud images and applications
 * supports auto-replenishable fixed standby runner pools for jobs to be picked up immediately
 * simpler alternative to what GitHub lists in `Recommended autoscaling solutions <https://docs.github.com/en/actions/hosting-your-own-runners/managing-self-hosted-runners/autoscaling-with-self-hosted-runners#recommended-autoscaling-solutions>`_
 
-----
-
------------
+===========
 Limitations
------------
+===========
 
-* **Group runners are not supported**
+**Group runners are not supported**
+  ✎ However, you can run individual services for each repository using different Hetzner Cloud projects.
 
-     However, you can run individual services for each repository using different Hetzner Cloud projects.
+**Unique Hetzner Cloud project must be used for each repository**
+   ✎ However, unique projects allow to easily keep track of runner costs per repository.
 
-* **Unique Hetzner Cloud project must be used for each repository**
-
-     However, unique projects allow to easily keep track of runner costs per repository.
-
-----
-
--------------
+=============
 Prerequisites
--------------
+=============
 
 * Python >= 3.7
 * `Hetzner Cloud <https://www.hetzner.com/cloud>`_ account
 * GitHub API token with admin privileges to manage self-hosted runners
 
-----
-
-------------
+============
 Installation
-------------
+============
 
 .. code-block:: bash
 
    pip3 install testflows.github.runners
 
-----
+Check that the **github-runners** utility was installed correctly by executing the **github-runners -v** command.
+
+.. code-block:: bash
+
+   github-runners -v
+
+The **github-runners** utility is installed in to the *~/.local/bin/* folder. Please make sure that this folder
+is part of the **PATH**.
+
+.. code-block:: bash
+
+   which github-runners
+
+::
+
+   ~/.local/bin/github-runners
+
+If your **PATH** is missing this folder, on Ubuntu, modify your *~/.profile* and add the following section:
+
+:~/.profile:
+   .. code-block:: bash
+
+      # set PATH so it includes user's private bin if it exists
+      if [ -d "$HOME/.local/bin" ] ; then
+          PATH="$HOME/.local/bin:$PATH"
+      fi
 
-------------
+===========
 Quick Start
-------------
+===========
 
-Set environment variables corresponding to your GitHub repository and Hetzner Cloud project
+Set environment variables corresponding to your GitHub repository and Hetzner Cloud project.
 
 .. code-block:: bash
 
    export GITHUB_TOKEN=ghp_...
    export GITHUB_REPOSITORY=vzakaznikov/github-runners
    export HETZNER_TOKEN=GJzdc...
 
-and then start **github-runners** program
+Then, start the **github-runners** program:
 
 .. code-block:: bash
 
    github-runners
 
 ::
 
@@ -142,68 +155,261 @@
    07/22/2023 08:20:37 PM   INFO MainThread            main 🍀 Logging in to GitHub
    07/22/2023 08:20:37 PM   INFO MainThread            main 🍀 Getting repository vzakaznikov/github-runners
    07/22/2023 08:20:37 PM   INFO MainThread            main 🍀 Creating scale up service
    07/22/2023 08:20:37 PM   INFO MainThread            main 🍀 Creating scale down service
    07/22/2023 08:20:38 PM   INFO   worker_2   create_server 🍀 Create server
    ...
 
-or you can pass the required options inline as follows:
+Alternatively, you can pass the required options using the command line as follows:
 
 .. code-block:: bash
 
    github-runners --github-token <GITHUB_TOKEN> --github-repository <GITHUB_REPOSITORY> --hetzner-token <HETZNER_TOKEN>
 
-----
+========================
+Getting Started Tutorial
+========================
 
--------------------------
+:✅ Launch your first self-hosted runner in:
+   5 minutes
+
+This tutorial will guide you on how to use the **github-runners** program to provide autoscaling GitHub Actions runners
+for a GitHub repository and a Hetzner Cloud project that you'll create.
+
+-----------------------------------
+Installing TestFlows Github Runners
+-----------------------------------
+
+❶ Before we get started, you will need to install **testflows.github.runners** Python package. See the `Installation`_ section for more details.
+
+.. code-block:: bash
+
+  pip3 install testflows.github.runners
+
+❷ Check that the **github-runners** utility was installed correctly by executing the **github-runners -v** command.
+
+.. code-block:: bash
+
+   github-runners -v
+
+::
+
+   1.3.230731.1173142
+
+:✋ Note:
+   The **github-runners** utility is installed in to the *~/.local/bin/* folder. Please make sure that this folder
+   is part of the **PATH**.
+
+   .. code-block:: bash
+
+      which github-runners
+
+   ::
+
+      ~/.local/bin/github-runners
+
+   If your **PATH** is missing this folder, on Ubuntu, you can modify your *~/.profile* and add the following section:
+
+   :~/.profile:
+      .. code-block:: bash
+
+         # set PATH so it includes user's private bin if it exists
+         if [ -d "$HOME/.local/bin" ] ; then
+             PATH="$HOME/.local/bin:$PATH"
+         fi
+
+In order to launch the **github-runners** program, we'll need to specify GitHub repository as well as GitHub and
+Hetzner Cloud tokens. So, let's create these.
+
+----------------------------------------------------------
+Creating GitHub Repository with Actions Workflow and Token
+----------------------------------------------------------
+
+Before using the **github-runners**, you need a GitHub repository with a GitHub Actions workflow set up.
+
+❶ First, create GitHub Repository named **demo-testflows-github-runners** and note the repository name.
+
+The repository name will have the following format:
+
+::
+
+   <username>/demo-testflows-github-runners
+
+:For me, my GitHub repository is:
+   ::
+
+      vzakaznikov/demo-testflows-github-runners
+
+❷ Now, create an example GitHub Actions workflow as described in the `Quickstart for GitHub Actions <https://docs.github.com/en/actions/quickstart>`_ article.
+Note that we need to modify the example YAML configuration and specify that our job will run on a runner with the **self-hosted** and the **type-cpx21**
+labels.
+
+.. code-block:: yaml
+
+     Explore-GitHub-Actions:
+       runs-on: [self-hosted, type-cpx21]
+
+So, the complete *demo.yml* that uses self-hosted runner is as follows:
+
+:demo.yml:
+
+   .. code-block:: yaml
+
+      name: GitHub Actions Demo
+      run-name: ${{ github.actor }} is testing out GitHub Actions 🚀
+      on: [push]
+      jobs:
+        Explore-GitHub-Actions:
+          runs-on: [self-hosted, type-cpx21]
+          steps:
+            - run: echo "🎉 The job was automatically triggered by a ${{ github.event_name }} event."
+            - run: echo "🐧 This job is now running on a ${{ runner.os }} server hosted by GitHub!"
+            - run: echo "🔎 The name of your branch is ${{ github.ref }} and your repository is ${{ github.repository }}."
+            - name: Check out repository code
+              uses: actions/checkout@v3
+            - run: echo "💡 The ${{ github.repository }} repository has been cloned to the runner."
+            - run: echo "🖥️ The workflow is now ready to test your code on the runner."
+            - name: List files in the repository
+              run: |
+                ls ${{ github.workspace }}
+            - run: echo "🍏 This job's status is ${{ job.status }}."
+
+
+❸ Finally, you will need to create a GitHub API token with the **workflow** privileges. Make sure to save the token!
+
+:For me, my *demo* GitHub token is:
+   ::
+
+      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
+
+You should now have your GitHub repository ready.
+
+See these steps in action:
+
+.. image:: https://raw.githubusercontent.com/testflows/TestFlows-GitHub-Runners/master/docs/images/github_create_repo_and_token.gif
+   :align: center
+   :alt: Creating GitHub Repository and Token
+
+----------------------------------------
+Creating Hetzner Cloud Project and Token
+----------------------------------------
+
+Next you will need to create a Hetzner Cloud project and an API token that we can use to create an manage Hetzner Cloud server instances.
+
+❶ Create new Hetzner Cloud project **Demo GitHub Runners**.
+
+❷ Now, create an API token and save it.
+
+:For me, the Hetzner Cloud token for my *Demo GitHub Runners* project is:
+   ::
+
+      5Up04IHuY8mC7l0JxKwh3Aps4ghGIyL0NJ9rGlhyAmmkddzuRreR1YstTSTFCG0N
+
+You should now have your Hetzner Cloud project ready.
+
+See these steps in action:
+
+.. image:: https://raw.githubusercontent.com/testflows/TestFlows-GitHub-Runners/master/docs/images/hetzner_create_project_and_token.gif
+   :align: center
+   :alt: Creating GitHub Repository and Token
+
+----------------------
+Creating Cloud Service
+----------------------
+
+With the GitHub repository and GitHub and Hetzner Cloud tokens in hand, we can deploy the **github-runners** service
+to Hetzner Cloud instance. This way the service is not running on your local machine.
+
+The deployment we'll create a **github-runners** instance in your Hetzner Cloud project on which the service will be running.
+See the `Running as a Cloud Service`_ section for details.
+
+❶ To deploy the service run the **github-runners cloud deploy** command and specify your
+GitHub repository, GitHub and Hetzner Cloud tokens using
+**GITHUB_REPOSITORY**, **GITHUB_TOKEN**, and **HETZNER_TOKEN** environment variables.
+
+.. code-block:: bash
+
+   export GITHUB_REPOSITORY=
+   export HETZNER_TOKEN=
+   export GITHUB_TOKEN=
+   github-runners cloud deploy
+
+You should now have the cloud service up and running.
+
+See these steps in action:
+
+.. image:: https://raw.githubusercontent.com/testflows/TestFlows-GitHub-Runners/master/docs/images/cloud_deploy.gif
+   :align: center
+   :alt: Deploying Cloud Service
+
+------------------------------------------
+Waiting for GitHub Actions Job to Complete
+------------------------------------------
+
+❶ The **github-runners** cloud service is now running. So, now you can just seat back and wait until **github-runners**
+spins up a new runner to complete any queued up GitHub Actions jobs in your GitHub repository.
+
+See this step in action:
+
+.. image:: https://raw.githubusercontent.com/testflows/TestFlows-GitHub-Runners/master/docs/images/github_job_completed.gif
+   :align: center
+   :alt: Waiting For GitHub Actions Job to Complete
+
+As you can see our job was executed and completed using our own self-hosted runner!
+
+:✋ Note:
+
+   If you run into any issues you can check cloud service logs using the
+   **github-runners cloud logs -f** command. For other cloud service commands see the `Running as a Cloud Service`_ section.
+
+   .. code-block:: bash
+
+      github-runners cloud logs -f
+
+=========================
 Installation From Sources
--------------------------
+=========================
 
 For development, you can install from sources as follows:
 
 .. code-block:: bash
 
    git clone https://github.com/testflows/Github-Runners.git
    ./package && ./install
 
-----
-
--------------------
+===================
 Basic Configuration
--------------------
+===================
 
 By default, the program uses the following environment variables:
 
 * **GITHUB_TOKEN**
 * **GITHUB_REPOSITORY**
 * **HETZNER_TOKEN**
 
 or you can specify these values using the following options:
 
 * **--github-token**
 * **--github-repository**
 * **--hetzner-token**
 
-----
-
-------------------------------------
+====================================
 Specifying Maximum Number of Runners
-------------------------------------
+====================================
+
 The default maximum number of runners is **10**. You can set a different value
 based on your Hetzner Cloud limits using the **-m count, --max-runners count** option. For example,
 
 .. code-block:: bash
 
    github-runners --max-runners 40
 
-----
-
--------------------------------
+===============================
 Jobs That Require Docker Engine
--------------------------------
+===============================
 
 For jobs that require Docker to be installed, you can use the standard `Hetzner Docker CE application <https://docs.hetzner.com/cloud/apps/list/docker-ce/>`_
 which can be specified using the **image-** label. See `Specifying Runner Image`_ for more details about specifying custom runner images.
 
 For example
 
 :x64:
@@ -216,22 +422,21 @@
 :ARM64:
 
    .. code-block:: yaml
 
       job-name:
          runs-on: [self-hosted, type-cax11, image-arm-app-docker-ce]
 
-----
-
-----------------------
+======================
 Specifying Runner Type
-----------------------
+======================
 
+-----------
 x64 Runners
-============
+-----------
 
 The default server type is **cx11** which is an Intel, 1 vCPU, 2GB RAM shared-cpu x64 instance.
 
 :✋ Note:
    You can use **--default-type** option to set a different default server type.
 
 You can specify different x64 server instance type by using the **type-{name}** runner label.
@@ -242,16 +447,17 @@
 as follows:
 
 .. code-block:: yaml
 
    job-name:
       runs-on: [self-hosted, type-cpx21]
 
+-------------
 ARM64 Runners
-==============
+-------------
 
 The default, the server type is **cx11**, which is an Intel, 1 vCPU, 2GB RAM shared-cpu x64 instance.
 Therefore, in order to use ARM64 runners you must specify ARM64 server instance type by using the **type-{name}** runner label.
 The **{name}** must be a valid `ARM64 Hetzner Cloud server type <https://www.hetzner.com/cloud>`_
 name such as *cax11*, *cax21* etc. which correspond to the Ampere Altra, 2 vCPU, 4GB RAM and
 4 vCPU, 8GB RAM shared-cpu ARM64 instances respectively.
 
@@ -259,19 +465,17 @@
 as follows:
 
 .. code-block:: yaml
 
    job-name:
       runs-on: [self-hosted, type-cax21]
 
-----
-
----------------------------
+==========================
 Specifying Runner Location
----------------------------
+==========================
 
 By default, the default location of the server where the runner will be running is not specified. You can use the **--default-location**
 option to force specific default server location.
 
 You can also use the **in-{name}** runner label to specify server location for a specific job. Where **{name}** must be a valid
 `Hetzner Cloud location <https://docs.hetzner.com/cloud/general/locations/>`_ name such as *ash* for US, Ashburn, VA or
 *fsn1* for Germany, Falkenstein.
@@ -279,19 +483,17 @@
 For example,
 
 .. code-block:: yaml
 
    job-name:
       runs-on: [self-hosted, type-cx11, in-ash]
 
-----
-
------------------------
+=======================
 Specifying Runner Image
------------------------
+=======================
 
 By default, the default image of the server for the runner is **ubuntu-22.04**. You can use the **--default-image**
 option to force specific default server image.
 
 You can also use the **image-{architecture}-{type}-{name}** runner label to specify server image for a specific job.
 
 Where,
@@ -323,19 +525,17 @@
    must be unique.
 
    .. code-block:: yaml
 
       job-name:
          runs-on: [self-hosted, type-cx11, in-ash, image-x86-snapshot-snapshot_description]
 
-----
-
---------------------------------------------
+============================================
 Specifying Custom Runner Server Setup Script
---------------------------------------------
+============================================
 
 You can specify custom runner server setup script using the **--setup-script** option.
 
 For example,
 
 :custom_setup.sh:
    .. code-block:: bash
@@ -355,19 +555,17 @@
       apt-get -y install ca-certificates curl gnupg lsb-release python3-pip git unzip
 
 :command:
    .. code-block:: bash
 
       github-runners --setup-script ./custom_setup.sh
 
-----
-
---------------------------
+==========================
 Specifying Standby Runners
---------------------------
+==========================
 
 You can define standby runner groups to be always ready to pick your jobs using a custom configuration file.
 
 :✋ Note:
    Standby runner groups can only be defined using a configuration file.
    See `Using Configuration File`_ for more details.
 
@@ -401,19 +599,17 @@
                   labels=["type-cx21"],
                   count=2,
                   replenish_immediately=True,
             )
          ],
       )
 
-----
-
--------------------------------
+===============================
 Specifying Logger Configuration
--------------------------------
+===============================
 
 You can specify custom logger configuration using a configuration file.
 
 :✋ Note:
    Custom logger configuration can only be specified using a configuration file.
    See `Using Configuration File`_ for more details.
 
@@ -447,19 +643,17 @@
              },
              "loggers": {
                  "testflows.github.runners": {"level": "INFO", "handlers": ["default"]},
              },
          }
      )
 
-----
-
---------------------------------------
+======================================
 Deleting All Runners And Their Servers
---------------------------------------
+======================================
 
 You can delete all runners, including standby runners, and their servers using the **delete** command.
 
 :✋ Note:
    The **delete** command will not delete cloud service server. If you also want to delete it,
    you also need to execute **cloud delete** command. For more information, see `Deleting Cloud Service`_ section.
 
@@ -471,19 +665,17 @@
 
    07/29/2023 07:43:16 PM     INFO       MainThread             all 🍀 Logging in to Hetzner Cloud
    07/29/2023 07:43:16 PM     INFO       MainThread             all 🍀 Logging in to GitHub
    07/29/2023 07:43:16 PM     INFO       MainThread             all 🍀 Getting repository testflows/testflows-github-runners
    07/29/2023 07:43:17 PM     INFO       MainThread             all 🍀 Getting list of self-hosted runners
    07/29/2023 07:43:17 PM     INFO       MainThread             all 🍀 Getting list of servers
 
-----
-
-------------------------
+========================
 Using Configuration File
-------------------------
+========================
 
 Instead of passing configuration options using command line arguments, you can use
 configuration file. The configuration file is Python file that must define the **config**
 object of the `Config class`_.
 
 :✋ Note:
    When you mix command line options and custom configuration file,
@@ -528,16 +720,17 @@
 
 You can pass your custom configuration file using the **-c path, --config path** command line option.
 
 .. code-block:: bash
 
    github-runners -c config.py
 
+--------------------
 Configuration Schema
-=====================
+--------------------
 
 The `Config class`_ has the following schema:
 
 :schema:
    * **github_token: str**
    * **github_repository: str**
    * **hetzner_token: str**
@@ -566,59 +759,56 @@
          * **location: location**
          * **setup_script: path**
    * **standby_runners: list[standby_runner]**
       * **labels: list[str]**
       * **count: count**
       * **replenish_immediately: bool**
 
-----
-
--------
-SSH Key
--------
+==================
+Specifying SSH Key
+==================
 
 All server instances that are created are accessed via SSH using the **ssh** utility and therefore you must provide a valid SSH key
 using the **--ssh-key** option. If the **--ssh-key** option is no specified, then the *~/.ssh/id_rsa.pub* default key path will be used.
 
 The SSH key will be automatically added to your project using the MD5 hash of the public key as the SSH key name.
 
 :❗Warning:
    Given that each new SSH key is automatically added to your Hetzner project, you must manually delete them when no longer needed.
 
 Most GitHub users already have an SSH key associated with the account. If you want to know how to add an SSH key, see `Adding a new SSH key to your GitHub account    <https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account>`_ article.
 
+----------------------
 Generating New SSH Key
-=======================
+----------------------
 
 If you need to generate a new SSH key, see `Generating a new SSH key and adding it to the ssh-agent <https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent>`_ article.
 
-Cloud Deployment
-================
+----------------------------
+SSH Keys in Cloud Deployment
+----------------------------
 
 If you are deploying the **github-runners** program as a cloud service using the **github-runners <options> cloud deploy** command, then
 after provisoning a new cloud server instance that will host the **github-runners** service, a new SSH key will be
 auto-generated to access the runners. The auto-generated key will be placed in */home/runner/.ssh/id_rsa*, where **runner**
 is the user under which the **github-runners** service runs on the cloud instance. The auto-generated SSH key will be automatically
 added to your project using the MD5 hash of the public key as the SSH key name.
 
-----
-
------------------------
+====================
 Running as a Service
------------------------
+====================
 
 You can run **github-runners** as a service.
 
 :✋ Note:
    In order to install the service, the user that installed the module must have **sudo** privileges.
 
-----
-
+---------------------------
 Installing and Uninstalling
-===========================
+---------------------------
 
 After installation, you can use **service install** and **service uninstall** commands to install and
 uninstall the service.
 
 :✋ Note:
    The options that are passed to the **github-runners <options> service install** command
    will be the same options with which the service will be executed.
@@ -652,34 +842,32 @@
       Environment=GITHUB_TOKEN=ghp_...
       Environment=GITHUB_REPOSITORY=testflows/github-runners
       Environment=HETZNER_TOKEN=GJ..
       ExecStart=/home/user/.local/lib/python3.10/site-packages/testflows/github/runners/bin/github-runners --workers 10 --max-powered-off-time 20 --max-unused-runner-time 120 --max-runner-registration-time 60 --scale-up-interval 10 --scale-down-interval 10
       [Install]
       WantedBy=multi-user.target
 
-----
-
+-------------------------
 Modifying Program Options
-=========================
+-------------------------
 
 If you want to modify service program options you can stop the service,
 edit the **/etc/systemd/system/github-runners.service** file by hand, then reload service daemon,
 and start the service back up.
 
 .. code-block:: bash
 
    github-runners service stop
    sudo vim /etc/systemd/system/github-runners.service
    sudo systemctl daemon-reload
    github-runners service start
 
-----
-
+---------------
 Checking Status
-================
+---------------
 
 After installation, you can check the status of the service using the **service status** command.
 
 .. code-block:: bash
 
    github-runners service status:
 
@@ -701,18 +889,17 @@
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Logging in to Hetzner >
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Logging in to GitHub
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Getting repository vza>
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Creating scale up serv>
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Creating scale down se>
       lines 1-16/16 (END)
 
-----
-
+---------------------
 Manual Start and Stop
-=====================
+---------------------
 
 You can start and stop the service using the **service start** and **service stop** commands as follows:
 
 .. code-block:: bash
 
    github-runners service start
    github-runners service stop
@@ -720,18 +907,17 @@
 or using **service** system utility
 
 .. code-block:: bash
 
    sudo service github-runners start
    sudo service github-runners stop
 
-----
-
+-------------
 Checking Logs
-=============
+-------------
 
 You can get the logs for the service using the **service logs** command.
 
 Use **-f, --follow** option to follow logs journal.
 
 .. code-block:: bash
 
@@ -774,19 +960,17 @@
       Jul 24 14:24:42 user-node env[62771]: LANGUAGE=en_CA:en
       Jul 24 14:24:42 user-node env[62771]: PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/snap/bin
       Jul 24 14:24:42 user-node env[62771]: INVOCATION_ID=dc7b778f95fa4ccf95e4a4592b50d9e1
       Jul 24 14:24:42 user-node env[62771]: JOURNAL_STREAM=8:328542
       Jul 24 14:24:42 user-node env[62771]: SYSTEMD_EXEC_PID=62771
       ...
 
-----
-
---------------------------
+==========================
 Running as a Cloud Service
---------------------------
+==========================
 
 Instead of running **github-runners** program locally as a standalone application or as a service.
 You can easily deploy **github-runners** to run on a Hetzner Cloud instance.
 
 See **-h, --help** for all the available commands.
 
 :✋ Note:
@@ -794,18 +978,17 @@
    is **github-runners**. If you want to use a custom server name, then
    you must use the **cloud --name** option for any **cloud** commands.
 
 .. code-block:: bash
 
    github-runners cloud -h
 
-----
-
-Deployment
-==========
+---------
+Deploying
+---------
 
 You can deploy **github-runners** as a service to a new Hetzner Cloud server instance, that will be created for you automatically,
 using the **cloud deploy** command.
 
 :✋ Note:
    The options that are passed to the **github-runners <options> cloud deploy** command
    will be the same options with which the service will be executed.
@@ -864,15 +1047,15 @@
 
    github-runners deploy --location nbg1 --type cx11 --image ubuntu-22.04
 
 The cloud instance that runs the **github-runners** service can either be x64 or ARM64 instance. By default, **cpx11**
 AMD, 2 vCPU, 2GB RAM, shared-cpu x64 instance type is used.
 
 Using ARM64 Instance
-++++++++++++++++++++
+====================
 
 If you want to deploy the **github-runners** service to an ARM64 instance, then you must specify the instance
 type using the **--type** option.
 
 :✋ Note:
    Currently Hetzner Cloud has ARM64 instances only available in Germany, Falkenstein (**fsn1**) location.
 
@@ -880,41 +1063,39 @@
 as the value of the **--type** as follows:
 
 .. code-block:: bash
 
    github-runners deploy --location fsn1 --type cax21 --image ubuntu-22.04
 
 Using x64 Instance
-++++++++++++++++++
+==================
 
 By default, the **cpx11** AMD, 2 vCPU, 2GB RAM, shared-cpu x64 instance type is used. If you want to use
 a different x64 instance then specify desired type using the **--type** option.
 
-----
-
+-------------------------
 Redeploying Cloud Service
-=========================
+-------------------------
 
 You can change cloud service configuration or cloud service package version without deleting the existing cloud service server
 using the **cloud redeploy** command.
 
 .. code-block:: bash
 
    github-runners <options> cloud redeploy
 
 :✋ Note:
    The options that are passed to the **github-runners <options> cloud redeploy** command
    will be the same options with which the service will be executed.
 
 You can specify the version of the package to be installed using the **--version** option.
 
-----
-
+------------------
 Cloud Service Logs
-===================
+------------------
 
 You can check logs for the **github-runners** service running on a cloud instance using the **github-runners cloud logs** command.
 Specify **-f, --follow** if you want to follow the logs journal.
 
 For example,
 
 :dump the full log:
@@ -925,54 +1106,50 @@
 
 :follow the logs journal:
 
    .. code-block:: bash
 
       github-runners cloud logs -f
 
-----
-
+--------------------
 Cloud Service Status
-=====================
+--------------------
 
 You can check the status of the **github-runners** service running on a cloud instance using the **github-runners cloud status** command.
 
 For example,
 
 .. code-block:: bash
 
    github-runners cloud status
 
-----
-
+----------------------
 Stopping Cloud Service
-======================
+----------------------
 
 You can manually stop the **github-runners** service running on a cloud instance using the **github-runners cloud stop** command.
 
 .. code-block:: bash
 
    github-runners cloud stop
 
-----
-
+----------------------
 Starting Cloud Service
-======================
+----------------------
 
 You can manually start the **github-runners** service running on a cloud instance after it was being manually stopped
 using the **github-runners cloud start** command.
 
 .. code-block:: bash
 
    github-runners cloud start
 
-----
-
+------------------------
 Installing Cloud Service
-========================
+------------------------
 
 You can manually force installation of the **github-runners** service running on a cloud instance using
 the **github-runners cloud install** command.
 
 :✋ Note:
    Just like with the `github-runners <options> service install` command,
    the options that are passed to the `github-runners <options> cloud install` command
@@ -980,30 +1157,28 @@
 
 You can specify **-f, --force** option to force service re-installation if it is already installed.
 
 .. code-block:: bash
 
    github-runners <options> cloud install -f
 
-----
-
+--------------------------
 Uninstalling Cloud Service
-==========================
+--------------------------
 
 You can manually force uninstallation of the **github-runners** service running on a cloud instance using
 the **github-runners cloud uninstall** command.
 
 .. code-block:: bash
 
    github-runners cloud uninstall
 
-----
-
+-------------------------------
 Upgrading Cloud Service Package
-===============================
+-------------------------------
 
 You can manually upgrade the **github-runners** service package running on a cloud instance using
 the **github-runners cloud upgrade** command.
 
 If specific '--version' is specified then the *testflows.github.runners* package is upgraded to
 the specified version otherwise the version is upgraded to the latest available.
 
@@ -1015,18 +1190,17 @@
 .. code-block:: bash
 
    github-runners cloud upgrade --version <version>
 
 The service is not re-installed during the package upgrade process.
 Instead, it is stopped before the upgrade and then started back up
 
-----
-
+------------------------------
 Changing Cloud Service Options
-==============================
+------------------------------
 
 If you need to change cloud service options such as the **--setup-script** or the **--max-runners** etc.,
 you can keep the existing server and use **cloud redeploy** command.
 
 .. code-block:: bash
 
    github-runners <options> cloud redeploy --version latest
@@ -1041,18 +1215,17 @@
    github-runners <options> cloud deploy --version latest
 
 :✋ Note:
    Complete teardown will not affect any current jobs as the service is designed to
    be restartable. However, some servers might be left in an unfinished state
    but they will be cleaned up when the service is restarted.
 
-----
-
+----------------------
 Deleting Cloud Service
-======================
+----------------------
 
 You can delete the **github-runners** cloud service and the cloud instance that is running on using
 the **github-runners cloud delete** command.
 
 The **cloud delete** command, deletes the cloud service by first stopping the service and then deleting the server instance.
 
 :❗Warning:
@@ -1067,18 +1240,17 @@
       github-runners cloud delete
 
 :custom name:
    .. code-block:: bash
 
       github-runners cloud --name <custom_name> delete
 
-----
-
+-----------------------
 SSH in to Cloud Service
-==============================
+-----------------------
 
 You can open SSH client to the cloud service using the **cloud ssh** command. For example,
 
 .. code-block:: bash
 
    github-runners cloud ssh
 
@@ -1091,19 +1263,17 @@
 
 The output will contain the full **ssh** command including the IP address of the cloud service server.
 
 ::
 
    ssh -q -o "StrictHostKeyChecking no" root@5.161.87.21
 
-----
-
-------------------
+==================
 Scaling Up Runners
-------------------
+==================
 
 The program scales up runners by looking for any jobs that have **queued** status.
 For each such job, a corresponding Hetzner Cloud server instance is created with the following name:
 
 ::
 
    github-runner-{job.id}
@@ -1120,30 +1290,28 @@
 Also,
 
 :Note:
    There is no guarantee that a given runner will pick the job with the exact **job.id** that caused it to be created.
    This is expected and because for each **queued** job a unique runner will be created the number of runners will be
    equal the number of jobs and therefore under normal conditions all jobs will be executed as expected.
 
-----
-
+-------------------------
 Maximum Number of Runners
-=========================
+-------------------------
 
 By default, the maximum number of runners and therefore the maximum number of server instances is not set and therefore is unlimited.
 You can set the maximum number of runners using the **--max-runners** option.
 
 .. code-blocks::bash
 
    github-runners --max-runners 10
 
-----
-
+----------
 New Server
-==========
+----------
 
 The new server is accessed using SSH. It boots up with the specified OS image and is configured using
 the **setup** and **startup** scripts.
 
 :Server Type:
 
    The default server type is **cx11** which is an Intel, 1 vCPU, 2GB RAM shared-cpu x64 instance.
@@ -1173,18 +1341,17 @@
 
    The server is configured to be accessed using *ssh* utility and the SSH public key path is specified using the **--ssh-key**
    option.
 
 :Image Configuration:
    Each new server instance is configured using the `setup <#the-setup-script>`_ and the `startup <#the-start-up-script>`_ scripts.
 
-----
-
+----------------
 The Setup Script
-================
+----------------
 
 The **setup** script creates and configures **runner** user that has **sudo** privileges.
 
 :Setup:
 
    .. code-block:: bash
 
@@ -1194,18 +1361,17 @@
 
         adduser ubuntu --disabled-password --gecos ""
         echo "%wheel   ALL=(ALL:ALL) NOPASSWD:ALL" >> /etc/sudoers
         addgroup wheel
         usermod -aG wheel ubuntu
         usermod -aG sudo ubuntu
 
-----
-
+-------------------
 The Start-up Script
-===================
+-------------------
 
 The **startup** script installs GitHub Actions runner. After installation it configures the runner to start in an *--ephemeral* mode.
 The *--ephemeral* mode causes the runner to exit as soon as it completes a job. After the runner exits the server is powered off.
 
 :✋ Note:
    The **startup** script is executed as **ubuntu** user and therefore you must use **sudo** for any commands that need *root* privileges.
 
@@ -1245,50 +1411,49 @@
 
      echo "Configure runner"
      ./config.sh --unattended --replace --url https://github.com/${GITHUB_REPOSITORY} --token ${GITHUB_RUNNER_TOKEN} --name "$(hostname)" --runnergroup "${GITHUB_RUNNER_GROUP}" --labels "${GITHUB_RUNNER_LABELS}" --work _work --ephemeral
 
      echo "Start runner"
      bash -c "screen -d -m bash -c './run.sh; sudo poweroff'"
 
-----
-
---------------------
+====================
 Scaling Down Runners
---------------------
+====================
 
+-------------------
 Powered Off Servers
-===================
+-------------------
 
 The program scales down runners by first cleaning up powered off servers. The scale down service relies on the fact
 that the `startup <#the-start-up-script>`_ script starts an ephemeral runner which will pick up only 1 job and then will power itself off after the job is complete.
 
 The powered off servers are deleted after the **max-powered-off-time** interval which
 can be specified using the **--max-powered-off-time** option which by default is set to *20* sec.
 
+--------------
 Unused Runners
-==============
+--------------
 
 The scale down service also monitors all the runners that have **unused** status and tries to delete any servers associated with such
 runners if the runner is **unused** for more than the **max-unused-runner-time** period. This is needed in case a runner never gets a job
 assigned to it and the server will stay in the power on state. This cycle relies on the fact that the runner's name
 is the same as server's name. The **max-unused-runner-time** can be specified using the **--max-unused-runner-time** option which by default
 is set to *120* sec.
 
+--------------
 Zombie Servers
-==============
+--------------
 
 The scale down service will delete any zombie servers. A zombie server is defined as as any server that fails to register its runner within
 the **max-runner-registration-time**. The **max-runner-registration-time** can be specified using the **--max-runner-registration-time** option
 which by default is set to *60* sec.
 
-----
-
----------------------------
+===========================
 Handling Failing Conditions
----------------------------
+===========================
 
 The program is designed to handle the following failing conditions:
 
 :Server Never Registers a Runner:
    The server will remain in **running** state and should be reclaimed by the scale down service when it checks the actual runners registered for current servers.
    If it finds a server that is **running** but no runner is active for it it will be deleted after the **max-runner-registration-time** period.
 
@@ -1303,19 +1468,17 @@
 
 :Runner Never Gets a Job Assigned:
    If the runner never gets a job assigned, then the scale down service will remove the runner and delete its server after the **max-unused-runner-time** period.
 
 :Runner Created With a Mismatched Labels:
    The behavior will be the same as for the **Runner Never Gets a Job Assigned** case above.
 
-----
-
----------------
+===============
 Program Options
----------------
+===============
 
 The following options are supported:
 
 * **-h, --help**
   show this help message and exit
 
 * **-v, --version**
@@ -1491,16 +1654,16 @@
 
       * **start**
         start service
 
       * **stop**
         stop service
 
------------------
+=================
 Table of Contents
------------------
+=================
 
-.. contents:: Index:
+.. contents::
    :backlinks: top
    :depth: 4
 
 .. _Config class: https://github.com/testflows/TestFlows-GitHub-Runners/blob/main/testflows/github/runners/config.py#L45
```

### Comparing `testflows.github.runners-1.3.230731.1173142/README.rst` & `testflows.github.runners-1.3.230731.1223345/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: testflows.github.runners
+Version: 1.3.230731.1223345
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
@@ -13,22 +30,26 @@
 
 ======================================================
 Autoscaling GitHub Actions Runners Using Hetzner Cloud
 ======================================================
 
 A simple alternative to Github's `Recommended autoscaling solutions <https://docs.github.com/en/actions/hosting-your-own-runners/managing-self-hosted-runners/autoscaling-with-self-hosted-runners#recommended-autoscaling-solutions>`_.
 
+:🔍 Tip:
+   You can easily navigate this documentation page by clicking on any title to jump to the `Table of Contents`_.
+   Try it out, and remember, if you get lost just click any title!
+
 The **github-runners** service program starts and monitors queued up jobs for GitHub Actions workflows.
 When a new job is queued up, it creates a new Hetzner Cloud server instance
 that provides an ephemeral GitHub Actions runner. Each server instance is automatically
 powered off when job completes and then powered off servers are
 automatically deleted. Both **x64** (*x86*) and **arm64** (*arm*) runners are supported.
 See `Features`_ and `Limitations`_ for more details.
 
-.. image:: https://raw.githubusercontent.com/testflows/TestFlows-GitHub-Runners/master/intro.gif
+.. image:: https://raw.githubusercontent.com/testflows/TestFlows-GitHub-Runners/master/docs/images/intro.gif
    :align: center
    :alt: TestFlows GitHub Runners
 
 
 :❗Warning:
    This program is provided on "AS IS" basis without warranties or conditions of any kind. See LICENSE.
    Use it at your own risk. Manual monitoring is required to make sure server instances are cleaned up properly
@@ -38,86 +59,95 @@
 to avoid any cleanup. Server instances are not shared between any jobs.
 
 :✋ Note:
    Currently Hetzner Cloud server instances are billed on hourly basis. So a job that takes 1 min will be billed
    the same way as for a job that takes 59 minutes. Therefore, the minimal cost
    for any job is the cost of the server for 1 hour plus the cost for one public IPv4 address.
 
-----
-
-:🔍 Tip:
-   You can easily navigate this documentation page by clicking on any title to jump to the `Table of Contents`_.
-   Try it out, and remember, if you get lost just click any title!
-
-----
-
---------
+========
 Features
---------
+========
 
 * cost efficient on-demand runners using `Hetzner Cloud <https://www.hetzner.com/cloud>`_
 * simple configuration, no Webhooks, no need for AWS lambdas, and no need to setup any GitHub application
 * supports specifying custom runner server types, images, and locations using job labels
 * self-contained program that you can use to deploy, redeploy, and manage the service on a cloud instance
 * supports x64 (x86) and ARM64 (arm) runners
 * supports using any Hetzner Cloud server types
 * supports runners with pre-installed Docker
 * supports using any standard Hetzner Cloud images and applications
 * supports auto-replenishable fixed standby runner pools for jobs to be picked up immediately
 * simpler alternative to what GitHub lists in `Recommended autoscaling solutions <https://docs.github.com/en/actions/hosting-your-own-runners/managing-self-hosted-runners/autoscaling-with-self-hosted-runners#recommended-autoscaling-solutions>`_
 
-----
-
------------
+===========
 Limitations
------------
-
-* **Group runners are not supported**
-
-     However, you can run individual services for each repository using different Hetzner Cloud projects.
+===========
 
-* **Unique Hetzner Cloud project must be used for each repository**
+**Group runners are not supported**
+  ✎ However, you can run individual services for each repository using different Hetzner Cloud projects.
 
-     However, unique projects allow to easily keep track of runner costs per repository.
-
-----
+**Unique Hetzner Cloud project must be used for each repository**
+   ✎ However, unique projects allow to easily keep track of runner costs per repository.
 
--------------
+=============
 Prerequisites
--------------
+=============
 
 * Python >= 3.7
 * `Hetzner Cloud <https://www.hetzner.com/cloud>`_ account
 * GitHub API token with admin privileges to manage self-hosted runners
 
-----
-
-------------
+============
 Installation
-------------
+============
 
 .. code-block:: bash
 
    pip3 install testflows.github.runners
 
-----
+Check that the **github-runners** utility was installed correctly by executing the **github-runners -v** command.
+
+.. code-block:: bash
+
+   github-runners -v
+
+The **github-runners** utility is installed in to the *~/.local/bin/* folder. Please make sure that this folder
+is part of the **PATH**.
+
+.. code-block:: bash
+
+   which github-runners
+
+::
+
+   ~/.local/bin/github-runners
+
+If your **PATH** is missing this folder, on Ubuntu, modify your *~/.profile* and add the following section:
 
-------------
+:~/.profile:
+   .. code-block:: bash
+
+      # set PATH so it includes user's private bin if it exists
+      if [ -d "$HOME/.local/bin" ] ; then
+          PATH="$HOME/.local/bin:$PATH"
+      fi
+
+===========
 Quick Start
-------------
+===========
 
-Set environment variables corresponding to your GitHub repository and Hetzner Cloud project
+Set environment variables corresponding to your GitHub repository and Hetzner Cloud project.
 
 .. code-block:: bash
 
    export GITHUB_TOKEN=ghp_...
    export GITHUB_REPOSITORY=vzakaznikov/github-runners
    export HETZNER_TOKEN=GJzdc...
 
-and then start **github-runners** program
+Then, start the **github-runners** program:
 
 .. code-block:: bash
 
    github-runners
 
 ::
 
@@ -125,68 +155,261 @@
    07/22/2023 08:20:37 PM   INFO MainThread            main 🍀 Logging in to GitHub
    07/22/2023 08:20:37 PM   INFO MainThread            main 🍀 Getting repository vzakaznikov/github-runners
    07/22/2023 08:20:37 PM   INFO MainThread            main 🍀 Creating scale up service
    07/22/2023 08:20:37 PM   INFO MainThread            main 🍀 Creating scale down service
    07/22/2023 08:20:38 PM   INFO   worker_2   create_server 🍀 Create server
    ...
 
-or you can pass the required options inline as follows:
+Alternatively, you can pass the required options using the command line as follows:
 
 .. code-block:: bash
 
    github-runners --github-token <GITHUB_TOKEN> --github-repository <GITHUB_REPOSITORY> --hetzner-token <HETZNER_TOKEN>
 
-----
+========================
+Getting Started Tutorial
+========================
 
--------------------------
+:✅ Launch your first self-hosted runner in:
+   5 minutes
+
+This tutorial will guide you on how to use the **github-runners** program to provide autoscaling GitHub Actions runners
+for a GitHub repository and a Hetzner Cloud project that you'll create.
+
+-----------------------------------
+Installing TestFlows Github Runners
+-----------------------------------
+
+❶ Before we get started, you will need to install **testflows.github.runners** Python package. See the `Installation`_ section for more details.
+
+.. code-block:: bash
+
+  pip3 install testflows.github.runners
+
+❷ Check that the **github-runners** utility was installed correctly by executing the **github-runners -v** command.
+
+.. code-block:: bash
+
+   github-runners -v
+
+::
+
+   1.3.230731.1173142
+
+:✋ Note:
+   The **github-runners** utility is installed in to the *~/.local/bin/* folder. Please make sure that this folder
+   is part of the **PATH**.
+
+   .. code-block:: bash
+
+      which github-runners
+
+   ::
+
+      ~/.local/bin/github-runners
+
+   If your **PATH** is missing this folder, on Ubuntu, you can modify your *~/.profile* and add the following section:
+
+   :~/.profile:
+      .. code-block:: bash
+
+         # set PATH so it includes user's private bin if it exists
+         if [ -d "$HOME/.local/bin" ] ; then
+             PATH="$HOME/.local/bin:$PATH"
+         fi
+
+In order to launch the **github-runners** program, we'll need to specify GitHub repository as well as GitHub and
+Hetzner Cloud tokens. So, let's create these.
+
+----------------------------------------------------------
+Creating GitHub Repository with Actions Workflow and Token
+----------------------------------------------------------
+
+Before using the **github-runners**, you need a GitHub repository with a GitHub Actions workflow set up.
+
+❶ First, create GitHub Repository named **demo-testflows-github-runners** and note the repository name.
+
+The repository name will have the following format:
+
+::
+
+   <username>/demo-testflows-github-runners
+
+:For me, my GitHub repository is:
+   ::
+
+      vzakaznikov/demo-testflows-github-runners
+
+❷ Now, create an example GitHub Actions workflow as described in the `Quickstart for GitHub Actions <https://docs.github.com/en/actions/quickstart>`_ article.
+Note that we need to modify the example YAML configuration and specify that our job will run on a runner with the **self-hosted** and the **type-cpx21**
+labels.
+
+.. code-block:: yaml
+
+     Explore-GitHub-Actions:
+       runs-on: [self-hosted, type-cpx21]
+
+So, the complete *demo.yml* that uses self-hosted runner is as follows:
+
+:demo.yml:
+
+   .. code-block:: yaml
+
+      name: GitHub Actions Demo
+      run-name: ${{ github.actor }} is testing out GitHub Actions 🚀
+      on: [push]
+      jobs:
+        Explore-GitHub-Actions:
+          runs-on: [self-hosted, type-cpx21]
+          steps:
+            - run: echo "🎉 The job was automatically triggered by a ${{ github.event_name }} event."
+            - run: echo "🐧 This job is now running on a ${{ runner.os }} server hosted by GitHub!"
+            - run: echo "🔎 The name of your branch is ${{ github.ref }} and your repository is ${{ github.repository }}."
+            - name: Check out repository code
+              uses: actions/checkout@v3
+            - run: echo "💡 The ${{ github.repository }} repository has been cloned to the runner."
+            - run: echo "🖥️ The workflow is now ready to test your code on the runner."
+            - name: List files in the repository
+              run: |
+                ls ${{ github.workspace }}
+            - run: echo "🍏 This job's status is ${{ job.status }}."
+
+
+❸ Finally, you will need to create a GitHub API token with the **workflow** privileges. Make sure to save the token!
+
+:For me, my *demo* GitHub token is:
+   ::
+
+      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
+
+You should now have your GitHub repository ready.
+
+See these steps in action:
+
+.. image:: https://raw.githubusercontent.com/testflows/TestFlows-GitHub-Runners/master/docs/images/github_create_repo_and_token.gif
+   :align: center
+   :alt: Creating GitHub Repository and Token
+
+----------------------------------------
+Creating Hetzner Cloud Project and Token
+----------------------------------------
+
+Next you will need to create a Hetzner Cloud project and an API token that we can use to create an manage Hetzner Cloud server instances.
+
+❶ Create new Hetzner Cloud project **Demo GitHub Runners**.
+
+❷ Now, create an API token and save it.
+
+:For me, the Hetzner Cloud token for my *Demo GitHub Runners* project is:
+   ::
+
+      5Up04IHuY8mC7l0JxKwh3Aps4ghGIyL0NJ9rGlhyAmmkddzuRreR1YstTSTFCG0N
+
+You should now have your Hetzner Cloud project ready.
+
+See these steps in action:
+
+.. image:: https://raw.githubusercontent.com/testflows/TestFlows-GitHub-Runners/master/docs/images/hetzner_create_project_and_token.gif
+   :align: center
+   :alt: Creating GitHub Repository and Token
+
+----------------------
+Creating Cloud Service
+----------------------
+
+With the GitHub repository and GitHub and Hetzner Cloud tokens in hand, we can deploy the **github-runners** service
+to Hetzner Cloud instance. This way the service is not running on your local machine.
+
+The deployment we'll create a **github-runners** instance in your Hetzner Cloud project on which the service will be running.
+See the `Running as a Cloud Service`_ section for details.
+
+❶ To deploy the service run the **github-runners cloud deploy** command and specify your
+GitHub repository, GitHub and Hetzner Cloud tokens using
+**GITHUB_REPOSITORY**, **GITHUB_TOKEN**, and **HETZNER_TOKEN** environment variables.
+
+.. code-block:: bash
+
+   export GITHUB_REPOSITORY=
+   export HETZNER_TOKEN=
+   export GITHUB_TOKEN=
+   github-runners cloud deploy
+
+You should now have the cloud service up and running.
+
+See these steps in action:
+
+.. image:: https://raw.githubusercontent.com/testflows/TestFlows-GitHub-Runners/master/docs/images/cloud_deploy.gif
+   :align: center
+   :alt: Deploying Cloud Service
+
+------------------------------------------
+Waiting for GitHub Actions Job to Complete
+------------------------------------------
+
+❶ The **github-runners** cloud service is now running. So, now you can just seat back and wait until **github-runners**
+spins up a new runner to complete any queued up GitHub Actions jobs in your GitHub repository.
+
+See this step in action:
+
+.. image:: https://raw.githubusercontent.com/testflows/TestFlows-GitHub-Runners/master/docs/images/github_job_completed.gif
+   :align: center
+   :alt: Waiting For GitHub Actions Job to Complete
+
+As you can see our job was executed and completed using our own self-hosted runner!
+
+:✋ Note:
+
+   If you run into any issues you can check cloud service logs using the
+   **github-runners cloud logs -f** command. For other cloud service commands see the `Running as a Cloud Service`_ section.
+
+   .. code-block:: bash
+
+      github-runners cloud logs -f
+
+=========================
 Installation From Sources
--------------------------
+=========================
 
 For development, you can install from sources as follows:
 
 .. code-block:: bash
 
    git clone https://github.com/testflows/Github-Runners.git
    ./package && ./install
 
-----
-
--------------------
+===================
 Basic Configuration
--------------------
+===================
 
 By default, the program uses the following environment variables:
 
 * **GITHUB_TOKEN**
 * **GITHUB_REPOSITORY**
 * **HETZNER_TOKEN**
 
 or you can specify these values using the following options:
 
 * **--github-token**
 * **--github-repository**
 * **--hetzner-token**
 
-----
-
-------------------------------------
+====================================
 Specifying Maximum Number of Runners
-------------------------------------
+====================================
+
 The default maximum number of runners is **10**. You can set a different value
 based on your Hetzner Cloud limits using the **-m count, --max-runners count** option. For example,
 
 .. code-block:: bash
 
    github-runners --max-runners 40
 
-----
-
--------------------------------
+===============================
 Jobs That Require Docker Engine
--------------------------------
+===============================
 
 For jobs that require Docker to be installed, you can use the standard `Hetzner Docker CE application <https://docs.hetzner.com/cloud/apps/list/docker-ce/>`_
 which can be specified using the **image-** label. See `Specifying Runner Image`_ for more details about specifying custom runner images.
 
 For example
 
 :x64:
@@ -199,22 +422,21 @@
 :ARM64:
 
    .. code-block:: yaml
 
       job-name:
          runs-on: [self-hosted, type-cax11, image-arm-app-docker-ce]
 
-----
-
-----------------------
+======================
 Specifying Runner Type
-----------------------
+======================
 
+-----------
 x64 Runners
-============
+-----------
 
 The default server type is **cx11** which is an Intel, 1 vCPU, 2GB RAM shared-cpu x64 instance.
 
 :✋ Note:
    You can use **--default-type** option to set a different default server type.
 
 You can specify different x64 server instance type by using the **type-{name}** runner label.
@@ -225,16 +447,17 @@
 as follows:
 
 .. code-block:: yaml
 
    job-name:
       runs-on: [self-hosted, type-cpx21]
 
+-------------
 ARM64 Runners
-==============
+-------------
 
 The default, the server type is **cx11**, which is an Intel, 1 vCPU, 2GB RAM shared-cpu x64 instance.
 Therefore, in order to use ARM64 runners you must specify ARM64 server instance type by using the **type-{name}** runner label.
 The **{name}** must be a valid `ARM64 Hetzner Cloud server type <https://www.hetzner.com/cloud>`_
 name such as *cax11*, *cax21* etc. which correspond to the Ampere Altra, 2 vCPU, 4GB RAM and
 4 vCPU, 8GB RAM shared-cpu ARM64 instances respectively.
 
@@ -242,19 +465,17 @@
 as follows:
 
 .. code-block:: yaml
 
    job-name:
       runs-on: [self-hosted, type-cax21]
 
-----
-
----------------------------
+==========================
 Specifying Runner Location
----------------------------
+==========================
 
 By default, the default location of the server where the runner will be running is not specified. You can use the **--default-location**
 option to force specific default server location.
 
 You can also use the **in-{name}** runner label to specify server location for a specific job. Where **{name}** must be a valid
 `Hetzner Cloud location <https://docs.hetzner.com/cloud/general/locations/>`_ name such as *ash* for US, Ashburn, VA or
 *fsn1* for Germany, Falkenstein.
@@ -262,19 +483,17 @@
 For example,
 
 .. code-block:: yaml
 
    job-name:
       runs-on: [self-hosted, type-cx11, in-ash]
 
-----
-
------------------------
+=======================
 Specifying Runner Image
------------------------
+=======================
 
 By default, the default image of the server for the runner is **ubuntu-22.04**. You can use the **--default-image**
 option to force specific default server image.
 
 You can also use the **image-{architecture}-{type}-{name}** runner label to specify server image for a specific job.
 
 Where,
@@ -306,19 +525,17 @@
    must be unique.
 
    .. code-block:: yaml
 
       job-name:
          runs-on: [self-hosted, type-cx11, in-ash, image-x86-snapshot-snapshot_description]
 
-----
-
---------------------------------------------
+============================================
 Specifying Custom Runner Server Setup Script
---------------------------------------------
+============================================
 
 You can specify custom runner server setup script using the **--setup-script** option.
 
 For example,
 
 :custom_setup.sh:
    .. code-block:: bash
@@ -338,19 +555,17 @@
       apt-get -y install ca-certificates curl gnupg lsb-release python3-pip git unzip
 
 :command:
    .. code-block:: bash
 
       github-runners --setup-script ./custom_setup.sh
 
-----
-
---------------------------
+==========================
 Specifying Standby Runners
---------------------------
+==========================
 
 You can define standby runner groups to be always ready to pick your jobs using a custom configuration file.
 
 :✋ Note:
    Standby runner groups can only be defined using a configuration file.
    See `Using Configuration File`_ for more details.
 
@@ -384,19 +599,17 @@
                   labels=["type-cx21"],
                   count=2,
                   replenish_immediately=True,
             )
          ],
       )
 
-----
-
--------------------------------
+===============================
 Specifying Logger Configuration
--------------------------------
+===============================
 
 You can specify custom logger configuration using a configuration file.
 
 :✋ Note:
    Custom logger configuration can only be specified using a configuration file.
    See `Using Configuration File`_ for more details.
 
@@ -430,19 +643,17 @@
              },
              "loggers": {
                  "testflows.github.runners": {"level": "INFO", "handlers": ["default"]},
              },
          }
      )
 
-----
-
---------------------------------------
+======================================
 Deleting All Runners And Their Servers
---------------------------------------
+======================================
 
 You can delete all runners, including standby runners, and their servers using the **delete** command.
 
 :✋ Note:
    The **delete** command will not delete cloud service server. If you also want to delete it,
    you also need to execute **cloud delete** command. For more information, see `Deleting Cloud Service`_ section.
 
@@ -454,19 +665,17 @@
 
    07/29/2023 07:43:16 PM     INFO       MainThread             all 🍀 Logging in to Hetzner Cloud
    07/29/2023 07:43:16 PM     INFO       MainThread             all 🍀 Logging in to GitHub
    07/29/2023 07:43:16 PM     INFO       MainThread             all 🍀 Getting repository testflows/testflows-github-runners
    07/29/2023 07:43:17 PM     INFO       MainThread             all 🍀 Getting list of self-hosted runners
    07/29/2023 07:43:17 PM     INFO       MainThread             all 🍀 Getting list of servers
 
-----
-
-------------------------
+========================
 Using Configuration File
-------------------------
+========================
 
 Instead of passing configuration options using command line arguments, you can use
 configuration file. The configuration file is Python file that must define the **config**
 object of the `Config class`_.
 
 :✋ Note:
    When you mix command line options and custom configuration file,
@@ -511,16 +720,17 @@
 
 You can pass your custom configuration file using the **-c path, --config path** command line option.
 
 .. code-block:: bash
 
    github-runners -c config.py
 
+--------------------
 Configuration Schema
-=====================
+--------------------
 
 The `Config class`_ has the following schema:
 
 :schema:
    * **github_token: str**
    * **github_repository: str**
    * **hetzner_token: str**
@@ -549,59 +759,56 @@
          * **location: location**
          * **setup_script: path**
    * **standby_runners: list[standby_runner]**
       * **labels: list[str]**
       * **count: count**
       * **replenish_immediately: bool**
 
-----
-
--------
-SSH Key
--------
+==================
+Specifying SSH Key
+==================
 
 All server instances that are created are accessed via SSH using the **ssh** utility and therefore you must provide a valid SSH key
 using the **--ssh-key** option. If the **--ssh-key** option is no specified, then the *~/.ssh/id_rsa.pub* default key path will be used.
 
 The SSH key will be automatically added to your project using the MD5 hash of the public key as the SSH key name.
 
 :❗Warning:
    Given that each new SSH key is automatically added to your Hetzner project, you must manually delete them when no longer needed.
 
 Most GitHub users already have an SSH key associated with the account. If you want to know how to add an SSH key, see `Adding a new SSH key to your GitHub account    <https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account>`_ article.
 
+----------------------
 Generating New SSH Key
-=======================
+----------------------
 
 If you need to generate a new SSH key, see `Generating a new SSH key and adding it to the ssh-agent <https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent>`_ article.
 
-Cloud Deployment
-================
+----------------------------
+SSH Keys in Cloud Deployment
+----------------------------
 
 If you are deploying the **github-runners** program as a cloud service using the **github-runners <options> cloud deploy** command, then
 after provisoning a new cloud server instance that will host the **github-runners** service, a new SSH key will be
 auto-generated to access the runners. The auto-generated key will be placed in */home/runner/.ssh/id_rsa*, where **runner**
 is the user under which the **github-runners** service runs on the cloud instance. The auto-generated SSH key will be automatically
 added to your project using the MD5 hash of the public key as the SSH key name.
 
-----
-
------------------------
+====================
 Running as a Service
------------------------
+====================
 
 You can run **github-runners** as a service.
 
 :✋ Note:
    In order to install the service, the user that installed the module must have **sudo** privileges.
 
-----
-
+---------------------------
 Installing and Uninstalling
-===========================
+---------------------------
 
 After installation, you can use **service install** and **service uninstall** commands to install and
 uninstall the service.
 
 :✋ Note:
    The options that are passed to the **github-runners <options> service install** command
    will be the same options with which the service will be executed.
@@ -635,34 +842,32 @@
       Environment=GITHUB_TOKEN=ghp_...
       Environment=GITHUB_REPOSITORY=testflows/github-runners
       Environment=HETZNER_TOKEN=GJ..
       ExecStart=/home/user/.local/lib/python3.10/site-packages/testflows/github/runners/bin/github-runners --workers 10 --max-powered-off-time 20 --max-unused-runner-time 120 --max-runner-registration-time 60 --scale-up-interval 10 --scale-down-interval 10
       [Install]
       WantedBy=multi-user.target
 
-----
-
+-------------------------
 Modifying Program Options
-=========================
+-------------------------
 
 If you want to modify service program options you can stop the service,
 edit the **/etc/systemd/system/github-runners.service** file by hand, then reload service daemon,
 and start the service back up.
 
 .. code-block:: bash
 
    github-runners service stop
    sudo vim /etc/systemd/system/github-runners.service
    sudo systemctl daemon-reload
    github-runners service start
 
-----
-
+---------------
 Checking Status
-================
+---------------
 
 After installation, you can check the status of the service using the **service status** command.
 
 .. code-block:: bash
 
    github-runners service status:
 
@@ -684,18 +889,17 @@
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Logging in to Hetzner >
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Logging in to GitHub
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Getting repository vza>
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Creating scale up serv>
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Creating scale down se>
       lines 1-16/16 (END)
 
-----
-
+---------------------
 Manual Start and Stop
-=====================
+---------------------
 
 You can start and stop the service using the **service start** and **service stop** commands as follows:
 
 .. code-block:: bash
 
    github-runners service start
    github-runners service stop
@@ -703,18 +907,17 @@
 or using **service** system utility
 
 .. code-block:: bash
 
    sudo service github-runners start
    sudo service github-runners stop
 
-----
-
+-------------
 Checking Logs
-=============
+-------------
 
 You can get the logs for the service using the **service logs** command.
 
 Use **-f, --follow** option to follow logs journal.
 
 .. code-block:: bash
 
@@ -757,19 +960,17 @@
       Jul 24 14:24:42 user-node env[62771]: LANGUAGE=en_CA:en
       Jul 24 14:24:42 user-node env[62771]: PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/snap/bin
       Jul 24 14:24:42 user-node env[62771]: INVOCATION_ID=dc7b778f95fa4ccf95e4a4592b50d9e1
       Jul 24 14:24:42 user-node env[62771]: JOURNAL_STREAM=8:328542
       Jul 24 14:24:42 user-node env[62771]: SYSTEMD_EXEC_PID=62771
       ...
 
-----
-
---------------------------
+==========================
 Running as a Cloud Service
---------------------------
+==========================
 
 Instead of running **github-runners** program locally as a standalone application or as a service.
 You can easily deploy **github-runners** to run on a Hetzner Cloud instance.
 
 See **-h, --help** for all the available commands.
 
 :✋ Note:
@@ -777,18 +978,17 @@
    is **github-runners**. If you want to use a custom server name, then
    you must use the **cloud --name** option for any **cloud** commands.
 
 .. code-block:: bash
 
    github-runners cloud -h
 
-----
-
-Deployment
-==========
+---------
+Deploying
+---------
 
 You can deploy **github-runners** as a service to a new Hetzner Cloud server instance, that will be created for you automatically,
 using the **cloud deploy** command.
 
 :✋ Note:
    The options that are passed to the **github-runners <options> cloud deploy** command
    will be the same options with which the service will be executed.
@@ -847,15 +1047,15 @@
 
    github-runners deploy --location nbg1 --type cx11 --image ubuntu-22.04
 
 The cloud instance that runs the **github-runners** service can either be x64 or ARM64 instance. By default, **cpx11**
 AMD, 2 vCPU, 2GB RAM, shared-cpu x64 instance type is used.
 
 Using ARM64 Instance
-++++++++++++++++++++
+====================
 
 If you want to deploy the **github-runners** service to an ARM64 instance, then you must specify the instance
 type using the **--type** option.
 
 :✋ Note:
    Currently Hetzner Cloud has ARM64 instances only available in Germany, Falkenstein (**fsn1**) location.
 
@@ -863,41 +1063,39 @@
 as the value of the **--type** as follows:
 
 .. code-block:: bash
 
    github-runners deploy --location fsn1 --type cax21 --image ubuntu-22.04
 
 Using x64 Instance
-++++++++++++++++++
+==================
 
 By default, the **cpx11** AMD, 2 vCPU, 2GB RAM, shared-cpu x64 instance type is used. If you want to use
 a different x64 instance then specify desired type using the **--type** option.
 
-----
-
+-------------------------
 Redeploying Cloud Service
-=========================
+-------------------------
 
 You can change cloud service configuration or cloud service package version without deleting the existing cloud service server
 using the **cloud redeploy** command.
 
 .. code-block:: bash
 
    github-runners <options> cloud redeploy
 
 :✋ Note:
    The options that are passed to the **github-runners <options> cloud redeploy** command
    will be the same options with which the service will be executed.
 
 You can specify the version of the package to be installed using the **--version** option.
 
-----
-
+------------------
 Cloud Service Logs
-===================
+------------------
 
 You can check logs for the **github-runners** service running on a cloud instance using the **github-runners cloud logs** command.
 Specify **-f, --follow** if you want to follow the logs journal.
 
 For example,
 
 :dump the full log:
@@ -908,54 +1106,50 @@
 
 :follow the logs journal:
 
    .. code-block:: bash
 
       github-runners cloud logs -f
 
-----
-
+--------------------
 Cloud Service Status
-=====================
+--------------------
 
 You can check the status of the **github-runners** service running on a cloud instance using the **github-runners cloud status** command.
 
 For example,
 
 .. code-block:: bash
 
    github-runners cloud status
 
-----
-
+----------------------
 Stopping Cloud Service
-======================
+----------------------
 
 You can manually stop the **github-runners** service running on a cloud instance using the **github-runners cloud stop** command.
 
 .. code-block:: bash
 
    github-runners cloud stop
 
-----
-
+----------------------
 Starting Cloud Service
-======================
+----------------------
 
 You can manually start the **github-runners** service running on a cloud instance after it was being manually stopped
 using the **github-runners cloud start** command.
 
 .. code-block:: bash
 
    github-runners cloud start
 
-----
-
+------------------------
 Installing Cloud Service
-========================
+------------------------
 
 You can manually force installation of the **github-runners** service running on a cloud instance using
 the **github-runners cloud install** command.
 
 :✋ Note:
    Just like with the `github-runners <options> service install` command,
    the options that are passed to the `github-runners <options> cloud install` command
@@ -963,30 +1157,28 @@
 
 You can specify **-f, --force** option to force service re-installation if it is already installed.
 
 .. code-block:: bash
 
    github-runners <options> cloud install -f
 
-----
-
+--------------------------
 Uninstalling Cloud Service
-==========================
+--------------------------
 
 You can manually force uninstallation of the **github-runners** service running on a cloud instance using
 the **github-runners cloud uninstall** command.
 
 .. code-block:: bash
 
    github-runners cloud uninstall
 
-----
-
+-------------------------------
 Upgrading Cloud Service Package
-===============================
+-------------------------------
 
 You can manually upgrade the **github-runners** service package running on a cloud instance using
 the **github-runners cloud upgrade** command.
 
 If specific '--version' is specified then the *testflows.github.runners* package is upgraded to
 the specified version otherwise the version is upgraded to the latest available.
 
@@ -998,18 +1190,17 @@
 .. code-block:: bash
 
    github-runners cloud upgrade --version <version>
 
 The service is not re-installed during the package upgrade process.
 Instead, it is stopped before the upgrade and then started back up
 
-----
-
+------------------------------
 Changing Cloud Service Options
-==============================
+------------------------------
 
 If you need to change cloud service options such as the **--setup-script** or the **--max-runners** etc.,
 you can keep the existing server and use **cloud redeploy** command.
 
 .. code-block:: bash
 
    github-runners <options> cloud redeploy --version latest
@@ -1024,18 +1215,17 @@
    github-runners <options> cloud deploy --version latest
 
 :✋ Note:
    Complete teardown will not affect any current jobs as the service is designed to
    be restartable. However, some servers might be left in an unfinished state
    but they will be cleaned up when the service is restarted.
 
-----
-
+----------------------
 Deleting Cloud Service
-======================
+----------------------
 
 You can delete the **github-runners** cloud service and the cloud instance that is running on using
 the **github-runners cloud delete** command.
 
 The **cloud delete** command, deletes the cloud service by first stopping the service and then deleting the server instance.
 
 :❗Warning:
@@ -1050,18 +1240,17 @@
       github-runners cloud delete
 
 :custom name:
    .. code-block:: bash
 
       github-runners cloud --name <custom_name> delete
 
-----
-
+-----------------------
 SSH in to Cloud Service
-==============================
+-----------------------
 
 You can open SSH client to the cloud service using the **cloud ssh** command. For example,
 
 .. code-block:: bash
 
    github-runners cloud ssh
 
@@ -1074,19 +1263,17 @@
 
 The output will contain the full **ssh** command including the IP address of the cloud service server.
 
 ::
 
    ssh -q -o "StrictHostKeyChecking no" root@5.161.87.21
 
-----
-
-------------------
+==================
 Scaling Up Runners
-------------------
+==================
 
 The program scales up runners by looking for any jobs that have **queued** status.
 For each such job, a corresponding Hetzner Cloud server instance is created with the following name:
 
 ::
 
    github-runner-{job.id}
@@ -1103,30 +1290,28 @@
 Also,
 
 :Note:
    There is no guarantee that a given runner will pick the job with the exact **job.id** that caused it to be created.
    This is expected and because for each **queued** job a unique runner will be created the number of runners will be
    equal the number of jobs and therefore under normal conditions all jobs will be executed as expected.
 
-----
-
+-------------------------
 Maximum Number of Runners
-=========================
+-------------------------
 
 By default, the maximum number of runners and therefore the maximum number of server instances is not set and therefore is unlimited.
 You can set the maximum number of runners using the **--max-runners** option.
 
 .. code-blocks::bash
 
    github-runners --max-runners 10
 
-----
-
+----------
 New Server
-==========
+----------
 
 The new server is accessed using SSH. It boots up with the specified OS image and is configured using
 the **setup** and **startup** scripts.
 
 :Server Type:
 
    The default server type is **cx11** which is an Intel, 1 vCPU, 2GB RAM shared-cpu x64 instance.
@@ -1156,18 +1341,17 @@
 
    The server is configured to be accessed using *ssh* utility and the SSH public key path is specified using the **--ssh-key**
    option.
 
 :Image Configuration:
    Each new server instance is configured using the `setup <#the-setup-script>`_ and the `startup <#the-start-up-script>`_ scripts.
 
-----
-
+----------------
 The Setup Script
-================
+----------------
 
 The **setup** script creates and configures **runner** user that has **sudo** privileges.
 
 :Setup:
 
    .. code-block:: bash
 
@@ -1177,18 +1361,17 @@
 
         adduser ubuntu --disabled-password --gecos ""
         echo "%wheel   ALL=(ALL:ALL) NOPASSWD:ALL" >> /etc/sudoers
         addgroup wheel
         usermod -aG wheel ubuntu
         usermod -aG sudo ubuntu
 
-----
-
+-------------------
 The Start-up Script
-===================
+-------------------
 
 The **startup** script installs GitHub Actions runner. After installation it configures the runner to start in an *--ephemeral* mode.
 The *--ephemeral* mode causes the runner to exit as soon as it completes a job. After the runner exits the server is powered off.
 
 :✋ Note:
    The **startup** script is executed as **ubuntu** user and therefore you must use **sudo** for any commands that need *root* privileges.
 
@@ -1228,50 +1411,49 @@
 
      echo "Configure runner"
      ./config.sh --unattended --replace --url https://github.com/${GITHUB_REPOSITORY} --token ${GITHUB_RUNNER_TOKEN} --name "$(hostname)" --runnergroup "${GITHUB_RUNNER_GROUP}" --labels "${GITHUB_RUNNER_LABELS}" --work _work --ephemeral
 
      echo "Start runner"
      bash -c "screen -d -m bash -c './run.sh; sudo poweroff'"
 
-----
-
---------------------
+====================
 Scaling Down Runners
---------------------
+====================
 
+-------------------
 Powered Off Servers
-===================
+-------------------
 
 The program scales down runners by first cleaning up powered off servers. The scale down service relies on the fact
 that the `startup <#the-start-up-script>`_ script starts an ephemeral runner which will pick up only 1 job and then will power itself off after the job is complete.
 
 The powered off servers are deleted after the **max-powered-off-time** interval which
 can be specified using the **--max-powered-off-time** option which by default is set to *20* sec.
 
+--------------
 Unused Runners
-==============
+--------------
 
 The scale down service also monitors all the runners that have **unused** status and tries to delete any servers associated with such
 runners if the runner is **unused** for more than the **max-unused-runner-time** period. This is needed in case a runner never gets a job
 assigned to it and the server will stay in the power on state. This cycle relies on the fact that the runner's name
 is the same as server's name. The **max-unused-runner-time** can be specified using the **--max-unused-runner-time** option which by default
 is set to *120* sec.
 
+--------------
 Zombie Servers
-==============
+--------------
 
 The scale down service will delete any zombie servers. A zombie server is defined as as any server that fails to register its runner within
 the **max-runner-registration-time**. The **max-runner-registration-time** can be specified using the **--max-runner-registration-time** option
 which by default is set to *60* sec.
 
-----
-
----------------------------
+===========================
 Handling Failing Conditions
----------------------------
+===========================
 
 The program is designed to handle the following failing conditions:
 
 :Server Never Registers a Runner:
    The server will remain in **running** state and should be reclaimed by the scale down service when it checks the actual runners registered for current servers.
    If it finds a server that is **running** but no runner is active for it it will be deleted after the **max-runner-registration-time** period.
 
@@ -1286,19 +1468,17 @@
 
 :Runner Never Gets a Job Assigned:
    If the runner never gets a job assigned, then the scale down service will remove the runner and delete its server after the **max-unused-runner-time** period.
 
 :Runner Created With a Mismatched Labels:
    The behavior will be the same as for the **Runner Never Gets a Job Assigned** case above.
 
-----
-
----------------
+===============
 Program Options
----------------
+===============
 
 The following options are supported:
 
 * **-h, --help**
   show this help message and exit
 
 * **-v, --version**
@@ -1474,16 +1654,16 @@
 
       * **start**
         start service
 
       * **stop**
         stop service
 
------------------
+=================
 Table of Contents
------------------
+=================
 
-.. contents:: Index:
+.. contents::
    :backlinks: top
    :depth: 4
 
 .. _Config class: https://github.com/testflows/TestFlows-GitHub-Runners/blob/main/testflows/github/runners/config.py#L45
```

### Comparing `testflows.github.runners-1.3.230731.1173142/setup.py` & `testflows.github.runners-1.3.230731.1223345/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.3.230731.1173142",
+    version="1.3.230731.1223345",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/__init__.py` & `testflows.github.runners-1.3.230731.1223345/testflows/github/runners/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.3.230731.1173142"
+__version__ = "1.3.230731.1223345"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/actions.py` & `testflows.github.runners-1.3.230731.1223345/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/args.py` & `testflows.github.runners-1.3.230731.1223345/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.3.230731.1223345/testflows/github/runners/bin/github-runners`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/cloud.py` & `testflows.github.runners-1.3.230731.1223345/testflows/github/runners/cloud.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/config.py` & `testflows.github.runners-1.3.230731.1223345/testflows/github/runners/config.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/delete.py` & `testflows.github.runners-1.3.230731.1223345/testflows/github/runners/delete.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/logger.py` & `testflows.github.runners-1.3.230731.1223345/testflows/github/runners/logger.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/request.py` & `testflows.github.runners-1.3.230731.1223345/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.3.230731.1223345/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.3.230731.1223345/testflows/github/runners/scale_up.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.3.230731.1223345/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.3.230731.1223345/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scripts/deploy/setup.sh` & `testflows.github.runners-1.3.230731.1223345/testflows/github/runners/scripts/deploy/setup.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scripts/setup_docker.sh` & `testflows.github.runners-1.3.230731.1223345/testflows/github/runners/scripts/setup_docker.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.3.230731.1223345/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.3.230731.1223345/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/server.py` & `testflows.github.runners-1.3.230731.1223345/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/service.py` & `testflows.github.runners-1.3.230731.1223345/testflows/github/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/shell.py` & `testflows.github.runners-1.3.230731.1223345/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1173142/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.3.230731.1223345/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: testflows.github.runners
-Version: 1.3.230731.1173142
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
@@ -30,22 +13,26 @@
 
 ======================================================
 Autoscaling GitHub Actions Runners Using Hetzner Cloud
 ======================================================
 
 A simple alternative to Github's `Recommended autoscaling solutions <https://docs.github.com/en/actions/hosting-your-own-runners/managing-self-hosted-runners/autoscaling-with-self-hosted-runners#recommended-autoscaling-solutions>`_.
 
+:🔍 Tip:
+   You can easily navigate this documentation page by clicking on any title to jump to the `Table of Contents`_.
+   Try it out, and remember, if you get lost just click any title!
+
 The **github-runners** service program starts and monitors queued up jobs for GitHub Actions workflows.
 When a new job is queued up, it creates a new Hetzner Cloud server instance
 that provides an ephemeral GitHub Actions runner. Each server instance is automatically
 powered off when job completes and then powered off servers are
 automatically deleted. Both **x64** (*x86*) and **arm64** (*arm*) runners are supported.
 See `Features`_ and `Limitations`_ for more details.
 
-.. image:: https://raw.githubusercontent.com/testflows/TestFlows-GitHub-Runners/master/intro.gif
+.. image:: https://raw.githubusercontent.com/testflows/TestFlows-GitHub-Runners/master/docs/images/intro.gif
    :align: center
    :alt: TestFlows GitHub Runners
 
 
 :❗Warning:
    This program is provided on "AS IS" basis without warranties or conditions of any kind. See LICENSE.
    Use it at your own risk. Manual monitoring is required to make sure server instances are cleaned up properly
@@ -55,86 +42,95 @@
 to avoid any cleanup. Server instances are not shared between any jobs.
 
 :✋ Note:
    Currently Hetzner Cloud server instances are billed on hourly basis. So a job that takes 1 min will be billed
    the same way as for a job that takes 59 minutes. Therefore, the minimal cost
    for any job is the cost of the server for 1 hour plus the cost for one public IPv4 address.
 
-----
-
-:🔍 Tip:
-   You can easily navigate this documentation page by clicking on any title to jump to the `Table of Contents`_.
-   Try it out, and remember, if you get lost just click any title!
-
-----
-
---------
+========
 Features
---------
+========
 
 * cost efficient on-demand runners using `Hetzner Cloud <https://www.hetzner.com/cloud>`_
 * simple configuration, no Webhooks, no need for AWS lambdas, and no need to setup any GitHub application
 * supports specifying custom runner server types, images, and locations using job labels
 * self-contained program that you can use to deploy, redeploy, and manage the service on a cloud instance
 * supports x64 (x86) and ARM64 (arm) runners
 * supports using any Hetzner Cloud server types
 * supports runners with pre-installed Docker
 * supports using any standard Hetzner Cloud images and applications
 * supports auto-replenishable fixed standby runner pools for jobs to be picked up immediately
 * simpler alternative to what GitHub lists in `Recommended autoscaling solutions <https://docs.github.com/en/actions/hosting-your-own-runners/managing-self-hosted-runners/autoscaling-with-self-hosted-runners#recommended-autoscaling-solutions>`_
 
-----
-
------------
+===========
 Limitations
------------
-
-* **Group runners are not supported**
-
-     However, you can run individual services for each repository using different Hetzner Cloud projects.
+===========
 
-* **Unique Hetzner Cloud project must be used for each repository**
+**Group runners are not supported**
+  ✎ However, you can run individual services for each repository using different Hetzner Cloud projects.
 
-     However, unique projects allow to easily keep track of runner costs per repository.
-
-----
+**Unique Hetzner Cloud project must be used for each repository**
+   ✎ However, unique projects allow to easily keep track of runner costs per repository.
 
--------------
+=============
 Prerequisites
--------------
+=============
 
 * Python >= 3.7
 * `Hetzner Cloud <https://www.hetzner.com/cloud>`_ account
 * GitHub API token with admin privileges to manage self-hosted runners
 
-----
-
-------------
+============
 Installation
-------------
+============
 
 .. code-block:: bash
 
    pip3 install testflows.github.runners
 
-----
+Check that the **github-runners** utility was installed correctly by executing the **github-runners -v** command.
+
+.. code-block:: bash
+
+   github-runners -v
+
+The **github-runners** utility is installed in to the *~/.local/bin/* folder. Please make sure that this folder
+is part of the **PATH**.
+
+.. code-block:: bash
+
+   which github-runners
+
+::
+
+   ~/.local/bin/github-runners
+
+If your **PATH** is missing this folder, on Ubuntu, modify your *~/.profile* and add the following section:
 
-------------
+:~/.profile:
+   .. code-block:: bash
+
+      # set PATH so it includes user's private bin if it exists
+      if [ -d "$HOME/.local/bin" ] ; then
+          PATH="$HOME/.local/bin:$PATH"
+      fi
+
+===========
 Quick Start
-------------
+===========
 
-Set environment variables corresponding to your GitHub repository and Hetzner Cloud project
+Set environment variables corresponding to your GitHub repository and Hetzner Cloud project.
 
 .. code-block:: bash
 
    export GITHUB_TOKEN=ghp_...
    export GITHUB_REPOSITORY=vzakaznikov/github-runners
    export HETZNER_TOKEN=GJzdc...
 
-and then start **github-runners** program
+Then, start the **github-runners** program:
 
 .. code-block:: bash
 
    github-runners
 
 ::
 
@@ -142,68 +138,261 @@
    07/22/2023 08:20:37 PM   INFO MainThread            main 🍀 Logging in to GitHub
    07/22/2023 08:20:37 PM   INFO MainThread            main 🍀 Getting repository vzakaznikov/github-runners
    07/22/2023 08:20:37 PM   INFO MainThread            main 🍀 Creating scale up service
    07/22/2023 08:20:37 PM   INFO MainThread            main 🍀 Creating scale down service
    07/22/2023 08:20:38 PM   INFO   worker_2   create_server 🍀 Create server
    ...
 
-or you can pass the required options inline as follows:
+Alternatively, you can pass the required options using the command line as follows:
 
 .. code-block:: bash
 
    github-runners --github-token <GITHUB_TOKEN> --github-repository <GITHUB_REPOSITORY> --hetzner-token <HETZNER_TOKEN>
 
-----
+========================
+Getting Started Tutorial
+========================
 
--------------------------
+:✅ Launch your first self-hosted runner in:
+   5 minutes
+
+This tutorial will guide you on how to use the **github-runners** program to provide autoscaling GitHub Actions runners
+for a GitHub repository and a Hetzner Cloud project that you'll create.
+
+-----------------------------------
+Installing TestFlows Github Runners
+-----------------------------------
+
+❶ Before we get started, you will need to install **testflows.github.runners** Python package. See the `Installation`_ section for more details.
+
+.. code-block:: bash
+
+  pip3 install testflows.github.runners
+
+❷ Check that the **github-runners** utility was installed correctly by executing the **github-runners -v** command.
+
+.. code-block:: bash
+
+   github-runners -v
+
+::
+
+   1.3.230731.1173142
+
+:✋ Note:
+   The **github-runners** utility is installed in to the *~/.local/bin/* folder. Please make sure that this folder
+   is part of the **PATH**.
+
+   .. code-block:: bash
+
+      which github-runners
+
+   ::
+
+      ~/.local/bin/github-runners
+
+   If your **PATH** is missing this folder, on Ubuntu, you can modify your *~/.profile* and add the following section:
+
+   :~/.profile:
+      .. code-block:: bash
+
+         # set PATH so it includes user's private bin if it exists
+         if [ -d "$HOME/.local/bin" ] ; then
+             PATH="$HOME/.local/bin:$PATH"
+         fi
+
+In order to launch the **github-runners** program, we'll need to specify GitHub repository as well as GitHub and
+Hetzner Cloud tokens. So, let's create these.
+
+----------------------------------------------------------
+Creating GitHub Repository with Actions Workflow and Token
+----------------------------------------------------------
+
+Before using the **github-runners**, you need a GitHub repository with a GitHub Actions workflow set up.
+
+❶ First, create GitHub Repository named **demo-testflows-github-runners** and note the repository name.
+
+The repository name will have the following format:
+
+::
+
+   <username>/demo-testflows-github-runners
+
+:For me, my GitHub repository is:
+   ::
+
+      vzakaznikov/demo-testflows-github-runners
+
+❷ Now, create an example GitHub Actions workflow as described in the `Quickstart for GitHub Actions <https://docs.github.com/en/actions/quickstart>`_ article.
+Note that we need to modify the example YAML configuration and specify that our job will run on a runner with the **self-hosted** and the **type-cpx21**
+labels.
+
+.. code-block:: yaml
+
+     Explore-GitHub-Actions:
+       runs-on: [self-hosted, type-cpx21]
+
+So, the complete *demo.yml* that uses self-hosted runner is as follows:
+
+:demo.yml:
+
+   .. code-block:: yaml
+
+      name: GitHub Actions Demo
+      run-name: ${{ github.actor }} is testing out GitHub Actions 🚀
+      on: [push]
+      jobs:
+        Explore-GitHub-Actions:
+          runs-on: [self-hosted, type-cpx21]
+          steps:
+            - run: echo "🎉 The job was automatically triggered by a ${{ github.event_name }} event."
+            - run: echo "🐧 This job is now running on a ${{ runner.os }} server hosted by GitHub!"
+            - run: echo "🔎 The name of your branch is ${{ github.ref }} and your repository is ${{ github.repository }}."
+            - name: Check out repository code
+              uses: actions/checkout@v3
+            - run: echo "💡 The ${{ github.repository }} repository has been cloned to the runner."
+            - run: echo "🖥️ The workflow is now ready to test your code on the runner."
+            - name: List files in the repository
+              run: |
+                ls ${{ github.workspace }}
+            - run: echo "🍏 This job's status is ${{ job.status }}."
+
+
+❸ Finally, you will need to create a GitHub API token with the **workflow** privileges. Make sure to save the token!
+
+:For me, my *demo* GitHub token is:
+   ::
+
+      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
+
+You should now have your GitHub repository ready.
+
+See these steps in action:
+
+.. image:: https://raw.githubusercontent.com/testflows/TestFlows-GitHub-Runners/master/docs/images/github_create_repo_and_token.gif
+   :align: center
+   :alt: Creating GitHub Repository and Token
+
+----------------------------------------
+Creating Hetzner Cloud Project and Token
+----------------------------------------
+
+Next you will need to create a Hetzner Cloud project and an API token that we can use to create an manage Hetzner Cloud server instances.
+
+❶ Create new Hetzner Cloud project **Demo GitHub Runners**.
+
+❷ Now, create an API token and save it.
+
+:For me, the Hetzner Cloud token for my *Demo GitHub Runners* project is:
+   ::
+
+      5Up04IHuY8mC7l0JxKwh3Aps4ghGIyL0NJ9rGlhyAmmkddzuRreR1YstTSTFCG0N
+
+You should now have your Hetzner Cloud project ready.
+
+See these steps in action:
+
+.. image:: https://raw.githubusercontent.com/testflows/TestFlows-GitHub-Runners/master/docs/images/hetzner_create_project_and_token.gif
+   :align: center
+   :alt: Creating GitHub Repository and Token
+
+----------------------
+Creating Cloud Service
+----------------------
+
+With the GitHub repository and GitHub and Hetzner Cloud tokens in hand, we can deploy the **github-runners** service
+to Hetzner Cloud instance. This way the service is not running on your local machine.
+
+The deployment we'll create a **github-runners** instance in your Hetzner Cloud project on which the service will be running.
+See the `Running as a Cloud Service`_ section for details.
+
+❶ To deploy the service run the **github-runners cloud deploy** command and specify your
+GitHub repository, GitHub and Hetzner Cloud tokens using
+**GITHUB_REPOSITORY**, **GITHUB_TOKEN**, and **HETZNER_TOKEN** environment variables.
+
+.. code-block:: bash
+
+   export GITHUB_REPOSITORY=
+   export HETZNER_TOKEN=
+   export GITHUB_TOKEN=
+   github-runners cloud deploy
+
+You should now have the cloud service up and running.
+
+See these steps in action:
+
+.. image:: https://raw.githubusercontent.com/testflows/TestFlows-GitHub-Runners/master/docs/images/cloud_deploy.gif
+   :align: center
+   :alt: Deploying Cloud Service
+
+------------------------------------------
+Waiting for GitHub Actions Job to Complete
+------------------------------------------
+
+❶ The **github-runners** cloud service is now running. So, now you can just seat back and wait until **github-runners**
+spins up a new runner to complete any queued up GitHub Actions jobs in your GitHub repository.
+
+See this step in action:
+
+.. image:: https://raw.githubusercontent.com/testflows/TestFlows-GitHub-Runners/master/docs/images/github_job_completed.gif
+   :align: center
+   :alt: Waiting For GitHub Actions Job to Complete
+
+As you can see our job was executed and completed using our own self-hosted runner!
+
+:✋ Note:
+
+   If you run into any issues you can check cloud service logs using the
+   **github-runners cloud logs -f** command. For other cloud service commands see the `Running as a Cloud Service`_ section.
+
+   .. code-block:: bash
+
+      github-runners cloud logs -f
+
+=========================
 Installation From Sources
--------------------------
+=========================
 
 For development, you can install from sources as follows:
 
 .. code-block:: bash
 
    git clone https://github.com/testflows/Github-Runners.git
    ./package && ./install
 
-----
-
--------------------
+===================
 Basic Configuration
--------------------
+===================
 
 By default, the program uses the following environment variables:
 
 * **GITHUB_TOKEN**
 * **GITHUB_REPOSITORY**
 * **HETZNER_TOKEN**
 
 or you can specify these values using the following options:
 
 * **--github-token**
 * **--github-repository**
 * **--hetzner-token**
 
-----
-
-------------------------------------
+====================================
 Specifying Maximum Number of Runners
-------------------------------------
+====================================
+
 The default maximum number of runners is **10**. You can set a different value
 based on your Hetzner Cloud limits using the **-m count, --max-runners count** option. For example,
 
 .. code-block:: bash
 
    github-runners --max-runners 40
 
-----
-
--------------------------------
+===============================
 Jobs That Require Docker Engine
--------------------------------
+===============================
 
 For jobs that require Docker to be installed, you can use the standard `Hetzner Docker CE application <https://docs.hetzner.com/cloud/apps/list/docker-ce/>`_
 which can be specified using the **image-** label. See `Specifying Runner Image`_ for more details about specifying custom runner images.
 
 For example
 
 :x64:
@@ -216,22 +405,21 @@
 :ARM64:
 
    .. code-block:: yaml
 
       job-name:
          runs-on: [self-hosted, type-cax11, image-arm-app-docker-ce]
 
-----
-
-----------------------
+======================
 Specifying Runner Type
-----------------------
+======================
 
+-----------
 x64 Runners
-============
+-----------
 
 The default server type is **cx11** which is an Intel, 1 vCPU, 2GB RAM shared-cpu x64 instance.
 
 :✋ Note:
    You can use **--default-type** option to set a different default server type.
 
 You can specify different x64 server instance type by using the **type-{name}** runner label.
@@ -242,16 +430,17 @@
 as follows:
 
 .. code-block:: yaml
 
    job-name:
       runs-on: [self-hosted, type-cpx21]
 
+-------------
 ARM64 Runners
-==============
+-------------
 
 The default, the server type is **cx11**, which is an Intel, 1 vCPU, 2GB RAM shared-cpu x64 instance.
 Therefore, in order to use ARM64 runners you must specify ARM64 server instance type by using the **type-{name}** runner label.
 The **{name}** must be a valid `ARM64 Hetzner Cloud server type <https://www.hetzner.com/cloud>`_
 name such as *cax11*, *cax21* etc. which correspond to the Ampere Altra, 2 vCPU, 4GB RAM and
 4 vCPU, 8GB RAM shared-cpu ARM64 instances respectively.
 
@@ -259,19 +448,17 @@
 as follows:
 
 .. code-block:: yaml
 
    job-name:
       runs-on: [self-hosted, type-cax21]
 
-----
-
----------------------------
+==========================
 Specifying Runner Location
----------------------------
+==========================
 
 By default, the default location of the server where the runner will be running is not specified. You can use the **--default-location**
 option to force specific default server location.
 
 You can also use the **in-{name}** runner label to specify server location for a specific job. Where **{name}** must be a valid
 `Hetzner Cloud location <https://docs.hetzner.com/cloud/general/locations/>`_ name such as *ash* for US, Ashburn, VA or
 *fsn1* for Germany, Falkenstein.
@@ -279,19 +466,17 @@
 For example,
 
 .. code-block:: yaml
 
    job-name:
       runs-on: [self-hosted, type-cx11, in-ash]
 
-----
-
------------------------
+=======================
 Specifying Runner Image
------------------------
+=======================
 
 By default, the default image of the server for the runner is **ubuntu-22.04**. You can use the **--default-image**
 option to force specific default server image.
 
 You can also use the **image-{architecture}-{type}-{name}** runner label to specify server image for a specific job.
 
 Where,
@@ -323,19 +508,17 @@
    must be unique.
 
    .. code-block:: yaml
 
       job-name:
          runs-on: [self-hosted, type-cx11, in-ash, image-x86-snapshot-snapshot_description]
 
-----
-
---------------------------------------------
+============================================
 Specifying Custom Runner Server Setup Script
---------------------------------------------
+============================================
 
 You can specify custom runner server setup script using the **--setup-script** option.
 
 For example,
 
 :custom_setup.sh:
    .. code-block:: bash
@@ -355,19 +538,17 @@
       apt-get -y install ca-certificates curl gnupg lsb-release python3-pip git unzip
 
 :command:
    .. code-block:: bash
 
       github-runners --setup-script ./custom_setup.sh
 
-----
-
---------------------------
+==========================
 Specifying Standby Runners
---------------------------
+==========================
 
 You can define standby runner groups to be always ready to pick your jobs using a custom configuration file.
 
 :✋ Note:
    Standby runner groups can only be defined using a configuration file.
    See `Using Configuration File`_ for more details.
 
@@ -401,19 +582,17 @@
                   labels=["type-cx21"],
                   count=2,
                   replenish_immediately=True,
             )
          ],
       )
 
-----
-
--------------------------------
+===============================
 Specifying Logger Configuration
--------------------------------
+===============================
 
 You can specify custom logger configuration using a configuration file.
 
 :✋ Note:
    Custom logger configuration can only be specified using a configuration file.
    See `Using Configuration File`_ for more details.
 
@@ -447,19 +626,17 @@
              },
              "loggers": {
                  "testflows.github.runners": {"level": "INFO", "handlers": ["default"]},
              },
          }
      )
 
-----
-
---------------------------------------
+======================================
 Deleting All Runners And Their Servers
---------------------------------------
+======================================
 
 You can delete all runners, including standby runners, and their servers using the **delete** command.
 
 :✋ Note:
    The **delete** command will not delete cloud service server. If you also want to delete it,
    you also need to execute **cloud delete** command. For more information, see `Deleting Cloud Service`_ section.
 
@@ -471,19 +648,17 @@
 
    07/29/2023 07:43:16 PM     INFO       MainThread             all 🍀 Logging in to Hetzner Cloud
    07/29/2023 07:43:16 PM     INFO       MainThread             all 🍀 Logging in to GitHub
    07/29/2023 07:43:16 PM     INFO       MainThread             all 🍀 Getting repository testflows/testflows-github-runners
    07/29/2023 07:43:17 PM     INFO       MainThread             all 🍀 Getting list of self-hosted runners
    07/29/2023 07:43:17 PM     INFO       MainThread             all 🍀 Getting list of servers
 
-----
-
-------------------------
+========================
 Using Configuration File
-------------------------
+========================
 
 Instead of passing configuration options using command line arguments, you can use
 configuration file. The configuration file is Python file that must define the **config**
 object of the `Config class`_.
 
 :✋ Note:
    When you mix command line options and custom configuration file,
@@ -528,16 +703,17 @@
 
 You can pass your custom configuration file using the **-c path, --config path** command line option.
 
 .. code-block:: bash
 
    github-runners -c config.py
 
+--------------------
 Configuration Schema
-=====================
+--------------------
 
 The `Config class`_ has the following schema:
 
 :schema:
    * **github_token: str**
    * **github_repository: str**
    * **hetzner_token: str**
@@ -566,59 +742,56 @@
          * **location: location**
          * **setup_script: path**
    * **standby_runners: list[standby_runner]**
       * **labels: list[str]**
       * **count: count**
       * **replenish_immediately: bool**
 
-----
-
--------
-SSH Key
--------
+==================
+Specifying SSH Key
+==================
 
 All server instances that are created are accessed via SSH using the **ssh** utility and therefore you must provide a valid SSH key
 using the **--ssh-key** option. If the **--ssh-key** option is no specified, then the *~/.ssh/id_rsa.pub* default key path will be used.
 
 The SSH key will be automatically added to your project using the MD5 hash of the public key as the SSH key name.
 
 :❗Warning:
    Given that each new SSH key is automatically added to your Hetzner project, you must manually delete them when no longer needed.
 
 Most GitHub users already have an SSH key associated with the account. If you want to know how to add an SSH key, see `Adding a new SSH key to your GitHub account    <https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account>`_ article.
 
+----------------------
 Generating New SSH Key
-=======================
+----------------------
 
 If you need to generate a new SSH key, see `Generating a new SSH key and adding it to the ssh-agent <https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent>`_ article.
 
-Cloud Deployment
-================
+----------------------------
+SSH Keys in Cloud Deployment
+----------------------------
 
 If you are deploying the **github-runners** program as a cloud service using the **github-runners <options> cloud deploy** command, then
 after provisoning a new cloud server instance that will host the **github-runners** service, a new SSH key will be
 auto-generated to access the runners. The auto-generated key will be placed in */home/runner/.ssh/id_rsa*, where **runner**
 is the user under which the **github-runners** service runs on the cloud instance. The auto-generated SSH key will be automatically
 added to your project using the MD5 hash of the public key as the SSH key name.
 
-----
-
------------------------
+====================
 Running as a Service
------------------------
+====================
 
 You can run **github-runners** as a service.
 
 :✋ Note:
    In order to install the service, the user that installed the module must have **sudo** privileges.
 
-----
-
+---------------------------
 Installing and Uninstalling
-===========================
+---------------------------
 
 After installation, you can use **service install** and **service uninstall** commands to install and
 uninstall the service.
 
 :✋ Note:
    The options that are passed to the **github-runners <options> service install** command
    will be the same options with which the service will be executed.
@@ -652,34 +825,32 @@
       Environment=GITHUB_TOKEN=ghp_...
       Environment=GITHUB_REPOSITORY=testflows/github-runners
       Environment=HETZNER_TOKEN=GJ..
       ExecStart=/home/user/.local/lib/python3.10/site-packages/testflows/github/runners/bin/github-runners --workers 10 --max-powered-off-time 20 --max-unused-runner-time 120 --max-runner-registration-time 60 --scale-up-interval 10 --scale-down-interval 10
       [Install]
       WantedBy=multi-user.target
 
-----
-
+-------------------------
 Modifying Program Options
-=========================
+-------------------------
 
 If you want to modify service program options you can stop the service,
 edit the **/etc/systemd/system/github-runners.service** file by hand, then reload service daemon,
 and start the service back up.
 
 .. code-block:: bash
 
    github-runners service stop
    sudo vim /etc/systemd/system/github-runners.service
    sudo systemctl daemon-reload
    github-runners service start
 
-----
-
+---------------
 Checking Status
-================
+---------------
 
 After installation, you can check the status of the service using the **service status** command.
 
 .. code-block:: bash
 
    github-runners service status:
 
@@ -701,18 +872,17 @@
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Logging in to Hetzner >
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Logging in to GitHub
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Getting repository vza>
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Creating scale up serv>
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Creating scale down se>
       lines 1-16/16 (END)
 
-----
-
+---------------------
 Manual Start and Stop
-=====================
+---------------------
 
 You can start and stop the service using the **service start** and **service stop** commands as follows:
 
 .. code-block:: bash
 
    github-runners service start
    github-runners service stop
@@ -720,18 +890,17 @@
 or using **service** system utility
 
 .. code-block:: bash
 
    sudo service github-runners start
    sudo service github-runners stop
 
-----
-
+-------------
 Checking Logs
-=============
+-------------
 
 You can get the logs for the service using the **service logs** command.
 
 Use **-f, --follow** option to follow logs journal.
 
 .. code-block:: bash
 
@@ -774,19 +943,17 @@
       Jul 24 14:24:42 user-node env[62771]: LANGUAGE=en_CA:en
       Jul 24 14:24:42 user-node env[62771]: PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/snap/bin
       Jul 24 14:24:42 user-node env[62771]: INVOCATION_ID=dc7b778f95fa4ccf95e4a4592b50d9e1
       Jul 24 14:24:42 user-node env[62771]: JOURNAL_STREAM=8:328542
       Jul 24 14:24:42 user-node env[62771]: SYSTEMD_EXEC_PID=62771
       ...
 
-----
-
---------------------------
+==========================
 Running as a Cloud Service
---------------------------
+==========================
 
 Instead of running **github-runners** program locally as a standalone application or as a service.
 You can easily deploy **github-runners** to run on a Hetzner Cloud instance.
 
 See **-h, --help** for all the available commands.
 
 :✋ Note:
@@ -794,18 +961,17 @@
    is **github-runners**. If you want to use a custom server name, then
    you must use the **cloud --name** option for any **cloud** commands.
 
 .. code-block:: bash
 
    github-runners cloud -h
 
-----
-
-Deployment
-==========
+---------
+Deploying
+---------
 
 You can deploy **github-runners** as a service to a new Hetzner Cloud server instance, that will be created for you automatically,
 using the **cloud deploy** command.
 
 :✋ Note:
    The options that are passed to the **github-runners <options> cloud deploy** command
    will be the same options with which the service will be executed.
@@ -864,15 +1030,15 @@
 
    github-runners deploy --location nbg1 --type cx11 --image ubuntu-22.04
 
 The cloud instance that runs the **github-runners** service can either be x64 or ARM64 instance. By default, **cpx11**
 AMD, 2 vCPU, 2GB RAM, shared-cpu x64 instance type is used.
 
 Using ARM64 Instance
-++++++++++++++++++++
+====================
 
 If you want to deploy the **github-runners** service to an ARM64 instance, then you must specify the instance
 type using the **--type** option.
 
 :✋ Note:
    Currently Hetzner Cloud has ARM64 instances only available in Germany, Falkenstein (**fsn1**) location.
 
@@ -880,41 +1046,39 @@
 as the value of the **--type** as follows:
 
 .. code-block:: bash
 
    github-runners deploy --location fsn1 --type cax21 --image ubuntu-22.04
 
 Using x64 Instance
-++++++++++++++++++
+==================
 
 By default, the **cpx11** AMD, 2 vCPU, 2GB RAM, shared-cpu x64 instance type is used. If you want to use
 a different x64 instance then specify desired type using the **--type** option.
 
-----
-
+-------------------------
 Redeploying Cloud Service
-=========================
+-------------------------
 
 You can change cloud service configuration or cloud service package version without deleting the existing cloud service server
 using the **cloud redeploy** command.
 
 .. code-block:: bash
 
    github-runners <options> cloud redeploy
 
 :✋ Note:
    The options that are passed to the **github-runners <options> cloud redeploy** command
    will be the same options with which the service will be executed.
 
 You can specify the version of the package to be installed using the **--version** option.
 
-----
-
+------------------
 Cloud Service Logs
-===================
+------------------
 
 You can check logs for the **github-runners** service running on a cloud instance using the **github-runners cloud logs** command.
 Specify **-f, --follow** if you want to follow the logs journal.
 
 For example,
 
 :dump the full log:
@@ -925,54 +1089,50 @@
 
 :follow the logs journal:
 
    .. code-block:: bash
 
       github-runners cloud logs -f
 
-----
-
+--------------------
 Cloud Service Status
-=====================
+--------------------
 
 You can check the status of the **github-runners** service running on a cloud instance using the **github-runners cloud status** command.
 
 For example,
 
 .. code-block:: bash
 
    github-runners cloud status
 
-----
-
+----------------------
 Stopping Cloud Service
-======================
+----------------------
 
 You can manually stop the **github-runners** service running on a cloud instance using the **github-runners cloud stop** command.
 
 .. code-block:: bash
 
    github-runners cloud stop
 
-----
-
+----------------------
 Starting Cloud Service
-======================
+----------------------
 
 You can manually start the **github-runners** service running on a cloud instance after it was being manually stopped
 using the **github-runners cloud start** command.
 
 .. code-block:: bash
 
    github-runners cloud start
 
-----
-
+------------------------
 Installing Cloud Service
-========================
+------------------------
 
 You can manually force installation of the **github-runners** service running on a cloud instance using
 the **github-runners cloud install** command.
 
 :✋ Note:
    Just like with the `github-runners <options> service install` command,
    the options that are passed to the `github-runners <options> cloud install` command
@@ -980,30 +1140,28 @@
 
 You can specify **-f, --force** option to force service re-installation if it is already installed.
 
 .. code-block:: bash
 
    github-runners <options> cloud install -f
 
-----
-
+--------------------------
 Uninstalling Cloud Service
-==========================
+--------------------------
 
 You can manually force uninstallation of the **github-runners** service running on a cloud instance using
 the **github-runners cloud uninstall** command.
 
 .. code-block:: bash
 
    github-runners cloud uninstall
 
-----
-
+-------------------------------
 Upgrading Cloud Service Package
-===============================
+-------------------------------
 
 You can manually upgrade the **github-runners** service package running on a cloud instance using
 the **github-runners cloud upgrade** command.
 
 If specific '--version' is specified then the *testflows.github.runners* package is upgraded to
 the specified version otherwise the version is upgraded to the latest available.
 
@@ -1015,18 +1173,17 @@
 .. code-block:: bash
 
    github-runners cloud upgrade --version <version>
 
 The service is not re-installed during the package upgrade process.
 Instead, it is stopped before the upgrade and then started back up
 
-----
-
+------------------------------
 Changing Cloud Service Options
-==============================
+------------------------------
 
 If you need to change cloud service options such as the **--setup-script** or the **--max-runners** etc.,
 you can keep the existing server and use **cloud redeploy** command.
 
 .. code-block:: bash
 
    github-runners <options> cloud redeploy --version latest
@@ -1041,18 +1198,17 @@
    github-runners <options> cloud deploy --version latest
 
 :✋ Note:
    Complete teardown will not affect any current jobs as the service is designed to
    be restartable. However, some servers might be left in an unfinished state
    but they will be cleaned up when the service is restarted.
 
-----
-
+----------------------
 Deleting Cloud Service
-======================
+----------------------
 
 You can delete the **github-runners** cloud service and the cloud instance that is running on using
 the **github-runners cloud delete** command.
 
 The **cloud delete** command, deletes the cloud service by first stopping the service and then deleting the server instance.
 
 :❗Warning:
@@ -1067,18 +1223,17 @@
       github-runners cloud delete
 
 :custom name:
    .. code-block:: bash
 
       github-runners cloud --name <custom_name> delete
 
-----
-
+-----------------------
 SSH in to Cloud Service
-==============================
+-----------------------
 
 You can open SSH client to the cloud service using the **cloud ssh** command. For example,
 
 .. code-block:: bash
 
    github-runners cloud ssh
 
@@ -1091,19 +1246,17 @@
 
 The output will contain the full **ssh** command including the IP address of the cloud service server.
 
 ::
 
    ssh -q -o "StrictHostKeyChecking no" root@5.161.87.21
 
-----
-
-------------------
+==================
 Scaling Up Runners
-------------------
+==================
 
 The program scales up runners by looking for any jobs that have **queued** status.
 For each such job, a corresponding Hetzner Cloud server instance is created with the following name:
 
 ::
 
    github-runner-{job.id}
@@ -1120,30 +1273,28 @@
 Also,
 
 :Note:
    There is no guarantee that a given runner will pick the job with the exact **job.id** that caused it to be created.
    This is expected and because for each **queued** job a unique runner will be created the number of runners will be
    equal the number of jobs and therefore under normal conditions all jobs will be executed as expected.
 
-----
-
+-------------------------
 Maximum Number of Runners
-=========================
+-------------------------
 
 By default, the maximum number of runners and therefore the maximum number of server instances is not set and therefore is unlimited.
 You can set the maximum number of runners using the **--max-runners** option.
 
 .. code-blocks::bash
 
    github-runners --max-runners 10
 
-----
-
+----------
 New Server
-==========
+----------
 
 The new server is accessed using SSH. It boots up with the specified OS image and is configured using
 the **setup** and **startup** scripts.
 
 :Server Type:
 
    The default server type is **cx11** which is an Intel, 1 vCPU, 2GB RAM shared-cpu x64 instance.
@@ -1173,18 +1324,17 @@
 
    The server is configured to be accessed using *ssh* utility and the SSH public key path is specified using the **--ssh-key**
    option.
 
 :Image Configuration:
    Each new server instance is configured using the `setup <#the-setup-script>`_ and the `startup <#the-start-up-script>`_ scripts.
 
-----
-
+----------------
 The Setup Script
-================
+----------------
 
 The **setup** script creates and configures **runner** user that has **sudo** privileges.
 
 :Setup:
 
    .. code-block:: bash
 
@@ -1194,18 +1344,17 @@
 
         adduser ubuntu --disabled-password --gecos ""
         echo "%wheel   ALL=(ALL:ALL) NOPASSWD:ALL" >> /etc/sudoers
         addgroup wheel
         usermod -aG wheel ubuntu
         usermod -aG sudo ubuntu
 
-----
-
+-------------------
 The Start-up Script
-===================
+-------------------
 
 The **startup** script installs GitHub Actions runner. After installation it configures the runner to start in an *--ephemeral* mode.
 The *--ephemeral* mode causes the runner to exit as soon as it completes a job. After the runner exits the server is powered off.
 
 :✋ Note:
    The **startup** script is executed as **ubuntu** user and therefore you must use **sudo** for any commands that need *root* privileges.
 
@@ -1245,50 +1394,49 @@
 
      echo "Configure runner"
      ./config.sh --unattended --replace --url https://github.com/${GITHUB_REPOSITORY} --token ${GITHUB_RUNNER_TOKEN} --name "$(hostname)" --runnergroup "${GITHUB_RUNNER_GROUP}" --labels "${GITHUB_RUNNER_LABELS}" --work _work --ephemeral
 
      echo "Start runner"
      bash -c "screen -d -m bash -c './run.sh; sudo poweroff'"
 
-----
-
---------------------
+====================
 Scaling Down Runners
---------------------
+====================
 
+-------------------
 Powered Off Servers
-===================
+-------------------
 
 The program scales down runners by first cleaning up powered off servers. The scale down service relies on the fact
 that the `startup <#the-start-up-script>`_ script starts an ephemeral runner which will pick up only 1 job and then will power itself off after the job is complete.
 
 The powered off servers are deleted after the **max-powered-off-time** interval which
 can be specified using the **--max-powered-off-time** option which by default is set to *20* sec.
 
+--------------
 Unused Runners
-==============
+--------------
 
 The scale down service also monitors all the runners that have **unused** status and tries to delete any servers associated with such
 runners if the runner is **unused** for more than the **max-unused-runner-time** period. This is needed in case a runner never gets a job
 assigned to it and the server will stay in the power on state. This cycle relies on the fact that the runner's name
 is the same as server's name. The **max-unused-runner-time** can be specified using the **--max-unused-runner-time** option which by default
 is set to *120* sec.
 
+--------------
 Zombie Servers
-==============
+--------------
 
 The scale down service will delete any zombie servers. A zombie server is defined as as any server that fails to register its runner within
 the **max-runner-registration-time**. The **max-runner-registration-time** can be specified using the **--max-runner-registration-time** option
 which by default is set to *60* sec.
 
-----
-
----------------------------
+===========================
 Handling Failing Conditions
----------------------------
+===========================
 
 The program is designed to handle the following failing conditions:
 
 :Server Never Registers a Runner:
    The server will remain in **running** state and should be reclaimed by the scale down service when it checks the actual runners registered for current servers.
    If it finds a server that is **running** but no runner is active for it it will be deleted after the **max-runner-registration-time** period.
 
@@ -1303,19 +1451,17 @@
 
 :Runner Never Gets a Job Assigned:
    If the runner never gets a job assigned, then the scale down service will remove the runner and delete its server after the **max-unused-runner-time** period.
 
 :Runner Created With a Mismatched Labels:
    The behavior will be the same as for the **Runner Never Gets a Job Assigned** case above.
 
-----
-
----------------
+===============
 Program Options
----------------
+===============
 
 The following options are supported:
 
 * **-h, --help**
   show this help message and exit
 
 * **-v, --version**
@@ -1491,16 +1637,16 @@
 
       * **start**
         start service
 
       * **stop**
         stop service
 
------------------
+=================
 Table of Contents
------------------
+=================
 
-.. contents:: Index:
+.. contents::
    :backlinks: top
    :depth: 4
 
 .. _Config class: https://github.com/testflows/TestFlows-GitHub-Runners/blob/main/testflows/github/runners/config.py#L45
```

### Comparing `testflows.github.runners-1.3.230731.1173142/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.3.230731.1223345/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

