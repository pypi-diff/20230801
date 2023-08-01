# Comparing `tmp/many_abis-0.1.7.tar.gz` & `tmp/many_abis-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "many_abis-0.1.7.tar", last modified: Sat Apr 22 05:36:07 2023, max compression
+gzip compressed data, was "many_abis-0.1.8.tar", last modified: Tue Aug  1 04:08:47 2023, max compression
```

## Comparing `many_abis-0.1.7.tar` & `many_abis-0.1.8.tar`

### file list

```diff
@@ -1,83 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.493439 many_abis-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-04-22 05:36:07.493439 many_abis-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-04-22 05:35:53.000000 many_abis-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.485439 many_abis-0.1.7/many_abis/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/abis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.485439 many_abis-0.1.7/many_abis/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.485439 many_abis-0.1.7/many_abis/assets/dex/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.485439 many_abis-0.1.7/many_abis/assets/dex/aave/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.485439 many_abis-0.1.7/many_abis/assets/dex/aave/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v1/atoken.abi
--rw-r--r--   0 runner    (1001) docker     (123)    22101 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v1/lending_pool.abi
--rw-r--r--   0 runner    (1001) docker     (123)    11612 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v1/lending_pool_addresses_provider.abi
--rw-r--r--   0 runner    (1001) docker     (123)    34411 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v1/lending_pool_core.abi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.489439 many_abis-0.1.7/many_abis/assets/dex/aave/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v2/collector.abi
--rw-r--r--   0 runner    (1001) docker     (123)    10795 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v2/incentives_controller.abi
--rw-r--r--   0 runner    (1001) docker     (123)    22079 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v2/lending_pool.abi
--rw-r--r--   0 runner    (1001) docker     (123)    34411 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v2/lending_pool_addresses_provider.abi
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v2/lending_pool_addresses_provider_registry.abi
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v2/lending_pool_collateral_manager.abi
--rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v2/lending_pool_configurator.abi
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v2/lending_rate_oracle.abi
--rw-r--r--   0 runner    (1001) docker     (123)    15658 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v2/pool_admin.abi
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v2/price_oracle.abi
--rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v2/protocal_data_provider.abi
--rw-r--r--   0 runner    (1001) docker     (123)    32705 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v2/ui_incentive_data_provider.abi
--rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v2/ui_pool_data_provider.abi
--rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v2/weth_gateway.abi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.485439 many_abis-0.1.7/many_abis/assets/dex/joe/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.489439 many_abis-0.1.7/many_abis/assets/dex/joe/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/joe/v2/factory.abi
--rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/joe/v2/pair.abi
--rw-r--r--   0 runner    (1001) docker     (123)    19626 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/joe/v2/router.abi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.485439 many_abis-0.1.7/many_abis/assets/dex/pancake/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.489439 many_abis-0.1.7/many_abis/assets/dex/pancake/v3/
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/pancake/v3/IPeriphery_payments_with_fee.abi
--rw-r--r--   0 runner    (1001) docker     (123)    30717 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/pancake/v3/master_chef_v3.abi
--rw-r--r--   0 runner    (1001) docker     (123)    24647 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/pancake/v3/non_fungible_position_manager.abi
--rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/pancake/v3/pool_v3.abi
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/pancake/v3/quoter.abi
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/pancake/v3/quoter_v2.abi
--rw-r--r--   0 runner    (1001) docker     (123)    12082 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/pancake/v3/router_v3.abi
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/pancake/v3/self_permit.abi
--rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/pancake/v3/staker.abi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.485439 many_abis-0.1.7/many_abis/assets/dex/uniswap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.489439 many_abis-0.1.7/many_abis/assets/dex/uniswap/bsc/
--rw-r--r--   0 runner    (1001) docker     (123)     9425 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/uniswap/bsc/router.abi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.489439 many_abis-0.1.7/many_abis/assets/dex/uniswap/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    32705 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/uniswap/v1/exchange.abi
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/uniswap/v1/factory.abi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.493439 many_abis-0.1.7/many_abis/assets/dex/uniswap/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/uniswap/v2/factory.abi
--rw-r--r--   0 runner    (1001) docker     (123)    13409 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/uniswap/v2/pair.abi
--rw-r--r--   0 runner    (1001) docker     (123)    19603 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/uniswap/v2/router.abi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.493439 many_abis-0.1.7/many_abis/assets/dex/uniswap/v3/
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/uniswap/v3/factory.abi
--rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/uniswap/v3/multicall.abi
--rw-r--r--   0 runner    (1001) docker     (123)    24310 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/uniswap/v3/non_fungible_position_manage.abi
--rw-r--r--   0 runner    (1001) docker     (123)    19610 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/uniswap/v3/pool.abi
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/uniswap/v3/quoter.abi
--rw-r--r--   0 runner    (1001) docker     (123)    11745 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/uniswap/v3/router.abi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.493439 many_abis-0.1.7/many_abis/assets/erc/
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/erc/ERC1155.abi
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/erc/ERC20.abi
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/erc/ERC721.abi
--rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/erc/ERC777.abi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.493439 many_abis-0.1.7/many_abis/assets/tokens/
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/tokens/weth9.abi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.493439 many_abis-0.1.7/many_abis/assets/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    21093 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/utils/chains.json
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/chains.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.485439 many_abis-0.1.7/many_abis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-04-22 05:36:07.000000 many_abis-0.1.7/many_abis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-22 05:36:07.000000 many_abis-0.1.7/many_abis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 05:36:07.000000 many_abis-0.1.7/many_abis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-22 05:36:07.000000 many_abis-0.1.7/many_abis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-22 05:36:07.000000 many_abis-0.1.7/many_abis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 05:36:07.493439 many_abis-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-22 05:35:53.000000 many_abis-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:08:47.372528 many_abis-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-08-01 04:08:47.372528 many_abis-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-08-01 04:08:35.000000 many_abis-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:08:47.368528 many_abis-0.1.8/many_abis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-08-01 04:08:47.000000 many_abis-0.1.8/many_abis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-01 04:08:47.000000 many_abis-0.1.8/many_abis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 04:08:47.000000 many_abis-0.1.8/many_abis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 04:08:47.000000 many_abis-0.1.8/many_abis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 04:08:47.000000 many_abis-0.1.8/many_abis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 04:08:47.372528 many_abis-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-08-01 04:08:35.000000 many_abis-0.1.8/setup.py
```

### Comparing `many_abis-0.1.7/PKG-INFO` & `many_abis-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: many_abis
-Version: 0.1.7
+Version: 0.1.8
 Summary: A simple way to get different DEXs abis for block chains.
 Home-page: https://github.com/ackness/many_abis
 Author: Yong
 Author-email: ackness8@gmail.com
 License: MIT
 Keywords: abi,dex,block chain,bsc,eth,matic,heco,kcc,pancakeswap,mdex,quickswap,uniswap,koffeeswap
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Many Abis
 
-![Version](https://img.shields.io/badge/many--abis-v0.1.7-green)
+![Version](https://img.shields.io/badge/many--abis-v0.1.8-green)
 ![Pypi](https://img.shields.io/pypi/dm/many-abis)
 
 ![GitHub Org's stars](https://img.shields.io/github/stars/ackness/many_abis?style=social)
 ![GitHub forks](https://img.shields.io/github/forks/ackness/many_abis?style=social)
 
 ---
```

### Comparing `many_abis-0.1.7/README.md` & `many_abis-0.1.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Many Abis
 
-![Version](https://img.shields.io/badge/many--abis-v0.1.7-green)
+![Version](https://img.shields.io/badge/many--abis-v0.1.8-green)
 ![Pypi](https://img.shields.io/pypi/dm/many-abis)
 
 ![GitHub Org's stars](https://img.shields.io/github/stars/ackness/many_abis?style=social)
 ![GitHub forks](https://img.shields.io/github/forks/ackness/many_abis?style=social)
 
 ---
```

### Comparing `many_abis-0.1.7/many_abis.egg-info/PKG-INFO` & `many_abis-0.1.8/many_abis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: many-abis
-Version: 0.1.7
+Version: 0.1.8
 Summary: A simple way to get different DEXs abis for block chains.
 Home-page: https://github.com/ackness/many_abis
 Author: Yong
 Author-email: ackness8@gmail.com
 License: MIT
 Keywords: abi,dex,block chain,bsc,eth,matic,heco,kcc,pancakeswap,mdex,quickswap,uniswap,koffeeswap
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Many Abis
 
-![Version](https://img.shields.io/badge/many--abis-v0.1.7-green)
+![Version](https://img.shields.io/badge/many--abis-v0.1.8-green)
 ![Pypi](https://img.shields.io/pypi/dm/many-abis)
 
 ![GitHub Org's stars](https://img.shields.io/github/stars/ackness/many_abis?style=social)
 ![GitHub forks](https://img.shields.io/github/forks/ackness/many_abis?style=social)
 
 ---
```

### Comparing `many_abis-0.1.7/setup.py` & `many_abis-0.1.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
-# print(find_packages())
+
 setup(
     name='many_abis',
-    packages=['many_abis'],
+    # packages=['many_abis'],
+    packages=find_packages(where="many_abis"),
     package_dir={'many_abis': 'many_abis'},
-    package_data={'': [
-        '**/*.abi', '**/*.json']},
-    version='0.1.7',
+    package_data={'': ["assets/*"]},
+    version='0.1.8',
     license='MIT',
     description='A simple way to get different DEXs abis for block chains.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Yong',
     author_email='ackness8@gmail.com',
     url='https://github.com/ackness/many_abis',
     keywords=['abi', 'dex', 'block chain', 'bsc', 'eth', 'matic', 'heco',
               'kcc', 'pancakeswap', 'mdex', 'quickswap', 'uniswap', 'koffeeswap'],
 
     install_requires=[
         "eth_utils",
         "addict"
     ],
+    python_requires='>=3.8',
 
 )
```

