# Comparing `tmp/sparglim-0.1.1.tar.gz` & `tmp/sparglim-0.1.2.tar.gz`

## Comparing `sparglim-0.1.1.tar` & `sparglim-0.1.2.tar`

### file list

```diff
@@ -1,73 +1,74 @@
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 sparglim-0.1.1/.dockerignore
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 sparglim-0.1.1/.editorconfig
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 sparglim-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 sparglim-0.1.1/RELEASE.md
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 sparglim-0.1.1/config-template.md
--rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 sparglim-0.1.1/config.md
--rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 sparglim-0.1.1/generate-config.sh
--rwxr-xr-x   0        0        0     1828 2020-02-02 00:00:00.000000 sparglim-0.1.1/generate_config_docs.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 sparglim-0.1.1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 sparglim-0.1.1/.github/workflows/lint.yml
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 sparglim-0.1.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 sparglim-0.1.1/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 sparglim-0.1.1/dev/docker/Dockerfile.jupyterlab-sparglim
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 sparglim-0.1.1/dev/docker/Dockerfile.sparglim-server
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 sparglim-0.1.1/dev/jupyter-sparglim-on-k8s/README.md
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 sparglim-0.1.1/dev/jupyter-sparglim-on-k8s/k8s/deployment.yaml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sparglim-0.1.1/dev/jupyter-sparglim-on-k8s/k8s/headless-service.yaml
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 sparglim-0.1.1/dev/jupyter-sparglim-on-k8s/k8s/lab-service.yaml
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 sparglim-0.1.1/dev/jupyter-sparglim-sc/README.md
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 sparglim-0.1.1/dev/jupyter-sparglim-sc/k8s/jupyter-sparglim/deployment.yaml
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 sparglim-0.1.1/dev/jupyter-sparglim-sc/k8s/jupyter-sparglim/lab-service.yaml
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.1/dev/jupyter-sparglim-sc/k8s/sparglim-server/connect-server-service.yaml
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 sparglim-0.1.1/dev/jupyter-sparglim-sc/k8s/sparglim-server/deployment.yaml
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.1/dev/jupyter-sparglim-sc/k8s/sparglim-server/headless-service.yaml
--rwxr-xr-x   0        0        0      236 2020-02-02 00:00:00.000000 sparglim-0.1.1/dev/scripts/reload.sh
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 sparglim-0.1.1/dev/sparglim-server/README.md
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.1/dev/sparglim-server/k8s/connect-server-service.yaml
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 sparglim-0.1.1/dev/sparglim-server/k8s/deployment.yaml
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.1/dev/sparglim-server/k8s/headless-service.yaml
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 sparglim-0.1.1/docker/Dockerfile.jupyterlab-sparglim
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 sparglim-0.1.1/docker/Dockerfile.sparglim-server
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 sparglim-0.1.1/examples/jupyter-sparglim-on-k8s/README.md
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 sparglim-0.1.1/examples/jupyter-sparglim-on-k8s/k8s/deployment.yaml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sparglim-0.1.1/examples/jupyter-sparglim-on-k8s/k8s/headless-service.yaml
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 sparglim-0.1.1/examples/jupyter-sparglim-on-k8s/k8s/lab-service.yaml
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 sparglim-0.1.1/examples/jupyter-sparglim-sc/README.md
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 sparglim-0.1.1/examples/jupyter-sparglim-sc/k8s/jupyter-sparglim/deployment.yaml
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 sparglim-0.1.1/examples/jupyter-sparglim-sc/k8s/jupyter-sparglim/lab-service.yaml
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.1/examples/jupyter-sparglim-sc/k8s/sparglim-server/connect-server-service.yaml
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 sparglim-0.1.1/examples/jupyter-sparglim-sc/k8s/sparglim-server/deployment.yaml
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.1/examples/jupyter-sparglim-sc/k8s/sparglim-server/headless-service.yaml
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 sparglim-0.1.1/examples/sparglim-server/README.md
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.1/examples/sparglim-server/k8s/connect-server-service.yaml
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 sparglim-0.1.1/examples/sparglim-server/k8s/deployment.yaml
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.1/examples/sparglim-server/k8s/headless-service.yaml
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 sparglim-0.1.1/sparglim/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 sparglim-0.1.1/sparglim/exceptions.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 sparglim-0.1.1/sparglim/log.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.1/sparglim/py.typed
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 sparglim-0.1.1/sparglim/utils.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 sparglim-0.1.1/sparglim/config/__init__.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 sparglim-0.1.1/sparglim/config/builder.py
--rw-r--r--   0        0        0    11844 2020-02-02 00:00:00.000000 sparglim-0.1.1/sparglim/config/configer.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 sparglim-0.1.1/sparglim/config/k8s.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 sparglim-0.1.1/sparglim/server/__init__.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 sparglim-0.1.1/sparglim/server/cli.py
--rw-r--r--   0        0        0     8921 2020-02-02 00:00:00.000000 sparglim-0.1.1/sparglim/server/daemon.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 sparglim-0.1.1/sparglim/server/tailer.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 sparglim-0.1.1/sparglim/sql/__init__.py
--rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 sparglim-0.1.1/sparglim/sql/magic.py
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 sparglim-0.1.1/tests/conftest.py
--rw-r--r--   0        0        0     9525 2020-02-02 00:00:00.000000 sparglim-0.1.1/tests/test_builder.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 sparglim-0.1.1/tests/test_daemon.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 sparglim-0.1.1/tests/test_magic.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 sparglim-0.1.1/tests/example/people.json
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 sparglim-0.1.1/tests/mock/sbin/entrypoint.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 sparglim-0.1.1/tests/mock/sbin/mock_spark_server.py
--rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 sparglim-0.1.1/tests/mock/sbin/start-connect-server.sh
--rw-r--r--   0        0        0    10147 2020-02-02 00:00:00.000000 sparglim-0.1.1/.gitignore
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 sparglim-0.1.1/LICENSE
--rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 sparglim-0.1.1/README.md
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 sparglim-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 sparglim-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 sparglim-0.1.2/.dockerignore
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 sparglim-0.1.2/.editorconfig
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 sparglim-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 sparglim-0.1.2/RELEASE.md
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 sparglim-0.1.2/config-template.md
+-rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 sparglim-0.1.2/config.md
+-rwxr-xr-x   0        0        0       69 2020-02-02 00:00:00.000000 sparglim-0.1.2/generate-config.sh
+-rwxr-xr-x   0        0        0     1828 2020-02-02 00:00:00.000000 sparglim-0.1.2/generate_config_docs.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 sparglim-0.1.2/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 sparglim-0.1.2/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 sparglim-0.1.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 sparglim-0.1.2/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 sparglim-0.1.2/dev/docker/Dockerfile.jupyterlab-sparglim
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 sparglim-0.1.2/dev/docker/Dockerfile.sparglim-server
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 sparglim-0.1.2/dev/jupyter-sparglim-on-k8s/README.md
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 sparglim-0.1.2/dev/jupyter-sparglim-on-k8s/k8s/deployment.yaml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sparglim-0.1.2/dev/jupyter-sparglim-on-k8s/k8s/headless-service.yaml
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 sparglim-0.1.2/dev/jupyter-sparglim-on-k8s/k8s/lab-service.yaml
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 sparglim-0.1.2/dev/jupyter-sparglim-sc/README.md
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 sparglim-0.1.2/dev/jupyter-sparglim-sc/k8s/jupyter-sparglim/deployment.yaml
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 sparglim-0.1.2/dev/jupyter-sparglim-sc/k8s/jupyter-sparglim/lab-service.yaml
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.2/dev/jupyter-sparglim-sc/k8s/sparglim-server/connect-server-service.yaml
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 sparglim-0.1.2/dev/jupyter-sparglim-sc/k8s/sparglim-server/deployment.yaml
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.2/dev/jupyter-sparglim-sc/k8s/sparglim-server/headless-service.yaml
+-rwxr-xr-x   0        0        0      236 2020-02-02 00:00:00.000000 sparglim-0.1.2/dev/scripts/reload.sh
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 sparglim-0.1.2/dev/sparglim-server/README.md
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.2/dev/sparglim-server/k8s/connect-server-service.yaml
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 sparglim-0.1.2/dev/sparglim-server/k8s/deployment.yaml
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.2/dev/sparglim-server/k8s/headless-service.yaml
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 sparglim-0.1.2/docker/Dockerfile.jupyterlab-sparglim
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 sparglim-0.1.2/docker/Dockerfile.sparglim-server
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 sparglim-0.1.2/docker/README.md
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 sparglim-0.1.2/examples/jupyter-sparglim-on-k8s/README.md
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 sparglim-0.1.2/examples/jupyter-sparglim-on-k8s/k8s/deployment.yaml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sparglim-0.1.2/examples/jupyter-sparglim-on-k8s/k8s/headless-service.yaml
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 sparglim-0.1.2/examples/jupyter-sparglim-on-k8s/k8s/lab-service.yaml
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 sparglim-0.1.2/examples/jupyter-sparglim-sc/README.md
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 sparglim-0.1.2/examples/jupyter-sparglim-sc/k8s/jupyter-sparglim/deployment.yaml
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 sparglim-0.1.2/examples/jupyter-sparglim-sc/k8s/jupyter-sparglim/lab-service.yaml
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.2/examples/jupyter-sparglim-sc/k8s/sparglim-server/connect-server-service.yaml
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 sparglim-0.1.2/examples/jupyter-sparglim-sc/k8s/sparglim-server/deployment.yaml
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.2/examples/jupyter-sparglim-sc/k8s/sparglim-server/headless-service.yaml
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 sparglim-0.1.2/examples/sparglim-server/README.md
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.2/examples/sparglim-server/k8s/connect-server-service.yaml
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 sparglim-0.1.2/examples/sparglim-server/k8s/deployment.yaml
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.2/examples/sparglim-server/k8s/headless-service.yaml
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 sparglim-0.1.2/sparglim/__init__.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sparglim-0.1.2/sparglim/exceptions.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 sparglim-0.1.2/sparglim/log.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.2/sparglim/py.typed
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 sparglim-0.1.2/sparglim/utils.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 sparglim-0.1.2/sparglim/config/__init__.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 sparglim-0.1.2/sparglim/config/builder.py
+-rw-r--r--   0        0        0    11573 2020-02-02 00:00:00.000000 sparglim-0.1.2/sparglim/config/configer.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 sparglim-0.1.2/sparglim/config/k8s.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 sparglim-0.1.2/sparglim/server/__init__.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 sparglim-0.1.2/sparglim/server/cli.py
+-rw-r--r--   0        0        0     8921 2020-02-02 00:00:00.000000 sparglim-0.1.2/sparglim/server/daemon.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 sparglim-0.1.2/sparglim/server/tailer.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 sparglim-0.1.2/sparglim/sql/__init__.py
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 sparglim-0.1.2/sparglim/sql/magic.py
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 sparglim-0.1.2/tests/conftest.py
+-rw-r--r--   0        0        0     9665 2020-02-02 00:00:00.000000 sparglim-0.1.2/tests/test_builder.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 sparglim-0.1.2/tests/test_daemon.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 sparglim-0.1.2/tests/test_magic.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 sparglim-0.1.2/tests/example/people.json
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 sparglim-0.1.2/tests/mock/sbin/entrypoint.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 sparglim-0.1.2/tests/mock/sbin/mock_spark_server.py
+-rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 sparglim-0.1.2/tests/mock/sbin/start-connect-server.sh
+-rw-r--r--   0        0        0    10147 2020-02-02 00:00:00.000000 sparglim-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 sparglim-0.1.2/LICENSE
+-rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 sparglim-0.1.2/README.md
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 sparglim-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6930 2020-02-02 00:00:00.000000 sparglim-0.1.2/PKG-INFO
```

### Comparing `sparglim-0.1.1/.pre-commit-config.yaml` & `sparglim-0.1.2/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 repos:
   # FIXME: This is slow and unreliable.
-  - repo: local
-    hooks:
-      - id: generate-config
-        name: Generate config
-        entry: ./generate-config.sh
-        language: system
-        verbose: true
+  # - repo: local
+  #   hooks:
+  #     - id: generate-config
+  #       name: Generate config
+  #       entry: ./generate-config.sh
+  #       language: system
+  #       verbose: true
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: end-of-file-fixer
       - id: check-case-conflict
       - id: check-executables-have-shebangs
```

### Comparing `sparglim-0.1.1/RELEASE.md` & `sparglim-0.1.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.1/config-template.md` & `sparglim-0.1.2/config-template.md`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.1/config.md` & `sparglim-0.1.2/config.md`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.1/generate_config_docs.py` & `sparglim-0.1.2/generate_config_docs.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.1/.github/workflows/publish.yml` & `sparglim-0.1.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.1/.github/workflows/python-package.yml` & `sparglim-0.1.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.1/dev/docker/Dockerfile.jupyterlab-sparglim` & `sparglim-0.1.2/dev/docker/Dockerfile.jupyterlab-sparglim`

 * *Files 10% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 
 COPY --chown=application:application ./ ./sparglim
 RUN pip install --no-cache-dir ./sparglim[all]
 
 ENTRYPOINT ["tini","--","jupyter-lab", "--ip=0.0.0.0", "--port=8888", "--no-browser", "--IdentityProvider.token=''"]
 EXPOSE 8888
 
-# docker build -t wh1isper/jupyterlab-sparglim:dev -f dev/docker/Dockerfile.jupyterlab-sparglim . && ./scripts/reload.sh
+# docker build -t wh1isper/jupyterlab-sparglim:dev -f dev/docker/Dockerfile.jupyterlab-sparglim .
```

### Comparing `sparglim-0.1.1/dev/jupyter-sparglim-on-k8s/k8s/deployment.yaml` & `sparglim-0.1.2/dev/jupyter-sparglim-on-k8s/k8s/deployment.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.1/dev/jupyter-sparglim-sc/README.md` & `sparglim-0.1.2/dev/jupyter-sparglim-sc/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 This is development verification for [examples/jupyter-sparglim-sc](../../examples/jupyter-sparglim-sc)
 
 Use  [docker/Dockerfile.jupyterlab-sparglim](../docker/Dockerfile.jupyterlab-sparglim) and [docker/Dockerfile.sparglim-server](../docker/Dockerfile.sparglim-server)  and to build a dev version `jupyterlab-sparglim` and  `sparglim-server`
 
-```
+```bash
 # In project root dir
 docker build -t wh1isper/jupyterlab-sparglim:dev -f dev/docker/Dockerfile.jupyterlab-sparglim .
 docker build -t wh1isper/sparglim-server:dev -f dev/docker/Dockerfile.sparglim-server .
 
+# apply yaml
+kubectl apply -f dev/jupyter-sparglim-sc/k8s/jupyter-sparglim
+kubectl apply -f dev/jupyter-sparglim-sc/k8s/sparglim-server
 
 # reload by deleting deployment pod
 ./dev/scripts/reload.sh
 ```
```

### Comparing `sparglim-0.1.1/dev/jupyter-sparglim-sc/k8s/jupyter-sparglim/deployment.yaml` & `sparglim-0.1.2/dev/jupyter-sparglim-sc/k8s/jupyter-sparglim/deployment.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.1/dev/jupyter-sparglim-sc/k8s/sparglim-server/deployment.yaml` & `sparglim-0.1.2/dev/jupyter-sparglim-sc/k8s/sparglim-server/deployment.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.1/dev/sparglim-server/k8s/deployment.yaml` & `sparglim-0.1.2/dev/sparglim-server/k8s/deployment.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.1/examples/jupyter-sparglim-on-k8s/README.md` & `sparglim-0.1.2/examples/jupyter-sparglim-on-k8s/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -63,16 +63,15 @@
 
 ## SQL
 
 This will auto config SparkSession to `k8s` mode, via env `SPARGLIM_SQL_MODE`
 
 ```python
 %load_ext sparglim.sql
-from sparglim.config.builder import ConfigBuilder
-spark = ConfigBuilder().get_or_create() # No need to config_k8s(), ConfigBuilder is a Singleton
+spark
 ```
 
 Test it:
 
 ```python
 %sql SHOW TABLES;
 ```
```

### Comparing `sparglim-0.1.1/examples/jupyter-sparglim-on-k8s/k8s/deployment.yaml` & `sparglim-0.1.2/examples/jupyter-sparglim-on-k8s/k8s/deployment.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.1/examples/jupyter-sparglim-sc/README.md` & `sparglim-0.1.2/examples/jupyter-sparglim-sc/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -57,16 +57,15 @@
 
 ## SQL
 
 This will auto config SparkSession to `connect_client` mode, via env `SPARGLIM_SQL_MODE`
 
 ```python
 %load_ext sparglim.sql
-from sparglim.config.builder import ConfigBuilder
-spark = ConfigBuilder().get_or_create() # No need to config_connect_client(), ConfigBuilder is a Singleton
+spark
 ```
 
 Test it:
 
 ```python
 %sql SHOW TABLES
 ```
```

### Comparing `sparglim-0.1.1/examples/jupyter-sparglim-sc/k8s/jupyter-sparglim/deployment.yaml` & `sparglim-0.1.2/examples/jupyter-sparglim-sc/k8s/jupyter-sparglim/deployment.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.1/examples/jupyter-sparglim-sc/k8s/sparglim-server/deployment.yaml` & `sparglim-0.1.2/examples/jupyter-sparglim-sc/k8s/sparglim-server/deployment.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.1/examples/sparglim-server/README.md` & `sparglim-0.1.2/examples/sparglim-server/README.md`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.1/examples/sparglim-server/k8s/deployment.yaml` & `sparglim-0.1.2/examples/sparglim-server/k8s/deployment.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.1/sparglim/utils.py` & `sparglim-0.1.2/sparglim/utils.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.1/sparglim/config/builder.py` & `sparglim-0.1.2/sparglim/config/builder.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-from typing import Optional
+#  Copyright (c) 2023 Wh1isper
+#  Licensed under the BSD 3-Clause License
+from __future__ import annotations
+
+from typing import Any, Dict, Optional
 
 from pyspark import SparkConf
 from pyspark.sql import SparkSession
 
 from sparglim.config.configer import SparkEnvConfiger
-from sparglim.exceptions import UnconfigurableError
+from sparglim.exceptions import AlreadyConfiguredError, UnconfigurableError
 from sparglim.log import logger
 from sparglim.utils import Singleton
 
 
 class ConfigBuilder(SparkEnvConfiger, metaclass=Singleton):
     def __init__(self):
         super().__init__()
@@ -42,7 +46,16 @@
         return self._spark
 
     def set_runtime_conf(self, k, v):
         if not self._spark:
             raise UnconfigurableError("SparkSession not created yet")
         logger.info(f"Set runtime config: {k}={v}")
         self._spark.conf.set(k, v)
+
+    def config(self, c: Dict[str, Any]) -> ConfigBuilder:
+        try:
+            super().config(c)
+        except AlreadyConfiguredError:
+            raise AlreadyConfiguredError(
+                "ConfigBuilder already configured, try get_or_create() or clear()"
+            )
+        return self
```

### Comparing `sparglim-0.1.1/sparglim/config/configer.py` & `sparglim-0.1.2/sparglim/config/configer.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,30 +4,33 @@
 from __future__ import annotations
 
 import os
 from collections import UserDict
 from functools import wraps
 from typing import Any, Dict, Iterable, Literal, Optional, Tuple, Union
 
-from sparglim.exceptions import UnconfigurableError
+from kubernetes.config.incluster_config import SERVICE_TOKEN_FILENAME
+
+from sparglim.config.k8s import INCLUSTER, get_k8s_config, get_namespace
+from sparglim.exceptions import AlreadyConfiguredError, UnconfigurableError
 from sparglim.log import logger
 from sparglim.utils import get_host_ip
 
 ConfigEnvMapper = Dict[str, Tuple[Union[Iterable, str], Optional[str]]]
 
 
 class Config(UserDict):
     def __init__(self, dict=None, /, **kwargs):
         self.master_configured: bool = False
         super().__init__(dict, **kwargs)
 
     def __setitem__(self, key: Any, item: Any) -> None:
         will_config_master = key in ["spark.master", "spark.remote"]
         if self.master_configured and will_config_master:
-            raise UnconfigurableError("Spark master/remote already configured, try clear() first")
+            raise AlreadyConfiguredError("Spark master/remote already configured.")
         if will_config_master:
             self.master_configured = True
 
         return super().__setitem__(key, item)
 
     def pretty_format(self) -> str:
         lines = ["{"]
@@ -178,60 +181,48 @@
     def config(self, c: Dict[str, Any]) -> SparkEnvConfiger:
         self._merge_config(c)
         return self
 
     def config_s3(self, custom_config: Optional[Dict[str, Any]] = None) -> SparkEnvConfiger:
         if not custom_config:
             custom_config = dict()
-        self.config(
+        return self.config(
             {
                 **self._config_from_env(self._s3),
                 **custom_config,
             }
         )
-        return self
 
     def config_kerberos(self, custom_config: Optional[Dict[str, Any]] = None) -> SparkEnvConfiger:
         if not custom_config:
             custom_config = dict()
-        self.config(
+        return self.config(
             {
                 **self._config_from_env(self._kerberos),
                 **custom_config,
             }
         )
-        return self
 
     def config_local(self, custom_config: Optional[Dict[str, Any]] = None) -> SparkEnvConfiger:
         logger.info(f"Config master: local mode")
         if not custom_config:
             custom_config = dict()
-        self.config(
+        return self.config(
             {
                 **self._config_from_env(self._local),
                 **custom_config,
             }
         )
-        return self
 
     def config_k8s(
         self,
         custom_config: Optional[Dict[str, Any]] = None,
         *,
         k8s_config_path: Optional[str] = None,
     ) -> SparkEnvConfiger:
-        try:
-            from kubernetes.config.incluster_config import SERVICE_TOKEN_FILENAME
-
-            from sparglim.config.k8s import INCLUSTER, get_k8s_config, get_namespace
-        except ImportError:
-            raise UnconfigurableError(
-                "kubernetes is not installed, try install package `sparglim[k8s]`"
-            )
-
         logger.info(f"Config master: k8s mode")
         if not custom_config:
             custom_config = dict()
         env_config = self._config_from_env(self._k8s)
         if not env_config.get("spark.kubernetes.namespace"):
             env_config["spark.kubernetes.namespace"] = get_namespace()
         if INCLUSTER:
@@ -267,35 +258,33 @@
         k8s_config = {
             "spark.master": f"k8s://{url}",
             "spark.kubernetes.authenticate.caCertFile": ca,
             "spark.kubernetes.authenticate.clientKeyFile": key_file,
             "spark.kubernetes.authenticate.clientCertFile": cert_file,
         }
 
-        self.config(
+        return self.config(
             {
                 **env_config,
                 **k8s_config,
                 **custom_config,
             }
         )
-        return self
 
     def config_connect_client(
         self, custom_config: Optional[Dict[str, Any]] = None
     ) -> SparkEnvConfiger:
         if not custom_config:
             custom_config = dict()
-        self.config(
+        return self.config(
             {
                 **self._config_from_env(self._connect_client),
                 **custom_config,
             }
         )
-        return self
 
     def config_connect_server(
         self,
         mode: Optional[str] = None,
         custom_config: Optional[Dict[str, Any]] = None,
         *,
         k8s_config_path: Optional[str] = None,
@@ -310,9 +299,8 @@
             elif mode == "k8s":
                 self.config_k8s(custom_config, k8s_config_path=k8s_config_path)
             else:
                 raise UnconfigurableError(f"Unknown mode: {mode}")
         if k8s_config_path and mode != "k8s":
             logger.warning(f"k8s_config_path has no effort for mode: {mode}")
         logger.info(f"Config connect server")
-        self.config(self._config_from_env(self._connect_server))
-        return self
+        return self.config(self._config_from_env(self._connect_server))
```

### Comparing `sparglim-0.1.1/sparglim/config/k8s.py` & `sparglim-0.1.2/sparglim/config/k8s.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.1/sparglim/server/cli.py` & `sparglim-0.1.2/sparglim/server/cli.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.1/sparglim/server/daemon.py` & `sparglim-0.1.2/sparglim/server/daemon.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.1/sparglim/server/tailer.py` & `sparglim-0.1.2/sparglim/server/tailer.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.1/sparglim/sql/magic.py` & `sparglim-0.1.2/sparglim/sql/magic.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,32 +10,29 @@
 from sparglim.exceptions import UnconfigurableError
 from sparglim.log import logger
 
 
 @magics_class
 class SparkMagic(Magics):
     """
-    # Enable magic
+    # Enable magic, will initiliaze SparkSession as `spark`
 
         ```ipython
         %load_ext sparglim.sql
+        spark # show SparkSession brief info
         ```
 
     # Example:
 
         Init a table
 
         ```python
         from datetime import datetime, date
         from pyspark.sql import Row
 
-        from sparglim.config.builder import ConfigBuilder
-        spark = ConfigBuilder().get_or_create()
-
-
         df = spark.createDataFrame([
             Row(a=1, b=2., c='string1', d=date(2000, 1, 1), e=datetime(2000, 1, 1, 12, 0)),
             Row(a=2, b=3., c='string2', d=date(2000, 2, 1), e=datetime(2000, 1, 2, 12, 0)),
             Row(a=4, b=5., c='string3', d=date(2000, 3, 1), e=datetime(2000, 1, 3, 12, 0))
         ])
         df.show()
         df.createOrReplaceTempView("tb")
```

### Comparing `sparglim-0.1.1/tests/conftest.py` & `sparglim-0.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.1/tests/test_builder.py` & `sparglim-0.1.2/tests/test_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from datetime import date, datetime
 from typing import Dict
 
 import pytest
 from pyspark.sql import Row
 
 from sparglim.config.builder import ConfigBuilder
-from sparglim.exceptions import UnconfigurableError
+from sparglim.exceptions import AlreadyConfiguredError, UnconfigurableError
 
 
 @pytest.fixture
 def config_builder():
     c = ConfigBuilder()
     yield c
     c.clear()
@@ -56,16 +56,19 @@
         config_mode(k8s_config_path=k8s_config_path)
     else:
         config_mode()
     if mode != "connect_server":
         assert config_builder.master_configured
 
     if mode in ["local", "k8s"]:
-        with pytest.raises(UnconfigurableError) as e:
-            config_mode()
+        with pytest.raises(AlreadyConfiguredError) as e:
+            if mode == "k8s":
+                config_mode(k8s_config_path=k8s_config_path)
+            else:
+                config_mode()
 
 
 def test_merge(config_builder: ConfigBuilder):
     prev = config_builder.get_all().copy()
     to_merge = {"a": "b"}
     config_builder._merge_config(to_merge)
     assert config_builder.get_all() == {**prev, **to_merge}
```

### Comparing `sparglim-0.1.1/tests/test_daemon.py` & `sparglim-0.1.2/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.1/tests/test_magic.py` & `sparglim-0.1.2/tests/test_magic.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 example_file = os.path.join(_HERE, "example/people.json")
 
 
 ipy = get_ipython()
 ipy.run_line_magic("load_ext", "sparglim.sql")
 
 
+def test_spark_init():
+    ipy.run_cell("spark")
+
+
 def test_sql():
     ipy.run_line_magic("sql", "SHOW DATABASES")
 
 
 def test_line():
     ipy.run_line_magic("sql", f'CREATE TABLE tb_people USING json OPTIONS (path "{example_file}")')
```

### Comparing `sparglim-0.1.1/tests/mock/sbin/entrypoint.py` & `sparglim-0.1.2/tests/mock/sbin/entrypoint.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.1/tests/mock/sbin/mock_spark_server.py` & `sparglim-0.1.2/tests/mock/sbin/mock_spark_server.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.1/.gitignore` & `sparglim-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.1/LICENSE` & `sparglim-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.1/README.md` & `sparglim-0.1.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-![](https://img.shields.io/github/license/wh1isper/sparglim)
-![](https://img.shields.io/github/v/release/wh1isper/sparglim?logo=github)
-![](https://img.shields.io/github/v/release/wh1isper/sparglim?include_prereleases&label=pre-release&logo=github)
+![](https://github.com/Wh1isper/sparglim/actions/workflows/python-package.yml/badge.svg)
 ![](https://img.shields.io/pypi/dm/sparglim)
 ![](https://img.shields.io/github/last-commit/wh1isper/sparglim)
 ![](https://img.shields.io/pypi/pyversions/sparglim)
+![](https://img.shields.io/github/license/wh1isper/sparglim)
+![](https://img.shields.io/github/v/release/wh1isper/sparglim?logo=github)
+![](https://img.shields.io/github/v/release/wh1isper/sparglim?include_prereleases&label=pre-release&logo=github)
 
 # Sparglim ✨
 
 Sparglim is aimed at providing a clean solution for PySpark applications in cloud-native scenarios (On K8S、Connect Server etc.).
 
 **This is a fledgling project, looking forward to any PRs, Feature Requests and Discussions!**
 
@@ -43,30 +44,48 @@
 - Install only for config and daemon spark connect server `pip install sparglim`
 - Install for pyspark app `pip install sparglim[pyspark]`
 - Install for using magic within ipython/jupyter (will also install pyspark) `pip install sparglim[magic]`
 - **Install for all above** (such as using magic in jupyterlab on k8s) `pip install sparglim[all]`
 
 ## Feature
 
-- Config Spark via environment variables, see [config spark](./config.md)
+- [Config Spark via environment variables](./config.md)
 - `%SQL` and `%%SQL` magic for executing Spark SQL in IPython/Jupyter
   - SQL statement can be written in multiple lines, support using `;` to separate statements
   - Support config `connect client`, see [Spark Connect Overview](https://spark.apache.org/docs/latest/spark-connect-overview.html#spark-connect-overview)
   - *TODO: Visualize the result of SQL statement(Spark Dataframe)*
 - `sparglim-server` for daemon Spark Connect Server
 
 ## User cases
 
-### PySpark App
+### Basic
+
+```python
+from sparglim.config.builder import ConfigBuilder
+from datetime import datetime, date
+from pyspark.sql import Row
+
+# Create a local[*] spark session with s3&kerberos config
+spark = ConfigBuilder().get_or_create()
+
+df = spark.createDataFrame([
+    Row(a=1, b=2., c='string1', d=date(2000, 1, 1), e=datetime(2000, 1, 1, 12, 0)),
+    Row(a=2, b=3., c='string2', d=date(2000, 2, 1), e=datetime(2000, 1, 2, 12, 0)),
+    Row(a=4, b=5., c='string3', d=date(2000, 3, 1), e=datetime(2000, 1, 3, 12, 0))
+])
+df.show()
+```
+
+### Building a PySpark App
 
 To config Spark on k8s for Data explorations, see [examples/jupyter-sparglim-on-k8s](./examples/jupyter-sparglim-on-k8s)
 
-*TODO: To config Spark for ELT Application/Service, see [pyspark-sampling](https://github.com/Wh1isper/pyspark-sampling/)*
+To config Spark for ELT Application/Service, see project [pyspark-sampling](https://github.com/Wh1isper/pyspark-sampling/)
 
-### Spark Connect Server on K8S
+### Deploy Spark Connect Server on K8S (And Connect to it)
 
 To daemon Spark Connect Server on K8S, see [examples/sparglim-server](./examples/sparglim-server)
 
 To daemon Spark Connect Server on K8S and Connect it in JupyterLab , see [examples/jupyter-sparglim-sc](./examples/jupyter-sparglim-sc)
 
 ### Connect to Spark Connect Server
 
@@ -103,36 +122,29 @@
 pip install sparglim["magic"]
 ```
 
 Load magic in IPython/Jupyter
 
 ```ipython
 %load_ext sparglim.sql
+spark # show SparkSession brief info
 ```
 
 Create a view:
 
 ```python
-from sparglim.config.builder import ConfigBuilder
-
-
 from datetime import datetime, date
 from pyspark.sql import Row
 
-c: ConfigBuilder = ConfigBuilder()
-spark = c.get_or_create()
-
-
 df = spark.createDataFrame([
             Row(a=1, b=2., c='string1', d=date(2000, 1, 1), e=datetime(2000, 1, 1, 12, 0)),
             Row(a=2, b=3., c='string2', d=date(2000, 2, 1), e=datetime(2000, 1, 2, 12, 0)),
             Row(a=4, b=5., c='string3', d=date(2000, 3, 1), e=datetime(2000, 1, 3, 12, 0))
         ])
 df.createOrReplaceTempView("tb")
-
 ```
 
 Query the view by `%SQL`:
 
 ```ipython
 %sql SELECT * FROM tb
 ```
```

### Comparing `sparglim-0.1.1/pyproject.toml` & `sparglim-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.1/PKG-INFO` & `sparglim-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparglim
-Version: 0.1.1
+Version: 0.1.2
 Summary: sparglim
 Project-URL: Source, https://github.com/wh1isper/sparglim
 Author-email: wh1isper <9573586@qq.com>
 License: BSD license
 License-File: LICENSE
 Keywords: ipython,magic,pyspark,sparglim,spark
 Classifier: Programming Language :: Python :: 3
@@ -32,20 +32,21 @@
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest-timeout; extra == 'test'
 Requires-Dist: pytype; extra == 'test'
 Requires-Dist: sparglim[all]; extra == 'test'
 Description-Content-Type: text/markdown
 
-![](https://img.shields.io/github/license/wh1isper/sparglim)
-![](https://img.shields.io/github/v/release/wh1isper/sparglim?logo=github)
-![](https://img.shields.io/github/v/release/wh1isper/sparglim?include_prereleases&label=pre-release&logo=github)
+![](https://github.com/Wh1isper/sparglim/actions/workflows/python-package.yml/badge.svg)
 ![](https://img.shields.io/pypi/dm/sparglim)
 ![](https://img.shields.io/github/last-commit/wh1isper/sparglim)
 ![](https://img.shields.io/pypi/pyversions/sparglim)
+![](https://img.shields.io/github/license/wh1isper/sparglim)
+![](https://img.shields.io/github/v/release/wh1isper/sparglim?logo=github)
+![](https://img.shields.io/github/v/release/wh1isper/sparglim?include_prereleases&label=pre-release&logo=github)
 
 # Sparglim ✨
 
 Sparglim is aimed at providing a clean solution for PySpark applications in cloud-native scenarios (On K8S、Connect Server etc.).
 
 **This is a fledgling project, looking forward to any PRs, Feature Requests and Discussions!**
 
@@ -81,30 +82,48 @@
 - Install only for config and daemon spark connect server `pip install sparglim`
 - Install for pyspark app `pip install sparglim[pyspark]`
 - Install for using magic within ipython/jupyter (will also install pyspark) `pip install sparglim[magic]`
 - **Install for all above** (such as using magic in jupyterlab on k8s) `pip install sparglim[all]`
 
 ## Feature
 
-- Config Spark via environment variables, see [config spark](./config.md)
+- [Config Spark via environment variables](./config.md)
 - `%SQL` and `%%SQL` magic for executing Spark SQL in IPython/Jupyter
   - SQL statement can be written in multiple lines, support using `;` to separate statements
   - Support config `connect client`, see [Spark Connect Overview](https://spark.apache.org/docs/latest/spark-connect-overview.html#spark-connect-overview)
   - *TODO: Visualize the result of SQL statement(Spark Dataframe)*
 - `sparglim-server` for daemon Spark Connect Server
 
 ## User cases
 
-### PySpark App
+### Basic
+
+```python
+from sparglim.config.builder import ConfigBuilder
+from datetime import datetime, date
+from pyspark.sql import Row
+
+# Create a local[*] spark session with s3&kerberos config
+spark = ConfigBuilder().get_or_create()
+
+df = spark.createDataFrame([
+    Row(a=1, b=2., c='string1', d=date(2000, 1, 1), e=datetime(2000, 1, 1, 12, 0)),
+    Row(a=2, b=3., c='string2', d=date(2000, 2, 1), e=datetime(2000, 1, 2, 12, 0)),
+    Row(a=4, b=5., c='string3', d=date(2000, 3, 1), e=datetime(2000, 1, 3, 12, 0))
+])
+df.show()
+```
+
+### Building a PySpark App
 
 To config Spark on k8s for Data explorations, see [examples/jupyter-sparglim-on-k8s](./examples/jupyter-sparglim-on-k8s)
 
-*TODO: To config Spark for ELT Application/Service, see [pyspark-sampling](https://github.com/Wh1isper/pyspark-sampling/)*
+To config Spark for ELT Application/Service, see project [pyspark-sampling](https://github.com/Wh1isper/pyspark-sampling/)
 
-### Spark Connect Server on K8S
+### Deploy Spark Connect Server on K8S (And Connect to it)
 
 To daemon Spark Connect Server on K8S, see [examples/sparglim-server](./examples/sparglim-server)
 
 To daemon Spark Connect Server on K8S and Connect it in JupyterLab , see [examples/jupyter-sparglim-sc](./examples/jupyter-sparglim-sc)
 
 ### Connect to Spark Connect Server
 
@@ -141,36 +160,29 @@
 pip install sparglim["magic"]
 ```
 
 Load magic in IPython/Jupyter
 
 ```ipython
 %load_ext sparglim.sql
+spark # show SparkSession brief info
 ```
 
 Create a view:
 
 ```python
-from sparglim.config.builder import ConfigBuilder
-
-
 from datetime import datetime, date
 from pyspark.sql import Row
 
-c: ConfigBuilder = ConfigBuilder()
-spark = c.get_or_create()
-
-
 df = spark.createDataFrame([
             Row(a=1, b=2., c='string1', d=date(2000, 1, 1), e=datetime(2000, 1, 1, 12, 0)),
             Row(a=2, b=3., c='string2', d=date(2000, 2, 1), e=datetime(2000, 1, 2, 12, 0)),
             Row(a=4, b=5., c='string3', d=date(2000, 3, 1), e=datetime(2000, 1, 3, 12, 0))
         ])
 df.createOrReplaceTempView("tb")
-
 ```
 
 Query the view by `%SQL`:
 
 ```ipython
 %sql SELECT * FROM tb
 ```
```

