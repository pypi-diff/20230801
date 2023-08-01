# Comparing `tmp/binance-connector-3.1.1.tar.gz` & `tmp/binance-connector-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binance-connector-3.1.1.tar", last modified: Mon Jul  3 01:53:56 2023, max compression
+gzip compressed data, was "binance-connector-3.2.0.tar", last modified: Tue Aug  1 02:06:01 2023, max compression
```

## Comparing `binance-connector-3.1.1.tar` & `binance-connector-3.2.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:53:56.458161 binance-connector-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-03 01:53:50.000000 binance-connector-3.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-03 01:53:50.000000 binance-connector-3.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-07-03 01:53:56.458161 binance-connector-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10101 2023-07-03 01:53:50.000000 binance-connector-3.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:53:56.446161 binance-connector-3.1.1/binance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:53:56.446161 binance-connector-3.1.1/binance/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/lib/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/lib/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:53:56.454161 binance-connector-3.1.1/binance/spot/
--rw-r--r--   0 runner    (1001) docker     (123)    15170 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/spot/_blvt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/spot/_bswap.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/spot/_c2c.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/spot/_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/spot/_data_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/spot/_fiat.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/spot/_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/spot/_gift_card.py
--rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/spot/_loan.py
--rw-r--r--   0 runner    (1001) docker     (123)    33152 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/spot/_margin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/spot/_market.py
--rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/spot/_mining.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/spot/_nft.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/spot/_pay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/spot/_portfolio_margin.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/spot/_rebate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/spot/_savings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/spot/_staking.py
--rw-r--r--   0 runner    (1001) docker     (123)    30191 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/spot/_sub_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    14542 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/spot/_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)    16702 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/spot/_wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:53:56.454161 binance-connector-3.1.1/binance/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/websocket/binance_socket_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:53:56.454161 binance-connector-3.1.1/binance/websocket/spot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/websocket/spot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:53:56.454161 binance-connector-3.1.1/binance/websocket/spot/websocket_api/
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/websocket/spot/websocket_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14057 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/websocket/spot/websocket_api/_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    24597 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/websocket/spot/websocket_api/_market.py
--rw-r--r--   0 runner    (1001) docker     (123)    38486 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/websocket/spot/websocket_api/_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/websocket/spot/websocket_api/_user_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/websocket/spot/websocket_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-07-03 01:53:50.000000 binance-connector-3.1.1/binance/websocket/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:53:56.458161 binance-connector-3.1.1/binance_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-07-03 01:53:56.000000 binance-connector-3.1.1/binance_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-03 01:53:56.000000 binance-connector-3.1.1/binance_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 01:53:56.000000 binance-connector-3.1.1/binance_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-03 01:53:56.000000 binance-connector-3.1.1/binance_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-03 01:53:56.000000 binance-connector-3.1.1/binance_connector.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:53:56.458161 binance-connector-3.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 01:53:50.000000 binance-connector-3.1.1/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:53:56.458161 binance-connector-3.1.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-03 01:53:50.000000 binance-connector-3.1.1/requirements/common.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-03 01:53:56.458161 binance-connector-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-03 01:53:50.000000 binance-connector-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:06:01.646999 binance-connector-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-01 02:05:58.000000 binance-connector-3.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-01 02:05:58.000000 binance-connector-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-08-01 02:06:01.646999 binance-connector-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10101 2023-08-01 02:05:58.000000 binance-connector-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:06:01.634999 binance-connector-3.2.0/binance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:06:01.634999 binance-connector-3.2.0/binance/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/lib/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/lib/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:06:01.642999 binance-connector-3.2.0/binance/spot/
+-rw-r--r--   0 runner    (1001) docker     (123)    15170 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_blvt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_bswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_c2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_data_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_fiat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_gift_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_loan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33152 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_margin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9698 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_market.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_mining.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_nft.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_pay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_portfolio_margin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_rebate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_savings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_staking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30191 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_sub_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14542 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16702 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:06:01.642999 binance-connector-3.2.0/binance/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/websocket/binance_socket_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:06:01.642999 binance-connector-3.2.0/binance/websocket/spot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/websocket/spot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:06:01.646999 binance-connector-3.2.0/binance/websocket/spot/websocket_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/websocket/spot/websocket_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14057 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/websocket/spot/websocket_api/_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24597 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/websocket/spot/websocket_api/_market.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38486 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/websocket/spot/websocket_api/_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/websocket/spot/websocket_api/_user_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/websocket/spot/websocket_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/websocket/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:06:01.646999 binance-connector-3.2.0/binance_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-08-01 02:06:01.000000 binance-connector-3.2.0/binance_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-08-01 02:06:01.000000 binance-connector-3.2.0/binance_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 02:06:01.000000 binance-connector-3.2.0/binance_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-01 02:06:01.000000 binance-connector-3.2.0/binance_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 02:06:01.000000 binance-connector-3.2.0/binance_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:06:01.646999 binance-connector-3.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:05:58.000000 binance-connector-3.2.0/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:06:01.646999 binance-connector-3.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 02:05:58.000000 binance-connector-3.2.0/requirements/common.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-08-01 02:06:01.646999 binance-connector-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-01 02:05:58.000000 binance-connector-3.2.0/setup.py
```

### Comparing `binance-connector-3.1.1/LICENSE.md` & `binance-connector-3.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `binance-connector-3.1.1/PKG-INFO` & `binance-connector-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binance-connector
-Version: 3.1.1
+Version: 3.2.0
 Summary: This is a lightweight library that works as a connector to Binance public API.
 Home-page: https://github.com/binance/binance-connector-python
 License: MIT
 Keywords: Binance,Public API
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `binance-connector-3.1.1/README.md` & `binance-connector-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `binance-connector-3.1.1/binance/api.py` & `binance-connector-3.2.0/binance/api.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.1.1/binance/error.py` & `binance-connector-3.2.0/binance/error.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.1.1/binance/lib/authentication.py` & `binance-connector-3.2.0/binance/lib/authentication.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.1.1/binance/lib/enums.py` & `binance-connector-3.2.0/binance/lib/enums.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.1.1/binance/lib/utils.py` & `binance-connector-3.2.0/binance/lib/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 def check_enum_parameter(value, enum_class):
     if value not in set(item.value for item in enum_class):
         raise ParameterValueError([value])
 
 
 def check_type_parameter(value, name, data_type):
-    if value is not None and type(value) != data_type:
+    if value is not None and not isinstance(value, data_type):
         raise ParameterTypeError([name, data_type])
 
 
 def get_timestamp():
     return int(time.time() * 1000)
```

### Comparing `binance-connector-3.1.1/binance/spot/__init__.py` & `binance-connector-3.2.0/binance/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.1.1/binance/spot/_blvt.py` & `binance-connector-3.2.0/binance/spot/_blvt.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.1.1/binance/spot/_bswap.py` & `binance-connector-3.2.0/binance/spot/_bswap.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.1.1/binance/spot/_c2c.py` & `binance-connector-3.2.0/binance/spot/_c2c.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.1.1/binance/spot/_convert.py` & `binance-connector-3.2.0/binance/spot/_convert.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.1.1/binance/spot/_data_stream.py` & `binance-connector-3.2.0/binance/spot/_data_stream.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.1.1/binance/spot/_fiat.py` & `binance-connector-3.2.0/binance/spot/_fiat.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.1.1/binance/spot/_futures.py` & `binance-connector-3.2.0/binance/spot/_futures.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.1.1/binance/spot/_gift_card.py` & `binance-connector-3.2.0/binance/spot/_gift_card.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.1.1/binance/spot/_loan.py` & `binance-connector-3.2.0/binance/spot/_loan.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.1.1/binance/spot/_margin.py` & `binance-connector-3.2.0/binance/spot/_margin.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.1.1/binance/spot/_market.py` & `binance-connector-3.2.0/binance/spot/_market.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         symbol (str): the trading pair
     Keyword Args:
         limit (int, optional): limit the results. Default 500; max 1000.
         formId (int, optional): trade id to fetch from. Default gets most recent trades.
     """
     check_required_parameter(symbol, "symbol")
     params = {"symbol": symbol, **kwargs}
-    return self.limit_request("GET", "/api/v3/historicalTrades", params)
+    return self.query("/api/v3/historicalTrades", params)
 
 
 def agg_trades(self, symbol: str, **kwargs):
     """Compressed/Aggregate Trades List
 
     GET /api/v3/aggTrades
```

### Comparing `binance-connector-3.1.1/binance/spot/_mining.py` & `binance-connector-3.2.0/binance/spot/_mining.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.1.1/binance/spot/_nft.py` & `binance-connector-3.2.0/binance/spot/_nft.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.1.1/binance/spot/_portfolio_margin.py` & `binance-connector-3.2.0/binance/spot/_portfolio_margin.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.1.1/binance/spot/_savings.py` & `binance-connector-3.2.0/binance/spot/_savings.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.1.1/binance/spot/_staking.py` & `binance-connector-3.2.0/binance/spot/_staking.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.1.1/binance/spot/_sub_account.py` & `binance-connector-3.2.0/binance/spot/_sub_account.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.1.1/binance/spot/_trade.py` & `binance-connector-3.2.0/binance/spot/_trade.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.1.1/binance/spot/_wallet.py` & `binance-connector-3.2.0/binance/spot/_wallet.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.1.1/binance/websocket/binance_socket_manager.py` & `binance-connector-3.2.0/binance/websocket/binance_socket_manager.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.1.1/binance/websocket/spot/websocket_api/__init__.py` & `binance-connector-3.2.0/binance/websocket/spot/websocket_api/__init__.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.1.1/binance/websocket/spot/websocket_api/_account.py` & `binance-connector-3.2.0/binance/websocket/spot/websocket_api/_account.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.1.1/binance/websocket/spot/websocket_api/_market.py` & `binance-connector-3.2.0/binance/websocket/spot/websocket_api/_market.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.1.1/binance/websocket/spot/websocket_api/_trade.py` & `binance-connector-3.2.0/binance/websocket/spot/websocket_api/_trade.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.1.1/binance/websocket/spot/websocket_api/_user_data.py` & `binance-connector-3.2.0/binance/websocket/spot/websocket_api/_user_data.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.1.1/binance/websocket/spot/websocket_stream.py` & `binance-connector-3.2.0/binance/websocket/spot/websocket_stream.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.1.1/binance/websocket/websocket_client.py` & `binance-connector-3.2.0/binance/websocket/websocket_client.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.1.1/binance_connector.egg-info/PKG-INFO` & `binance-connector-3.2.0/binance_connector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binance-connector
-Version: 3.1.1
+Version: 3.2.0
 Summary: This is a lightweight library that works as a connector to Binance public API.
 Home-page: https://github.com/binance/binance-connector-python
 License: MIT
 Keywords: Binance,Public API
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `binance-connector-3.1.1/binance_connector.egg-info/SOURCES.txt` & `binance-connector-3.2.0/binance_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `binance-connector-3.1.1/setup.py` & `binance-connector-3.2.0/setup.py`

 * *Files identical despite different names*

