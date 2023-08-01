# Comparing `tmp/ape-infura-0.6.2.tar.gz` & `tmp/ape-infura-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-infura-0.6.2.tar", last modified: Tue Jun 13 01:44:20 2023, max compression
+gzip compressed data, was "ape-infura-0.6.3.tar", last modified: Tue Aug  1 15:08:01 2023, max compression
```

## Comparing `ape-infura-0.6.2.tar` & `ape-infura-0.6.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:44:20.780394 ape-infura-0.6.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:44:20.780394 ape-infura-0.6.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:44:20.780394 ape-infura-0.6.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-13 01:42:49.000000 ape-infura-0.6.2/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-13 01:42:49.000000 ape-infura-0.6.2/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-13 01:42:49.000000 ape-infura-0.6.2/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-13 01:42:49.000000 ape-infura-0.6.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-13 01:42:49.000000 ape-infura-0.6.2/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:44:20.780394 ape-infura-0.6.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-13 01:42:49.000000 ape-infura-0.6.2/.github/workflows/commit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-13 01:42:49.000000 ape-infura-0.6.2/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 01:42:49.000000 ape-infura-0.6.2/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-13 01:42:49.000000 ape-infura-0.6.2/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-13 01:42:49.000000 ape-infura-0.6.2/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-13 01:42:49.000000 ape-infura-0.6.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 01:42:49.000000 ape-infura-0.6.2/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-13 01:42:49.000000 ape-infura-0.6.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-13 01:42:49.000000 ape-infura-0.6.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-13 01:42:49.000000 ape-infura-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-13 01:44:20.780394 ape-infura-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-13 01:42:49.000000 ape-infura-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:44:20.780394 ape-infura-0.6.2/ape_infura/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-13 01:42:49.000000 ape-infura-0.6.2/ape_infura/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-13 01:42:49.000000 ape-infura-0.6.2/ape_infura/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 01:42:49.000000 ape-infura-0.6.2/ape_infura/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 01:44:20.000000 ape-infura-0.6.2/ape_infura/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:44:20.780394 ape-infura-0.6.2/ape_infura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-13 01:44:20.000000 ape-infura-0.6.2/ape_infura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-13 01:44:20.000000 ape-infura-0.6.2/ape_infura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 01:44:20.000000 ape-infura-0.6.2/ape_infura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 01:44:20.000000 ape-infura-0.6.2/ape_infura.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-13 01:44:20.000000 ape-infura-0.6.2/ape_infura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-13 01:44:20.000000 ape-infura-0.6.2/ape_infura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-13 01:42:49.000000 ape-infura-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-13 01:44:20.784394 ape-infura-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-06-13 01:42:49.000000 ape-infura-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:44:20.780394 ape-infura-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 01:42:49.000000 ape-infura-0.6.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-13 01:42:49.000000 ape-infura-0.6.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-13 01:42:49.000000 ape-infura-0.6.2/tests/test_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:08:01.485396 ape-infura-0.6.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:08:01.485396 ape-infura-0.6.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:08:01.485396 ape-infura-0.6.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-01 15:06:29.000000 ape-infura-0.6.3/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-08-01 15:06:29.000000 ape-infura-0.6.3/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-01 15:06:29.000000 ape-infura-0.6.3/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-08-01 15:06:29.000000 ape-infura-0.6.3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-01 15:06:29.000000 ape-infura-0.6.3/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:08:01.485396 ape-infura-0.6.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-01 15:06:29.000000 ape-infura-0.6.3/.github/workflows/commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-01 15:06:29.000000 ape-infura-0.6.3/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-01 15:06:29.000000 ape-infura-0.6.3/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-01 15:06:29.000000 ape-infura-0.6.3/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-08-01 15:06:29.000000 ape-infura-0.6.3/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-08-01 15:06:29.000000 ape-infura-0.6.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-01 15:06:29.000000 ape-infura-0.6.3/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-01 15:06:29.000000 ape-infura-0.6.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-08-01 15:06:29.000000 ape-infura-0.6.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-08-01 15:06:29.000000 ape-infura-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-08-01 15:08:01.485396 ape-infura-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-08-01 15:06:29.000000 ape-infura-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:08:01.485396 ape-infura-0.6.3/ape_infura/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-01 15:06:29.000000 ape-infura-0.6.3/ape_infura/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-08-01 15:06:29.000000 ape-infura-0.6.3/ape_infura/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:29.000000 ape-infura-0.6.3/ape_infura/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-01 15:08:00.000000 ape-infura-0.6.3/ape_infura/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:08:01.485396 ape-infura-0.6.3/ape_infura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-08-01 15:08:01.000000 ape-infura-0.6.3/ape_infura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-08-01 15:08:01.000000 ape-infura-0.6.3/ape_infura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 15:08:01.000000 ape-infura-0.6.3/ape_infura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 15:08:01.000000 ape-infura-0.6.3/ape_infura.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-08-01 15:08:01.000000 ape-infura-0.6.3/ape_infura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 15:08:01.000000 ape-infura-0.6.3/ape_infura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-01 15:06:29.000000 ape-infura-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-01 15:08:01.485396 ape-infura-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-08-01 15:06:29.000000 ape-infura-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:08:01.485396 ape-infura-0.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:06:29.000000 ape-infura-0.6.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-08-01 15:06:29.000000 ape-infura-0.6.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-01 15:06:29.000000 ape-infura-0.6.3/tests/test_provider.py
```

### Comparing `ape-infura-0.6.2/.github/ISSUE_TEMPLATE/bug.md` & `ape-infura-0.6.3/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-infura-0.6.2/.github/ISSUE_TEMPLATE/feature.md` & `ape-infura-0.6.3/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-infura-0.6.2/.github/ISSUE_TEMPLATE/work-item.md` & `ape-infura-0.6.3/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-infura-0.6.2/.github/release-drafter.yml` & `ape-infura-0.6.3/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-infura-0.6.2/.github/workflows/commit.yaml` & `ape-infura-0.6.3/.github/workflows/commit.yaml`

 * *Files identical despite different names*

### Comparing `ape-infura-0.6.2/.github/workflows/prtitle.yaml` & `ape-infura-0.6.3/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-infura-0.6.2/.github/workflows/publish.yaml` & `ape-infura-0.6.3/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-infura-0.6.2/.github/workflows/test.yaml` & `ape-infura-0.6.3/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ape-infura-0.6.2/.gitignore` & `ape-infura-0.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-infura-0.6.2/.pre-commit-config.yaml` & `ape-infura-0.6.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-infura-0.6.2/CONTRIBUTING.md` & `ape-infura-0.6.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-infura-0.6.2/LICENSE` & `ape-infura-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-infura-0.6.2/PKG-INFO` & `ape-infura-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-infura
-Version: 0.6.2
+Version: 0.6.3
 Summary: ape-infura: Infura Provider plugins for Ethereum-based networks
 Home-page: https://github.com/ApeWorX/ape-infura
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -32,14 +32,15 @@
 Use the [Infura](https://infura.io/) provider plugin to interact with blockchains via APIs.
 This plugin supports the following ecosystems:
 
 - Ethereum
 - Polygon
 - Arbitrum
 - Optimism
+- Linea
 
 ## Dependencies
 
 - [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
 
 ## Installation
```

### Comparing `ape-infura-0.6.2/README.md` & `ape-infura-0.6.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Use the [Infura](https://infura.io/) provider plugin to interact with blockchains via APIs.
 This plugin supports the following ecosystems:
 
 - Ethereum
 - Polygon
 - Arbitrum
 - Optimism
+- Linea
 
 ## Dependencies
 
 - [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
 
 ## Installation
```

### Comparing `ape-infura-0.6.2/ape_infura/__init__.py` & `ape-infura-0.6.3/ape_infura/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,14 +16,18 @@
         "mainnet",
         "goerli",
     ],
     "polygon": [
         "mainnet",
         "mumbai",
     ],
+    "linea": [
+        "mainnet",
+        "goerli",
+    ],
 }
 
 
 @plugins.register(plugins.ProviderPlugin)
 def providers():
     for ecosystem_name in NETWORKS:
         for network_name in NETWORKS[ecosystem_name]:
```

### Comparing `ape-infura-0.6.2/ape_infura/provider.py` & `ape-infura-0.6.3/ape_infura/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,16 +55,17 @@
     def connect(self):
         self._web3 = Web3(HTTPProvider(self.uri))
 
         # Any chain that *began* as PoA needs the middleware for pre-merge blocks
         ethereum_goerli = 5
         optimism = (10, 420)
         polygon = (137, 80001)
+        linea = (59144, 59140)
 
-        if self._web3.eth.chain_id in (ethereum_goerli, *optimism, *polygon):
+        if self._web3.eth.chain_id in (ethereum_goerli, *optimism, *polygon, *linea):
             self._web3.middleware_onion.inject(geth_poa_middleware, layer=0)
 
         self._web3.eth.set_gas_price_strategy(rpc_gas_price_strategy)
 
     def disconnect(self):
         self._web3 = None
```

### Comparing `ape-infura-0.6.2/ape_infura.egg-info/PKG-INFO` & `ape-infura-0.6.3/ape_infura.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-infura
-Version: 0.6.2
+Version: 0.6.3
 Summary: ape-infura: Infura Provider plugins for Ethereum-based networks
 Home-page: https://github.com/ApeWorX/ape-infura
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -32,14 +32,15 @@
 Use the [Infura](https://infura.io/) provider plugin to interact with blockchains via APIs.
 This plugin supports the following ecosystems:
 
 - Ethereum
 - Polygon
 - Arbitrum
 - Optimism
+- Linea
 
 ## Dependencies
 
 - [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
 
 ## Installation
```

### Comparing `ape-infura-0.6.2/ape_infura.egg-info/SOURCES.txt` & `ape-infura-0.6.3/ape_infura.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-infura-0.6.2/ape_infura.egg-info/requires.txt` & `ape-infura-0.6.3/ape_infura.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 pytest>=6.0
 pytest-xdist
 pytest-cov
 hypothesis<7.0,>=6.2.0
 ape-arbitrum
 ape-optimism
 ape-polygon
+ape-linea
 black<24,>=23.3.0
 mypy<1,>=0.991
 flake8<7,>=6.0.0
 isort<6,>=5.10.1
 types-setuptools
 mdformat>=0.7.16
 mdformat-gfm>=0.3.5
@@ -54,7 +55,8 @@
 pytest>=6.0
 pytest-xdist
 pytest-cov
 hypothesis<7.0,>=6.2.0
 ape-arbitrum
 ape-optimism
 ape-polygon
+ape-linea
```

### Comparing `ape-infura-0.6.2/pyproject.toml` & `ape-infura-0.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-infura-0.6.2/setup.py` & `ape-infura-0.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
         "pytest>=6.0",  # Core testing package
         "pytest-xdist",  # multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "hypothesis>=6.2.0,<7.0",  # Strategy-based fuzzer
         "ape-arbitrum",
         "ape-optimism",
         "ape-polygon",
+        "ape-linea",
     ],
     "lint": [
         "black>=23.3.0,<24",  # auto-formatter and linter
         "mypy>=0.991,<1",  # Static type analyzer
         "flake8>=6.0.0,<7",  # Style linter
         "isort>=5.10.1,<6",  # Import sorting linter
         "types-setuptools",  # Needed due to mypy typeshed
```

### Comparing `ape-infura-0.6.2/tests/test_provider.py` & `ape-infura-0.6.3/tests/test_provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,16 @@
         ("ethereum", "sepolia"),
         ("arbitrum", "mainnet"),
         ("arbitrum", "goerli"),
         ("optimism", "mainnet"),
         ("optimism", "goerli"),
         ("polygon", "mainnet"),
         ("polygon", "mumbai"),
+        ("linea", "mainnet"),
+        ("linea", "goerli"),
     ],
 )
 def test_infura(ecosystem, network):
     ecosystem_cls = networks.get_ecosystem(ecosystem)
     network_cls = ecosystem_cls.get_network(network)
     with network_cls.use_provider("infura") as provider:
         assert isinstance(provider, Infura)
```

