# Comparing `tmp/ape-etherscan-0.6.7.tar.gz` & `tmp/ape-etherscan-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-etherscan-0.6.7.tar", last modified: Tue Jun 20 00:43:37 2023, max compression
+gzip compressed data, was "ape-etherscan-0.6.8.tar", last modified: Tue Aug  1 15:29:17 2023, max compression
```

## Comparing `ape-etherscan-0.6.7.tar` & `ape-etherscan-0.6.8.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:43:37.871966 ape-etherscan-0.6.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:43:37.867966 ape-etherscan-0.6.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:43:37.867966 ape-etherscan-0.6.7/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:43:37.867966 ape-etherscan-0.6.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/.github/workflows/commit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-20 00:43:37.871966 ape-etherscan-0.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:43:37.867966 ape-etherscan-0.6.7/ape_etherscan/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/ape_etherscan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13354 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/ape_etherscan/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/ape_etherscan/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/ape_etherscan/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/ape_etherscan/explorer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/ape_etherscan/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/ape_etherscan/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/ape_etherscan/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/ape_etherscan/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12584 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/ape_etherscan/verify.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-20 00:43:37.000000 ape-etherscan-0.6.7/ape_etherscan/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:43:37.867966 ape-etherscan-0.6.7/ape_etherscan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-20 00:43:37.000000 ape-etherscan-0.6.7/ape_etherscan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-20 00:43:37.000000 ape-etherscan-0.6.7/ape_etherscan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 00:43:37.000000 ape-etherscan-0.6.7/ape_etherscan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 00:43:37.000000 ape-etherscan-0.6.7/ape_etherscan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-20 00:43:37.000000 ape-etherscan-0.6.7/ape_etherscan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-20 00:43:37.000000 ape-etherscan-0.6.7/ape_etherscan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-20 00:43:37.871966 ape-etherscan-0.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:43:37.867966 ape-etherscan-0.6.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15418 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:43:37.871966 ape-etherscan-0.6.7/tests/mock_responses/
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/tests/mock_responses/get_account_transactions.json
--rw-r--r--   0 runner    (1001) docker     (123)    85181 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/tests/mock_responses/get_contract_response.json
--rw-r--r--   0 runner    (1001) docker     (123)    93453 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/tests/mock_responses/get_proxy_contract_response.json
--rw-r--r--   0 runner    (1001) docker     (123)    93483 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/tests/mock_responses/get_vyper_contract_response.json
--rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-06-20 00:42:22.000000 ape-etherscan-0.6.7/tests/test_etherscan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:29:17.228869 ape-etherscan-0.6.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:29:17.224869 ape-etherscan-0.6.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:29:17.224869 ape-etherscan-0.6.8/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:29:17.228869 ape-etherscan-0.6.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/.github/workflows/commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-08-01 15:29:17.228869 ape-etherscan-0.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:29:17.228869 ape-etherscan-0.6.8/ape_etherscan/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/ape_etherscan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13604 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/ape_etherscan/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/ape_etherscan/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/ape_etherscan/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/ape_etherscan/explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/ape_etherscan/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/ape_etherscan/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/ape_etherscan/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/ape_etherscan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14899 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/ape_etherscan/verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-01 15:29:16.000000 ape-etherscan-0.6.8/ape_etherscan/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:29:17.228869 ape-etherscan-0.6.8/ape_etherscan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-08-01 15:29:17.000000 ape-etherscan-0.6.8/ape_etherscan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-08-01 15:29:17.000000 ape-etherscan-0.6.8/ape_etherscan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 15:29:17.000000 ape-etherscan-0.6.8/ape_etherscan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 15:29:17.000000 ape-etherscan-0.6.8/ape_etherscan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-08-01 15:29:17.000000 ape-etherscan-0.6.8/ape_etherscan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-01 15:29:17.000000 ape-etherscan-0.6.8/ape_etherscan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-01 15:29:17.232869 ape-etherscan-0.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:29:17.228869 ape-etherscan-0.6.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17694 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:29:17.228869 ape-etherscan-0.6.8/tests/mock_responses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/tests/mock_responses/get_account_transactions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/tests/mock_responses/get_account_transactions_with_ctor_args.json
+-rw-r--r--   0 runner    (1001) docker     (123)    85181 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/tests/mock_responses/get_contract_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)    93453 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/tests/mock_responses/get_proxy_contract_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)    93483 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/tests/mock_responses/get_vyper_contract_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9359 2023-08-01 15:28:15.000000 ape-etherscan-0.6.8/tests/test_etherscan.py
```

### Comparing `ape-etherscan-0.6.7/.github/ISSUE_TEMPLATE/bug.md` & `ape-etherscan-0.6.8/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.7/.github/ISSUE_TEMPLATE/feature.md` & `ape-etherscan-0.6.8/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.7/.github/ISSUE_TEMPLATE/work-item.md` & `ape-etherscan-0.6.8/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.7/.github/release-drafter.yml` & `ape-etherscan-0.6.8/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.7/.github/workflows/codeql.yml` & `ape-etherscan-0.6.8/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.7/.github/workflows/commit.yaml` & `ape-etherscan-0.6.8/.github/workflows/commit.yaml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.7/.github/workflows/prtitle.yaml` & `ape-etherscan-0.6.8/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.7/.github/workflows/publish.yaml` & `ape-etherscan-0.6.8/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.7/.github/workflows/stale-prs.yml` & `ape-etherscan-0.6.8/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.7/.github/workflows/test.yaml` & `ape-etherscan-0.6.8/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.7/.gitignore` & `ape-etherscan-0.6.8/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.7/.pre-commit-config.yaml` & `ape-etherscan-0.6.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.7/CONTRIBUTING.md` & `ape-etherscan-0.6.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.7/LICENSE` & `ape-etherscan-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.7/PKG-INFO` & `ape-etherscan-0.6.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-etherscan
-Version: 0.6.7
+Version: 0.6.8
 Summary: ape-etherscan: Etherscan Explorer Plugin for Ethereum-based networks
 Home-page: https://github.com/ApeWorX/ape-etherscan
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -135,8 +135,11 @@
 ```python
 from ape import networks
 
 etherscan = networks.provider.network.explorer
 etherscan.publish_contract("0x55a8a39bc9694714e2874c1ce77aa1e599461e18")
 ```
 
+Not every network's explorer supports multi-file verification.
+For those networks, the corresponding compiler plugin's `flatten` functionality is invoked, in order to verify the contract as a single file.
+
 **NOTE**: You must set an Etherscan API key environment variable to use the publishing feature.
```

### Comparing `ape-etherscan-0.6.7/README.md` & `ape-etherscan-0.6.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -106,8 +106,11 @@
 ```python
 from ape import networks
 
 etherscan = networks.provider.network.explorer
 etherscan.publish_contract("0x55a8a39bc9694714e2874c1ce77aa1e599461e18")
 ```
 
+Not every network's explorer supports multi-file verification.
+For those networks, the corresponding compiler plugin's `flatten` functionality is invoked, in order to verify the contract as a single file.
+
 **NOTE**: You must set an Etherscan API key environment variable to use the publishing feature.
```

### Comparing `ape-etherscan-0.6.7/ape_etherscan/__init__.py` & `ape-etherscan-0.6.8/ape_etherscan/__init__.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.7/ape_etherscan/client.py` & `ape-etherscan-0.6.8/ape_etherscan/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -295,27 +295,34 @@
         libraries = libraries or {}
         if len(libraries) > 10:
             raise ValueError(f"Can only have up to 10 libraries (received {len(libraries)}).")
 
         if not compiler_version.startswith("v"):
             compiler_version = f"v{compiler_version}"
 
+        if "sourceCode" in standard_json_output:
+            source_code = standard_json_output["sourceCode"]
+            code_format = "solidity-single-file"
+        else:
+            source_code = StringIO(json.dumps(standard_json_output))
+            code_format = "solidity-standard-json-input"
+
         json_dict = {
             **self.base_params,
             "action": "verifysourcecode",
-            "codeformat": "solidity-standard-json-input",
+            "codeformat": code_format,
             "compilerversion": compiler_version,
             "constructorArguements": constructor_arguments,
             "contractaddress": self._address,
             "contractname": contract_name,
             "evmversion": evm_version,
             "licenseType": license_type,
             "optimizationUsed": int(optimization_used),
             "runs": optimization_runs,
-            "sourceCode": StringIO(json.dumps(standard_json_output)),
+            "sourceCode": source_code,
         }
         iterator = 1
         for lib_address, lib_name in libraries.items():
             json_dict[f"libraryname{iterator}"] = lib_name
             json_dict[f"libraryaddress{iterator}"] = lib_address
             iterator += 1
```

### Comparing `ape-etherscan-0.6.7/ape_etherscan/config.py` & `ape-etherscan-0.6.8/ape_etherscan/config.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.7/ape_etherscan/exceptions.py` & `ape-etherscan-0.6.8/ape_etherscan/exceptions.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.7/ape_etherscan/explorer.py` & `ape-etherscan-0.6.8/ape_etherscan/explorer.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.7/ape_etherscan/query.py` & `ape-etherscan-0.6.8/ape_etherscan/query.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.7/ape_etherscan/types.py` & `ape-etherscan-0.6.8/ape_etherscan/types.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.7/ape_etherscan/utils.py` & `ape-etherscan-0.6.8/ape_etherscan/utils.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.7/ape_etherscan/verify.py` & `ape-etherscan-0.6.8/ape_etherscan/verify.py`

 * *Files 22% similar despite different names*

```diff
@@ -29,14 +29,16 @@
     "agpl-3.0": 13,
     "agpl-3.0-only": 13,
     "agpl-3.0-later": 13,
     "busl-1.1": 14,
 }
 _SPDX_ID_KEY = "SPDX-License-Identifier: "
 
+ECOSYSTEMS_VERIFY_USING_JSON = ("ethereum",)
+
 
 class LicenseType(Enum):
     """
     https://etherscan.io/contract-license-types
     """
 
     NO_LICENSE = 1
@@ -192,20 +194,20 @@
 
         if not deploy_receipt:
             raise ContractVerificationError(
                 f"Failed to find to deploy receipt for '{self.address}'"
             )
 
         runtime_bytecode = self._contract_type.runtime_bytecode
-        bytecode_len = 0
         if runtime_bytecode:
-            bytecode_len = len(runtime_bytecode.bytecode or "")
-
-        start_index = bytecode_len
-        return deploy_receipt["input"][start_index:]
+            return extract_constructor_arguments(
+                deploy_receipt["input"], runtime_bytecode.bytecode or ""
+            )
+        else:
+            raise ContractVerificationError("Failed to find runtime bytecode.")
 
     @cached_property
     def license_code(self) -> LicenseType:
         """
         The license type used in the code.
         """
 
@@ -262,21 +264,27 @@
 
         if logger.level == LogLevel.DEBUG:
             logger.debug("Dumping standard JSON output:\n")
             standard_json = json.dumps(standard_input_json, indent=2)
             logger.debug(f"{standard_json}\n")
 
         # NOTE: Etherscan does not allow directory prefixes on the source ID.
-        request_source_id = Path(source_id).name
+        if self.provider.network.ecosystem.name in ECOSYSTEMS_VERIFY_USING_JSON:
+            request_source_id = Path(source_id).name
+            contract_name = f"{request_source_id}:{self._contract_type.name}"
+        else:
+            # When we have a flattened contract, we don't need to specify the file name
+            # only the contract name
+            contract_name = f"{self._contract_type.name}"
 
         try:
             guid = self._contract_client.verify_source_code(
                 standard_input_json,
                 str(version),
-                contract_name=f"{request_source_id}:{self._contract_type.name}",
+                contract_name=contract_name,
                 optimization_used=optimized,
                 optimization_runs=runs,
                 constructor_arguments=self.constructor_arguments,
                 evm_version=evm_version,
                 license_type=license_code_value,
             )
         except EtherscanResponseError as err:
@@ -302,26 +310,41 @@
             source_imports = compiler.get_imports([_source_path]).get(_source_id, [])
             for imported_source_id in source_imports:
                 sources[imported_source_id] = {
                     "content": (base_dir / imported_source_id).read_text()
                 }
                 build_map(imported_source_id)
 
+        def flatten_source(_source_id: str) -> str:
+            _source_path = base_dir / _source_id
+            flattened_source = str(compiler.flatten_contract(_source_path))
+            return flattened_source
+
         build_map(source_id)
 
         # "libraries" field not allows in `settings` dict.
         if "libraries" in settings:
             # libraries are handled below.
             settings.pop("libraries")
 
-        data = {
-            "language": compiler.name.capitalize(),
-            "sources": sources,
-            "settings": settings,
-        }
+        if self.provider.network.ecosystem.name in ECOSYSTEMS_VERIFY_USING_JSON:
+            # Use standard input json format
+            data = {
+                "language": compiler.name.capitalize(),
+                "sources": sources,
+                "settings": settings,
+            }
+        else:
+            # Use flattened source, single-file approach
+            data = {
+                "language": compiler.name.capitalize(),
+                "sourceCode": flatten_source(source_id),
+                "settings": settings,
+            }
+
         if hasattr(compiler, "libraries") and compiler.libraries:
             libraries = compiler.libraries
             index = 1
             max_libraries = 10
             for _, library in libraries.items():
                 for name, address in library.items():
                     if index > max_libraries:
@@ -374,7 +397,37 @@
 
             status_message = f"Contract verification status: {verification_update}"
             logger.info(status_message)
             time.sleep(3)
 
         else:
             raise ContractVerificationError("Timed out waiting for contract verification.")
+
+
+def extract_constructor_arguments(deployment_bytecode: str, runtime_bytecode: str) -> str:
+    # Ensure the bytecodes are stripped of the "0x" prefix
+    deployment_bytecode = (
+        deployment_bytecode[2:] if deployment_bytecode.startswith("0x") else deployment_bytecode
+    )
+    runtime_bytecode = (
+        runtime_bytecode[2:] if runtime_bytecode.startswith("0x") else runtime_bytecode
+    )
+
+    if deployment_bytecode.endswith(runtime_bytecode):
+        # If the runtime bytecode is at the end of the deployment bytecode,
+        # there are no constructor arguments
+        return ""
+
+    # Find the start of the runtime bytecode within the deployment bytecode
+    start_index = deployment_bytecode.find(runtime_bytecode)
+
+    # If the runtime bytecode is not found within the deployment bytecode,
+    # return an error message
+    if start_index == -1:
+        raise ContractVerificationError("Runtime bytecode not found within deployment bytecode")
+
+    # Cut the deployment bytecode at the start of the runtime bytecode
+    # The remaining part is the constructor arguments
+    constructor_args_start_index = start_index + len(runtime_bytecode)
+    constructor_arguments = deployment_bytecode[constructor_args_start_index:]
+
+    return constructor_arguments
```

### Comparing `ape-etherscan-0.6.7/ape_etherscan.egg-info/PKG-INFO` & `ape-etherscan-0.6.8/ape_etherscan.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-etherscan
-Version: 0.6.7
+Version: 0.6.8
 Summary: ape-etherscan: Etherscan Explorer Plugin for Ethereum-based networks
 Home-page: https://github.com/ApeWorX/ape-etherscan
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -135,8 +135,11 @@
 ```python
 from ape import networks
 
 etherscan = networks.provider.network.explorer
 etherscan.publish_contract("0x55a8a39bc9694714e2874c1ce77aa1e599461e18")
 ```
 
+Not every network's explorer supports multi-file verification.
+For those networks, the corresponding compiler plugin's `flatten` functionality is invoked, in order to verify the contract as a single file.
+
 **NOTE**: You must set an Etherscan API key environment variable to use the publishing feature.
```

### Comparing `ape-etherscan-0.6.7/ape_etherscan.egg-info/SOURCES.txt` & `ape-etherscan-0.6.8/ape_etherscan.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -36,10 +36,11 @@
 ape_etherscan.egg-info/not-zip-safe
 ape_etherscan.egg-info/requires.txt
 ape_etherscan.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
 tests/test_etherscan.py
 tests/mock_responses/get_account_transactions.json
+tests/mock_responses/get_account_transactions_with_ctor_args.json
 tests/mock_responses/get_contract_response.json
 tests/mock_responses/get_proxy_contract_response.json
 tests/mock_responses/get_vyper_contract_response.json
```

### Comparing `ape-etherscan-0.6.7/ape_etherscan.egg-info/requires.txt` & `ape-etherscan-0.6.8/ape_etherscan.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.7/pyproject.toml` & `ape-etherscan-0.6.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.7/setup.py` & `ape-etherscan-0.6.8/setup.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.7/tests/conftest.py` & `ape-etherscan-0.6.8/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -55,14 +55,21 @@
 }
 
 contract foo {
     function register(uint value) public {
         require(MyLib.insert(value));
     }
 }
+
+contract fooWithConstructor {
+    uint public value;
+    constructor(uint _value) {
+        value = _value;
+    }
+}
 """
 BAR_SOURCE_CODE = r"""
 // SPDX-License-Identifier: AGPL-3.0
 pragma solidity ^0.8.20;
 
 contract bar {
 }
@@ -390,14 +397,32 @@
 
         with open(test_data_path) as response_data_file:
             response = self.get_mock_response(response_data_file, file_name=file_name)
             self.add_handler("GET", "account", params, return_value=response)
             self.set_network("ethereum", "mainnet")
             return response
 
+    def setup_mock_account_transactions_with_ctor_args_response(
+        self, address: Optional[AddressType] = None
+    ):
+        file_name = "get_account_transactions_with_ctor_args.json"
+        test_data_path = MOCK_RESPONSES_PATH / file_name
+
+        if address:
+            params = EXPECTED_ACCOUNT_TXNS_PARAMS.copy()
+            params["address"] = address
+        else:
+            params = EXPECTED_ACCOUNT_TXNS_PARAMS
+
+        with open(test_data_path) as response_data_file:
+            response = self.get_mock_response(response_data_file, file_name=file_name)
+            self.add_handler("GET", "account", params, return_value=response)
+            self.set_network("ethereum", "mainnet")
+            return response
+
     def get_mock_response(
         self, response_data: Optional[Union[IO, Dict, str, MagicMock]] = None, **kwargs
     ):
         if isinstance(response_data, str):
             return self.get_mock_response({"result": response_data})
 
         elif isinstance(response_data, _io.TextIOWrapper):
@@ -417,15 +442,15 @@
             setattr(response, key, val)
 
         return response
 
 
 @pytest.fixture
 def verification_params(address_to_verify):
-    ctor_args = "000000000000000000000000000000000000000000000000000000000000002833623465633162323163303133643932303665363338366532313839353566356166306565336362000000000000000000000000000000000000000000000000"  # noqa: E501
+    ctor_args = ""  # noqa: E501
 
     return {
         "action": "verifysourcecode",
         "codeformat": "solidity-standard-json-input",
         "constructorArguements": ctor_args,
         "contractaddress": address_to_verify,
         "contractname": "foo.sol:foo",
@@ -434,29 +459,74 @@
         "module": "contract",
         "optimizationUsed": 1,
         "runs": 200,
         "sourceCode": StringIO(json.dumps(STANDARD_INPUT_JSON)),
     }
 
 
+@pytest.fixture
+def verification_params_with_ctor_args(address_to_verify_with_ctor_args):
+    # abi-encoded representation of uint256 value 42
+    ctor_args = "000000000000000000000000000000000000000000000000000000000000002a"  # noqa: E501
+
+    json_data = STANDARD_INPUT_JSON.copy()
+    json_data["libraryaddress1"] = "0xF2Df0b975c0C9eFa2f8CA0491C2d1685104d2488"
+
+    return {
+        "action": "verifysourcecode",
+        "codeformat": "solidity-standard-json-input",
+        "constructorArguements": ctor_args,
+        "contractaddress": address_to_verify_with_ctor_args,
+        "contractname": "foo.sol:fooWithConstructor",
+        "evmversion": None,
+        "licenseType": 1,
+        "module": "contract",
+        "optimizationUsed": 1,
+        "runs": 200,
+        "sourceCode": StringIO(json.dumps(json_data)),
+    }
+
+
 @pytest.fixture(scope="session")
 def address_to_verify(fake_connection, project, account):
     # Deploy the library first.
     library = account.deploy(project.MyLib)
     ape.chain.contracts._local_contract_types[library.address] = library.contract_type
 
     # Add the library to recompile contract `foo`.
     solidity = project.compiler_manager.solidity
     solidity.add_library(library)
 
-    # Use foo address for verification.
     foo = project.foo.deploy(sender=account)
     ape.chain.contracts._local_contract_types[address] = foo.contract_type
     return foo.address
 
 
 @pytest.fixture(scope="session")
+def address_to_verify_with_ctor_args(fake_connection, project, account):
+    # Deploy the library first.
+    library = account.deploy(project.MyLib)
+    ape.chain.contracts._local_contract_types[library.address] = library.contract_type
+
+    # Add the library to recompile contract `foo`.
+    solidity = project.compiler_manager.solidity
+    solidity.add_library(library)
+
+    foo = project.fooWithConstructor.deploy(42, sender=account)
+    ape.chain.contracts._local_contract_types[address] = foo.contract_type
+    return foo.address
+
+
+@pytest.fixture(scope="session")
 def expected_verification_log(address_to_verify):
     return (
         "Contract verification successful!\n"
         f"https://etherscan.io/address/{address_to_verify}#code"
     )
+
+
+@pytest.fixture(scope="session")
+def expected_verification_log_with_ctor_args(address_to_verify_with_ctor_args):
+    return (
+        "Contract verification successful!\n"
+        f"https://etherscan.io/address/{address_to_verify_with_ctor_args}#code"
+    )
```

### Comparing `ape-etherscan-0.6.7/tests/mock_responses/get_contract_response.json` & `ape-etherscan-0.6.8/tests/mock_responses/get_contract_response.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.7/tests/mock_responses/get_proxy_contract_response.json` & `ape-etherscan-0.6.8/tests/mock_responses/get_proxy_contract_response.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.7/tests/mock_responses/get_vyper_contract_response.json` & `ape-etherscan-0.6.8/tests/mock_responses/get_vyper_contract_response.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.7/tests/test_etherscan.py` & `ape-etherscan-0.6.8/tests/test_etherscan.py`

 * *Files 12% similar despite different names*

```diff
@@ -98,14 +98,40 @@
             side_effect=verification_tester.sim,
         )
         return verification_tester
 
     return setup
 
 
+@pytest.fixture
+def setup_verification_test_with_ctor_args(
+    mock_backend,
+    verification_params_with_ctor_args,
+    verification_tester_cls,
+    address_to_verify_with_ctor_args,
+):
+    def setup(found_handler: Callable, threshold: int = 2):
+        mock_backend.setup_mock_account_transactions_with_ctor_args_response(
+            address=address_to_verify_with_ctor_args
+        )
+        mock_backend.add_handler(
+            "POST", "contract", verification_params_with_ctor_args, return_value=PUBLISH_GUID
+        )
+        verification_tester = verification_tester_cls(found_handler, threshold=threshold)
+        mock_backend.add_handler(
+            "GET",
+            "contract",
+            {"guid": PUBLISH_GUID},
+            side_effect=verification_tester.sim,
+        )
+        return verification_tester
+
+    return setup
+
+
 @base_url_test
 def test_get_address_url(ecosystem, network, url, address, get_explorer):
     expected = f"https://{url}/address/{address}"
     explorer = get_explorer(ecosystem, network)
     actual = explorer.get_address_url(address)
     assert actual == expected
 
@@ -208,7 +234,20 @@
 ):
     def raise_err():
         raise EtherscanResponseError(mocker.MagicMock(), "Resource not found")
 
     setup_verification_test(raise_err, threshold=1)
     explorer.publish_contract(address_to_verify)
     assert caplog.records[-1].message == expected_verification_log
+
+
+def test_publish_contract_with_ctor_args(
+    explorer,
+    address_to_verify_with_ctor_args,
+    setup_verification_test_with_ctor_args,
+    expected_verification_log_with_ctor_args,
+    caplog,
+    fake_connection,
+):
+    setup_verification_test_with_ctor_args(lambda: "Pass - You made it!")
+    explorer.publish_contract(address_to_verify_with_ctor_args)
+    assert caplog.records[-1].message == expected_verification_log_with_ctor_args
```

